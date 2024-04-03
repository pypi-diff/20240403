# Comparing `tmp/metabeaver-0.3.4.tar.gz` & `tmp/metabeaver-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metabeaver-0.3.4.tar", last modified: Tue Apr  2 18:00:26 2024, max compression
+gzip compressed data, was "metabeaver-0.3.5.tar", last modified: Tue Apr  2 19:59:14 2024, max compression
```

## Comparing `metabeaver-0.3.4.tar` & `metabeaver-0.3.5.tar`

### file list

```diff
@@ -1,130 +1,130 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 18:00:26.546290 metabeaver-0.3.4/
--rw-rw-rw-   0        0        0      682 2024-04-02 18:00:26.541225 metabeaver-0.3.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-02 18:00:25.511592 metabeaver-0.3.4/metabeaver/
-drwxrwxrwx   0        0        0        0 2024-04-02 18:00:25.652660 metabeaver-0.3.4/metabeaver/BeaverTown/
--rw-rw-rw-   0        0        0       54 2024-02-20 17:36:10.000000 metabeaver-0.3.4/metabeaver/BeaverTown/__init__.py
--rw-rw-rw-   0        0        0      523 2024-02-20 17:54:11.000000 metabeaver-0.3.4/metabeaver/BeaverTown/abstractBeaver.py
--rw-rw-rw-   0        0        0      928 2023-11-01 11:25:56.000000 metabeaver-0.3.4/metabeaver/BeaverTown/beaverOn.py
--rw-rw-rw-   0        0        0       54 2023-11-28 08:40:24.000000 metabeaver-0.3.4/metabeaver/BeaverTown/pumpkinPie.py
-drwxrwxrwx   0        0        0        0 2024-04-02 18:00:25.686280 metabeaver-0.3.4/metabeaver/Binary/
--rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.4/metabeaver/Binary/__init__.py
--rw-rw-rw-   0        0        0     3173 2024-02-10 12:14:12.000000 metabeaver-0.3.4/metabeaver/Binary/binaryOperations.py
-drwxrwxrwx   0        0        0        0 2024-04-02 18:00:25.706436 metabeaver-0.3.4/metabeaver/Caching/
--rw-rw-rw-   0        0        0     2084 2023-10-15 13:36:19.000000 metabeaver-0.3.4/metabeaver/Caching/LeastRecentlyUsed.py
--rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.4/metabeaver/Caching/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 18:00:25.744642 metabeaver-0.3.4/metabeaver/DataManipulation/
--rw-rw-rw-   0        0        0        0 2023-09-01 14:45:09.000000 metabeaver-0.3.4/metabeaver/DataManipulation/__init__.py
--rw-rw-rw-   0        0        0      859 2023-05-22 12:30:24.000000 metabeaver-0.3.4/metabeaver/DataManipulation/localPickle.py
--rw-rw-rw-   0        0        0      831 2023-05-15 09:25:04.000000 metabeaver-0.3.4/metabeaver/DataManipulation/universalResourceLinkHandler.py
-drwxrwxrwx   0        0        0        0 2024-04-02 18:00:25.806367 metabeaver-0.3.4/metabeaver/DataStructures/
--rw-rw-rw-   0        0        0     3440 2023-12-30 09:15:13.000000 metabeaver-0.3.4/metabeaver/DataStructures/BinarySearchTree.py
--rw-rw-rw-   0        0        0      182 2023-12-28 08:32:20.000000 metabeaver-0.3.4/metabeaver/DataStructures/Node.py
--rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.4/metabeaver/DataStructures/__init__.py
--rw-rw-rw-   0        0        0      400 2023-09-27 14:26:46.000000 metabeaver-0.3.4/metabeaver/DataStructures/firstInFirstOutQueue.py
--rw-rw-rw-   0        0        0        0 2023-10-16 07:07:41.000000 metabeaver-0.3.4/metabeaver/DataStructures/firstInLastOut.py
--rw-rw-rw-   0        0        0        0 2023-10-16 07:07:21.000000 metabeaver-0.3.4/metabeaver/DataStructures/linkedList.py
-drwxrwxrwx   0        0        0        0 2024-04-02 18:00:25.811439 metabeaver-0.3.4/metabeaver/DatabaseFunctionality/
-drwxrwxrwx   0        0        0        0 2024-04-02 18:00:25.816455 metabeaver-0.3.4/metabeaver/DatabaseFunctionality/SQL/
--rw-rw-rw-   0        0        0       54 2023-12-20 14:54:31.000000 metabeaver-0.3.4/metabeaver/DatabaseFunctionality/SQL/__init__.py
--rw-rw-rw-   0        0        0     1051 2024-03-08 12:25:31.000000 metabeaver-0.3.4/metabeaver/DatabaseFunctionality/SQL/rawSQL.py
-drwxrwxrwx   0        0        0        0 2024-04-02 18:00:25.931668 metabeaver-0.3.4/metabeaver/DatabaseFunctionality/SQLite/
--rw-rw-rw-   0        0        0    32341 2023-12-21 09:23:48.000000 metabeaver-0.3.4/metabeaver/DatabaseFunctionality/SQLite/SQLiteDatabase.py
--rw-rw-rw-   0        0        0       54 2023-12-20 14:54:31.000000 metabeaver-0.3.4/metabeaver/DatabaseFunctionality/SQLite/__init__.py
--rw-rw-rw-   0        0        0     1803 2023-11-28 08:53:13.000000 metabeaver-0.3.4/metabeaver/DatabaseFunctionality/SQLite/commonCreateUpdate.py
--rw-rw-rw-   0        0        0     1854 2023-11-28 11:03:59.000000 metabeaver-0.3.4/metabeaver/DatabaseFunctionality/SQLite/inspectTable.py
--rw-rw-rw-   0        0        0       54 2023-12-20 14:54:15.000000 metabeaver-0.3.4/metabeaver/DatabaseFunctionality/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 18:00:25.951332 metabeaver-0.3.4/metabeaver/DatesAndTime/
--rw-rw-rw-   0        0        0        0 2023-09-01 14:45:09.000000 metabeaver-0.3.4/metabeaver/DatesAndTime/__init__.py
--rw-rw-rw-   0        0        0      692 2024-03-06 21:17:29.000000 metabeaver-0.3.4/metabeaver/DatesAndTime/getToday.py
-drwxrwxrwx   0        0        0        0 2024-04-02 18:00:25.951332 metabeaver-0.3.4/metabeaver/Dynamic Programming/
--rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.4/metabeaver/Dynamic Programming/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 18:00:25.971384 metabeaver-0.3.4/metabeaver/FileIO/
--rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.4/metabeaver/FileIO/__init__.py
--rw-rw-rw-   0        0        0      966 2024-03-02 22:41:17.000000 metabeaver-0.3.4/metabeaver/FileIO/yamlIO.py
-drwxrwxrwx   0        0        0        0 2024-04-02 18:00:26.006521 metabeaver-0.3.4/metabeaver/Formatting/
--rw-rw-rw-   0        0        0        0 2023-09-01 14:45:09.000000 metabeaver-0.3.4/metabeaver/Formatting/__init__.py
--rw-rw-rw-   0        0        0      450 2023-09-02 17:13:50.000000 metabeaver-0.3.4/metabeaver/Formatting/printControl.py
--rw-rw-rw-   0        0        0     1063 2023-10-04 07:18:25.000000 metabeaver-0.3.4/metabeaver/Formatting/printControlTest.py
-drwxrwxrwx   0        0        0        0 2024-04-02 18:00:26.011999 metabeaver-0.3.4/metabeaver/GoogleCloudPlatform/
-drwxrwxrwx   0        0        0        0 2024-04-02 18:00:26.071366 metabeaver-0.3.4/metabeaver/GoogleCloudPlatform/BigQuery/
--rw-rw-rw-   0        0        0     5076 2024-01-05 18:52:24.000000 metabeaver-0.3.4/metabeaver/GoogleCloudPlatform/BigQuery/TableManagement.py
--rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.3.4/metabeaver/GoogleCloudPlatform/BigQuery/__init__.py
--rw-rw-rw-   0        0        0      718 2024-01-05 19:16:53.000000 metabeaver-0.3.4/metabeaver/GoogleCloudPlatform/BigQuery/clientFromCredentials.py
--rw-rw-rw-   0        0        0      144 2024-01-05 19:00:29.000000 metabeaver-0.3.4/metabeaver/GoogleCloudPlatform/BigQuery/credentialsFromEnv.py
--rw-rw-rw-   0        0        0     3611 2024-04-02 16:17:47.000000 metabeaver-0.3.4/metabeaver/GoogleCloudPlatform/BigQuery/getTableData.py
--rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.3.4/metabeaver/GoogleCloudPlatform/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 18:00:26.101523 metabeaver-0.3.4/metabeaver/Graph Algorithms/
--rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.4/metabeaver/Graph Algorithms/__init__.py
--rw-rw-rw-   0        0        0        0 2023-10-11 14:48:31.000000 metabeaver-0.3.4/metabeaver/Graph Algorithms/bellmanFord.py
--rw-rw-rw-   0        0        0        0 2023-10-11 14:43:10.000000 metabeaver-0.3.4/metabeaver/Graph Algorithms/breadthFirstSearch.py
--rw-rw-rw-   0        0        0      990 2024-02-13 10:13:17.000000 metabeaver-0.3.4/metabeaver/Graph Algorithms/depthFirstSearch.py
--rw-rw-rw-   0        0        0        0 2023-10-11 14:48:06.000000 metabeaver-0.3.4/metabeaver/Graph Algorithms/dijkstra.py
--rw-rw-rw-   0        0        0        0 2023-10-11 14:43:34.000000 metabeaver-0.3.4/metabeaver/Graph Algorithms/monteCarloTreeSearch.py
-drwxrwxrwx   0        0        0        0 2024-04-02 18:00:26.121413 metabeaver-0.3.4/metabeaver/Graphing/
--rw-rw-rw-   0        0        0        0 2023-09-01 14:45:09.000000 metabeaver-0.3.4/metabeaver/Graphing/__init__.py
--rw-rw-rw-   0        0        0      824 2023-05-26 14:44:50.000000 metabeaver-0.3.4/metabeaver/Graphing/markdownGenerator.py
-drwxrwxrwx   0        0        0        0 2024-04-02 18:00:26.146376 metabeaver-0.3.4/metabeaver/InstallationScripts/
--rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.3.4/metabeaver/InstallationScripts/__init__.py
--rw-rw-rw-   0        0        0     1246 2023-04-07 12:06:41.000000 metabeaver-0.3.4/metabeaver/InstallationScripts/autoGenerateRequirementsText.py
-drwxrwxrwx   0        0        0        0 2024-04-02 18:00:26.146376 metabeaver-0.3.4/metabeaver/InterviewQuestions/
-drwxrwxrwx   0        0        0        0 2024-04-02 18:00:26.206488 metabeaver-0.3.4/metabeaver/InterviewQuestions/Arrays/
--rw-rw-rw-   0        0        0       54 2024-03-06 21:33:39.000000 metabeaver-0.3.4/metabeaver/InterviewQuestions/Arrays/__init__.py
--rw-rw-rw-   0        0        0     1100 2024-01-16 09:07:23.000000 metabeaver-0.3.4/metabeaver/InterviewQuestions/Arrays/bestTimeSellStock.py
--rw-rw-rw-   0        0        0     2374 2024-02-12 11:00:27.000000 metabeaver-0.3.4/metabeaver/InterviewQuestions/Arrays/removeThirdDuplicate.py
--rw-rw-rw-   0        0        0     3115 2024-01-10 09:29:29.000000 metabeaver-0.3.4/metabeaver/InterviewQuestions/Arrays/twoSum.py
-drwxrwxrwx   0        0        0        0 2024-04-02 18:00:26.226600 metabeaver-0.3.4/metabeaver/InterviewQuestions/Stacks/
--rw-rw-rw-   0        0        0       54 2024-03-06 21:34:35.000000 metabeaver-0.3.4/metabeaver/InterviewQuestions/Stacks/__init__.py
--rw-rw-rw-   0        0        0     1043 2023-10-24 15:28:24.000000 metabeaver-0.3.4/metabeaver/InterviewQuestions/Stacks/calculateFromSymbols.py
--rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.4/metabeaver/InterviewQuestions/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 18:00:26.236675 metabeaver-0.3.4/metabeaver/LearnPython/
-drwxrwxrwx   0        0        0        0 2024-04-02 18:00:26.251363 metabeaver-0.3.4/metabeaver/LearnPython/ControlFlow/
--rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.4/metabeaver/LearnPython/ControlFlow/__init__.py
--rw-rw-rw-   0        0        0     2615 2024-03-01 09:39:54.000000 metabeaver-0.3.4/metabeaver/LearnPython/ControlFlow/ifelifelse.py
--rw-rw-rw-   0        0        0       54 2024-02-20 17:10:29.000000 metabeaver-0.3.4/metabeaver/LearnPython/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 18:00:26.274843 metabeaver-0.3.4/metabeaver/Machine Learning/
-drwxrwxrwx   0        0        0        0 2024-04-02 18:00:26.286411 metabeaver-0.3.4/metabeaver/Machine Learning/LLM/
--rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.4/metabeaver/Machine Learning/LLM/__init__.py
--rw-rw-rw-   0        0        0       54 2024-03-28 19:26:50.000000 metabeaver-0.3.4/metabeaver/Machine Learning/LLM/loadWithLlamaCPP.py
--rw-rw-rw-   0        0        0     1996 2024-04-02 16:08:53.000000 metabeaver-0.3.4/metabeaver/Machine Learning/LLM/loadWithTransformers.py
--rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.4/metabeaver/Machine Learning/__init__.py
--rw-rw-rw-   0        0        0     2915 2024-02-18 11:36:59.000000 metabeaver-0.3.4/metabeaver/Machine Learning/lassoRegression.py
-drwxrwxrwx   0        0        0        0 2024-04-02 18:00:26.312440 metabeaver-0.3.4/metabeaver/Mathematical Operations/
--rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.4/metabeaver/Mathematical Operations/__init__.py
--rw-rw-rw-   0        0        0        0 2023-10-16 16:20:54.000000 metabeaver-0.3.4/metabeaver/Mathematical Operations/greatestCommonDenominator.py
--rw-rw-rw-   0        0        0     1072 2024-03-01 15:21:44.000000 metabeaver-0.3.4/metabeaver/Mathematical Operations/vectorDotProduct.py
-drwxrwxrwx   0        0        0        0 2024-04-02 18:00:26.312440 metabeaver-0.3.4/metabeaver/MetaProgramming/
--rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.3.4/metabeaver/MetaProgramming/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 18:00:26.312440 metabeaver-0.3.4/metabeaver/OperationBeaver/
--rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.3.4/metabeaver/OperationBeaver/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 18:00:26.343339 metabeaver-0.3.4/metabeaver/Search Algorithms/
--rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.4/metabeaver/Search Algorithms/__init__.py
--rw-rw-rw-   0        0        0     2686 2023-11-01 10:30:45.000000 metabeaver-0.3.4/metabeaver/Search Algorithms/binarySearch.py
-drwxrwxrwx   0        0        0        0 2024-04-02 18:00:26.361467 metabeaver-0.3.4/metabeaver/Set Theory/
--rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.4/metabeaver/Set Theory/__init__.py
--rw-rw-rw-   0        0        0     5497 2023-10-06 17:16:32.000000 metabeaver-0.3.4/metabeaver/Set Theory/findAllSubsets.py
-drwxrwxrwx   0        0        0        0 2024-04-02 18:00:26.454620 metabeaver-0.3.4/metabeaver/Sorting Algorithms/
--rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.4/metabeaver/Sorting Algorithms/__init__.py
--rw-rw-rw-   0        0        0     3080 2023-12-12 09:32:50.000000 metabeaver-0.3.4/metabeaver/Sorting Algorithms/heapSort.py
--rw-rw-rw-   0        0        0     1539 2023-10-15 18:11:43.000000 metabeaver-0.3.4/metabeaver/Sorting Algorithms/insertionSort.py
--rw-rw-rw-   0        0        0     1275 2024-01-09 08:35:40.000000 metabeaver-0.3.4/metabeaver/Sorting Algorithms/mergeSort.py
--rw-rw-rw-   0        0        0     1136 2023-10-13 07:08:11.000000 metabeaver-0.3.4/metabeaver/Sorting Algorithms/quickSort.py
--rw-rw-rw-   0        0        0     3213 2023-10-12 10:18:23.000000 metabeaver-0.3.4/metabeaver/Sorting Algorithms/timsort.py
-drwxrwxrwx   0        0        0        0 2024-04-02 18:00:26.475302 metabeaver-0.3.4/metabeaver/Testing/
--rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.3.4/metabeaver/Testing/__init__.py
--rw-rw-rw-   0        0        0     3544 2023-11-03 10:47:27.000000 metabeaver-0.3.4/metabeaver/Testing/scratchPad.py
-drwxrwxrwx   0        0        0        0 2024-04-02 18:00:26.511417 metabeaver-0.3.4/metabeaver/TextValidation/
--rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.4/metabeaver/TextValidation/__init__.py
--rw-rw-rw-   0        0        0     1418 2023-09-27 14:33:38.000000 metabeaver-0.3.4/metabeaver/TextValidation/closureChecker.py
--rw-rw-rw-   0        0        0     4004 2023-11-01 10:50:46.000000 metabeaver-0.3.4/metabeaver/TextValidation/establishLargestPalindrome.py
-drwxrwxrwx   0        0        0        0 2024-04-02 18:00:26.534210 metabeaver-0.3.4/metabeaver/WebScraping/
--rw-rw-rw-   0        0        0       54 2023-11-28 09:31:41.000000 metabeaver-0.3.4/metabeaver/WebScraping/__init__.py
--rw-rw-rw-   0        0        0     1322 2023-11-28 09:40:35.000000 metabeaver-0.3.4/metabeaver/WebScraping/simpleRequests.py
--rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.3.4/metabeaver/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 18:00:26.541225 metabeaver-0.3.4/metabeaver.egg-info/
--rw-rw-rw-   0        0        0      682 2024-04-02 18:00:25.000000 metabeaver-0.3.4/metabeaver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4000 2024-04-02 18:00:25.000000 metabeaver-0.3.4/metabeaver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 18:00:25.000000 metabeaver-0.3.4/metabeaver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2024-04-02 18:00:25.000000 metabeaver-0.3.4/metabeaver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-02 18:00:25.000000 metabeaver-0.3.4/metabeaver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-02 18:00:26.546290 metabeaver-0.3.4/setup.cfg
--rw-rw-rw-   0        0        0     1253 2024-04-02 17:44:36.000000 metabeaver-0.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 19:59:14.226143 metabeaver-0.3.5/
+-rw-rw-rw-   0        0        0      339 2024-04-02 19:59:14.226143 metabeaver-0.3.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-02 19:59:14.086392 metabeaver-0.3.5/metabeaver/
+drwxrwxrwx   0        0        0        0 2024-04-02 19:59:14.112516 metabeaver-0.3.5/metabeaver/BeaverTown/
+-rw-rw-rw-   0        0        0       54 2024-02-20 17:36:10.000000 metabeaver-0.3.5/metabeaver/BeaverTown/__init__.py
+-rw-rw-rw-   0        0        0      523 2024-02-20 17:54:11.000000 metabeaver-0.3.5/metabeaver/BeaverTown/abstractBeaver.py
+-rw-rw-rw-   0        0        0      928 2023-11-01 11:25:56.000000 metabeaver-0.3.5/metabeaver/BeaverTown/beaverOn.py
+-rw-rw-rw-   0        0        0       54 2023-11-28 08:40:24.000000 metabeaver-0.3.5/metabeaver/BeaverTown/pumpkinPie.py
+drwxrwxrwx   0        0        0        0 2024-04-02 19:59:14.112516 metabeaver-0.3.5/metabeaver/Binary/
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.5/metabeaver/Binary/__init__.py
+-rw-rw-rw-   0        0        0     3173 2024-02-10 12:14:12.000000 metabeaver-0.3.5/metabeaver/Binary/binaryOperations.py
+drwxrwxrwx   0        0        0        0 2024-04-02 19:59:14.116073 metabeaver-0.3.5/metabeaver/Caching/
+-rw-rw-rw-   0        0        0     2084 2023-10-15 13:36:19.000000 metabeaver-0.3.5/metabeaver/Caching/LeastRecentlyUsed.py
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.5/metabeaver/Caching/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 19:59:14.116073 metabeaver-0.3.5/metabeaver/DataManipulation/
+-rw-rw-rw-   0        0        0        0 2023-09-01 14:45:09.000000 metabeaver-0.3.5/metabeaver/DataManipulation/__init__.py
+-rw-rw-rw-   0        0        0      859 2023-05-22 12:30:24.000000 metabeaver-0.3.5/metabeaver/DataManipulation/localPickle.py
+-rw-rw-rw-   0        0        0      831 2023-05-15 09:25:04.000000 metabeaver-0.3.5/metabeaver/DataManipulation/universalResourceLinkHandler.py
+drwxrwxrwx   0        0        0        0 2024-04-02 19:59:14.127322 metabeaver-0.3.5/metabeaver/DataStructures/
+-rw-rw-rw-   0        0        0     3440 2023-12-30 09:15:13.000000 metabeaver-0.3.5/metabeaver/DataStructures/BinarySearchTree.py
+-rw-rw-rw-   0        0        0      182 2023-12-28 08:32:20.000000 metabeaver-0.3.5/metabeaver/DataStructures/Node.py
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.5/metabeaver/DataStructures/__init__.py
+-rw-rw-rw-   0        0        0      400 2023-09-27 14:26:46.000000 metabeaver-0.3.5/metabeaver/DataStructures/firstInFirstOutQueue.py
+-rw-rw-rw-   0        0        0        0 2023-10-16 07:07:41.000000 metabeaver-0.3.5/metabeaver/DataStructures/firstInLastOut.py
+-rw-rw-rw-   0        0        0        0 2023-10-16 07:07:21.000000 metabeaver-0.3.5/metabeaver/DataStructures/linkedList.py
+drwxrwxrwx   0        0        0        0 2024-04-02 19:59:14.127322 metabeaver-0.3.5/metabeaver/DatabaseFunctionality/
+drwxrwxrwx   0        0        0        0 2024-04-02 19:59:14.127322 metabeaver-0.3.5/metabeaver/DatabaseFunctionality/SQL/
+-rw-rw-rw-   0        0        0       54 2023-12-20 14:54:31.000000 metabeaver-0.3.5/metabeaver/DatabaseFunctionality/SQL/__init__.py
+-rw-rw-rw-   0        0        0     1051 2024-03-08 12:25:31.000000 metabeaver-0.3.5/metabeaver/DatabaseFunctionality/SQL/rawSQL.py
+drwxrwxrwx   0        0        0        0 2024-04-02 19:59:14.136353 metabeaver-0.3.5/metabeaver/DatabaseFunctionality/SQLite/
+-rw-rw-rw-   0        0        0    32341 2023-12-21 09:23:48.000000 metabeaver-0.3.5/metabeaver/DatabaseFunctionality/SQLite/SQLiteDatabase.py
+-rw-rw-rw-   0        0        0       54 2023-12-20 14:54:31.000000 metabeaver-0.3.5/metabeaver/DatabaseFunctionality/SQLite/__init__.py
+-rw-rw-rw-   0        0        0     1803 2023-11-28 08:53:13.000000 metabeaver-0.3.5/metabeaver/DatabaseFunctionality/SQLite/commonCreateUpdate.py
+-rw-rw-rw-   0        0        0     1854 2023-11-28 11:03:59.000000 metabeaver-0.3.5/metabeaver/DatabaseFunctionality/SQLite/inspectTable.py
+-rw-rw-rw-   0        0        0       54 2023-12-20 14:54:15.000000 metabeaver-0.3.5/metabeaver/DatabaseFunctionality/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 19:59:14.136353 metabeaver-0.3.5/metabeaver/DatesAndTime/
+-rw-rw-rw-   0        0        0        0 2023-09-01 14:45:09.000000 metabeaver-0.3.5/metabeaver/DatesAndTime/__init__.py
+-rw-rw-rw-   0        0        0      692 2024-03-06 21:17:29.000000 metabeaver-0.3.5/metabeaver/DatesAndTime/getToday.py
+drwxrwxrwx   0        0        0        0 2024-04-02 19:59:14.136353 metabeaver-0.3.5/metabeaver/Dynamic Programming/
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.5/metabeaver/Dynamic Programming/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 19:59:14.143402 metabeaver-0.3.5/metabeaver/FileIO/
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.5/metabeaver/FileIO/__init__.py
+-rw-rw-rw-   0        0        0      966 2024-03-02 22:41:17.000000 metabeaver-0.3.5/metabeaver/FileIO/yamlIO.py
+drwxrwxrwx   0        0        0        0 2024-04-02 19:59:14.146410 metabeaver-0.3.5/metabeaver/Formatting/
+-rw-rw-rw-   0        0        0        0 2023-09-01 14:45:09.000000 metabeaver-0.3.5/metabeaver/Formatting/__init__.py
+-rw-rw-rw-   0        0        0      450 2023-09-02 17:13:50.000000 metabeaver-0.3.5/metabeaver/Formatting/printControl.py
+-rw-rw-rw-   0        0        0     1063 2023-10-04 07:18:25.000000 metabeaver-0.3.5/metabeaver/Formatting/printControlTest.py
+drwxrwxrwx   0        0        0        0 2024-04-02 19:59:14.146410 metabeaver-0.3.5/metabeaver/GoogleCloudPlatform/
+drwxrwxrwx   0        0        0        0 2024-04-02 19:59:14.156536 metabeaver-0.3.5/metabeaver/GoogleCloudPlatform/BigQuery/
+-rw-rw-rw-   0        0        0     5076 2024-01-05 18:52:24.000000 metabeaver-0.3.5/metabeaver/GoogleCloudPlatform/BigQuery/TableManagement.py
+-rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.3.5/metabeaver/GoogleCloudPlatform/BigQuery/__init__.py
+-rw-rw-rw-   0        0        0      718 2024-01-05 19:16:53.000000 metabeaver-0.3.5/metabeaver/GoogleCloudPlatform/BigQuery/clientFromCredentials.py
+-rw-rw-rw-   0        0        0      144 2024-01-05 19:00:29.000000 metabeaver-0.3.5/metabeaver/GoogleCloudPlatform/BigQuery/credentialsFromEnv.py
+-rw-rw-rw-   0        0        0     4849 2024-04-02 19:13:41.000000 metabeaver-0.3.5/metabeaver/GoogleCloudPlatform/BigQuery/getTableData.py
+-rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.3.5/metabeaver/GoogleCloudPlatform/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 19:59:14.166067 metabeaver-0.3.5/metabeaver/Graph Algorithms/
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.5/metabeaver/Graph Algorithms/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-10-11 14:48:31.000000 metabeaver-0.3.5/metabeaver/Graph Algorithms/bellmanFord.py
+-rw-rw-rw-   0        0        0        0 2023-10-11 14:43:10.000000 metabeaver-0.3.5/metabeaver/Graph Algorithms/breadthFirstSearch.py
+-rw-rw-rw-   0        0        0      990 2024-02-13 10:13:17.000000 metabeaver-0.3.5/metabeaver/Graph Algorithms/depthFirstSearch.py
+-rw-rw-rw-   0        0        0        0 2023-10-11 14:48:06.000000 metabeaver-0.3.5/metabeaver/Graph Algorithms/dijkstra.py
+-rw-rw-rw-   0        0        0        0 2023-10-11 14:43:34.000000 metabeaver-0.3.5/metabeaver/Graph Algorithms/monteCarloTreeSearch.py
+drwxrwxrwx   0        0        0        0 2024-04-02 19:59:14.166067 metabeaver-0.3.5/metabeaver/Graphing/
+-rw-rw-rw-   0        0        0        0 2023-09-01 14:45:09.000000 metabeaver-0.3.5/metabeaver/Graphing/__init__.py
+-rw-rw-rw-   0        0        0      824 2023-05-26 14:44:50.000000 metabeaver-0.3.5/metabeaver/Graphing/markdownGenerator.py
+drwxrwxrwx   0        0        0        0 2024-04-02 19:59:14.166067 metabeaver-0.3.5/metabeaver/InstallationScripts/
+-rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.3.5/metabeaver/InstallationScripts/__init__.py
+-rw-rw-rw-   0        0        0     1246 2023-04-07 12:06:41.000000 metabeaver-0.3.5/metabeaver/InstallationScripts/autoGenerateRequirementsText.py
+drwxrwxrwx   0        0        0        0 2024-04-02 19:59:14.166067 metabeaver-0.3.5/metabeaver/InterviewQuestions/
+drwxrwxrwx   0        0        0        0 2024-04-02 19:59:14.176109 metabeaver-0.3.5/metabeaver/InterviewQuestions/Arrays/
+-rw-rw-rw-   0        0        0       54 2024-03-06 21:33:39.000000 metabeaver-0.3.5/metabeaver/InterviewQuestions/Arrays/__init__.py
+-rw-rw-rw-   0        0        0     1100 2024-01-16 09:07:23.000000 metabeaver-0.3.5/metabeaver/InterviewQuestions/Arrays/bestTimeSellStock.py
+-rw-rw-rw-   0        0        0     2374 2024-02-12 11:00:27.000000 metabeaver-0.3.5/metabeaver/InterviewQuestions/Arrays/removeThirdDuplicate.py
+-rw-rw-rw-   0        0        0     3115 2024-01-10 09:29:29.000000 metabeaver-0.3.5/metabeaver/InterviewQuestions/Arrays/twoSum.py
+drwxrwxrwx   0        0        0        0 2024-04-02 19:59:14.176109 metabeaver-0.3.5/metabeaver/InterviewQuestions/Stacks/
+-rw-rw-rw-   0        0        0       54 2024-03-06 21:34:35.000000 metabeaver-0.3.5/metabeaver/InterviewQuestions/Stacks/__init__.py
+-rw-rw-rw-   0        0        0     1043 2023-10-24 15:28:24.000000 metabeaver-0.3.5/metabeaver/InterviewQuestions/Stacks/calculateFromSymbols.py
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.5/metabeaver/InterviewQuestions/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 19:59:14.176109 metabeaver-0.3.5/metabeaver/LearnPython/
+drwxrwxrwx   0        0        0        0 2024-04-02 19:59:14.186118 metabeaver-0.3.5/metabeaver/LearnPython/ControlFlow/
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.5/metabeaver/LearnPython/ControlFlow/__init__.py
+-rw-rw-rw-   0        0        0     2615 2024-03-01 09:39:54.000000 metabeaver-0.3.5/metabeaver/LearnPython/ControlFlow/ifelifelse.py
+-rw-rw-rw-   0        0        0       54 2024-02-20 17:10:29.000000 metabeaver-0.3.5/metabeaver/LearnPython/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 19:59:14.186118 metabeaver-0.3.5/metabeaver/Machine Learning/
+drwxrwxrwx   0        0        0        0 2024-04-02 19:59:14.191145 metabeaver-0.3.5/metabeaver/Machine Learning/LLM/
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.5/metabeaver/Machine Learning/LLM/__init__.py
+-rw-rw-rw-   0        0        0       54 2024-03-28 19:26:50.000000 metabeaver-0.3.5/metabeaver/Machine Learning/LLM/loadWithLlamaCPP.py
+-rw-rw-rw-   0        0        0     1996 2024-04-02 16:08:53.000000 metabeaver-0.3.5/metabeaver/Machine Learning/LLM/loadWithTransformers.py
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.5/metabeaver/Machine Learning/__init__.py
+-rw-rw-rw-   0        0        0     2915 2024-02-18 11:36:59.000000 metabeaver-0.3.5/metabeaver/Machine Learning/lassoRegression.py
+drwxrwxrwx   0        0        0        0 2024-04-02 19:59:14.196152 metabeaver-0.3.5/metabeaver/Mathematical Operations/
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.5/metabeaver/Mathematical Operations/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-10-16 16:20:54.000000 metabeaver-0.3.5/metabeaver/Mathematical Operations/greatestCommonDenominator.py
+-rw-rw-rw-   0        0        0     1072 2024-03-01 15:21:44.000000 metabeaver-0.3.5/metabeaver/Mathematical Operations/vectorDotProduct.py
+drwxrwxrwx   0        0        0        0 2024-04-02 19:59:14.196152 metabeaver-0.3.5/metabeaver/MetaProgramming/
+-rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.3.5/metabeaver/MetaProgramming/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 19:59:14.196152 metabeaver-0.3.5/metabeaver/OperationBeaver/
+-rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.3.5/metabeaver/OperationBeaver/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 19:59:14.196152 metabeaver-0.3.5/metabeaver/Search Algorithms/
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.5/metabeaver/Search Algorithms/__init__.py
+-rw-rw-rw-   0        0        0     2686 2023-11-01 10:30:45.000000 metabeaver-0.3.5/metabeaver/Search Algorithms/binarySearch.py
+drwxrwxrwx   0        0        0        0 2024-04-02 19:59:14.206986 metabeaver-0.3.5/metabeaver/Set Theory/
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.5/metabeaver/Set Theory/__init__.py
+-rw-rw-rw-   0        0        0     5497 2023-10-06 17:16:32.000000 metabeaver-0.3.5/metabeaver/Set Theory/findAllSubsets.py
+drwxrwxrwx   0        0        0        0 2024-04-02 19:59:14.206986 metabeaver-0.3.5/metabeaver/Sorting Algorithms/
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.5/metabeaver/Sorting Algorithms/__init__.py
+-rw-rw-rw-   0        0        0     3080 2023-12-12 09:32:50.000000 metabeaver-0.3.5/metabeaver/Sorting Algorithms/heapSort.py
+-rw-rw-rw-   0        0        0     1539 2023-10-15 18:11:43.000000 metabeaver-0.3.5/metabeaver/Sorting Algorithms/insertionSort.py
+-rw-rw-rw-   0        0        0     1275 2024-01-09 08:35:40.000000 metabeaver-0.3.5/metabeaver/Sorting Algorithms/mergeSort.py
+-rw-rw-rw-   0        0        0     1136 2023-10-13 07:08:11.000000 metabeaver-0.3.5/metabeaver/Sorting Algorithms/quickSort.py
+-rw-rw-rw-   0        0        0     3213 2023-10-12 10:18:23.000000 metabeaver-0.3.5/metabeaver/Sorting Algorithms/timsort.py
+drwxrwxrwx   0        0        0        0 2024-04-02 19:59:14.216357 metabeaver-0.3.5/metabeaver/Testing/
+-rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.3.5/metabeaver/Testing/__init__.py
+-rw-rw-rw-   0        0        0     3544 2023-11-03 10:47:27.000000 metabeaver-0.3.5/metabeaver/Testing/scratchPad.py
+drwxrwxrwx   0        0        0        0 2024-04-02 19:59:14.222136 metabeaver-0.3.5/metabeaver/TextValidation/
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.3.5/metabeaver/TextValidation/__init__.py
+-rw-rw-rw-   0        0        0     1418 2023-09-27 14:33:38.000000 metabeaver-0.3.5/metabeaver/TextValidation/closureChecker.py
+-rw-rw-rw-   0        0        0     4004 2023-11-01 10:50:46.000000 metabeaver-0.3.5/metabeaver/TextValidation/establishLargestPalindrome.py
+drwxrwxrwx   0        0        0        0 2024-04-02 19:59:14.226143 metabeaver-0.3.5/metabeaver/WebScraping/
+-rw-rw-rw-   0        0        0       54 2023-11-28 09:31:41.000000 metabeaver-0.3.5/metabeaver/WebScraping/__init__.py
+-rw-rw-rw-   0        0        0     1322 2023-11-28 09:40:35.000000 metabeaver-0.3.5/metabeaver/WebScraping/simpleRequests.py
+-rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.3.5/metabeaver/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 19:59:14.226143 metabeaver-0.3.5/metabeaver.egg-info/
+-rw-rw-rw-   0        0        0      339 2024-04-02 19:59:14.000000 metabeaver-0.3.5/metabeaver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4000 2024-04-02 19:59:14.000000 metabeaver-0.3.5/metabeaver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 19:59:14.000000 metabeaver-0.3.5/metabeaver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-04-02 19:59:14.000000 metabeaver-0.3.5/metabeaver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-02 19:59:14.000000 metabeaver-0.3.5/metabeaver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-02 19:59:14.226143 metabeaver-0.3.5/setup.cfg
+-rw-rw-rw-   0        0        0     1307 2024-04-02 19:58:08.000000 metabeaver-0.3.5/setup.py
```

### Comparing `metabeaver-0.3.4/metabeaver/BeaverTown/abstractBeaver.py` & `metabeaver-0.3.5/metabeaver/BeaverTown/abstractBeaver.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.4/metabeaver/BeaverTown/beaverOn.py` & `metabeaver-0.3.5/metabeaver/BeaverTown/beaverOn.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.4/metabeaver/Binary/binaryOperations.py` & `metabeaver-0.3.5/metabeaver/Binary/binaryOperations.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.4/metabeaver/Caching/LeastRecentlyUsed.py` & `metabeaver-0.3.5/metabeaver/Caching/LeastRecentlyUsed.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.4/metabeaver/DataManipulation/localPickle.py` & `metabeaver-0.3.5/metabeaver/DataManipulation/localPickle.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.4/metabeaver/DataManipulation/universalResourceLinkHandler.py` & `metabeaver-0.3.5/metabeaver/DataManipulation/universalResourceLinkHandler.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.4/metabeaver/DataStructures/BinarySearchTree.py` & `metabeaver-0.3.5/metabeaver/DataStructures/BinarySearchTree.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.4/metabeaver/DatabaseFunctionality/SQL/rawSQL.py` & `metabeaver-0.3.5/metabeaver/DatabaseFunctionality/SQL/rawSQL.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.4/metabeaver/DatabaseFunctionality/SQLite/SQLiteDatabase.py` & `metabeaver-0.3.5/metabeaver/DatabaseFunctionality/SQLite/SQLiteDatabase.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.4/metabeaver/DatabaseFunctionality/SQLite/commonCreateUpdate.py` & `metabeaver-0.3.5/metabeaver/DatabaseFunctionality/SQLite/commonCreateUpdate.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.4/metabeaver/DatabaseFunctionality/SQLite/inspectTable.py` & `metabeaver-0.3.5/metabeaver/DatabaseFunctionality/SQLite/inspectTable.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.4/metabeaver/DatesAndTime/getToday.py` & `metabeaver-0.3.5/metabeaver/DatesAndTime/getToday.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.4/metabeaver/FileIO/yamlIO.py` & `metabeaver-0.3.5/metabeaver/FileIO/yamlIO.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.4/metabeaver/Formatting/printControlTest.py` & `metabeaver-0.3.5/metabeaver/Formatting/printControlTest.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.4/metabeaver/GoogleCloudPlatform/BigQuery/TableManagement.py` & `metabeaver-0.3.5/metabeaver/GoogleCloudPlatform/BigQuery/TableManagement.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.4/metabeaver/GoogleCloudPlatform/BigQuery/clientFromCredentials.py` & `metabeaver-0.3.5/metabeaver/GoogleCloudPlatform/BigQuery/clientFromCredentials.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.4/metabeaver/Graph Algorithms/depthFirstSearch.py` & `metabeaver-0.3.5/metabeaver/Graph Algorithms/depthFirstSearch.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.4/metabeaver/Graphing/markdownGenerator.py` & `metabeaver-0.3.5/metabeaver/Graphing/markdownGenerator.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.4/metabeaver/InstallationScripts/autoGenerateRequirementsText.py` & `metabeaver-0.3.5/metabeaver/InstallationScripts/autoGenerateRequirementsText.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.4/metabeaver/InterviewQuestions/Arrays/bestTimeSellStock.py` & `metabeaver-0.3.5/metabeaver/InterviewQuestions/Arrays/bestTimeSellStock.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.4/metabeaver/InterviewQuestions/Arrays/removeThirdDuplicate.py` & `metabeaver-0.3.5/metabeaver/InterviewQuestions/Arrays/removeThirdDuplicate.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.4/metabeaver/InterviewQuestions/Arrays/twoSum.py` & `metabeaver-0.3.5/metabeaver/InterviewQuestions/Arrays/twoSum.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.4/metabeaver/InterviewQuestions/Stacks/calculateFromSymbols.py` & `metabeaver-0.3.5/metabeaver/InterviewQuestions/Stacks/calculateFromSymbols.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.4/metabeaver/LearnPython/ControlFlow/ifelifelse.py` & `metabeaver-0.3.5/metabeaver/LearnPython/ControlFlow/ifelifelse.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.4/metabeaver/Machine Learning/LLM/loadWithTransformers.py` & `metabeaver-0.3.5/metabeaver/Machine Learning/LLM/loadWithTransformers.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.4/metabeaver/Machine Learning/lassoRegression.py` & `metabeaver-0.3.5/metabeaver/Machine Learning/lassoRegression.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.4/metabeaver/Mathematical Operations/vectorDotProduct.py` & `metabeaver-0.3.5/metabeaver/Mathematical Operations/vectorDotProduct.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.4/metabeaver/Search Algorithms/binarySearch.py` & `metabeaver-0.3.5/metabeaver/Search Algorithms/binarySearch.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.4/metabeaver/Set Theory/findAllSubsets.py` & `metabeaver-0.3.5/metabeaver/Set Theory/findAllSubsets.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.4/metabeaver/Sorting Algorithms/heapSort.py` & `metabeaver-0.3.5/metabeaver/Sorting Algorithms/heapSort.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.4/metabeaver/Sorting Algorithms/insertionSort.py` & `metabeaver-0.3.5/metabeaver/Sorting Algorithms/insertionSort.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.4/metabeaver/Sorting Algorithms/mergeSort.py` & `metabeaver-0.3.5/metabeaver/Sorting Algorithms/mergeSort.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.4/metabeaver/Sorting Algorithms/quickSort.py` & `metabeaver-0.3.5/metabeaver/Sorting Algorithms/quickSort.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.4/metabeaver/Sorting Algorithms/timsort.py` & `metabeaver-0.3.5/metabeaver/Sorting Algorithms/timsort.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.4/metabeaver/Testing/scratchPad.py` & `metabeaver-0.3.5/metabeaver/Testing/scratchPad.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.4/metabeaver/TextValidation/closureChecker.py` & `metabeaver-0.3.5/metabeaver/TextValidation/closureChecker.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.4/metabeaver/TextValidation/establishLargestPalindrome.py` & `metabeaver-0.3.5/metabeaver/TextValidation/establishLargestPalindrome.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.4/metabeaver/WebScraping/simpleRequests.py` & `metabeaver-0.3.5/metabeaver/WebScraping/simpleRequests.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.4/metabeaver.egg-info/SOURCES.txt` & `metabeaver-0.3.5/metabeaver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metabeaver-0.3.4/setup.py` & `metabeaver-0.3.5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from setuptools import setup, find_packages
 
 setup(
     name='metabeaver',
-    version='0.3.4', # Major, minor, patch
+    version='0.3.5', # Major, minor, patch
     packages=find_packages(exclude=['Testing', '*.xlsx', '*.xls']),
     install_requires=[
+        'google-cloud-bigquery',
+        'google-cloud-core',
         'numpy',
         'pandas',
-        'google-cloud-core',
-        'google-cloud-bigquery',
+        #transformers,
+        #llama-cpp-python,
     ],
-    description='Beaverish about data. '
-                'Metabeaver originally started as a "glue" project to bring together commonly used code. '
-                'It has since expanded to contain common operations, metaprogramming, and Computer Sci resources. ' 
-                'It is intended a resource to learn computer science, Python, and limit the need to rebuild the wheel. '
-                'For development operations, please see Operation Beaver.'
-    ,
+    description='Beaverish about data. \n'
+                'Metabeaver originally started as a "glue" project to bring together commonly used code. \n'
+                'It has since expanded to contain common operations, metaprogramming, and Computer Sci resources. \n' 
+                'It is intended a resource to learn computer science, Python, and limit the need to rebuild the wheel. \n'
+                'For development operations, please see Operation Beaver.',
     author='Luke Anthony Pollen',
     author_email='luke@pollenanalytics.com',
     url='https://github.com/rainbowpusheenthe3rd/dataBeaver',
 )
 
 
 ##### ERRATA #####
```

