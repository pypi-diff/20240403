# Comparing `tmp/isagog_ai-0.7.9.tar.gz` & `tmp/isagog_ai-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isagog_ai-0.7.9.tar", max compression
+gzip compressed data, was "isagog_ai-0.8.0.tar", max compression
```

## Comparing `isagog_ai-0.7.9.tar` & `isagog_ai-0.8.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0        0 2023-11-09 14:36:49.454784 isagog_ai-0.7.9/isagog/__init__.py
--rw-r--r--   0        0        0        0 2023-11-09 14:36:49.455784 isagog_ai-0.7.9/isagog/client/__init__.py
--rw-r--r--   0        0        0     8486 2024-03-25 14:38:52.061686 isagog_ai-0.7.9/isagog/client/kg_client.py
--rw-r--r--   0        0        0     5232 2024-03-25 14:27:33.690965 isagog_ai-0.7.9/isagog/client/nlp_client.py
--rw-r--r--   0        0        0        0 2024-01-17 10:28:20.797474 isagog_ai-0.7.9/isagog/generator/__init__.py
--rw-r--r--   0        0        0     5438 2024-01-30 16:42:35.759384 isagog_ai-0.7.9/isagog/generator/sparql_generator.py
--rw-r--r--   0        0        0        0 2023-11-09 14:36:49.456784 isagog_ai-0.7.9/isagog/model/__init__.py
--rw-r--r--   0        0        0    12672 2023-12-21 10:57:56.624555 isagog_ai-0.7.9/isagog/model/kg_model.py
--rw-r--r--   0        0        0    26807 2024-02-05 11:55:57.301151 isagog_ai-0.7.9/isagog/model/kg_query.py
--rw-r--r--   0        0        0      371 2023-11-09 14:36:49.457780 isagog_ai-0.7.9/isagog/model/nlp_model.py
--rw-r--r--   0        0        0      577 2023-12-16 19:08:20.361655 isagog_ai-0.7.9/LICENSE
--rw-r--r--   0        0        0      569 2024-03-25 14:27:33.703961 isagog_ai-0.7.9/pyproject.toml
--rw-r--r--   0        0        0       48 2023-11-28 11:06:21.183153 isagog_ai-0.7.9/README.md
--rw-r--r--   0        0        0      710 1970-01-01 00:00:00.000000 isagog_ai-0.7.9/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-11-09 14:36:49.454784 isagog_ai-0.8.0/isagog/__init__.py
+-rw-r--r--   0        0        0        0 2023-11-09 14:36:49.455784 isagog_ai-0.8.0/isagog/client/__init__.py
+-rw-r--r--   0        0        0     8560 2024-03-29 14:48:01.626394 isagog_ai-0.8.0/isagog/client/kg_client.py
+-rw-r--r--   0        0        0     5928 2024-03-29 14:48:01.665081 isagog_ai-0.8.0/isagog/client/nlp_client.py
+-rw-r--r--   0        0        0        0 2024-03-29 08:28:01.370228 isagog_ai-0.8.0/isagog/generator/__init__.py
+-rw-r--r--   0        0        0     5647 2024-03-29 14:48:01.711776 isagog_ai-0.8.0/isagog/generator/sparql_generator.py
+-rw-r--r--   0        0        0        0 2023-11-09 14:36:49.456784 isagog_ai-0.8.0/isagog/model/__init__.py
+-rw-r--r--   0        0        0    13646 2024-03-29 14:48:01.643535 isagog_ai-0.8.0/isagog/model/kg_model.py
+-rw-r--r--   0        0        0    26876 2024-03-29 14:48:01.680285 isagog_ai-0.8.0/isagog/model/kg_query.py
+-rw-r--r--   0        0        0      443 2024-03-29 14:48:01.725437 isagog_ai-0.8.0/isagog/model/nlp_model.py
+-rw-r--r--   0        0        0      577 2023-12-16 19:08:20.361655 isagog_ai-0.8.0/LICENSE
+-rw-r--r--   0        0        0      569 2024-03-29 11:45:02.491727 isagog_ai-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0       48 2023-11-28 11:06:21.183153 isagog_ai-0.8.0/README.md
+-rw-r--r--   0        0        0      710 1970-01-01 00:00:00.000000 isagog_ai-0.8.0/PKG-INFO
```

### Comparing `isagog_ai-0.7.9/isagog/client/kg_client.py` & `isagog_ai-0.8.0/isagog/client/kg_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,124 +1,110 @@
 """
-Interface to Isagog KG service
+Interface to the Isagog Knoledge Graph service
+(c) Isagog S.r.l. 2024, MIT License
 """
 import logging
 import os
-import sys
 import time
 from typing import Type, TypeVar
 
 import requests
-
-from isagog.model.kg_query import UnarySelectQuery, DisjunctiveClause, AtomicClause, Comparison, Value
-from isagog.model.kg_model import Individual, Entity, Assertion, Ontology, Attribute, Concept, Relation, ID
 from dotenv import load_dotenv
 
+from isagog.model.kg_model import Individual, Entity, Assertion, Ontology, Attribute, Concept, Relation, ID
+from isagog.model.kg_query import UnarySelectQuery, DisjunctiveClause, AtomicClause, Comparison, Value
 
 load_dotenv()
 
-log = logging.getLogger("isagog-cli")
-
-log.setLevel(os.getenv("ISAGOG_AI_LOG_LEVEL", logging.INFO))
-
-handler = logging.StreamHandler(sys.stdout)
-# Create a formatter and set the format for the handler
-formatter = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
-handler.setFormatter(formatter)
-
-# Add the handler to the logger
-log.addHandler(handler)
-
-
-
+KG_DEFAULT_TIMEOUT = int(os.getenv('KG_DEFAULT_TIMEOUT', 120))
 
