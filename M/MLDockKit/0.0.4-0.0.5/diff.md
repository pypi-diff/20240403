# Comparing `tmp/MLDockKit-0.0.4.tar.gz` & `tmp/MLDockKit-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MLDockKit-0.0.4.tar", last modified: Mon Jan 22 19:59:44 2024, max compression
+gzip compressed data, was "MLDockKit-0.0.5.tar", last modified: Wed Apr  3 09:14:56 2024, max compression
```

## Comparing `MLDockKit-0.0.4.tar` & `MLDockKit-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 clabe     (1000) clabe     (1000)        0 2024-01-22 19:59:44.165727 MLDockKit-0.0.4/
--rw-rw-r--   0 clabe     (1000) clabe     (1000)     1142 2024-01-22 19:28:47.000000 MLDockKit-0.0.4/LICENSE
-drwxrwxr-x   0 clabe     (1000) clabe     (1000)        0 2024-01-22 19:59:44.157727 MLDockKit-0.0.4/MLDockKit/
--rw-rw-r--   0 clabe     (1000) clabe     (1000)   181468 2024-01-22 19:28:47.000000 MLDockKit-0.0.4/MLDockKit/5gs4.pdbqt
--rw-rw-r--   0 clabe     (1000) clabe     (1000)     8732 2024-01-22 19:28:47.000000 MLDockKit-0.0.4/MLDockKit/MLDockKit.py
--rw-rw-r--   0 clabe     (1000) clabe     (1000)       48 2024-01-22 19:30:05.000000 MLDockKit-0.0.4/MLDockKit/__init__.py
--rw-rw-r--   0 clabe     (1000) clabe     (1000) 18848673 2024-01-22 19:28:48.000000 MLDockKit-0.0.4/MLDockKit/padel_model.joblib
-drwxrwxr-x   0 clabe     (1000) clabe     (1000)        0 2024-01-22 19:59:44.165727 MLDockKit-0.0.4/MLDockKit.egg-info/
--rw-r--r--   0 clabe     (1000) clabe     (1000)     4751 2024-01-22 19:59:44.000000 MLDockKit-0.0.4/MLDockKit.egg-info/PKG-INFO
--rw-rw-r--   0 clabe     (1000) clabe     (1000)      285 2024-01-22 19:59:44.000000 MLDockKit-0.0.4/MLDockKit.egg-info/SOURCES.txt
--rw-rw-r--   0 clabe     (1000) clabe     (1000)        1 2024-01-22 19:59:44.000000 MLDockKit-0.0.4/MLDockKit.egg-info/dependency_links.txt
--rw-rw-r--   0 clabe     (1000) clabe     (1000)       66 2024-01-22 19:59:44.000000 MLDockKit-0.0.4/MLDockKit.egg-info/requires.txt
--rw-rw-r--   0 clabe     (1000) clabe     (1000)       10 2024-01-22 19:59:44.000000 MLDockKit-0.0.4/MLDockKit.egg-info/top_level.txt
--rw-r--r--   0 clabe     (1000) clabe     (1000)     4751 2024-01-22 19:59:44.165727 MLDockKit-0.0.4/PKG-INFO
--rw-rw-r--   0 clabe     (1000) clabe     (1000)     3748 2024-01-22 19:37:12.000000 MLDockKit-0.0.4/README.md
--rw-rw-r--   0 clabe     (1000) clabe     (1000)       38 2024-01-22 19:59:44.165727 MLDockKit-0.0.4/setup.cfg
--rw-rw-r--   0 clabe     (1000) clabe     (1000)     1396 2024-01-22 19:36:20.000000 MLDockKit-0.0.4/setup.py
+drwxrwxr-x   0 clabe     (1000) clabe     (1000)        0 2024-04-03 09:14:56.437784 MLDockKit-0.0.5/
+-rw-rw-r--   0 clabe     (1000) clabe     (1000)     1142 2024-01-22 19:28:47.000000 MLDockKit-0.0.5/LICENSE
+drwxrwxr-x   0 clabe     (1000) clabe     (1000)        0 2024-04-03 09:14:56.425786 MLDockKit-0.0.5/MLDockKit/
+-rw-rw-r--   0 clabe     (1000) clabe     (1000)   181468 2024-01-22 19:28:47.000000 MLDockKit-0.0.5/MLDockKit/5gs4.pdbqt
+-rw-rw-r--   0 clabe     (1000) clabe     (1000)    11483 2024-04-03 09:14:40.000000 MLDockKit-0.0.5/MLDockKit/MLDockKit.py
+-rw-rw-r--   0 clabe     (1000) clabe     (1000)       48 2024-04-03 06:58:15.000000 MLDockKit-0.0.5/MLDockKit/__init__.py
+-rw-rw-r--   0 clabe     (1000) clabe     (1000) 18848673 2024-01-22 19:28:48.000000 MLDockKit-0.0.5/MLDockKit/padel_model.joblib
+drwxrwxr-x   0 clabe     (1000) clabe     (1000)        0 2024-04-03 09:14:56.433785 MLDockKit-0.0.5/MLDockKit.egg-info/
+-rw-r--r--   0 clabe     (1000) clabe     (1000)     4373 2024-04-03 09:14:56.000000 MLDockKit-0.0.5/MLDockKit.egg-info/PKG-INFO
+-rw-rw-r--   0 clabe     (1000) clabe     (1000)      285 2024-04-03 09:14:56.000000 MLDockKit-0.0.5/MLDockKit.egg-info/SOURCES.txt
+-rw-rw-r--   0 clabe     (1000) clabe     (1000)        1 2024-04-03 09:14:56.000000 MLDockKit-0.0.5/MLDockKit.egg-info/dependency_links.txt
+-rw-rw-r--   0 clabe     (1000) clabe     (1000)       71 2024-04-03 09:14:56.000000 MLDockKit-0.0.5/MLDockKit.egg-info/requires.txt
+-rw-rw-r--   0 clabe     (1000) clabe     (1000)       10 2024-04-03 09:14:56.000000 MLDockKit-0.0.5/MLDockKit.egg-info/top_level.txt
+-rw-r--r--   0 clabe     (1000) clabe     (1000)     4373 2024-04-03 09:14:56.433785 MLDockKit-0.0.5/PKG-INFO
+-rw-rw-r--   0 clabe     (1000) clabe     (1000)     3350 2024-04-02 18:07:18.000000 MLDockKit-0.0.5/README.md
+-rw-rw-r--   0 clabe     (1000) clabe     (1000)       38 2024-04-03 09:14:56.437784 MLDockKit-0.0.5/setup.cfg
+-rw-rw-r--   0 clabe     (1000) clabe     (1000)     1404 2024-04-03 07:12:46.000000 MLDockKit-0.0.5/setup.py
```

### Comparing `MLDockKit-0.0.4/LICENSE` & `MLDockKit-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `MLDockKit-0.0.4/MLDockKit/5gs4.pdbqt` & `MLDockKit-0.0.5/MLDockKit/5gs4.pdbqt`

 * *Files identical despite different names*

