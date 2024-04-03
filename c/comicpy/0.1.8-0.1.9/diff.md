# Comparing `tmp/comicpy-0.1.8.tar.gz` & `tmp/comicpy-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comicpy-0.1.8.tar", max compression
+gzip compressed data, was "comicpy-0.1.9.tar", max compression
```

## Comparing `comicpy-0.1.8.tar` & `comicpy-0.1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     5328 2024-02-26 17:33:26.964873 comicpy-0.1.8/README.md
--rw-r--r--   0        0        0      563 2024-02-25 15:36:56.100244 comicpy-0.1.8/comicpy/__init__.py
--rw-r--r--   0        0        0     2692 2024-02-20 21:42:24.273422 comicpy-0.1.8/comicpy/checkfile.py
--rw-r--r--   0        0        0     7019 2024-02-26 17:16:16.181003 comicpy-0.1.8/comicpy/cli.py
--rw-r--r--   0        0        0    22645 2024-02-26 17:11:51.535530 comicpy-0.1.8/comicpy/comicpy.py
--rw-r--r--   0        0        0     2084 2024-02-25 01:40:46.946642 comicpy-0.1.8/comicpy/exceptionsClasses.py
--rw-r--r--   0        0        0      817 2024-02-20 21:42:25.878437 comicpy-0.1.8/comicpy/filesigns.py
--rw-r--r--   0        0        0      186 2024-02-17 16:05:33.435937 comicpy-0.1.8/comicpy/handlers/__init__.py
--rw-r--r--   0        0        0     6234 2024-02-26 16:54:14.706626 comicpy-0.1.8/comicpy/handlers/baseziprar.py
--rw-r--r--   0        0        0     1835 2024-02-26 16:07:55.485823 comicpy-0.1.8/comicpy/handlers/imageshandler.py
--rw-r--r--   0        0        0     3406 2024-02-26 16:05:49.338720 comicpy-0.1.8/comicpy/handlers/pdfhandler.py
--rw-r--r--   0        0        0     8350 2024-02-26 16:56:33.039970 comicpy-0.1.8/comicpy/handlers/rarhandler.py
--rw-r--r--   0        0        0     7483 2024-02-26 17:00:58.436471 comicpy-0.1.8/comicpy/handlers/ziphandler.py
--rw-r--r--   0        0        0     6231 2024-02-26 02:39:21.408126 comicpy-0.1.8/comicpy/models.py
--rw-r--r--   0        0        0     2754 2024-02-26 17:10:55.653012 comicpy-0.1.8/comicpy/utils.py
--rw-r--r--   0        0        0     1814 2024-02-26 15:59:51.495594 comicpy-0.1.8/comicpy/valid_extentions.py
--rw-r--r--   0        0        0      944 2024-02-26 17:33:58.461185 comicpy-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     6288 1970-01-01 00:00:00.000000 comicpy-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     5264 2024-02-26 17:42:09.213037 comicpy-0.1.9/README.md
+-rw-r--r--   0        0        0      563 2024-02-25 15:36:56.100244 comicpy-0.1.9/comicpy/__init__.py
+-rw-r--r--   0        0        0     2692 2024-02-20 21:42:24.273422 comicpy-0.1.9/comicpy/checkfile.py
+-rw-r--r--   0        0        0     7019 2024-02-26 17:16:16.181003 comicpy-0.1.9/comicpy/cli.py
+-rw-r--r--   0        0        0    22299 2024-02-26 23:01:02.759516 comicpy-0.1.9/comicpy/comicpy.py
+-rw-r--r--   0        0        0     2084 2024-02-25 01:40:46.946642 comicpy-0.1.9/comicpy/exceptionsClasses.py
+-rw-r--r--   0        0        0      817 2024-02-20 21:42:25.878437 comicpy-0.1.9/comicpy/filesigns.py
+-rw-r--r--   0        0        0      186 2024-02-17 16:05:33.435937 comicpy-0.1.9/comicpy/handlers/__init__.py
+-rw-r--r--   0        0        0     6427 2024-02-26 22:57:19.147467 comicpy-0.1.9/comicpy/handlers/baseziprar.py
+-rw-r--r--   0        0        0     1863 2024-02-26 21:59:17.684126 comicpy-0.1.9/comicpy/handlers/imageshandler.py
+-rw-r--r--   0        0        0     3406 2024-02-26 22:54:26.152854 comicpy-0.1.9/comicpy/handlers/pdfhandler.py
+-rw-r--r--   0        0        0     7984 2024-02-26 22:37:14.826269 comicpy-0.1.9/comicpy/handlers/rarhandler.py
+-rw-r--r--   0        0        0     7211 2024-02-26 23:04:14.147209 comicpy-0.1.9/comicpy/handlers/ziphandler.py
+-rw-r--r--   0        0        0     6247 2024-02-26 23:01:56.331990 comicpy-0.1.9/comicpy/models.py
+-rw-r--r--   0        0        0     2754 2024-02-26 17:10:55.653012 comicpy-0.1.9/comicpy/utils.py
+-rw-r--r--   0        0        0     1814 2024-02-26 15:59:51.495594 comicpy-0.1.9/comicpy/valid_extentions.py
+-rw-r--r--   0        0        0      944 2024-02-26 23:05:44.156005 comicpy-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     6224 1970-01-01 00:00:00.000000 comicpy-0.1.9/PKG-INFO
```

### Comparing `comicpy-0.1.8/README.md` & `comicpy-0.1.9/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -75,16 +75,18 @@
 | --join | Join or does not files thath are in the directory. Default is "False". |
 | -u {b,kb,mb,gb}, --unit {b,kb,mb,gb} | Unit of measure of data size. Default is "mb". |
 | --password PASSWORD | Password of file protected. |
 
 
 ```bash
 $ comicpy --type d -p rars_dir --filter rar -c rar --check --join -o prefix_final_ --password PASS
+$ for i in $(ls -d Zip_Dir_*/); do
+> comicpy --type d -p "$i" --filter zip -c zip --check -o ${i: 0:-1} --join
+> done
 $
-$ for i in $(ls -d Zip_Dir_*/); do comicpy --type d -p $i --filter zip -c zip --check -o ${i: 0:-1} --join ; done
 ```
 
 
 
 ## Development - usage
 
 > `path='.'` parameter of `ComicPy.to_write()`, indicates that files will be written by default to the current directory. It can be changed.
