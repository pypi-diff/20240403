# Comparing `tmp/weas-widget-0.0.9.tar.gz` & `tmp/weas_widget-0.1.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weas-widget-0.0.9.tar", last modified: Sat Feb 24 19:47:03 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `weas-widget-0.0.9.tar` & `weas_widget-0.1.0a0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-02-24 19:47:03.564230 weas-widget-0.0.9/
--rw-r--r--   0 xing      (1000) xing      (1000)     5145 2024-02-24 19:47:03.564230 weas-widget-0.0.9/PKG-INFO
--rw-rw-r--   0 xing      (1000) xing      (1000)     4408 2024-02-23 16:37:50.000000 weas-widget-0.0.9/README.md
--rw-rw-r--   0 xing      (1000) xing      (1000)       38 2024-02-24 19:47:03.564230 weas-widget-0.0.9/setup.cfg
--rw-rw-r--   0 xing      (1000) xing      (1000)     1120 2024-02-24 19:45:54.000000 weas-widget-0.0.9/setup.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-02-24 19:47:03.564230 weas-widget-0.0.9/weas_widget/
--rw-rw-r--   0 xing      (1000) xing      (1000)     4257 2024-02-24 19:46:45.000000 weas-widget-0.0.9/weas_widget/__init__.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-02-24 19:47:03.564230 weas-widget-0.0.9/weas_widget/datas/
--rw-rw-r--   0 xing      (1000) xing      (1000)        0 2024-02-13 14:30:48.000000 weas-widget-0.0.9/weas_widget/datas/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)      878 2024-01-31 13:14:49.000000 weas-widget-0.0.9/weas_widget/datas/tio2.cif
--rw-rw-r--   0 xing      (1000) xing      (1000)     6048 2024-02-24 19:46:45.000000 weas-widget-0.0.9/weas_widget/index.js
--rw-rw-r--   0 xing      (1000) xing      (1000)      517 2024-02-22 22:38:17.000000 weas-widget-0.0.9/weas_widget/style.css
--rw-rw-r--   0 xing      (1000) xing      (1000)     4525 2024-02-22 22:38:17.000000 weas-widget-0.0.9/weas_widget/utils.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-02-24 19:47:03.564230 weas-widget-0.0.9/weas_widget.egg-info/
--rw-r--r--   0 xing      (1000) xing      (1000)     5145 2024-02-24 19:47:03.000000 weas-widget-0.0.9/weas_widget.egg-info/PKG-INFO
--rw-rw-r--   0 xing      (1000) xing      (1000)      337 2024-02-24 19:47:03.000000 weas-widget-0.0.9/weas_widget.egg-info/SOURCES.txt
--rw-rw-r--   0 xing      (1000) xing      (1000)        1 2024-02-24 19:47:03.000000 weas-widget-0.0.9/weas_widget.egg-info/dependency_links.txt
--rw-rw-r--   0 xing      (1000) xing      (1000)       21 2024-02-24 19:47:03.000000 weas-widget-0.0.9/weas_widget.egg-info/requires.txt
--rw-rw-r--   0 xing      (1000) xing      (1000)       12 2024-02-24 19:47:03.000000 weas-widget-0.0.9/weas_widget.egg-info/top_level.txt
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 weas_widget-0.1.0a0/src/weas_widget/__init__.py
+-rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 weas_widget-0.1.0a0/src/weas_widget/atoms_viewer.py
+-rw-r--r--   0        0        0     3713 2020-02-02 00:00:00.000000 weas_widget-0.1.0a0/src/weas_widget/base_class.py
+-rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 weas_widget-0.1.0a0/src/weas_widget/base_widget.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 weas_widget-0.1.0a0/src/weas_widget/camera.py
+-rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 weas_widget-0.1.0a0/src/weas_widget/data.py
+-rw-r--r--   0        0        0     5111 2020-02-02 00:00:00.000000 weas_widget-0.1.0a0/src/weas_widget/utils.py
+-rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 weas_widget-0.1.0a0/src/weas_widget/weas.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 weas_widget-0.1.0a0/src/weas_widget/plugins/__init__.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 weas_widget-0.1.0a0/src/weas_widget/plugins/instanced_mesh_pritimive.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 weas_widget-0.1.0a0/src/weas_widget/plugins/isosurface.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 weas_widget-0.1.0a0/src/weas_widget/plugins/vector_field.py
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 weas_widget-0.1.0a0/src/weas_widget/static/widget.css
+-rw-r--r--   0        0        0   698930 2020-02-02 00:00:00.000000 weas_widget-0.1.0a0/src/weas_widget/static/widget.js
+-rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 weas_widget-0.1.0a0/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 weas_widget-0.1.0a0/LICENSE
+-rw-r--r--   0        0        0     5099 2020-02-02 00:00:00.000000 weas_widget-0.1.0a0/README.md
+-rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 weas_widget-0.1.0a0/pyproject.toml
+-rw-r--r--   0        0        0     8080 2020-02-02 00:00:00.000000 weas_widget-0.1.0a0/PKG-INFO
```

### Comparing `weas-widget-0.0.9/PKG-INFO` & `weas_widget-0.1.0a0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,194 +1,224 @@
-Metadata-Version: 2.1
-Name: weas-widget
-Version: 0.0.9
-Summary: A widget to visualize and interact with atomistic structures in Jupyter Notebook.
-Home-page: https://github.com/superstar54/weas-widget
-Author: Xing Wang
-Author-email: xingwang1991@gmail.com
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Description-Content-Type: text/markdown
-Requires-Dist: anywidget
-Requires-Dist: ipywidgets
-
 
 # Welcome to WEAS Widget!
 [![PyPI version](https://badge.fury.io/py/weas-widget.svg)](https://badge.fury.io/py/weas-widget)
 [![Docs status](https://readthedocs.org/projects/weas-widget/badge)](http://weas-widget.readthedocs.io/)
+[![Unit test](https://github.com/superstar54/weas-widget/actions/workflows/ci.yml/badge.svg)](https://github.com/superstar54/weas-widget/actions/workflows/ci.yml)
 
-
-A widget to visualize and edit atomistic structures in Jupyter Notebook. It uses [WEAS](https://github.com/superstar54/weas) (Web Environment For Atomistic Structure) in the backend.
+A widget to visualize and edit atomic structures in Jupyter Notebooks. It uses [WEAS](https://github.com/superstar54/weas) (Web Environment For Atomistic Structure) in the backend.
 
 
 <img src="docs/source/_static/images/example-adsorption.gif"  width="100%"/>
 
 
 Features:
 
 - Model: space-filling, ball-stick, polyhedral.
-- Supported File type: cif, xyz.
+- Supports importing data from ASE and Pymatgen.
 - Edit structure: move, rotate, delete and replace atoms.
-- Support periodic boundary conditions
-- Animation
-- Isosurface
-- Vector field, e.g., magnetic moment
+- Supports periodic boundary conditions
+- Animations
+- Isosurfaces
+- Vector fields, e.g., magnetic moments, phonons, ...
 
 
 ## Installation
 
-Use the pip:
+With `pip`:
+
+```console
+pip install weas-widget
+```
+
+To install the latest version from source, first clone the repository and then install using `pip`:
 
 ```console
-    pip install weas-widget
+git clone https://github.com/superstar54/weas-widget
+cd weas-widget
+npm install
+npm run build
+pip install -e .
+```
+
+## How to use
+
+```python
+from ase.build import molecule
+from weas_widget import WeasWidget
+atoms = molecule("C2H6SO")
+viewer = WeasWidget()
+viewer.from_ase(atoms)
+viewer
 ```
 
-To install the latest version from source, first clone the repository and then install using pip:
+<img src="docs/source/_static/images/example-c2h6so.png"  width="300px"/>
+
+
+Full documentation at: https://weas-widget.readthedocs.io/en/latest/index.html
+
+
+## Reporting issues
+If you encounter any problems, please first update the widget to the latest version.
 
 ```console
-    $ git clone https://github.com/superstar54/weas-widget
-    $ pip install -e weas-widget
+    pip install weas-widget  --upgrade
 ```
 
+If the problem persists, please open a [GitHub issue](https://github.com/superstar54/weas-widget/issues)
+
+
+## Features
 
-## Edit the structure with mouse and keyboard
-WEAS supports editing the atoms directly in the GUI and synchronizing with the structure of the Python object.
 
 ### Select Atoms
-There are two methods for selecting atoms:
 - Pick Selection: Click directly on an atom to select it.
 - Range Selection: Hold the `Shift` key and drag the right mouse button to select a group of atoms.
 
-
-
 ### Move, Rotate selected atoms
 
-Press the transform shortcut, and move your mouse.
+Press the keyboard shortcut, and move your mouse.
 
 |Operation | Shortcut|
 |----------|---------|
 | Move     | `g`   |
 | Rotate   | `r`   |
+| Duplicate| `d`   |
 
 
 ### Delete selected atoms
-Press the ``x`` key to delete the selected atoms
-
-
-### Export edited atoms
-One can export the edited atoms to ASE or Pymatgen
+Press the ``Delete`` key
 
-## Example
-
-### Load structure
-One can load a structure from ASE or Pymatgen
 
+### Export
+- Export the modified atomic structure to ASE or Pymatgen
 ```python
-from ase.build import molecule
-from weas_widget import WeasWidget
-atoms = molecule("C2H6SO")
-viewer = WeasWidget()
-viewer.from_ase(atoms)
-viewer
+atoms = viewer.to_ase()
+```
+- Save image to a path by:
+```python
+viewer.save_image("/home/xing/filename.png")
+```
+- Download image by:
+```python
+viewer.download_image("filename.png")
 ```
 
-<img src="docs/source/_static/images/example-c2h6so.png"  width="300px"/>
-
-
-
-### Crystal view
-For a nice visualization of a crystal, one usually shows the polyhedra and the atoms on the unit cell boundary, as well as the bonded atoms outside the cell.
+### Visualizing crystal structures
+For a nice visualization of a crystal, show
+- unit cell
+- bonded atoms outside the cell
+- polyhedra
 
 ```python
 from weas_widget import WeasWidget
 viewer1 = WeasWidget()
 viewer1.load_example("tio2.cif")
-viewer1.modelStyle = 2
-viewer1.boundary = [[-0.1, 1.1], [-0.1, 1.1], [-0.1, 1.1]]
-viewer1.showBondedAtoms = True
-viewer1.colorType = "VESTA"
+viewer1.avr.model_style = 2
+viewer1.avr.boundary = [[-0.1, 1.1], [-0.1, 1.1], [-0.1, 1.1]]
+viewer1.avr.show_bonded_atoms = True
+viewer1.avr.color_type = "VESTA"
 viewer1
 ```
 
 <img src="docs/source/_static/images/example-tio2.png"  width="300px"/>
 
 
-### Isosurface
+### Isosurfaces
 
 ```python
 from ase.build import molecule
 from weas_widget import WeasWidget
 from ase.io.cube import read_cube_data
 volume, atoms = read_cube_data("h2o-homo.cube")
 viewer = WeasWidget()
 viewer.from_ase(atoms)
-viewer.volumetricData = {"values": volume}
-viewer.isoSettings = [{"isovalue": 0.0001, "mode": 0}]
+viewer.avr.iso.volumetric_data = {"values": volume}
+viewer.avr.iso.settings = [{"isovalue": 0.0001, "mode": 0}]
 viewer
 ```
 <img src="docs/source/_static/images/example-isosurface.png"  width="300px"/>
 
 
-### Magnetic moment
-Show the magnetic moment as a vector field.
+### Magnetic moments
+Show the magnetic moments as a vector field.
 
 ```python
 from ase.build import bulk
 from weas_widget import WeasWidget
 import numpy as np
 atoms = bulk("Fe", cubic=True)
 atoms*=[2, 2, 1]
 atoms.set_array("moment", np.ones(len(atoms)))
 viewer = WeasWidget()
 viewer.from_ase(atoms)
-viewer.modelStyle = 1
+viewer.avr.model_style = 1
 viewer
 ```
 <img src="docs/source/_static/images/example-magnetic-moment.png"  width="300px"/>
 
 
-### Phonon
-One can visualize the phonon dispersion via lattice vibrations. One only need to use the eigenstates (calculated with an external software) to generate the trajectory.
+### Phonons
+Animate vibrational (phonon) modes (computed with external software).
 
 ```python
 import numpy as np
 from ase.build import bulk
 from weas_widget import WeasWidget
 from weas_widget.utils import generate_phonon_trajectory
 
 atoms = bulk("Fe", cubic=True)
 eigenvector = np.array([[0, -0.0, 0.5], [0, 0.0, -0.5]])
 trajectory = generate_phonon_trajectory(atoms, eigenvector, repeat=[4, 4, 1])
 viewer = WeasWidget()
 viewer.from_ase(trajectory)
 # set a vector field to show the arrow
-viewer.vectorField = {"origins": "positions", "vectors": "movement", "radius": 0.1}
+viewer.avr.vf.settings = [{"origins": "positions", "vectors": "movement", "radius": 0.1}]
+viewer.avr.vf.show = True
 viewer
 ```
 
 <img src="docs/source/_static/images/example-phonon.gif"  width="300px"/>
 
 
 
-### Download image
+## Test
 
-```python
-viewer.download_image("filename.png")
+### Unit test
+
+```console
+pytest
 ```
 
-## How to use
+### End-to-end test
+
+The e2e test is similar to [ipywidgets](https://ipywidgets.readthedocs.io/en/latest/dev_testing.html).
+
+For the first time, one needs to install the dependence.
+
+```
+cd tests/notebooks/
+yarn install
+```
 
-Please visit: https://weas-widget.readthedocs.io/en/latest/index.html
+Then run in a terminal:
 
+```
+yarn start
+```
 
+In another terminal:
+
+```
+yarn test
+```
+
+If the snapshots need to be updated:
+
+```
+yarn test:update
+```
 
 ## Contact
 * Xing Wang  <xingwang1991@gmail.com>
 
 ## License
 [MIT](http://opensource.org/licenses/MIT)
```

### Comparing `weas-widget-0.0.9/weas_widget/utils.py` & `weas_widget-0.1.0a0/src/weas_widget/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,43 +19,42 @@
                 return weas_atoms
             else:
                 raise ValueError("The list of atoms is empty")
         species = {}
         cell = ase_atoms.get_cell().array.flatten().tolist()
         positions = ase_atoms.get_positions()
         symbols = ase_atoms.get_chemical_symbols()
-        numbers = ase_atoms.get_atomic_numbers()
-        speciesArray = symbols
         for i in range(len(symbols)):
-            species[symbols[i]] = [symbols[i], numbers[i]]
+            species[symbols[i]] = symbols[i]
         # save other arrays to attributes
         attributes = {"atom": {}, "species": {}}
         for key in ase_atoms.arrays.keys():
             if key not in ["positions", "numbers"]:
                 attributes["atom"][key] = ase_atoms.arrays[key]
 
         weas_atoms = {
             "species": species,
             "cell": cell,
             "positions": positions,
-            "speciesArray": speciesArray,
+            "symbols": symbols,
             "attributes": attributes,
         }
         return weas_atoms
 
     @classmethod
     def to_ase(cls, weas_atoms):
         # Convert the widget's format to an ASE Atoms object
         from ase import Atoms
         import numpy as np
 
         # if atoms is a list of atoms, convert all atoms to a list of ase atoms
         if isinstance(weas_atoms, list):
-            return [cls.to_ase(atom) for atom in weas_atoms]
-        symbols = [weas_atoms["species"][s][0] for s in weas_atoms["speciesArray"]]
+            trajectory = [cls.to_ase(atom) for atom in weas_atoms]
+            return trajectory[0] if len(trajectory) == 1 else trajectory
+        symbols = [weas_atoms["species"][s] for s in weas_atoms["symbols"]]
         positions = weas_atoms["positions"]
         cell = np.array(weas_atoms["cell"]).reshape(3, 3)
         ase_atoms = Atoms(symbols=symbols, positions=positions, cell=cell)
         return ase_atoms
 
 
 class Pymatgen_Adapter:
@@ -65,35 +64,34 @@
     @classmethod
     def to_weas(cls, pymatgen_structure):
         # Convert a Pymatgen Structure object to the widget's format
         species = {}
         cell = pymatgen_structure.lattice.matrix.flatten().tolist()
         positions = [site.coords for site in pymatgen_structure.sites]
         symbols = [site.species_string for site in pymatgen_structure.sites]
-        speciesArray = symbols
         for i in range(len(symbols)):
-            species[symbols[i]] = [symbols[i]]
+            species[symbols[i]] = symbols[i]
         weas_atoms = {
             "species": species,
             "cell": cell,
             "positions": positions,
-            "speciesArray": speciesArray,
+            "symbols": symbols,
         }
         return weas_atoms
 
     @classmethod
     def to_pymatgen(cls, weas_atoms):
         # Convert the widget's format to a Pymatgen Structure object
         from pymatgen.core import Structure, Lattice
 
         if isinstance(weas_atoms, list):
             return [cls.to_pymatgen(atom) for atom in weas_atoms]
 
         lattice = Lattice(weas_atoms["cell"])
-        species = weas_atoms["speciesArray"]
+        species = weas_atoms["symbols"]
         sites = weas_atoms["positions"]
         structure = Structure(lattice, species, sites)
         return structure
 
 
 def generate_phonon_trajectory(
     atoms,
@@ -122,7 +120,26 @@
         # new atoms
         new_atoms = atoms.copy()
         new_atoms.positions = atoms.positions + vectors
         new_atoms.set_array(attribute, vectors * scale)
         new_atoms = new_atoms.repeat(repeat)
         trajectory.append(new_atoms)
     return trajectory
+
+
+def load_online_example(name="tio2.cif"):
+    """Load an example from the online data."""
+    from ase.io import read
+    import requests
+    from io import StringIO
+
+    url = "https://raw.githubusercontent.com/superstar54/weas/main/demo/datas/" + name
+    # Download the file content
+    response = requests.get(url)
+    if response.status_code == 200:
+        file_content = response.text
+        # Use StringIO to simulate a file-like object for ASE to read from
+        file_like_object = StringIO(file_content)
+        atoms = read(file_like_object, format="cif")
+        return atoms
+    else:
+        raise ValueError(f"Failed to download the file {name}")
```