### Comparing `MLDockKit-0.0.4/MLDockKit/MLDockKit.py` & `MLDockKit-0.0.5/MLDockKit/MLDockKit.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,14 +15,28 @@
 import os
 import subprocess
 
 
 # constants
 docking_protein = "5gs4.pdbqt"
 prediction_model = "padel_model.joblib"
+current_directory = os.getcwd()
+file_paths = ["ligand_clean.sdf", "ligand.pdbqt"]
+
+def delete_files_with_extension(directory, extensions):
+    """
+    Delete files with specified extensions in a directory.
+    """
+    for file in os.listdir(directory):
+        if any(file.endswith(ext) for ext in extensions):
+            os.remove(os.path.join(directory, file))
+
+# Delete files in the working directory
+current_directory = os.getcwd()
+delete_files_with_extension(current_directory, [".sdf", ".pdbqt"])            
 
 
 def getbox(selection="sele", extending=6.0, software="vina"):
     ([minX, minY, minZ], [maxX, maxY, maxZ]) = cmd.get_extent(selection)
 
     minX = minX - float(extending)
     minY = minY - float(extending)
@@ -96,23 +110,19 @@
             "Num H Donors": "Number Hydrogen Bond Donors",
             "Num H Acceptors": "Number of Hydrogen Bond Acceptors",
             "Num Rotatable Bonds": "Number of Rotatable Bonds",
             "Carbon Count": "Carbon Count",
             "Oxygen Count": "Oxygen Count",
         }
 
