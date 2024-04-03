# Comparing `tmp/pelicandbms-0.5.5.tar.gz` & `tmp/pelicandbms-0.5.55.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pelicandbms-0.5.5.tar", last modified: Wed Mar 20 13:13:17 2024, max compression
+gzip compressed data, was "pelicandbms-0.5.55.tar", last modified: Wed Apr  3 08:49:02 2024, max compression
```

## Comparing `pelicandbms-0.5.5.tar` & `pelicandbms-0.5.55.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-03-20 13:13:17.638081 pelicandbms-0.5.5/
--rw-rw-rw-   0        0        0    35162 2022-12-05 10:38:56.000000 pelicandbms-0.5.5/LICENSE
--rw-rw-rw-   0        0        0      634 2024-03-20 13:13:17.637085 pelicandbms-0.5.5/PKG-INFO
--rw-rw-rw-   0        0        0      174 2022-12-05 10:28:28.000000 pelicandbms-0.5.5/README.MD
--rw-rw-rw-   0        0        0      571 2024-03-20 13:12:53.000000 pelicandbms-0.5.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-20 13:13:17.638081 pelicandbms-0.5.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-20 13:13:17.581720 pelicandbms-0.5.5/src/
--rw-rw-rw-   0        0        0       96 2024-03-20 11:28:38.000000 pelicandbms-0.5.5/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-20 13:13:17.584714 pelicandbms-0.5.5/src/example_package_dv1555/
--rw-rw-rw-   0        0        0     5913 2024-03-20 13:12:03.000000 pelicandbms-0.5.5/src/example_package_dv1555/samples_pelican.py
--rw-rw-rw-   0        0        0    87006 2024-03-20 13:11:51.000000 pelicandbms-0.5.5/src/pelicandb.py
-drwxrwxrwx   0        0        0        0 2024-03-20 13:13:17.635091 pelicandbms-0.5.5/src/pelicandbms.egg-info/
--rw-rw-rw-   0        0        0      634 2024-03-20 13:13:17.000000 pelicandbms-0.5.5/src/pelicandbms.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2024-03-20 13:13:17.000000 pelicandbms-0.5.5/src/pelicandbms.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-20 13:13:17.000000 pelicandbms-0.5.5/src/pelicandbms.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-03-20 13:13:17.000000 pelicandbms-0.5.5/src/pelicandbms.egg-info/requires.txt
--rw-rw-rw-   0        0        0       42 2024-03-20 13:13:17.000000 pelicandbms-0.5.5/src/pelicandbms.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-03 08:49:02.894445 pelicandbms-0.5.55/
+-rw-rw-rw-   0        0        0    35162 2022-12-05 10:38:56.000000 pelicandbms-0.5.55/LICENSE
+-rw-rw-rw-   0        0        0    13402 2024-04-03 08:49:02.893448 pelicandbms-0.5.55/PKG-INFO
+-rw-rw-rw-   0        0        0    12946 2024-04-03 08:25:46.000000 pelicandbms-0.5.55/README.rst
+-rw-rw-rw-   0        0        0      572 2024-04-03 08:27:03.000000 pelicandbms-0.5.55/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-03 08:49:02.894445 pelicandbms-0.5.55/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-03 08:49:02.869366 pelicandbms-0.5.55/src/
+-rw-rw-rw-   0        0        0       96 2024-03-20 11:28:38.000000 pelicandbms-0.5.55/src/__init__.py
+-rw-rw-rw-   0        0        0    87201 2024-04-03 07:22:20.000000 pelicandbms-0.5.55/src/pelicandb.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:49:02.892452 pelicandbms-0.5.55/src/pelicandbms.egg-info/
+-rw-rw-rw-   0        0        0    13402 2024-04-03 08:49:02.000000 pelicandbms-0.5.55/src/pelicandbms.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2024-04-03 08:49:02.000000 pelicandbms-0.5.55/src/pelicandbms.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 08:49:02.000000 pelicandbms-0.5.55/src/pelicandbms.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-03 08:49:02.000000 pelicandbms-0.5.55/src/pelicandbms.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       77 2024-04-03 08:49:02.000000 pelicandbms-0.5.55/src/pelicandbms.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     9649 2024-04-03 08:19:50.000000 pelicandbms-0.5.55/src/samples_pelican.py
+-rw-rw-rw-   0        0        0    12108 2024-04-03 06:19:01.000000 pelicandbms-0.5.55/src/samples_pelican_ru.py
```

### Comparing `pelicandbms-0.5.5/LICENSE` & `pelicandbms-0.5.55/LICENSE`

 * *Files identical despite different names*

### Comparing `pelicandbms-0.5.5/pyproject.toml` & `pelicandbms-0.5.55/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pelicandbms"
-version = "0.5.05"
+version = "0.5.55"
 authors = [
   { name="Dmitry Vorontsov", email="dv1555@hotmail.com" },
 ]
 description = "Ultrafast binary JSON-oriented NoSQL"