+# Type variable for the Entity hierarchy
 E = TypeVar('E', bound='Entity')
 
 
 class KnowledgeBase(object):
     """
     Interface to knowledge base service
     """
 
     def __init__(self,
                  route: str,
                  ontology: Ontology = None,
                  dataset: str = None,
-                 version: str = "latest"):
+                 version: str = None,
+                 logger=None):
         """
 
         :param route: the service's endpoint route
         :param ontology: the kb ontology
         :param dataset: the dataset name; if None, uses the service's default
         :param version: the service's version identifier
         """
         assert route
         self.route = route
         self.dataset = dataset
         self.ontology = ontology
-        self.version = version
-        log.debug("KnowledgeBase initialized with route %s", route)
+        self.version = version if version else "latest"
+        self.logger = logger if logger else logging.getLogger()
+        self.logger.info("Isagog KG client (%s) initialized on route %s", hex(id(self)), route)
 
     def get_entity(self,
                    _id: str,
                    expand: bool = True,
-                   limit: int = 1024,
                    entity_type: Type[E] = Entity
                    ) -> E | None:
         """
-        Gets all individual entity data from the kg
-
+        Gets the entity by its identifier
         :param _id: the entity identifier
-        :param limit:
-        :param expand:
+        :param expand: whether to return entity attributes
         :param entity_type: the entity type (default: Entity)
         """
 
         assert _id
 
-        log.debug("Fetching %s", _id)
+        self.logger.debug("Fetching %s", _id)
 
         if not issubclass(entity_type, Entity):
             raise ValueError(f"{entity_type} not an Entity")
 
         expand = "true" if expand else "false"
 
-        params = f"id={_id}&expand={expand}&limit={limit}"
+        params = f"id={_id}&expand={expand}"
 
         if self.dataset:
             params += f"&dataset={self.dataset}"
 
         res = requests.get(
             url=self.route,
             params=params,
             headers={"Accept": "application/json"},
         )
         if res.ok:
-            log.debug("Fetched %s", _id)
+            self.logger.debug("Fetched %s", _id)
             return entity_type(_id, **res.json())
         else:
-            log.error("Couldn't fetch %s due to %s", _id, res.reason)
+            self.logger.error("Couldn't fetch %s due to %s", _id, res.reason)
             return None
 
     def query_assertions(self,
                          subject: Individual,
                          properties: list[Attribute | Relation],
-                         timeout=30
+                         timeout=KG_DEFAULT_TIMEOUT
                          ) -> list[Assertion]:
         """
-        Returns entity properties, if any
+        Returns specific entity properties
 
         :param timeout:
         :param subject:
         :param properties: the queried properties
         :return: a list of dictionaries { property: values }
         """
         assert (subject and properties)
 
-        log.debug("Querying assertions for %s", subject.id)
+        self.logger.debug("Querying assertions for %s", subject.id)
 
         query = UnarySelectQuery(subject=subject)
 
         for prop in properties:
             query.add_fetch_clause(predicate=str(prop))
 
         query_dict = query.to_dict(self.version)
@@ -129,77 +115,77 @@
             headers={"Accept": "application/json"},
             timeout=timeout
         )
 
         if res.ok:
             res_list = res.json()
             if len(res_list) == 0:
-                log.warning("Void attribute query")
+                self.logger.warning("Void attribute query")
                 return []
             else:
                 res_attrib_list = res_list[0].get('attributes', OSError("malformed response"))
 
                 def __get_values(_prop: str) -> str:
                     try:
                         record = next(item for item in res_attrib_list if item['id'] == _prop)
                         return record.get('values', OSError("malformed response"))
                     except StopIteration:
                         raise OSError("incomplete response: %s not found", _prop)
 
                 return [Assertion(predicate=prop, values=__get_values(prop)) for prop in properties]
         else:
-            log.warning("Query of entity %s failed due to %s", subject, res.reason)
+            self.logger.warning("Query of entity %s failed due to %s", subject, res.reason)
             return []
 
     def search_individuals(self,
                            kinds: list[Concept] = None,
-                           search_values: dict[Attribute, Value] = None,
-                           timeout=30
+                           constraints: dict[Attribute, Value] = None,
+                           timeout=KG_DEFAULT_TIMEOUT
                            ) -> list[Individual]:
         """
         Retrieves individuals by string search
-        :param timeout:
-        :param kinds:
-        :param search_values:
-        :return:
+        :param timeout: the request timeout
+        :param kinds: the kinds to search for
+        :param constraints: the search constraints
+        :return: a list of matching individuals
         """
-        assert (kinds or (search_values and len(search_values) > 0))
-        log.debug("Searching individuals")
+        assert (kinds or (constraints and len(constraints) > 0))
+        self.logger.debug("Searching individuals")
         entities = []
         query = UnarySelectQuery()
         if kinds:
             query.add_kinds(kinds)
-        if len(search_values) == 1:
-            attribute, value = next(iter(search_values.items()))
+        if len(constraints) == 1:
+            attribute, value = next(iter(constraints.items()))
             search_clause = AtomicClause(property=attribute, argument=value, method=Comparison.REGEX)
         else:
             search_clause = DisjunctiveClause()
