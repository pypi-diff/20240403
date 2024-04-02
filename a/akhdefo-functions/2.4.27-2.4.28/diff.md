# Comparing `tmp/akhdefo_functions-2.4.27-py3-none-any.whl.zip` & `tmp/akhdefo_functions-2.4.28-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 164202 bytes, number of entries: 20
+Zip file size: 164261 bytes, number of entries: 20
 -rw-rw-rw-  2.0 fat    16653 b- defN 24-Feb-22 18:14 akhdefo_functions/ASF.py
 -rw-rw-rw-  2.0 fat    53386 b- defN 24-Feb-16 02:34 akhdefo_functions/AkhdefoPlot.py
 -rw-rw-rw-  2.0 fat     9259 b- defN 24-Jan-03 23:08 akhdefo_functions/Akhdefo_Coreg.py
 -rw-rw-rw-  2.0 fat   114378 b- defN 24-Feb-21 21:23 akhdefo_functions/Akhdefo_GOI.py
 -rw-rw-rw-  2.0 fat    45641 b- defN 24-Feb-16 03:08 akhdefo_functions/Akhdefo_TS.py
 -rw-rw-rw-  2.0 fat    87861 b- defN 24-Jan-28 01:23 akhdefo_functions/Akhdefo_Tools.py
--rw-rw-rw-  2.0 fat   153287 b- defN 24-Mar-28 19:23 akhdefo_functions/Akhdefo_Utilities.py
+-rw-rw-rw-  2.0 fat   153511 b- defN 24-Apr-02 23:18 akhdefo_functions/Akhdefo_Utilities.py
 -rw-rw-rw-  2.0 fat    27051 b- defN 24-Feb-22 03:34 akhdefo_functions/Filter_PreProc.py
 -rw-rw-rw-  2.0 fat     8056 b- defN 24-Jan-03 23:08 akhdefo_functions/Mosaic_Crop.py
 -rw-rw-rw-  2.0 fat    45101 b- defN 24-Jan-03 23:08 akhdefo_functions/OpticalFlow.py
 -rw-rw-rw-  2.0 fat    12943 b- defN 24-Feb-19 20:51 akhdefo_functions/S1.py
 -rw-rw-rw-  2.0 fat    38790 b- defN 24-Jan-03 23:08 akhdefo_functions/Stacked_Velocity.py
 -rw-rw-rw-  2.0 fat    11849 b- defN 24-Jan-03 23:08 akhdefo_functions/Unzip_CopyFiles.py
 -rw-rw-rw-  2.0 fat     9190 b- defN 24-Jan-28 10:03 akhdefo_functions/Video_Streamer.py
--rw-rw-rw-  2.0 fat      619 b- defN 24-Mar-28 19:24 akhdefo_functions/__init__.py
+-rw-rw-rw-  2.0 fat      619 b- defN 24-Apr-02 23:19 akhdefo_functions/__init__.py
 -rw-rw-rw-  2.0 fat     2128 b- defN 24-Feb-19 20:51 akhdefo_functions/tqdm_joblib.py
--rw-rw-rw-  2.0 fat     3936 b- defN 24-Mar-28 19:25 akhdefo_functions-2.4.27.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Mar-28 19:25 akhdefo_functions-2.4.27.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       18 b- defN 24-Mar-28 19:25 akhdefo_functions-2.4.27.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1782 b- defN 24-Mar-28 19:25 akhdefo_functions-2.4.27.dist-info/RECORD
-20 files, 642020 bytes uncompressed, 161284 bytes compressed:  74.9%
+-rw-rw-rw-  2.0 fat     3936 b- defN 24-Apr-02 23:21 akhdefo_functions-2.4.28.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-02 23:21 akhdefo_functions-2.4.28.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       18 b- defN 24-Apr-02 23:21 akhdefo_functions-2.4.28.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1782 b- defN 24-Apr-02 23:21 akhdefo_functions-2.4.28.dist-info/RECORD
+20 files, 642244 bytes uncompressed, 161343 bytes compressed:  74.9%
```

## zipnote {}

```diff
@@ -42,20 +42,20 @@
 
 Filename: akhdefo_functions/__init__.py
 Comment: 
 
 Filename: akhdefo_functions/tqdm_joblib.py
 Comment: 
 
-Filename: akhdefo_functions-2.4.27.dist-info/METADATA
+Filename: akhdefo_functions-2.4.28.dist-info/METADATA
 Comment: 
 
-Filename: akhdefo_functions-2.4.27.dist-info/WHEEL
+Filename: akhdefo_functions-2.4.28.dist-info/WHEEL
 Comment: 
 
-Filename: akhdefo_functions-2.4.27.dist-info/top_level.txt
+Filename: akhdefo_functions-2.4.28.dist-info/top_level.txt
 Comment: 
 