-        df = pd.DataFrame(
-            {
-                "Descriptor": list(descriptors.keys()),
-                "Value": list(descriptors.values()),
-            }
-        )
-        df["Descriptor"] = df["Descriptor"].map(aliases)
+        formatted_descriptors = ""
+        for key, value in descriptors.items():
+            formatted_descriptors += f"{aliases[key]}: {value}\n"
 
-        return df
+        return formatted_descriptors
 
 
 def predict_pIC50(smiles):
     """Prediction model is based on RandomForest regression constructed using a collection of all known cannonical SMILES that interact with Oestrogen Receptor alpha protein stored in the ChEMBL database.
 
     Params
     ------
@@ -158,15 +168,15 @@
 
     # Specify the path to the "padel_model.joblib" file
     prediction_model = os.path.join(script_dir, "padel_model.joblib")
     loaded_model = joblib.load(prediction_model)
     y_pred = loaded_model.predict(X)
     predicted_value = y_pred[0]
     predicted_value = format(predicted_value, ".2f")
-    return f"The pIC50 of your compound is {predicted_value}"
+    return f"Predicted pIC50: {predicted_value}"
 
 
 def prot_lig_docking(smiles):
     """Docking procedure is performed by Autodock Vina on the Oestrogen Receptor alpha protein, pdb_id: 5gs4 prepared for docking by the Angel Moreno's Jupyter_Dock scripts.
 
     Params
     ------
@@ -180,25 +190,26 @@
 
     prot_lig_docking("Oc1ccc2c(c1)S[C@H](c1ccco1)[C@H](c1ccc(OCCN3CCCCC3)cc1)O2")
     """
 
     # Get the directory of the currently executing script
 
     script_dir = os.path.dirname(__file__)
+    current_directory = os.getcwd()
 
     mol = Chem.MolFromSmiles(smiles)
     if mol is None:
         raise ValueError("You entered an invalid SMILES string")
 
     # Convert SMILES to molecule object
     mol = Chem.AddHs(mol)
     AllChem.EmbedMolecule(mol, randomSeed=42)
 
     # Write the molecule to an SDF file
-    sdf_file = os.path.join(script_dir, "ligand_clean.sdf")
+    sdf_file = os.path.join(current_directory, "ligand_clean.sdf")
     writer = SDWriter(sdf_file)
     writer.write(mol)
     writer.close()
 
     # Prepare the ligand
     mol_supplier = SDMolSupplier(sdf_file, removeHs=False)
     preparator = MoleculePreparation()
@@ -206,15 +217,15 @@
     for mol in mol_supplier:
         mol_setups = preparator.prepare(mol)
         for setup in mol_setups:
             pdbqt_tuple = PDBQTWriterLegacy.write_string(setup)
             pdbqt_string = pdbqt_tuple[0]
 
             # Save pdbqt_string to the ligand.pdbqt file
-            pdbqt_file = os.path.join(script_dir, "ligand.pdbqt")
+            pdbqt_file = os.path.join(current_directory, "ligand.pdbqt")
             with open(pdbqt_file, "w") as pdbqt_file:
                 pdbqt_file.write(pdbqt_string)
 
     docking_protein = os.path.join(
         script_dir, "5gs4.pdbqt"
     )  # Replace with the actual path
     cmd.load(filename=docking_protein, format="pdb", object="prot")
@@ -227,28 +238,28 @@
     v.set_ligand_from_file(pdbqt_file.name)
     v.compute_vina_maps(
         center=[center["center_x"], center["center_y"], center["center_z"]],
         box_size=[size["size_x"], size["size_y"], size["size_z"]],
     )
 
     v.dock(exhaustiveness=10, n_poses=10)
-    vina_out_file = os.path.join(script_dir, "5gs4_ligand_vina_out.pdbqt")
-    sdf_file = os.path.join(script_dir, "5gs4_ligand_vina_out.sdf")
+    vina_out_file = os.path.join(current_directory, "5gs4_ligand_vina_out.pdbqt")
+    sdf_file = os.path.join(current_directory, "5gs4_ligand_vina_out.sdf")
     v.write_poses(vina_out_file, n_poses=10, overwrite=True)
     pdbqt_to_sdf(
         pdbqt_file=vina_out_file,
-        output=os.path.join(script_dir, "5gs4_ligand_vina_out.sdf"),
+        output=os.path.join(current_directory, "5gs4_ligand_vina_out.sdf"),
     )
 
     results = Chem.SDMolSupplier(sdf_file)
 
     p = Chem.MolToMolBlock(results[0], False)
 
     if results:
-        return "Best docking score: {}".format(results[0].GetProp("Score"))
+        return "Docking score: {}".format(results[0].GetProp("Score"))
     else:
         return "No results available"
 
 
 # Run PyMOL with the specified PDBQT files
 def vizualize_dock_results():
     """Visualization and protein-ligand interaction in pymol. Users should only run this function after running prot_lig_docking function.
