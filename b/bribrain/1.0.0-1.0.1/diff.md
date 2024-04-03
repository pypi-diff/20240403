# Comparing `tmp/bribrain-1.0.0.tar.gz` & `tmp/bribrain-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bribrain-1.0.0.tar", last modified: Thu Mar 21 14:27:32 2024, max compression
+gzip compressed data, was "dist/bribrain-1.0.1.tar", last modified: Wed Apr  3 03:09:39 2024, max compression
```

## Comparing `bribrain-1.0.0.tar` & `bribrain-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 cdsw      (8536) cdsw      (8536)        0 2024-03-21 14:27:32.000000 bribrain-1.0.0/
-drwxr-xr-x   0 cdsw      (8536) cdsw      (8536)        0 2024-03-21 14:27:32.000000 bribrain-1.0.0/bribrain/
--rwx------   0 cdsw      (8536) cdsw      (8536)       90 2024-03-20 04:25:35.000000 bribrain-1.0.0/bribrain/__init__.py
--rwx------   0 cdsw      (8536) cdsw      (8536)     2456 2024-03-14 14:03:41.000000 bribrain-1.0.0/bribrain/config.py
--rwx------   0 cdsw      (8536) cdsw      (8536)     6702 2024-03-19 03:25:45.000000 bribrain-1.0.0/bribrain/function.py
--rwx------   0 cdsw      (8536) cdsw      (8536)    79822 2024-03-21 10:44:04.000000 bribrain-1.0.0/bribrain/ingestion.py
--rwx------   0 cdsw      (8536) cdsw      (8536)    16610 2024-03-21 03:28:26.000000 bribrain-1.0.0/bribrain/load.py
-drwxr-xr-x   0 cdsw      (8536) cdsw      (8536)        0 2024-03-21 14:27:32.000000 bribrain-1.0.0/bribrain.egg-info/
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)      446 2024-03-21 14:27:32.000000 bribrain-1.0.0/bribrain.egg-info/PKG-INFO
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)      267 2024-03-21 14:27:32.000000 bribrain-1.0.0/bribrain.egg-info/SOURCES.txt
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)        1 2024-03-21 14:27:32.000000 bribrain-1.0.0/bribrain.egg-info/dependency_links.txt
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)       41 2024-03-21 14:27:32.000000 bribrain-1.0.0/bribrain.egg-info/requires.txt
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)        9 2024-03-21 14:27:32.000000 bribrain-1.0.0/bribrain.egg-info/top_level.txt
--rwx------   0 cdsw      (8536) cdsw      (8536)      631 2024-03-21 14:26:25.000000 bribrain-1.0.0/setup.py
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)      446 2024-03-21 14:27:32.000000 bribrain-1.0.0/PKG-INFO
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)       38 2024-03-21 14:27:32.000000 bribrain-1.0.0/setup.cfg
+drwxr-xr-x   0 cdsw      (8536) cdsw      (8536)        0 2024-04-03 03:09:39.000000 bribrain-1.0.1/
+drwxr-xr-x   0 cdsw      (8536) cdsw      (8536)        0 2024-04-03 03:09:39.000000 bribrain-1.0.1/bribrain/
+-rwx------   0 cdsw      (8536) cdsw      (8536)       90 2024-03-20 04:25:35.000000 bribrain-1.0.1/bribrain/__init__.py
+-rwx------   0 cdsw      (8536) cdsw      (8536)     2456 2024-03-14 14:03:41.000000 bribrain-1.0.1/bribrain/config.py
+-rwx------   0 cdsw      (8536) cdsw      (8536)     4330 2024-04-03 02:49:31.000000 bribrain-1.0.1/bribrain/function.py
+-rwx------   0 cdsw      (8536) cdsw      (8536)    80247 2024-04-03 03:09:21.000000 bribrain-1.0.1/bribrain/ingestion.py
+-rwx------   0 cdsw      (8536) cdsw      (8536)    16791 2024-04-03 02:49:50.000000 bribrain-1.0.1/bribrain/load.py
+drwxr-xr-x   0 cdsw      (8536) cdsw      (8536)        0 2024-04-03 03:09:39.000000 bribrain-1.0.1/bribrain.egg-info/
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)      460 2024-04-03 03:09:38.000000 bribrain-1.0.1/bribrain.egg-info/PKG-INFO
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)      267 2024-04-03 03:09:38.000000 bribrain-1.0.1/bribrain.egg-info/SOURCES.txt
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)        1 2024-04-03 03:09:38.000000 bribrain-1.0.1/bribrain.egg-info/dependency_links.txt
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)       40 2024-04-03 03:09:38.000000 bribrain-1.0.1/bribrain.egg-info/requires.txt
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)        9 2024-04-03 03:09:38.000000 bribrain-1.0.1/bribrain.egg-info/top_level.txt
+-rwx------   0 cdsw      (8536) cdsw      (8536)      647 2024-04-03 02:15:59.000000 bribrain-1.0.1/setup.py
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)      460 2024-04-03 03:09:39.000000 bribrain-1.0.1/PKG-INFO
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)       38 2024-04-03 03:09:39.000000 bribrain-1.0.1/setup.cfg
```

### Comparing `bribrain-1.0.0/bribrain/config.py` & `bribrain-1.0.1/bribrain/config.py`

 * *Files identical despite different names*

### Comparing `bribrain-1.0.0/bribrain/ingestion.py` & `bribrain-1.0.1/bribrain/ingestion.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #=============================================================#
 ###  CREATED AT     : 18 MARET 2024                         ###