@@ -134,18 +136,24 @@
 ...             extention_filter='rar',
 ...             compressor='rar',
 ...             password=None,
 ...             join=False
 ...           )
 >>> metaFileCompress = comic.to_write(listCurrentFiles=data)
 >>> print(metaFileCompress)
-[{'name': './final_CBR_file/chapter_1.cbr', 'size': '0.02 GB'}, {'name': './final_CBR_file/chapter_2.cbr', 'size': '0.01 GB'}, {'name': './final_CBR_file/chapter_3.cbr', 'size': '0.01 GB'}, {'name': './final_CBR_file/chapter_4.cbr', 'size': '0.01 GB'}]
+[
+  {'name': './final_CBR_file/chapter_1.cbr', 'size': '0.02 GB'},
+  {'name': './final_CBR_file/chapter_2.cbr', 'size': '0.01 GB'}
+]
 >>>>
 >>> for item in metaFileCompress:
-...   comic.check_integrity(filename=item['name'], show=True)
+...   comic.check_integrity(
+...      filename=item['name'],
+...      show=True
+...   )
 ...
 File is valid?:  "True"
 True
 File is valid?:  "True"
 True
 File is valid?:  "True"
 True
@@ -173,13 +181,16 @@
 ...                 join=True
 ...               )
 >>> metaFileCompress = comic.to_write(listCurrentFiles=data)
 >>> print(metaFileCompress)
 [{'name': 'result/final_CBR_file/final_CBR_file.cbr', 'size': '0.05 GB'}]
 >>>
 >>> for item in metaFileCompress:
-...   comic.check_integrity(filename=item['name'], show=True)
+...   comic.check_integrity(
+...      filename=item['name'],
+...      show=True
+...   )
 ...
 File is valid?:  "True"
 True
 >>>
 ```
```

### Comparing `comicpy-0.1.8/comicpy/__init__.py` & `comicpy-0.1.9/comicpy/__init__.py`

 * *Files identical despite different names*

### Comparing `comicpy-0.1.8/comicpy/checkfile.py` & `comicpy-0.1.9/comicpy/checkfile.py`

 * *Files identical despite different names*

### Comparing `comicpy-0.1.8/comicpy/cli.py` & `comicpy-0.1.9/comicpy/cli.py`

 * *Files identical despite different names*

### Comparing `comicpy-0.1.8/comicpy/comicpy.py` & `comicpy-0.1.9/comicpy/comicpy.py`

 * *Files 2% similar despite different names*

```diff
@@ -225,15 +225,15 @@
             return True
         return False
 
     def process_pdf(
         self,
         filename: str,
         compressor: Union[RAR, ZIP] = 'zip',
-    ) -> CompressorFileData:
+    ) -> List[CurrentFile]:
         """
         Process PDF file, load content, extract images.
 
         Args:
             filename: str -> PDF file name.
 
         Returns:
@@ -246,40 +246,32 @@
 
         compressor = compressor.replace('.', '').lower().strip()
 
         self.raiser_error_compressor(compressor_str=compressor)
 
         self.check_file(currentFile=self.currentFile)
 
-        listImagesPDF = self.pdfphandler.process_pdf(
-                            currentFilePDF=self.currentFile
+        compressFileData = self.pdfphandler.process_pdf(
+                            currentFilePDF=self.currentFile,
+                            compressor=compressor
                         )
-        compressFileData = CompressorFileData(
-                    filename=self.currentFile.name.replace(' ', '_'),
-                    list_data=listImagesPDF,
-                    type=compressor,
-                    unit=self.unit
-                )
-        compressFileData.setExtention()
 
         compressedCurrentFileIO = self.to_compressor(
                             filename=compressFileData.filename,
-                            dataRawFile=compressFileData,
+                            listCompressorData=compressFileData,
                             compressor=compressor,
                             join_files=False
                         )
-        compressedCurrentFileIO.name = self.currentFile.name
-
         return compressedCurrentFileIO
 
     def process_zip(
         self,
         filename: str,
         password: str = None
-    ) -> CompressorFileData:
+    ) -> List[CurrentFile]:
         """
         Process ZIP files.
 
         Args:
             filename: str -> ZIP file name.
 
         Returns:
@@ -293,38 +285,38 @@
 
         is_protected = self.check_protectedFile(
                 handler=self.ziphandler,
                 compressCurrentFile=self.currentFile,
                 password=password
             )
         if is_protected:
-            # zipCompressorFileData = self.ziphandler.extract_images(
             zipCompressorFileData = self.ziphandler.extract_content(
                                         currentFileZip=self.currentFile,
                                         password=password
                                     )
+
             compressedCurrentFileIO = self.to_compressor(
                                 filename=zipCompressorFileData.filename,
-                                dataRawFile=[zipCompressorFileData],
+                                listCompressorData=[zipCompressorFileData],
                                 compressor='zip',
                                 join_files=False
                             )
             return compressedCurrentFileIO
 
         else:
             zipCompressorFileData = self.ziphandler.rename_zip_cbz(
                                     currentFileZip=self.currentFile
                                 )
-            return zipCompressorFileData
+            return [zipCompressorFileData]
 
     def process_rar(
         self,
         filename: str,
         password: str = None
-    ) -> CompressorFileData:
+    ) -> List[CurrentFile]:
         """
         Process RAR files.
 
         Args:
             filename: str -> RAR file name.
 
         Returns:
@@ -333,36 +325,36 @@
         """
 
         self.load_file(filename=filename)
 
         self.check_file(currentFile=self.currentFile)
 
         is_protected = self.check_protectedFile(
-                handler=self.ziphandler,
+                handler=self.rarhandler,
                 compressCurrentFile=self.currentFile,
                 password=password
             )
         if is_protected:
-            rarCompressorFileData = self.rarhandler.extract_images(
+            rarCompressorFileData = self.rarhandler.extract_content(
                                         currentFileRar=self.currentFile,
                                         password=password
                                     )
             compressedCurrentFileIO = self.to_compressor(
                                 filename=rarCompressorFileData.filename,
-                                dataRawFile=[rarCompressorFileData],
+                                listCompressorData=[rarCompressorFileData],
                                 compressor='rar',
                                 join_files=False
                             )
             return compressedCurrentFileIO
 
         else:
             rarCompressorFileData = self.rarhandler.rename_rar_cbr(
                                     currentFileRar=self.currentFile
                                 )
-            return rarCompressorFileData
+            return [rarCompressorFileData]
 
     def get_file_glob(
         self,
         extention: str
     ) -> list:
         """
         Search by extention.
```