-Filename: akhdefo_functions-2.4.27.dist-info/RECORD
+Filename: akhdefo_functions-2.4.28.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## akhdefo_functions/Akhdefo_Utilities.py

```diff
@@ -2162,14 +2162,15 @@
             new_image[y, x] = new_value
         
         return new_image
     
     
     ############################
     
+    import logging
 
     def set_video_bitrate(input_video_path, output_video_path, bitrate_kbps):
         """
         Set the bitrate of a video using FFmpeg. If the output file already exists, a new file with a suffix is created instead.
 
         Parameters:
         - input_video_path: Path to the input video file.
@@ -2193,20 +2194,23 @@
                 'ffmpeg',
                 '-i', input_video_path,
                 '-b:v', f'{bitrate_kbps}k',
                 '-bufsize', f'{int(bitrate_kbps * 2)}k',  # Optional: Adjust buffer size
                 output_video_path
             ]
 
-            # Execute the FFmpeg command
             subprocess.run(command, check=True)
-
-            print(f"Video with bitrate {bitrate_kbps} kbps saved as {output_video_path}")
+            logging.info(f"Video with bitrate {bitrate_kbps} kbps saved as {output_video_path}")
+            return True
         except subprocess.CalledProcessError as e:
-            print(f"Failed to set bitrate: {e}")
+            logging.error(f"Failed to set bitrate: {e}")
+            return False
+        except Exception as e:
+            logging.error(f"An unexpected error occurred: {e}")
+            return False
     
     def delete_older_mp4(folder_path, bitrate_kbps):
         # Convert string path to Path object for easier manipulation
         folder = Path(folder_path)
         
         # Ensure the "converted" subfolder exists
         converted_folder = folder / "converted"
@@ -2220,15 +2224,15 @@
             # Get the last modified times of the files
             file_mod_times = [(file, os.path.getmtime(file)) for file in mp4_files]
             
             # Sort the files based on modification time (most recent last)
             sorted_files = sorted(file_mod_times, key=lambda x: x[1], reverse=True)
             
             # Exclude the most recent file from conversion
-            files_to_convert = sorted_files[5:]  # All except the most recent
+            files_to_convert = sorted_files [1:]  # All except the most recent
             
             for file, _ in files_to_convert:
                 # Define the output path for the converted file
                 converted_output_path = converted_folder / file.name
                 
                 # Apply video conversion here; example function call (set_video_bitrate)
                 # Assuming set_video_bitrate function is defined to take source path, output path, and bitrate
@@ -2253,17 +2257,19 @@
                         print(f"An unexpected error occurred: {e}")
                         break  # Exit the loop on any other exception
 
                 if not success:
                     print(f"Operation skipped after {5} attempts.")
                             
                     print(f"Converted and saved: {converted_output_path}")
-                # Optionally, delete the original file after conversion
-                os.remove(file)
-                # print(f"Deleted original file: {file.name}")
+                try:
+                    os.remove(file)
+                except Exception as e:  # Catching all exceptions
+                    pass  # If an error occurs, just skip the deletion and continue the program
+
 
     def delete_files_except_last_n(directory, n=2):
         """Delete all files in the given directory except the last n files based on modification time."""
         files = list(Path(directory).glob('*'))  # List all items in the directory
         files = [f for f in files if f.is_file()]  # Filter out subdirectories
         files.sort(key=os.path.getmtime, reverse=True)  # Sort files by modification time, newest first
 
@@ -3103,16 +3109,16 @@
             out_v.release()   
             # Release everything when done
             
             
             os.replace(temp_file_name, save_gif_image)
            
             
-            #if current_hour!=last_hour:
-            delete_older_mp4('plots/Videos', 1500)
+            if current_hour!=last_hour:
+                delete_older_mp4('plots/Videos', 1500)
                 
                 #shutil.move(temp_file_name, save_gif_image)
                 
             # if not ret:  
             #     for img in imagescreenshot_list:
             #         # Assuming the images are in BGR format, if not, convert them
             #         out_v.write(img)
```

## akhdefo_functions/__init__.py

```diff
@@ -1,14 +1,14 @@
 """
 akhdefo_functions
 
 collection of python modules performs geospatial image processing to moniter land deformation
 """
 
-__version__ = "2.4.27"
+__version__ = "2.4.28"
 __author__ = 'Mahmud Mustafa Muhammad'
 __credits__ = 'Simon Fraser university-Department of Earth Sciences'
 
 
 from .AkhdefoPlot import*
 from .Akhdefo_Tools import*
 from .Akhdefo_TS import*
```