-readme = "README.MD"
+readme = "README.RST"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Operating System :: OS Independent",
 ]
```

### Comparing `pelicandbms-0.5.5/src/pelicandb.py` & `pelicandbms-0.5.55/src/pelicandb.py`

 * *Files 2% similar despite different names*

```diff
@@ -435,29 +435,23 @@
         Delete document/list of document/query results
 
         :condition: document ID/ list of documents IDs/ query condition
 
         """
         def delete(self,condition, **kwargs):
              
-             if isinstance(dataset, str):
-                try:
-                    dataset = json.loads(dataset)
-                except:
-                    raise ValueError(f'Dataset is not a JSON') 
-        
-             f = self._before_change_handler
-             if f!=None:
-                f("delete",dataset)   
-
              if isinstance(condition,str):
                 item = self.get(condition)  
 
                 if item == None:
-                    raise ValueError(f'Item not found {condition}')     
+                    raise ValueError(f'Item not found {condition}') 
+
+                f = self._before_change_handler
+                if f!=None:
+                    f("delete",[condition,item])    
                   
                             
                 if "session" in kwargs:
                     return self.fast_delete(item, session = kwargs.get("session"),NoIndex=kwargs.get("no_index"))                     
                 else:
                     return self.fast_delete(item,NoIndex=kwargs.get("no_index")) 
              
@@ -474,14 +468,18 @@
                   if isinstance(condition,dict): 
                        result = copy.deepcopy(self.find(condition))
                        for item in result:
                         
                         if item!=None:
                             set.append(item) 
 
+                  f = self._before_change_handler
+                  if f!=None:
+                    f("delete",[condition,set])  
+                  
                   if "session" in kwargs:
 
                     return self.delete_many(set, session = kwargs.get("session"))                     
                   
                   else:
                     
                     return self.delete_many(set)                                  
@@ -492,14 +490,15 @@
         def clear(self,  **kwargs) -> str:
             self._recording=True
             self._data = {}
             self._data_idx = {}
             self._maindata_temp = {}
 
             self._recording=False
+            self._modification_uuid=None
 
             if self._is_index():
                 if os.path.exists(self._path):
                     os.remove(self._path) 
             else:     
                 if os.path.exists(self._path):
                     os.remove(self._path)
@@ -699,15 +698,15 @@
                 for value_document in self.all():
                     if key in value_document:
                         id = hashlib.sha1(value_document.get(key).encode()).hexdigest()
                         self._db[name]._data[id] =value_document["_id"]
                     
                 
                 self._db[name]._write_index()
-                self._db[name]._recording=False    
+            self._db[name]._recording=False    
 
         """
         reindex function for text indexes
 
         :index_name: name of a index
 
         """       
@@ -773,15 +772,15 @@
 
                                               
 
         def _add_values_to_unique_indexes(self,documents):
             indexes = self._db._get_unique_indexes()
             for index,value in indexes.items():
                 if value['collection'] == self._name:
-                      
+                    d = self._db[index]._data  
                     self._db[index]._recording=True
                     for document in documents:
                         if value['key'] in document:
                             if not(isinstance(document.get(value['key']),dict) or isinstance(document.get(value['key']),list)):
                                 self._db[index]._data[hashlib.sha1(document.get(value['key']).encode()).hexdigest()]=document['_id']
                       
                     if not value.get("dynamic") == True:
@@ -790,15 +789,15 @@
 
         def _delete_values_from_unique_indexes(self,documents):                        
             indexes = self._db._get_unique_indexes()
             
             for index,value in indexes.items():
                 
                 if value['collection'] == self._name:
-                      
+                    d = self._db[index]._data  
                     self._db[index]._recording=True
                     for document in documents:
                         if value['key'] in document:
                             if '_id' in document:
                                 key = next((k for k in self._db[index]._data if self._db[index]._data[k] == document['_id']), None)
                                 if key!= None:
                                         self._db[index]._data.pop(key,None)
@@ -906,16 +905,16 @@
                       self._db[index]._recording=True
                       for document in documents:
                         if value['key'] in document:
                             if isinstance(document.get(value['key']),str):
                                 new_index = {"_id":hashlib.sha1(document.get(value['key']).encode()).hexdigest()}
                                 self._db[index]._data.pop(new_index["_id"],None)
                                 
-                           
-                      self._db[index]._write_index()
+                      if not value.get("dynamic") == True:       
+                        self._db[index]._write_index()
                       self._db[index]._recording=False          
                                     
         
         """B-tree indexes"""
 
 
         """