### Comparing `comicpy-0.1.8/comicpy/exceptionsClasses.py` & `comicpy-0.1.9/comicpy/exceptionsClasses.py`

 * *Files identical despite different names*

### Comparing `comicpy-0.1.8/comicpy/filesigns.py` & `comicpy-0.1.9/comicpy/filesigns.py`

 * *Files identical despite different names*

### Comparing `comicpy-0.1.8/comicpy/handlers/baseziprar.py` & `comicpy-0.1.9/comicpy/handlers/baseziprar.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,47 +36,50 @@
         self.imageshandler = ImagesHandler()
 
     def read_file(
         self,
         instanceCompress: Union[RarFile, AESZipFile],
         itemFile: bytes,
         password: str = None,
-    ) -> None:
+    ) -> bytes:
         """
         Read data of file, using password for protected files.
 
         Args
             instanceCompress: `RarFile` or `AESZipFile` instance.
             item: file to read.
             password: password string to unlock the archive data.
 
         Returns
+            bytes: data of file.
         """
         if isinstance(instanceCompress, AESZipFile):
             return instanceCompress.read(itemFile)
         elif isinstance(instanceCompress, RarFile):
             return instanceCompress.read(
                                     itemFile,
                                     pwd=password
                                 )
 
     def iterateFiles(
         self,
         instanceCompress: Union[RarFile, AESZipFile],
         password: str = None
-    ) -> list:
+    ) -> CompressorFileData:
         """
         Iterates over files of RAR or ZIP files, read their data.
 
         Args
             instanceCompress: `RarFile` or `AESZipFile` instance.
             password: password string to unlock the archive data.
 
-        Returns
-            list: list of content of file RAR or ZIP.
+        Returns:
+            CompressorFileData: instances contains name of directory of images,
+                                list of ImageComicData instances, type of
+                                compressor.
         """
         images_Extentions = self.validextentions.get_images_extentions()
         listContentData = []
         directory_name = None
 
         for item in instanceCompress.namelist():
             directory_name = self.paths.get_dirname(item).replace(' ', '_')
```

### Comparing `comicpy-0.1.8/comicpy/handlers/imageshandler.py` & `comicpy-0.1.9/comicpy/handlers/imageshandler.py`

 * *Files 9% similar despite different names*

```diff
@@ -63,10 +63,11 @@
         if type(currentImage) is bytes:
             currentImage = Image.open(io.BytesIO(currentImage))
 
         imageResized = currentImage.resize(size_tuple)
 
         imageResized.save(
                 newImageIO,
-                format=ImagesHandler.validFormats[extention]
+                format=ImagesHandler.validFormats[extention],
+                quality=90
             )
         return newImageIO