-###  UPDATED AT     : 18 MARET 2024                         ###
+###  UPDATED AT     : 03 APRIL 2024                         ###
 ###  COPYRIGHT      : ANDRI ARIYANTO                        ###
 ###  DESCRIPTION    : Module untuk melakukan ingest data    ###
 #=============================================================#
 
 import os # memungkinkan pengguna untuk berinteraksi dengan sistem operasi yang dijalankan sekarang
 import re # membantu mencocokkan atau menemukan string atau set string lainnya, menggunakan sintaksis khusus yang dimiliki suatu pola.
 import json # untuk mengubah kamus python menjadi string JSON yang dapat ditulis menjadi file
@@ -232,25 +232,30 @@
   Return:
       int: ikuran folder besaran bytes dalam tipe integer
   """
   hive_schema = params["hive_schema"] # menyimpan nama hive schema
   hive_table = params["hive_table"] # menyimpan nama hive table
   last_partition = params["last_partition"] # menyimpan value partisi terakhir dari tabel target (None jika bukan tabel berpartisi)
   
+  if hive_schema.startswith("dev"):
+    hdfs_path = "/dev/"
+  else:
+    hdfs_path = "/user/hive/warehouse/"
+
   # penanganan error ketika direktori tujuan tidak tersedia
   try:
     path = lambda p: spark._jvm.org.apache.hadoop.fs.Path(p) # membuat variabel path untuk menunjukan lokasi direktori pada hive
     fs = spark._jvm.org.apache.hadoop.fs.FileSystem.get(spark._jsc.hadoopConfiguration()) # membuat variabel untuk dapak mengakses File System pada hive
     
     # melakukan kondisional untuk mendapatkan ukuran keseluruhan atau hanya partisi terakhit dari tabel target
     if last and last_partition != None: # kondisi ketika terdapat value pada partisi terakhir dan parameter last True
-      hdfs = fs.getContentSummary(path("/user/hive/warehouse/{}.db/{}/{}".format(hive_schema, hive_table, last_partition))) # mendapatkan informasi ukuran hdfs folder partisi terakhir
+      hdfs = fs.getContentSummary(path(hdfs_path+"{}.db/{}/{}".format(hive_schema, hive_table, last_partition))) # mendapatkan informasi ukuran hdfs folder partisi terakhir
       return hdfs.getLength() # return ukuran hdfs folder dalam besaran bytes
     else: # kondisi ketika tidak terdapat value pada partisi terakhir atau parameter last False
-      hdfs = fs.getContentSummary(path("/user/hive/warehouse/{}.db/{}".format(hive_schema, hive_table))) # mendapatkan informasi ukuran hdfs folder keseluruhan data
+      hdfs = fs.getContentSummary(path(hdfs_path+"{}.db/{}".format(hive_schema, hive_table))) # mendapatkan informasi ukuran hdfs folder keseluruhan data
       return hdfs.getLength() # return ukuran hdfs folder dalam besaran bytes
   except:
     return 0 # return 0 jika direktori tujuan tidak tersedia
 # 9 ===================================================================================================================================================================================================
 def get_format_date(format_date):
   """Mengubah format tanggal input menjadi format tanggal sintaks python
   