@@ -990,19 +989,22 @@
 
         """
         initialize data at first call
         """
         def __getattr__(self, item):
             if item=='_data':
                 if self._is_modification() or not hasattr(object, '_data') :
-                    self._data = self._read_collection()
+                    
                     if not self._is_index():
+                        self._data = self._read_collection()
                         self._data_idx=self._read_collection_idx()
                         if self._db._RAM == True:
                            self._maindata = self._read_collection_maindata()     
+                    else:       
+                        self._data = self._read_index()
                 
                 
                     return object.__getattribute__(self, '_data')
                 
                        
             
             if item=='_data_idx':
@@ -1058,27 +1060,34 @@
         def _is_modification(self):
             if  self._recording==True:
                  return False
             
             if  self._modification_uuid==None:
                  return True
             
+
+
+            if not os.path.isfile(self._path):
+                return False
+
+
             if self._db.singleton == True:
                  return False
-              
+            
+
             uid=None
             with open(self._path,"r", encoding='utf-8') as f:
                 text =f.read(36)
                 uid = text[:36]
 
             return uid!=self._modification_uuid
 
         def _read_collection(self):
             
-            print("read_started")
+            #print("read_started")
             
             collection = {}
                 
             if os.path.isfile(self._path):
                     path = Path(self._path)    
                     path.parent.mkdir(parents=True, exist_ok=True) 
 
@@ -1108,15 +1117,15 @@
                         raise ValueError(f'Lock collection timeout error: {self._path}')
 
             return collection
         
         
         def _read_collection_txt(self):
 
-            print("read_txt_started")
+            #print("read_txt_started")
             
             collection = {}
                 
             if os.path.isfile(self._path):
                     path = Path(self._path)    
                     path.parent.mkdir(parents=True, exist_ok=True) 
 
@@ -1133,15 +1142,15 @@
                     except Timeout:
                         raise ValueError(f'Lock collection timeout error') 
 
             return collection
         
         def _read_collection_idx(self):
 
-            print("read_idx_started")
+            #print("read_idx_started")
             
             collection = {}
                 
             if os.path.isfile(self._path_id):
                     path = Path(self._path_id)    
                     path.parent.mkdir(parents=True, exist_ok=True) 
 
@@ -1182,42 +1191,46 @@
             lock = SoftFileLock(self._path+".lock")
             try:
                     with  lock.acquire(timeout=self._db['_timeout']):
                         with open(self._path,"w", encoding='utf-8') as f: 
                             f.write(prefix)
                             f.write("\n")
                             self._modification_uuid=prefix