-            for attribute, value in search_values.items():
+            for attribute, value in constraints.items():
                 search_clause.add_atom(property=attribute, argument=value, method=Comparison.REGEX)
 
         query.clause(search_clause)
 
         res = requests.post(
             url=self.route,
             json=query.to_dict(self.version),
             headers={"Accept": "application/json"},
             timeout=timeout
         )
 
         if res.ok:
             entities.extend([Individual(r.get('id'), **r) for r in res.json()])
         else:
-            log.error("Search individuals failed: code %d, reason %s", res.status_code, res.reason)
+            self.logger.error("Search individuals failed: code %d, reason %s", res.status_code, res.reason)
 
         return entities
 
     def query_individuals(self,
                           query: UnarySelectQuery,
                           kind: Type[E] = Individual,
-                          timeout=30
+                          timeout=KG_DEFAULT_TIMEOUT
                           ) -> list[E]:
         """
 
         :param query:
         :param kind:
         :param timeout:
         :return:
@@ -215,31 +201,31 @@
             url=self.route,
             json=req,
             headers={"Accept": "application/json"},
             timeout=timeout
         )
 
         if res.ok:
-            log.debug("Query individuals successful in %d seconds", time.time() - start_time)
+            self.logger.debug("Query individuals successful in %d seconds", time.time() - start_time)
             return [kind(r.get('id'), **r) for r in res.json()]
         elif res.status_code < 500:
-            log.warning("query individuals return code %d, reason %s", res.status_code, res.reason)
+            self.logger.warning("query individuals return code %d, reason %s", res.status_code, res.reason)
         else:
-            log.error("query individuals return code code %d, reason %s", res.status_code, res.reason)
+            self.logger.error("query individuals return code code %d, reason %s", res.status_code, res.reason)
         return []
 
     def upsert_individual(self, individual: Individual, auth_token=None) -> bool:
         """
         Updates an individual or insert it if not present; existing properties are preserved
 
         :param individual: the individual
         :param auth_token:
         :return:
         """
-        log.debug("Updating individual %s", individual.id)
+        self.logger.debug("Updating individual %s", individual.id)
         params = {
             'id': individual.id
         }
 
         if self.dataset and (self.version == "latest" or self.version > "v1.0.0"):
             params['dataset'] = self.dataset
```

### Comparing `isagog_ai-0.7.9/isagog/client/nlp_client.py` & `isagog_ai-0.8.0/isagog/client/nlp_client.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,29 @@
+"""
+Client for Isagog NLP service
+(c) Isagog S.r.l. 2024, MIT License
+"""
 import logging
-import sys
+import os
+import time
 
 import requests
 from dotenv import load_dotenv
-import os
 
 from isagog.model.nlp_model import Word, NamedEntity
 
 load_dotenv()
 
-log = logging.getLogger("isagog-cli")
-
-log.setLevel(os.getenv("ISAGOG_AI_LOG_LEVEL", logging.INFO))
-
-handler = logging.StreamHandler(sys.stdout)
-
-# Create a formatter and set the format for the handler
-formatter = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
-handler.setFormatter(formatter)
-
-# Add the handler to the logger
-log.addHandler(handler)
+NLP_DEFAULT_TIMEOUT = int(os.getenv('NLP_DEFAULT_TIMEOUT', 60))
 
 DEFAULT_LEXICAL_POS = ["NOUN", "VERB", "ADJ", "ADV"]
 DEFAULT_SEARCH_POS = ["NOUN", "VERB", "PROPN"]
 
-def truncate(s: str, n = 10):
+
+def truncate(s: str, n=10):
     """
     Truncate a string to the first N characters, adding '...' if the string is longer.
 
     :param s: The string to be truncated.
     :param n: The maximum length of the truncated string.
     :return: The truncated string.
     """
@@ -43,119 +37,143 @@
 class LanguageProcessor(object):
     """
     Interface to Language service
     """
 
     def __init__(self,
                  route: str,
-                 version: str = None):
+                 version: str = None,
+                 logger=logging.getLogger()):
         self.route = route
         self.version = version
-        log.debug("LanguageProcessor initialized with route %s", route)
+        self.logger = logger
+        self.logger.info("Isagog NLP client (%s) initialized on route %s", hex(id(self)), route)
 
-    def similarity_ranking(self, target: str,
-                           candidates: list[str]) -> list[(int, float)]:
+    def similarity_ranking(self,
+                           target: str,
+                           candidates: list[str],
+                           timeout=NLP_DEFAULT_TIMEOUT) -> list[(int, float)]:
 
         """
         Ranks the candidates based on their similarity with the supplied text
+        :param timeout:
         :param target:
         :param candidates:
         :return:
         """
-        log.debug("Ranking for %s", target)
+        start = time.time()
         req = {
             "target": target,
             "candidates": candidates,
         }
 
         res = requests.post(
             url=self.route + "/rank",
             json=req,
-            timeout=30
+            timeout=timeout
         )
 
         if res.ok:
+            self.logger.debug("Ranked %s in %d seconds", truncate(target), time.time() - start)
             return [(rank[0], rank[1]) for rank in res.json()]
         else:
-            log.error("similarity ranking failed: code=%d, reason=%s", res.status_code, res.reason)
+            self.logger.error("similarity ranking failed: code=%d, reason=%s", res.status_code, res.reason)
             return []
 
-    def extract_keywords_from(self, text: str, number=5) -> list[str]:
+    def extract_keywords_from(self,
+                              text: str,
+                              number=5,
+                              timeout=NLP_DEFAULT_TIMEOUT) -> list[str]:
         """
         Extract the main N words (keywords) from the supplied text
