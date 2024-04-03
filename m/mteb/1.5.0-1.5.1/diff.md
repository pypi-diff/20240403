# Comparing `tmp/mteb-1.5.0.tar.gz` & `tmp/mteb-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mteb-1.5.0.tar", last modified: Tue Apr  2 17:03:38 2024, max compression
+gzip compressed data, was "mteb-1.5.1.tar", last modified: Wed Apr  3 12:30:54 2024, max compression
```

## Comparing `mteb-1.5.0.tar` & `mteb-1.5.1.tar`

### file list

```diff
@@ -1,371 +1,371 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.082607 mteb-1.5.0/
--rw-r--r--   0 root         (0) root         (0)    11357 2024-04-02 17:03:33.000000 mteb-1.5.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)    23581 2024-04-02 17:03:38.082607 mteb-1.5.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9190 2024-04-02 17:03:33.000000 mteb-1.5.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.026606 mteb-1.5.0/mteb/
--rw-r--r--   0 root         (0) root         (0)     1917 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.030607 mteb-1.5.0/mteb/abstasks/
--rw-r--r--   0 root         (0) root         (0)     1751 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/abstasks/AbsTask.py
--rw-r--r--   0 root         (0) root         (0)     3063 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/abstasks/AbsTaskBitextMining.py
--rw-r--r--   0 root         (0) root         (0)     5881 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/abstasks/AbsTaskClassification.py
--rw-r--r--   0 root         (0) root         (0)     2389 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/abstasks/AbsTaskClustering.py
--rw-r--r--   0 root         (0) root         (0)     2542 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/abstasks/AbsTaskPairClassification.py
--rw-r--r--   0 root         (0) root         (0)     1120 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/abstasks/AbsTaskReranking.py
--rw-r--r--   0 root         (0) root         (0)    11806 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/abstasks/AbsTaskRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2007 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/abstasks/AbsTaskSTS.py
--rw-r--r--   0 root         (0) root         (0)     2296 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/abstasks/AbsTaskSummarization.py
--rw-r--r--   0 root         (0) root         (0)      880 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/abstasks/CrosslingualTask.py
--rw-r--r--   0 root         (0) root         (0)     2831 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/abstasks/LangMapping.py
--rw-r--r--   0 root         (0) root         (0)      998 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/abstasks/MultilingualTask.py
--rw-r--r--   0 root         (0) root         (0)     6391 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/abstasks/TaskMetadata.py
--rw-r--r--   0 root         (0) root         (0)      422 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/abstasks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5296 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/cmd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.030607 mteb-1.5.0/mteb/evaluation/
--rw-r--r--   0 root         (0) root         (0)    13078 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/evaluation/MTEB.py
--rw-r--r--   0 root         (0) root         (0)       56 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/evaluation/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.030607 mteb-1.5.0/mteb/evaluation/evaluators/
--rw-r--r--   0 root         (0) root         (0)     5849 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/evaluation/evaluators/BitextMiningEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     8942 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/evaluation/evaluators/ClassificationEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     1463 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/evaluation/evaluators/ClusteringEvaluator.py
--rw-r--r--   0 root         (0) root         (0)      744 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/evaluation/evaluators/Evaluator.py
--rw-r--r--   0 root         (0) root         (0)     7140 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/evaluation/evaluators/PairClassificationEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     9613 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/evaluation/evaluators/RerankingEvaluator.py
--rw-r--r--   0 root         (0) root         (0)    12487 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/evaluation/evaluators/RetrievalEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     2394 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/evaluation/evaluators/STSEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     4841 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/evaluation/evaluators/SummarizationEvaluator.py
--rw-r--r--   0 root         (0) root         (0)      324 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/evaluation/evaluators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5482 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/evaluation/evaluators/utils.py
--rw-r--r--   0 root         (0) root         (0)      835 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/logging.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.034607 mteb-1.5.0/mteb/tasks/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.034607 mteb-1.5.0/mteb/tasks/BitextMining/
--rw-r--r--   0 root         (0) root         (0)      369 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/BitextMining/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.034607 mteb-1.5.0/mteb/tasks/BitextMining/da/
--rw-r--r--   0 root         (0) root         (0)     1398 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/BitextMining/da/BornholmskBitextMining.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/BitextMining/da/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.034607 mteb-1.5.0/mteb/tasks/BitextMining/multilingual/
--rw-r--r--   0 root         (0) root         (0)     1076 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/BitextMining/multilingual/BUCCBitextMining.py
--rw-r--r--   0 root         (0) root         (0)     2194 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/BitextMining/multilingual/DiaBLaBitextMining.py
--rw-r--r--   0 root         (0) root         (0)     5780 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/BitextMining/multilingual/FloresBitextMining.py
--rw-r--r--   0 root         (0) root         (0)     1411 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/BitextMining/multilingual/NorwegianCourtsBitextMining.py
--rw-r--r--   0 root         (0) root         (0)     2797 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/BitextMining/multilingual/TatoebaBitextMining.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/BitextMining/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.034607 mteb-1.5.0/mteb/tasks/BitextMining/nb/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/BitextMining/nb/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1351 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/BitextMining/nb/norwegian_courts_bitext_mining.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.034607 mteb-1.5.0/mteb/tasks/Classification/
--rw-r--r--   0 root         (0) root         (0)     1232 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Classification/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.034607 mteb-1.5.0/mteb/tasks/Classification/da/
--rw-r--r--   0 root         (0) root         (0)     1316 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Classification/da/AngryTweetsClassification.py
--rw-r--r--   0 root         (0) root         (0)     1615 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Classification/da/DKHateClassification.py
--rw-r--r--   0 root         (0) root         (0)     2505 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Classification/da/DalajClassification.py
--rw-r--r--   0 root         (0) root         (0)     1610 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Classification/da/DanishPoliticalCommentsClassification.py
--rw-r--r--   0 root         (0) root         (0)     2937 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Classification/da/DdiscoCohesionClassification.py
--rw-r--r--   0 root         (0) root         (0)     1255 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Classification/da/LccSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Classification/da/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.038607 mteb-1.5.0/mteb/tasks/Classification/en/
--rw-r--r--   0 root         (0) root         (0)     1035 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Classification/en/AmazonPolarityClassification.py
--rw-r--r--   0 root         (0) root         (0)     1048 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Classification/en/Banking77Classification.py
--rw-r--r--   0 root         (0) root         (0)     1368 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Classification/en/EmotionClassification.py
--rw-r--r--   0 root         (0) root         (0)      984 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Classification/en/ImdbClassification.py
--rw-r--r--   0 root         (0) root         (0)     1400 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Classification/en/ToxicConversationsClassification.py
--rw-r--r--   0 root         (0) root         (0)     1275 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Classification/en/TweetSentimentExtractionClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Classification/en/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.038607 mteb-1.5.0/mteb/tasks/Classification/multilingual/
--rw-r--r--   0 root         (0) root         (0)     1485 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Classification/multilingual/AmazonCounterfactualClassification.py
--rw-r--r--   0 root         (0) root         (0)     1235 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Classification/multilingual/AmazonReviewsClassification.py
--rw-r--r--   0 root         (0) root         (0)     1164 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Classification/multilingual/MTOPDomainClassification.py
--rw-r--r--   0 root         (0) root         (0)     1164 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Classification/multilingual/MTOPIntentClassification.py
--rw-r--r--   0 root         (0) root         (0)     1403 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Classification/multilingual/MasakhaNEWSClassification.py
--rw-r--r--   0 root         (0) root         (0)     1823 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Classification/multilingual/MassiveIntentClassification.py
--rw-r--r--   0 root         (0) root         (0)     1829 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Classification/multilingual/MassiveScenarioClassification.py
--rw-r--r--   0 root         (0) root         (0)     1468 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Classification/multilingual/NordicLangClassification.py
--rw-r--r--   0 root         (0) root         (0)     6035 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Classification/multilingual/ScalaClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Classification/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.038607 mteb-1.5.0/mteb/tasks/Classification/nb/
--rw-r--r--   0 root         (0) root         (0)     1110 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Classification/nb/NoRecClassification.py
--rw-r--r--   0 root         (0) root         (0)     1160 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Classification/nb/NorwegianParliamentClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Classification/nb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.042607 mteb-1.5.0/mteb/tasks/Classification/pl/
--rw-r--r--   0 root         (0) root         (0)     4892 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Classification/pl/PolishClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Classification/pl/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.042607 mteb-1.5.0/mteb/tasks/Classification/sv/
--rw-r--r--   0 root         (0) root         (0)     1031 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Classification/sv/SweRecClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Classification/sv/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.042607 mteb-1.5.0/mteb/tasks/Classification/zh/
--rw-r--r--   0 root         (0) root         (0)     6535 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Classification/zh/CMTEBClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Classification/zh/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.042607 mteb-1.5.0/mteb/tasks/Clustering/
--rw-r--r--   0 root         (0) root         (0)     1249 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.042607 mteb-1.5.0/mteb/tasks/Clustering/de/
--rw-r--r--   0 root         (0) root         (0)     1126 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/de/BlurbsClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1109 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/de/BlurbsClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1094 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/de/TenKGnadClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1074 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/de/TenKGnadClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/de/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.046607 mteb-1.5.0/mteb/tasks/Clustering/en/
--rw-r--r--   0 root         (0) root         (0)     1095 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/en/ArxivClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1081 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/en/ArxivClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1122 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/en/BigPatentClustering.py
--rw-r--r--   0 root         (0) root         (0)     1065 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/en/BiorxivClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1055 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/en/BiorxivClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1066 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/en/MedrxivClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1056 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/en/MedrxivClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1096 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/en/RedditClustering.py
--rw-r--r--   0 root         (0) root         (0)     1085 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/en/RedditClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1121 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/en/StackExchangeClustering.py
--rw-r--r--   0 root         (0) root         (0)     1109 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/en/StackExchangeClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1078 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/en/TwentyNewsgroupsClustering.py
--rw-r--r--   0 root         (0) root         (0)     1129 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/en/WikiCitiesClustering.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/en/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.046607 mteb-1.5.0/mteb/tasks/Clustering/es/
--rw-r--r--   0 root         (0) root         (0)     1023 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/es/FloresClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1052 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/es/SpanishNewsClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/es/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.046607 mteb-1.5.0/mteb/tasks/Clustering/fr/
--rw-r--r--   0 root         (0) root         (0)     1901 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/fr/AlloProfClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1747 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/fr/AlloProfClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1600 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/fr/HALClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1931 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/fr/MLSUMClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1746 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/fr/MLSUMClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/fr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.046607 mteb-1.5.0/mteb/tasks/Clustering/multilingual/
--rw-r--r--   0 root         (0) root         (0)     2494 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     2513 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.046607 mteb-1.5.0/mteb/tasks/Clustering/nb/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/nb/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3436 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/nb/snl_clustering.py
--rw-r--r--   0 root         (0) root         (0)     3590 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/nb/vg_clustering.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.046607 mteb-1.5.0/mteb/tasks/Clustering/pl/
--rw-r--r--   0 root         (0) root         (0)     1129 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/pl/PolishClustering.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/pl/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.050607 mteb-1.5.0/mteb/tasks/Clustering/sv/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/sv/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3920 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/sv/swedn_clustering.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.050607 mteb-1.5.0/mteb/tasks/Clustering/zh/
--rw-r--r--   0 root         (0) root         (0)     3585 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/zh/CMTEBClustering.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/zh/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.050607 mteb-1.5.0/mteb/tasks/PairClassification/
--rw-r--r--   0 root         (0) root         (0)      301 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/PairClassification/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.050607 mteb-1.5.0/mteb/tasks/PairClassification/en/
--rw-r--r--   0 root         (0) root         (0)     1146 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/PairClassification/en/SprintDuplicateQuestionsPC.py
--rw-r--r--   0 root         (0) root         (0)     1080 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/PairClassification/en/TwitterSemEval2015PC.py
--rw-r--r--   0 root         (0) root         (0)     1034 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/PairClassification/en/TwitterURLCorpusPC.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/PairClassification/en/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.050607 mteb-1.5.0/mteb/tasks/PairClassification/multilingual/
--rw-r--r--   0 root         (0) root         (0)     2687 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/PairClassification/multilingual/OpusparcusPC.py
--rw-r--r--   0 root         (0) root         (0)     1902 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/PairClassification/multilingual/PawsX.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/PairClassification/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.050607 mteb-1.5.0/mteb/tasks/PairClassification/pl/
--rw-r--r--   0 root         (0) root         (0)     3442 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/PairClassification/pl/PolishPC.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/PairClassification/pl/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.050607 mteb-1.5.0/mteb/tasks/PairClassification/zh/
--rw-r--r--   0 root         (0) root         (0)     1837 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/PairClassification/zh/CMTEBPairClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/PairClassification/zh/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.050607 mteb-1.5.0/mteb/tasks/Reranking/
--rw-r--r--   0 root         (0) root         (0)      339 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Reranking/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.054607 mteb-1.5.0/mteb/tasks/Reranking/en/
--rw-r--r--   0 root         (0) root         (0)     1112 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Reranking/en/AskUbuntuDupQuestions.py
--rw-r--r--   0 root         (0) root         (0)     1058 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Reranking/en/MindSmallReranking.py
--rw-r--r--   0 root         (0) root         (0)     3010 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Reranking/en/SciDocsReranking.py
--rw-r--r--   0 root         (0) root         (0)     1131 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Reranking/en/StackOverflowDupQuestions.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Reranking/en/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.054607 mteb-1.5.0/mteb/tasks/Reranking/fr/
--rw-r--r--   0 root         (0) root         (0)     1173 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Reranking/fr/AlloprofReranking.py
--rw-r--r--   0 root         (0) root         (0)     1059 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Reranking/fr/SyntecReranking.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Reranking/fr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.054607 mteb-1.5.0/mteb/tasks/Reranking/multilingual/
--rw-r--r--   0 root         (0) root         (0)     1206 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Reranking/multilingual/MIRACLReranking.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Reranking/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.054607 mteb-1.5.0/mteb/tasks/Reranking/zh/
--rw-r--r--   0 root         (0) root         (0)     3504 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Reranking/zh/CMTEBReranking.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Reranking/zh/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.054607 mteb-1.5.0/mteb/tasks/Retrieval/
--rw-r--r--   0 root         (0) root         (0)     2462 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.054607 mteb-1.5.0/mteb/tasks/Retrieval/da/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/da/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3788 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/da/dan_fever.py
--rw-r--r--   0 root         (0) root         (0)     2577 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/da/t2nord_retrieval.py
--rw-r--r--   0 root         (0) root         (0)     3142 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/da/twitterhjerne.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.054607 mteb-1.5.0/mteb/tasks/Retrieval/de/
--rw-r--r--   0 root         (0) root         (0)     1997 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/de/GerDaLIRRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2896 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/de/GermanDPRRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2111 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/de/GermanQuADRetrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/de/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.062607 mteb-1.5.0/mteb/tasks/Retrieval/en/
--rw-r--r--   0 root         (0) root         (0)     1005 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/en/ArguAnaRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1059 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/en/CQADupstackAndroidRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1059 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/en/CQADupstackEnglishRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1056 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/en/CQADupstackGamingRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1047 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/en/CQADupstackGisRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1071 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/en/CQADupstackMathematicaRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1059 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/en/CQADupstackPhysicsRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1071 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/en/CQADupstackProgrammersRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1053 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/en/CQADupstackStatsRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1047 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/en/CQADupstackTexRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1050 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/en/CQADupstackUnixRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1068 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/en/CQADupstackWebmastersRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1065 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/en/CQADupstackWordpressRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1089 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/en/ClimateFEVERRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1025 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/en/DBPediaRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1169 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/en/FEVERRetrieval.py
--rw-r--r--   0 root         (0) root         (0)      977 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/en/FiQA2018Retrieval.py
--rw-r--r--   0 root         (0) root         (0)     3699 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/en/HagridRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1145 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/en/HotpotQARetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1003 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/en/MSMARCORetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1033 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/en/MSMARCOv2Retrieval.py
--rw-r--r--   0 root         (0) root         (0)     1018 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/en/NFCorpusRetrieval.py
--rw-r--r--   0 root         (0) root         (0)      993 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/en/NQRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2032 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/en/NarrativeQARetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1149 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/en/QuoraRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1108 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/en/SCIDOCSRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1040 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/en/SciFactRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1063 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/en/TRECCOVIDRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1003 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/en/Touche2020Retrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/en/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.062607 mteb-1.5.0/mteb/tasks/Retrieval/es/
--rw-r--r--   0 root         (0) root         (0)     2117 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/es/SpanishPassageRetrievalS2P.py
--rw-r--r--   0 root         (0) root         (0)     2119 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/es/SpanishPassageRetrievalS2S.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/es/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.062607 mteb-1.5.0/mteb/tasks/Retrieval/fr/
--rw-r--r--   0 root         (0) root         (0)     2178 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/fr/AlloprofRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2456 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/fr/BSARDRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2164 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/fr/SyntecRetrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/fr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.062607 mteb-1.5.0/mteb/tasks/Retrieval/ko/
--rw-r--r--   0 root         (0) root         (0)      900 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/ko/KoMiracl.py
--rw-r--r--   0 root         (0) root         (0)      900 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/ko/KoMrtydi.py
--rw-r--r--   0 root         (0) root         (0)      916 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/ko/KoStrategyQA.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/ko/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.066607 mteb-1.5.0/mteb/tasks/Retrieval/multilingual/
--rw-r--r--   0 root         (0) root         (0)     3248 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/multilingual/MIRACLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2905 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/multilingual/MintakaRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     3250 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/multilingual/MultiLongDocRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2921 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/multilingual/XMarketRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2925 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/multilingual/XPQARetrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.066607 mteb-1.5.0/mteb/tasks/Retrieval/nb/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/nb/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3946 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/nb/norquad.py
--rw-r--r--   0 root         (0) root         (0)     2702 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/nb/snl_retrieval.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.066607 mteb-1.5.0/mteb/tasks/Retrieval/pl/
--rw-r--r--   0 root         (0) root         (0)      961 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/pl/ArguAnaPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1034 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/pl/DBPediaPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)      978 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/pl/FiQAPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1106 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/pl/HotpotQAPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1003 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/pl/MSMARCOPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1034 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/pl/NFCorpusPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)      991 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/pl/NQPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1157 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/pl/QuoraPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1085 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/pl/SCIDOCSPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1047 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/pl/SciFactPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1079 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/pl/TRECCOVIDPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/pl/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.066607 mteb-1.5.0/mteb/tasks/Retrieval/sv/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/sv/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3213 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/sv/swedn_retrieval.py
--rw-r--r--   0 root         (0) root         (0)     2613 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/sv/swefaq_retrieval.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.070607 mteb-1.5.0/mteb/tasks/Retrieval/zh/
--rw-r--r--   0 root         (0) root         (0)    10336 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/zh/CMTEBRetrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/zh/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.070607 mteb-1.5.0/mteb/tasks/STS/
--rw-r--r--   0 root         (0) root         (0)      562 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/STS/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.070607 mteb-1.5.0/mteb/tasks/STS/de/
--rw-r--r--   0 root         (0) root         (0)     1364 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/STS/de/GermanSTSBenchmarkSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/STS/de/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.070607 mteb-1.5.0/mteb/tasks/STS/en/
--rw-r--r--   0 root         (0) root         (0)     1178 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/STS/en/BiossesSTS.py
--rw-r--r--   0 root         (0) root         (0)     1147 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/STS/en/STS12STS.py
--rw-r--r--   0 root         (0) root         (0)     1144 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/STS/en/STS13STS.py
--rw-r--r--   0 root         (0) root         (0)     1178 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/STS/en/STS14STS.py
--rw-r--r--   0 root         (0) root         (0)     1142 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/STS/en/STS15STS.py
--rw-r--r--   0 root         (0) root         (0)     1142 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/STS/en/STS16STS.py
--rw-r--r--   0 root         (0) root         (0)     1202 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/STS/en/STSBenchmarkSTS.py
--rw-r--r--   0 root         (0) root         (0)     1187 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/STS/en/SickrSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/STS/en/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.070607 mteb-1.5.0/mteb/tasks/STS/es/
--rw-r--r--   0 root         (0) root         (0)     1515 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/STS/es/STSES.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/STS/es/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.070607 mteb-1.5.0/mteb/tasks/STS/fr/
--rw-r--r--   0 root         (0) root         (0)     1483 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/STS/fr/SickFrSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/STS/fr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.070607 mteb-1.5.0/mteb/tasks/STS/multilingual/
--rw-r--r--   0 root         (0) root         (0)     1362 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/STS/multilingual/STS17CrosslingualSTS.py
--rw-r--r--   0 root         (0) root         (0)     1484 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/STS/multilingual/STS22CrosslingualSTS.py
--rw-r--r--   0 root         (0) root         (0)     2518 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/STS/multilingual/STSBenchmarkMultilingualSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/STS/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.074607 mteb-1.5.0/mteb/tasks/STS/pl/
--rw-r--r--   0 root         (0) root         (0)     2256 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/STS/pl/PolishSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/STS/pl/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.074607 mteb-1.5.0/mteb/tasks/STS/zh/
--rw-r--r--   0 root         (0) root         (0)     7080 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/STS/zh/CMTEBSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/STS/zh/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.074607 mteb-1.5.0/mteb/tasks/Summarization/
--rw-r--r--   0 root         (0) root         (0)      122 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Summarization/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.074607 mteb-1.5.0/mteb/tasks/Summarization/en/
--rw-r--r--   0 root         (0) root         (0)     1237 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Summarization/en/SummEvalSummarization.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Summarization/en/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.074607 mteb-1.5.0/mteb/tasks/Summarization/fr/
--rw-r--r--   0 root         (0) root         (0)     1277 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Summarization/fr/SummEvalFrSummarization.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Summarization/fr/__init__.py
--rw-r--r--   0 root         (0) root         (0)      252 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.082607 mteb-1.5.0/mteb.egg-info/
--rw-r--r--   0 root         (0) root         (0)    23581 2024-04-02 17:03:37.000000 mteb-1.5.0/mteb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12579 2024-04-02 17:03:38.000000 mteb-1.5.0/mteb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-02 17:03:37.000000 mteb-1.5.0/mteb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2024-04-02 17:03:37.000000 mteb-1.5.0/mteb.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      234 2024-04-02 17:03:37.000000 mteb-1.5.0/mteb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       31 2024-04-02 17:03:37.000000 mteb-1.5.0/mteb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2120 2024-04-02 17:03:34.000000 mteb-1.5.0/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.074607 mteb-1.5.0/scripts/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.074607 mteb-1.5.0/scripts/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.074607 mteb-1.5.0/scripts/data/amazon_polarity/
--rw-r--r--   0 root         (0) root         (0)      842 2024-04-02 17:03:33.000000 mteb-1.5.0/scripts/data/amazon_polarity/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.074607 mteb-1.5.0/scripts/data/amazon_reviews_multi/
--rw-r--r--   0 root         (0) root         (0)     1379 2024-04-02 17:03:33.000000 mteb-1.5.0/scripts/data/amazon_reviews_multi/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.078607 mteb-1.5.0/scripts/data/arxiv/
--rw-r--r--   0 root         (0) root         (0)     3146 2024-04-02 17:03:33.000000 mteb-1.5.0/scripts/data/arxiv/script_clustering.py
--rw-r--r--   0 root         (0) root         (0)     1451 2024-04-02 17:03:33.000000 mteb-1.5.0/scripts/data/arxiv/script_raw.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.078607 mteb-1.5.0/scripts/data/biorxiv/
--rw-r--r--   0 root         (0) root         (0)     1781 2024-04-02 17:03:33.000000 mteb-1.5.0/scripts/data/biorxiv/script_clustering.py
--rw-r--r--   0 root         (0) root         (0)     1674 2024-04-02 17:03:33.000000 mteb-1.5.0/scripts/data/biorxiv/script_raw.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.078607 mteb-1.5.0/scripts/data/bucc/
--rw-r--r--   0 root         (0) root         (0)     1171 2024-04-02 17:03:33.000000 mteb-1.5.0/scripts/data/bucc/create_data.py
--rw-r--r--   0 root         (0) root         (0)     5929 2024-04-02 17:03:33.000000 mteb-1.5.0/scripts/data/create_task_table.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.078607 mteb-1.5.0/scripts/data/germanquad/
--rw-r--r--   0 root         (0) root         (0)     2132 2024-04-02 17:03:33.000000 mteb-1.5.0/scripts/data/germanquad/process_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.078607 mteb-1.5.0/scripts/data/hal/
--rw-r--r--   0 root         (0) root         (0)     1512 2024-04-02 17:03:33.000000 mteb-1.5.0/scripts/data/hal/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.078607 mteb-1.5.0/scripts/data/imdb/
--rw-r--r--   0 root         (0) root         (0)      682 2024-04-02 17:03:33.000000 mteb-1.5.0/scripts/data/imdb/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.078607 mteb-1.5.0/scripts/data/medrxiv/
--rw-r--r--   0 root         (0) root         (0)     1780 2024-04-02 17:03:33.000000 mteb-1.5.0/scripts/data/medrxiv/script_clustering.py
--rw-r--r--   0 root         (0) root         (0)     1617 2024-04-02 17:03:33.000000 mteb-1.5.0/scripts/data/medrxiv/script_raw.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.078607 mteb-1.5.0/scripts/data/mind/
--rw-r--r--   0 root         (0) root         (0)     1377 2024-04-02 17:03:33.000000 mteb-1.5.0/scripts/data/mind/prepare_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.078607 mteb-1.5.0/scripts/data/redditp2p/
--rw-r--r--   0 root         (0) root         (0)     1880 2024-04-02 17:03:33.000000 mteb-1.5.0/scripts/data/redditp2p/script_clustering.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.078607 mteb-1.5.0/scripts/data/stackexchangep2p/
--rw-r--r--   0 root         (0) root         (0)     1627 2024-04-02 17:03:33.000000 mteb-1.5.0/scripts/data/stackexchangep2p/script_clustering.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.078607 mteb-1.5.0/scripts/data/sts22-crosslingual-sts/
--rw-r--r--   0 root         (0) root         (0)     2436 2024-04-02 17:03:33.000000 mteb-1.5.0/scripts/data/sts22-crosslingual-sts/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.078607 mteb-1.5.0/scripts/data/summeval_fr/
--rw-r--r--   0 root         (0) root         (0)     1692 2024-04-02 17:03:33.000000 mteb-1.5.0/scripts/data/summeval_fr/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.078607 mteb-1.5.0/scripts/data/toxic_conversations_50k/
--rw-r--r--   0 root         (0) root         (0)     1151 2024-04-02 17:03:33.000000 mteb-1.5.0/scripts/data/toxic_conversations_50k/create_data.py
--rw-r--r--   0 root         (0) root         (0)     2516 2024-04-02 17:03:33.000000 mteb-1.5.0/scripts/merge_cqadupstack.py
--rw-r--r--   0 root         (0) root         (0)     5217 2024-04-02 17:03:33.000000 mteb-1.5.0/scripts/mteb_meta.py
--rw-r--r--   0 root         (0) root         (0)      673 2024-04-02 17:03:33.000000 mteb-1.5.0/scripts/run_mteb_chinese.py
--rw-r--r--   0 root         (0) root         (0)     2819 2024-04-02 17:03:33.000000 mteb-1.5.0/scripts/run_mteb_english.py
--rw-r--r--   0 root         (0) root         (0)     1852 2024-04-02 17:03:33.000000 mteb-1.5.0/scripts/run_mteb_french.py
--rw-r--r--   0 root         (0) root         (0)     1305 2024-04-02 17:03:33.000000 mteb-1.5.0/scripts/run_mteb_german.py
--rw-r--r--   0 root         (0) root         (0)     1033 2024-04-02 17:03:33.000000 mteb-1.5.0/scripts/run_mteb_korean.py
--rw-r--r--   0 root         (0) root         (0)      975 2024-04-02 17:03:33.000000 mteb-1.5.0/scripts/run_mteb_polish.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-02 17:03:38.082607 mteb-1.5.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.082607 mteb-1.5.0/tests/
--rw-r--r--   0 root         (0) root         (0)      632 2024-04-02 17:03:33.000000 mteb-1.5.0/tests/test_ClusteringEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     1560 2024-04-02 17:03:33.000000 mteb-1.5.0/tests/test_PairClassificationEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     1130 2024-04-02 17:03:33.000000 mteb-1.5.0/tests/test_RerankingEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     1113 2024-04-02 17:03:33.000000 mteb-1.5.0/tests/test_RetrievalEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     3501 2024-04-02 17:03:33.000000 mteb-1.5.0/tests/test_TaskMetadata.py
--rw-r--r--   0 root         (0) root         (0)     2137 2024-04-02 17:03:33.000000 mteb-1.5.0/tests/test_all_abstasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.661619 mteb-1.5.1/
+-rw-r--r--   0 root         (0) root         (0)    11357 2024-04-03 12:30:50.000000 mteb-1.5.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    23581 2024-04-03 12:30:54.661619 mteb-1.5.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9190 2024-04-03 12:30:50.000000 mteb-1.5.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.605618 mteb-1.5.1/mteb/
+-rw-r--r--   0 root         (0) root         (0)     1917 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.605618 mteb-1.5.1/mteb/abstasks/
+-rw-r--r--   0 root         (0) root         (0)     1751 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/abstasks/AbsTask.py
+-rw-r--r--   0 root         (0) root         (0)     3063 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/abstasks/AbsTaskBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)     5881 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/abstasks/AbsTaskClassification.py
+-rw-r--r--   0 root         (0) root         (0)     2389 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/abstasks/AbsTaskClustering.py
+-rw-r--r--   0 root         (0) root         (0)     2542 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/abstasks/AbsTaskPairClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1120 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/abstasks/AbsTaskReranking.py
+-rw-r--r--   0 root         (0) root         (0)    11806 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/abstasks/AbsTaskRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2007 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/abstasks/AbsTaskSTS.py
+-rw-r--r--   0 root         (0) root         (0)     2296 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/abstasks/AbsTaskSummarization.py
+-rw-r--r--   0 root         (0) root         (0)      880 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/abstasks/CrosslingualTask.py
+-rw-r--r--   0 root         (0) root         (0)     2831 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/abstasks/LangMapping.py
+-rw-r--r--   0 root         (0) root         (0)      998 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/abstasks/MultilingualTask.py
+-rw-r--r--   0 root         (0) root         (0)     6430 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/abstasks/TaskMetadata.py
+-rw-r--r--   0 root         (0) root         (0)      422 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/abstasks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5296 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/cmd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.609618 mteb-1.5.1/mteb/evaluation/
+-rw-r--r--   0 root         (0) root         (0)    13124 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/evaluation/MTEB.py
+-rw-r--r--   0 root         (0) root         (0)       56 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/evaluation/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.609618 mteb-1.5.1/mteb/evaluation/evaluators/
+-rw-r--r--   0 root         (0) root         (0)     5849 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/evaluation/evaluators/BitextMiningEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     8942 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/evaluation/evaluators/ClassificationEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     1463 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/evaluation/evaluators/ClusteringEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)      744 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/evaluation/evaluators/Evaluator.py
+-rw-r--r--   0 root         (0) root         (0)     7140 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/evaluation/evaluators/PairClassificationEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     9613 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/evaluation/evaluators/RerankingEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)    12487 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/evaluation/evaluators/RetrievalEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     2394 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/evaluation/evaluators/STSEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     4841 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/evaluation/evaluators/SummarizationEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)      324 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/evaluation/evaluators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5482 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/evaluation/evaluators/utils.py
+-rw-r--r--   0 root         (0) root         (0)      835 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/logging.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.609618 mteb-1.5.1/mteb/tasks/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.609618 mteb-1.5.1/mteb/tasks/BitextMining/
+-rw-r--r--   0 root         (0) root         (0)      369 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/BitextMining/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.609618 mteb-1.5.1/mteb/tasks/BitextMining/da/
+-rw-r--r--   0 root         (0) root         (0)     1398 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/BitextMining/da/BornholmskBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/BitextMining/da/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.613618 mteb-1.5.1/mteb/tasks/BitextMining/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     1076 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/BitextMining/multilingual/BUCCBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)     2194 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/BitextMining/multilingual/DiaBLaBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)     5780 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/BitextMining/multilingual/FloresBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)     1411 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/BitextMining/multilingual/NorwegianCourtsBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)     2797 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/BitextMining/multilingual/TatoebaBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/BitextMining/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.613618 mteb-1.5.1/mteb/tasks/BitextMining/nb/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/BitextMining/nb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1351 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/BitextMining/nb/norwegian_courts_bitext_mining.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.613618 mteb-1.5.1/mteb/tasks/Classification/
+-rw-r--r--   0 root         (0) root         (0)     1232 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Classification/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.613618 mteb-1.5.1/mteb/tasks/Classification/da/
+-rw-r--r--   0 root         (0) root         (0)     1316 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Classification/da/AngryTweetsClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1615 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Classification/da/DKHateClassification.py
+-rw-r--r--   0 root         (0) root         (0)     2505 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Classification/da/DalajClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1610 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Classification/da/DanishPoliticalCommentsClassification.py
+-rw-r--r--   0 root         (0) root         (0)     2937 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Classification/da/DdiscoCohesionClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1255 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Classification/da/LccSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Classification/da/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.613618 mteb-1.5.1/mteb/tasks/Classification/en/
+-rw-r--r--   0 root         (0) root         (0)     1035 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Classification/en/AmazonPolarityClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1048 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Classification/en/Banking77Classification.py
+-rw-r--r--   0 root         (0) root         (0)     1368 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Classification/en/EmotionClassification.py
+-rw-r--r--   0 root         (0) root         (0)      984 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Classification/en/ImdbClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1400 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Classification/en/ToxicConversationsClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1275 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Classification/en/TweetSentimentExtractionClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Classification/en/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.617618 mteb-1.5.1/mteb/tasks/Classification/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     1485 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Classification/multilingual/AmazonCounterfactualClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1235 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Classification/multilingual/AmazonReviewsClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1164 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Classification/multilingual/MTOPDomainClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1164 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Classification/multilingual/MTOPIntentClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1403 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Classification/multilingual/MasakhaNEWSClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1823 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Classification/multilingual/MassiveIntentClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1829 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Classification/multilingual/MassiveScenarioClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1468 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Classification/multilingual/NordicLangClassification.py
+-rw-r--r--   0 root         (0) root         (0)     6075 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Classification/multilingual/ScalaClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Classification/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.617618 mteb-1.5.1/mteb/tasks/Classification/nb/
+-rw-r--r--   0 root         (0) root         (0)     1115 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Classification/nb/NoRecClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1160 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Classification/nb/NorwegianParliamentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Classification/nb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.617618 mteb-1.5.1/mteb/tasks/Classification/pl/
+-rw-r--r--   0 root         (0) root         (0)     4892 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Classification/pl/PolishClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Classification/pl/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.617618 mteb-1.5.1/mteb/tasks/Classification/sv/
+-rw-r--r--   0 root         (0) root         (0)     1037 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Classification/sv/SweRecClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Classification/sv/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.617618 mteb-1.5.1/mteb/tasks/Classification/zh/
+-rw-r--r--   0 root         (0) root         (0)     6535 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Classification/zh/CMTEBClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Classification/zh/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.617618 mteb-1.5.1/mteb/tasks/Clustering/
+-rw-r--r--   0 root         (0) root         (0)     1249 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.621618 mteb-1.5.1/mteb/tasks/Clustering/de/
+-rw-r--r--   0 root         (0) root         (0)     1126 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/de/BlurbsClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1118 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/de/BlurbsClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1094 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/de/TenKGnadClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1074 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/de/TenKGnadClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/de/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.621618 mteb-1.5.1/mteb/tasks/Clustering/en/
+-rw-r--r--   0 root         (0) root         (0)     1095 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/en/ArxivClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1081 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/en/ArxivClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1122 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/en/BigPatentClustering.py
+-rw-r--r--   0 root         (0) root         (0)     1065 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/en/BiorxivClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1055 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/en/BiorxivClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1066 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/en/MedrxivClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1056 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/en/MedrxivClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1096 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/en/RedditClustering.py
+-rw-r--r--   0 root         (0) root         (0)     1085 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/en/RedditClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1121 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/en/StackExchangeClustering.py
+-rw-r--r--   0 root         (0) root         (0)     1109 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/en/StackExchangeClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1078 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/en/TwentyNewsgroupsClustering.py
+-rw-r--r--   0 root         (0) root         (0)     1129 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/en/WikiCitiesClustering.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/en/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.625618 mteb-1.5.1/mteb/tasks/Clustering/es/
+-rw-r--r--   0 root         (0) root         (0)     1027 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/es/FloresClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1054 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/es/SpanishNewsClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/es/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.625618 mteb-1.5.1/mteb/tasks/Clustering/fr/
+-rw-r--r--   0 root         (0) root         (0)     1905 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/fr/AlloProfClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1751 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/fr/AlloProfClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1619 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/fr/HALClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1926 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/fr/MLSUMClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1741 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/fr/MLSUMClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/fr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.625618 mteb-1.5.1/mteb/tasks/Clustering/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     2499 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     2513 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.625618 mteb-1.5.1/mteb/tasks/Clustering/nb/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/nb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3436 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/nb/snl_clustering.py
+-rw-r--r--   0 root         (0) root         (0)     3590 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/nb/vg_clustering.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.625618 mteb-1.5.1/mteb/tasks/Clustering/pl/
+-rw-r--r--   0 root         (0) root         (0)     1131 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/pl/PolishClustering.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/pl/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.625618 mteb-1.5.1/mteb/tasks/Clustering/sv/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/sv/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3920 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/sv/swedn_clustering.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.625618 mteb-1.5.1/mteb/tasks/Clustering/zh/
+-rw-r--r--   0 root         (0) root         (0)     3615 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/zh/CMTEBClustering.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Clustering/zh/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.625618 mteb-1.5.1/mteb/tasks/PairClassification/
+-rw-r--r--   0 root         (0) root         (0)      301 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/PairClassification/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.629618 mteb-1.5.1/mteb/tasks/PairClassification/en/
+-rw-r--r--   0 root         (0) root         (0)     1146 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/PairClassification/en/SprintDuplicateQuestionsPC.py
+-rw-r--r--   0 root         (0) root         (0)     1080 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/PairClassification/en/TwitterSemEval2015PC.py
+-rw-r--r--   0 root         (0) root         (0)     1034 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/PairClassification/en/TwitterURLCorpusPC.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/PairClassification/en/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.629618 mteb-1.5.1/mteb/tasks/PairClassification/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     2687 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/PairClassification/multilingual/OpusparcusPC.py
+-rw-r--r--   0 root         (0) root         (0)     1902 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/PairClassification/multilingual/PawsX.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/PairClassification/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.629618 mteb-1.5.1/mteb/tasks/PairClassification/pl/
+-rw-r--r--   0 root         (0) root         (0)     3553 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/PairClassification/pl/PolishPC.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/PairClassification/pl/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.629618 mteb-1.5.1/mteb/tasks/PairClassification/zh/
+-rw-r--r--   0 root         (0) root         (0)     1837 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/PairClassification/zh/CMTEBPairClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/PairClassification/zh/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.629618 mteb-1.5.1/mteb/tasks/Reranking/
+-rw-r--r--   0 root         (0) root         (0)      339 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Reranking/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.629618 mteb-1.5.1/mteb/tasks/Reranking/en/
+-rw-r--r--   0 root         (0) root         (0)     1112 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Reranking/en/AskUbuntuDupQuestions.py
+-rw-r--r--   0 root         (0) root         (0)     1058 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Reranking/en/MindSmallReranking.py
+-rw-r--r--   0 root         (0) root         (0)     3010 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Reranking/en/SciDocsReranking.py
+-rw-r--r--   0 root         (0) root         (0)     1131 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Reranking/en/StackOverflowDupQuestions.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Reranking/en/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.629618 mteb-1.5.1/mteb/tasks/Reranking/fr/
+-rw-r--r--   0 root         (0) root         (0)     1189 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Reranking/fr/AlloprofReranking.py
+-rw-r--r--   0 root         (0) root         (0)     1059 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Reranking/fr/SyntecReranking.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Reranking/fr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.633618 mteb-1.5.1/mteb/tasks/Reranking/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     1206 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Reranking/multilingual/MIRACLReranking.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Reranking/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.633618 mteb-1.5.1/mteb/tasks/Reranking/zh/
+-rw-r--r--   0 root         (0) root         (0)     3504 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Reranking/zh/CMTEBReranking.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Reranking/zh/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.633618 mteb-1.5.1/mteb/tasks/Retrieval/
+-rw-r--r--   0 root         (0) root         (0)     2462 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.633618 mteb-1.5.1/mteb/tasks/Retrieval/da/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/da/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3788 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/da/dan_fever.py
+-rw-r--r--   0 root         (0) root         (0)     2577 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/da/t2nord_retrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3142 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/da/twitterhjerne.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.633618 mteb-1.5.1/mteb/tasks/Retrieval/de/
+-rw-r--r--   0 root         (0) root         (0)     1997 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/de/GerDaLIRRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2896 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/de/GermanDPRRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2121 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/de/GermanQuADRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/de/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.641618 mteb-1.5.1/mteb/tasks/Retrieval/en/
+-rw-r--r--   0 root         (0) root         (0)     1005 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/en/ArguAnaRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1059 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/en/CQADupstackAndroidRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1059 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/en/CQADupstackEnglishRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1056 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/en/CQADupstackGamingRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1047 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/en/CQADupstackGisRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1071 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/en/CQADupstackMathematicaRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1059 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/en/CQADupstackPhysicsRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1071 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/en/CQADupstackProgrammersRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1053 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/en/CQADupstackStatsRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1047 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/en/CQADupstackTexRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1050 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/en/CQADupstackUnixRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1068 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/en/CQADupstackWebmastersRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1065 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/en/CQADupstackWordpressRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1089 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/en/ClimateFEVERRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1025 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/en/DBPediaRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1169 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/en/FEVERRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)      977 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/en/FiQA2018Retrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3699 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/en/HagridRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1145 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/en/HotpotQARetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1003 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/en/MSMARCORetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1033 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/en/MSMARCOv2Retrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1018 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/en/NFCorpusRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)      993 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/en/NQRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2032 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/en/NarrativeQARetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1149 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/en/QuoraRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1108 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/en/SCIDOCSRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1040 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/en/SciFactRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1063 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/en/TRECCOVIDRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1003 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/en/Touche2020Retrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/en/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.641618 mteb-1.5.1/mteb/tasks/Retrieval/es/
+-rw-r--r--   0 root         (0) root         (0)     2117 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/es/SpanishPassageRetrievalS2P.py
+-rw-r--r--   0 root         (0) root         (0)     2119 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/es/SpanishPassageRetrievalS2S.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/es/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.641618 mteb-1.5.1/mteb/tasks/Retrieval/fr/
+-rw-r--r--   0 root         (0) root         (0)     2182 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/fr/AlloprofRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2469 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/fr/BSARDRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2164 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/fr/SyntecRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/fr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.641618 mteb-1.5.1/mteb/tasks/Retrieval/ko/
+-rw-r--r--   0 root         (0) root         (0)      900 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/ko/KoMiracl.py
+-rw-r--r--   0 root         (0) root         (0)      900 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/ko/KoMrtydi.py
+-rw-r--r--   0 root         (0) root         (0)      916 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/ko/KoStrategyQA.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/ko/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.641618 mteb-1.5.1/mteb/tasks/Retrieval/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     3248 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/multilingual/MIRACLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2905 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/multilingual/MintakaRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3250 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/multilingual/MultiLongDocRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2921 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/multilingual/XMarketRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2925 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/multilingual/XPQARetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.645619 mteb-1.5.1/mteb/tasks/Retrieval/nb/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/nb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3946 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/nb/norquad.py
+-rw-r--r--   0 root         (0) root         (0)     2702 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/nb/snl_retrieval.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.645619 mteb-1.5.1/mteb/tasks/Retrieval/pl/
+-rw-r--r--   0 root         (0) root         (0)      961 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/pl/ArguAnaPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1034 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/pl/DBPediaPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)      978 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/pl/FiQAPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1106 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/pl/HotpotQAPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1003 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/pl/MSMARCOPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1034 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/pl/NFCorpusPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)      991 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/pl/NQPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1157 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/pl/QuoraPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1085 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/pl/SCIDOCSPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1047 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/pl/SciFactPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1079 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/pl/TRECCOVIDPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/pl/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.645619 mteb-1.5.1/mteb/tasks/Retrieval/sv/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/sv/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3213 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/sv/swedn_retrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2613 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/sv/swefaq_retrieval.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.645619 mteb-1.5.1/mteb/tasks/Retrieval/zh/
+-rw-r--r--   0 root         (0) root         (0)    10336 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/zh/CMTEBRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Retrieval/zh/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.645619 mteb-1.5.1/mteb/tasks/STS/
+-rw-r--r--   0 root         (0) root         (0)      562 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/STS/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.649618 mteb-1.5.1/mteb/tasks/STS/de/
+-rw-r--r--   0 root         (0) root         (0)     1364 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/STS/de/GermanSTSBenchmarkSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/STS/de/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.649618 mteb-1.5.1/mteb/tasks/STS/en/
+-rw-r--r--   0 root         (0) root         (0)     1178 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/STS/en/BiossesSTS.py
+-rw-r--r--   0 root         (0) root         (0)     1147 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/STS/en/STS12STS.py
+-rw-r--r--   0 root         (0) root         (0)     1144 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/STS/en/STS13STS.py
+-rw-r--r--   0 root         (0) root         (0)     1178 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/STS/en/STS14STS.py
+-rw-r--r--   0 root         (0) root         (0)     1142 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/STS/en/STS15STS.py
+-rw-r--r--   0 root         (0) root         (0)     1142 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/STS/en/STS16STS.py
+-rw-r--r--   0 root         (0) root         (0)     1202 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/STS/en/STSBenchmarkSTS.py
+-rw-r--r--   0 root         (0) root         (0)     1179 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/STS/en/SickrSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/STS/en/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.649618 mteb-1.5.1/mteb/tasks/STS/es/
+-rw-r--r--   0 root         (0) root         (0)     1480 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/STS/es/STSES.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/STS/es/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.649618 mteb-1.5.1/mteb/tasks/STS/fr/
+-rw-r--r--   0 root         (0) root         (0)     1466 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/STS/fr/SickFrSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/STS/fr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.649618 mteb-1.5.1/mteb/tasks/STS/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     1362 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/STS/multilingual/STS17CrosslingualSTS.py
+-rw-r--r--   0 root         (0) root         (0)     1484 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/STS/multilingual/STS22CrosslingualSTS.py
+-rw-r--r--   0 root         (0) root         (0)     2528 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/STS/multilingual/STSBenchmarkMultilingualSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/STS/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.649618 mteb-1.5.1/mteb/tasks/STS/pl/
+-rw-r--r--   0 root         (0) root         (0)     2256 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/STS/pl/PolishSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/STS/pl/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.653619 mteb-1.5.1/mteb/tasks/STS/zh/
+-rw-r--r--   0 root         (0) root         (0)     7080 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/STS/zh/CMTEBSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/STS/zh/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.653619 mteb-1.5.1/mteb/tasks/Summarization/
+-rw-r--r--   0 root         (0) root         (0)      122 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Summarization/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.653619 mteb-1.5.1/mteb/tasks/Summarization/en/
+-rw-r--r--   0 root         (0) root         (0)     1237 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Summarization/en/SummEvalSummarization.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Summarization/en/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.653619 mteb-1.5.1/mteb/tasks/Summarization/fr/
+-rw-r--r--   0 root         (0) root         (0)     1298 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Summarization/fr/SummEvalFrSummarization.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/Summarization/fr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      252 2024-04-03 12:30:50.000000 mteb-1.5.1/mteb/tasks/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.657619 mteb-1.5.1/mteb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    23581 2024-04-03 12:30:54.000000 mteb-1.5.1/mteb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12579 2024-04-03 12:30:54.000000 mteb-1.5.1/mteb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 12:30:54.000000 mteb-1.5.1/mteb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2024-04-03 12:30:54.000000 mteb-1.5.1/mteb.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      234 2024-04-03 12:30:54.000000 mteb-1.5.1/mteb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2024-04-03 12:30:54.000000 mteb-1.5.1/mteb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2120 2024-04-03 12:30:51.000000 mteb-1.5.1/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.653619 mteb-1.5.1/scripts/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.653619 mteb-1.5.1/scripts/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.653619 mteb-1.5.1/scripts/data/amazon_polarity/
+-rw-r--r--   0 root         (0) root         (0)      842 2024-04-03 12:30:50.000000 mteb-1.5.1/scripts/data/amazon_polarity/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.653619 mteb-1.5.1/scripts/data/amazon_reviews_multi/
+-rw-r--r--   0 root         (0) root         (0)     1379 2024-04-03 12:30:50.000000 mteb-1.5.1/scripts/data/amazon_reviews_multi/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.653619 mteb-1.5.1/scripts/data/arxiv/
+-rw-r--r--   0 root         (0) root         (0)     3146 2024-04-03 12:30:50.000000 mteb-1.5.1/scripts/data/arxiv/script_clustering.py
+-rw-r--r--   0 root         (0) root         (0)     1451 2024-04-03 12:30:50.000000 mteb-1.5.1/scripts/data/arxiv/script_raw.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.653619 mteb-1.5.1/scripts/data/biorxiv/
+-rw-r--r--   0 root         (0) root         (0)     1781 2024-04-03 12:30:50.000000 mteb-1.5.1/scripts/data/biorxiv/script_clustering.py
+-rw-r--r--   0 root         (0) root         (0)     1674 2024-04-03 12:30:50.000000 mteb-1.5.1/scripts/data/biorxiv/script_raw.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.657619 mteb-1.5.1/scripts/data/bucc/
+-rw-r--r--   0 root         (0) root         (0)     1171 2024-04-03 12:30:50.000000 mteb-1.5.1/scripts/data/bucc/create_data.py
+-rw-r--r--   0 root         (0) root         (0)     5929 2024-04-03 12:30:50.000000 mteb-1.5.1/scripts/data/create_task_table.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.657619 mteb-1.5.1/scripts/data/germanquad/
+-rw-r--r--   0 root         (0) root         (0)     2132 2024-04-03 12:30:50.000000 mteb-1.5.1/scripts/data/germanquad/process_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.657619 mteb-1.5.1/scripts/data/hal/
+-rw-r--r--   0 root         (0) root         (0)     1512 2024-04-03 12:30:50.000000 mteb-1.5.1/scripts/data/hal/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.657619 mteb-1.5.1/scripts/data/imdb/
+-rw-r--r--   0 root         (0) root         (0)      682 2024-04-03 12:30:50.000000 mteb-1.5.1/scripts/data/imdb/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.657619 mteb-1.5.1/scripts/data/medrxiv/
+-rw-r--r--   0 root         (0) root         (0)     1780 2024-04-03 12:30:50.000000 mteb-1.5.1/scripts/data/medrxiv/script_clustering.py
+-rw-r--r--   0 root         (0) root         (0)     1617 2024-04-03 12:30:50.000000 mteb-1.5.1/scripts/data/medrxiv/script_raw.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.657619 mteb-1.5.1/scripts/data/mind/
+-rw-r--r--   0 root         (0) root         (0)     1377 2024-04-03 12:30:50.000000 mteb-1.5.1/scripts/data/mind/prepare_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.657619 mteb-1.5.1/scripts/data/redditp2p/
+-rw-r--r--   0 root         (0) root         (0)     1880 2024-04-03 12:30:50.000000 mteb-1.5.1/scripts/data/redditp2p/script_clustering.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.657619 mteb-1.5.1/scripts/data/stackexchangep2p/
+-rw-r--r--   0 root         (0) root         (0)     1627 2024-04-03 12:30:50.000000 mteb-1.5.1/scripts/data/stackexchangep2p/script_clustering.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.657619 mteb-1.5.1/scripts/data/sts22-crosslingual-sts/
+-rw-r--r--   0 root         (0) root         (0)     2436 2024-04-03 12:30:50.000000 mteb-1.5.1/scripts/data/sts22-crosslingual-sts/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.657619 mteb-1.5.1/scripts/data/summeval_fr/
+-rw-r--r--   0 root         (0) root         (0)     1692 2024-04-03 12:30:50.000000 mteb-1.5.1/scripts/data/summeval_fr/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.657619 mteb-1.5.1/scripts/data/toxic_conversations_50k/
+-rw-r--r--   0 root         (0) root         (0)     1151 2024-04-03 12:30:50.000000 mteb-1.5.1/scripts/data/toxic_conversations_50k/create_data.py
+-rw-r--r--   0 root         (0) root         (0)     2516 2024-04-03 12:30:50.000000 mteb-1.5.1/scripts/merge_cqadupstack.py
+-rw-r--r--   0 root         (0) root         (0)     5217 2024-04-03 12:30:50.000000 mteb-1.5.1/scripts/mteb_meta.py
+-rw-r--r--   0 root         (0) root         (0)      673 2024-04-03 12:30:50.000000 mteb-1.5.1/scripts/run_mteb_chinese.py
+-rw-r--r--   0 root         (0) root         (0)     2819 2024-04-03 12:30:50.000000 mteb-1.5.1/scripts/run_mteb_english.py
+-rw-r--r--   0 root         (0) root         (0)     1852 2024-04-03 12:30:50.000000 mteb-1.5.1/scripts/run_mteb_french.py
+-rw-r--r--   0 root         (0) root         (0)     1305 2024-04-03 12:30:50.000000 mteb-1.5.1/scripts/run_mteb_german.py
+-rw-r--r--   0 root         (0) root         (0)     1033 2024-04-03 12:30:50.000000 mteb-1.5.1/scripts/run_mteb_korean.py
+-rw-r--r--   0 root         (0) root         (0)      975 2024-04-03 12:30:50.000000 mteb-1.5.1/scripts/run_mteb_polish.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-03 12:30:54.661619 mteb-1.5.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:30:54.657619 mteb-1.5.1/tests/
+-rw-r--r--   0 root         (0) root         (0)      632 2024-04-03 12:30:50.000000 mteb-1.5.1/tests/test_ClusteringEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     1560 2024-04-03 12:30:50.000000 mteb-1.5.1/tests/test_PairClassificationEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     1130 2024-04-03 12:30:50.000000 mteb-1.5.1/tests/test_RerankingEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     1113 2024-04-03 12:30:50.000000 mteb-1.5.1/tests/test_RetrievalEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     3471 2024-04-03 12:30:50.000000 mteb-1.5.1/tests/test_TaskMetadata.py
+-rw-r--r--   0 root         (0) root         (0)     3524 2024-04-03 12:30:50.000000 mteb-1.5.1/tests/test_all_abstasks.py
```

### Comparing `mteb-1.5.0/LICENSE` & `mteb-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/PKG-INFO` & `mteb-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mteb
-Version: 1.5.0
+Version: 1.5.1
 Summary: Massive Text Embedding Benchmark
 Author-email: MTEB Contributors <niklas@huggingface.co>, nouamane@huggingface.co, info@nils-reimers.de
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `mteb-1.5.0/README.md` & `mteb-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/__init__.py` & `mteb-1.5.1/mteb/__init__.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/abstasks/AbsTask.py` & `mteb-1.5.1/mteb/abstasks/AbsTask.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/abstasks/AbsTaskBitextMining.py` & `mteb-1.5.1/mteb/abstasks/AbsTaskBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/abstasks/AbsTaskClassification.py` & `mteb-1.5.1/mteb/abstasks/AbsTaskClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/abstasks/AbsTaskClustering.py` & `mteb-1.5.1/mteb/abstasks/AbsTaskClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/abstasks/AbsTaskPairClassification.py` & `mteb-1.5.1/mteb/abstasks/AbsTaskPairClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/abstasks/AbsTaskReranking.py` & `mteb-1.5.1/mteb/abstasks/AbsTaskReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/abstasks/AbsTaskRetrieval.py` & `mteb-1.5.1/mteb/abstasks/AbsTaskRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/abstasks/AbsTaskSTS.py` & `mteb-1.5.1/mteb/abstasks/AbsTaskSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/abstasks/AbsTaskSummarization.py` & `mteb-1.5.1/mteb/abstasks/AbsTaskSummarization.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/abstasks/CrosslingualTask.py` & `mteb-1.5.1/mteb/abstasks/CrosslingualTask.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/abstasks/LangMapping.py` & `mteb-1.5.1/mteb/abstasks/LangMapping.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/abstasks/MultilingualTask.py` & `mteb-1.5.1/mteb/abstasks/MultilingualTask.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/abstasks/TaskMetadata.py` & `mteb-1.5.1/mteb/abstasks/TaskMetadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 from pydantic import (
     AnyUrl,
     BaseModel,
     BeforeValidator,
     TypeAdapter,
     field_validator,
-    model_validator,
 )
 from typing_extensions import Annotated, Literal
 
 TASK_SUBTYPE = Literal[
     "Article retrieval",
     "Dialect pairing",
     "Dialog Systems",
@@ -168,11 +167,15 @@
                 "See https://huggingface.co/docs/datasets/main/en/package_reference/loading_methods#datasets.load_dataset"
             )
         return dataset
 
     @field_validator("dataset")
     def _check_dataset_revision_is_specified(cls, dataset):
         if "revision" not in dataset:
-            raise ValueError("You must explicitly specify a revision for the dataset (either a SHA or None).")
+            raise ValueError(
+                "You must explicitly specify a revision for the dataset (either a SHA or None)."
+            )
         if dataset["revision"] is None:
-            logging.warning("It is encourage to specify a dataset revision for reproducability")
+            logging.warning(
+                "It is encourage to specify a dataset revision for reproducability"
+            )
         return dataset
```