-                            
-                            f.write(json.dumps(self._data)) 
+                            str_data = json.dumps(self._data)
+                            #str_data[1:-1]
+                            f.write(str_data) 
 
             except Timeout:
                 raise ValueError(f'Lock collection timeout error: {self._path}')
 
         def _read_index(self):
             path = Path(self._path)    
             
             path.parent.mkdir(parents=True, exist_ok=True) 
             collection ={}
-           
-            lock = SoftFileLock(str(path.absolute())+".lock")
-            try:
-                    with  lock.acquire(timeout=self._db['_timeout']):
-                        
-                        if os.path.isfile(str(path.absolute())):
-                            with open(str(path.absolute()),"r", encoding='utf-8') as f:
-                                content = f.readlines()
-                                txt = content[1:]
-                                collection = json.loads(txt[0])   
-                                uid = content[0].rstrip()
-                                self._modification_uuid =uid
-                                
-                            return collection    
-            except Timeout:
-                   raise ValueError(f'Lock collection timeout error: {self._path}') 
-        
+            
+            if os.path.isfile(str(path.absolute())):
+                lock = SoftFileLock(str(path.absolute())+".lock")
+                try:
+                        with  lock.acquire(timeout=self._db['_timeout']):
+                            
+                            if os.path.isfile(str(path.absolute())):
+                                with open(str(path.absolute()),"r", encoding='utf-8') as f:
+                                    content = f.readlines()
+                                    txt = content[1:]
+                                    collection = json.loads(txt[0])   
+                                    uid = content[0].rstrip()
+                                    self._modification_uuid =uid
+                                    
+                                return collection    
+                except Timeout:
+                    raise ValueError(f'Lock collection timeout error: {self._path}') 
+            else:
+                return collection
+            
         """
         Handlers
         """
         def register_before_change_handler(self,handler):
             self._before_change_handler = handler
 
         """
@@ -1386,16 +1399,15 @@
                                 self._add_values_to_unique_indexes([document])
                                 self._add_values_to_text_indexes([document])
                                 #self._db._add_value_to_subscriptions(self._name,doc_id)
 
             return doc_id     
 
         """
-        Remove documents as text block from file 
-        and value from collection dictionary
+        Remove documents from idx-file 
 
         :document: document or list of documents to be added
         
         Arguments:
         :NoIndex: OFF to change indexes
         :session: transaction instance
 
@@ -1469,18 +1481,20 @@
                 ids =  []
 
                
                 for document in documents:
                     if "_id" in document:
                         doc_id = document['_id']
 
+                    
                     if self.get(doc_id)==None:
                         raise ValueError(f'Value with ID {str(doc_id)} not in collection')
                     
-                    
+                    ids.append(doc_id)
+
                     self._data_idx.pop(doc_id,None)
 
                     
                 return ids,None,None,None,None
                 
                 #self._data = collection
  
@@ -1515,67 +1529,67 @@
                     
                     if self._db.queue!=None:
                         self._db.queue.put([documents,self._name,self._db._name,"delete"]) 
                     else:     
                         self._delete_values_from_unique_indexes(documents)
                         self._delete_values_from_text_indexes(documents)
 
-                return doc_id   
+                return res   
                 
             return None    
 
         def insert_many(self,documents, **kwargs):
-            start_time = time.time()
+            #start_time = time.time()
             collection = self._data
-            print("insert_many - read collection: --- %s seconds ---" % (time.time() - start_time))
+            #print("insert_many - read collection: --- %s seconds ---" % (time.time() - start_time))
 
             self._recording = True
 
             begin = 0
 
             if 'session' in kwargs: #updating with transaction
                 session = kwargs['session']
                 if self._name in session._operations_add:
                         for line in session._operations_add[self._name]:
                             begin = line[3] 
                             #_doc_id = line[0]
                             #last_version = self._data_idx[_doc_id]
                             #begin = self._data[_doc_id+"_"+str(last_version)][1]
 