+        :param timeout:
         :param text:
         :param number:
         :return:
         """
-        log.debug("Extracting %d keywords from %s", number, truncate(text))
+        self.logger.debug("Extracting %d keywords from %s", number, truncate(text))
         res = requests.post(
             url=self.route + "/analyze",
             json={
                 "text": text,
                 "tasks": ["keyword"],
                 "keyword_number": number
             },
             headers={"Accept": "application/json"},
-            timeout=20
+            timeout=timeout
         )
         if res.ok:
             res_dict = res.json()
             words = [kwr[0] for kwr in res_dict["keyword"]]
             return words
         else:
-            log.error("fail to extract from '%s': code=%d, reason=%s", text, res.status_code, res.reason)
+            self.logger.error("fail to extract from '%s': code=%d, reason=%s", text, res.status_code, res.reason)
             return []
 
-    def extract_words(self, text: str, filter_pos=None) -> list[str]:
+    def extract_words(self,
+                      text: str,
+                      filter_pos=None,
+                      timeout=NLP_DEFAULT_TIMEOUT) -> list[str]:
         """
         Extract all the word token with the given part-of-speech
+        :param timeout:
         :param text:
         :param filter_pos: part of speech list
         :return:
         """
-        log.debug("Extracting words from %s", truncate(text))
+        self.logger.debug("Extracting words from %s", truncate(text))
         if not filter_pos:
             filter_pos = DEFAULT_LEXICAL_POS
 
         res = requests.post(
             url=self.route + "/analyze",
             json={
                 "text": text,
                 "tasks": ["word"]
             },
             headers={"Accept": "application/json"},
-            timeout=20
+            timeout=timeout
         )
         if res.ok:
             res_dict = res.json()
             words = [Word(**{k: v for k, v in r.items() if k in Word._fields}) for r in res_dict["words"]]
             return [w.text for w in words if w.pos in filter_pos]
         else:
-            log.error("fail to extract from '%s': code=%d, reason=%s", text, res.status_code, res.reason)
+            self.logger.error("fail to extract from '%s': code=%d, reason=%s", text, res.status_code, res.reason)
             return []
 
-    def extract_words_entities(self, text: str, filter_pos=None) -> (list[Word], list[NamedEntity]):
-        log.debug("Extracting words and entities from %s", truncate(text))
+    def extract_words_entities(self,
+                               text: str,
+                               filter_pos=None,
+                               timeout=NLP_DEFAULT_TIMEOUT) -> (list[Word], list[NamedEntity]):
+        """
+        Extract words and entities from the supplied text
+        :param text:
+        :param filter_pos:
+        :param timeout:
+        :return:
+        """
+        self.logger.debug("Extracting words and entities from %s", truncate(text))
         if not filter_pos:
             filter_pos = DEFAULT_LEXICAL_POS
 
         res = requests.post(
             url=self.route + "/analyze",
             json={
                 "text": text,
                 "tasks": ["word", "entity"]
             },
             headers={"Accept": "application/json"},
-            timeout=20
+            timeout=timeout
         )
 
         if res.ok:
             res_dict = res.json()
             words = list(filter(lambda w: w.pos in filter_pos,
                                 [Word(**{k: v for k, v in r.items() if k in Word._fields}) for r in res_dict["words"]]))
             entities = [NamedEntity(**{k: v for k, v in r.items() if k in NamedEntity._fields}) for r in
                         res_dict["entities"]]
             return words, entities
 
         else:
-            log.error("fail to extract from '%s': code=%d, reason=%s", text, res.status_code, res.reason)
+            self.logger.error("fail to extract from '%s': code=%d, reason=%s", text, res.status_code, res.reason)
             return [], []
```

### Comparing `isagog_ai-0.7.9/isagog/generator/sparql_generator.py` & `isagog_ai-0.8.0/isagog/generator/sparql_generator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,22 @@
+"""
+SPARQL query generator
+(c) Isagog S.r.l. 2024, MIT License
+"""
 from io import StringIO
 
 from isagog.model.kg_query import UnarySelectQuery, AtomicClause, Comparison, Variable, \
     ConjunctiveClause, DisjunctiveClause, _SCOREVAR, SelectQuery
 from isagog.model.kg_query import Generator, Clause
 
 
 class SPARQLGenerator(Generator):
+    """
+    SPARQL query generator
+    """
 
     def generate_clause(self, clause: Clause, **kwargs) -> str:
 
         if isinstance(clause, AtomicClause):
             """
             Generates the sparql triple clause
             """
@@ -99,34 +106,33 @@
             strio.write(f" {rv} ")
         if query.is_scored():
             strio.write(f" ?{_SCOREVAR} ")
         strio.write(" WHERE {\n")
         if query.has_disjunctive_clauses():
             strio.write("\t{\n")
             for clause in query.atom_clauses():
-                strio.write("\t\t" + clause.to_sparql())
+                strio.write("\t\t" + self.generate_clause(clause))  # clause.to_sparql()
             for clause in query.conjunctive_clauses():
-                strio.write("\t\t" + clause.to_sparql())
+                strio.write("\t\t" + self.generate_clause(clause))  # clause.to_sparql()
 
             strio.write("\t}\n")
 
             for clause in query.disjunctive_clauses():
-                strio.write(clause.to_sparql())
-            # strio.write("\t}\n")
+                strio.write(self.generate_clause(clause))  # clause.to_sparql()
+
         else:
             for clause in query.clauses:
-                strio.write("\t" + clause.to_sparql())
+                strio.write("\t" + self.generate_clause(clause))  # clause.to_sparql()
 
         if query.min_score:
             strio.write(f'\tFILTER (?{_SCOREVAR} >= {query.min_score})\n')
 
         strio.write("}\n")
         if query.is_scored():
             strio.write(f"ORDER BY DESC(?{_SCOREVAR})\n")
         if query.limit > 0:
             strio.write(f"LIMIT {query.limit}\n")
 
         return strio.getvalue()
 
 
 _SPARQLGEN = SPARQLGenerator()
-
```

### Comparing `isagog_ai-0.7.9/isagog/model/kg_model.py` & `isagog_ai-0.8.0/isagog/model/kg_model.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,29 @@
 """