```

### Comparing `comicpy-0.1.8/comicpy/handlers/pdfhandler.py` & `comicpy-0.1.9/comicpy/handlers/pdfhandler.py`

 * *Files identical despite different names*

### Comparing `comicpy-0.1.8/comicpy/handlers/rarhandler.py` & `comicpy-0.1.9/comicpy/handlers/rarhandler.py`

 * *Files 7% similar despite different names*

```diff
@@ -77,34 +77,27 @@
             return False
         except PasswordRequired:
             return True
 
     def rename_rar_cbr(
         self,
         currentFileRar: CurrentFile
-    ) -> CompressorFileData:
+    ) -> CurrentFile:
         """
         Add CBR name and extention of `CurrentFile` instance.
 
         Args:
             CurrentFile: instance with data RAR file.
 
         Returns:
             CurrentFile: same instance with new name and extention.
         """
         currentFileRar.extention = '.cbr'
         currentFileRar.name = currentFileRar.name.replace(' ', '_')
-        rarFileCompress = CompressorFileData(
-                                    filename=currentFileRar.name,
-                                    list_data=[currentFileRar],
-                                    type='rar',
-                                    unit=self.unit,
-                                    join=False,
-                                )
-        return rarFileCompress
+        return currentFileRar
 
     def extract_content(
         self,
         currentFileRar: CurrentFile,
         password: str = None,
         imageSize: Union[SMALL, MEDIUM, LARGE] = 'small'
     ) -> CompressorFileData:
```

### Comparing `comicpy-0.1.8/comicpy/handlers/ziphandler.py` & `comicpy-0.1.9/comicpy/handlers/ziphandler.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,34 +71,27 @@
             return False
         except RuntimeError:
             return True
 
     def rename_zip_cbz(
         self,
         currentFileZip: CurrentFile
-    ) -> CompressorFileData:
+    ) -> CurrentFile:
         """
         Add CBZ name and extention of `CurrentFile` instance.
 
         Args:
             CurrentFile: instance with data ZIP file.
 
         Returns:
             CurrentFile: same instance with new name and extention.
         """
         currentFileZip.extention = '.cbz'
         currentFileZip.name = currentFileZip.name.replace(' ', '_')
-        zipFileCompress = CompressorFileData(
-                                    filename=currentFileZip.name,
-                                    list_data=[currentFileZip],
-                                    type='zip',
-                                    unit=self.unit,
-                                    join=False,
-                                )
-        return zipFileCompress
+        return currentFileZip
 
     def extract_content(
         self,
         currentFileZip: CurrentFile,
         password: str = None,
         imageSize: Union[SMALL, MEDIUM, LARGE] = 'small',
     ) -> CompressorFileData:
@@ -120,14 +113,17 @@
         with pyzipper.AESZipFile(
             bytesZipFile,
             mode='r',
             compression=pyzipper.ZIP_DEFLATED,
             encryption=pyzipper.WZ_AES
         ) as zip_file:
 
