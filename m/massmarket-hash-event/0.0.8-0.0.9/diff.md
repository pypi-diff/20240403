# Comparing `tmp/massmarket_hash_event-0.0.8.tar.gz` & `tmp/massmarket_hash_event-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "massmarket_hash_event-0.0.8.tar", last modified: Tue Apr  2 20:32:25 2024, max compression
+gzip compressed data, was "massmarket_hash_event-0.0.9.tar", last modified: Wed Apr  3 13:56:31 2024, max compression
```

## Comparing `massmarket_hash_event-0.0.8.tar` & `massmarket_hash_event-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 cryptix   (1001) users      (100)        0 2024-04-02 20:32:25.389539 massmarket_hash_event-0.0.8/
--rw-r--r--   0 cryptix   (1001) users      (100)      860 2024-04-02 20:32:25.389539 massmarket_hash_event-0.0.8/PKG-INFO
-drwxr-xr-x   0 cryptix   (1001) users      (100)        0 2024-04-02 20:32:25.388539 massmarket_hash_event-0.0.8/massmarket_hash_event/
--rw-r--r--   0 cryptix   (1001) users      (100)     4082 2024-04-02 20:21:48.000000 massmarket_hash_event-0.0.8/massmarket_hash_event/__init__.py
--rw-r--r--   0 cryptix   (1001) users      (100)    10779 2024-04-02 19:46:53.000000 massmarket_hash_event-0.0.8/massmarket_hash_event/schema_pb2.py
--rw-r--r--   0 cryptix   (1001) users      (100)    16470 2024-04-02 19:46:53.000000 massmarket_hash_event-0.0.8/massmarket_hash_event/schema_pb2.pyi
--rw-r--r--   0 cryptix   (1001) users      (100)     3038 2024-04-02 19:49:12.000000 massmarket_hash_event-0.0.8/massmarket_hash_event/typedData.json
-drwxr-xr-x   0 cryptix   (1001) users      (100)        0 2024-04-02 20:32:25.388539 massmarket_hash_event-0.0.8/massmarket_hash_event.egg-info/
--rw-r--r--   0 cryptix   (1001) users      (100)      860 2024-04-02 20:32:25.000000 massmarket_hash_event-0.0.8/massmarket_hash_event.egg-info/PKG-INFO
--rw-r--r--   0 cryptix   (1001) users      (100)      428 2024-04-02 20:32:25.000000 massmarket_hash_event-0.0.8/massmarket_hash_event.egg-info/SOURCES.txt
--rw-r--r--   0 cryptix   (1001) users      (100)        1 2024-04-02 20:32:25.000000 massmarket_hash_event-0.0.8/massmarket_hash_event.egg-info/dependency_links.txt
--rw-r--r--   0 cryptix   (1001) users      (100)       20 2024-04-02 20:32:25.000000 massmarket_hash_event-0.0.8/massmarket_hash_event.egg-info/requires.txt
--rw-r--r--   0 cryptix   (1001) users      (100)       22 2024-04-02 20:32:25.000000 massmarket_hash_event-0.0.8/massmarket_hash_event.egg-info/top_level.txt
--rw-r--r--   0 cryptix   (1001) users      (100)     1390 2024-04-02 20:32:20.000000 massmarket_hash_event-0.0.8/pyproject.toml
--rw-r--r--   0 cryptix   (1001) users      (100)       38 2024-04-02 20:32:25.389539 massmarket_hash_event-0.0.8/setup.cfg
-drwxr-xr-x   0 cryptix   (1001) users      (100)        0 2024-04-02 20:32:25.389539 massmarket_hash_event-0.0.8/tests/
--rw-r--r--   0 cryptix   (1001) users      (100)     1266 2024-04-02 19:44:37.000000 massmarket_hash_event-0.0.8/tests/test_encode.py
--rw-r--r--   0 cryptix   (1001) users      (100)     6071 2024-04-02 20:25:46.000000 massmarket_hash_event-0.0.8/tests/test_signatures.py
+drwxr-xr-x   0 cryptix   (1001) users      (100)        0 2024-04-03 13:56:31.878405 massmarket_hash_event-0.0.9/
+-rw-r--r--   0 cryptix   (1001) users      (100)      860 2024-04-03 13:56:31.878405 massmarket_hash_event-0.0.9/PKG-INFO
+drwxr-xr-x   0 cryptix   (1001) users      (100)        0 2024-04-03 13:56:31.877405 massmarket_hash_event-0.0.9/massmarket_hash_event/
+-rw-r--r--   0 cryptix   (1001) users      (100)     3967 2024-04-03 13:54:58.000000 massmarket_hash_event-0.0.9/massmarket_hash_event/__init__.py
+-rw-r--r--   0 cryptix   (1001) users      (100)    10811 2024-04-03 13:54:58.000000 massmarket_hash_event-0.0.9/massmarket_hash_event/schema_pb2.py
+-rw-r--r--   0 cryptix   (1001) users      (100)    16441 2024-04-03 13:54:58.000000 massmarket_hash_event-0.0.9/massmarket_hash_event/schema_pb2.pyi
+-rw-r--r--   0 cryptix   (1001) users      (100)     2976 2024-04-03 13:52:41.000000 massmarket_hash_event-0.0.9/massmarket_hash_event/typedData.json
+drwxr-xr-x   0 cryptix   (1001) users      (100)        0 2024-04-03 13:56:31.877405 massmarket_hash_event-0.0.9/massmarket_hash_event.egg-info/
+-rw-r--r--   0 cryptix   (1001) users      (100)      860 2024-04-03 13:56:31.000000 massmarket_hash_event-0.0.9/massmarket_hash_event.egg-info/PKG-INFO
+-rw-r--r--   0 cryptix   (1001) users      (100)      428 2024-04-03 13:56:31.000000 massmarket_hash_event-0.0.9/massmarket_hash_event.egg-info/SOURCES.txt
+-rw-r--r--   0 cryptix   (1001) users      (100)        1 2024-04-03 13:56:31.000000 massmarket_hash_event-0.0.9/massmarket_hash_event.egg-info/dependency_links.txt
+-rw-r--r--   0 cryptix   (1001) users      (100)       20 2024-04-03 13:56:31.000000 massmarket_hash_event-0.0.9/massmarket_hash_event.egg-info/requires.txt
+-rw-r--r--   0 cryptix   (1001) users      (100)       22 2024-04-03 13:56:31.000000 massmarket_hash_event-0.0.9/massmarket_hash_event.egg-info/top_level.txt
+-rw-r--r--   0 cryptix   (1001) users      (100)     1390 2024-04-03 13:56:14.000000 massmarket_hash_event-0.0.9/pyproject.toml
+-rw-r--r--   0 cryptix   (1001) users      (100)       38 2024-04-03 13:56:31.878405 massmarket_hash_event-0.0.9/setup.cfg
+drwxr-xr-x   0 cryptix   (1001) users      (100)        0 2024-04-03 13:56:31.878405 massmarket_hash_event-0.0.9/tests/
+-rw-r--r--   0 cryptix   (1001) users      (100)     1266 2024-04-03 13:54:58.000000 massmarket_hash_event-0.0.9/tests/test_encode.py
+-rw-r--r--   0 cryptix   (1001) users      (100)     6058 2024-04-03 13:56:01.000000 massmarket_hash_event-0.0.9/tests/test_signatures.py
```

### Comparing `massmarket_hash_event-0.0.8/PKG-INFO` & `massmarket_hash_event-0.0.9/massmarket_hash_event.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: massmarket_hash_event
-Version: 0.0.8
+Name: massmarket-hash-event
+Version: 0.0.9
 Summary: Helper functions to hash events for signature creation and verification on Mass Market.
 Author-email: Henry Bubert <henry@mass.market>
 License: MIT
 Project-URL: Homepage, https://mass.market
 Project-URL: Repository, https://github.com/masslbs/network-schema.git
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `massmarket_hash_event-0.0.8/massmarket_hash_event/__init__.py` & `massmarket_hash_event-0.0.9/massmarket_hash_event/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,18 +55,16 @@
     # convert event to typedData
     event_td_data = event_to_typedData_dict(evt, event_td_spec)
     if event_name == "ChangeStock":
         # remove cart_id if empty
         if len(event_td_data["cart_id"]) == 0:
             event_td_spec.remove({"name": "cart_id", "type": "bytes32"})
             event_td_spec.remove({"name": "tx_hash", "type": "bytes32"})
-            event_td_spec.remove({"name": "block_no", "type": "uint64"})
             del event_td_data["cart_id"]
             del event_td_data["tx_hash"]
-            del event_td_data["block_no"]
     typed_data = {
         "types": {
             "EIP712Domain": [
                 {"name": "name", "type": "string"},
                 {"name": "version", "type": "string"},
                 {"name": "chainId", "type": "uint256"},
                 {"name": "verifyingContract", "type": "address"},
```