-KG model
+    A model for Knowledge Graph entities and relations
+    (c) Isagog S.r.l. 2024, MIT License
 """
-import logging
-from typing import IO, Optional, TextIO, Any
+
+from typing import IO, TextIO, Any
 
 from rdflib import OWL, Graph, RDF, URIRef, RDFS
 
-log = logging.getLogger("isagog-cli")
+# Type definitions
+
+ID = URIRef | str  # Identifier type
+
+ALLOWED_TYPES = [OWL.Axiom, OWL.NamedIndividual, OWL.ObjectProperty, OWL.DatatypeProperty, OWL.Class]
 
 
 def _uri_label(uri: str) -> str:
+    """
+    Extracts a label from a URI
+    :param uri:
+    :return:
+    """
     if "#" in uri:
         return uri.split("#")[-1]
     elif "/" in uri:
         return uri.split("/")[-1]
     else:
         return uri
 
@@ -40,22 +50,14 @@
         if classkey is not None and hasattr(obj, "__class__"):
             data[classkey] = obj.__class__.__name__
         return data
     else:
         return obj
 
 
-ID = URIRef | str
-"""
-  Identifier type
-"""
-
-ALLOWED_TYPES = [OWL.Axiom, OWL.NamedIndividual, OWL.ObjectProperty, OWL.DatatypeProperty, OWL.Class]
-
-
 class Entity(object):
     """
     Any identified knowledge entity, either predicative (property) or individual
     """
 
     def __init__(self, _id: ID, **kwargs):
         assert _id
@@ -110,15 +112,15 @@
 
 class Attribute(Entity):
     """
     Assertions ranging on concrete domains
     owl:DatatypeProperties
     """
 
-    def __init__(self, _id: ID,  **kwargs):
+    def __init__(self, _id: ID, **kwargs):
         """
 
         :param _id:
         :param kwargs: domain
         """
         kwargs['owl'] = OWL.DatatypeProperty
         super().__init__(_id, **kwargs)
@@ -295,34 +297,39 @@
 
 
 VOID_ATTRIBUTE = AttributeInstance(id='http://isagog.com/attribute#void')
 
 
 class RelationInstance(Assertion):
     """
-    Relation instance as defined in
+    Relational assertion, as defined in
     isagog_api/openapi/isagog_kg.openapi.yaml
     """
 
     def __init__(self, **kwargs):
         predicate = kwargs.get('property', kwargs.get('id', KeyError("missing relation property")))
         values = kwargs.get('values', [])
         if values:
             specimen = values[0]
             if isinstance(specimen, Individual):
                 pass
-            elif isinstance(specimen,dict):
+            elif isinstance(specimen, dict):
                 inst_values = [Individual(_id=r_data.get('id'), **r_data) for r_data in values]
                 values = inst_values
             else:
                 raise ValueError("bad values for relation instance")
         super().__init__(predicate=predicate,
                          values=values)
 
     def all_values(self, only_id=True) -> list:
+        """
+        Returns all values of the relation instance
+        :param only_id:
+        :return:
+        """
         if only_id:
             return [ind.id for ind in self.values]
         else:
             return self.values
 
     def first_value(self, only_id=True, default=None) -> Any | None:
         if len(self.values) > 0:
@@ -339,15 +346,15 @@
     def kind_map(self) -> dict:
         """
         Returns a map of individuals by kind
         :return: a map of kind : individuals
         """
         kind_map = {}
         for individual in self.values:
-            for kind in individual.kinds:
+            for kind in individual.kind:
                 if kind not in kind_map:
                     kind_map[kind] = []
                 kind_map[kind].append(individual)
         return kind_map
 
 
 VOID_RELATION = RelationInstance(predicate='http://isagog.com/relation#void')
@@ -360,51 +367,75 @@
     (Individual)
     """
 
     def __init__(self, _id: ID, **kwargs):
         super().__init__(_id, **kwargs)
         self.__owl__ = OWL.NamedIndividual
         self.label = kwargs.get('label', _uri_label(self.id))
-        self.kinds = kwargs.get('kinds', [OWL.Thing])
+        self.kind = kwargs.get('kind', kwargs.get('kinds', [OWL.Thing]))  # back compatibility w 0.7
         self.comment = kwargs.get('comment', '')
         self.attributes = [AttributeInstance(**a_data) for a_data in
                            kwargs.get('attributes', list[AttributeInstance]())]
         self.relations = [RelationInstance(**r_data) for r_data in kwargs.get('relations', list[RelationInstance]())]
-        self.score = float(kwargs.get('score', 0.0))
+        if 'score' in kwargs:
+            self.score = float(kwargs.get('score'))
         if self.has_attribute("https://isagog.com/ontology#profile"):
             self.profile = {
                 profile_value.split("=")[0]: int(profile_value.split("=")[1])
                 for profile_value in self.get_attribute("https://isagog.com/ontology#profile").values
             }
         else:
             self.profile = {}
 