@@ -256,10 +267,77 @@
     Usage
     -----
     from MLDockKit import vizualize_dock_results
 
     vizualize_dock_results()
     """
     script_dir = os.path.dirname(__file__)
+    current_directory = os.getcwd()
     docking_protein = os.path.join(script_dir, "5gs4.pdbqt")
-    vina_out_file = os.path.join(script_dir, "5gs4_ligand_vina_out.pdbqt")
-    return subprocess.run(["pymol", docking_protein, vina_out_file])
+    vina_out_file = os.path.join(current_directory, "5gs4_ligand_vina_out.pdbqt")
+    return subprocess.run(["pymol", "-Q", docking_protein, vina_out_file])
+
+
+def MLDockKit(smiles, output_file="MLDockKit_output.txt"):
+    """
+    Perform the entire molecular modeling pipeline:
+    1. Calculate Lipinski descriptors
+    2. Predict pIC50
+    3. Perform protein-ligand docking
+    4. Visualize docking results
+
+    Params:
+    smiles (str): An rdkit valid canonical SMILES or chemical structure of a compound.
+    output_file (str): File path to save the output.
+
+    Returns:
+    str: Summary of the pipeline execution.
+    """
+    try:
+        with open(output_file, "w") as f:
+            f.write("." * 200 + "\n")
+            # Calculate Lipinski descriptors
+            lipinski_descriptors = calculate_lipinski_descriptors(smiles)
+            f.write("Lipinski Descriptors"+ "\n")
+            f.write(str(lipinski_descriptors))
+            f.write("\n" + "." * 200 + "\n")
+            print("\n" +'###Computation of Lipinsky descriptors complete'+"\n")
+            
+            # Predict pIC50
+            pIC50_prediction = predict_pIC50(smiles)
+            f.write(pIC50_prediction + "\n")
+            f.write("\n" + "." * 200 + "\n")
+            print('###Prediction of pIC50 complete'+"\n")
+
+            # Perform protein-ligand docking
+            docking_result = prot_lig_docking(smiles)
+            #f.write("\n")
+            f.write(docking_result + "\n")
+            f.write("\n" + "." * 200 + "\n")
+            print("\n" + '###Docking process complete'+"\n")
+            print("##MLDockKit output is saved to " + output_file + "and image rentered in pymol"+"\n")
+            #f.write("\n"+"\n")
+
+            # Delete files in the script directory
+            script_dir = os.path.dirname(__file__)
+            delete_files_with_extension(script_dir, [".smi", ".csv"])
+            # Delete files in the working directory
+        
+
+        # Iterate over files in the directory
+        for file in os.listdir(current_directory):
+            if file in file_paths:
+                file_path = os.path.join(current_directory, file)  # Get the full path
+                os.remove(file_path)    
+
+
+        # Visualize docking results
+        vizualize_dock_results()
+
+    except Exception as e:
+        return f"Error occurred: {str(e)}"
+
+
+
+
+
+
```

### Comparing `MLDockKit-0.0.4/MLDockKit/padel_model.joblib` & `MLDockKit-0.0.5/MLDockKit/padel_model.joblib`

 * *Files identical despite different names*

### Comparing `MLDockKit-0.0.4/MLDockKit.egg-info/PKG-INFO` & `MLDockKit-0.0.5/MLDockKit.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MLDockKit
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python package that calculates Lipinsky descriptors, predicts pIC50 and performs docking
 Home-page: https://github.com/clabe-wekesa/MLDockKit
 Author: Edwin Mwakio, Clabe Wekesa, Patrick okoth
 Author-email: simiyu86wekesa@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -21,14 +21,15 @@
 Requires-Dist: pandas
 Requires-Dist: padelpy
 Requires-Dist: joblib
 Requires-Dist: meeko
 Requires-Dist: scikit-learn==1.3.0
 Requires-Dist: scipy
 Requires-Dist: numpy
+Requires-Dist: vina
 
 # MLDockKit
 This is a simple platform for computing Lipinsky's Rule of five using the rdkit package, predicting pIC50 of canonical SMILES that are potential targets against Oestrogen receptor alpha protein as ant-prostate cancer agaents using a preformatted RandomForest model, and docking of the canonical SMILE with the Oestrogen receptor alpha protein using Audodock Vina package. 
 ### Purpose of the Package
 The purpose of the package is to provide a unified platform for computing prostate cancer drug likeness indicess and performing docking on the same compounds. 
 ### Features
 Important chemoinformatics features of Oestrogen receptor alpha antagonists such as:
@@ -54,38 +55,24 @@
 conda install -c cyclus java-jre
 
 pip install -U numpy vina
 
 pip install MLDockKit
 ```
 
-### Usage
-#### Computating Lipinsky descriptors
-```python
->>>from MLDockKit import calculate_lipinski_descriptors
->>>calculate_lipinski_descriptors("Oc1ccc2c(c1)S[C@H](c1ccco1)[C@H](c1ccc(OCCN3CCCCC3)cc1)O2")
-```
-#### Predictioning pIC50
-```python
->>>from MLDockKit import predict_pIC50
->>>predict_pIC50("Oc1ccc2c(c1)S[C@H](c1ccco1)[C@H](c1ccc(OCCN3CCCCC3)cc1)O2")
-```
-#### Docking with protein, pdb_id 5gs4
-```python
->>>from MLDockKit import prot_lig_docking
->>>prot_lig_docking("Oc1ccc2c(c1)S[C@H](c1ccco1)[C@H](c1ccc(OCCN3CCCCC3)cc1)O2")
-```
-#### Visualization of docking results
-This opens pymol for visulization and analysis. If you need help on pymol analysis please have a look on [pymol documentation](https://fitzkee.chemistry.msstate.edu/sites/default/files/ch8990/pymol-tutorial.pdf)
+### Run MLDockKit pipeline
 
 ```python
->>>from MLDockKit import vizualize_dock_results
->>>vizualize_dock_results()
+>>>from MLDockKit import MLDockKit
+>>>MLDockKit("Oc1ccc2c(c1)S[C@H](c1ccco1)[C@H](c1ccc(OCCN3CCCCC3)cc1)O2")
 ```
 
+### Output
+The pipeline's output is an MLDockKit_output.txt file which contains **Lipinsky descriptos**, **predicted pIC50 value** and the **docking score**. Docking image is rentered in pymol for further analysis by the user. Also, the ligand's and protein's **.sfd** and **.pdpqt** files are rentered in the user's working directory.
+
 ### Acknowledgment
 Autodock Vina and pymol were greatily used in writing the codes for molecular docking and visualization. If you use these functions in your work, please cite the original publications for [vina](https://pubs.acs.org/doi/10.1021/acs.jcim.1c00203) and [pymol](https://citeseerx.ist.psu.edu/document?repid=rep1&type=pdf&doi=ab82608e9a44c17b60d7f908565fba628295dc72#page=44)
 
 We extracted part of Angel Ruiz Moreno's Jupyter_Dock [Jupyter Dock](https://github.com/AngelRuizMoreno/Jupyter_Dock) to include it in our visualization function. 
 
 ### Contribution
 We welcome any contributions. Should you notice a bug, please let us know through issues in the, [GitHub Issue Tracker](https://github.com/clabe-wekesa/MLDockKit/issues)
```

### Comparing `MLDockKit-0.0.4/PKG-INFO` & `MLDockKit-0.0.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MLDockKit
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python package that calculates Lipinsky descriptors, predicts pIC50 and performs docking
 Home-page: https://github.com/clabe-wekesa/MLDockKit
 Author: Edwin Mwakio, Clabe Wekesa, Patrick okoth
 Author-email: simiyu86wekesa@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -21,14 +21,15 @@
 Requires-Dist: pandas
 Requires-Dist: padelpy
 Requires-Dist: joblib
 Requires-Dist: meeko
 Requires-Dist: scikit-learn==1.3.0
 Requires-Dist: scipy
 Requires-Dist: numpy
+Requires-Dist: vina
 
 # MLDockKit
 This is a simple platform for computing Lipinsky's Rule of five using the rdkit package, predicting pIC50 of canonical SMILES that are potential targets against Oestrogen receptor alpha protein as ant-prostate cancer agaents using a preformatted RandomForest model, and docking of the canonical SMILE with the Oestrogen receptor alpha protein using Audodock Vina package. 
 ### Purpose of the Package
 The purpose of the package is to provide a unified platform for computing prostate cancer drug likeness indicess and performing docking on the same compounds. 
 ### Features
 Important chemoinformatics features of Oestrogen receptor alpha antagonists such as:
@@ -54,38 +55,24 @@
 conda install -c cyclus java-jre
 
 pip install -U numpy vina
 
 pip install MLDockKit
 ```
 
-### Usage
-#### Computating Lipinsky descriptors
-```python
->>>from MLDockKit import calculate_lipinski_descriptors
->>>calculate_lipinski_descriptors("Oc1ccc2c(c1)S[C@H](c1ccco1)[C@H](c1ccc(OCCN3CCCCC3)cc1)O2")
-```
-#### Predictioning pIC50
-```python
->>>from MLDockKit import predict_pIC50
->>>predict_pIC50("Oc1ccc2c(c1)S[C@H](c1ccco1)[C@H](c1ccc(OCCN3CCCCC3)cc1)O2")
-```
-#### Docking with protein, pdb_id 5gs4
-```python
->>>from MLDockKit import prot_lig_docking
->>>prot_lig_docking("Oc1ccc2c(c1)S[C@H](c1ccco1)[C@H](c1ccc(OCCN3CCCCC3)cc1)O2")
-```
-#### Visualization of docking results
-This opens pymol for visulization and analysis. If you need help on pymol analysis please have a look on [pymol documentation](https://fitzkee.chemistry.msstate.edu/sites/default/files/ch8990/pymol-tutorial.pdf)
+### Run MLDockKit pipeline
 
 ```python
->>>from MLDockKit import vizualize_dock_results
->>>vizualize_dock_results()
+>>>from MLDockKit import MLDockKit
+>>>MLDockKit("Oc1ccc2c(c1)S[C@H](c1ccco1)[C@H](c1ccc(OCCN3CCCCC3)cc1)O2")
 ```
 
+### Output
+The pipeline's output is an MLDockKit_output.txt file which contains **Lipinsky descriptos**, **predicted pIC50 value** and the **docking score**. Docking image is rentered in pymol for further analysis by the user. Also, the ligand's and protein's **.sfd** and **.pdpqt** files are rentered in the user's working directory.
+
 ### Acknowledgment
 Autodock Vina and pymol were greatily used in writing the codes for molecular docking and visualization. If you use these functions in your work, please cite the original publications for [vina](https://pubs.acs.org/doi/10.1021/acs.jcim.1c00203) and [pymol](https://citeseerx.ist.psu.edu/document?repid=rep1&type=pdf&doi=ab82608e9a44c17b60d7f908565fba628295dc72#page=44)
 
 We extracted part of Angel Ruiz Moreno's Jupyter_Dock [Jupyter Dock](https://github.com/AngelRuizMoreno/Jupyter_Dock) to include it in our visualization function. 
 
 ### Contribution
 We welcome any contributions. Should you notice a bug, please let us know through issues in the, [GitHub Issue Tracker](https://github.com/clabe-wekesa/MLDockKit/issues)
```

### Comparing `MLDockKit-0.0.4/README.md` & `MLDockKit-0.0.5/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -26,38 +26,24 @@
 conda install -c cyclus java-jre
 
 pip install -U numpy vina
 
 pip install MLDockKit
 ```
 
-### Usage
-#### Computating Lipinsky descriptors
-```python
->>>from MLDockKit import calculate_lipinski_descriptors
->>>calculate_lipinski_descriptors("Oc1ccc2c(c1)S[C@H](c1ccco1)[C@H](c1ccc(OCCN3CCCCC3)cc1)O2")
-```
-#### Predictioning pIC50
-```python
->>>from MLDockKit import predict_pIC50
->>>predict_pIC50("Oc1ccc2c(c1)S[C@H](c1ccco1)[C@H](c1ccc(OCCN3CCCCC3)cc1)O2")
-```
-#### Docking with protein, pdb_id 5gs4
-```python
->>>from MLDockKit import prot_lig_docking
->>>prot_lig_docking("Oc1ccc2c(c1)S[C@H](c1ccco1)[C@H](c1ccc(OCCN3CCCCC3)cc1)O2")
-```
-#### Visualization of docking results
-This opens pymol for visulization and analysis. If you need help on pymol analysis please have a look on [pymol documentation](https://fitzkee.chemistry.msstate.edu/sites/default/files/ch8990/pymol-tutorial.pdf)
+### Run MLDockKit pipeline
 
 ```python
->>>from MLDockKit import vizualize_dock_results
->>>vizualize_dock_results()
+>>>from MLDockKit import MLDockKit
+>>>MLDockKit("Oc1ccc2c(c1)S[C@H](c1ccco1)[C@H](c1ccc(OCCN3CCCCC3)cc1)O2")
 ```
 
+### Output
+The pipeline's output is an MLDockKit_output.txt file which contains **Lipinsky descriptos**, **predicted pIC50 value** and the **docking score**. Docking image is rentered in pymol for further analysis by the user. Also, the ligand's and protein's **.sfd** and **.pdpqt** files are rentered in the user's working directory.
+
 ### Acknowledgment
 Autodock Vina and pymol were greatily used in writing the codes for molecular docking and visualization. If you use these functions in your work, please cite the original publications for [vina](https://pubs.acs.org/doi/10.1021/acs.jcim.1c00203) and [pymol](https://citeseerx.ist.psu.edu/document?repid=rep1&type=pdf&doi=ab82608e9a44c17b60d7f908565fba628295dc72#page=44)
 
 We extracted part of Angel Ruiz Moreno's Jupyter_Dock [Jupyter Dock](https://github.com/AngelRuizMoreno/Jupyter_Dock) to include it in our visualization function. 
 
 ### Contribution
 We welcome any contributions. Should you notice a bug, please let us know through issues in the, [GitHub Issue Tracker](https://github.com/clabe-wekesa/MLDockKit/issues)
```

### Comparing `MLDockKit-0.0.4/setup.py` & `MLDockKit-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 
 # Read README for long description
 with open('README.md', 'r', encoding='utf-8') as readme_file:
 	LONG_DESCRIPTION = readme_file.read()
 
 setuptools.setup(
     name="MLDockKit",
-    version="0.0.4",
+    version="0.0.5",
     include_package_data=True,
     description='Python package that calculates Lipinsky descriptors, predicts pIC50 and performs docking',
     url = "https://github.com/clabe-wekesa/MLDockKit",
     license = "MIT",
     packages=setuptools.find_packages(),
     install_requires=[
         # List your Python dependencies here
-        'rdkit', 'pandas', 'padelpy', 'joblib', 'meeko', 'scikit-learn==1.3.0', 'scipy', 'numpy'
+        'rdkit', 'pandas', 'padelpy', 'joblib', 'meeko', 'scikit-learn==1.3.0', 'scipy', 'numpy', 'vina'
     ],
     author='Edwin Mwakio, Clabe Wekesa, Patrick okoth',
     author_email='simiyu86wekesa@gmail.com',  
     package_data={
         # Include your non-Python files here
         'MLDockKit': ['padel_model.joblib', '5gs4.pdbqt'],
     },
```