@@ -514,27 +519,33 @@
       params : parameter-parameter pendukung yang disimpan dalam bentuk dictionaries
 
   Return : Hasil partisi number
 
   """
   hive_table = params["hive_table"] # menyimpan nama hive tabel
   params["hive_blocksize"] = int(params["repartition_size"])*1024*1024 # update hive_blocksize dengan integer partisi size
-  params["sample_schema"] = "temp" # update sample schema dengan temporary
+  params["sample_schema"] = params["hive_schema"] # update sample schema dengan temporary
   params["sample_table"] = "sample_" + hive_table # update sampel tabel dengan hive tabel
+  
+  if hive_schema.startswith("dev"):
+    hdfs_path = "/dev/"
+  else:
+    hdfs_path = "/user/hive/warehouse/"
+    
   # membuat sampel tabel
   df\
     .sample(False,0.1,None)\
     .write\
     .format("parquet")\
     .mode("overwrite")\
     .saveAsTable("{}.{}".format(params["sample_schema"], params["sample_table"]))
   # mengambil partisi number pada hive temporary
   path = lambda p: spark._jvm.org.apache.hadoop.fs.Path(p)
   fs = spark._jvm.org.apache.hadoop.fs.FileSystem.get(spark._jsc.hadoopConfiguration())
-  hdfs_folder = fs.getContentSummary(path("/user/hive/warehouse/{}.db/{}/".format(params["sample_schema"], params["sample_table"])))
+  hdfs_folder = fs.getContentSummary(path(hdfs_path+"{}.db/{}/".format(params["sample_schema"], params["sample_table"])))
   # menimpa num_file_partitions ke partisi number aktual
   repartition_number = float(hdfs_folder.getLength()*10)/float(params["hive_blocksize"]) # menambahkan jumlah partisi dengan format float
   params["repartition_number"] = int(1 if repartition_number < 1 else repartition_number)
   # menghapus sampel tabel
   spark.sql("DROP TABLE {}.{}".format(params["sample_schema"], params["sample_table"]))
   return params
 # 17 ==================================================================================================================================================================================================
@@ -730,18 +741,25 @@
 
   """
   hive_mode = params["strategy"].lower() # menyimpan nama strategy pada hive_mode
   hive_schema = params["hive_schema"] # menyimpan nama hive_schema pada hive_schema
   hive_table = params["hive_table"] # menyimpan nama hive_table pada hive_table
   repartition_column = params["repartition_column"] # menyimpan nama repartition_colum pada repartition_column
   repartition_number = params["repartition_number"] # menyimpan nama repartition_number pada repartition_number
+
+  if hive_schema.startswith("dev"):
+    hdfs_path = "/dev/"
+  else:
+    hdfs_path = "/user/hive/warehouse/"
+    
   if repartition_column != None and repartition_column.strip() != "": # cek repartition_column apabila kosong
     df = df.repartition(repartition_number, repartition_column) # update kolom dengan angka dan kolom
   else: # selain itu
     df = df.repartition(repartition_number) # update kolom dengan nomor partisi