-    def has_attribute(self, attribute_id: str) -> bool:
+    def has_attribute(self, attribute_id: ID) -> bool:
+        """
+        Checks if the individual has a given ontology defined attribute
+        :param attribute_id:
+        :return:
+        """
         found = next(filter(lambda x: x.property == attribute_id, self.attributes), None)
         return found and not found.is_empty()
 
-    def get_attribute(self, attribute_id: str) -> AttributeInstance | Any:
+    def get_attribute(self, attribute_id: ID) -> AttributeInstance | Any:
+        """
+        Gets the ontology defined attribute instance of the individual
+        :param attribute_id:
+        :return:
+        """
         found = next(filter(lambda x: x.property == attribute_id, self.attributes), None)
         if found and not found.is_empty():
             return found
         else:
             return VOID_ATTRIBUTE
 
-    def has_relation(self, relation_id: str) -> bool:
+    def has_relation(self, relation_id: ID) -> bool:
+        """
+        Checks if the individual has a given ontology defined relation
+        :param relation_id:
+        :return:
+        """
         found = next(filter(lambda x: x.property == relation_id, self.relations), None)
         return found and not found.is_empty()
 
-    def get_relation(self, relation_id: str) -> RelationInstance | Any:
+    def get_relation(self, relation_id: ID) -> RelationInstance | Any:
+        """
+        Gets the ontology defined relation instance of the individual
+        :param relation_id:
+        :return:
+        """
         found = next(filter(lambda x: x.property == relation_id, self.relations), None)
         if found and not found.is_empty():
             return found
         else:
             return VOID_RELATION
 
     def set_score(self, score: float):
         self.score = score
 
     def get_score(self) -> float | None:
-        return self.score
+        if hasattr(self, 'score'):
+            return self.score
+        else:
+            return None
 
     def has_score(self) -> bool:
-        return self.score is not None
+        return hasattr(self, 'score')
```

### Comparing `isagog_ai-0.7.9/isagog/model/kg_query.py` & `isagog_ai-0.8.0/isagog/model/kg_query.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """
-KG Query module
+    A model for knowledge graph queries
+    The model is based on a triple query language (subject, property, argument)
+    (c) Isagog S.r.l. 2024, MIT License
 """
 from __future__ import annotations
 import logging
 import random
 import re
 from enum import Enum
 from typing import Protocol
@@ -15,18 +17,14 @@
                     ("text", "http://jena.apache.org/text")]
 
 # don't change this for the sake of back compatibility
 _SUBJVAR = 'i'
 _KINDVAR = 'k'
 _SCOREVAR = 'score'
 
-"""
-  Support deprecated methods
-"""
-
 
 class Comparison(Enum):
     EXACT = "exact_match"
     KEYWORD = "keyword_search"
     REGEX = "regex"
     SIMILARITY = "similarity"
     GREATER = "greater_than"
@@ -56,14 +54,15 @@
             value = str(_id)
         return super(Identifier, cls).__new__(cls, _id)
 
     def n3(self):
         return URIRef(self).n3()
 
 
+# The following are predefined identifiers
 RDF_TYPE = Identifier(RDF.type)
 RDFS_LABEL = Identifier(RDFS.label)
 OWL_CLASS = Identifier(OWL.Class)
 
 
 class Variable(str):
     """
@@ -116,28 +115,23 @@
         self.value = value
 
     def __str__(self) -> str:
         return str(self.value)
 
 
 class Clause(object):
-
+    """
+    A selection clause
+    """
     def __init__(self,
                  subject: Identifier | Variable | str = None,
                  optional=False):
         self.subject = subject
         self.optional = optional
 
-    def to_sparql(self) -> str:
-        """
-        Deprecated, use a SPARQL generator instead
-        :return:
-        """
-        pass
-
     def to_dict(self, **kwargs) -> dict:
         pass
 
     def is_defined(self) -> bool:
         return self.subject is not None
 
     def from_dict(self, data: dict, **kwargs):
@@ -154,14 +148,17 @@
         pass
 
     def generate_clause(self, clause: Clause, **kwargs) -> str:
         pass
 
 
 class AtomicClause(Clause):
+    """
+    A single triple clause
+    """
 
     @staticmethod
     def _instantiate_argument(arg) -> Value | Identifier | Variable:
         if isinstance(arg, Variable) or isinstance(arg, Identifier) or isinstance(arg, Value):
             return arg
         elif isinstance(arg, URIRef):
             return Identifier(arg)
@@ -172,15 +169,14 @@
             if arg.startswith('?'):
                 return Variable(arg)
             elif arg.startswith('<') or ':' in arg[:8]:
                 return Identifier(arg)
             else:
                 return Value(arg)
 
-
     @staticmethod
     def _instantiate_variable(variable) -> Variable:
         if isinstance(variable, Variable):
             return variable
         else:
             return Variable(variable)
 
@@ -201,16 +197,22 @@
                  property: Identifier | str = None,  # no property variable allowed
                  argument: str | int | float | Value | Identifier | Variable = None,
                  variable: Variable | str = None,
                  method: Comparison = Comparison.ANY,
                  project=True,
                  optional=False):
         """
-        A select clause
 
