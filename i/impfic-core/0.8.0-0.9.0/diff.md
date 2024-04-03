# Comparing `tmp/impfic_core-0.8.0.tar.gz` & `tmp/impfic_core-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "impfic_core-0.8.0.tar", max compression
+gzip compressed data, was "impfic_core-0.9.0.tar", max compression
```

## Comparing `impfic_core-0.8.0.tar` & `impfic_core-0.9.0.tar`

### file list

```diff
@@ -1,34 +1,35 @@
--rw-r--r--   0        0        0     4913 2024-02-20 14:25:31.536362 impfic_core-0.8.0/README.md
--rw-r--r--   0        0        0       22 2024-03-20 12:26:48.292087 impfic_core-0.8.0/impfic_core/__init__.py
--rw-r--r--   0        0        0     1225 2024-02-21 10:47:17.314822 impfic_core-0.8.0/impfic_core/api.py
--rw-r--r--   0        0        0     3206 2024-01-03 12:59:17.212116 impfic_core-0.8.0/impfic_core/extract/extract_stats.py
--rw-r--r--   0        0        0     2917 2023-01-25 09:52:41.454777 impfic_core-0.8.0/impfic_core/fetch/fetch_elastic.py
--rw-r--r--   0        0        0     5810 2024-01-24 09:28:10.211911 impfic_core-0.8.0/impfic_core/map/map_genre.py
--rw-r--r--   0        0        0     5195 2024-01-24 09:20:46.150217 impfic_core-0.8.0/impfic_core/map/map_isbns.py
--rw-r--r--   0        0        0        0 2023-01-26 10:23:09.851408 impfic_core-0.8.0/impfic_core/measures/__init__.py
--rw-r--r--   0        0        0     1476 2023-12-14 12:10:05.166333 impfic_core-0.8.0/impfic_core/measures/fractality.py
--rw-r--r--   0        0        0     7968 2023-08-16 13:12:06.345581 impfic_core-0.8.0/impfic_core/measures/keyness.py
--rw-r--r--   0        0        0      430 2023-01-26 12:31:38.658019 impfic_core-0.8.0/impfic_core/measures/length.py
--rw-r--r--   0        0        0        0 2023-01-26 10:48:01.700250 impfic_core-0.8.0/impfic_core/measures/temp.py
--rw-r--r--   0        0        0     9669 2024-02-21 15:03:16.871565 impfic_core-0.8.0/impfic_core/measures/text_features.py
--rw-r--r--   0        0        0        0 2024-02-21 08:51:38.189144 impfic_core-0.8.0/impfic_core/parse/__init__.py
--rw-r--r--   0        0        0     1113 2024-01-22 14:28:18.771343 impfic_core-0.8.0/impfic_core/parse/chunk.py
--rw-r--r--   0        0        0     9455 2024-02-20 15:03:48.039738 impfic_core-0.8.0/impfic_core/parse/doc.py
--rw-r--r--   0        0        0    20719 2022-06-03 11:32:00.518470 impfic_core-0.8.0/impfic_core/parse/parse_alpino_sentence.py
--rw-r--r--   0        0        0     7958 2024-01-08 15:06:47.592308 impfic_core-0.8.0/impfic_core/parse/parse_book_metadata.py
--rw-r--r--   0        0        0    10827 2023-06-19 20:03:21.184079 impfic_core-0.8.0/impfic_core/parse/parse_review.py
--rw-r--r--   0        0        0     9569 2024-02-20 15:08:26.311201 impfic_core-0.8.0/impfic_core/parse/parse_trankit_sentence.py
--rw-r--r--   0        0        0     1288 2022-03-17 09:17:20.173729 impfic_core-0.8.0/impfic_core/parse/pronouns.py
--rw-r--r--   0        0        0        0 2024-02-20 10:40:21.612208 impfic_core-0.8.0/impfic_core/parse/sentence.py
--rw-r--r--   0        0        0        0 2024-01-22 17:03:34.131901 impfic_core-0.8.0/impfic_core/pattern/__init__.py
--rw-r--r--   0        0        0    14082 2024-03-20 12:21:29.075331 impfic_core-0.8.0/impfic_core/pattern/patterns.py
--rw-r--r--   0        0        0     5640 2024-03-06 10:31:54.093654 impfic_core-0.8.0/impfic_core/pattern/patterns_nl.py
--rw-r--r--   0        0        0      250 2024-02-20 12:07:28.815921 impfic_core-0.8.0/impfic_core/pattern/tag_sets.py
--rw-r--r--   0        0        0     1269 2024-01-23 22:56:05.198707 impfic_core-0.8.0/impfic_core/pattern/tag_sets_de.py
--rw-r--r--   0        0        0     1599 2024-02-21 08:01:51.905946 impfic_core-0.8.0/impfic_core/pattern/tag_sets_en.py
--rw-r--r--   0        0        0     1480 2024-03-06 10:53:20.620976 impfic_core-0.8.0/impfic_core/pattern/tag_sets_nl.py
--rw-r--r--   0        0        0     1115 2023-01-24 10:00:50.162744 impfic_core-0.8.0/impfic_core/plot/plot.py
--rw-r--r--   0        0        0     1494 2022-06-03 13:31:23.582595 impfic_core-0.8.0/impfic_core/resources/rbn.py
--rw-r--r--   0        0        0       24 2023-02-07 11:17:14.637009 impfic_core-0.8.0/impfic_core/secrets_example.py
--rw-r--r--   0        0        0     1339 2024-03-20 12:26:48.291642 impfic_core-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     5979 1970-01-01 00:00:00.000000 impfic_core-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     4913 2024-02-20 14:25:31.536362 impfic_core-0.9.0/README.md
+-rw-r--r--   0        0        0       22 2024-03-27 14:50:04.169304 impfic_core-0.9.0/impfic_core/__init__.py
+-rw-r--r--   0        0        0     2201 2024-03-20 13:24:36.391602 impfic_core-0.9.0/impfic_core/analysis/prep_word2vec_emotion_recognition.py
+-rw-r--r--   0        0        0     1225 2024-02-21 10:47:17.314822 impfic_core-0.9.0/impfic_core/api.py
+-rw-r--r--   0        0        0     3206 2024-01-03 12:59:17.212116 impfic_core-0.9.0/impfic_core/extract/extract_stats.py
+-rw-r--r--   0        0        0     2917 2023-01-25 09:52:41.454777 impfic_core-0.9.0/impfic_core/fetch/fetch_elastic.py
+-rw-r--r--   0        0        0     5810 2024-01-24 09:28:10.211911 impfic_core-0.9.0/impfic_core/map/map_genre.py
+-rw-r--r--   0        0        0     5195 2024-01-24 09:20:46.150217 impfic_core-0.9.0/impfic_core/map/map_isbns.py
+-rw-r--r--   0        0        0        0 2023-01-26 10:23:09.851408 impfic_core-0.9.0/impfic_core/measures/__init__.py
+-rw-r--r--   0        0        0     1476 2023-12-14 12:10:05.166333 impfic_core-0.9.0/impfic_core/measures/fractality.py
+-rw-r--r--   0        0        0     7968 2023-08-16 13:12:06.345581 impfic_core-0.9.0/impfic_core/measures/keyness.py
+-rw-r--r--   0        0        0      430 2023-01-26 12:31:38.658019 impfic_core-0.9.0/impfic_core/measures/length.py
+-rw-r--r--   0        0        0        0 2023-01-26 10:48:01.700250 impfic_core-0.9.0/impfic_core/measures/temp.py
+-rw-r--r--   0        0        0     9798 2024-03-27 14:35:37.306599 impfic_core-0.9.0/impfic_core/measures/text_features.py
+-rw-r--r--   0        0        0        0 2024-02-21 08:51:38.189144 impfic_core-0.9.0/impfic_core/parse/__init__.py
+-rw-r--r--   0        0        0     1113 2024-01-22 14:28:18.771343 impfic_core-0.9.0/impfic_core/parse/chunk.py
+-rw-r--r--   0        0        0     9873 2024-03-27 14:48:44.336140 impfic_core-0.9.0/impfic_core/parse/doc.py
+-rw-r--r--   0        0        0    20719 2022-06-03 11:32:00.518470 impfic_core-0.9.0/impfic_core/parse/parse_alpino_sentence.py
+-rw-r--r--   0        0        0     7958 2024-01-08 15:06:47.592308 impfic_core-0.9.0/impfic_core/parse/parse_book_metadata.py
+-rw-r--r--   0        0        0    10827 2023-06-19 20:03:21.184079 impfic_core-0.9.0/impfic_core/parse/parse_review.py
+-rw-r--r--   0        0        0     9569 2024-02-20 15:08:26.311201 impfic_core-0.9.0/impfic_core/parse/parse_trankit_sentence.py
+-rw-r--r--   0        0        0     1288 2022-03-17 09:17:20.173729 impfic_core-0.9.0/impfic_core/parse/pronouns.py
+-rw-r--r--   0        0        0        0 2024-02-20 10:40:21.612208 impfic_core-0.9.0/impfic_core/parse/sentence.py
+-rw-r--r--   0        0        0        0 2024-01-22 17:03:34.131901 impfic_core-0.9.0/impfic_core/pattern/__init__.py
+-rw-r--r--   0        0        0    14563 2024-03-27 14:10:44.600782 impfic_core-0.9.0/impfic_core/pattern/patterns.py
+-rw-r--r--   0        0        0     9256 2024-03-27 13:28:49.782810 impfic_core-0.9.0/impfic_core/pattern/patterns_nl.py
+-rw-r--r--   0        0        0      250 2024-02-20 12:07:28.815921 impfic_core-0.9.0/impfic_core/pattern/tag_sets.py
+-rw-r--r--   0        0        0     1269 2024-01-23 22:56:05.198707 impfic_core-0.9.0/impfic_core/pattern/tag_sets_de.py
+-rw-r--r--   0        0        0     1599 2024-02-21 08:01:51.905946 impfic_core-0.9.0/impfic_core/pattern/tag_sets_en.py
+-rw-r--r--   0        0        0     1480 2024-03-06 10:53:20.620976 impfic_core-0.9.0/impfic_core/pattern/tag_sets_nl.py
+-rw-r--r--   0        0        0     1115 2023-01-24 10:00:50.162744 impfic_core-0.9.0/impfic_core/plot/plot.py
+-rw-r--r--   0        0        0     1494 2022-06-03 13:31:23.582595 impfic_core-0.9.0/impfic_core/resources/rbn.py
+-rw-r--r--   0        0        0       24 2023-02-07 11:17:14.637009 impfic_core-0.9.0/impfic_core/secrets_example.py
+-rw-r--r--   0        0        0     1339 2024-03-27 14:50:04.168650 impfic_core-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     5979 1970-01-01 00:00:00.000000 impfic_core-0.9.0/PKG-INFO
```

### Comparing `impfic_core-0.8.0/README.md` & `impfic_core-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `impfic_core-0.8.0/impfic_core/api.py` & `impfic_core-0.9.0/impfic_core/api.py`

 * *Files identical despite different names*