+
   # load to hive
   if hive_mode.upper() == "APPEND": # cek hive mode dengan kondisi APPEND
     partition =  set_datetime().date().strftime("%Y%m%d") # menyimpan format waktu dan tanggal pada partition
     params["hive_partition_col"] = "ds" # update hive_partition_col dengan dttm_ingest
     params["hive_partition_date"] = str(partition) # update hive_partition_date dengan format string
     df = df.withColumn("ds", F.lit(partition)) # update kolom dengan dttm_ingest
     hive_table_exist = spark.sql("SHOW TABLES IN {} LIKE '{}'".format(hive_schema, hive_table)).count()
@@ -753,15 +771,15 @@
   else: # selain itu
     drop_hive_table(spark, params) # menghapus tabel di spark
     df = df.withColumn("hdfs_dttm_ingest", F.lit(set_datetime())) # membuat kolom tabel berisi dttm_ingest dengan status waktu data ketika di ingest
     df.write.format("parquet").mode(hive_mode).saveAsTable("{}.transit_{}".format(hive_schema, hive_table)) # membuat tabel dengan partisi berdasarkan dttm ingest pada /user/hive/warehouse/{}.db/{}/ dengan format hive_schema, hive_table
     spark.sql("REFRESH TABLE {}.transit_{}".format(hive_schema, hive_table)) # refresh tabel di spark
     spark.sql("DROP TABLE IF EXISTS {}.{}".format(hive_schema, hive_table)) # menghapus tabel jika ada sebelumnya
     spark.sql("ALTER TABLE {0}.transit_{1} RENAME TO {0}.{1}".format(hive_schema, hive_table)) # menyimpan tabel baru
-    spark.sql("ALTER TABLE {0}.{1} SET SERDEPROPERTIES('path'='hdfs://bribigdata/user/hive/warehouse/{0}.db/{1}')".format(hive_schema, hive_table)) # menyimpan tabel di hive database
+    spark.sql("ALTER TABLE {0}.{1} SET SERDEPROPERTIES('path'='hdfs://bribigdata{2}{0}.db/{1}')".format(hive_schema, hive_table, hdfs_path)) # menyimpan tabel di hive database
   # refresh metadata after modifying sql statement before
   query=""" 
     hive -e 'ALTER TABLE {}.{} SET TBLPROPERTIES("EXTERNAL"="FALSE");' 
   """.format(hive_schema, hive_table) # membuat query untuk dikirimkan ke terminal
   popen = subprocess.Popen(query,shell=True,stderr=subprocess.PIPE) # mengirimkan ke terminal
   stdout,stderr = popen.communicate() # mengirimkan kembali ke hive 
   if popen.returncode != 0: # cek apabila data yang kembali dari terminal berisi kosong
@@ -785,28 +803,35 @@
   hive_schema = params["hive_schema"] # menyimpan nama hive_schema pada hive_schema
   hive_table = params["hive_table"] # menyimpan nama hive_table pada hive_table
   hive_partition_col = params["hive_partition_col"].split("|") # menyimpan partisi kolom di hive_partition_col
   hive_partition_source = params["hive_partition_source"] # menyimpan sumber partisi di hive_partition_source
   hive_partition_date = params["hive_partition_date"].split("|") # menyimpan tanggal partisi di hive_partition_date
   repartition_column = params["repartition_column"] # menyimpan kolom partisi di repartition_column
   repartition_number = params["repartition_number"] # menyimpan kolom nomor di repartition_number
+
+  if hive_schema.startswith("dev"):
+    hdfs_path = "/dev/"
+  else:
+    hdfs_path = "/user/hive/warehouse/"
+
   if repartition_column != None and repartition_column.strip() != "": # cek repartition_column apabila kosong
     df = df.repartition(repartition_number, repartition_column) # update kolom dengan angka dan kolom
   else: # selain itu
     df = df.repartition(repartition_number) # update kolom dengan nomor partisi