+        :param subject:
+        :param property:
+        :param argument:
+        :param variable:
+        :param method:
+        :param project:
+        :param optional:
         """
 
         super().__init__(subject=subject, optional=optional)
 
         self.subject = subject
         if self.subject and isinstance(subject, str):
             self.subject = Variable(subject) if subject.startswith("?") else Identifier(subject)
@@ -223,25 +225,17 @@
         self.project = project
 
     def is_defined(self) -> bool:
         return (self.subject is not None
                 and self.property is not None
                 and (self.argument is not None or self.variable is not None))
 
-    def to_sparql(self) -> str:
-        """
-        Deprecated
-        Generates the sparql triple clause
-        """
-        from isagog.generator.sparql_generator import _SPARQLGEN
-
-        return _SPARQLGEN.generate_clause(self)
-
     def to_dict(self, **kwargs) -> dict:
         out = {
+            'type': 'atomic',
             'property': self.property,
             'method': self.method.value,
             'project': self.project,
             'optional': self.optional
         }
         if self.subject:
             out['subject'] = self.subject
@@ -251,20 +245,14 @@
             elif isinstance(self.argument, Variable):
                 out['variable'] = self.argument
             else:
                 out['identifier'] = self.argument
         if self.variable:
             out['variable'] = self.variable
 
-        match kwargs.get('version', 'latest'):
-            case 'latest':
-                out['type'] = "atomic"
-            case "v1.0.0":
-                pass
-
         return out
 
     def from_dict(self, data: dict, **kwargs):
         """
         Openapi spec:  components.schemas.Clause
         """
         subject = kwargs.get('subject')  #: Variable | Identifier,
@@ -323,15 +311,14 @@
                     self.project = bool(val)
                 case 'optional':
                     self.optional = bool(val)
                 case _:
                     raise ValueError(f"Invalid clause key {key}")
 
 
-
 class CompositeClause(Clause):
     """
         A list of atomic clauses
     """
 
     def __init__(self,
                  subject: Identifier | Variable = None,
@@ -370,24 +357,25 @@
 
     def __init__(self,
                  clauses: list[Clause] = None,
                  optional=False):
         super().__init__(clauses=clauses,
                          optional=optional)
 
-    def to_sparql(self) -> str:
-        """
-        Deprecated
-        :return:
-        """
-        from isagog.generator.sparql_generator import _SPARQLGEN
-        return _SPARQLGEN.generate_clause(self)
+    # def to_sparql(self) -> str:
+    #     """
+    #     Deprecated
+    #     :return:
+    #     """
+    #     from isagog.generator.sparql_generator import _SPARQLGEN
+    #     return _SPARQLGEN.generate_clause(self)
 
     def to_dict(self, **kwargs) -> dict:
         out = {
+            'type': 'conjunction',
             'clauses': [c.to_dict() for c in self.clauses]
         }
 
         match kwargs.get('version', 'latest'):
             case "latest":
                 out['type'] = "conjunction"
             case "v1.0.0":
@@ -433,24 +421,19 @@
 
     def to_sparql(self) -> str:
         from isagog.generator.sparql_generator import _SPARQLGEN
         return _SPARQLGEN.generate_clause(self)
 
     def to_dict(self, **kwargs) -> dict:
         out = {
+            'type': 'union',
             'subject': self.subject,
             'clauses': [c.to_dict() for c in self.clauses]
         }
 