### Comparing `massmarket_hash_event-0.0.8/massmarket_hash_event/schema_pb2.py` & `massmarket_hash_event-0.0.9/massmarket_hash_event/schema_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2024 Mass Labs
+#
+# SPDX-License-Identifier: MIT
+
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: schema.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
@@ -9,15 +13,15 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0cschema.proto\x12\x0bmarket.mass\"c\n\rStoreManifest\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\x0c\x12\x16\n\x0estore_token_id\x18\x02 \x01(\x0c\x12\x0e\n\x06\x64omain\x18\x03 \x01(\t\x12\x18\n\x10published_tag_id\x18\x04 \x01(\x0c\"\xcd\x02\n\x0eUpdateManifest\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\x0c\x12\x38\n\x05\x66ield\x18\x02 \x01(\x0e\x32).market.mass.UpdateManifest.ManifestField\x12\x10\n\x06string\x18\x03 \x01(\tH\x00\x12\x10\n\x06tag_id\x18\x04 \x01(\x0cH\x00\x12\x14\n\nerc20_addr\x18\x05 \x01(\x0cH\x00\"\xab\x01\n\rManifestField\x12\x1e\n\x1aMANIFEST_FIELD_UNSPECIFIED\x10\x00\x12\x19\n\x15MANIFEST_FIELD_DOMAIN\x10\x01\x12 \n\x1cMANIFEST_FIELD_PUBLISHED_TAG\x10\x02\x12\x1c\n\x18MANIFEST_FIELD_ADD_ERC20\x10\x03\x12\x1f\n\x1bMANIFEST_FIELD_REMOVE_ERC20\x10\x04\x42\x07\n\x05value\"?\n\nCreateItem\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\x0c\x12\r\n\x05price\x18\x02 \x01(\t\x12\x10\n\x08metadata\x18\x03 \x01(\x0c\"\xe7\x01\n\nUpdateItem\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\x0c\x12\x0f\n\x07item_id\x18\x02 \x01(\x0c\x12\x30\n\x05\x66ield\x18\x03 \x01(\x0e\x32!.market.mass.UpdateItem.ItemField\x12\x0f\n\x05price\x18\x04 \x01(\tH\x00\x12\x12\n\x08metadata\x18\x05 \x01(\x0cH\x00\"V\n\tItemField\x12\x1a\n\x16ITEM_FIELD_UNSPECIFIED\x10\x00\x12\x14\n\x10ITEM_FIELD_PRICE\x10\x01\x12\x17\n\x13ITEM_FIELD_METADATA\x10\x02\x42\x07\n\x05value\"+\n\tCreateTag\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\x0c\x12\x0c\n\x04name\x18\x02 \x01(\t\"=\n\x08\x41\x64\x64ToTag\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\x0c\x12\x0e\n\x06tag_id\x18\x02 \x01(\x0c\x12\x0f\n\x07item_id\x18\x03 \x01(\x0c\"B\n\rRemoveFromTag\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\x0c\x12\x0e\n\x06tag_id\x18\x02 \x01(\x0c\x12\x0f\n\x07item_id\x18\x03 \x01(\x0c\";\n\tRenameTag\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\x0c\x12\x0e\n\x06tag_id\x18\x02 \x01(\x0c\x12\x0c\n\x04name\x18\x03 \x01(\t\"-\n\tDeleteTag\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\x0c\x12\x0e\n\x06tag_id\x18\x02 \x01(\x0c\"t\n\x0b\x43hangeStock\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\x0c\x12\x10\n\x08item_ids\x18\x02 \x03(\x0c\x12\r\n\x05\x64iffs\x18\x03 \x03(\x11\x12\x0f\n\x07\x63\x61rt_id\x18\x04 \x01(\x0c\x12\x0f\n\x07tx_hash\x18\x05 \x01(\x0c\x12\x10\n\x08\x62lock_no\x18\x06 \x01(\x04\"Q\n\nNewKeyCard\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\x0c\x12\x18\n\x10user_wallet_addr\x18\x02 \x01(\x0c\x12\x17\n\x0f\x63\x61rd_public_key\x18\x03 \x01(\x0c\"\x1e\n\nCreateCart\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\x0c\"R\n\nChangeCart\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\x0c\x12\x0f\n\x07\x63\x61rt_id\x18\x02 \x01(\x0c\x12\x0f\n\x07item_id\x18\x03 \x01(\x0c\x12\x10\n\x08quantity\x18\x04 \x01(\x11\"\xa2\x05\n\x05\x45vent\x12\x11\n\tsignature\x18\x01 \x01(\x0c\x12\x34\n\x0estore_manifest\x18\x02 \x01(\x0b\x32\x1a.market.mass.StoreManifestH\x00\x12\x36\n\x0fupdate_manifest\x18\x03 \x01(\x0b\x32\x1b.market.mass.UpdateManifestH\x00\x12.\n\x0b\x63reate_item\x18\x04 \x01(\x0b\x32\x17.market.mass.CreateItemH\x00\x12.\n\x0bupdate_item\x18\x05 \x01(\x0b\x32\x17.market.mass.UpdateItemH\x00\x12,\n\ncreate_tag\x18\x06 \x01(\x0b\x32\x16.market.mass.CreateTagH\x00\x12+\n\nadd_to_tag\x18\x07 \x01(\x0b\x32\x15.market.mass.AddToTagH\x00\x12\x35\n\x0fremove_from_tag\x18\x08 \x01(\x0b\x32\x1a.market.mass.RemoveFromTagH\x00\x12,\n\nrename_tag\x18\t \x01(\x0b\x32\x16.market.mass.RenameTagH\x00\x12,\n\ndelete_tag\x18\n \x01(\x0b\x32\x16.market.mass.DeleteTagH\x00\x12.\n\x0b\x63reate_cart\x18\x0b \x01(\x0b\x32\x17.market.mass.CreateCartH\x00\x12.\n\x0b\x63hange_cart\x18\x0c \x01(\x0b\x32\x17.market.mass.ChangeCartH\x00\x12\x30\n\x0c\x63hange_stock\x18\r \x01(\x0b\x32\x18.market.mass.ChangeStockH\x00\x12/\n\x0cnew_key_card\x18\x0e \x01(\x0b\x32\x17.market.mass.NewKeyCardH\x00\x42\x07\n\x05union\"=\n\x13\x41uthenticateRequest\x12\x12\n\nrequest_id\x18\x01 \x01(\x0c\x12\x12\n\npublic_key\x18\x02 \x01(\x0c\"`\n\x14\x41uthenticateResponse\x12\x12\n\nrequest_id\x18\x01 \x01(\x0c\x12!\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x12.market.mass.Error\x12\x11\n\tchallenge\x18\x03 \x01(\x0c\"?\n\x16\x43hallengeSolvedRequest\x12\x12\n\nrequest_id\x18\x01 \x01(\x0c\x12\x11\n\tsignature\x18\x02 \x01(\x0c\"P\n\x17\x43hallengeSolvedResponse\x12\x12\n\nrequest_id\x18\x01 \x01(\x0c\x12!\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x12.market.mass.Error\"L\n\x11\x43ommitCartRequest\x12\x12\n\nrequest_id\x18\x01 \x01(\x0c\x12\x0f\n\x07\x63\x61rt_id\x18\x02 \x01(\x0c\x12\x12\n\nerc20_addr\x18\x03 \x01(\x0c\"\xea\x01\n\x12\x43ommitCartResponse\x12\x12\n\nrequest_id\x18\x01 \x01(\x0c\x12!\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x12.market.mass.Error\x12\x18\n\x10purchase_address\x18\x03 \x01(\x0c\x12;\n\x06totals\x18\x04 \x03(\x0b\x32+.market.mass.CommitCartResponse.TotalsEntry\x12\x17\n\x0ftotal_in_crypto\x18\x05 \x01(\t\x1a-\n\x0bTotalsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"-\n\x17GetBlobUploadURLRequest\x12\x12\n\nrequest_id\x18\x01 \x01(\x0c\"^\n\x18GetBlobUploadURLResponse\x12\x12\n\nrequest_id\x18\x01 \x01(\x0c\x12!\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x12.market.mass.Error\x12\x0b\n\x03url\x18\x03 \x01(\t\"J\n\x11\x45ventWriteRequest\x12\x12\n\nrequest_id\x18\x01 \x01(\x0c\x12!\n\x05\x65vent\x18\x02 \x01(\x0b\x32\x12.market.mass.Event\"~\n\x12\x45ventWriteResponse\x12\x12\n\nrequest_id\x18\x01 \x01(\x0c\x12!\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x12.market.mass.Error\x12\x16\n\x0enew_store_hash\x18\x03 \x01(\x0c\x12\x19\n\x11\x65vent_sequence_no\x18\x04 \x01(\x04\"@\n\x11SyncStatusRequest\x12\x12\n\nrequest_id\x18\x01 \x01(\x0c\x12\x17\n\x0funpushed_events\x18\x02 \x01(\x04\"K\n\x12SyncStatusResponse\x12\x12\n\nrequest_id\x18\x01 \x01(\x0c\x12!\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x12.market.mass.Error\"J\n\x10\x45ventPushRequest\x12\x12\n\nrequest_id\x18\x01 \x01(\x0c\x12\"\n\x06\x65vents\x18\x02 \x03(\x0b\x32\x12.market.mass.Event\"J\n\x11\x45ventPushResponse\x12\x12\n\nrequest_id\x18\x01 \x01(\x0c\x12!\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x12.market.mass.Error\"!\n\x0bPingRequest\x12\x12\n\nrequest_id\x18\x01 \x01(\x0c\"E\n\x0cPingResponse\x12\x12\n\nrequest_id\x18\x01 \x01(\x0c\x12!\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x12.market.mass.Error\"&\n\x05\x45rror\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\x0f\n\x07message\x18\x02 \x01(\tb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0cschema.proto\x12\x0bmarket.mass\"c\n\rStoreManifest\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\x0c\x12\x16\n\x0estore_token_id\x18\x02 \x01(\x0c\x12\x0e\n\x06\x64omain\x18\x03 \x01(\t\x12\x18\n\x10published_tag_id\x18\x04 \x01(\x0c\"\xcd\x02\n\x0eUpdateManifest\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\x0c\x12\x38\n\x05\x66ield\x18\x02 \x01(\x0e\x32).market.mass.UpdateManifest.ManifestField\x12\x10\n\x06string\x18\x03 \x01(\tH\x00\x12\x10\n\x06tag_id\x18\x04 \x01(\x0cH\x00\x12\x14\n\nerc20_addr\x18\x05 \x01(\x0cH\x00\"\xab\x01\n\rManifestField\x12\x1e\n\x1aMANIFEST_FIELD_UNSPECIFIED\x10\x00\x12\x19\n\x15MANIFEST_FIELD_DOMAIN\x10\x01\x12 \n\x1cMANIFEST_FIELD_PUBLISHED_TAG\x10\x02\x12\x1c\n\x18MANIFEST_FIELD_ADD_ERC20\x10\x03\x12\x1f\n\x1bMANIFEST_FIELD_REMOVE_ERC20\x10\x04\x42\x07\n\x05value\"?\n\nCreateItem\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\x0c\x12\r\n\x05price\x18\x02 \x01(\t\x12\x10\n\x08metadata\x18\x03 \x01(\x0c\"\xe7\x01\n\nUpdateItem\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\x0c\x12\x0f\n\x07item_id\x18\x02 \x01(\x0c\x12\x30\n\x05\x66ield\x18\x03 \x01(\x0e\x32!.market.mass.UpdateItem.ItemField\x12\x0f\n\x05price\x18\x04 \x01(\tH\x00\x12\x12\n\x08metadata\x18\x05 \x01(\x0cH\x00\"V\n\tItemField\x12\x1a\n\x16ITEM_FIELD_UNSPECIFIED\x10\x00\x12\x14\n\x10ITEM_FIELD_PRICE\x10\x01\x12\x17\n\x13ITEM_FIELD_METADATA\x10\x02\x42\x07\n\x05value\"+\n\tCreateTag\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\x0c\x12\x0c\n\x04name\x18\x02 \x01(\t\"=\n\x08\x41\x64\x64ToTag\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\x0c\x12\x0e\n\x06tag_id\x18\x02 \x01(\x0c\x12\x0f\n\x07item_id\x18\x03 \x01(\x0c\"B\n\rRemoveFromTag\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\x0c\x12\x0e\n\x06tag_id\x18\x02 \x01(\x0c\x12\x0f\n\x07item_id\x18\x03 \x01(\x0c\";\n\tRenameTag\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\x0c\x12\x0e\n\x06tag_id\x18\x02 \x01(\x0c\x12\x0c\n\x04name\x18\x03 \x01(\t\"-\n\tDeleteTag\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\x0c\x12\x0e\n\x06tag_id\x18\x02 \x01(\x0c\"b\n\x0b\x43hangeStock\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\x0c\x12\x10\n\x08item_ids\x18\x02 \x03(\x0c\x12\r\n\x05\x64iffs\x18\x03 \x03(\x11\x12\x0f\n\x07\x63\x61rt_id\x18\x04 \x01(\x0c\x12\x0f\n\x07tx_hash\x18\x05 \x01(\x0c\"Q\n\nNewKeyCard\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\x0c\x12\x18\n\x10user_wallet_addr\x18\x02 \x01(\x0c\x12\x17\n\x0f\x63\x61rd_public_key\x18\x03 \x01(\x0c\"\x1e\n\nCreateCart\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\x0c\"R\n\nChangeCart\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\x0c\x12\x0f\n\x07\x63\x61rt_id\x18\x02 \x01(\x0c\x12\x0f\n\x07item_id\x18\x03 \x01(\x0c\x12\x10\n\x08quantity\x18\x04 \x01(\x11\"\xa2\x05\n\x05\x45vent\x12\x11\n\tsignature\x18\x01 \x01(\x0c\x12\x34\n\x0estore_manifest\x18\x02 \x01(\x0b\x32\x1a.market.mass.StoreManifestH\x00\x12\x36\n\x0fupdate_manifest\x18\x03 \x01(\x0b\x32\x1b.market.mass.UpdateManifestH\x00\x12.\n\x0b\x63reate_item\x18\x04 \x01(\x0b\x32\x17.market.mass.CreateItemH\x00\x12.\n\x0bupdate_item\x18\x05 \x01(\x0b\x32\x17.market.mass.UpdateItemH\x00\x12,\n\ncreate_tag\x18\x06 \x01(\x0b\x32\x16.market.mass.CreateTagH\x00\x12+\n\nadd_to_tag\x18\x07 \x01(\x0b\x32\x15.market.mass.AddToTagH\x00\x12\x35\n\x0fremove_from_tag\x18\x08 \x01(\x0b\x32\x1a.market.mass.RemoveFromTagH\x00\x12,\n\nrename_tag\x18\t \x01(\x0b\x32\x16.market.mass.RenameTagH\x00\x12,\n\ndelete_tag\x18\n \x01(\x0b\x32\x16.market.mass.DeleteTagH\x00\x12.\n\x0b\x63reate_cart\x18\x0b \x01(\x0b\x32\x17.market.mass.CreateCartH\x00\x12.\n\x0b\x63hange_cart\x18\x0c \x01(\x0b\x32\x17.market.mass.ChangeCartH\x00\x12\x30\n\x0c\x63hange_stock\x18\r \x01(\x0b\x32\x18.market.mass.ChangeStockH\x00\x12/\n\x0cnew_key_card\x18\x0e \x01(\x0b\x32\x17.market.mass.NewKeyCardH\x00\x42\x07\n\x05union\"=\n\x13\x41uthenticateRequest\x12\x12\n\nrequest_id\x18\x01 \x01(\x0c\x12\x12\n\npublic_key\x18\x02 \x01(\x0c\"`\n\x14\x41uthenticateResponse\x12\x12\n\nrequest_id\x18\x01 \x01(\x0c\x12!\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x12.market.mass.Error\x12\x11\n\tchallenge\x18\x03 \x01(\x0c\"?\n\x16\x43hallengeSolvedRequest\x12\x12\n\nrequest_id\x18\x01 \x01(\x0c\x12\x11\n\tsignature\x18\x02 \x01(\x0c\"P\n\x17\x43hallengeSolvedResponse\x12\x12\n\nrequest_id\x18\x01 \x01(\x0c\x12!\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x12.market.mass.Error\"L\n\x11\x43ommitCartRequest\x12\x12\n\nrequest_id\x18\x01 \x01(\x0c\x12\x0f\n\x07\x63\x61rt_id\x18\x02 \x01(\x0c\x12\x12\n\nerc20_addr\x18\x03 \x01(\x0c\"\xea\x01\n\x12\x43ommitCartResponse\x12\x12\n\nrequest_id\x18\x01 \x01(\x0c\x12!\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x12.market.mass.Error\x12\x18\n\x10purchase_address\x18\x03 \x01(\x0c\x12;\n\x06totals\x18\x04 \x03(\x0b\x32+.market.mass.CommitCartResponse.TotalsEntry\x12\x17\n\x0ftotal_in_crypto\x18\x05 \x01(\t\x1a-\n\x0bTotalsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"-\n\x17GetBlobUploadURLRequest\x12\x12\n\nrequest_id\x18\x01 \x01(\x0c\"^\n\x18GetBlobUploadURLResponse\x12\x12\n\nrequest_id\x18\x01 \x01(\x0c\x12!\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x12.market.mass.Error\x12\x0b\n\x03url\x18\x03 \x01(\t\"J\n\x11\x45ventWriteRequest\x12\x12\n\nrequest_id\x18\x01 \x01(\x0c\x12!\n\x05\x65vent\x18\x02 \x01(\x0b\x32\x12.market.mass.Event\"~\n\x12\x45ventWriteResponse\x12\x12\n\nrequest_id\x18\x01 \x01(\x0c\x12!\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x12.market.mass.Error\x12\x16\n\x0enew_store_hash\x18\x03 \x01(\x0c\x12\x19\n\x11\x65vent_sequence_no\x18\x04 \x01(\x04\"@\n\x11SyncStatusRequest\x12\x12\n\nrequest_id\x18\x01 \x01(\x0c\x12\x17\n\x0funpushed_events\x18\x02 \x01(\x04\"K\n\x12SyncStatusResponse\x12\x12\n\nrequest_id\x18\x01 \x01(\x0c\x12!\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x12.market.mass.Error\"J\n\x10\x45ventPushRequest\x12\x12\n\nrequest_id\x18\x01 \x01(\x0c\x12\"\n\x06\x65vents\x18\x02 \x03(\x0b\x32\x12.market.mass.Event\"J\n\x11\x45ventPushResponse\x12\x12\n\nrequest_id\x18\x01 \x01(\x0c\x12!\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x12.market.mass.Error\"!\n\x0bPingRequest\x12\x12\n\nrequest_id\x18\x01 \x01(\x0c\"E\n\x0cPingResponse\x12\x12\n\nrequest_id\x18\x01 \x01(\x0c\x12!\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x12.market.mass.Error\"&\n\x05\x45rror\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\x0f\n\x07message\x18\x02 \x01(\tb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'schema_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   DESCRIPTOR._options = None
   _globals['_COMMITCARTRESPONSE_TOTALSENTRY']._options = None
@@ -41,53 +45,53 @@
   _globals['_REMOVEFROMTAG']._serialized_start=873
   _globals['_REMOVEFROMTAG']._serialized_end=939
   _globals['_RENAMETAG']._serialized_start=941
   _globals['_RENAMETAG']._serialized_end=1000
   _globals['_DELETETAG']._serialized_start=1002
   _globals['_DELETETAG']._serialized_end=1047
   _globals['_CHANGESTOCK']._serialized_start=1049
-  _globals['_CHANGESTOCK']._serialized_end=1165
-  _globals['_NEWKEYCARD']._serialized_start=1167
-  _globals['_NEWKEYCARD']._serialized_end=1248
-  _globals['_CREATECART']._serialized_start=1250
-  _globals['_CREATECART']._serialized_end=1280
-  _globals['_CHANGECART']._serialized_start=1282
-  _globals['_CHANGECART']._serialized_end=1364
-  _globals['_EVENT']._serialized_start=1367
-  _globals['_EVENT']._serialized_end=2041
-  _globals['_AUTHENTICATEREQUEST']._serialized_start=2043
-  _globals['_AUTHENTICATEREQUEST']._serialized_end=2104
-  _globals['_AUTHENTICATERESPONSE']._serialized_start=2106
-  _globals['_AUTHENTICATERESPONSE']._serialized_end=2202
-  _globals['_CHALLENGESOLVEDREQUEST']._serialized_start=2204
-  _globals['_CHALLENGESOLVEDREQUEST']._serialized_end=2267
-  _globals['_CHALLENGESOLVEDRESPONSE']._serialized_start=2269
-  _globals['_CHALLENGESOLVEDRESPONSE']._serialized_end=2349
-  _globals['_COMMITCARTREQUEST']._serialized_start=2351
-  _globals['_COMMITCARTREQUEST']._serialized_end=2427
-  _globals['_COMMITCARTRESPONSE']._serialized_start=2430
-  _globals['_COMMITCARTRESPONSE']._serialized_end=2664
-  _globals['_COMMITCARTRESPONSE_TOTALSENTRY']._serialized_start=2619
-  _globals['_COMMITCARTRESPONSE_TOTALSENTRY']._serialized_end=2664
-  _globals['_GETBLOBUPLOADURLREQUEST']._serialized_start=2666
-  _globals['_GETBLOBUPLOADURLREQUEST']._serialized_end=2711
-  _globals['_GETBLOBUPLOADURLRESPONSE']._serialized_start=2713
-  _globals['_GETBLOBUPLOADURLRESPONSE']._serialized_end=2807
-  _globals['_EVENTWRITEREQUEST']._serialized_start=2809
-  _globals['_EVENTWRITEREQUEST']._serialized_end=2883
-  _globals['_EVENTWRITERESPONSE']._serialized_start=2885
-  _globals['_EVENTWRITERESPONSE']._serialized_end=3011
-  _globals['_SYNCSTATUSREQUEST']._serialized_start=3013
-  _globals['_SYNCSTATUSREQUEST']._serialized_end=3077
-  _globals['_SYNCSTATUSRESPONSE']._serialized_start=3079
-  _globals['_SYNCSTATUSRESPONSE']._serialized_end=3154
-  _globals['_EVENTPUSHREQUEST']._serialized_start=3156
-  _globals['_EVENTPUSHREQUEST']._serialized_end=3230
-  _globals['_EVENTPUSHRESPONSE']._serialized_start=3232
-  _globals['_EVENTPUSHRESPONSE']._serialized_end=3306
-  _globals['_PINGREQUEST']._serialized_start=3308
-  _globals['_PINGREQUEST']._serialized_end=3341
-  _globals['_PINGRESPONSE']._serialized_start=3343
-  _globals['_PINGRESPONSE']._serialized_end=3412
-  _globals['_ERROR']._serialized_start=3414
-  _globals['_ERROR']._serialized_end=3452
+  _globals['_CHANGESTOCK']._serialized_end=1147
+  _globals['_NEWKEYCARD']._serialized_start=1149
+  _globals['_NEWKEYCARD']._serialized_end=1230
+  _globals['_CREATECART']._serialized_start=1232
+  _globals['_CREATECART']._serialized_end=1262
+  _globals['_CHANGECART']._serialized_start=1264
+  _globals['_CHANGECART']._serialized_end=1346
+  _globals['_EVENT']._serialized_start=1349
+  _globals['_EVENT']._serialized_end=2023
+  _globals['_AUTHENTICATEREQUEST']._serialized_start=2025
+  _globals['_AUTHENTICATEREQUEST']._serialized_end=2086
+  _globals['_AUTHENTICATERESPONSE']._serialized_start=2088
+  _globals['_AUTHENTICATERESPONSE']._serialized_end=2184
+  _globals['_CHALLENGESOLVEDREQUEST']._serialized_start=2186
+  _globals['_CHALLENGESOLVEDREQUEST']._serialized_end=2249
+  _globals['_CHALLENGESOLVEDRESPONSE']._serialized_start=2251
+  _globals['_CHALLENGESOLVEDRESPONSE']._serialized_end=2331
+  _globals['_COMMITCARTREQUEST']._serialized_start=2333
+  _globals['_COMMITCARTREQUEST']._serialized_end=2409
+  _globals['_COMMITCARTRESPONSE']._serialized_start=2412
+  _globals['_COMMITCARTRESPONSE']._serialized_end=2646
+  _globals['_COMMITCARTRESPONSE_TOTALSENTRY']._serialized_start=2601
+  _globals['_COMMITCARTRESPONSE_TOTALSENTRY']._serialized_end=2646
+  _globals['_GETBLOBUPLOADURLREQUEST']._serialized_start=2648
+  _globals['_GETBLOBUPLOADURLREQUEST']._serialized_end=2693
+  _globals['_GETBLOBUPLOADURLRESPONSE']._serialized_start=2695
+  _globals['_GETBLOBUPLOADURLRESPONSE']._serialized_end=2789
+  _globals['_EVENTWRITEREQUEST']._serialized_start=2791
+  _globals['_EVENTWRITEREQUEST']._serialized_end=2865
+  _globals['_EVENTWRITERESPONSE']._serialized_start=2867
+  _globals['_EVENTWRITERESPONSE']._serialized_end=2993
+  _globals['_SYNCSTATUSREQUEST']._serialized_start=2995
+  _globals['_SYNCSTATUSREQUEST']._serialized_end=3059
+  _globals['_SYNCSTATUSRESPONSE']._serialized_start=3061
+  _globals['_SYNCSTATUSRESPONSE']._serialized_end=3136
+  _globals['_EVENTPUSHREQUEST']._serialized_start=3138
+  _globals['_EVENTPUSHREQUEST']._serialized_end=3212
+  _globals['_EVENTPUSHRESPONSE']._serialized_start=3214
+  _globals['_EVENTPUSHRESPONSE']._serialized_end=3288
+  _globals['_PINGREQUEST']._serialized_start=3290
+  _globals['_PINGREQUEST']._serialized_end=3323
+  _globals['_PINGRESPONSE']._serialized_start=3325
+  _globals['_PINGRESPONSE']._serialized_end=3394
+  _globals['_ERROR']._serialized_start=3396
+  _globals['_ERROR']._serialized_end=3434
 # @@protoc_insertion_point(module_scope)
```

### Comparing `massmarket_hash_event-0.0.8/massmarket_hash_event/schema_pb2.pyi` & `massmarket_hash_event-0.0.9/massmarket_hash_event/schema_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2024 Mass Labs
+#
+# SPDX-License-Identifier: MIT
+
 from google.protobuf.internal import containers as _containers
 from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
@@ -119,28 +123,26 @@
     EVENT_ID_FIELD_NUMBER: _ClassVar[int]
     TAG_ID_FIELD_NUMBER: _ClassVar[int]
     event_id: bytes
     tag_id: bytes
     def __init__(self, event_id: _Optional[bytes] = ..., tag_id: _Optional[bytes] = ...) -> None: ...
 
 class ChangeStock(_message.Message):
-    __slots__ = ["event_id", "item_ids", "diffs", "cart_id", "tx_hash", "block_no"]
+    __slots__ = ["event_id", "item_ids", "diffs", "cart_id", "tx_hash"]
     EVENT_ID_FIELD_NUMBER: _ClassVar[int]
     ITEM_IDS_FIELD_NUMBER: _ClassVar[int]
     DIFFS_FIELD_NUMBER: _ClassVar[int]
     CART_ID_FIELD_NUMBER: _ClassVar[int]
     TX_HASH_FIELD_NUMBER: _ClassVar[int]
-    BLOCK_NO_FIELD_NUMBER: _ClassVar[int]
     event_id: bytes
     item_ids: _containers.RepeatedScalarFieldContainer[bytes]
     diffs: _containers.RepeatedScalarFieldContainer[int]
     cart_id: bytes
     tx_hash: bytes
-    block_no: int
-    def __init__(self, event_id: _Optional[bytes] = ..., item_ids: _Optional[_Iterable[bytes]] = ..., diffs: _Optional[_Iterable[int]] = ..., cart_id: _Optional[bytes] = ..., tx_hash: _Optional[bytes] = ..., block_no: _Optional[int] = ...) -> None: ...
+    def __init__(self, event_id: _Optional[bytes] = ..., item_ids: _Optional[_Iterable[bytes]] = ..., diffs: _Optional[_Iterable[int]] = ..., cart_id: _Optional[bytes] = ..., tx_hash: _Optional[bytes] = ...) -> None: ...
 
 class NewKeyCard(_message.Message):
     __slots__ = ["event_id", "user_wallet_addr", "card_public_key"]
     EVENT_ID_FIELD_NUMBER: _ClassVar[int]
     USER_WALLET_ADDR_FIELD_NUMBER: _ClassVar[int]
     CARD_PUBLIC_KEY_FIELD_NUMBER: _ClassVar[int]
     event_id: bytes
```

### Comparing `massmarket_hash_event-0.0.8/massmarket_hash_event/typedData.json` & `massmarket_hash_event-0.0.9/massmarket_hash_event/typedData.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9935897435897435%*

 * *Differences: {"'ChangeStock'": '{delete: [5]}'}*

```diff
@@ -47,18 +47,14 @@
         {
             "name": "cart_id",
             "type": "bytes32"
         },
         {
             "name": "tx_hash",
             "type": "bytes32"
-        },
-        {
-            "name": "block_no",
-            "type": "uint64"
         }
     ],
     "CreateCart": [
         {
             "name": "event_id",
             "type": "bytes32"
         }
```

### Comparing `massmarket_hash_event-0.0.8/massmarket_hash_event.egg-info/PKG-INFO` & `massmarket_hash_event-0.0.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: massmarket-hash-event
-Version: 0.0.8
+Name: massmarket_hash_event
+Version: 0.0.9
 Summary: Helper functions to hash events for signature creation and verification on Mass Market.
 Author-email: Henry Bubert <henry@mass.market>
 License: MIT
 Project-URL: Homepage, https://mass.market
 Project-URL: Repository, https://github.com/masslbs/network-schema.git
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `massmarket_hash_event-0.0.8/pyproject.toml` & `massmarket_hash_event-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "massmarket_hash_event"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
     {name = "Henry Bubert", email = "henry@mass.market"},
 ]
 description = "Helper functions to hash events for signature creation and verification on Mass Market."
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT"}
```

### Comparing `massmarket_hash_event-0.0.8/tests/test_encode.py` & `massmarket_hash_event-0.0.9/tests/test_encode.py`

 * *Files identical despite different names*

### Comparing `massmarket_hash_event-0.0.8/tests/test_signatures.py` & `massmarket_hash_event-0.0.9/tests/test_signatures.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,15 +114,15 @@
 
     (schema_pb2.Event(update_item=schema_pb2.UpdateItem(field=schema_pb2.UpdateItem.ITEM_FIELD_METADATA, item_id=test_event_id, metadata=b'{ "name": "test" }')),
       "0x88b1733cb885c6bf06bc6d3c12b5a7c08dc66b952759d84a10a1f4c1d7ae3130"),
 
     (schema_pb2.Event(change_stock=schema_pb2.ChangeStock(item_ids=[test_event_id], diffs=[1])),
       "0xe6c9896786eaa08950cb49cca8ed1ed5fb3c128979ea7bf0d0187e478fcd88d1"),
 
-    (schema_pb2.Event(change_stock=schema_pb2.ChangeStock(item_ids=[test_event_id], diffs=[1], cart_id=test_event_id, tx_hash=bytes(bytearray(32)), block_no=23)),
-      "0x9cebd0af7cf5a4255d352ae3afba93b0e4272efb25e685ff6279c0d9c102beb8"),
+    (schema_pb2.Event(change_stock=schema_pb2.ChangeStock(item_ids=[test_event_id], diffs=[1], cart_id=test_event_id, tx_hash=bytes(bytearray(32)))),
+      "0x5fb473c812fc700fb609043a5760565fbc14551645b3efd79bb6766b13bd9c22"),
   ]
   for idx, (evt, expected) in enumerate(events):
     data = h.hash_event(evt)
     signed_message = pk.sign_message(data)
     msg_hash = signed_message.messageHash.hex()
     assert msg_hash == expected, f"Failed on event {idx}"
```