+            if password is not None:
+                zip_file.pwd = password.encode('utf-8')
+
             return super().iterateFiles(
                 instanceCompress=zip_file,
                 password=password
             )
 
     def to_zip(
         self,
```

### Comparing `comicpy-0.1.8/comicpy/models.py` & `comicpy-0.1.9/comicpy/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,16 +183,17 @@
         self.filename = filename
         self.list_data = list_data
         self.type = type
         self.join = join
         self.items = 0
         self.extention = None
         self.unit = unit
-        self.size = self.get_size()
+        self.size = 0
         self.set_items()
+        self.get_size()
 
     def set_items(self) -> None:
         self.items = len(self.list_data)
 
     def setExtention(self) -> str:
         """
         Sets `extention` attribute.
@@ -228,15 +229,16 @@
             self.unit = 'mb'
             size_unit = SizeUnits[self.unit]
 
         sizes = [
             item.bytes_data.getbuffer().nbytes
             for item in self.list_data
         ]
-        return sum(sizes) / size_unit
+
+        self.size = sum(sizes) / size_unit
 
     def __len__(self) -> int:
         return len(self.list_data)
 
     def __str__(self) -> str:
         """
         Returns:
```

### Comparing `comicpy-0.1.8/comicpy/utils.py` & `comicpy-0.1.9/comicpy/utils.py`

 * *Files identical despite different names*

### Comparing `comicpy-0.1.8/comicpy/valid_extentions.py` & `comicpy-0.1.9/comicpy/valid_extentions.py`

 * *Files identical despite different names*

### Comparing `comicpy-0.1.8/pyproject.toml` & `comicpy-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "comicpy"
-version = "0.1.8"
+version = "0.1.9"
 description = "Tool to create CBR or CBZ files, supports PDF, ZIP, RAR files."
 authors = ["kurotom <55354389+kurotom@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{include = 'comicpy'}]
 keywords = ["comic", "cbz", "cbr", "manga"]
 repository = "https://github.com/kurotom/comicpy"
 classifiers = [
```

### Comparing `comicpy-0.1.8/PKG-INFO` & `comicpy-0.1.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comicpy
-Version: 0.1.8
+Version: 0.1.9
 Summary: Tool to create CBR or CBZ files, supports PDF, ZIP, RAR files.
 Home-page: https://github.com/kurotom/comicpy
 Keywords: comic,cbz,cbr,manga
 Author: kurotom
 Author-email: 55354389+kurotom@users.noreply.github.com
 Requires-Python: >=3.7,<4.0
 Classifier: Operating System :: OS Independent
@@ -99,16 +99,18 @@
 | --join | Join or does not files thath are in the directory. Default is "False". |
 | -u {b,kb,mb,gb}, --unit {b,kb,mb,gb} | Unit of measure of data size. Default is "mb". |
 | --password PASSWORD | Password of file protected. |
 
 
 ```bash
 $ comicpy --type d -p rars_dir --filter rar -c rar --check --join -o prefix_final_ --password PASS
+$ for i in $(ls -d Zip_Dir_*/); do
+> comicpy --type d -p "$i" --filter zip -c zip --check -o ${i: 0:-1} --join
+> done
 $
-$ for i in $(ls -d Zip_Dir_*/); do comicpy --type d -p $i --filter zip -c zip --check -o ${i: 0:-1} --join ; done
 ```
 
 
 
 ## Development - usage
 
 > `path='.'` parameter of `ComicPy.to_write()`, indicates that files will be written by default to the current directory. It can be changed.
@@ -158,18 +160,24 @@
 ...             extention_filter='rar',
 ...             compressor='rar',
 ...             password=None,
 ...             join=False
 ...           )
 >>> metaFileCompress = comic.to_write(listCurrentFiles=data)
 >>> print(metaFileCompress)
-[{'name': './final_CBR_file/chapter_1.cbr', 'size': '0.02 GB'}, {'name': './final_CBR_file/chapter_2.cbr', 'size': '0.01 GB'}, {'name': './final_CBR_file/chapter_3.cbr', 'size': '0.01 GB'}, {'name': './final_CBR_file/chapter_4.cbr', 'size': '0.01 GB'}]
+[
+  {'name': './final_CBR_file/chapter_1.cbr', 'size': '0.02 GB'},
+  {'name': './final_CBR_file/chapter_2.cbr', 'size': '0.01 GB'}
+]
 >>>>
 >>> for item in metaFileCompress:
-...   comic.check_integrity(filename=item['name'], show=True)
+...   comic.check_integrity(
+...      filename=item['name'],
+...      show=True
+...   )
 ...
 File is valid?:  "True"
 True
 File is valid?:  "True"
 True
 File is valid?:  "True"
 True
@@ -197,14 +205,17 @@
 ...                 join=True
 ...               )
 >>> metaFileCompress = comic.to_write(listCurrentFiles=data)
 >>> print(metaFileCompress)
 [{'name': 'result/final_CBR_file/final_CBR_file.cbr', 'size': '0.05 GB'}]
 >>>
 >>> for item in metaFileCompress:
-...   comic.check_integrity(filename=item['name'], show=True)
+...   comic.check_integrity(
+...      filename=item['name'],
+...      show=True
+...   )
 ...
 File is valid?:  "True"
 True
 >>>
 ```
```