-        match kwargs.get('version', "latest"):
-            case "latest":
-                out['type'] = "union"
-            case "v1.0.0":
-                pass
-
         return out
 
     def from_dict(self, data: dict, **kwargs):
         subject = kwargs.get('subject', self.subject)
         for atom_dict in data.get('clauses', []):
             atom = AtomicClause()
             atom.from_dict(data=atom_dict,
@@ -516,15 +499,14 @@
         :param property:
         :param subject:
         :param argument:
         :param variable:
         :param method:
         :param project:
         :param optional:
-        :param kwargs:
         :return:
         """
         atomic_clause = AtomicClause(property=property,
                                      subject=subject,
                                      argument=argument,
                                      variable=variable,
                                      method=method,
@@ -551,21 +533,21 @@
                 if isinstance(c.subject, Variable):
                     _vars.append(c.subject)
         return set(_vars)
 
     def has_return_vars(self) -> bool:
         return len(self.project_vars()) > 0
 
-    def to_sparql(self) -> str:
-        """
-        This method is deprecated and will be removed in a future version.
-
-        Use generate_query with a SPARQL generator instead.
-        """
-        raise NotImplementedError()
+    # def to_sparql(self) -> str:
+    #     """
+    #     This method is deprecated and will be removed in a future version.
+    #
+    #     Use generate_query with a SPARQL generator instead.
+    #     """
+    #     raise NotImplementedError()
 
     def generate(self, generator: Generator) -> str:
         return generator.generate_query(self)
 
     def to_dict(self, version: str = None) -> dict:
         pass
 
@@ -681,27 +663,31 @@
            Openapi spec:  components.schemas.Clause
         """
         try:
             for key, val in data.items():
                 match key:
                     case 'subject':
                         self.subject = self._new_id(val)
-                    case 'kinds':
+                    case 'kind' | 'kinds':  # backward compatibility w 0.7
                         self.add_kinds(val)
                     case 'clauses':
                         for clause_data in val:
-                            match clause_data.get('type', 'atomic'):
+                            match clause_data.get('type'):
                                 case 'atomic':
                                     clause = AtomicClause()
                                 case 'union':
                                     clause = DisjunctiveClause()
                                 case 'conjunction':
                                     clause = ConjunctiveClause()
                                 case _:
-                                    raise ValueError(f"Clause type unknown")
+                                    if 'clauses' in clause_data:
+                                        # if not otherwise specified, assume a conjunction
+                                        clause = ConjunctiveClause()
+                                    else:
+                                        clause = AtomicClause()
                             subject = clause_data.get('subject', self.subject)
                             clause.from_dict(data=clause_data, subject=subject)
                             self.add(clause)
                     case 'graph':
                         self.graph = str(val)
                     case 'limit':
                         self.limit = int(val)
@@ -712,28 +698,28 @@
                     case 'dataset':
                         pass
                     case _:
                         logging.error("Illegal key %s", key)
         except Exception as e:
             raise ValueError(f"Malformed query due to: {e}")
 
-    def to_sparql(self) -> str:
-        """
-        Deprecated
-        :return:
-
-        """
-        from isagog.generator.sparql_generator import _SPARQLGEN
-
-        return _SPARQLGEN.generate_query(self)
+    # def to_sparql(self) -> str:
+    #     """
+    #     Deprecated
+    #     :return:
+    #
+    #     """
+    #     from isagog.generator.sparql_generator import _SPARQLGEN
+    #
+    #     return _SPARQLGEN.generate_query(self)
 
-    def to_dict(self, version="latest") -> dict:
+    def to_dict(self, version=None) -> dict:
 
         out = {}
-        if version == "latest" or version > "v1.0.0":
+        if version is None or version > "1.0.0":
             out['subject'] = self.subject
 
         out['clauses'] = [c.to_dict(version=version) for c in self.clauses]
         out['graph'] = self.graph
         out['limit'] = self.limit
         out['lang'] = self.lang
         if self.min_score:
```

### Comparing `isagog_ai-0.7.9/LICENSE` & `isagog_ai-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `isagog_ai-0.7.9/pyproject.toml` & `isagog_ai-0.8.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b74 6f6f 6c2e 706f 6574 7279 5d0d 0a6e  [tool.poetry]..n
 00000010: 616d 6520 3d20 2269 7361 676f 672d 6169  ame = "isagog-ai
 00000020: 220d 0a76 6572 7369 6f6e 203d 2022 302e  "..version = "0.
-00000030: 372e 3922 0d0a 6465 7363 7269 7074 696f  7.9"..descriptio
+00000030: 382e 3022 0d0a 6465 7363 7269 7074 696f  8.0"..descriptio
 00000040: 6e20 3d20 2263 6c69 656e 7420 666f 7220  n = "client for 
 00000050: 6973 6167 6f67 2061 6920 7365 7276 6963  isagog ai servic
 00000060: 6573 220d 0a61 7574 686f 7273 203d 205b  es"..authors = [
 00000070: 2247 7569 646f 2056 6574 6572 6520 3c67  "Guido Vetere <g
 00000080: 2e76 6574 6572 6540 6973 6167 6f67 2e63  .vetere@isagog.c
 00000090: 6f6d 3e22 5d0d 0a72 6561 646d 6520 3d20  om>"]..readme = 
 000000a0: 2252 4541 444d 452e 6d64 220d 0a70 6163  "README.md"..pac
@@ -21,16 +21,16 @@
 00000140: 2e64 6570 656e 6465 6e63 6965 735d 0d0a  .dependencies]..
 00000150: 7079 7468 6f6e 203d 2022 5e33 2e31 3022  python = "^3.10"
 00000160: 0d0a 7264 666c 6962 203d 2022 5e37 2e30  ..rdflib = "^7.0
 00000170: 2e30 220d 0a72 6571 7565 7374 7320 3d20  .0"..requests = 
 00000180: 225e 322e 3238 2e32 220d 0a75 726c 6c69  "^2.28.2"..urlli
 00000190: 6233 203d 2022 5e32 2e30 2e36 220d 0a74  b3 = "^2.0.6"..t
 000001a0: 6f6d 6c20 3d20 225e 302e 3130 2e32 220d  oml = "^0.10.2".
-000001b0: 0a70 7974 6573 7420 3d20 225e 372e 342e  .pytest = "^7.4.
-000001c0: 3322 0d0a 7079 7468 6f6e 2d64 6f74 656e  3"..python-doten
+000001b0: 0a70 7974 6573 7420 3d20 225e 382e 312e  .pytest = "^8.1.
+000001c0: 3122 0d0a 7079 7468 6f6e 2d64 6f74 656e  1"..python-doten
 000001d0: 7620 3d20 225e 312e 302e 3022 0d0a 0d0a  v = "^1.0.0"....
 000001e0: 0d0a 5b62 7569 6c64 2d73 7973 7465 6d5d  ..[build-system]
 000001f0: 0d0a 7265 7175 6972 6573 203d 205b 2270  ..requires = ["p
 00000200: 6f65 7472 792d 636f 7265 225d 0d0a 6275  oetry-core"]..bu
 00000210: 696c 642d 6261 636b 656e 6420 3d20 2270  ild-backend = "p
 00000220: 6f65 7472 792e 636f 7265 2e6d 6173 6f6e  oetry.core.mason
 00000230: 7279 2e61 7069 220d 0a                   ry.api"..
```

### Comparing `isagog_ai-0.7.9/PKG-INFO` & `isagog_ai-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: isagog-ai
-Version: 0.7.9
+Version: 0.8.0
 Summary: client for isagog ai services
 Author: Guido Vetere
 Author-email: g.vetere@isagog.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: pytest (>=7.4.3,<8.0.0)
+Requires-Dist: pytest (>=8.1.1,<9.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: rdflib (>=7.0.0,<8.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: urllib3 (>=2.0.6,<3.0.0)
 Description-Content-Type: text/markdown
```