+
   # load to hive
   if hive_mode.upper() == "OVERWRITE": # cek hive apabila kondisi overwrite
     # start
     drop_hive_table(spark, params) # menghapus tabel di spark
     df.write.partitionBy(hive_partition_col).format("parquet").mode(hive_mode).saveAsTable("{}.transit_{}".format(hive_schema, hive_table)) # membuat transit tabel dengan partisi berdasarkan hive_partition_col untuk hive_schema, hive_table
     spark.sql("MSCK REPAIR TABLE {}.transit_{}".format(hive_schema, hive_table)) # memperbaiki tabel berpartisi
     spark.sql("REFRESH TABLE {}.transit_{}".format(hive_schema, hive_table)) # refresh transit tabel di spark
     spark.sql("DROP TABLE IF EXISTS {}.{}".format(hive_schema, hive_table)) # menghapus tabel jika ada sebelumnya
     spark.sql("ALTER TABLE {0}.transit_{1} RENAME TO {0}.{1}".format(hive_schema, hive_table)) # mengubah nama transit tabel
-    spark.sql("ALTER TABLE {0}.{1} SET SERDEPROPERTIES('path'='hdfs://bribigdata/user/hive/warehouse/{0}.db/{1}')".format(hive_schema, hive_table)) # menyimpan tabel di hive database
+    spark.sql("ALTER TABLE {0}.{1} SET SERDEPROPERTIES('path'='hdfs://bribigdata{2}{0}.db/{1}')".format(hive_schema, hive_table, hdfs_path)) # menyimpan tabel di hive database
   else: # selain itu
     # masih belum menemukan kasus hive_partition_source tidak kosong
     hive_table_exist = spark.sql("SHOW TABLES IN {} LIKE '{}'".format(hive_schema, hive_table)).count()
     if hive_table_exist == 1:
       if hive_partition_source != None: # cek apabila partisi source tidak kosong 
         hive_partition_source = hive_partition_source.spilt("|") # menyimpan sumber partisi di hive_partition_source
         df.write.partitionBy(hive_partition_col).parquet("/user/cdh-etl1/parquet/", mode = 'overwrite') # membuat ulang tabel partisi hive
@@ -881,15 +906,15 @@
    # membuat dataframe pada temporary tabel informasi metadata menggunakan format yang sudah tersedia
   spark.createDataFrame(tuple(data), schema)\
     .coalesce(1)\
     .write\
     .partitionBy("ds")\
     .mode("append")\
     .format("parquet")\
-    .saveAsTable("temp.log_activity_raw_ingestion_table") # simpan sebagai tabel log activity
+    .saveAsTable("dev_ddb.log_activity_raw_ingestion_table") # simpan sebagai tabel log activity
 # 26 ==================================================================================================================================================================================================
 def ingest_metadata_info(spark, params): 
   """ Mencatat setiap info metadata yang sudah di ingest
 	
 	Parameter :
 		Spark 	: objek SparkSession
 		params	: parameter-parameter pendukung yang disimpan dalam bentuk dictionaries
@@ -925,15 +950,15 @@
   )]
   spark.createDataFrame(tuple(data), schema)\
     .coalesce(1)\
     .write\
     .partitionBy("ds")\
     .mode("append")\
     .format("parquet")\
-    .saveAsTable("temp.metadata_raw_describe_table") # membuat dataframe pada temporary tabel informasi metadata menggunakan format yang sudah tersedia
+    .saveAsTable("dev_ddb.metadata_raw_describe_table") # membuat dataframe pada temporary tabel informasi metadata menggunakan format yang sudah tersedia
 # 27 ==================================================================================================================================================================================================
 # edit disini untuk menambankan database baru (sudah ditambah postgress dan db2)
 def is_source_database_exist(spark, params):
   """ Cek database tersedia
  
  Parameter :
   Spark  : objek SparkSession
```

### Comparing `bribrain-1.0.0/bribrain/load.py` & `bribrain-1.0.1/bribrain/load.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #=============================================================#
 ###  CREATED AT     : 04 MARET 2024                         ###
-###  UPDATED AT     : 07 MARET 2024                         ###
+###  UPDATED AT     : 03 APRIL 2024                         ###
 ###  COPYRIGHT      : ANDRI ARIYANTO                        ###
 ###  DESCRIPTION    : Module untuk melakukan load data      ###
 #=============================================================#
 
 ## HDFS ==============================================================================================
 
 def load_to_hive(spark, df, schema, table, partition=None, mode="append", repartition_number=None, blocksize=256):