-            start_time = time.time()
+            #start_time = time.time()
             
             if os.path.exists(self._path_data) and begin==0:
                 in_file = open(self._path_data, "rb") 
                 data = in_file.read() 
                 begin = len(data)
                 in_file.close()
             
-            print("getting begin: --- %s seconds ---" % (time.time() - start_time))
+            #print("getting begin: --- %s seconds ---" % (time.time() - start_time))
              
 
             def updater():
 
                 ids = []
                 versions = []
 
                 dbytes = b''
 
                 _begin = begin  
 
                 datastr= ""
 
-                t1 = 0
-                t2 = 0
-                t3 = 0
-                t4 = 0
-                t5 = 0
+                #t1 = 0
+                #t2 = 0
+                #t3 = 0
+                #t4 = 0
+                #t5 = 0
                     
                 liststr=[]    
                 for document in documents:    
-                    start_time = time.time()
+                    #start_time = time.time()
                     if "_id" in document:
                         doc_id = document['_id']
                     else:
                         doc_id = self._get_next_id()     
                         document["_id"]  = doc_id
 
                     last_version = self._data_idx.get(doc_id)
@@ -1588,61 +1602,61 @@
                             
 
                     else:
                         _version=0     
                     
                     document["_version"]  = _version 
 
-                    t1+=(time.time() - start_time)
+                    #t1+=(time.time() - start_time)
                     
 
-                    start_time = time.time()
+                    #start_time = time.time()
                     
                     bytes = pickle.dumps(document,pickle.HIGHEST_PROTOCOL)
 
-                    t2+=(time.time() - start_time)
+                    #t2+=(time.time() - start_time)
 
-                    start_time = time.time()
+                    #start_time = time.time()
                     
                     dbytes+= bytes
 
-                    t3+=(time.time() - start_time)
-                    start_time = time.time()
+                    #t3+=(time.time() - start_time)
+                    #start_time = time.time()
                     full_id = doc_id+"_"+str(_version)
                     value = [_begin,_begin+len(bytes),_version,doc_id]
                     
                     self._data[full_id]  = value
                     #if datastr=="":
                     #    datastr = format_datastr(doc_id+"_"+str(_version),value)
                     #else:     
                     #    datastr +="\n"+ format_datastr(doc_id+"_"+str(_version),value)
                     liststr.append(format_datastr(doc_id+"_"+str(_version),value))    
 
-                    t4+=(time.time() - start_time)
-                    start_time = time.time()
+                    #t4+=(time.time() - start_time)
+                    #start_time = time.time()
                     _begin+=len(bytes)
                     
                     self._data_idx[doc_id] = _version 
 
                     if self._db._RAM == True:
                         self._maindata[doc_id] = document   
 
                     ids.append(doc_id)
                     versions.append(_version)
-                    t5+=(time.time() - start_time)
+                    #t5+=(time.time() - start_time)
 
                     if 'session' in kwargs:
                          self._maindata_temp[doc_id] = document
 
                 datastr = "\n".join(liststr)
-                print("updater 1: --- %s seconds ---" % (t1))
-                print("updater 2: --- %s seconds ---" % (t2))
-                print("updater 3: --- %s seconds ---" % (t3))
-                print("updater 3: --- %s seconds ---" % (t4))
-                print("updater 3: --- %s seconds ---" % (t5))
+                #print("updater 1: --- %s seconds ---" % (t1))
+                #print("updater 2: --- %s seconds ---" % (t2))
+                #print("updater 3: --- %s seconds ---" % (t3))
+                #print("updater 3: --- %s seconds ---" % (t4))
+                #print("updater 3: --- %s seconds ---" % (t5))
                     
                 return ids,dbytes,versions,_begin,datastr
                     
 
             if 'session' in kwargs: #updating with transaction
                     if not kwargs.get("NoIndex") == True and (kwargs.get("upsert")==True or kwargs.get("update")==True):  
                         