### Comparing `impfic_core-0.8.0/impfic_core/extract/extract_stats.py` & `impfic_core-0.9.0/impfic_core/extract/extract_stats.py`

 * *Files identical despite different names*

### Comparing `impfic_core-0.8.0/impfic_core/fetch/fetch_elastic.py` & `impfic_core-0.9.0/impfic_core/fetch/fetch_elastic.py`

 * *Files identical despite different names*

### Comparing `impfic_core-0.8.0/impfic_core/map/map_genre.py` & `impfic_core-0.9.0/impfic_core/map/map_genre.py`

 * *Files identical despite different names*

### Comparing `impfic_core-0.8.0/impfic_core/map/map_isbns.py` & `impfic_core-0.9.0/impfic_core/map/map_isbns.py`

 * *Files identical despite different names*

### Comparing `impfic_core-0.8.0/impfic_core/measures/fractality.py` & `impfic_core-0.9.0/impfic_core/measures/fractality.py`

 * *Files identical despite different names*

### Comparing `impfic_core-0.8.0/impfic_core/measures/keyness.py` & `impfic_core-0.9.0/impfic_core/measures/keyness.py`

 * *Files identical despite different names*

### Comparing `impfic_core-0.8.0/impfic_core/measures/text_features.py` & `impfic_core-0.9.0/impfic_core/measures/text_features.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,42 +97,46 @@
         various statistics for the book, including counts and measures of sentence
         length as integers and floats.
     """
     book_chunk_files = get_book_chunk_files(isbn, data_dir)
     book_chunks = [book_chunk for book_chunk in read_book_chunk_files(book_chunk_files)]
     book_docs = [trankit_json_to_doc(book_chunk) for book_chunk in book_chunks]
     total, present, past, pv, clause_count, presp, pastp, press, pasts = get_verb_count(book_docs, pattern)
-    num_tokens, sent_len_mean, sent_len_median, sent_len_stdev, unique_tokens = get_length_stats(book_docs)
+    num_tokens, num_sents, sent_len_mean, sent_len_median, sent_len_stdev, unique_tokens = get_length_stats(book_docs)
     pron_count, propn_count, det_count = get_funcword_count(book_docs)
     noun_count, adj_count, adv_count, intj_count = get_uposword_count(book_docs)
     sconj_count, cconj_count, punct_count = get_gramword_count(book_docs)
     # added present_perfect_count below as 'pp'
-    stats = [isbn, total, present, past, pv, clause_count, presp, pastp, press, pasts, num_tokens, sent_len_mean, sent_len_median, sent_len_stdev,
+    stats = [isbn,
+             total, present, past, pv, clause_count, presp, pastp, press, pasts,
+             num_tokens, num_sents, sent_len_mean, sent_len_median, sent_len_stdev,
              unique_tokens, pron_count, propn_count, det_count, noun_count, adj_count, adv_count, intj_count,
              sconj_count, cconj_count, punct_count]
     return stats
 
 
 def get_length_stats(book_docs: List[Doc]):
     """Count length of sentences in book docs"""
     sentence_lengths = []
     num_tokens = 0
+    num_sents = 0
     unique_tokens = set()
     for doc in book_docs:
+        num_sents += len(doc.sentences)
         for sentence in doc.sentences:
             sentence_length = len(sentence)
             sentence_lengths.append(sentence_length)
             num_tokens += sentence_length
             unique_tokens.update(token.text for token in sentence.tokens)
     unique_tokens_count = len(unique_tokens)
     sentence_lengths = np.array(sentence_lengths)
     sent_len_mean = sentence_lengths.mean()
     sent_len_median = np.median(sentence_lengths)
     sent_len_stdev = sentence_lengths.std()
-    return num_tokens, sent_len_mean, sent_len_median, sent_len_stdev, unique_tokens_count
+    return num_tokens, num_sents, sent_len_mean, sent_len_median, sent_len_stdev, unique_tokens_count
 
 
 def get_verb_count(book_docs: List[Doc], pattern: Pattern) -> tuple:
     """counts frequency of types of verbs from book docs"""
     all_present_tense_count = 0
     all_past_tense_count = 0
     total_verb_count = 0
@@ -253,15 +257,15 @@
         parsed_isbns = parsed_isbns[:max_items]
     print("2 - get all book stats")
     all_stats = get_all_book_stats(parsed_isbns, data_dir, lang)
     print("3 - assign name columns")
     columns = [
         'isbn', 'total_verbs', 'all_present_verbs', 'all_past_verbs', 'pv_verbs',
         # added present perfect verbs here as 'pp_verbs'
-        'clause_count', 'pres_part_verbs', 'past_part_verbs', 'pres_simple_verbs', 'past_simple_verbs',
-        'num_tokens', 'sent_len_mean', 'sent_len_median',
+        'num_clauses', 'pres_part_verbs', 'past_part_verbs', 'pres_simple_verbs', 'past_simple_verbs',
+        'num_tokens', 'num_sents', 'sent_len_mean', 'sent_len_median',
         'sent_len_stdev', 'unique_tokens_count',
         'pron_count', 'propn_count', 'det_count', 'noun_count', 'adj_count', 'adv_count', 'intj_count',
         'sconj_count', 'cconj_count', 'punct_count'
     ]
     print("4 - save dataframe")
     return pd.DataFrame(all_stats, columns=columns)
```

### Comparing `impfic_core-0.8.0/impfic_core/parse/chunk.py` & `impfic_core-0.9.0/impfic_core/parse/chunk.py`

 * *Files identical despite different names*

### Comparing `impfic_core-0.8.0/impfic_core/parse/doc.py` & `impfic_core-0.9.0/impfic_core/parse/doc.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,14 +167,16 @@
     return Entity(entity_tokens, entity_text, start_in_doc, end_in_doc, label)
 
 
 def trankit_json_to_entities(sent_tokens: List[Token], sent: Dict[str, any]) -> List[Entity]:
     """Turn the tokens of a Trankit sentence with NER labels into entities."""
     entity_tokens = []
     entities = []
+    if len(sent_tokens) == 0:
+        return entities
     sent_start = sent_tokens[0].start
     for token in sent_tokens:
         if token.ner[0] in 'OBS':
             if len(entity_tokens) > 0:
                 entity = trankit_json_to_entity(entity_tokens, sent, sent_start)
                 entities.append(entity)
             entity_tokens = []
@@ -196,16 +198,26 @@
         tokens=tokens,
         entities=entities,
         start=sent['start'],
         end=sent['end']
     )
 
 
-def trankit_json_to_sentence(token_offset: int, sentence: Dict[str, any]) -> Sentence:
-    tokens = [trankit_json_to_token(ti+token_offset, ti, token) for ti, token in enumerate(sentence['tokens'])]
+def trankit_json_to_sentence(token_offset: int, sentence: Dict[str, any],
+                             skip_bad_tokens: bool = False) -> Sentence:
+    if skip_bad_tokens is True:
+        tokens = []
+        for ti, token in enumerate(sentence['tokens']):
+            try:
+                token = trankit_json_to_token(ti+token_offset, ti, token)
+                tokens.append(token)
+            except KeyError:
+                continue
+    else:
+        tokens = [trankit_json_to_token(ti+token_offset, ti, token) for ti, token in enumerate(sentence['tokens'])]
     entities = trankit_json_to_entities(tokens, sentence)
     return Sentence(
         id=sentence['id'],
         text=sentence['text'],
         tokens=tokens,
         entities=entities,
         start=sentence['tokens'][0]['dspan'][0],
```

### Comparing `impfic_core-0.8.0/impfic_core/parse/parse_alpino_sentence.py` & `impfic_core-0.9.0/impfic_core/parse/parse_alpino_sentence.py`

 * *Files identical despite different names*

### Comparing `impfic_core-0.8.0/impfic_core/parse/parse_book_metadata.py` & `impfic_core-0.9.0/impfic_core/parse/parse_book_metadata.py`

 * *Files identical despite different names*

### Comparing `impfic_core-0.8.0/impfic_core/parse/parse_review.py` & `impfic_core-0.9.0/impfic_core/parse/parse_review.py`

 * *Files identical despite different names*

### Comparing `impfic_core-0.8.0/impfic_core/parse/parse_trankit_sentence.py` & `impfic_core-0.9.0/impfic_core/parse/parse_trankit_sentence.py`

 * *Files identical despite different names*

### Comparing `impfic_core-0.8.0/impfic_core/parse/pronouns.py` & `impfic_core-0.9.0/impfic_core/parse/pronouns.py`

 * *Files identical despite different names*

### Comparing `impfic_core-0.8.0/impfic_core/pattern/patterns.py` & `impfic_core-0.9.0/impfic_core/pattern/patterns.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,24 +130,27 @@
         return False
 
     ####################
     # Grouping methods #
     ####################
 
     @staticmethod
-    def group_tokens_by_head(tokens: List[Token]) -> Dict[int, List[Token]]:
+    def group_tokens_by_head(tokens: List[Token], debug: int = 0) -> Dict[int, List[Token]]:
         """Group a list of tokens by their head tokens."""
         head_group = defaultdict(list)
         if len(tokens) == 0:
+            if debug > 1:
+                print('Pattern.group_tokens_by_head - no tokens, returning no groups')
             return head_group
         for token in tokens:
             head_group[token.head].append(token)
         for head_id in head_group:
-            head_token = tokens[head_id]
-            head_group[head_id].append(head_token)
+            if head_id != -1:
+                head_token = tokens[head_id]
+                head_group[head_id].append(head_token)
         return head_group
 
     def get_head_verb_id(self, head_id: int, tokens: List[Token]) -> int:
         """Return the id of the head verb of a set of tokens for a given head id,
         or -1 if the head id is -1 (the root node)."""
         if head_id == -1:
             return -1
@@ -174,52 +177,61 @@
         """Group a list of tokens by their head verb tokens."""
         head_group = self.group_tokens_by_head(tokens)
         head_verb_group = defaultdict(list)
         if len(tokens) == 0:
             return head_verb_group
         for head_id in head_group:
             if debug > 0:
-                print(f'group_tokens_by_head_verb - head_id: {head_id}')
+                print(f'Pattern.group_tokens_by_head_verb - 1 - head_id: {head_id}')
             if head_id > len(tokens):
-                print('head_id larger than number of tokens:')
-                print('group_tokens_by_head_verb - head_id:', head_id)
-                print('group_tokens_by_head_verb - tokens:', tokens)
+                print('Pattern.group_tokens_by_head_verb - head_id larger than number of tokens:')
+                print('Pattern.group_tokens_by_head_verb - head_id:', head_id)
+                print('Pattern.group_tokens_by_head_verb - tokens:', tokens)
             head_verb_id = self.get_head_verb_id(head_id, tokens)
             if debug > 0:
-                print(f'group_tokens_by_head_verb - head_verb_id: {head_verb_id}\n\n')
-            if head_verb_id == -1:
+                print(f'Pattern.roup_tokens_by_head_verb - 2 - head_verb_id: {head_verb_id}\n\n')
+            # if head_verb_id == -1:
                 # list of tokens has no verb
-                continue
+            #     continue
             for token in head_group[head_id]:
                 if debug > 0:
-                    print(f'group_tokens_by_head_verb - head_id: {head_id}\thead_verb_id: {head_verb_id}'
+                    print(f'Pattern.group_tokens_by_head_verb - 3 - head_id: {head_id}\thead_verb_id: {head_verb_id}'
                           f'\ttoken:', token.text, token.id, token.head)
                     print('\t\ttoken (upos, deprel):', (token.upos, token.deprel))
                     print('\t\ttoken.id in head_group:', token.id in head_group)
                     print('\t\ttoken.id is_head_verb:', self.is_head_verb(token))
                 if token.id in head_group and self.is_head_verb(token):
                     if token not in head_verb_group[token.id]:
                         if debug > 0:
-                            print('HEAD VERB:', token.id, token.text, token.deprel)
+                            print('Pattern.group_token_by_head_verb - HEAD VERB:', token.id, token.text, token.deprel)
                         head_verb_group[token.id].append(token)
                 elif token not in head_verb_group[head_verb_id]:
                     head_verb_group[head_verb_id].append(token)
                     if debug > 0:
                         print(f'\tadding token: {token.id} {token.text} to head_verb_id {head_verb_id}')
                 else:
                     if debug > 0:
                         print('\tskipping token:', token)
                     pass
-            for head_verb_id in sorted(head_verb_group):
-                if debug > 0:
-                    print('\n---------------------\n')
-                    print('content of head_verb_group with head_verb_id:', head_verb_id)
+            if debug > 1:
+                for head_verb_id in sorted(head_verb_group):
+                    print('\n\t---------------------\n')
+                    print('\tcontent of head_verb_group with head_verb_id:', head_verb_id)
                     for token in sorted(head_verb_group[head_verb_id], key=lambda t: t.id):
                         print('\t', token.id, token.text)
                     print('\n---------------------\n')
+        if copy_conj_subject is True:
+            head_verb_group = self.copy_subject_across_conjunctions(head_verb_group)
+        for head_verb_id in head_verb_group:
+            head_verb_group[head_verb_id].sort(key=lambda t: t.id)
+        head_verb_group = self.merge_verb_groups(head_verb_group)
+        return head_verb_group
+
+    @staticmethod
+    def merge_verb_groups(head_verb_group: Dict[int, List[Token]]):
         merge_into = {}
         for head_verb_id in head_verb_group:
             for other_head_verb_id in head_verb_group:
                 if head_verb_id == other_head_verb_id:
                     continue
                 if head_verb_id in [token.id for token in head_verb_group[other_head_verb_id]]:
                     if other_head_verb_id in merge_into:
@@ -228,18 +240,14 @@
                         merge_into[head_verb_id] = other_head_verb_id
         for head_verb_id in merge_into:
             new_head_verb_id = merge_into[head_verb_id]
             merge_tokens = [token for token in head_verb_group[head_verb_id]
                             if token not in head_verb_group[new_head_verb_id]]
             head_verb_group[new_head_verb_id].extend(merge_tokens)
             del head_verb_group[head_verb_id]
-        if copy_conj_subject is True:
-            head_verb_group = self.copy_subject_across_conjunctions(head_verb_group)
-        for head_verb_id in head_verb_group:
-            head_verb_group[head_verb_id].sort(key=lambda t: t.id)
         return head_verb_group
 
     def copy_subject_across_conjunctions(self, head_verb_group: Dict[int, List[Token]]) -> Dict[int, List[Token]]:
         for head_id in head_verb_group:
             if head_id == -1:
                 continue
             for t in head_verb_group[head_id]:
```

### Comparing `impfic_core-0.8.0/impfic_core/pattern/tag_sets_de.py` & `impfic_core-0.9.0/impfic_core/pattern/tag_sets_de.py`

 * *Files identical despite different names*

### Comparing `impfic_core-0.8.0/impfic_core/pattern/tag_sets_en.py` & `impfic_core-0.9.0/impfic_core/pattern/tag_sets_en.py`

 * *Files identical despite different names*

### Comparing `impfic_core-0.8.0/impfic_core/pattern/tag_sets_nl.py` & `impfic_core-0.9.0/impfic_core/pattern/tag_sets_nl.py`

 * *Files identical despite different names*

### Comparing `impfic_core-0.8.0/impfic_core/plot/plot.py` & `impfic_core-0.9.0/impfic_core/plot/plot.py`

 * *Files identical despite different names*

### Comparing `impfic_core-0.8.0/impfic_core/resources/rbn.py` & `impfic_core-0.9.0/impfic_core/resources/rbn.py`

 * *Files identical despite different names*

### Comparing `impfic_core-0.8.0/pyproject.toml` & `impfic_core-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "impfic-core"
-version = "0.8.0"
+version = "0.9.0"
 description = "Utility functions for the Impact and Fiction project"
 authors = ["Marijn Koolen <marijn.koolen@huygens.knaw.nl>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/impact-and-fiction/impfic-core"
 repository = "https://github.com/impact-and-fiction/impfic-core"
 classifiers = [
@@ -31,15 +31,15 @@
 version = 'poetry_scripts:version'
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.bumpver]
-current_version = "0.8.0"
+current_version = "0.9.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `impfic_core-0.8.0/PKG-INFO` & `impfic_core-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: impfic-core
-Version: 0.8.0
+Version: 0.9.0
 Summary: Utility functions for the Impact and Fiction project
 Home-page: https://github.com/impact-and-fiction/impfic-core
 License: MIT
 Author: Marijn Koolen
 Author-email: marijn.koolen@huygens.knaw.nl
 Requires-Python: >=3.8,<=3.12
 Classifier: Development Status :: 4 - Beta
```