### Comparing `mteb-1.5.0/mteb/cmd.py` & `mteb-1.5.1/mteb/cmd.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/evaluation/MTEB.py` & `mteb-1.5.1/mteb/evaluation/MTEB.py`

 * *Files 0% similar despite different names*

```diff
@@ -300,15 +300,17 @@
                 # load data
                 logger.info(f"Loading dataset for {task.metadata_dict['name']}")
                 task.load_data(eval_splits=task_eval_splits, **kwargs)
 
                 # run evaluation
                 task_results = {
                     "mteb_version": version("mteb"),  # noqa: F405
-                    "dataset_revision": task.metadata_dict["dataset"].get("revision", None),
+                    "dataset_revision": task.metadata_dict["dataset"].get(
+                        "revision", None
+                    ),
                     "mteb_dataset_name": task.metadata_dict["name"],
                 }
                 for split in task_eval_splits:
                     tick = time()
                     results = task.evaluate(
                         model, split, output_folder=output_folder, **kwargs
                     )
```

### Comparing `mteb-1.5.0/mteb/evaluation/evaluators/BitextMiningEvaluator.py` & `mteb-1.5.1/mteb/evaluation/evaluators/BitextMiningEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/evaluation/evaluators/ClassificationEvaluator.py` & `mteb-1.5.1/mteb/evaluation/evaluators/ClassificationEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/evaluation/evaluators/ClusteringEvaluator.py` & `mteb-1.5.1/mteb/evaluation/evaluators/ClusteringEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/evaluation/evaluators/Evaluator.py` & `mteb-1.5.1/mteb/evaluation/evaluators/Evaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/evaluation/evaluators/PairClassificationEvaluator.py` & `mteb-1.5.1/mteb/evaluation/evaluators/PairClassificationEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/evaluation/evaluators/RerankingEvaluator.py` & `mteb-1.5.1/mteb/evaluation/evaluators/RerankingEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/evaluation/evaluators/RetrievalEvaluator.py` & `mteb-1.5.1/mteb/evaluation/evaluators/RetrievalEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/evaluation/evaluators/STSEvaluator.py` & `mteb-1.5.1/mteb/evaluation/evaluators/STSEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/evaluation/evaluators/SummarizationEvaluator.py` & `mteb-1.5.1/mteb/evaluation/evaluators/SummarizationEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/evaluation/evaluators/utils.py` & `mteb-1.5.1/mteb/evaluation/evaluators/utils.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/logging.py` & `mteb-1.5.1/mteb/logging.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/BitextMining/da/BornholmskBitextMining.py` & `mteb-1.5.1/mteb/tasks/BitextMining/da/BornholmskBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/BitextMining/multilingual/BUCCBitextMining.py` & `mteb-1.5.1/mteb/tasks/BitextMining/multilingual/BUCCBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/BitextMining/multilingual/DiaBLaBitextMining.py` & `mteb-1.5.1/mteb/tasks/BitextMining/multilingual/DiaBLaBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/BitextMining/multilingual/FloresBitextMining.py` & `mteb-1.5.1/mteb/tasks/BitextMining/multilingual/FloresBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/BitextMining/multilingual/NorwegianCourtsBitextMining.py` & `mteb-1.5.1/mteb/tasks/BitextMining/multilingual/NorwegianCourtsBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/BitextMining/multilingual/TatoebaBitextMining.py` & `mteb-1.5.1/mteb/tasks/BitextMining/multilingual/TatoebaBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/BitextMining/nb/norwegian_courts_bitext_mining.py` & `mteb-1.5.1/mteb/tasks/BitextMining/nb/norwegian_courts_bitext_mining.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 
 class NorwegianCourtsBitextMining(AbsTaskBitextMining):
     metadata = TaskMetadata(
         name="NorwegianCourtsBitextMining",
         dataset={
-            "path": "kaedrodrur/norwegian-courts",
+            "path": "kardosdrur/norwegian-courts",
             "revision": "d79af07e969a6678fcbbe819956840425816468f",
         },
         description="Nynorsk and Bokmål parallel corpus from Norwegian courts. ",
         reference="https://opus.nlpl.eu/ELRC-Courts_Norway-v1.php",
         type="BitextMining",
         category="s2s",
         eval_splits=["test"],
```

### Comparing `mteb-1.5.0/mteb/tasks/Classification/__init__.py` & `mteb-1.5.1/mteb/tasks/Classification/__init__.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Classification/da/AngryTweetsClassification.py` & `mteb-1.5.1/mteb/tasks/Classification/da/AngryTweetsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Classification/da/DKHateClassification.py` & `mteb-1.5.1/mteb/tasks/Classification/da/DKHateClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Classification/da/DalajClassification.py` & `mteb-1.5.1/mteb/tasks/Classification/da/DalajClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Classification/da/DanishPoliticalCommentsClassification.py` & `mteb-1.5.1/mteb/tasks/Classification/da/DanishPoliticalCommentsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Classification/da/DdiscoCohesionClassification.py` & `mteb-1.5.1/mteb/tasks/Classification/da/DdiscoCohesionClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Classification/da/LccSentimentClassification.py` & `mteb-1.5.1/mteb/tasks/Classification/da/LccSentimentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Classification/en/AmazonPolarityClassification.py` & `mteb-1.5.1/mteb/tasks/Classification/en/AmazonPolarityClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Classification/en/Banking77Classification.py` & `mteb-1.5.1/mteb/tasks/Classification/en/Banking77Classification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Classification/en/EmotionClassification.py` & `mteb-1.5.1/mteb/tasks/Classification/en/EmotionClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Classification/en/ImdbClassification.py` & `mteb-1.5.1/mteb/tasks/Classification/en/ImdbClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Classification/en/ToxicConversationsClassification.py` & `mteb-1.5.1/mteb/tasks/Classification/en/ToxicConversationsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Classification/en/TweetSentimentExtractionClassification.py` & `mteb-1.5.1/mteb/tasks/Classification/en/TweetSentimentExtractionClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Classification/multilingual/AmazonCounterfactualClassification.py` & `mteb-1.5.1/mteb/tasks/Classification/multilingual/AmazonCounterfactualClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Classification/multilingual/AmazonReviewsClassification.py` & `mteb-1.5.1/mteb/tasks/Classification/multilingual/AmazonReviewsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Classification/multilingual/MTOPDomainClassification.py` & `mteb-1.5.1/mteb/tasks/Classification/multilingual/MTOPDomainClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Classification/multilingual/MTOPIntentClassification.py` & `mteb-1.5.1/mteb/tasks/Classification/multilingual/MTOPIntentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Classification/multilingual/MasakhaNEWSClassification.py` & `mteb-1.5.1/mteb/tasks/Classification/multilingual/MasakhaNEWSClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Classification/multilingual/MassiveIntentClassification.py` & `mteb-1.5.1/mteb/tasks/Classification/multilingual/MassiveIntentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Classification/multilingual/MassiveScenarioClassification.py` & `mteb-1.5.1/mteb/tasks/Classification/multilingual/MassiveScenarioClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Classification/multilingual/NordicLangClassification.py` & `mteb-1.5.1/mteb/tasks/Classification/multilingual/NordicLangClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Classification/multilingual/ScalaClassification.py` & `mteb-1.5.1/mteb/tasks/Classification/multilingual/ScalaClassification.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 
 class ScalaDaClassification(AbsTaskClassification):
     metadata = TaskMetadata(
         name="ScalaDaClassification",
         description="A modified version of DDT modified for linguistic acceptability classification",
         reference="https://aclanthology.org/2023.nodalida-1.20/",
         dataset={
-            "path": "ScandEval/scala-da",
-            "revision": "1de08520a7b361e92ffa2a2201ebd41942c54675",
+            "path": "mteb/scala_da_classification",
+            "revision": "e60a77795ed5488fb7a03751cf6f2b026fa27a71",
         },
         type="Classification",
         category="s2s",
         eval_splits=["test"],
         eval_langs=["da"],
         main_score="accuracy",
         date=None,
@@ -50,16 +50,16 @@
 
 class ScalaNbClassification(AbsTaskClassification):
     metadata = TaskMetadata(
         name="ScalaNbClassification",
         description="A Norwegian dataset for linguistic acceptability classification for Bokmål",
         reference="https://aclanthology.org/2023.nodalida-1.20/",
         dataset={
-            "path": "ScandEval/scala-nb",
-            "revision": "237111a078ad5a834a55c57803d40bbe410ed03b",
+            "path": "mteb/scala_nb_classification",
+            "revision": "dda7af4696bd8d5150441908ea8ed6e68a357c13",
         },
         type="Classification",
         category="s2s",
         eval_splits=["test"],
         eval_langs=["nb"],
         main_score="accuracy",
         date=None,
@@ -94,16 +94,16 @@
 
 class ScalaNnClassification(AbsTaskClassification):
     metadata = TaskMetadata(
         name="ScalaNnClassification",
         description="A Norwegian dataset for linguistic acceptability classification for Nynorsk",
         reference="https://aclanthology.org/2023.nodalida-1.20/",
         dataset={
-            "path": "ScandEval/scala-nn",
-            "revision": "9d9a2a4092ed3cacf0744592f6d2f32ab8ef4c0b",
+            "path": "mteb/scala_nn_classification",
+            "revision": "d81637ad324afb995ae395a87055380e8118a9c0",
         },
         type="Classification",
         category="s2s",
         eval_splits=["test"],
         eval_langs=["nn"],
         main_score="accuracy",
         date=None,
@@ -138,16 +138,16 @@
 
 class ScalaSvClassification(AbsTaskClassification):
     metadata = TaskMetadata(
         name="ScalaSvClassification",
         description="A Swedish dataset for linguistic acceptability classification",
         reference="https://aclanthology.org/2023.nodalida-1.20/",
         dataset={
-            "path": "ScandEval/scala-sv",
-            "revision": "1b48e3dcb02872335ff985ff938a054a4ed99008",
+            "path": "mteb/scala_sv_classification",
+            "revision": "aded78beae37445bf3917102d0b332049cfc8c99",
         },
         type="Classification",
         category="s2s",
         eval_splits=["test"],
         eval_langs=["sv"],
         main_score="accuracy",
         date=None,
```

### Comparing `mteb-1.5.0/mteb/tasks/Classification/nb/NoRecClassification.py` & `mteb-1.5.1/mteb/tasks/Classification/nb/NoRecClassification.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 class NoRecClassification(AbsTaskClassification):
     metadata = TaskMetadata(
         name="NoRecClassification",
         description="A Norwegian dataset for sentiment classification on review",
         reference="https://aclanthology.org/L18-1661/",
         dataset={
             # using the mini version to keep results ~comparable to the ScandEval benchmark
-            "path": "ScandEval/norec-mini",
-            "revision": "07b99ab3363c2e7f8f87015b01c21f4d9b917ce3",
+            "path": "mteb/norec_classification",
+            "revision": "5b740b7c42c73d586420812a35745fc37118862f",
         },
         type="Classification",
         category="s2s",
         eval_splits=["test"],
         eval_langs=["nb"],
         main_score="accuracy",
         date=None,
```

### Comparing `mteb-1.5.0/mteb/tasks/Classification/nb/NorwegianParliamentClassification.py` & `mteb-1.5.1/mteb/tasks/Classification/nb/NorwegianParliamentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Classification/pl/PolishClassification.py` & `mteb-1.5.1/mteb/tasks/Classification/pl/PolishClassification.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 class CbdClassification(AbsTaskClassification):
     metadata = TaskMetadata(
         name="CBD",
         description="Polish Tweets annotated for cyberbullying detection.",
         reference="http://2019.poleval.pl/files/poleval2019.pdf",
         dataset={
             "path": "PL-MTEB/cbd",
-            "revision": "59d12749a3c91a186063c7d729ec392fda94681c",
+            "revision": "36ddb419bcffe6a5374c3891957912892916f28d",
         },
         type="Classification",
         category="s2s",
         eval_splits=["test"],
         eval_langs=["pl"],
         main_score="accuracy",
         date=None,
@@ -38,15 +38,15 @@
     metadata = TaskMetadata(
         name="PolEmo2.0-IN",
         description="A collection of Polish online reviews from four domains: medicine, hotels, products and "
         "school. The PolEmo2.0-IN task is to predict the sentiment of in-domain (medicine and hotels) reviews.",
         reference="https://aclanthology.org/K19-1092.pdf",
         dataset={
             "path": "PL-MTEB/polemo2_in",
-            "revision": "9e9b1f8ef51616073f47f306f7f47dd91663f86a",
+            "revision": "d90724373c70959f17d2331ad51fb60c71176b03",
         },
         type="Classification",
         category="s2s",
         eval_splits=["test"],
         eval_langs=["pl"],
         main_score="accuracy",
         date=None,
@@ -69,15 +69,15 @@
         name="PolEmo2.0-OUT",
         description="A collection of Polish online reviews from four domains: medicine, hotels, products and "
         "school. The PolEmo2.0-OUT task is to predict the sentiment of out-of-domain (products and "
         "school) reviews using models train on reviews from medicine and hotels domains.",
         reference="https://aclanthology.org/K19-1092.pdf",
         dataset={
             "path": "PL-MTEB/polemo2_out",
-            "revision": "c99d599f0a6ab9b85b065da6f9d94f9cf731679f",
+            "revision": "6a21ab8716e255ab1867265f8b396105e8aa63d4",
         },
         type="Classification",
         category="s2s",
         eval_splits=["test"],
         eval_langs=["pl"],
         main_score="accuracy",
         date=None,
@@ -98,15 +98,15 @@
 class AllegroReviewsClassification(AbsTaskClassification):
     metadata = TaskMetadata(
         name="AllegroReviews",
         description="A Polish dataset for sentiment classification on reviews from e-commerce marketplace Allegro.",
         reference="https://aclanthology.org/2020.acl-main.111.pdf",
         dataset={
             "path": "PL-MTEB/allegro-reviews",
-            "revision": "477b8bd4448b5ef8ed01ba82bf9ff67f6e109207",
+            "revision": "b89853e6de927b0e3bfa8ecc0e56fe4e02ceafc6",
         },
         type="Classification",
         category="s2s",
         eval_splits=["test"],
         eval_langs=["pl"],
         main_score="accuracy",
         date=None,
@@ -127,15 +127,15 @@
 class PacClassification(AbsTaskClassification):
     metadata = TaskMetadata(
         name="PAC",
         description="Polish Paraphrase Corpus",
         reference="https://arxiv.org/pdf/2211.13112.pdf",
         dataset={
             "path": "laugustyniak/abusive-clauses-pl",
-            "revision": "8a04d940a42cd40658986fdd8e3da561533a3646",
+            "revision": "fc69d1c153a8ccdcf1eef52f4e2a27f88782f543",
         },
         type="Classification",
         category="p2p",
         eval_splits=["test"],
         eval_langs=["pl"],
         main_score="accuracy",
         date=None,
```

### Comparing `mteb-1.5.0/mteb/tasks/Classification/sv/SweRecClassification.py` & `mteb-1.5.1/mteb/tasks/Retrieval/en/DBPediaRetrieval.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 from __future__ import annotations
 
-from mteb.abstasks import AbsTaskClassification
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
+from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
 
-class SweRecClassification(AbsTaskClassification):
+
+class DBPedia(AbsTaskRetrieval):
     metadata = TaskMetadata(
-        name="SweRecClassification",
-        description="A Swedish dataset for sentiment classification on review",
-        reference="https://aclanthology.org/2023.nodalida-1.20/",
+        name="DBPedia",
+        description="DBpedia-Entity is a standard test collection for entity search over the DBpedia knowledge base",
+        reference="https://github.com/iai-group/DBpedia-Entity/",
         dataset={
-            "path": "SweRecClassification",
-            "revision": "3c62f26bafdc4c4e1c16401ad4b32f0a94b46612",
+            "path": "mteb/dbpedia",
+            "revision": "c0f706b76e590d620bd6618b3ca8efdd34e2d659",
         },
-        type="Classification",
-        category="s2s",
-        eval_splits=["test"],
-        eval_langs=["sv"],
-        main_score="accuracy",
+        type="Retrieval",
+        category="s2p",
+        eval_splits=["dev", "test"],
+        eval_langs=["en"],
+        main_score="ndcg_at_10",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
         dialect=None,
         text_creation=None,
         bibtex_citation=None,
-        n_samples={"test": 1024},
-        avg_character_length={"test": 318.8},
+        n_samples=None,
+        avg_character_length=None,
     )
```

### Comparing `mteb-1.5.0/mteb/tasks/Classification/zh/CMTEBClassification.py` & `mteb-1.5.1/mteb/tasks/Classification/zh/CMTEBClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Clustering/__init__.py` & `mteb-1.5.1/mteb/tasks/Clustering/__init__.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Clustering/de/BlurbsClusteringP2P.py` & `mteb-1.5.1/mteb/tasks/Clustering/de/BlurbsClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Clustering/de/BlurbsClusteringS2S.py` & `mteb-1.5.1/mteb/tasks/Clustering/en/RedditClustering.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskClustering import AbsTaskClustering
 
 
-class BlurbsClusteringS2S(AbsTaskClustering):
+class RedditClustering(AbsTaskClustering):
     metadata = TaskMetadata(
-        name="BlurbsClusteringS2S",
-        description="Clustering of book titles. Clustering of 28 sets, either on the main or secondary genre.",
-        reference="https://www.inf.uni-hamburg.de/en/inst/ab/lt/resources/data/germeval-2019-hmc.html",
+        name="RedditClustering",
+        description="Clustering of titles from 199 subreddits. Clustering of 25 sets, each with 10-50 classes, and each class with 100 - 1000 sentences.",
+        reference="https://arxiv.org/abs/2104.07081",
         dataset={
-            "path": "slvnwhrl/blurbs-clustering-s2s",
-            "revision": "5bfd9ee0ae3d2ef0d9a0e0bd0c3b2d0",
+            "path": "mteb/reddit-clustering",
+            "revision": "24640382cdbf8abc73003fb0fa6d111a705499eb",
         },
         type="Clustering",
         category="s2s",
         eval_splits=["test"],
-        eval_langs=["de"],
+        eval_langs=["en"],
         main_score="v_measure",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
         dialect=None,
         text_creation=None,
         bibtex_citation=None,
-        n_samples={"test": 174637},
-        avg_character_length={"test": 23.02},
+        n_samples={"test": 420464},
+        avg_character_length={"test": 64.7},
     )
```

### Comparing `mteb-1.5.0/mteb/tasks/Clustering/de/TenKGnadClusteringP2P.py` & `mteb-1.5.1/mteb/tasks/Clustering/de/TenKGnadClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Clustering/de/TenKGnadClusteringS2S.py` & `mteb-1.5.1/mteb/tasks/Clustering/de/TenKGnadClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Clustering/en/ArxivClusteringP2P.py` & `mteb-1.5.1/mteb/tasks/Clustering/en/ArxivClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Clustering/en/ArxivClusteringS2S.py` & `mteb-1.5.1/mteb/tasks/Clustering/en/ArxivClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Clustering/en/BigPatentClustering.py` & `mteb-1.5.1/mteb/tasks/Clustering/en/BigPatentClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Clustering/en/BiorxivClusteringP2P.py` & `mteb-1.5.1/mteb/tasks/Clustering/en/BiorxivClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Clustering/en/BiorxivClusteringS2S.py` & `mteb-1.5.1/mteb/tasks/Clustering/en/BiorxivClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Clustering/en/MedrxivClusteringP2P.py` & `mteb-1.5.1/mteb/tasks/Clustering/en/MedrxivClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Clustering/en/MedrxivClusteringS2S.py` & `mteb-1.5.1/mteb/tasks/Clustering/en/MedrxivClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Clustering/en/RedditClustering.py` & `mteb-1.5.1/mteb/tasks/Clustering/en/StackExchangeClustering.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskClustering import AbsTaskClustering
 
 
-class RedditClustering(AbsTaskClustering):
+class StackExchangeClustering(AbsTaskClustering):
     metadata = TaskMetadata(
-        name="RedditClustering",
-        description="Clustering of titles from 199 subreddits. Clustering of 25 sets, each with 10-50 classes, and each class with 100 - 1000 sentences.",
+        name="StackExchangeClustering",
+        description="Clustering of titles from 121 stackexchanges. Clustering of 25 sets, each with 10-50 classes, and each class with 100 - 1000 sentences.",
         reference="https://arxiv.org/abs/2104.07081",
         dataset={
-            "path": "mteb/reddit-clustering",
-            "revision": "24640382cdbf8abc73003fb0fa6d111a705499eb",
+            "path": "mteb/stackexchange-clustering",
+            "revision": "6cbc1f7b2bc0622f2e39d2c77fa502909748c259",
         },
         type="Clustering",
         category="s2s",
         eval_splits=["test"],
         eval_langs=["en"],
         main_score="v_measure",
         date=None,
@@ -25,10 +25,10 @@
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
         dialect=None,
         text_creation=None,
         bibtex_citation=None,
-        n_samples={"test": 420464},
-        avg_character_length={"test": 64.7},
+        n_samples={"test": 373850},
+        avg_character_length={"test": 57.0},
     )
```

### Comparing `mteb-1.5.0/mteb/tasks/Clustering/en/RedditClusteringP2P.py` & `mteb-1.5.1/mteb/tasks/Clustering/en/RedditClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Clustering/en/StackExchangeClustering.py` & `mteb-1.5.1/mteb/tasks/Clustering/en/WikiCitiesClustering.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskClustering import AbsTaskClustering
 
 
-class StackExchangeClustering(AbsTaskClustering):
+class WikiCitiesClustering(AbsTaskClustering):
     metadata = TaskMetadata(
-        name="StackExchangeClustering",
-        description="Clustering of titles from 121 stackexchanges. Clustering of 25 sets, each with 10-50 classes, and each class with 100 - 1000 sentences.",
-        reference="https://arxiv.org/abs/2104.07081",
+        name="WikiCitiesClustering",
+        description="Clustering of Wikipedia articles of cities by country from https://huggingface.co/datasets/wikipedia. Test set includes 126 countries, and a total of 3531 cities.",
+        reference="https://huggingface.co/datasets/wikipedia",
         dataset={
-            "path": "mteb/stackexchange-clustering",
-            "revision": "6cbc1f7b2bc0622f2e39d2c77fa502909748c259",
+            "path": "jinaai/cities_wiki_clustering",
+            "revision": "ddc9ee9242fa65332597f70e967ecc38b9d734fa",
         },
         type="Clustering",
-        category="s2s",
+        category="p2p",
         eval_splits=["test"],
         eval_langs=["en"],
         main_score="v_measure",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
         dialect=None,
         text_creation=None,
         bibtex_citation=None,
-        n_samples={"test": 373850},
-        avg_character_length={"test": 57.0},
+        n_samples=None,
+        avg_character_length=None,
     )
```

### Comparing `mteb-1.5.0/mteb/tasks/Clustering/en/StackExchangeClusteringP2P.py` & `mteb-1.5.1/mteb/tasks/Clustering/en/StackExchangeClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Clustering/en/TwentyNewsgroupsClustering.py` & `mteb-1.5.1/mteb/tasks/Clustering/en/TwentyNewsgroupsClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Clustering/en/WikiCitiesClustering.py` & `mteb-1.5.1/mteb/tasks/Clustering/es/FloresClusteringS2S.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskClustering import AbsTaskClustering
 
 
-class WikiCitiesClustering(AbsTaskClustering):
+class FloresClusteringS2S(AbsTaskClustering):
     metadata = TaskMetadata(
-        name="WikiCitiesClustering",
-        description="Clustering of Wikipedia articles of cities by country from https://huggingface.co/datasets/wikipedia. Test set includes 126 countries, and a total of 3531 cities.",
-        reference="https://huggingface.co/datasets/wikipedia",
+        name="FloresClusteringS2S",
+        description="Clustering of sentences from various web articles, 32 topics in total.",
+        reference="https://huggingface.co/datasets/facebook/flores",
         dataset={
-            "path": "jinaai/cities_wiki_clustering",
-            "revision": "ddc9ee9242fa65332597f70e967ecc38b9d734fa",
+            "path": "facebook/flores",
+            "revision": "2db78afdeaccaedc3b33a95442a4e55766887e17",
         },
         type="Clustering",
-        category="p2p",
+        category="s2s",
         eval_splits=["test"],
-        eval_langs=["en"],
+        eval_langs=["es"],
         main_score="v_measure",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
```

### Comparing `mteb-1.5.0/mteb/tasks/Clustering/es/FloresClusteringS2S.py` & `mteb-1.5.1/mteb/tasks/Retrieval/en/CQADupstackWordpressRetrieval.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
-from ....abstasks.AbsTaskClustering import AbsTaskClustering
+from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
 
 
-class FloresClusteringS2S(AbsTaskClustering):
+class CQADupstackWordpressRetrieval(AbsTaskRetrieval):
     metadata = TaskMetadata(
-        name="FloresClusteringS2S",
-        description="Clustering of sentences from various web articles, 32 topics in total.",
-        reference="https://huggingface.co/datasets/facebook/flores",
+        name="CQADupstackWordpressRetrieval",
         dataset={
-            "path": "mteb/flores",
-            "revision": "480b580487f53a46f881354a8348335d4edbb2de",
+            "path": "mteb/cqadupstack-wordpress",
+            "revision": "4ffe81d471b1924886b33c7567bfb200e9eec5c4",
         },
-        type="Clustering",
-        category="s2s",
+        description="CQADupStack: A Benchmark Data Set for Community Question-Answering Research",
+        reference="http://nlp.cis.unimelb.edu.au/resources/cqadupstack/",
+        type="Retrieval",
+        category="s2p",
         eval_splits=["test"],
-        eval_langs=["es"],
-        main_score="v_measure",
+        eval_langs=["en"],
+        main_score="ndcg_at_10",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
```

### Comparing `mteb-1.5.0/mteb/tasks/Clustering/es/SpanishNewsClusteringP2P.py` & `mteb-1.5.1/mteb/tasks/Clustering/es/SpanishNewsClusteringP2P.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 
 class SpanishNewsClusteringP2P(AbsTaskClustering):
     metadata = TaskMetadata(
         name="SpanishNewsClusteringP2P",
         description="Clustering of news articles, 7 topics in total.",
         reference="https://www.kaggle.com/datasets/kevinmorgado/spanish-news-classification",
         dataset={
-            "path": "mteb/spanish_news_clustering",
-            "revision": "b5edc3d3d7c12c7b9f883e9da50f6732f3624142",
+            "path": "jinaai/spanish_news_clustering",
+            "revision": "bf8ca8ddc5b7da4f7004720ddf99bbe0483480e6",
         },
         type="Clustering",
         category="p2p",
         eval_splits=["test"],
         eval_langs=["es"],
         main_score="v_measure",
         date=None,
```

### Comparing `mteb-1.5.0/mteb/tasks/Clustering/fr/AlloProfClusteringP2P.py` & `mteb-1.5.1/mteb/tasks/Clustering/fr/AlloProfClusteringP2P.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 class AlloProfClusteringP2P(AbsTaskClustering):
     metadata = TaskMetadata(
         name="AlloProfClusteringP2P",
         description="Clustering of document titles and descriptions from Allo Prof dataset. Clustering of 10 sets on the document topic.",
         reference="https://huggingface.co/datasets/lyon-nlp/alloprof",
         dataset={
-            "path": "mteb/alloprof",
+            "path": "lyon-nlp/alloprof",
             "revision": "392ba3f5bcc8c51f578786c1fc3dae648662cb9b",
             "name": "documents",
         },
         type="Clustering",
         category="p2p",
         eval_splits=["test"],
         eval_langs=["fr"],
```

### Comparing `mteb-1.5.0/mteb/tasks/Clustering/fr/AlloProfClusteringS2S.py` & `mteb-1.5.1/mteb/tasks/Clustering/fr/HALClusteringS2S.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,23 +4,22 @@
 import numpy as np
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskClustering import AbsTaskClustering
 
 
-class AlloProfClusteringS2S(AbsTaskClustering):
+class HALClusteringS2S(AbsTaskClustering):
     metadata = TaskMetadata(
-        name="AlloProfClusteringS2S",
-        description="Clustering of document titles from Allo Prof dataset. Clustering of 10 sets on the document topic.",
-        reference="https://huggingface.co/datasets/lyon-nlp/alloprof",
+        name="HALClusteringS2S",
+        description="Clustering of titles from HAL (https://huggingface.co/datasets/lyon-nlp/clustering-hal-s2s)",
+        reference="https://huggingface.co/datasets/lyon-nlp/clustering-hal-s2s",
         dataset={
-            "path": "mteb/alloprof",
-            "revision": "392ba3f5bcc8c51f578786c1fc3dae648662cb9b",
-            "name": "documents",
+            "path": "lyon-nlp/clustering-hal-s2s",
+            "revision": "e06ebbbb123f8144bef1a5d18796f3dec9ae2915",
         },
         type="Clustering",
         category="s2s",
         eval_splits=["test"],
         eval_langs=["fr"],
         main_score="v_measure",
         date=None,
@@ -37,17 +36,15 @@
         avg_character_length=None,
     )
 
     def dataset_transform(self):
         """
         Convert to standard format
         """
-        self.dataset = self.dataset.remove_columns("uuid")
-        self.dataset = self.dataset.remove_columns("text")
-        titles = self.dataset["documents"]["title"]
-        topics = self.dataset["documents"]["topic"]
+        self.dataset = self.dataset.remove_columns("hal_id")
+        titles = self.dataset["test"]["title"]
+        domains = self.dataset["test"]["domain"]
         new_format = {
             "sentences": [split.tolist() for split in np.array_split(titles, 10)],
-            "labels": [split.tolist() for split in np.array_split(topics, 10)],
+            "labels": [split.tolist() for split in np.array_split(domains, 10)],
         }
         self.dataset["test"] = datasets.Dataset.from_dict(new_format)
-        self.dataset.pop("documents")
```

### Comparing `mteb-1.5.0/mteb/tasks/Clustering/fr/HALClusteringS2S.py` & `mteb-1.5.1/mteb/tasks/Clustering/fr/AlloProfClusteringS2S.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,22 +4,23 @@
 import numpy as np
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskClustering import AbsTaskClustering
 
 
-class HALClusteringS2S(AbsTaskClustering):
+class AlloProfClusteringS2S(AbsTaskClustering):
     metadata = TaskMetadata(
-        name="HALClusteringS2S",
-        description="Clustering of titles from HAL (https://huggingface.co/datasets/lyon-nlp/clustering-hal-s2s)",
-        reference="https://huggingface.co/datasets/lyon-nlp/clustering-hal-s2s",
+        name="AlloProfClusteringS2S",
+        description="Clustering of document titles from Allo Prof dataset. Clustering of 10 sets on the document topic.",
+        reference="https://huggingface.co/datasets/lyon-nlp/alloprof",
         dataset={
-            "path": "mteb/hal",
-            "revision": "e06ebbbb123f8144bef1a5d18796f3dec9ae2915",
+            "path": "lyon-nlp/alloprof",
+            "revision": "392ba3f5bcc8c51f578786c1fc3dae648662cb9b",
+            "name": "documents",
         },
         type="Clustering",
         category="s2s",
         eval_splits=["test"],
         eval_langs=["fr"],
         main_score="v_measure",
         date=None,
@@ -36,15 +37,17 @@
         avg_character_length=None,
     )
 
     def dataset_transform(self):
         """
         Convert to standard format
         """
-        self.dataset = self.dataset.remove_columns("hal_id")
-        titles = self.dataset["test"]["title"]
-        domains = self.dataset["test"]["domain"]
+        self.dataset = self.dataset.remove_columns("uuid")
+        self.dataset = self.dataset.remove_columns("text")
+        titles = self.dataset["documents"]["title"]
+        topics = self.dataset["documents"]["topic"]
         new_format = {
             "sentences": [split.tolist() for split in np.array_split(titles, 10)],
-            "labels": [split.tolist() for split in np.array_split(domains, 10)],
+            "labels": [split.tolist() for split in np.array_split(topics, 10)],
         }
         self.dataset["test"] = datasets.Dataset.from_dict(new_format)
+        self.dataset.pop("documents")
```

### Comparing `mteb-1.5.0/mteb/tasks/Clustering/fr/MLSUMClusteringP2P.py` & `mteb-1.5.1/mteb/tasks/Clustering/fr/MLSUMClusteringP2P.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 class MLSUMClusteringP2P(AbsTaskClustering):
     metadata = TaskMetadata(
         name="MLSUMClusteringP2P",
         description="Clustering of newspaper article contents and titles from MLSUM dataset. Clustering of 10 sets on the newpaper article topics.",
         reference="https://huggingface.co/datasets/mlsum",
         dataset={
-            "path": "mteb/mlsum",
+            "path": "mlsum",
             "revision": "b5d54f8f3b61ae17845046286940f03c6bc79bc7",
             "name": "fr",
             "split": "test",
         },
         type="Clustering",
         category="p2p",
         eval_splits=["test"],
```

### Comparing `mteb-1.5.0/mteb/tasks/Clustering/fr/MLSUMClusteringS2S.py` & `mteb-1.5.1/mteb/tasks/Clustering/fr/MLSUMClusteringS2S.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 class MLSUMClusteringS2S(AbsTaskClustering):
     metadata = TaskMetadata(
         name="MLSUMClusteringS2S",
         description="Clustering of newspaper article contents and titles from MLSUM dataset. Clustering of 10 sets on the newpaper article topics.",
         reference="https://huggingface.co/datasets/mlsum",
         dataset={
-            "path": "mteb/mlsum",
+            "path": "mlsum",
             "revision": "b5d54f8f3b61ae17845046286940f03c6bc79bc7",
             "name": "fr",
             "split": "test",
         },
         type="Clustering",
         category="s2s",
         eval_splits=["test"],
```

### Comparing `mteb-1.5.0/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringP2P.py` & `mteb-1.5.1/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringP2P.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 class MasakhaNEWSClusteringP2P(AbsTaskClustering, MultilingualTask):
     metadata = TaskMetadata(
         name="MasakhaNEWSClusteringP2P",
         description="Clustering of news article headlines and texts from MasakhaNEWS dataset. Clustering of 10 sets on the news article label.",
         reference="https://huggingface.co/datasets/masakhane/masakhanews",
         dataset={
-            "path": "mteb/masakhanews",
+            "path": "masakhane/masakhanews",
             "revision": "8ccc72e69e65f40c70e117d8b3c08306bb788b60",
         },
         type="Clustering",
         category="p2p",
         eval_splits=["test"],
         eval_langs=_LANGUAGES,
         main_score="v_measure",
```

### Comparing `mteb-1.5.0/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringS2S.py` & `mteb-1.5.1/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Clustering/nb/snl_clustering.py` & `mteb-1.5.1/mteb/tasks/Clustering/nb/snl_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Clustering/nb/vg_clustering.py` & `mteb-1.5.1/mteb/tasks/Clustering/nb/vg_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Clustering/pl/PolishClustering.py` & `mteb-1.5.1/mteb/tasks/Clustering/pl/PolishClustering.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 class EightTagsClustering(AbsTaskClustering):
     metadata = TaskMetadata(
         name="EightTagsClustering",
         description="Clustering of headlines from social media posts in Polish belonging to 8 categories: film, history, "
         "food, medicine, motorization, work, sport and technology.",
         reference="https://aclanthology.org/2020.lrec-1.207.pdf",
         dataset={
-            "path": "mteb/polish-clustering",
-            "revision": "e7a26af6f3ae46b30dde8737f02c07b1505bcc73",
+            "path": "PL-MTEB/8tags-clustering",
+            "revision": "78b962b130c6690659c65abf67bf1c2f030606b6",
         },
         type="Clustering",
         category="s2s",
         eval_splits=["test"],
         eval_langs=["pl"],
         main_score="v_measure",
         date=None,
```

### Comparing `mteb-1.5.0/mteb/tasks/Clustering/sv/swedn_clustering.py` & `mteb-1.5.1/mteb/tasks/Clustering/sv/swedn_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Clustering/zh/CMTEBClustering.py` & `mteb-1.5.1/mteb/tasks/Clustering/zh/CMTEBClustering.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 class CLSClusteringS2S(AbsTaskClustering):
     metadata = TaskMetadata(
         name="CLSClusteringS2S",
         description="Clustering of titles from CLS dataset. Clustering of 13 sets on the main category.",
         reference="https://arxiv.org/abs/2209.05034",
         dataset={
-            "path": "mteb/cls",
+            "path": "C-MTEB/CLSClusteringS2S",
             "revision": "e458b3f5414b62b7f9f83499ac1f5497ae2e869f",
         },
         type="Clustering",
         category="s2s",
         eval_splits=["test"],
         eval_langs=["zh"],
         main_score="v_measure",
@@ -36,15 +36,15 @@
 
 class CLSClusteringP2P(AbsTaskClustering):
     metadata = TaskMetadata(
         name="CLSClusteringP2P",
         description="Clustering of titles + abstract from CLS dataset. Clustering of 13 sets on the main category.",
         reference="https://arxiv.org/abs/2209.05034",
         dataset={
-            "path": "mteb/cls",
+            "path": "C-MTEB/CLSClusteringP2P",
             "revision": "4b6227591c6c1a73bc76b1055f3b7f3588e72476",
         },
         type="Clustering",
         category="p2p",
         eval_splits=["test"],
         eval_langs=["zh"],
         main_score="v_measure",
```

### Comparing `mteb-1.5.0/mteb/tasks/PairClassification/en/SprintDuplicateQuestionsPC.py` & `mteb-1.5.1/mteb/tasks/PairClassification/en/SprintDuplicateQuestionsPC.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/PairClassification/en/TwitterSemEval2015PC.py` & `mteb-1.5.1/mteb/tasks/PairClassification/en/TwitterSemEval2015PC.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/PairClassification/en/TwitterURLCorpusPC.py` & `mteb-1.5.1/mteb/tasks/PairClassification/en/TwitterURLCorpusPC.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/PairClassification/multilingual/OpusparcusPC.py` & `mteb-1.5.1/mteb/tasks/PairClassification/multilingual/OpusparcusPC.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/PairClassification/multilingual/PawsX.py` & `mteb-1.5.1/mteb/tasks/PairClassification/multilingual/PawsX.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/PairClassification/pl/PolishPC.py` & `mteb-1.5.1/mteb/tasks/PairClassification/pl/PolishPC.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 class SickePLPC(AbsTaskPairClassification):
     metadata = TaskMetadata(
         name="SICK-E-PL",
         dataset={
             "path": "PL-MTEB/sicke-pl-pairclassification",
-            "revision": "5c59e41555244b7e45c9a6be2d720ab4bafae558",
+            "revision": "71bba34b0ece6c56dfcf46d9758a27f7a90f17e9",
         },
         description="Polish version of SICK dataset for textual entailment.",
         reference="https://aclanthology.org/2020.lrec-1.207",
         category="s2s",
         type="PairClassification",
         eval_splits=["test"],
         eval_langs=["pl"],
@@ -35,15 +35,15 @@
 
 
 class PpcPC(AbsTaskPairClassification):
     metadata = TaskMetadata(
         name="PpcPC",
         dataset={
             "path": "PL-MTEB/ppc-pairclassification",
-            "revision": "1.0",
+            "revision": "2c7d2df57801a591f6b1e3aaf042e7a04ec7d9f2",
         },
         description="Polish Paraphrase Corpus",
         reference="https://arxiv.org/pdf/2207.12759.pdf",
         category="s2s",
         type="PairClassification",
         eval_splits=["test"],
         eval_langs=["pl"],
@@ -64,15 +64,15 @@
 
 
 class CdscePC(AbsTaskPairClassification):
     metadata = TaskMetadata(
         name="CDSC-E",
         dataset={
             "path": "PL-MTEB/cdsce-pairclassification",
-            "revision": "1.0",
+            "revision": "0a3d4aa409b22f80eb22cbf59b492637637b536d",
         },
         description="Compositional Distributional Semantics Corpus for textual entailment.",
         reference="https://aclanthology.org/P17-1073.pdf",
         category="s2s",
         type="PairClassification",
         eval_splits=["test"],
         eval_langs=["pl"],
@@ -93,15 +93,15 @@
 
 
 class PscPC(AbsTaskPairClassification):
     metadata = TaskMetadata(
         name="PSC",
         dataset={
             "path": "PL-MTEB/psc-pairclassification",
-            "revision": "1.0",
+            "revision": "d05a294af9e1d3ff2bfb6b714e08a24a6cabc669",
         },
         description="Polish Summaries Corpus",
         reference="http://www.lrec-conf.org/proceedings/lrec2014/pdf/1211_Paper.pdf",
         category="s2s",
         type="PairClassification",
         eval_splits=["test"],
         eval_langs=["pl"],
```

### Comparing `mteb-1.5.0/mteb/tasks/PairClassification/zh/CMTEBPairClassification.py` & `mteb-1.5.1/mteb/tasks/PairClassification/zh/CMTEBPairClassification.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 class Ocnli(AbsTaskPairClassification):
     metadata = TaskMetadata(
         name="Ocnli",
         description="Original Chinese Natural Language Inference dataset",
         reference="https://arxiv.org/abs/2010.05444",
         dataset={
             "path": "C-MTEB/OCNLI",
-            "revision": "7bd1ee0ae3a820d8a4b6f8a624063f8504a3564d",
+            "revision": "66e76a618a34d6d565d5538088562851e6daa7ec",
         },
         type="PairClassification",
         category="s2s",
         eval_splits=["validation", "test"],
         eval_langs=["zh"],
         main_score="accuracy",
         date=None,
```

### Comparing `mteb-1.5.0/mteb/tasks/Reranking/en/AskUbuntuDupQuestions.py` & `mteb-1.5.1/mteb/tasks/Reranking/en/AskUbuntuDupQuestions.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Reranking/en/MindSmallReranking.py` & `mteb-1.5.1/mteb/tasks/Reranking/en/MindSmallReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Reranking/en/SciDocsReranking.py` & `mteb-1.5.1/mteb/tasks/Reranking/en/SciDocsReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Reranking/en/StackOverflowDupQuestions.py` & `mteb-1.5.1/mteb/tasks/Reranking/en/StackOverflowDupQuestions.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Reranking/fr/AlloprofReranking.py` & `mteb-1.5.1/mteb/tasks/Reranking/fr/AlloprofReranking.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 
 class AlloprofReranking(AbsTaskReranking):
     metadata = TaskMetadata(
         name="AlloprofReranking",
         description="This dataset was provided by AlloProf, an organisation in Quebec, Canada offering resources and a help forum curated by a large number of teachers to students on all subjects taught from in primary and secondary school",
         reference="https://huggingface.co/datasets/antoinelb7/alloprof",
         dataset={
-            "path": "mteb/alloprof-reranking",
-            "revision": "666fdacebe0291776e86f29345663dfaf80a0db9",
+            "path": "lyon-nlp/mteb-fr-reranking-alloprof-s2p",
+            "revision": "e40c8a63ce02da43200eccb5b0846fcaa888f562",
         },
         type="Reranking",
         category="s2s",
         eval_splits=["test"],
         eval_langs=["fr"],
         main_score="map",
         date=None,
```

### Comparing `mteb-1.5.0/mteb/tasks/Reranking/fr/SyntecReranking.py` & `mteb-1.5.1/mteb/tasks/Reranking/fr/SyntecReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Reranking/multilingual/MIRACLReranking.py` & `mteb-1.5.1/mteb/tasks/Reranking/multilingual/MIRACLReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Reranking/zh/CMTEBReranking.py` & `mteb-1.5.1/mteb/tasks/Reranking/zh/CMTEBReranking.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 class CMedQAv1(AbsTaskReranking):
     metadata = TaskMetadata(
         name="CMedQAv1-reranking",
         description="Chinese community medical question answering",
         reference="https://github.com/zhangsheng93/cMedQA",
         dataset={
             "path": "C-MTEB/CMedQAv1-reranking",
-            "revision": "cd540c506dae1cf9e9a59c3e06f42030d54e7301",
+            "revision": "8d7f1e942507dac42dc58017c1a001c3717da7df",
         },
         type="Reranking",
         category="s2s",
         eval_splits=["test"],
         eval_langs=["zh"],
         main_score="map",
         date=None,
```

### Comparing `mteb-1.5.0/mteb/tasks/Retrieval/__init__.py` & `mteb-1.5.1/mteb/tasks/Retrieval/__init__.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Retrieval/da/dan_fever.py` & `mteb-1.5.1/mteb/tasks/Retrieval/da/dan_fever.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Retrieval/da/t2nord_retrieval.py` & `mteb-1.5.1/mteb/tasks/Retrieval/da/t2nord_retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Retrieval/da/twitterhjerne.py` & `mteb-1.5.1/mteb/tasks/Retrieval/da/twitterhjerne.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Retrieval/de/GerDaLIRRetrieval.py` & `mteb-1.5.1/mteb/tasks/Retrieval/de/GerDaLIRRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Retrieval/de/GermanDPRRetrieval.py` & `mteb-1.5.1/mteb/tasks/Retrieval/de/GermanDPRRetrieval.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
     metadata = TaskMetadata(
         name="GermanDPR",
         description="GermanDPR is a German Question Answering dataset for open-domain QA. It associates questions with a textual context containing the answer",
         reference="https://www.deepset.ai/germanquad",
         dataset={
             "path": "deepset/germanquad",
-            "revision": "5129d02422a66be600ac89cd3e8531b4f97d347d",
+            "revision": "fff05ceaf2ffbe5b65c7e0c57e678f7b7e1a0581",
         },
         type="Retrieval",
         category="s2p",
         eval_splits=[_EVAL_SPLIT],
         eval_langs=[_LANGUAGE],
         main_score="ndcg_at_10",
         date=None,
```

### Comparing `mteb-1.5.0/mteb/tasks/Retrieval/de/GermanQuADRetrieval.py` & `mteb-1.5.1/mteb/tasks/Retrieval/de/GermanQuADRetrieval.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 class GermanQuADRetrieval(AbsTaskRetrieval):
     metadata = TaskMetadata(
         name="GermanQuAD-Retrieval",
         description="Context Retrieval for German Question Answering",
         reference="https://www.kaggle.com/datasets/GermanQuAD",
         dataset={
-            "path": "mteb/germanquad",
+            "path": "mteb/germanquad-retrieval",
             "revision": "f5c87ae5a2e7a5106606314eef45255f03151bb3",
         },
         type="Retrieval",
         category="s2p",
         eval_splits=["test"],
         eval_langs=["de"],
         main_score="mrr_at_5",
```

### Comparing `mteb-1.5.0/mteb/tasks/Retrieval/en/ArguAnaRetrieval.py` & `mteb-1.5.1/mteb/tasks/Retrieval/en/ArguAnaRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Retrieval/en/CQADupstackAndroidRetrieval.py` & `mteb-1.5.1/mteb/tasks/Retrieval/en/CQADupstackAndroidRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Retrieval/en/CQADupstackEnglishRetrieval.py` & `mteb-1.5.1/mteb/tasks/Retrieval/en/CQADupstackEnglishRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Retrieval/en/CQADupstackGamingRetrieval.py` & `mteb-1.5.1/mteb/tasks/Retrieval/en/CQADupstackGamingRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Retrieval/en/CQADupstackGisRetrieval.py` & `mteb-1.5.1/mteb/tasks/Retrieval/en/CQADupstackGisRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Retrieval/en/CQADupstackMathematicaRetrieval.py` & `mteb-1.5.1/mteb/tasks/Retrieval/en/CQADupstackMathematicaRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Retrieval/en/CQADupstackPhysicsRetrieval.py` & `mteb-1.5.1/mteb/tasks/Retrieval/en/CQADupstackPhysicsRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Retrieval/en/CQADupstackProgrammersRetrieval.py` & `mteb-1.5.1/mteb/tasks/Retrieval/en/CQADupstackProgrammersRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Retrieval/en/CQADupstackStatsRetrieval.py` & `mteb-1.5.1/mteb/tasks/Retrieval/en/CQADupstackStatsRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Retrieval/en/CQADupstackTexRetrieval.py` & `mteb-1.5.1/mteb/tasks/Retrieval/en/CQADupstackUnixRetrieval.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
 
 
-class CQADupstackTexRetrieval(AbsTaskRetrieval):
+class CQADupstackUnixRetrieval(AbsTaskRetrieval):
     metadata = TaskMetadata(
-        name="CQADupstackTexRetrieval",
+        name="CQADupstackUnixRetrieval",
         description="CQADupStack: A Benchmark Data Set for Community Question-Answering Research",
         reference="http://nlp.cis.unimelb.edu.au/resources/cqadupstack/",
         dataset={
-            "path": "mteb/cqadupstack-tex",
+            "path": "mteb/cqadupstack-unix",
             "revision": "6c6430d3a6d36f8d2a829195bc5dc94d7e063e53",
         },
         type="Retrieval",
         category="s2p",
         eval_splits=["test"],
         eval_langs=["en"],
         main_score="ndcg_at_10",
```

### Comparing `mteb-1.5.0/mteb/tasks/Retrieval/en/CQADupstackUnixRetrieval.py` & `mteb-1.5.1/mteb/tasks/Retrieval/en/CQADupstackTexRetrieval.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
 
 
-class CQADupstackUnixRetrieval(AbsTaskRetrieval):
+class CQADupstackTexRetrieval(AbsTaskRetrieval):
     metadata = TaskMetadata(
-        name="CQADupstackUnixRetrieval",
+        name="CQADupstackTexRetrieval",
         description="CQADupStack: A Benchmark Data Set for Community Question-Answering Research",
         reference="http://nlp.cis.unimelb.edu.au/resources/cqadupstack/",
         dataset={
-            "path": "mteb/cqadupstack-unix",
-            "revision": "6c6430d3a6d36f8d2a829195bc5dc94d7e063e53",
+            "path": "mteb/cqadupstack-tex",
+            "revision": "46989137a86843e03a6195de44b09deda022eec7",
         },
         type="Retrieval",
         category="s2p",
         eval_splits=["test"],
         eval_langs=["en"],
         main_score="ndcg_at_10",
         date=None,
```

### Comparing `mteb-1.5.0/mteb/tasks/Retrieval/en/CQADupstackWebmastersRetrieval.py` & `mteb-1.5.1/mteb/tasks/Retrieval/en/CQADupstackWebmastersRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Retrieval/en/CQADupstackWordpressRetrieval.py` & `mteb-1.5.1/mteb/tasks/Retrieval/pl/NQPLRetrieval.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
 
 
-class CQADupstackWordpressRetrieval(AbsTaskRetrieval):
+class NQPL(AbsTaskRetrieval):
     metadata = TaskMetadata(
-        name="CQADupstackWordpressRetrieval",
+        name="NQ-PL",
+        description="Natural Questions: A Benchmark for Question Answering Research",
+        reference="https://ai.google.com/research/NaturalQuestions/",
         dataset={
-            "path": "mteb/cqadupstack-wordpress",
-            "revision": "4ffe81d471b1924886b33c7567bfb200e9eec5c4",
+            "path": "clarin-knext/nq-pl",
+            "revision": "f171245712cf85dd4700b06bef18001578d0ca8d",
         },
-        description="CQADupStack: A Benchmark Data Set for Community Question-Answering Research",
-        reference="http://nlp.cis.unimelb.edu.au/resources/cqadupstack/",
         type="Retrieval",
         category="s2p",
         eval_splits=["test"],
-        eval_langs=["en"],
+        eval_langs=["pl"],
         main_score="ndcg_at_10",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
```

### Comparing `mteb-1.5.0/mteb/tasks/Retrieval/en/ClimateFEVERRetrieval.py` & `mteb-1.5.1/mteb/tasks/Retrieval/en/ClimateFEVERRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Retrieval/en/DBPediaRetrieval.py` & `mteb-1.5.1/mteb/tasks/Retrieval/pl/DBPediaPLRetrieval.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
 
 
-class DBPedia(AbsTaskRetrieval):
+class DBPediaPL(AbsTaskRetrieval):
     metadata = TaskMetadata(
-        name="DBPedia",
+        name="DBPedia-PL",
         description="DBpedia-Entity is a standard test collection for entity search over the DBpedia knowledge base",
         reference="https://github.com/iai-group/DBpedia-Entity/",
         dataset={
-            "path": "mteb/dbpedia",
-            "revision": "c0f706b76e590d620bd6618b3ca8efdd34e2d659",
+            "path": "clarin-knext/dbpedia-pl",
+            "revision": "76afe41d9af165cc40999fcaa92312b8b012064a",
         },
         type="Retrieval",
         category="s2p",
-        eval_splits=["dev", "test"],
-        eval_langs=["en"],
+        eval_splits=["test"],
+        eval_langs=["pl"],
         main_score="ndcg_at_10",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
```

### Comparing `mteb-1.5.0/mteb/tasks/Retrieval/en/FEVERRetrieval.py` & `mteb-1.5.1/mteb/tasks/Retrieval/en/FEVERRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Retrieval/en/FiQA2018Retrieval.py` & `mteb-1.5.1/mteb/tasks/Retrieval/en/FiQA2018Retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Retrieval/en/HagridRetrieval.py` & `mteb-1.5.1/mteb/tasks/Retrieval/en/HagridRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Retrieval/en/HotpotQARetrieval.py` & `mteb-1.5.1/mteb/tasks/Retrieval/en/HotpotQARetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Retrieval/en/MSMARCORetrieval.py` & `mteb-1.5.1/mteb/tasks/Retrieval/en/MSMARCORetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Retrieval/en/MSMARCOv2Retrieval.py` & `mteb-1.5.1/mteb/tasks/Retrieval/en/MSMARCOv2Retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Retrieval/en/NFCorpusRetrieval.py` & `mteb-1.5.1/mteb/tasks/Retrieval/en/NFCorpusRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Retrieval/en/NQRetrieval.py` & `mteb-1.5.1/mteb/tasks/Retrieval/en/NQRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Retrieval/en/NarrativeQARetrieval.py` & `mteb-1.5.1/mteb/tasks/Retrieval/en/NarrativeQARetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Retrieval/en/QuoraRetrieval.py` & `mteb-1.5.1/mteb/tasks/Retrieval/en/QuoraRetrieval.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 class QuoraRetrieval(AbsTaskRetrieval):
     metadata = TaskMetadata(
         name="QuoraRetrieval",
         dataset={
             "path": "mteb/quora",
-            "revision": "0be27e93455051e531182b85e85e425aba12e9d4",
+            "revision": "e4e08e0b7dbe3c8700f0daef558ff32256715259",
         },
         description=(
             "QuoraRetrieval is based on questions that are marked as duplicates on the Quora platform. Given a"
             " question, find other (duplicate) questions."
         ),
         reference="https://quoradata.quora.com/First-Quora-Dataset-Release-Question-Pairs",
         type="Retrieval",
```

### Comparing `mteb-1.5.0/mteb/tasks/Retrieval/en/SCIDOCSRetrieval.py` & `mteb-1.5.1/mteb/tasks/Retrieval/pl/FiQAPLRetrieval.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
 
 
-class SCIDOCS(AbsTaskRetrieval):
+class FiQAPLRetrieval(AbsTaskRetrieval):
     metadata = TaskMetadata(
-        name="SCIDOCS",
+        name="FiQA-PL",
+        description="Financial Opinion Mining and Question Answering",
+        reference="https://sites.google.com/view/fiqa/",
         dataset={
-            "path": "mteb/scidocs",
-            "revision": "56a6d0140cf6356659e2a7c1413286a774468d44",
+            "path": "clarin-knext/fiqa-pl",
+            "revision": "2e535829717f8bf9dc829b7f911cc5bbd4e6608e",
         },
-        description=(
-            "SciDocs, a new evaluation benchmark consisting of seven document-level tasks ranging from citation"
-            " prediction, to document classification and recommendation."
-        ),
-        reference="https://allenai.org/data/scidocs",
         type="Retrieval",
         category="s2p",
         eval_splits=["test"],
-        eval_langs=["en"],
+        eval_langs=["pl"],
         main_score="ndcg_at_10",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
```

### Comparing `mteb-1.5.0/mteb/tasks/Retrieval/en/SciFactRetrieval.py` & `mteb-1.5.1/mteb/tasks/Retrieval/en/SciFactRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Retrieval/en/TRECCOVIDRetrieval.py` & `mteb-1.5.1/mteb/tasks/Retrieval/pl/TRECCOVIDPLRetrieval.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
 
 
-class TRECCOVID(AbsTaskRetrieval):
+class TRECCOVIDPL(AbsTaskRetrieval):
     metadata = TaskMetadata(
-        name="TRECCOVID",
+        name="TRECCOVID-PL",
         description="TRECCOVID is an ad-hoc search challenge based on the COVID-19 dataset containing scientific articles related to the COVID-19 pandemic.",
         reference="https://ir.nist.gov/covidSubmit/index.html",
         dataset={
-            "path": "mteb/trec-covid",
-            "revision": "1271c7809071a13532e05f25fb53511ffce77117",
+            "path": "clarin-knext/trec-covid-pl",
+            "revision": "81bcb408f33366c2a20ac54adafad1ae7e877fdd",
         },
         type="Retrieval",
         category="s2p",
         eval_splits=["test"],
-        eval_langs=["en"],
+        eval_langs=["pl"],
         main_score="ndcg_at_10",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
```

### Comparing `mteb-1.5.0/mteb/tasks/Retrieval/en/Touche2020Retrieval.py` & `mteb-1.5.1/mteb/tasks/Retrieval/en/Touche2020Retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Retrieval/es/SpanishPassageRetrievalS2P.py` & `mteb-1.5.1/mteb/tasks/Retrieval/es/SpanishPassageRetrievalS2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Retrieval/es/SpanishPassageRetrievalS2S.py` & `mteb-1.5.1/mteb/tasks/Retrieval/es/SpanishPassageRetrievalS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Retrieval/fr/AlloprofRetrieval.py` & `mteb-1.5.1/mteb/tasks/Retrieval/fr/AlloprofRetrieval.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 
 class AlloprofRetrieval(AbsTaskRetrieval):
     metadata = TaskMetadata(
         name="AlloprofRetrieval",
         description="This dataset was provided by AlloProf, an organisation in Quebec, Canada offering resources and a help forum curated by a large number of teachers to students on all subjects taught from in primary and secondary school",
         reference="https://huggingface.co/datasets/antoinelb7/alloprof",
         dataset={
-            "path": "mteb/alloprof",
-            "revision": "392ba3f5bcc8c51f578786c1fc3dae648662cb9b",
+            "path": "lyon-nlp/alloprof",
+            "revision": "2df7bee4080bedf2e97de3da6bd5c7bc9fc9c4d2",
         },
         type="Retrieval",
         category="s2p",
         eval_splits=["test"],
         eval_langs=["fr"],
         main_score="ndcg_at_10",
         date=None,
```

### Comparing `mteb-1.5.0/mteb/tasks/Retrieval/fr/BSARDRetrieval.py` & `mteb-1.5.1/mteb/tasks/Retrieval/fr/BSARDRetrieval.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 class BSARDRetrieval(AbsTaskRetrieval):
     metadata = TaskMetadata(
         name="BSARDRetrieval",
         description="The Belgian Statutory Article Retrieval Dataset (BSARD) is a French native dataset for studying legal information retrieval. BSARD consists of more than 22,600 statutory articles from Belgian law and about 1,100 legal questions posed by Belgian citizens and labeled by experienced jurists with relevant articles from the corpus.",
         reference="https://huggingface.co/datasets/maastrichtlawtech/bsard",
         dataset={
-            "path": "mteb/bsard",
+            "path": "maastrichtlawtech/bsard",
             "revision": "5effa1b9b5fa3b0f9e12523e6e43e5f86a6e6d59",
         },
         type="Retrieval",
         category="s2p",
         eval_splits=["test"],
         eval_langs=["fr"],
         main_score="ndcg_at_100",
```

### Comparing `mteb-1.5.0/mteb/tasks/Retrieval/fr/SyntecRetrieval.py` & `mteb-1.5.1/mteb/tasks/Retrieval/fr/SyntecRetrieval.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
     metadata = TaskMetadata(
         name="SyntecRetrieval",
         description="This dataset has been built from the Syntec Collective bargaining agreement.",
         reference="https://huggingface.co/datasets/lyon-nlp/mteb-fr-retrieval-syntec-s2p",
         dataset={
             "path": "lyon-nlp/mteb-fr-retrieval-syntec-s2p",
-            "revision": "b205c5084a0934ce8af14338bf03feb19499c84d",
+            "revision": "aa460cd4d177e6a3c04fcd2affd95e8243289033",
         },
         type="Retrieval",
         category="s2p",
         eval_splits=_EVAL_SPLITS,
         eval_langs=["fr"],
         main_score="map",
         date=None,
```

### Comparing `mteb-1.5.0/mteb/tasks/Retrieval/ko/KoMiracl.py` & `mteb-1.5.1/mteb/tasks/Retrieval/ko/KoMiracl.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Retrieval/ko/KoMrtydi.py` & `mteb-1.5.1/mteb/tasks/Retrieval/ko/KoMrtydi.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Retrieval/ko/KoStrategyQA.py` & `mteb-1.5.1/mteb/tasks/Retrieval/ko/KoStrategyQA.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Retrieval/multilingual/MIRACLRetrieval.py` & `mteb-1.5.1/mteb/tasks/Retrieval/multilingual/MIRACLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Retrieval/multilingual/MintakaRetrieval.py` & `mteb-1.5.1/mteb/tasks/Retrieval/multilingual/MintakaRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Retrieval/multilingual/MultiLongDocRetrieval.py` & `mteb-1.5.1/mteb/tasks/Retrieval/multilingual/MultiLongDocRetrieval.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 class MultiLongDocRetrieval(MultilingualTask, AbsTaskRetrieval):
     metadata = TaskMetadata(
         name="MultiLongDocRetrieval",
         description="MultiLongDocRetrieval",
         reference="https://arxiv.org/abs/2402.03216",
         dataset={
             "path": "Shitao/MLDR",
-            "revision": "d79af07e969a6678fcbbe819956840425816468f",
+            "revision": "d67138e705d963e346253a80e59676ddb418810a",
         },
         type="Retrieval",
         category="s2p",
         eval_splits=["dev", "test"],
         eval_langs=_LANGUAGES,
         main_score="ndcg_at_10",
         date=None,
```

### Comparing `mteb-1.5.0/mteb/tasks/Retrieval/multilingual/XMarketRetrieval.py` & `mteb-1.5.1/mteb/tasks/Retrieval/multilingual/XMarketRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Retrieval/multilingual/XPQARetrieval.py` & `mteb-1.5.1/mteb/tasks/Retrieval/multilingual/XPQARetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Retrieval/nb/norquad.py` & `mteb-1.5.1/mteb/tasks/Retrieval/nb/norquad.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from mteb.abstasks import AbsTaskRetrieval, TaskMetadata
 
 
 class NorQuadRetrieval(AbsTaskRetrieval):
     metadata = TaskMetadata(
         name="NorQuadRetrieval",
         dataset={
-            "path": "ScandEval/norquad-mini",
-            "revision": "a47881440ce4b18ef61a99be66dc4badbf5aac6e",
+            "path": "mteb/norquad_retrieval",
+            "revision": "9dcfcdb2aa578dd178330d49bf564248935f7fbe",
         },
         description="Human-created question for Norwegian wikipedia passages.",
         reference="https://aclanthology.org/2023.nodalida-1.17/",
         type="Retrieval",
         category="p2p",
         eval_splits=["test"],
         eval_langs=["nb"],
```

### Comparing `mteb-1.5.0/mteb/tasks/Retrieval/nb/snl_retrieval.py` & `mteb-1.5.1/mteb/tasks/Retrieval/nb/snl_retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Retrieval/pl/ArguAnaPLRetrieval.py` & `mteb-1.5.1/mteb/tasks/Retrieval/pl/ArguAnaPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Retrieval/pl/DBPediaPLRetrieval.py` & `mteb-1.5.1/mteb/tasks/Retrieval/pl/NFCorpusPLRetrieval.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
 
 
-class DBPediaPL(AbsTaskRetrieval):
+class NFCorpusPL(AbsTaskRetrieval):
     metadata = TaskMetadata(
-        name="DBPedia-PL",
-        description="DBpedia-Entity is a standard test collection for entity search over the DBpedia knowledge base",
-        reference="https://github.com/iai-group/DBpedia-Entity/",
+        name="NFCorpus-PL",
+        description="NFCorpus: A Full-Text Learning to Rank Dataset for Medical Information Retrieval",
+        reference="https://www.cl.uni-heidelberg.de/statnlpgroup/nfcorpus/",
         dataset={
-            "path": "clarin-knext/dbpedia-pl",
-            "revision": "76afe41d9af165cc40999fcaa92312b8b012064a",
+            "path": "clarin-knext/nfcorpus-pl",
+            "revision": "9a6f9567fda928260afed2de480d79c98bf0bec0",
         },
         type="Retrieval",
         category="s2p",
         eval_splits=["test"],
         eval_langs=["pl"],
         main_score="ndcg_at_10",
         date=None,
```

### Comparing `mteb-1.5.0/mteb/tasks/Retrieval/pl/FiQAPLRetrieval.py` & `mteb-1.5.1/mteb/tasks/Retrieval/en/SCIDOCSRetrieval.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
 
 
-class FiQAPLRetrieval(AbsTaskRetrieval):
+class SCIDOCS(AbsTaskRetrieval):
     metadata = TaskMetadata(
-        name="FiQA-PL",
-        description="Financial Opinion Mining and Question Answering",
-        reference="https://sites.google.com/view/fiqa/",
+        name="SCIDOCS",
         dataset={
-            "path": "clarin-knext/fiqa-pl",
-            "revision": "2e535829717f8bf9dc829b7f911cc5bbd4e6608e",
+            "path": "mteb/scidocs",
+            "revision": "f8c2fcf00f625baaa80f62ec5bd9e1fff3b8ae88",
         },
+        description=(
+            "SciDocs, a new evaluation benchmark consisting of seven document-level tasks ranging from citation"
+            " prediction, to document classification and recommendation."
+        ),
+        reference="https://allenai.org/data/scidocs",
         type="Retrieval",
         category="s2p",
         eval_splits=["test"],
-        eval_langs=["pl"],
+        eval_langs=["en"],
         main_score="ndcg_at_10",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
```

### Comparing `mteb-1.5.0/mteb/tasks/Retrieval/pl/HotpotQAPLRetrieval.py` & `mteb-1.5.1/mteb/tasks/Retrieval/pl/HotpotQAPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Retrieval/pl/MSMARCOPLRetrieval.py` & `mteb-1.5.1/mteb/tasks/Retrieval/pl/MSMARCOPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Retrieval/pl/NFCorpusPLRetrieval.py` & `mteb-1.5.1/mteb/tasks/Retrieval/pl/QuoraPLRetrieval.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
 
 
-class NFCorpusPL(AbsTaskRetrieval):
+class QuoraPLRetrieval(AbsTaskRetrieval):
     metadata = TaskMetadata(
-        name="NFCorpus-PL",
-        description="NFCorpus: A Full-Text Learning to Rank Dataset for Medical Information Retrieval",
-        reference="https://www.cl.uni-heidelberg.de/statnlpgroup/nfcorpus/",
+        name="Quora-PL",
+        description="QuoraRetrieval is based on questions that are marked as duplicates on the Quora platform. Given a question, find other (duplicate) questions.",
+        reference="https://quoradata.quora.com/First-Quora-Dataset-Release-Question-Pairs",
         dataset={
-            "path": "clarin-knext/nfcorpus-pl",
-            "revision": "9a6f9567fda928260afed2de480d79c98bf0bec0",
+            "path": "clarin-knext/quora-pl",
+            "revision": "0be27e93455051e531182b85e85e425aba12e9d4",
         },
         type="Retrieval",
-        category="s2p",
-        eval_splits=["test"],
+        category="s2s",
+        eval_splits=["validation", "test"],  # validation for new DataLoader
         eval_langs=["pl"],
         main_score="ndcg_at_10",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
```

### Comparing `mteb-1.5.0/mteb/tasks/Retrieval/pl/NQPLRetrieval.py` & `mteb-1.5.1/mteb/tasks/Retrieval/pl/SciFactPLRetrieval.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
 
 
-class NQPL(AbsTaskRetrieval):
+class SciFactPL(AbsTaskRetrieval):
     metadata = TaskMetadata(
-        name="NQ-PL",
-        description="Natural Questions: A Benchmark for Question Answering Research",
-        reference="https://ai.google.com/research/NaturalQuestions/",
+        name="SciFact-PL",
+        description="SciFact verifies scientific claims using evidence from the research literature containing scientific paper abstracts.",
+        reference="https://github.com/allenai/scifact",
         dataset={
-            "path": "clarin-knext/nq-pl",
-            "revision": "f171245712cf85dd4700b06bef18001578d0ca8d",
+            "path": "clarin-knext/scifact-pl",
+            "revision": "47932a35f045ef8ed01ba82bf9ff67f6e109207e",
         },
         type="Retrieval",
         category="s2p",
         eval_splits=["test"],
         eval_langs=["pl"],
         main_score="ndcg_at_10",
         date=None,
```

### Comparing `mteb-1.5.0/mteb/tasks/Retrieval/pl/QuoraPLRetrieval.py` & `mteb-1.5.1/mteb/tasks/Retrieval/en/TRECCOVIDRetrieval.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
 
 
-class QuoraPLRetrieval(AbsTaskRetrieval):
+class TRECCOVID(AbsTaskRetrieval):
     metadata = TaskMetadata(
-        name="Quora-PL",
-        description="QuoraRetrieval is based on questions that are marked as duplicates on the Quora platform. Given a question, find other (duplicate) questions.",
-        reference="https://quoradata.quora.com/First-Quora-Dataset-Release-Question-Pairs",
+        name="TRECCOVID",
+        description="TRECCOVID is an ad-hoc search challenge based on the COVID-19 dataset containing scientific articles related to the COVID-19 pandemic.",
+        reference="https://ir.nist.gov/covidSubmit/index.html",
         dataset={
-            "path": "clarin-knext/quora-pl",
-            "revision": "0be27e93455051e531182b85e85e425aba12e9d4",
+            "path": "mteb/trec-covid",
+            "revision": "bb9466bac8153a0349341eb1b22e06409e78ef4e",
         },
         type="Retrieval",
-        category="s2s",
-        eval_splits=["validation", "test"],  # validation for new DataLoader
-        eval_langs=["pl"],
+        category="s2p",
+        eval_splits=["test"],
+        eval_langs=["en"],
         main_score="ndcg_at_10",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
```

### Comparing `mteb-1.5.0/mteb/tasks/Retrieval/pl/SCIDOCSPLRetrieval.py` & `mteb-1.5.1/mteb/tasks/Retrieval/pl/SCIDOCSPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Retrieval/pl/SciFactPLRetrieval.py` & `mteb-1.5.1/mteb/tasks/Classification/sv/SweRecClassification.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 from __future__ import annotations
 
+from mteb.abstasks import AbsTaskClassification
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
-from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
 
-
-class SciFactPL(AbsTaskRetrieval):
+class SweRecClassification(AbsTaskClassification):
     metadata = TaskMetadata(
-        name="SciFact-PL",
-        description="SciFact verifies scientific claims using evidence from the research literature containing scientific paper abstracts.",
-        reference="https://github.com/allenai/scifact",
+        name="SweRecClassification",
+        description="A Swedish dataset for sentiment classification on review",
+        reference="https://aclanthology.org/2023.nodalida-1.20/",
         dataset={
-            "path": "clarin-knext/scifact-pl",
-            "revision": "47932a35f045ef8ed01ba82bf9ff67f6e109207e",
+            "path": "mteb/swerec_classification",
+            "revision": "b07c6ce548f6a7ac8d546e1bbe197a0086409190",
         },
-        type="Retrieval",
-        category="s2p",
+        type="Classification",
+        category="s2s",
         eval_splits=["test"],
-        eval_langs=["pl"],
-        main_score="ndcg_at_10",
+        eval_langs=["sv"],
+        main_score="accuracy",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
         dialect=None,
         text_creation=None,
         bibtex_citation=None,
-        n_samples=None,
-        avg_character_length=None,
+        n_samples={"test": 1024},
+        avg_character_length={"test": 318.8},
     )
```

### Comparing `mteb-1.5.0/mteb/tasks/Retrieval/pl/TRECCOVIDPLRetrieval.py` & `mteb-1.5.1/mteb/tasks/STS/en/STS16STS.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,41 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
-from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
+from ....abstasks.AbsTaskSTS import AbsTaskSTS
 
 
-class TRECCOVIDPL(AbsTaskRetrieval):
+class STS16STS(AbsTaskSTS):
     metadata = TaskMetadata(
-        name="TRECCOVID-PL",
-        description="TRECCOVID is an ad-hoc search challenge based on the COVID-19 dataset containing scientific articles related to the COVID-19 pandemic.",
-        reference="https://ir.nist.gov/covidSubmit/index.html",
+        name="STS16",
         dataset={
-            "path": "clarin-knext/trec-covid-pl",
-            "revision": "81bcb408f33366c2a20ac54adafad1ae7e877fdd",
+            "path": "mteb/sts16-sts",
+            "revision": "4d8694f8f0e0100860b497b999b3dbed754a0513",
         },
-        type="Retrieval",
-        category="s2p",
+        description="SemEval STS 2016 dataset",
+        reference="https://www.aclweb.org/anthology/S16-1001",
+        type="STS",
+        category="s2s",
         eval_splits=["test"],
-        eval_langs=["pl"],
-        main_score="ndcg_at_10",
+        eval_langs=["en"],
+        main_score="cosine_spearman",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
         dialect=None,
         text_creation=None,
         bibtex_citation=None,
         n_samples=None,
         avg_character_length=None,
     )
+
+    @property
+    def metadata_dict(self) -> dict[str, str]:
+        metadata_dict = super().metadata_dict
+        metadata_dict["min_score"] = 0
+        metadata_dict["max_score"] = 5
+        return metadata_dict
```

### Comparing `mteb-1.5.0/mteb/tasks/Retrieval/sv/swedn_retrieval.py` & `mteb-1.5.1/mteb/tasks/Retrieval/sv/swedn_retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Retrieval/sv/swefaq_retrieval.py` & `mteb-1.5.1/mteb/tasks/Retrieval/sv/swefaq_retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Retrieval/zh/CMTEBRetrieval.py` & `mteb-1.5.1/mteb/tasks/Retrieval/zh/CMTEBRetrieval.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,15 +149,15 @@
 class CovidRetrieval(AbsTaskRetrieval):
     metadata = TaskMetadata(
         name="CovidRetrieval",
         description="COVID-19 news articles",
         reference="https://arxiv.org/abs/2203.03367",
         dataset={
             "path": "C-MTEB/CovidRetrieval",
-            "revision": "687de13dc7294d6fd9be10c6945f9e8fec8166b9",
+            "revision": "1271c7809071a13532e05f25fb53511ffce77117",
         },
         type="Retrieval",
         category="s2p",
         eval_splits=["test"],
         eval_langs=["zh"],
         main_score="ndcg_at_10",
         date=None,
```

### Comparing `mteb-1.5.0/mteb/tasks/STS/__init__.py` & `mteb-1.5.1/mteb/tasks/STS/__init__.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/STS/de/GermanSTSBenchmarkSTS.py` & `mteb-1.5.1/mteb/tasks/STS/de/GermanSTSBenchmarkSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/STS/en/BiossesSTS.py` & `mteb-1.5.1/mteb/tasks/STS/en/BiossesSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/STS/en/STS12STS.py` & `mteb-1.5.1/mteb/tasks/STS/en/STS12STS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/STS/en/STS13STS.py` & `mteb-1.5.1/mteb/tasks/STS/en/STS13STS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/STS/en/STS14STS.py` & `mteb-1.5.1/mteb/tasks/STS/en/STS14STS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/STS/en/STS15STS.py` & `mteb-1.5.1/mteb/tasks/STS/en/STS15STS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/STS/en/STS16STS.py` & `mteb-1.5.1/mteb/tasks/STS/en/SickrSTS.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskSTS import AbsTaskSTS
 
 
-class STS16STS(AbsTaskSTS):
+class SickrSTS(AbsTaskSTS):
     metadata = TaskMetadata(
-        name="STS16",
+        name="SICK-R",
         dataset={
-            "path": "mteb/sts16-sts",
-            "revision": "4d8694f8f0e0100860b497b999b3dbed754a0513",
+            "path": "mteb/sickr-sts",
+            "revision": "20a6d6f312dd54037fe07a32d58e5e168867909d",
         },
-        description="SemEval STS 2016 dataset",
-        reference="https://www.aclweb.org/anthology/S16-1001",
+        description="Semantic Textual Similarity SICK-R dataset as described here:",
+        reference="https://aclanthology.org/2020.lrec-1.207",
         type="STS",
         category="s2s",
         eval_splits=["test"],
         eval_langs=["en"],
         main_score="cosine_spearman",
         date=None,
         form=None,
```

### Comparing `mteb-1.5.0/mteb/tasks/STS/en/STSBenchmarkSTS.py` & `mteb-1.5.1/mteb/tasks/STS/en/STSBenchmarkSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/STS/en/SickrSTS.py` & `mteb-1.5.1/mteb/tasks/STS/pl/PolishSTS.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,62 @@
 from __future__ import annotations
 
+from mteb.abstasks.AbsTaskSTS import AbsTaskSTS
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
-from ....abstasks.AbsTaskSTS import AbsTaskSTS
 
-
-class SickrSTS(AbsTaskSTS):
+class SickrPLSTS(AbsTaskSTS):
     metadata = TaskMetadata(
-        name="SICK-R",
+        name="SICK-R-PL",
         dataset={
-            "path": "MMathematica/sickr-sts",
-            "revision": "a6ea5a8cab320b040a23452cc28066d9beae2cee",
+            "path": "PL-MTEB/sickr-pl-sts",
+            "revision": "fd5c2441b7eeff8676768036142af4cfa42c1339",
         },
-        description="Semantic Textual Similarity SICK-R dataset as described here:",
+        description="Polish version of SICK dataset for textual relatedness.",
         reference="https://aclanthology.org/2020.lrec-1.207",
         type="STS",
         category="s2s",
         eval_splits=["test"],
-        eval_langs=["en"],
+        eval_langs=["pl"],
+        main_score="cosine_spearman",
+        date=None,
+        form=None,
+        domains=None,
+        task_subtypes=None,
+        license=None,
+        socioeconomic_status=None,
+        annotations_creators=None,
+        dialect=None,
+        text_creation=None,
+        bibtex_citation=None,
+        n_samples={"test": 9812},
+        avg_character_length={"test": 42.8},
+    )
+
+    @property
+    def metadata_dict(self) -> dict[str, str]:
+        metadata_dict = super().metadata_dict
+        metadata_dict["min_score"] = 1
+        metadata_dict["max_score"] = 5
+        return metadata_dict
+
+
+class CdscrSTS(AbsTaskSTS):
+    metadata = TaskMetadata(
+        name="CDSC-R",
+        dataset={
+            "path": "PL-MTEB/cdscr-sts",
+            "revision": "1cd6abbb00df7d14be3dbd76a7dcc64b3a79a7cd",
+        },
+        description="Compositional Distributional Semantics Corpus for textual relatedness.",
+        reference="https://aclanthology.org/P17-1073.pdf",
+        type="STS",
+        category="s2s",
+        eval_splits=["test"],
+        eval_langs=["pl"],
         main_score="cosine_spearman",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
@@ -32,10 +67,10 @@
         n_samples=None,
         avg_character_length=None,
     )
 
     @property
     def metadata_dict(self) -> dict[str, str]:
         metadata_dict = super().metadata_dict
-        metadata_dict["min_score"] = 0
+        metadata_dict["min_score"] = 1
         metadata_dict["max_score"] = 5
         return metadata_dict
```

### Comparing `mteb-1.5.0/mteb/tasks/STS/es/STSES.py` & `mteb-1.5.1/mteb/tasks/STS/es/STSES.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 from __future__ import annotations
 
-from datasets import load_dataset
-
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskSTS import AbsTaskSTS
 
 _EVAL_SPLIT = "test"
 
 
 class STSES(AbsTaskSTS):
     metadata = TaskMetadata(
         name="STSES",
         dataset={
             "path": "PlanTL-GOB-ES/sts-es",
             "revision": "0912bb6c9393c76d62a7c5ee81c4c817ff47c9f4",
-            "trust_remote_code": True
+            "trust_remote_code": True,
         },
         description="Spanish test sets from SemEval-2014 (Agirre et al., 2014) and SemEval-2015 (Agirre et al., 2015)",
         reference="https://huggingface.co/datasets/PlanTL-GOB-ES/sts-es",
         type="STS",
         category="s2s",
         eval_splits=[_EVAL_SPLIT],
         eval_langs=["es"],
@@ -45,8 +43,7 @@
         metadata_dict["max_score"] = 5
         return metadata_dict
 
     def dataset_transform(self):
         data = self.dataset[_EVAL_SPLIT]
         data = data.add_column("score", [d["label"] for d in data])
         self.dataset = {_EVAL_SPLIT: data}
-
```

### Comparing `mteb-1.5.0/mteb/tasks/STS/fr/SickFrSTS.py` & `mteb-1.5.1/mteb/tasks/STS/fr/SickFrSTS.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 from __future__ import annotations
 
-import datasets
-
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskSTS import AbsTaskSTS
 
 
 class SickFrSTS(AbsTaskSTS):
     metadata = TaskMetadata(
```

### Comparing `mteb-1.5.0/mteb/tasks/STS/multilingual/STS17CrosslingualSTS.py` & `mteb-1.5.1/mteb/tasks/STS/multilingual/STS17CrosslingualSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/STS/multilingual/STS22CrosslingualSTS.py` & `mteb-1.5.1/mteb/tasks/STS/multilingual/STS22CrosslingualSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/STS/multilingual/STSBenchmarkMultilingualSTS.py` & `mteb-1.5.1/mteb/tasks/STS/multilingual/STSBenchmarkMultilingualSTS.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 _SPLITS = ["dev", "test"]
 
 
 class STSBenchmarkMultilingualSTS(AbsTaskSTS, MultilingualTask):
     metadata = TaskMetadata(
         name="STSBenchmarkMultilingualSTS",
         dataset={
-            "path": "stsb_multi_mt",
+            "path": "PhilipMay/stsb_multi_mt",
             "revision": "93d57ef91790589e3ce9c365164337a8a78b7632",
         },
         description=(
             "Semantic Textual Similarity Benchmark (STSbenchmark) dataset,"
             "but translated using DeepL API."
         ),
         reference="https://github.com/PhilipMay/stsb-multi-mt/",
```

### Comparing `mteb-1.5.0/mteb/tasks/STS/zh/CMTEBSTS.py` & `mteb-1.5.1/mteb/tasks/STS/zh/CMTEBSTS.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 class ATEC(AbsTaskSTS):
     metadata = TaskMetadata(
         name="ATEC",
         dataset={
             "path": "C-MTEB/ATEC",
-            "revision": "0f319b1142f2ae3f7dc7be10c3c7f3598ec6c602",
+            "revision": "0f319b1142f28d00e055a6770f3f726ae9b7d865",
         },
         description="A Chinese dataset for textual relatedness",
         reference="https://aclanthology.org/2021.emnlp-main.357",
         type="STS",
         category="s2s",
         eval_splits=["validation", "test"],
         eval_langs=["zh"],
```

### Comparing `mteb-1.5.0/mteb/tasks/Summarization/en/SummEvalSummarization.py` & `mteb-1.5.1/mteb/tasks/Summarization/en/SummEvalSummarization.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/mteb/tasks/Summarization/fr/SummEvalFrSummarization.py` & `mteb-1.5.1/mteb/tasks/Summarization/fr/SummEvalFrSummarization.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 class SummEvalFrSummarization(AbsTaskSummarization):
     metadata = TaskMetadata(
         name="SummEvalFr",
         description="News Article Summary Semantic Similarity Estimation translated from english to french with DeepL.",
         reference="https://github.com/Yale-LILY/SummEval",
         dataset={
-            "path": "lyon-nlp/summeval",
+            "path": "lyon-nlp/summarization-summeval-fr-p2p",
             "revision": "b385812de6a9577b6f4d0f88c6a6e35395a94054",
         },
         type="Summarization",
         category="p2p",
         eval_splits=["test"],
         eval_langs=["fr"],
         main_score="cosine_spearman",
```

### Comparing `mteb-1.5.0/mteb.egg-info/PKG-INFO` & `mteb-1.5.1/mteb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mteb
-Version: 1.5.0
+Version: 1.5.1
 Summary: Massive Text Embedding Benchmark
 Author-email: MTEB Contributors <niklas@huggingface.co>, nouamane@huggingface.co, info@nils-reimers.de
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `mteb-1.5.0/mteb.egg-info/SOURCES.txt` & `mteb-1.5.1/mteb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/pyproject.toml` & `mteb-1.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mteb"
-version = "1.5.0"
+version = "1.5.1"
 description = "Massive Text Embedding Benchmark"
 readme = "README.md"
 authors = [
     { name = "MTEB Contributors", email = "niklas@huggingface.co" },
     { email = "nouamane@huggingface.co" },
     { email = "info@nils-reimers.de" },
 ]
```

### Comparing `mteb-1.5.0/scripts/data/amazon_polarity/create_data.py` & `mteb-1.5.1/scripts/data/amazon_polarity/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/scripts/data/amazon_reviews_multi/create_data.py` & `mteb-1.5.1/scripts/data/amazon_reviews_multi/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/scripts/data/arxiv/script_clustering.py` & `mteb-1.5.1/scripts/data/arxiv/script_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/scripts/data/arxiv/script_raw.py` & `mteb-1.5.1/scripts/data/arxiv/script_raw.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/scripts/data/biorxiv/script_clustering.py` & `mteb-1.5.1/scripts/data/biorxiv/script_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/scripts/data/biorxiv/script_raw.py` & `mteb-1.5.1/scripts/data/biorxiv/script_raw.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/scripts/data/bucc/create_data.py` & `mteb-1.5.1/scripts/data/bucc/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/scripts/data/create_task_table.py` & `mteb-1.5.1/scripts/data/create_task_table.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/scripts/data/germanquad/process_data.py` & `mteb-1.5.1/scripts/data/germanquad/process_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/scripts/data/hal/create_data.py` & `mteb-1.5.1/scripts/data/hal/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/scripts/data/imdb/create_data.py` & `mteb-1.5.1/scripts/data/imdb/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/scripts/data/medrxiv/script_clustering.py` & `mteb-1.5.1/scripts/data/medrxiv/script_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/scripts/data/medrxiv/script_raw.py` & `mteb-1.5.1/scripts/data/medrxiv/script_raw.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/scripts/data/mind/prepare_data.py` & `mteb-1.5.1/scripts/data/mind/prepare_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/scripts/data/redditp2p/script_clustering.py` & `mteb-1.5.1/scripts/data/redditp2p/script_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/scripts/data/stackexchangep2p/script_clustering.py` & `mteb-1.5.1/scripts/data/stackexchangep2p/script_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/scripts/data/sts22-crosslingual-sts/create_data.py` & `mteb-1.5.1/scripts/data/sts22-crosslingual-sts/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/scripts/data/summeval_fr/create_data.py` & `mteb-1.5.1/scripts/data/summeval_fr/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/scripts/data/toxic_conversations_50k/create_data.py` & `mteb-1.5.1/scripts/data/toxic_conversations_50k/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/scripts/merge_cqadupstack.py` & `mteb-1.5.1/scripts/merge_cqadupstack.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/scripts/mteb_meta.py` & `mteb-1.5.1/scripts/mteb_meta.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/scripts/run_mteb_chinese.py` & `mteb-1.5.1/scripts/run_mteb_chinese.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/scripts/run_mteb_english.py` & `mteb-1.5.1/scripts/run_mteb_english.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/scripts/run_mteb_french.py` & `mteb-1.5.1/scripts/run_mteb_french.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/scripts/run_mteb_german.py` & `mteb-1.5.1/scripts/run_mteb_german.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/scripts/run_mteb_korean.py` & `mteb-1.5.1/scripts/run_mteb_korean.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/scripts/run_mteb_polish.py` & `mteb-1.5.1/scripts/run_mteb_polish.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/tests/test_ClusteringEvaluator.py` & `mteb-1.5.1/tests/test_ClusteringEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/tests/test_PairClassificationEvaluator.py` & `mteb-1.5.1/tests/test_PairClassificationEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/tests/test_RerankingEvaluator.py` & `mteb-1.5.1/tests/test_RerankingEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/tests/test_RetrievalEvaluator.py` & `mteb-1.5.1/tests/test_RetrievalEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.0/tests/test_TaskMetadata.py` & `mteb-1.5.1/tests/test_TaskMetadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import logging
+
 import pytest
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
+
 def test_given_dataset_config_then_it_is_valid():
     my_task = TaskMetadata(
         name="MyTask",
         dataset={
             "path": "test/dataset",
             "revision": "1.0",
         },
@@ -84,22 +86,20 @@
             dialect=None,
             text_creation=None,
             bibtex_citation=None,
             avg_character_length=None,
             n_samples=None,
         )
 
+
 def test_given_none_revision_path_then_it_logs_warning(caplog):
     with caplog.at_level(logging.WARNING):
         my_task = TaskMetadata(
             name="MyTask",
-            dataset={
-                "path": "test/dataset",
-                "revision": None
-            },
+            dataset={"path": "test/dataset", "revision": None},
             description="testing",
             reference=None,
             type="Classification",
             category="s2s",
             eval_splits=["test"],
             eval_langs=["en"],
             main_score="map",
@@ -114,11 +114,11 @@
             text_creation=None,
             bibtex_citation=None,
             avg_character_length=None,
             n_samples=None,
         )
 
         assert my_task.dataset["revision"] is None
-        assert len([
-            record for record in caplog.records if record.levelname == "WARNING"
-        ]) == 1
-
+        assert (
+            len([record for record in caplog.records if record.levelname == "WARNING"])
+            == 1
+        )
```