@@ -1711,80 +1725,78 @@
 
             collection = self._data
             
             path = Path(self._path)    
             path.parent.mkdir(parents=True, exist_ok=True) 
 
             prefix = str(uuid.uuid4())
-            start_time = time.time()
             
+            #starting updater code
             doc_id,dbytes,_version,end,datastr = updater() 
-            print("Updater: --- %s seconds ---" % (time.time() - start_time))  
+            
 
             gc.enable()    
 
             if kwargs.get("shrink") == True:
                 os.remove(self._path)
                 os.remove(self._path_data)
                 self._modification_uuid=None
               
             lock = SoftFileLock(self._path+".lock")
 
-            start_time1 = time.time()
+            
             try:
                 with  lock.acquire(timeout=self._db['_timeout']):
                         
                     try:    
                         
-                        start_time = time.time()
+                        #Writing a pointer file (*.ptr) with a modification prefix
                         prefix_updated=False
                         with open(self._path,"a", encoding='utf-8') as f: 
                                     
                             if self._modification_uuid==None:
                                 f.write(prefix)
                                 f.write("\n")
                                 self._modification_uuid=prefix
                                 prefix_updated=True
                                 
 
                             f.write(datastr)
                             f.write("\n") 
                         
 
-                        
+                        #update prefix if needed
                         if not prefix_updated:
                             with open(self._path,"r+", encoding='utf-8') as f:
                                 text =f.read(36)
                                 f.seek(0)
                                 f.write(prefix)
                                 self._modification_uuid=prefix                                    
 
-                        print("Write _data: --- %s seconds ---" % (time.time() - start_time))      
                         
-
-                        start_time = time.time()
+                        #write last version dictionary                                
                         with open(self._path_id, 'wb') as f:
                             pickle.dump(self._data_idx, f, pickle.HIGHEST_PROTOCOL)            
-                        print("Write _data_idx: --- %s seconds ---" % (time.time() - start_time))  
                         
-                        start_time = time.time()    
+                        
+                        #write binary data-file
                         out_file = open(self._path_data, "ab")
                         out_file.write(dbytes)
                         out_file.close()   
-                        print("Write _maindata: --- %s seconds ---" % (time.time() - start_time))      
+                        
 
                     except Exception:
                         raise ValueError(f'Write collections error') 
                         
 
                         
             except Timeout:
                     raise ValueError(f'Lock collection timeout error: {self._path}')     
 
-            print("Write total: --- %s seconds ---" % (time.time() - start_time1))   
+            
             return  doc_id               
             
             
         def _update_collection_without_bytes(self,updater: Callable[[Dict[int, Mapping]], None]):
             
             collection = self._data
             
@@ -1973,15 +1985,15 @@
         
         if not os.path.exists(basepath):
             os.makedirs(basepath)
         
         for file in os.listdir(basepath):
                 if file.endswith(".lock"):
                     duration = time.time()-os.path.getmtime(basepath +os.sep+file)
-                    if duration>LOCK_TIMEOUT*5:
+                    if duration>LOCK_TIMEOUT*2:
                          os.remove(basepath +os.sep+file)
         
 
         #self._collections: Dict[str, Collection] = {}
         self.__dict__: Dict[str, self.Collection] = {}
         self.__dict__['_basepath']=basepath
         
@@ -2207,15 +2219,15 @@
             raise ValueError(f'Message  string is not a JSON') 
     if not isinstance(jmessage,list):
         raise ValueError(f'Root element in message should be a list')          
     for db_set in jmessage:
         for db_name,db_value in db_set.items():
             
             if not db_name in dbs:
-                raise ValueError(f'Databese {db_name} is not initialized')          
+                raise ValueError(f'Database {db_name} is not initialized')          
 
             db = dbs[db_name]
             if isinstance(db_value, list):
                 session_results = {}
                 with DBSession(db) as s:
                     for transaction_item in db_value:
```