## Comparing `akhdefo_functions-2.4.27.dist-info/METADATA` & `akhdefo_functions-2.4.28.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akhdefo-functions
-Version: 2.4.27
+Version: 2.4.28
 Summary: Land Deformation Monitoring Using Optical Satellite Imagery
 Home-page: https://github.com/mahmudsfu/AkhDefo
 Author: Mahmud Mustafa Muhammad
 Author-email: Mahmud Mustafa Muhammad <mahmud.muhamm1@gmail.com>
 License: Academic Free License (AFL)
 Project-URL: GitHub-Page, https://github.com/mahmudsfu/AkhDefo
 Project-URL: Bug Tracker, https://github.com/mahmudsfu/AkhDefo/issues
```

## Comparing `akhdefo_functions-2.4.27.dist-info/RECORD` & `akhdefo_functions-2.4.28.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 akhdefo_functions/ASF.py,sha256=AihzExxQedmh9TpJXuQd68P1LQuQ_5db6P_PAElJ2sM,16653
 akhdefo_functions/AkhdefoPlot.py,sha256=84cBmjfNpcMGfhfVv8MBmDCdW5igAXqdJwfrG8a80Es,53386
 akhdefo_functions/Akhdefo_Coreg.py,sha256=UuuPPszg4cH-KOyraCdYAazbIoKeXiZ0yK3iUF8XtMI,9259
 akhdefo_functions/Akhdefo_GOI.py,sha256=NIdUTrE6Lv_ZcMyWt7d03-SZm-gAj5D3Wr2VHX7Ydps,114378
 akhdefo_functions/Akhdefo_TS.py,sha256=wsJh7LWEuPupTXSmIH029rLfLdM18h33P-e6TkfQeSY,45641
 akhdefo_functions/Akhdefo_Tools.py,sha256=5mwra9yY45gRvXV9mtcr_sL8fWqstDHSg79mx-M2WSc,87861
-akhdefo_functions/Akhdefo_Utilities.py,sha256=5WkQGzAqHCV87m4tkIn7rI-HbtPZ6F7vZKUuXf8SDAs,153287
+akhdefo_functions/Akhdefo_Utilities.py,sha256=mVevWu9OQ5E59HakEWksoeW3z_ZzH9vE8JMlStPr6Iw,153511
 akhdefo_functions/Filter_PreProc.py,sha256=E8LRXjJmos0nHpjR6QIaCymluQdfFqrDoXyRWSSTYn8,27051
 akhdefo_functions/Mosaic_Crop.py,sha256=E-NgHQLqyTwjHoAIZgGRO2OiPupS6xPmPQTr_l3ieuo,8056
 akhdefo_functions/OpticalFlow.py,sha256=Vf7wHnVxwpSE51ZlvraSALSSfG6JwdchuL0GkN68DvA,45101
 akhdefo_functions/S1.py,sha256=x6D0MZdhRgcGnp_DN6eD6WutPboFczN5WS6WLzKb3E4,12943
 akhdefo_functions/Stacked_Velocity.py,sha256=YkHPI9NMhf_k6nKzzU8tUY5tv5Oa4feyatPHEOtFRmg,38790
 akhdefo_functions/Unzip_CopyFiles.py,sha256=-KlUh2hfSsPuCCEU02zuRkQb7t7y7AzCF342xNw7yWQ,11849
 akhdefo_functions/Video_Streamer.py,sha256=vnKu6SVM_rt3e_bZXrejpnR2NOW2TYVdAwyKe1FZljY,9190
-akhdefo_functions/__init__.py,sha256=C4kwNorDHRD1c91w0Nsf0fbIIaSgvfI8FAUHZl12cVo,619
+akhdefo_functions/__init__.py,sha256=1xnOuTRZitSXa4b6EWrvRdWm1NBA2a1r3eYrQfrI-3E,619
 akhdefo_functions/tqdm_joblib.py,sha256=FeR0O-APzoGIrHifyWbyP6zXAiIXBYweqeGieJ6iWuM,2128
-akhdefo_functions-2.4.27.dist-info/METADATA,sha256=jgejsZ2XO_kArdtWEc_EwxgRl35gHoKKr8XT8frSNVs,3936
-akhdefo_functions-2.4.27.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-akhdefo_functions-2.4.27.dist-info/top_level.txt,sha256=f44EhlHyHyMPViIAioSeoagzxgVrlg6NsdfXRHB7U-U,18
-akhdefo_functions-2.4.27.dist-info/RECORD,,
+akhdefo_functions-2.4.28.dist-info/METADATA,sha256=gDFBbDTztITD6amWMFzTAzwAfK9BADIl2nUlUAjkFUk,3936
+akhdefo_functions-2.4.28.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+akhdefo_functions-2.4.28.dist-info/top_level.txt,sha256=f44EhlHyHyMPViIAioSeoagzxgVrlg6NsdfXRHB7U-U,18
+akhdefo_functions-2.4.28.dist-info/RECORD,,
```