@@ -24,15 +24,30 @@
           (default is None)      
       blocksize (int): ukuran per file dalam satuan megabyte
           (default is 256)
     
   Returns:
       -
   """
+  
+  spark = bribrain.sparkSession()
+  df = spark.read.table("dev_ddb.bribrain_userpool_raw")
+  schema = "dev_ddb"
+  table = "bribrain_userpool_raw"
     
+  schema = "datamart"
+  table = "bribrain_bank_swift_code"
+  
+  if schema.startswith("dev"):
+    hdfs_path = "/dev/"
+  else:
+    hdfs_path = "/user/hive/warehouse/"
+    
+  hdfs_path
+  
   print("Write table to Hive: {}.{}".format(schema, table))
     
   # pengecekan partitioned table
   if partition:
     
     # kondisi ketika tabel berpartisi
     partition = partition.split(",")
@@ -49,34 +64,34 @@
       condition = ' AND '.join(["{}='{}'".format(col, row[col]) for col in partition])
       df_write = df.filter(condition)
       
 
       if not repartition_number:
         tag = '_'.join([row[col].strip() for col in partition]).lower()
 
-        spark.sql("DROP TABLE IF EXISTS dev_ddb.sample_{}_{}".format(table, tag))
+        spark.sql("DROP TABLE IF EXISTS {}.sample_{}_{}".format(schema, table, tag))
 
         # penulisan sample data untuk estimasi ukuran data
         df_write\
           .sample(False,0.1,None)\
           .write\
           .format("parquet")\
           .mode("overwrite")\
-          .saveAsTable("dev_ddb.sample_{}_{}".format(table, tag))
+          .saveAsTable("{}.sample_{}_{}".format(schema, table, tag))
 
         # mendapatkan metadata content summary dari sample table
         path = lambda p: spark._jvm.org.apache.hadoop.fs.Path(p)
         fs = spark._jvm.org.apache.hadoop.fs.FileSystem.get(spark._jsc.hadoopConfiguration())
-        hdfs_folder = fs.getContentSummary(path("/dev/dev_ddb.db/sample_{}_{}/".format(table, tag)))
+        hdfs_folder = fs.getContentSummary(path(hdfs_path+"{}.db/sample_{}_{}/".format(schema, table, tag)))
 
         # kalkulasi jumlah file yang optimal sesuai standard blocksize
         blocksize_number = float(hdfs_folder.getLength()*10)/float(blocksize*1024*1024)
         repartition_number = int(1 if blocksize_number < 1 else blocksize_number)
 
-        spark.sql("DROP TABLE dev_ddb.sample_{}_{}".format(table, tag))
+        spark.sql("DROP TABLE {}.sample_{}_{}".format(schema, table, tag))
 
       # set jumlah file sesuai hasil kalkulasi
       df_write = df_write.repartition(repartition_number)
     
       # penghapusan data partisi jika sudah ada di target tabel
       if spark.sql("SHOW TABLES IN {} LIKE '{}'".format(schema, table)).count() != 0:
         query_drop_partition = "ALTER TABLE {}.{} DROP IF EXISTS PARTITION({})".format(schema, table, condition.replace(" AND ",","))
@@ -102,34 +117,34 @@
       row_total += row_count
       print("{}) Count Record ({}) = {}".format(str(i+1).ljust(unit, " "), condition.replace(" AND ",","), row_count))
 
   else:
     
     if not repartition_number:
       # kondisi ketika tabel berpartisi    
-      spark.sql("DROP TABLE IF EXISTS temp.sample_{}".format(table))
+      spark.sql("DROP TABLE IF EXISTS {}.sample_{}".format(schema, table))
 
       # penulisan sample data untuk estimasi ukuran data
       df\
         .sample(False,0.1,None)\
         .write\
         .format("parquet")\
         .mode("overwrite")\
-        .saveAsTable("dev_ddb.sample_{}".format(table))
+        .saveAsTable("{}.sample_{}".format(schema, table))
 
       # mendapatkan metadata content summary dari sample table
       path = lambda p: spark._jvm.org.apache.hadoop.fs.Path(p)
       fs = spark._jvm.org.apache.hadoop.fs.FileSystem.get(spark._jsc.hadoopConfiguration())
-      hdfs_folder = fs.getContentSummary(path("/user/dev/dev_ddb.db/sample_{}/".format(table)))
+      hdfs_folder = fs.getContentSummary(path(hdfs_path+"{}.db/sample_{}_{}/".format(schema, table)))
 
       # kalkulasi jumlah file yang optimal sesuai standard blocksize
       blocksize_number = float(hdfs_folder.getLength()*10)/float(blocksize*1024*1024)
       repartition_number = int(1 if blocksize_number < 1 else blocksize_number)
 
-      spark.sql("DROP TABLE dev_ddb.sample_{}".format(table))
+      spark.sql("DROP TABLE {}.sample_{}".format(schema, table))
 
     # set jumlah file sesuai hasil kalkulasi
     df = df.repartition(repartition_number)
 
     # penulisan pyspark dataframe ke hdfs
     df\
       .write\
@@ -385,15 +400,14 @@
   conn.close()
 
   
 def mysql_execute_fetchall(schema, ip, port, username, password, query):
   """Menjalankan query di mysql
   
   Args:
-      database (str): target database di mysql
       schema (str): target schema di mysql
       table (str): target table di mysql
       ip (str): target ip di mysql
       port (str): target port di mysql
       username (str): username di mysql
       password (str): password di mysql
       query (str): query yang akan di eksekusi
@@ -427,15 +441,14 @@
 
 
   
 def mysql_drop_table(schema, table, ip, port, username, password):
   """Melakukan query drop table di mysql
   
   Args:
-      database (str): target database di mysql
       schema (str): target schema di mysql yang akan di hapus
       table (str): target table di mysql yang akan di hapus
       ip (str): target ip di mysql
       port (str): target port di mysql
       username (str): username di mysql
       password (str): password di mysql
     
@@ -449,15 +462,14 @@
   # eksekusi query drop table
   mysql_execute_command(schema, ip, port, username, password, query)
         
 def mysql_truncate_table(schema, table, ip, port, username, password):
   """Melakukan query truncate table di mysql
   
   Args:
-      database (str): target database di mysql
       schema (str): target schema di mysql yang akan di truncate
       table (str): target table di mysql yang akan di truncate
       ip (str): target ip di mysql
       port (str): target port di mysql
       username (str): username di mysql
       password (str): password di mysql
     
@@ -472,15 +484,14 @@
   mysql_execute_command(schema, ip, port, username, password, query)
   
 def load_to_mysql(df, schema, table, ip, port, username, password, mode="append", strategy=None, ddl=None):
   """Melakukan penulisan pyspark dataframe sebagai tabel di mysql
   
   Args:
       df (pyspark.sql.dataframe.DataFrame): pyspark dataframe yang akan di tulis sebagai tabel mysql
-      database (str): target database di mysql
       schema (str): target schema di mysql
       table (str): target table di mysql
       ip (str): target ip di mysql
       port (str): target port di mysql
       username (str): username di mysql
       password (str): password di mysql
       mode (str): cara yang dilakukan untuk penulisan tabel
```

### Comparing `bribrain-1.0.0/setup.py` & `bribrain-1.0.1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '1.0.1'
 DESCRIPTION = 'Standard code for Dept BRIBrain'
 
 # Setting up
 setup(
     name="bribrain",
     version=VERSION,
     author="Andri Ariyanto",
     author_email="ariyant.andri@gmail.com",
     description=DESCRIPTION,
     packages=find_packages(),
-    install_requires=['mysql-connector-python', 'psycopg2', 'pycrypto'],
-    keywords=['python', 'ddb', 'bribrain'],
+    install_requires=['mysql-connector-python==8.0.28', 'psycopg2'],
+    keywords=['python', 'ddb', 'bribrain', 'andri', 'gondrol'],
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ]
 )
```

