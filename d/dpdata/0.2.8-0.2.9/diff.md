# Comparing `tmp/dpdata-0.2.8.tar.gz` & `tmp/dpdata-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dpdata-0.2.8.tar", last modified: Wed Aug  3 03:14:44 2022, max compression
+gzip compressed data, was "dpdata-0.2.9.tar", last modified: Mon Oct  3 02:59:07 2022, max compression
```

## Comparing `dpdata-0.2.8.tar` & `dpdata-0.2.9.tar`

### file list

```diff
@@ -1,654 +1,654 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.899389 dpdata-0.2.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.791388 dpdata-0.2.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.807388 dpdata-0.2.8/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)     1330 2022-08-03 03:14:31.000000 dpdata-0.2.8/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (121)     1077 2022-08-03 03:14:31.000000 dpdata-0.2.8/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (121)      404 2022-08-03 03:14:31.000000 dpdata-0.2.8/.github/ISSUE_TEMPLATE/generic-issue.md
--rw-r--r--   0 runner    (1001) docker     (121)      663 2022-08-03 03:14:31.000000 dpdata-0.2.8/.github/ISSUE_TEMPLATE/request-for-help.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.807388 dpdata-0.2.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      570 2022-08-03 03:14:31.000000 dpdata-0.2.8/.github/workflows/mirror_gitee.yml
--rw-r--r--   0 runner    (1001) docker     (121)      846 2022-08-03 03:14:31.000000 dpdata-0.2.8/.github/workflows/pub-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (121)      793 2022-08-03 03:14:31.000000 dpdata-0.2.8/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (121)      339 2022-08-03 03:14:31.000000 dpdata-0.2.8/.github/workflows/test_import.yml
--rw-r--r--   0 runner    (1001) docker     (121)      261 2022-08-03 03:14:31.000000 dpdata-0.2.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     7652 2022-08-03 03:14:31.000000 dpdata-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    14088 2022-08-03 03:14:44.899389 dpdata-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    13533 2022-08-03 03:14:31.000000 dpdata-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.807388 dpdata-0.2.8/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      603 2022-08-03 03:14:31.000000 dpdata-0.2.8/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-08-03 03:14:31.000000 dpdata-0.2.8/docs/cli.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5917 2022-08-03 03:14:31.000000 dpdata-0.2.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      152 2022-08-03 03:14:31.000000 dpdata-0.2.8/docs/formats.rst
--rw-r--r--   0 runner    (1001) docker     (121)      492 2022-08-03 03:14:31.000000 dpdata-0.2.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2851 2022-08-03 03:14:31.000000 dpdata-0.2.8/docs/make_format.py
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-08-03 03:14:31.000000 dpdata-0.2.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.807388 dpdata-0.2.8/dpdata/
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-08-03 03:14:31.000000 dpdata-0.2.8/dpdata/__about__.py
--rw-r--r--   0 runner    (1001) docker     (121)      516 2022-08-03 03:14:31.000000 dpdata-0.2.8/dpdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-08-03 03:14:44.000000 dpdata-0.2.8/dpdata/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.807388 dpdata-0.2.8/dpdata/abacus/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:31.000000 dpdata-0.2.8/dpdata/abacus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6063 2022-08-03 03:14:31.000000 dpdata-0.2.8/dpdata/abacus/md.py
--rw-r--r--   0 runner    (1001) docker     (121)     5256 2022-08-03 03:14:31.000000 dpdata-0.2.8/dpdata/abacus/relax.py
--rw-r--r--   0 runner    (1001) docker     (121)    10603 2022-08-03 03:14:31.000000 dpdata-0.2.8/dpdata/abacus/scf.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.815388 dpdata-0.2.8/dpdata/amber/
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-03 03:14:31.000000 dpdata-0.2.8/dpdata/amber/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      972 2022-08-03 03:14:31.000000 dpdata-0.2.8/dpdata/amber/mask.py
--rw-r--r--   0 runner    (1001) docker     (121)     4637 2022-08-03 03:14:31.000000 dpdata-0.2.8/dpdata/amber/md.py
--rw-r--r--   0 runner    (1001) docker     (121)     3803 2022-08-03 03:14:31.000000 dpdata-0.2.8/dpdata/amber/sqm.py
--rw-r--r--   0 runner    (1001) docker     (121)     2460 2022-08-03 03:14:31.000000 dpdata-0.2.8/dpdata/ase_calculator.py
--rw-r--r--   0 runner    (1001) docker     (121)     6978 2022-08-03 03:14:31.000000 dpdata-0.2.8/dpdata/bond_order_system.py
--rw-r--r--   0 runner    (1001) docker     (121)     2689 2022-08-03 03:14:31.000000 dpdata-0.2.8/dpdata/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.815388 dpdata-0.2.8/dpdata/cp2k/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:31.000000 dpdata-0.2.8/dpdata/cp2k/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2105 2022-08-03 03:14:31.000000 dpdata-0.2.8/dpdata/cp2k/cell.py
--rw-r--r--   0 runner    (1001) docker     (121)    18230 2022-08-03 03:14:31.000000 dpdata-0.2.8/dpdata/cp2k/output.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.815388 dpdata-0.2.8/dpdata/deepmd/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:31.000000 dpdata-0.2.8/dpdata/deepmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5109 2022-08-03 03:14:31.000000 dpdata-0.2.8/dpdata/deepmd/comp.py
--rw-r--r--   0 runner    (1001) docker     (121)     5145 2022-08-03 03:14:31.000000 dpdata-0.2.8/dpdata/deepmd/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (121)     3971 2022-08-03 03:14:31.000000 dpdata-0.2.8/dpdata/deepmd/raw.py
--rw-r--r--   0 runner    (1001) docker     (121)     4081 2022-08-03 03:14:31.000000 dpdata-0.2.8/dpdata/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.815388 dpdata-0.2.8/dpdata/fhi_aims/
--rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:31.000000 dpdata-0.2.8/dpdata/fhi_aims/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     5210 2022-08-03 03:14:31.000000 dpdata-0.2.8/dpdata/fhi_aims/output.py
--rw-r--r--   0 runner    (1001) docker     (121)     3393 2022-08-03 03:14:31.000000 dpdata-0.2.8/dpdata/format.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.815388 dpdata-0.2.8/dpdata/gaussian/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:31.000000 dpdata-0.2.8/dpdata/gaussian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8126 2022-08-03 03:14:31.000000 dpdata-0.2.8/dpdata/gaussian/gjf.py
--rw-r--r--   0 runner    (1001) docker     (121)     2686 2022-08-03 03:14:31.000000 dpdata-0.2.8/dpdata/gaussian/log.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.819388 dpdata-0.2.8/dpdata/gromacs/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:31.000000 dpdata-0.2.8/dpdata/gromacs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3311 2022-08-03 03:14:31.000000 dpdata-0.2.8/dpdata/gromacs/gro.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.819388 dpdata-0.2.8/dpdata/lammps/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:31.000000 dpdata-0.2.8/dpdata/lammps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7217 2022-08-03 03:14:31.000000 dpdata-0.2.8/dpdata/lammps/dump.py
--rw-r--r--   0 runner    (1001) docker     (121)     6227 2022-08-03 03:14:31.000000 dpdata-0.2.8/dpdata/lammps/lmp.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.819388 dpdata-0.2.8/dpdata/md/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:31.000000 dpdata-0.2.8/dpdata/md/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1824 2022-08-03 03:14:31.000000 dpdata-0.2.8/dpdata/md/msd.py
--rw-r--r--   0 runner    (1001) docker     (121)     1887 2022-08-03 03:14:31.000000 dpdata-0.2.8/dpdata/md/pbc.py
--rw-r--r--   0 runner    (1001) docker     (121)     4251 2022-08-03 03:14:31.000000 dpdata-0.2.8/dpdata/md/rdf.py
--rw-r--r--   0 runner    (1001) docker     (121)     7072 2022-08-03 03:14:31.000000 dpdata-0.2.8/dpdata/md/water.py
--rw-r--r--   0 runner    (1001) docker     (121)    18474 2022-08-03 03:14:31.000000 dpdata-0.2.8/dpdata/periodic_table.json
--rw-r--r--   0 runner    (1001) docker     (121)     1774 2022-08-03 03:14:32.000000 dpdata-0.2.8/dpdata/periodic_table.py
--rw-r--r--   0 runner    (1001) docker     (121)      747 2022-08-03 03:14:32.000000 dpdata-0.2.8/dpdata/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.823388 dpdata-0.2.8/dpdata/plugins/
--rw-r--r--   0 runner    (1001) docker     (121)      599 2022-08-03 03:14:32.000000 dpdata-0.2.8/dpdata/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2299 2022-08-03 03:14:32.000000 dpdata-0.2.8/dpdata/plugins/abacus.py
--rw-r--r--   0 runner    (1001) docker     (121)     4567 2022-08-03 03:14:32.000000 dpdata-0.2.8/dpdata/plugins/amber.py
--rw-r--r--   0 runner    (1001) docker     (121)     6560 2022-08-03 03:14:32.000000 dpdata-0.2.8/dpdata/plugins/ase.py
--rw-r--r--   0 runner    (1001) docker     (121)     1017 2022-08-03 03:14:32.000000 dpdata-0.2.8/dpdata/plugins/cp2k.py
--rw-r--r--   0 runner    (1001) docker     (121)    10446 2022-08-03 03:14:32.000000 dpdata-0.2.8/dpdata/plugins/deepmd.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:32.000000 dpdata-0.2.8/dpdata/plugins/dftbplus.py
--rw-r--r--   0 runner    (1001) docker     (121)     1271 2022-08-03 03:14:32.000000 dpdata-0.2.8/dpdata/plugins/fhi_aims.py
--rw-r--r--   0 runner    (1001) docker     (121)     3371 2022-08-03 03:14:32.000000 dpdata-0.2.8/dpdata/plugins/gaussian.py
--rw-r--r--   0 runner    (1001) docker     (121)     1493 2022-08-03 03:14:32.000000 dpdata-0.2.8/dpdata/plugins/gromacs.py
--rw-r--r--   0 runner    (1001) docker     (121)     1404 2022-08-03 03:14:32.000000 dpdata-0.2.8/dpdata/plugins/lammps.py
--rw-r--r--   0 runner    (1001) docker     (121)      660 2022-08-03 03:14:32.000000 dpdata-0.2.8/dpdata/plugins/list.py
--rw-r--r--   0 runner    (1001) docker     (121)     2076 2022-08-03 03:14:32.000000 dpdata-0.2.8/dpdata/plugins/pwmat.py
--rw-r--r--   0 runner    (1001) docker     (121)     2847 2022-08-03 03:14:32.000000 dpdata-0.2.8/dpdata/plugins/pymatgen.py
--rw-r--r--   0 runner    (1001) docker     (121)     1653 2022-08-03 03:14:32.000000 dpdata-0.2.8/dpdata/plugins/qe.py
--rw-r--r--   0 runner    (1001) docker     (121)     1469 2022-08-03 03:14:32.000000 dpdata-0.2.8/dpdata/plugins/rdkit.py
--rw-r--r--   0 runner    (1001) docker     (121)     1822 2022-08-03 03:14:32.000000 dpdata-0.2.8/dpdata/plugins/siesta.py
--rw-r--r--   0 runner    (1001) docker     (121)     3846 2022-08-03 03:14:32.000000 dpdata-0.2.8/dpdata/plugins/vasp.py
--rw-r--r--   0 runner    (1001) docker     (121)     1483 2022-08-03 03:14:32.000000 dpdata-0.2.8/dpdata/plugins/xyz.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.827388 dpdata-0.2.8/dpdata/pwmat/
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-03 03:14:32.000000 dpdata-0.2.8/dpdata/pwmat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3408 2022-08-03 03:14:32.000000 dpdata-0.2.8/dpdata/pwmat/atomconfig.py
--rw-r--r--   0 runner    (1001) docker     (121)     6540 2022-08-03 03:14:32.000000 dpdata-0.2.8/dpdata/pwmat/movement.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.827388 dpdata-0.2.8/dpdata/pymatgen/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:32.000000 dpdata-0.2.8/dpdata/pymatgen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      938 2022-08-03 03:14:32.000000 dpdata-0.2.8/dpdata/pymatgen/molecule.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.827388 dpdata-0.2.8/dpdata/qe/
--rw-r--r--   0 runner    (1001) docker     (121)        2 2022-08-03 03:14:32.000000 dpdata-0.2.8/dpdata/qe/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     5108 2022-08-03 03:14:32.000000 dpdata-0.2.8/dpdata/qe/scf.py
--rw-r--r--   0 runner    (1001) docker     (121)     7546 2022-08-03 03:14:32.000000 dpdata-0.2.8/dpdata/qe/traj.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.827388 dpdata-0.2.8/dpdata/rdkit/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:32.000000 dpdata-0.2.8/dpdata/rdkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    24936 2022-08-03 03:14:32.000000 dpdata-0.2.8/dpdata/rdkit/sanitize.py
--rw-r--r--   0 runner    (1001) docker     (121)     4220 2022-08-03 03:14:32.000000 dpdata-0.2.8/dpdata/rdkit/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.827388 dpdata-0.2.8/dpdata/siesta/
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-03 03:14:32.000000 dpdata-0.2.8/dpdata/siesta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5070 2022-08-03 03:14:32.000000 dpdata-0.2.8/dpdata/siesta/aiMD_output.py
--rw-r--r--   0 runner    (1001) docker     (121)     4175 2022-08-03 03:14:32.000000 dpdata-0.2.8/dpdata/siesta/output.py
--rw-r--r--   0 runner    (1001) docker     (121)     3983 2022-08-03 03:14:32.000000 dpdata-0.2.8/dpdata/stat.py
--rw-r--r--   0 runner    (1001) docker     (121)    53253 2022-08-03 03:14:32.000000 dpdata-0.2.8/dpdata/system.py
--rw-r--r--   0 runner    (1001) docker     (121)     5114 2022-08-03 03:14:32.000000 dpdata-0.2.8/dpdata/unit.py
--rw-r--r--   0 runner    (1001) docker     (121)     3347 2022-08-03 03:14:32.000000 dpdata-0.2.8/dpdata/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.831388 dpdata-0.2.8/dpdata/vasp/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:32.000000 dpdata-0.2.8/dpdata/vasp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5268 2022-08-03 03:14:32.000000 dpdata-0.2.8/dpdata/vasp/outcar.py
--rw-r--r--   0 runner    (1001) docker     (121)     2872 2022-08-03 03:14:32.000000 dpdata-0.2.8/dpdata/vasp/poscar.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3834 2022-08-03 03:14:32.000000 dpdata-0.2.8/dpdata/vasp/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.831388 dpdata-0.2.8/dpdata/xyz/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:32.000000 dpdata-0.2.8/dpdata/xyz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5937 2022-08-03 03:14:32.000000 dpdata-0.2.8/dpdata/xyz/quip_gap_xyz.py
--rw-r--r--   0 runner    (1001) docker     (121)     1309 2022-08-03 03:14:32.000000 dpdata-0.2.8/dpdata/xyz/xyz.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.807388 dpdata-0.2.8/dpdata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    14088 2022-08-03 03:14:44.000000 dpdata-0.2.8/dpdata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    17852 2022-08-03 03:14:44.000000 dpdata-0.2.8/dpdata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-03 03:14:44.000000 dpdata-0.2.8/dpdata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-08-03 03:14:44.000000 dpdata-0.2.8/dpdata.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      243 2022-08-03 03:14:44.000000 dpdata-0.2.8/dpdata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)      235 2022-08-03 03:14:44.000000 dpdata-0.2.8/dpdata.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.831388 dpdata-0.2.8/plugin_example/
--rw-r--r--   0 runner    (1001) docker     (121)      277 2022-08-03 03:14:32.000000 dpdata-0.2.8/plugin_example/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.831388 dpdata-0.2.8/plugin_example/dpdata_random/
--rw-r--r--   0 runner    (1001) docker     (121)      869 2022-08-03 03:14:32.000000 dpdata-0.2.8/plugin_example/dpdata_random/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      251 2022-08-03 03:14:32.000000 dpdata-0.2.8/plugin_example/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-08-03 03:14:32.000000 dpdata-0.2.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-03 03:14:44.899389 dpdata-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2035 2022-08-03 03:14:32.000000 dpdata-0.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.847389 dpdata-0.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      673 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/POSCAR
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.847389 dpdata-0.2.8/tests/abacus.md/
--rw-r--r--   0 runner    (1001) docker     (121)      907 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/abacus.md/INPUT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.847389 dpdata-0.2.8/tests/abacus.md/OUT.abacus/
--rw-r--r--   0 runner    (1001) docker     (121)     4043 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/abacus.md/OUT.abacus/MD_dump
--rw-r--r--   0 runner    (1001) docker     (121)    88365 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/abacus.md/OUT.abacus/running_md.log
--rw-r--r--   0 runner    (1001) docker     (121)      458 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/abacus.md/STRU
--rw-r--r--   0 runner    (1001) docker     (121)      523 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/abacus.md/water_coord
--rw-r--r--   0 runner    (1001) docker     (121)      711 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/abacus.md/water_force
--rw-r--r--   0 runner    (1001) docker     (121)      710 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/abacus.md/water_virial
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.847389 dpdata-0.2.8/tests/abacus.md.nostress/
--rw-r--r--   0 runner    (1001) docker     (121)      416 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/abacus.md.nostress/INPUT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.847389 dpdata-0.2.8/tests/abacus.md.nostress/OUT.autotest/
--rw-r--r--   0 runner    (1001) docker     (121)     1888 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/abacus.md.nostress/OUT.autotest/MD_dump
--rw-r--r--   0 runner    (1001) docker     (121)    21769 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/abacus.md.nostress/OUT.autotest/running_md.log
--rw-r--r--   0 runner    (1001) docker     (121)      303 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/abacus.md.nostress/STRU
--rw-r--r--   0 runner    (1001) docker     (121)      234 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/abacus.md.nostress/Si_coord
--rw-r--r--   0 runner    (1001) docker     (121)      283 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/abacus.md.nostress/Si_force
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.847389 dpdata-0.2.8/tests/abacus.relax/
--rw-r--r--   0 runner    (1001) docker     (121)      603 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/abacus.relax/INPUT
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/abacus.relax/KPT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.851389 dpdata-0.2.8/tests/abacus.relax/OUT.abacus/
--rw-r--r--   0 runner    (1001) docker     (121)    12748 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/abacus.relax/OUT.abacus/INPUT
--rw-r--r--   0 runner    (1001) docker     (121)      468 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/abacus.relax/OUT.abacus/STRU_ION_D
--rw-r--r--   0 runner    (1001) docker     (121)      409 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/abacus.relax/OUT.abacus/STRU_READIN_ADJUST.cif
--rw-r--r--   0 runner    (1001) docker     (121)    54773 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/abacus.relax/OUT.abacus/running_cell-relax.log
--rw-r--r--   0 runner    (1001) docker     (121)      482 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/abacus.relax/STRU
--rw-r--r--   0 runner    (1001) docker     (121)      810 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/abacus.relax/coord.ref
--rw-r--r--   0 runner    (1001) docker     (121)      810 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/abacus.relax/force.ref
--rw-r--r--   0 runner    (1001) docker     (121)      810 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/abacus.relax/stress.ref
--rw-r--r--   0 runner    (1001) docker     (121)      810 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/abacus.relax/virial.ref
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.851389 dpdata-0.2.8/tests/abacus.scf/
--rw-r--r--   0 runner    (1001) docker     (121)      455 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/abacus.scf/INPUT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.851389 dpdata-0.2.8/tests/abacus.scf/OUT.ch4/
--rw-r--r--   0 runner    (1001) docker     (121)    26715 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/abacus.scf/OUT.ch4/running_scf.log
--rw-r--r--   0 runner    (1001) docker     (121)      743 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/abacus.scf/STRU.ch4
--rw-r--r--   0 runner    (1001) docker     (121)      164 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/abacus.scf/ch4_coord
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/abacus.scf/ch4_force
--rw-r--r--   0 runner    (1001) docker     (121)      106 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/abacus.scf/ch4_virial
--rw-r--r--   0 runner    (1001) docker     (121)      580 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/abacus.scf/stru_test
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.851389 dpdata-0.2.8/tests/amber/
--rw-r--r--   0 runner    (1001) docker     (121)     8237 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/amber/02_Heat.mden
--rw-r--r--   0 runner    (1001) docker     (121)   229960 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/amber/02_Heat.mdfrc
--rw-r--r--   0 runner    (1001) docker     (121)   230760 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/amber/02_Heat.nc
--rw-r--r--   0 runner    (1001) docker     (121)   321683 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/amber/02_Heat.parm7
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.855389 dpdata-0.2.8/tests/amber/corr/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.799388 dpdata-0.2.8/tests/amber/corr/dataset/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.855389 dpdata-0.2.8/tests/amber/corr/dataset/C6H11HW192O6OW96P1/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/amber/corr/dataset/C6H11HW192O6OW96P1/nopbc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.855389 dpdata-0.2.8/tests/amber/corr/dataset/C6H11HW192O6OW96P1/set.000/
--rw-r--r--   0 runner    (1001) docker     (121)      164 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/amber/corr/dataset/C6H11HW192O6OW96P1/set.000/box.npy
--rw-r--r--   0 runner    (1001) docker     (121)     3872 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/amber/corr/dataset/C6H11HW192O6OW96P1/set.000/coord.npy
--rw-r--r--   0 runner    (1001) docker     (121)      132 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/amber/corr/dataset/C6H11HW192O6OW96P1/set.000/energy.npy
--rw-r--r--   0 runner    (1001) docker     (121)     3872 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/amber/corr/dataset/C6H11HW192O6OW96P1/set.000/force.npy
--rw-r--r--   0 runner    (1001) docker     (121)      624 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/amber/corr/dataset/C6H11HW192O6OW96P1/type.raw
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/amber/corr/dataset/C6H11HW192O6OW96P1/type_map.raw
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.799388 dpdata-0.2.8/tests/amber/corr/dp_amber_mask/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.855389 dpdata-0.2.8/tests/amber/corr/dp_amber_mask/C6EP0H11HW192O6OW96P1/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/amber/corr/dp_amber_mask/C6EP0H11HW192O6OW96P1/nopbc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.855389 dpdata-0.2.8/tests/amber/corr/dp_amber_mask/C6EP0H11HW192O6OW96P1/set.000/
--rw-r--r--   0 runner    (1001) docker     (121)      164 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/amber/corr/dp_amber_mask/C6EP0H11HW192O6OW96P1/set.000/box.npy
--rw-r--r--   0 runner    (1001) docker     (121)     3872 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/amber/corr/dp_amber_mask/C6EP0H11HW192O6OW96P1/set.000/coord.npy
--rw-r--r--   0 runner    (1001) docker     (121)      132 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/amber/corr/dp_amber_mask/C6EP0H11HW192O6OW96P1/set.000/energy.npy
--rw-r--r--   0 runner    (1001) docker     (121)     3872 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/amber/corr/dp_amber_mask/C6EP0H11HW192O6OW96P1/set.000/force.npy
--rw-r--r--   0 runner    (1001) docker     (121)      624 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/amber/corr/dp_amber_mask/C6EP0H11HW192O6OW96P1/type.raw
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/amber/corr/dp_amber_mask/C6EP0H11HW192O6OW96P1/type_map.raw
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.855389 dpdata-0.2.8/tests/amber/corr/dp_corr/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.855389 dpdata-0.2.8/tests/amber/corr/dp_corr/set.000/
--rw-r--r--   0 runner    (1001) docker     (121)      164 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/amber/corr/dp_corr/set.000/box.npy
--rw-r--r--   0 runner    (1001) docker     (121)    72896 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/amber/corr/dp_corr/set.000/coord.npy
--rw-r--r--   0 runner    (1001) docker     (121)      132 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/amber/corr/dp_corr/set.000/energy.npy
--rw-r--r--   0 runner    (1001) docker     (121)    72896 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/amber/corr/dp_corr/set.000/force.npy
--rw-r--r--   0 runner    (1001) docker     (121)    12128 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/amber/corr/dp_corr/type.raw
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/amber/corr/dp_corr/type_map.raw
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.855389 dpdata-0.2.8/tests/amber/corr/dp_hl/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.855389 dpdata-0.2.8/tests/amber/corr/dp_hl/set.000/
--rw-r--r--   0 runner    (1001) docker     (121)      164 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/amber/corr/dp_hl/set.000/box.npy
--rw-r--r--   0 runner    (1001) docker     (121)    72896 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/amber/corr/dp_hl/set.000/coord.npy
--rw-r--r--   0 runner    (1001) docker     (121)      132 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/amber/corr/dp_hl/set.000/energy.npy
--rw-r--r--   0 runner    (1001) docker     (121)    72896 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/amber/corr/dp_hl/set.000/force.npy
--rw-r--r--   0 runner    (1001) docker     (121)    12128 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/amber/corr/dp_hl/type.raw
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/amber/corr/dp_hl/type_map.raw
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.855389 dpdata-0.2.8/tests/amber/corr/dp_ll/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.855389 dpdata-0.2.8/tests/amber/corr/dp_ll/set.000/
--rw-r--r--   0 runner    (1001) docker     (121)      164 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/amber/corr/dp_ll/set.000/box.npy
--rw-r--r--   0 runner    (1001) docker     (121)    72896 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/amber/corr/dp_ll/set.000/coord.npy
--rw-r--r--   0 runner    (1001) docker     (121)      132 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/amber/corr/dp_ll/set.000/energy.npy
--rw-r--r--   0 runner    (1001) docker     (121)    72896 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/amber/corr/dp_ll/set.000/force.npy
--rw-r--r--   0 runner    (1001) docker     (121)    12128 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/amber/corr/dp_ll/type.raw
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/amber/corr/dp_ll/type_map.raw
--rw-r--r--   0 runner    (1001) docker     (121)    73252 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/amber/corr/high_level.mdfrc
--rw-r--r--   0 runner    (1001) docker     (121)    27097 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/amber/corr/high_level.mdout
--rw-r--r--   0 runner    (1001) docker     (121)    73252 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/amber/corr/low_level.mdfrc
--rw-r--r--   0 runner    (1001) docker     (121)    27017 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/amber/corr/low_level.mdout
--rw-r--r--   0 runner    (1001) docker     (121)  1036937 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/amber/corr/qmmm.parm7
--rw-r--r--   0 runner    (1001) docker     (121)    97988 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/amber/corr/rc.nc
--rw-r--r--   0 runner    (1001) docker     (121)      474 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/amber/methane.mol
--rw-r--r--   0 runner    (1001) docker     (121)      407 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/amber/sqm.in
--rw-r--r--   0 runner    (1001) docker     (121)    25413 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/amber/sqm_forces.out
--rw-r--r--   0 runner    (1001) docker     (121)     6224 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/amber/sqm_no_forces.out
--rw-r--r--   0 runner    (1001) docker     (121)    46476 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/amber/sqm_opt.out
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.855389 dpdata-0.2.8/tests/ase_traj/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.859389 dpdata-0.2.8/tests/ase_traj/Al0He4O0/
--rw-r--r--   0 runner    (1001) docker     (121)      228 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/ase_traj/Al0He4O0/box.raw
--rw-r--r--   0 runner    (1001) docker     (121)      300 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/ase_traj/Al0He4O0/coord.raw
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/ase_traj/Al0He4O0/energy.raw
--rw-r--r--   0 runner    (1001) docker     (121)      306 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/ase_traj/Al0He4O0/force.raw
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/ase_traj/Al0He4O0/type.raw
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/ase_traj/Al0He4O0/type_map.raw
--rw-r--r--   0 runner    (1001) docker     (121)      229 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/ase_traj/Al0He4O0/virial.raw
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.859389 dpdata-0.2.8/tests/ase_traj/Al2He1O3/
--rw-r--r--   0 runner    (1001) docker     (121)      225 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/ase_traj/Al2He1O3/box.raw
--rw-r--r--   0 runner    (1001) docker     (121)      450 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/ase_traj/Al2He1O3/coord.raw
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/ase_traj/Al2He1O3/energy.raw
--rw-r--r--   0 runner    (1001) docker     (121)      461 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/ase_traj/Al2He1O3/force.raw
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/ase_traj/Al2He1O3/type.raw
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/ase_traj/Al2He1O3/type_map.raw
--rw-r--r--   0 runner    (1001) docker     (121)      225 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/ase_traj/Al2He1O3/virial.raw
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.859389 dpdata-0.2.8/tests/ase_traj/Al2He2O3/
--rw-r--r--   0 runner    (1001) docker     (121)      226 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/ase_traj/Al2He2O3/box.raw
--rw-r--r--   0 runner    (1001) docker     (121)      525 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/ase_traj/Al2He2O3/coord.raw
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/ase_traj/Al2He2O3/energy.raw
--rw-r--r--   0 runner    (1001) docker     (121)      536 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/ase_traj/Al2He2O3/force.raw
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/ase_traj/Al2He2O3/type.raw
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/ase_traj/Al2He2O3/type_map.raw
--rw-r--r--   0 runner    (1001) docker     (121)      227 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/ase_traj/Al2He2O3/virial.raw
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.859389 dpdata-0.2.8/tests/ase_traj/Al4He0O6/
--rw-r--r--   0 runner    (1001) docker     (121)      227 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/ase_traj/Al4He0O6/box.raw
--rw-r--r--   0 runner    (1001) docker     (121)      750 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/ase_traj/Al4He0O6/coord.raw
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/ase_traj/Al4He0O6/energy.raw
--rw-r--r--   0 runner    (1001) docker     (121)      767 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/ase_traj/Al4He0O6/force.raw
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/ase_traj/Al4He0O6/type.raw
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/ase_traj/Al4He0O6/type_map.raw
--rw-r--r--   0 runner    (1001) docker     (121)      225 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/ase_traj/Al4He0O6/virial.raw
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.859389 dpdata-0.2.8/tests/ase_traj/Al4He2O6/
--rw-r--r--   0 runner    (1001) docker     (121)      225 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/ase_traj/Al4He2O6/box.raw
--rw-r--r--   0 runner    (1001) docker     (121)      900 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/ase_traj/Al4He2O6/coord.raw
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/ase_traj/Al4He2O6/energy.raw
--rw-r--r--   0 runner    (1001) docker     (121)      911 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/ase_traj/Al4He2O6/force.raw
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/ase_traj/Al4He2O6/type.raw
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/ase_traj/Al4He2O6/type_map.raw
--rw-r--r--   0 runner    (1001) docker     (121)      225 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/ase_traj/Al4He2O6/virial.raw
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.859389 dpdata-0.2.8/tests/ase_traj/Al4He4O6/
--rw-r--r--   0 runner    (1001) docker     (121)      227 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/ase_traj/Al4He4O6/box.raw
--rw-r--r--   0 runner    (1001) docker     (121)     1050 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/ase_traj/Al4He4O6/coord.raw
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/ase_traj/Al4He4O6/energy.raw
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/ase_traj/Al4He4O6/force.raw
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/ase_traj/Al4He4O6/type.raw
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/ase_traj/Al4He4O6/type_map.raw
--rw-r--r--   0 runner    (1001) docker     (121)      227 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/ase_traj/Al4He4O6/virial.raw
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.863389 dpdata-0.2.8/tests/ase_traj/Al8He0O12/
--rw-r--r--   0 runner    (1001) docker     (121)      678 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/ase_traj/Al8He0O12/box.raw
--rw-r--r--   0 runner    (1001) docker     (121)     4500 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/ase_traj/Al8He0O12/coord.raw
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/ase_traj/Al8He0O12/energy.raw
--rw-r--r--   0 runner    (1001) docker     (121)     4593 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/ase_traj/Al8He0O12/force.raw
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/ase_traj/Al8He0O12/type.raw
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/ase_traj/Al8He0O12/type_map.raw
--rw-r--r--   0 runner    (1001) docker     (121)      679 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/ase_traj/Al8He0O12/virial.raw
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.863389 dpdata-0.2.8/tests/ase_traj/Al8He4O12/
--rw-r--r--   0 runner    (1001) docker     (121)      227 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/ase_traj/Al8He4O12/box.raw
--rw-r--r--   0 runner    (1001) docker     (121)     1800 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/ase_traj/Al8He4O12/coord.raw
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/ase_traj/Al8He4O12/energy.raw
--rw-r--r--   0 runner    (1001) docker     (121)     1836 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/ase_traj/Al8He4O12/force.raw
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/ase_traj/Al8He4O12/type.raw
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/ase_traj/Al8He4O12/type_map.raw
--rw-r--r--   0 runner    (1001) docker     (121)      227 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/ase_traj/Al8He4O12/virial.raw
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.863389 dpdata-0.2.8/tests/ase_traj/Al8He8O12/
--rw-r--r--   0 runner    (1001) docker     (121)      225 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/ase_traj/Al8He8O12/box.raw
--rw-r--r--   0 runner    (1001) docker     (121)     2100 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/ase_traj/Al8He8O12/coord.raw
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/ase_traj/Al8He8O12/energy.raw
--rw-r--r--   0 runner    (1001) docker     (121)     2161 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/ase_traj/Al8He8O12/force.raw
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/ase_traj/Al8He8O12/type.raw
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/ase_traj/Al8He8O12/type_map.raw
--rw-r--r--   0 runner    (1001) docker     (121)      225 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/ase_traj/Al8He8O12/virial.raw
--rw-r--r--   0 runner    (1001) docker     (121)    14428 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/ase_traj/HeAlO.traj
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.863389 dpdata-0.2.8/tests/bond_order/
--rw-r--r--   0 runner    (1001) docker     (121)      806 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/bond_order/BOH4-.mol
--rw-r--r--   0 runner    (1001) docker     (121)      902 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/bond_order/C5H5-.mol
--rw-r--r--   0 runner    (1001) docker     (121)      557 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/bond_order/CH3CC-.mol
--rw-r--r--   0 runner    (1001) docker     (121)      557 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/bond_order/CH3NC.mol
--rw-r--r--   0 runner    (1001) docker     (121)      723 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/bond_order/CH3NH3+.mol
--rw-r--r--   0 runner    (1001) docker     (121)      640 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/bond_order/CH3NO2.mol
--rw-r--r--   0 runner    (1001) docker     (121)      806 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/bond_order/CH3OAsO3_2-.mol
--rw-r--r--   0 runner    (1001) docker     (121)      557 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/bond_order/CH3OH.mol
--rw-r--r--   0 runner    (1001) docker     (121)      806 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/bond_order/CH3OPO3_2-.mol
--rw-r--r--   0 runner    (1001) docker     (121)      723 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/bond_order/CH3PH3+.mol
--rw-r--r--   0 runner    (1001) docker     (121)      557 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/bond_order/CH3SH.mol
--rw-r--r--   0 runner    (1001) docker     (121)      723 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/bond_order/CH3SO3-.mol
--rw-r--r--   0 runner    (1001) docker     (121)      889 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/bond_order/CH3_2SO.mol
--rw-r--r--   0 runner    (1001) docker     (121)      972 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/bond_order/CH3_2SO2.mol
--rw-r--r--   0 runner    (1001) docker     (121)     1138 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/bond_order/OCH3+.mol
--rw-r--r--   0 runner    (1001) docker     (121)     1138 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/bond_order/arg.mol
--rw-r--r--   0 runner    (1001) docker     (121)     4911 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/bond_order/formal_charge.mol
--rw-r--r--   0 runner    (1001) docker     (121)      889 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/bond_order/gly.mol
--rw-r--r--   0 runner    (1001) docker     (121)     1916 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/bond_order/methane.sdf
--rw-r--r--   0 runner    (1001) docker     (121)     2414 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/bond_order/methane_ethane.sdf
--rw-r--r--   0 runner    (1001) docker     (121)     1068 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/bond_order/oxpy.mol
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.803388 dpdata-0.2.8/tests/bond_order/refined-set-ligands/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.863389 dpdata-0.2.8/tests/bond_order/refined-set-ligands/obabel/
--rw-r--r--   0 runner    (1001) docker     (121)     4167 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/bond_order/refined-set-ligands/obabel/1a4r_ligand_obabel.sdf
--rw-r--r--   0 runner    (1001) docker     (121)     2017 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/bond_order/refined-set-ligands/obabel/1ai5_ligand_obabel.sdf
--rw-r--r--   0 runner    (1001) docker     (121)     2480 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/bond_order/refined-set-ligands/obabel/1f5l_ligand_obabel.sdf
--rw-r--r--   0 runner    (1001) docker     (121)     1352 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/bond_order/refined-set-ligands/obabel/1m1b_ligand_obabel.sdf
--rw-r--r--   0 runner    (1001) docker     (121)     4810 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/bond_order/refined-set-ligands/obabel/1mue_ligand_obabel.sdf
--rw-r--r--   0 runner    (1001) docker     (121)     3130 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/bond_order/refined-set-ligands/obabel/1w4q_ligand_obabel.sdf
--rw-r--r--   0 runner    (1001) docker     (121)     4439 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/bond_order/refined-set-ligands/obabel/2e94_ligand_obabel.sdf
--rw-r--r--   0 runner    (1001) docker     (121)     2425 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/bond_order/refined-set-ligands/obabel/4xaq_ligand_obabel.sdf
--rw-r--r--   0 runner    (1001) docker     (121)     6603 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/bond_order/refined-set-ligands/obabel/4xtw_ligand_obabel.sdf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.867389 dpdata-0.2.8/tests/bond_order/refined-set-ligands/origin/
--rw-r--r--   0 runner    (1001) docker     (121)     3213 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/bond_order/refined-set-ligands/origin/1a4r_ligand.sdf
--rw-r--r--   0 runner    (1001) docker     (121)     1559 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/bond_order/refined-set-ligands/origin/1ai5_ligand.sdf
--rw-r--r--   0 runner    (1001) docker     (121)     1911 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/bond_order/refined-set-ligands/origin/1f5l_ligand.sdf
--rw-r--r--   0 runner    (1001) docker     (121)     1050 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/bond_order/refined-set-ligands/origin/1m1b_ligand.sdf
--rw-r--r--   0 runner    (1001) docker     (121)     3704 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/bond_order/refined-set-ligands/origin/1mue_ligand.sdf
--rw-r--r--   0 runner    (1001) docker     (121)     2422 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/bond_order/refined-set-ligands/origin/1w4q_ligand.sdf
--rw-r--r--   0 runner    (1001) docker     (121)     3421 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/bond_order/refined-set-ligands/origin/2e94_ligand.sdf
--rw-r--r--   0 runner    (1001) docker     (121)     1859 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/bond_order/refined-set-ligands/origin/4xaq_ligand.sdf
--rw-r--r--   0 runner    (1001) docker     (121)     5071 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/bond_order/refined-set-ligands/origin/4xtw_ligand.sdf
--rw-r--r--   0 runner    (1001) docker     (121)     4633 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/comp_sys.py
--rw-r--r--   0 runner    (1001) docker     (121)     5956 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/computed_structure_entry.json
--rw-r--r--   0 runner    (1001) docker     (121)      222 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/context.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.867389 dpdata-0.2.8/tests/cp2k/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.875389 dpdata-0.2.8/tests/cp2k/aimd/
--rw-r--r--   0 runner    (1001) docker     (121)     4061 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/cp2k/aimd/DPGEN-1.ener
--rw-r--r--   0 runner    (1001) docker     (121)  1041450 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/cp2k/aimd/DPGEN-frc-1.xyz
--rw-r--r--   0 runner    (1001) docker     (121)  1041450 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/cp2k/aimd/DPGEN-pos-1.xyz
--rw-r--r--   0 runner    (1001) docker     (121)  4621389 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/cp2k/aimd/cp2k.log
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.875389 dpdata-0.2.8/tests/cp2k/aimd/deepmd/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.875389 dpdata-0.2.8/tests/cp2k/aimd/deepmd/set.000/
--rw-r--r--   0 runner    (1001) docker     (121)     1208 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/cp2k/aimd/deepmd/set.000/box.npy
--rw-r--r--   0 runner    (1001) docker     (121)   192008 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/cp2k/aimd/deepmd/set.000/coord.npy
--rw-r--r--   0 runner    (1001) docker     (121)      248 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/cp2k/aimd/deepmd/set.000/energy.npy
--rw-r--r--   0 runner    (1001) docker     (121)   192008 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/cp2k/aimd/deepmd/set.000/force.npy
--rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/cp2k/aimd/deepmd/type.raw
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/cp2k/aimd/deepmd/type_map.raw
--rw-r--r--   0 runner    (1001) docker     (121)    28510 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/cp2k/aimd/input.inp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.875389 dpdata-0.2.8/tests/cp2k/aimd_stress/
--rw-r--r--   0 runner    (1001) docker     (121)      207 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/cp2k/aimd_stress/DPGEN-pos-1.xyz
--rw-r--r--   0 runner    (1001) docker     (121)   110555 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/cp2k/aimd_stress/cp2k.log
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.875389 dpdata-0.2.8/tests/cp2k/aimd_stress/deepmd/
--rw-r--r--   0 runner    (1001) docker     (121)      225 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/cp2k/aimd_stress/deepmd/box.raw
--rw-r--r--   0 runner    (1001) docker     (121)      375 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/cp2k/aimd_stress/deepmd/coord.raw
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/cp2k/aimd_stress/deepmd/energy.raw
--rw-r--r--   0 runner    (1001) docker     (121)      382 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/cp2k/aimd_stress/deepmd/force.raw
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/cp2k/aimd_stress/deepmd/type.raw
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/cp2k/aimd_stress/deepmd/type_map.raw
--rw-r--r--   0 runner    (1001) docker     (121)      230 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/cp2k/aimd_stress/deepmd/virial.raw
--rw-r--r--   0 runner    (1001) docker     (121)     1966 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/cp2k/aimd_stress/input.inp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.875389 dpdata-0.2.8/tests/cp2k/cp2k_duplicate_header/
--rw-r--r--   0 runner    (1001) docker     (121)   186887 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/cp2k/cp2k_duplicate_header/cp2k_output_duplicate_header
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.875389 dpdata-0.2.8/tests/cp2k/cp2k_duplicate_header/deepmd/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.875389 dpdata-0.2.8/tests/cp2k/cp2k_duplicate_header/deepmd/set.000/
--rw-r--r--   0 runner    (1001) docker     (121)      164 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/cp2k/cp2k_duplicate_header/deepmd/set.000/box.npy
--rw-r--r--   0 runner    (1001) docker     (121)      488 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/cp2k/cp2k_duplicate_header/deepmd/set.000/coord.npy
--rw-r--r--   0 runner    (1001) docker     (121)      132 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/cp2k/cp2k_duplicate_header/deepmd/set.000/energy.npy
--rw-r--r--   0 runner    (1001) docker     (121)      488 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/cp2k/cp2k_duplicate_header/deepmd/set.000/force.npy
--rw-r--r--   0 runner    (1001) docker     (121)      164 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/cp2k/cp2k_duplicate_header/deepmd/set.000/virial.npy
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/cp2k/cp2k_duplicate_header/deepmd/type.raw
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/cp2k/cp2k_duplicate_header/deepmd/type_map.raw
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.875389 dpdata-0.2.8/tests/cp2k/cp2k_element_replace/
--rw-r--r--   0 runner    (1001) docker     (121)   329537 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/cp2k/cp2k_element_replace/cp2k_output_element_replace
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.879389 dpdata-0.2.8/tests/cp2k/cp2k_element_replace/deepmd/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.879389 dpdata-0.2.8/tests/cp2k/cp2k_element_replace/deepmd/set.000/
--rw-r--r--   0 runner    (1001) docker     (121)      164 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/cp2k/cp2k_element_replace/deepmd/set.000/box.npy
--rw-r--r--   0 runner    (1001) docker     (121)     7340 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/cp2k/cp2k_element_replace/deepmd/set.000/coord.npy
--rw-r--r--   0 runner    (1001) docker     (121)      132 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/cp2k/cp2k_element_replace/deepmd/set.000/energy.npy
--rw-r--r--   0 runner    (1001) docker     (121)     7340 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/cp2k/cp2k_element_replace/deepmd/set.000/force.npy
--rw-r--r--   0 runner    (1001) docker     (121)      164 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/cp2k/cp2k_element_replace/deepmd/set.000/virial.npy
--rw-r--r--   0 runner    (1001) docker     (121)     1202 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/cp2k/cp2k_element_replace/deepmd/type.raw
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/cp2k/cp2k_element_replace/deepmd/type_map.raw
--rw-r--r--   0 runner    (1001) docker     (121)   303494 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/cp2k/cp2k_nocon_output
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.879389 dpdata-0.2.8/tests/cp2k/cp2k_normal_output/
--rw-r--r--   0 runner    (1001) docker     (121)   107587 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/cp2k/cp2k_normal_output/cp2k_output
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.879389 dpdata-0.2.8/tests/cp2k/cp2k_normal_output/deepmd/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.879389 dpdata-0.2.8/tests/cp2k/cp2k_normal_output/deepmd/set.000/
--rw-r--r--   0 runner    (1001) docker     (121)      164 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/cp2k/cp2k_normal_output/deepmd/set.000/box.npy
--rw-r--r--   0 runner    (1001) docker     (121)      488 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/cp2k/cp2k_normal_output/deepmd/set.000/coord.npy
--rw-r--r--   0 runner    (1001) docker     (121)      132 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/cp2k/cp2k_normal_output/deepmd/set.000/energy.npy
--rw-r--r--   0 runner    (1001) docker     (121)      488 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/cp2k/cp2k_normal_output/deepmd/set.000/force.npy
--rw-r--r--   0 runner    (1001) docker     (121)      164 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/cp2k/cp2k_normal_output/deepmd/set.000/virial.npy
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/cp2k/cp2k_normal_output/deepmd/type.raw
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/cp2k/cp2k_normal_output/deepmd/type_map.raw
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.879389 dpdata-0.2.8/tests/fhi_aims/
--rw-r--r--   0 runner    (1001) docker     (121)    65680 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/fhi_aims/out_md
--rw-r--r--   0 runner    (1001) docker     (121)   124362 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/fhi_aims/out_scf
--rw-r--r--   0 runner    (1001) docker     (121)   420506 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/fhi_aims/output_multi_elements
--rw-r--r--   0 runner    (1001) docker     (121)      141 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/fhi_aims/ref_cell.txt
--rw-r--r--   0 runner    (1001) docker     (121)      423 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/fhi_aims/ref_cell_md.txt
--rw-r--r--   0 runner    (1001) docker     (121)      631 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/fhi_aims/ref_cell_md_m.txt
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/fhi_aims/ref_coord.txt
--rw-r--r--   0 runner    (1001) docker     (121)      516 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/fhi_aims/ref_coord_md.txt
--rw-r--r--   0 runner    (1001) docker     (121)    31680 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/fhi_aims/ref_coord_md_m.txt
--rw-r--r--   0 runner    (1001) docker     (121)       99 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/fhi_aims/ref_energy_md.txt
--rw-r--r--   0 runner    (1001) docker     (121)      204 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/fhi_aims/ref_energy_md_m.txt
--rw-r--r--   0 runner    (1001) docker     (121)      170 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/fhi_aims/ref_force.txt
--rw-r--r--   0 runner    (1001) docker     (121)      774 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/fhi_aims/ref_force_md.txt
--rw-r--r--   0 runner    (1001) docker     (121)    44640 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/fhi_aims/ref_force_md_m.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.883389 dpdata-0.2.8/tests/gaussian/
--rw-r--r--   0 runner    (1001) docker     (121)   151758 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/gaussian/aimd_gaussian_CH4_output
--rw-r--r--   0 runner    (1001) docker     (121)  1192096 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/gaussian/largeforce.gaussianlog
--rw-r--r--   0 runner    (1001) docker     (121)    18377 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/gaussian/methane.gaussianlog
--rw-r--r--   0 runner    (1001) docker     (121)    18377 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/gaussian/methane_reordered.gaussianlog
--rw-r--r--   0 runner    (1001) docker     (121)    18166 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/gaussian/methane_sub.gaussianlog
--rw-r--r--   0 runner    (1001) docker     (121)    15547 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/gaussian/noncoveraged.gaussianlog
--rw-r--r--   0 runner    (1001) docker     (121)    68303 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/gaussian/oxygen.gaussianlog
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.883389 dpdata-0.2.8/tests/gromacs/
--rw-r--r--   0 runner    (1001) docker     (121)      469 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/gromacs/1h.gro
--rw-r--r--   0 runner    (1001) docker     (121)      493 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/gromacs/1h.tri.gro
--rw-r--r--   0 runner    (1001) docker     (121)     1573 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/gromacs/case_for_format_atom_name.gro
--rw-r--r--   0 runner    (1001) docker     (121)      952 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/gromacs/multi_frames.gro
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.887389 dpdata-0.2.8/tests/poscars/
--rw-r--r--   0 runner    (1001) docker     (121)   148662 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/poscars/6362_OUTCAR
--rw-r--r--   0 runner    (1001) docker     (121)     1950 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/poscars/CONTCAR.h2o.md
--rw-r--r--   0 runner    (1001) docker     (121)    66878 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/poscars/OUTCAR.Ge.vdw
--rw-r--r--   0 runner    (1001) docker     (121)    31877 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/poscars/OUTCAR.ch4.1step
--rw-r--r--   0 runner    (1001) docker     (121)   144560 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/poscars/OUTCAR.ch4.ml
--rw-r--r--   0 runner    (1001) docker     (121)   130114 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/poscars/OUTCAR.ch4.unconverged
--rw-r--r--   0 runner    (1001) docker     (121)   122105 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/poscars/OUTCAR.h2o.md
--rw-r--r--   0 runner    (1001) docker     (121)   262639 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/poscars/OUTCAR.h2o.md.10
--rw-r--r--   0 runner    (1001) docker     (121)     2931 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/poscars/POSCAR.P42nmc
--rw-r--r--   0 runner    (1001) docker     (121)     4864 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/poscars/POSCAR.P42nmc.replace
--rw-r--r--   0 runner    (1001) docker     (121)      627 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/poscars/POSCAR.SiC
--rw-r--r--   0 runner    (1001) docker     (121)      629 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/poscars/POSCAR.SiC.const
--rw-r--r--   0 runner    (1001) docker     (121)      628 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/poscars/POSCAR.SiC.normal
--rw-r--r--   0 runner    (1001) docker     (121)     2742 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/poscars/POSCAR.SiC.replicate123
--rw-r--r--   0 runner    (1001) docker     (121)      629 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/poscars/POSCAR.SiC.uniform
--rw-r--r--   0 runner    (1001) docker     (121)      219 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/poscars/POSCAR.h2o.md
--rw-r--r--   0 runner    (1001) docker     (121)      242 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/poscars/POSCAR.h4o3
--rw-r--r--   0 runner    (1001) docker     (121)      150 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/poscars/POSCAR.oh.c
--rw-r--r--   0 runner    (1001) docker     (121)      134 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/poscars/POSCAR.oh.d
--rw-r--r--   0 runner    (1001) docker     (121)      155 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/poscars/POSCAR.oh.d.dup
--rw-r--r--   0 runner    (1001) docker     (121)     1120 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/poscars/conf.5.dump
--rw-r--r--   0 runner    (1001) docker     (121)      448 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/poscars/conf.dump
--rw-r--r--   0 runner    (1001) docker     (121)      229 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/poscars/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (121)    14032 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/poscars/conf.waterion.lmp
--rw-r--r--   0 runner    (1001) docker     (121)      475 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/poscars/conf_s_su.dump
--rw-r--r--   0 runner    (1001) docker     (121)      674 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/poscars/conf_unfold.dump
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.887389 dpdata-0.2.8/tests/poscars/deepmd.h2o.md/
--rw-r--r--   0 runner    (1001) docker     (121)      681 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/poscars/deepmd.h2o.md/box.raw
--rw-r--r--   0 runner    (1001) docker     (121)     1350 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/poscars/deepmd.h2o.md/coord.raw
--rw-r--r--   0 runner    (1001) docker     (121)       78 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/poscars/deepmd.h2o.md/energy.raw
--rw-r--r--   0 runner    (1001) docker     (121)     1382 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/poscars/deepmd.h2o.md/force.raw
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/poscars/deepmd.h2o.md/type.raw
--rw-r--r--   0 runner    (1001) docker     (121)      687 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/poscars/deepmd.h2o.md/virial.raw
--rw-r--r--   0 runner    (1001) docker     (121)    10091 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/poscars/h2o.md.json
--rw-r--r--   0 runner    (1001) docker     (121)     1539 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/poscars/poscar_ref_oh.py
--rw-r--r--   0 runner    (1001) docker     (121)      701 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/poscars/shift_origin.dump
--rw-r--r--   0 runner    (1001) docker     (121)      790 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/poscars/test_lammps_dump_s_su.py
--rw-r--r--   0 runner    (1001) docker     (121)    58956 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/poscars/vasprun.Ge.vdw.xml
--rw-r--r--   0 runner    (1001) docker     (121)   108944 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/poscars/vasprun.h2o.md.10.xml
--rw-r--r--   0 runner    (1001) docker     (121)    83635 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/poscars/vasprun.h2o.md.tribox.lower.xml
--rw-r--r--   0 runner    (1001) docker     (121)    82151 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/poscars/vasprun.h2o.md.tribox.xml
--rw-r--r--   0 runner    (1001) docker     (121)    73398 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/poscars/vasprun.h2o.md.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.891389 dpdata-0.2.8/tests/pwmat/
--rw-r--r--   0 runner    (1001) docker     (121)  2137763 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/pwmat/MOVEMENT
--rw-r--r--   0 runner    (1001) docker     (121)     1354 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/pwmat/OUT.MLMD
--rw-r--r--   0 runner    (1001) docker     (121)      447 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/pwmat/atom.config
--rw-r--r--   0 runner    (1001) docker     (121)      279 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/pwmat/atom.config.oh
--rw-r--r--   0 runner    (1001) docker     (121)      229 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/pwmat/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (121)     1972 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/pwmat/config_ref_ch4.py
--rw-r--r--   0 runner    (1001) docker     (121)     1506 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/pwmat/config_ref_oh.py
--rw-r--r--   0 runner    (1001) docker     (121)      174 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/pwmat/mlmd_cell
--rw-r--r--   0 runner    (1001) docker     (121)      350 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/pwmat/mlmd_coord
--rw-r--r--   0 runner    (1001) docker     (121)      350 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/pwmat/mlmd_force
--rw-r--r--   0 runner    (1001) docker     (121)      180 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/pwmat/ref_cell
--rw-r--r--   0 runner    (1001) docker     (121)      365 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/pwmat/ref_coord
--rw-r--r--   0 runner    (1001) docker     (121)      364 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/pwmat/ref_force
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.891389 dpdata-0.2.8/tests/pymatgen_data/
--rw-r--r--   0 runner    (1001) docker     (121)      632 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/pymatgen_data/FA-001.vasp
--rw-r--r--   0 runner    (1001) docker     (121)      614 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/pymatgen_data/FA-001.xyz
--rw-r--r--   0 runner    (1001) docker     (121)      348 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/pymatgen_data/mol2-new.vasp
--rw-r--r--   0 runner    (1001) docker     (121)      823 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/pymatgen_data/mol2.vasp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.891389 dpdata-0.2.8/tests/qe.scf/
--rw-r--r--   0 runner    (1001) docker     (121)      576 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/qe.scf/01.in
--rw-r--r--   0 runner    (1001) docker     (121)    12346 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/qe.scf/01.out
--rw-r--r--   0 runner    (1001) docker     (121)     6197 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/qe.scf/02.in
--rw-r--r--   0 runner    (1001) docker     (121)    45800 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/qe.scf/02.out
--rwxr-xr-x   0 runner    (1001) docker     (121)      829 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/qe.scf/Al.in
--rw-r--r--   0 runner    (1001) docker     (121)    21583 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/qe.scf/Al.out
--rw-r--r--   0 runner    (1001) docker     (121)      375 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/qe.scf/ch4_coord
--rw-r--r--   0 runner    (1001) docker     (121)      381 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/qe.scf/ch4_force
--rw-r--r--   0 runner    (1001) docker     (121)      228 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/qe.scf/ch4_virial
--rw-r--r--   0 runner    (1001) docker     (121)      226 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/qe.scf/h2o_cell
--rw-r--r--   0 runner    (1001) docker     (121)    14402 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/qe.scf/h2o_coord
--rw-r--r--   0 runner    (1001) docker     (121)    14706 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/qe.scf/h2o_force
--rw-r--r--   0 runner    (1001) docker     (121)      229 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/qe.scf/h2o_virial
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.895389 dpdata-0.2.8/tests/qe.traj/
--rw-r--r--   0 runner    (1001) docker     (121)      344 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/qe.traj/oh-md.evp
--rw-r--r--   0 runner    (1001) docker     (121)    29072 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/qe.traj/oh-md.for
--rw-r--r--   0 runner    (1001) docker     (121)    10435 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/qe.traj/oh-md.in
--rw-r--r--   0 runner    (1001) docker     (121)    29072 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/qe.traj/oh-md.pos
--rw-r--r--   0 runner    (1001) docker     (121)      960 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/qe.traj/traj6.cel
--rw-r--r--   0 runner    (1001) docker     (121)     1048 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/qe.traj/traj6.evp
--rw-r--r--   0 runner    (1001) docker     (121)     1020 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/qe.traj/traj6.for
--rw-r--r--   0 runner    (1001) docker     (121)     1550 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/qe.traj/traj6.in
--rw-r--r--   0 runner    (1001) docker     (121)     1032 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/qe.traj/traj6.pos
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.803388 dpdata-0.2.8/tests/siesta/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.895389 dpdata-0.2.8/tests/siesta/aimd/
--rw-r--r--   0 runner    (1001) docker     (121)      650 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/siesta/aimd/cell
--rw-r--r--   0 runner    (1001) docker     (121)    13800 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/siesta/aimd/coord
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/siesta/aimd/energy
--rw-r--r--   0 runner    (1001) docker     (121)    11532 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/siesta/aimd/force
--rw-r--r--   0 runner    (1001) docker     (121)    66496 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/siesta/aimd/output
--rw-r--r--   0 runner    (1001) docker     (121)      684 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/siesta/aimd/virial
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.895389 dpdata-0.2.8/tests/siesta/scf/
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/siesta/scf/ref_cell
--rw-r--r--   0 runner    (1001) docker     (121)      215 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/siesta/scf/ref_coord
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/siesta/scf/ref_energy
--rw-r--r--   0 runner    (1001) docker     (121)      185 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/siesta/scf/ref_force
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/siesta/scf/ref_virial
--rw-r--r--   0 runner    (1001) docker     (121)    23640 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/siesta/scf/siesta_output
--rw-r--r--   0 runner    (1001) docker     (121)     4840 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/test_abacus_md.py
--rw-r--r--   0 runner    (1001) docker     (121)     4863 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/test_abacus_pw_scf.py
--rw-r--r--   0 runner    (1001) docker     (121)     2694 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/test_abacus_relax.py
--rw-r--r--   0 runner    (1001) docker     (121)      665 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/test_abacus_stru_dump.py
--rw-r--r--   0 runner    (1001) docker     (121)     1447 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/test_amber_md.py
--rw-r--r--   0 runner    (1001) docker     (121)     2550 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/test_amber_sqm.py
--rw-r--r--   0 runner    (1001) docker     (121)     1539 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/test_ase_traj.py
--rw-r--r--   0 runner    (1001) docker     (121)     5233 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/test_bond_order_system.py
--rw-r--r--   0 runner    (1001) docker     (121)     1954 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/test_cell_to_low_triangle.py
--rw-r--r--   0 runner    (1001) docker     (121)      544 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     1616 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/test_corr.py
--rw-r--r--   0 runner    (1001) docker     (121)     1676 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/test_cp2k_aimd_output.py
--rw-r--r--   0 runner    (1001) docker     (121)     2151 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/test_cp2k_output.py
--rw-r--r--   0 runner    (1001) docker     (121)     3535 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/test_deepmd_comp.py
--rw-r--r--   0 runner    (1001) docker     (121)     2761 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/test_deepmd_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (121)     8103 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/test_deepmd_raw.py
--rw-r--r--   0 runner    (1001) docker     (121)      813 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/test_elements_index.py
--rw-r--r--   0 runner    (1001) docker     (121)     1083 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/test_empty.py
--rw-r--r--   0 runner    (1001) docker     (121)     1896 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/test_fhi_md_multi_elem_output.py
--rw-r--r--   0 runner    (1001) docker     (121)     1859 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/test_fhi_md_output.py
--rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/test_fhi_output.py
--rw-r--r--   0 runner    (1001) docker     (121)     4154 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/test_gaussian_driver.py
--rw-r--r--   0 runner    (1001) docker     (121)     2706 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/test_gaussian_log.py
--rw-r--r--   0 runner    (1001) docker     (121)     5606 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/test_gromacs_gro.py
--rw-r--r--   0 runner    (1001) docker     (121)      962 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/test_json.py
--rw-r--r--   0 runner    (1001) docker     (121)      453 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/test_lammps_dump_shift_origin.py
--rw-r--r--   0 runner    (1001) docker     (121)      834 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/test_lammps_dump_skipload.py
--rw-r--r--   0 runner    (1001) docker     (121)      780 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/test_lammps_dump_to_system.py
--rw-r--r--   0 runner    (1001) docker     (121)      794 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/test_lammps_dump_unfold.py
--rw-r--r--   0 runner    (1001) docker     (121)      985 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/test_lammps_lmp_dump.py
--rw-r--r--   0 runner    (1001) docker     (121)      435 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/test_lammps_lmp_to_system.py
--rw-r--r--   0 runner    (1001) docker     (121)     1600 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/test_msd.py
--rw-r--r--   0 runner    (1001) docker     (121)     6138 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/test_multisystems.py
--rw-r--r--   0 runner    (1001) docker     (121)      772 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/test_periodic_table.py
--rw-r--r--   0 runner    (1001) docker     (121)     5282 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/test_perturb.py
--rw-r--r--   0 runner    (1001) docker     (121)     1389 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/test_pick_atom_idx.py
--rw-r--r--   0 runner    (1001) docker     (121)     3211 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/test_predict.py
--rw-r--r--   0 runner    (1001) docker     (121)     1887 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/test_pwmat_config_dump.py
--rw-r--r--   0 runner    (1001) docker     (121)      963 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/test_pwmat_config_to_system.py
--rw-r--r--   0 runner    (1001) docker     (121)     1870 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/test_pwmat_mlmd.py
--rw-r--r--   0 runner    (1001) docker     (121)     2061 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/test_pwmat_movement.py
--rw-r--r--   0 runner    (1001) docker     (121)     1291 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/test_pymatgen_molecule.py
--rw-r--r--   0 runner    (1001) docker     (121)     2321 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/test_qe_cp_traj.py
--rw-r--r--   0 runner    (1001) docker     (121)     2636 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/test_qe_cp_traj_skipload.py
--rw-r--r--   0 runner    (1001) docker     (121)     4767 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/test_qe_pw_scf.py
--rw-r--r--   0 runner    (1001) docker     (121)      869 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/test_qe_pw_scf_crystal_atomic_positions.py
--rw-r--r--   0 runner    (1001) docker     (121)      694 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/test_qe_pw_scf_energy_bug.py
--rw-r--r--   0 runner    (1001) docker     (121)     3979 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/test_quip_gap_xyz.py
--rw-r--r--   0 runner    (1001) docker     (121)      582 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/test_remove_atom_names.py
--rw-r--r--   0 runner    (1001) docker     (121)     1410 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/test_remove_pbc.py
--rw-r--r--   0 runner    (1001) docker     (121)     1370 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/test_replace.py
--rw-r--r--   0 runner    (1001) docker     (121)      817 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/test_replicate.py
--rw-r--r--   0 runner    (1001) docker     (121)      768 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/test_shuffle.py
--rw-r--r--   0 runner    (1001) docker     (121)     3090 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/test_siesta_aiMD_output.py
--rw-r--r--   0 runner    (1001) docker     (121)     3004 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/test_siesta_output.py
--rw-r--r--   0 runner    (1001) docker     (121)     1055 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/test_sqm_driver.py
--rw-r--r--   0 runner    (1001) docker     (121)     1137 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/test_stat.py
--rw-r--r--   0 runner    (1001) docker     (121)     1841 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/test_system_append.py
--rw-r--r--   0 runner    (1001) docker     (121)     1077 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/test_system_apply_pbc.py
--rw-r--r--   0 runner    (1001) docker     (121)     1387 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/test_system_set_type.py
--rw-r--r--   0 runner    (1001) docker     (121)     1478 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/test_to_ase.py
--rw-r--r--   0 runner    (1001) docker     (121)      570 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/test_to_list.py
--rw-r--r--   0 runner    (1001) docker     (121)      777 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/test_to_pymatgen.py
--rw-r--r--   0 runner    (1001) docker     (121)      974 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/test_to_pymatgen_entry.py
--rw-r--r--   0 runner    (1001) docker     (121)     1292 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/test_type_map.py
--rw-r--r--   0 runner    (1001) docker     (121)     4172 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/test_vasp_outcar.py
--rw-r--r--   0 runner    (1001) docker     (121)     1861 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/test_vasp_poscar_dump.py
--rw-r--r--   0 runner    (1001) docker     (121)     1863 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/test_vasp_poscar_to_system.py
--rw-r--r--   0 runner    (1001) docker     (121)      761 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/test_vasp_unconverged_outcar.py
--rw-r--r--   0 runner    (1001) docker     (121)     1639 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/test_vasp_xml.py
--rw-r--r--   0 runner    (1001) docker     (121)     2206 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/test_water_ions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1406 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/test_xyz.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.895389 dpdata-0.2.8/tests/xyz/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.895389 dpdata-0.2.8/tests/xyz/B1C9/
--rw-r--r--   0 runner    (1001) docker     (121)      450 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/xyz/B1C9/box.raw
--rw-r--r--   0 runner    (1001) docker     (121)     1500 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/xyz/B1C9/coord.raw
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/xyz/B1C9/energy.raw
--rw-r--r--   0 runner    (1001) docker     (121)     1533 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/xyz/B1C9/force.raw
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/xyz/B1C9/type.raw
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/xyz/B1C9/type_map.raw
--rw-r--r--   0 runner    (1001) docker     (121)      457 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/xyz/B1C9/virial.raw
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.899389 dpdata-0.2.8/tests/xyz/B5C7/
--rw-r--r--   0 runner    (1001) docker     (121)      225 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/xyz/B5C7/box.raw
--rw-r--r--   0 runner    (1001) docker     (121)      900 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/xyz/B5C7/coord.raw
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/xyz/B5C7/energy.raw
--rw-r--r--   0 runner    (1001) docker     (121)      918 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/xyz/B5C7/force.raw
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/xyz/B5C7/type.raw
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/xyz/B5C7/type_map.raw
--rw-r--r--   0 runner    (1001) docker     (121)      225 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/xyz/B5C7/virial.raw
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:44.899389 dpdata-0.2.8/tests/xyz/B5C7_novirials/
--rw-r--r--   0 runner    (1001) docker     (121)      225 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/xyz/B5C7_novirials/box.raw
--rw-r--r--   0 runner    (1001) docker     (121)      900 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/xyz/B5C7_novirials/coord.raw
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/xyz/B5C7_novirials/energy.raw
--rw-r--r--   0 runner    (1001) docker     (121)      918 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/xyz/B5C7_novirials/force.raw
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/xyz/B5C7_novirials/type.raw
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/xyz/B5C7_novirials/type_map.raw
--rw-r--r--   0 runner    (1001) docker     (121)     1436 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/xyz/xyz_B5C7_novirials.xyz
--rw-r--r--   0 runner    (1001) docker     (121)     4440 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/xyz/xyz_unittest.field.xyz
--rw-r--r--   0 runner    (1001) docker     (121)     4413 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/xyz/xyz_unittest.sort.xyz
--rw-r--r--   0 runner    (1001) docker     (121)     4413 2022-08-03 03:14:32.000000 dpdata-0.2.8/tests/xyz/xyz_unittest.xyz
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.106610 dpdata-0.2.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:06.994610 dpdata-0.2.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.002610 dpdata-0.2.9/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)     1330 2022-10-03 02:58:54.000000 dpdata-0.2.9/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1077 2022-10-03 02:58:54.000000 dpdata-0.2.9/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (121)      404 2022-10-03 02:58:54.000000 dpdata-0.2.9/.github/ISSUE_TEMPLATE/generic-issue.md
+-rw-r--r--   0 runner    (1001) docker     (121)      663 2022-10-03 02:58:54.000000 dpdata-0.2.9/.github/ISSUE_TEMPLATE/request-for-help.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.002610 dpdata-0.2.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)      570 2022-10-03 02:58:54.000000 dpdata-0.2.9/.github/workflows/mirror_gitee.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      846 2022-10-03 02:58:54.000000 dpdata-0.2.9/.github/workflows/pub-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      793 2022-10-03 02:58:54.000000 dpdata-0.2.9/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      339 2022-10-03 02:58:54.000000 dpdata-0.2.9/.github/workflows/test_import.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      261 2022-10-03 02:58:54.000000 dpdata-0.2.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     7652 2022-10-03 02:58:54.000000 dpdata-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)    14088 2022-10-03 02:59:07.106610 dpdata-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    13533 2022-10-03 02:58:54.000000 dpdata-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.002610 dpdata-0.2.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)      603 2022-10-03 02:58:54.000000 dpdata-0.2.9/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)      125 2022-10-03 02:58:54.000000 dpdata-0.2.9/docs/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     5917 2022-10-03 02:58:54.000000 dpdata-0.2.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      152 2022-10-03 02:58:54.000000 dpdata-0.2.9/docs/formats.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      492 2022-10-03 02:58:54.000000 dpdata-0.2.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2851 2022-10-03 02:58:54.000000 dpdata-0.2.9/docs/make_format.py
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2022-10-03 02:58:54.000000 dpdata-0.2.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.006610 dpdata-0.2.9/dpdata/
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      516 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      176 2022-10-03 02:59:06.000000 dpdata-0.2.9/dpdata/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.006610 dpdata-0.2.9/dpdata/abacus/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/abacus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6063 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/abacus/md.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5256 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/abacus/relax.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10603 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/abacus/scf.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.006610 dpdata-0.2.9/dpdata/amber/
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/amber/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      972 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/amber/mask.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4637 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/amber/md.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3803 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/amber/sqm.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2460 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/ase_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6978 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/bond_order_system.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2689 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.006610 dpdata-0.2.9/dpdata/cp2k/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/cp2k/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2105 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/cp2k/cell.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18230 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/cp2k/output.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.006610 dpdata-0.2.9/dpdata/deepmd/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/deepmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5109 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/deepmd/comp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5145 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/deepmd/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3971 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/deepmd/raw.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4081 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.006610 dpdata-0.2.9/dpdata/fhi_aims/
+-rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/fhi_aims/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     5210 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/fhi_aims/output.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3393 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/format.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.010610 dpdata-0.2.9/dpdata/gaussian/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/gaussian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8126 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/gaussian/gjf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2686 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/gaussian/log.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.010610 dpdata-0.2.9/dpdata/gromacs/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/gromacs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3311 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/gromacs/gro.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.010610 dpdata-0.2.9/dpdata/lammps/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/lammps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7217 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/lammps/dump.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6227 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/lammps/lmp.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.010610 dpdata-0.2.9/dpdata/md/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/md/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1824 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/md/msd.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1887 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/md/pbc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4251 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/md/rdf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7072 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/md/water.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18474 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/periodic_table.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1774 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/periodic_table.py
+-rw-r--r--   0 runner    (1001) docker     (121)      747 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.014610 dpdata-0.2.9/dpdata/plugins/
+-rw-r--r--   0 runner    (1001) docker     (121)      599 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2299 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/plugins/abacus.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4567 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/plugins/amber.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6560 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/plugins/ase.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1017 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/plugins/cp2k.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10446 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/plugins/deepmd.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/plugins/dftbplus.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1271 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/plugins/fhi_aims.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3371 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/plugins/gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1493 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/plugins/gromacs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1404 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/plugins/lammps.py
+-rw-r--r--   0 runner    (1001) docker     (121)      660 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/plugins/list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2076 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/plugins/pwmat.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2847 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/plugins/pymatgen.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1653 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/plugins/qe.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1469 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/plugins/rdkit.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1822 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/plugins/siesta.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3846 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/plugins/vasp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1483 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/plugins/xyz.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.014610 dpdata-0.2.9/dpdata/pwmat/
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/pwmat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3408 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/pwmat/atomconfig.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6540 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/pwmat/movement.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.014610 dpdata-0.2.9/dpdata/pymatgen/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/pymatgen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      938 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/pymatgen/molecule.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.014610 dpdata-0.2.9/dpdata/qe/
+-rw-r--r--   0 runner    (1001) docker     (121)        2 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/qe/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     5108 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/qe/scf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7546 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/qe/traj.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.014610 dpdata-0.2.9/dpdata/rdkit/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/rdkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24936 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/rdkit/sanitize.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4220 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/rdkit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.014610 dpdata-0.2.9/dpdata/siesta/
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/siesta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5070 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/siesta/aiMD_output.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4175 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/siesta/output.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3983 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/stat.py
+-rw-r--r--   0 runner    (1001) docker     (121)    53253 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/system.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5114 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/unit.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3347 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.014610 dpdata-0.2.9/dpdata/vasp/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/vasp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5268 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/vasp/outcar.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2872 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/vasp/poscar.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3834 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/vasp/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.014610 dpdata-0.2.9/dpdata/xyz/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/xyz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5937 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/xyz/quip_gap_xyz.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1309 2022-10-03 02:58:54.000000 dpdata-0.2.9/dpdata/xyz/xyz.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.006610 dpdata-0.2.9/dpdata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    14088 2022-10-03 02:59:06.000000 dpdata-0.2.9/dpdata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    17852 2022-10-03 02:59:06.000000 dpdata-0.2.9/dpdata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-03 02:59:06.000000 dpdata-0.2.9/dpdata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2022-10-03 02:59:06.000000 dpdata-0.2.9/dpdata.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      243 2022-10-03 02:59:06.000000 dpdata-0.2.9/dpdata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      235 2022-10-03 02:59:06.000000 dpdata-0.2.9/dpdata.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.014610 dpdata-0.2.9/plugin_example/
+-rw-r--r--   0 runner    (1001) docker     (121)      277 2022-10-03 02:58:54.000000 dpdata-0.2.9/plugin_example/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.014610 dpdata-0.2.9/plugin_example/dpdata_random/
+-rw-r--r--   0 runner    (1001) docker     (121)      869 2022-10-03 02:58:54.000000 dpdata-0.2.9/plugin_example/dpdata_random/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      251 2022-10-03 02:58:54.000000 dpdata-0.2.9/plugin_example/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)       33 2022-10-03 02:58:54.000000 dpdata-0.2.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-03 02:59:07.106610 dpdata-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2035 2022-10-03 02:58:54.000000 dpdata-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.026610 dpdata-0.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      673 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/POSCAR
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.026610 dpdata-0.2.9/tests/abacus.md/
+-rw-r--r--   0 runner    (1001) docker     (121)      907 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/abacus.md/INPUT
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.030610 dpdata-0.2.9/tests/abacus.md/OUT.abacus/
+-rw-r--r--   0 runner    (1001) docker     (121)     4043 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/abacus.md/OUT.abacus/MD_dump
+-rw-r--r--   0 runner    (1001) docker     (121)    88365 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/abacus.md/OUT.abacus/running_md.log
+-rw-r--r--   0 runner    (1001) docker     (121)      458 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/abacus.md/STRU
+-rw-r--r--   0 runner    (1001) docker     (121)      523 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/abacus.md/water_coord
+-rw-r--r--   0 runner    (1001) docker     (121)      711 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/abacus.md/water_force
+-rw-r--r--   0 runner    (1001) docker     (121)      710 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/abacus.md/water_virial
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.026610 dpdata-0.2.9/tests/abacus.md.nostress/
+-rw-r--r--   0 runner    (1001) docker     (121)      416 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/abacus.md.nostress/INPUT
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.030610 dpdata-0.2.9/tests/abacus.md.nostress/OUT.autotest/
+-rw-r--r--   0 runner    (1001) docker     (121)     1888 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/abacus.md.nostress/OUT.autotest/MD_dump
+-rw-r--r--   0 runner    (1001) docker     (121)    21769 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/abacus.md.nostress/OUT.autotest/running_md.log
+-rw-r--r--   0 runner    (1001) docker     (121)      303 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/abacus.md.nostress/STRU
+-rw-r--r--   0 runner    (1001) docker     (121)      234 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/abacus.md.nostress/Si_coord
+-rw-r--r--   0 runner    (1001) docker     (121)      283 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/abacus.md.nostress/Si_force
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.030610 dpdata-0.2.9/tests/abacus.relax/
+-rw-r--r--   0 runner    (1001) docker     (121)      603 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/abacus.relax/INPUT
+-rw-r--r--   0 runner    (1001) docker     (121)       29 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/abacus.relax/KPT
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.034610 dpdata-0.2.9/tests/abacus.relax/OUT.abacus/
+-rw-r--r--   0 runner    (1001) docker     (121)    12748 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/abacus.relax/OUT.abacus/INPUT
+-rw-r--r--   0 runner    (1001) docker     (121)      468 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/abacus.relax/OUT.abacus/STRU_ION_D
+-rw-r--r--   0 runner    (1001) docker     (121)      409 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/abacus.relax/OUT.abacus/STRU_READIN_ADJUST.cif
+-rw-r--r--   0 runner    (1001) docker     (121)    54773 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/abacus.relax/OUT.abacus/running_cell-relax.log
+-rw-r--r--   0 runner    (1001) docker     (121)      482 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/abacus.relax/STRU
+-rw-r--r--   0 runner    (1001) docker     (121)      810 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/abacus.relax/coord.ref
+-rw-r--r--   0 runner    (1001) docker     (121)      810 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/abacus.relax/force.ref
+-rw-r--r--   0 runner    (1001) docker     (121)      810 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/abacus.relax/stress.ref
+-rw-r--r--   0 runner    (1001) docker     (121)      810 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/abacus.relax/virial.ref
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.034610 dpdata-0.2.9/tests/abacus.scf/
+-rw-r--r--   0 runner    (1001) docker     (121)      455 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/abacus.scf/INPUT
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.034610 dpdata-0.2.9/tests/abacus.scf/OUT.ch4/
+-rw-r--r--   0 runner    (1001) docker     (121)    26715 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/abacus.scf/OUT.ch4/running_scf.log
+-rw-r--r--   0 runner    (1001) docker     (121)      743 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/abacus.scf/STRU.ch4
+-rw-r--r--   0 runner    (1001) docker     (121)      164 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/abacus.scf/ch4_coord
+-rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/abacus.scf/ch4_force
+-rw-r--r--   0 runner    (1001) docker     (121)      106 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/abacus.scf/ch4_virial
+-rw-r--r--   0 runner    (1001) docker     (121)      580 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/abacus.scf/stru_test
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.038610 dpdata-0.2.9/tests/amber/
+-rw-r--r--   0 runner    (1001) docker     (121)     8237 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/amber/02_Heat.mden
+-rw-r--r--   0 runner    (1001) docker     (121)   229960 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/amber/02_Heat.mdfrc
+-rw-r--r--   0 runner    (1001) docker     (121)   230760 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/amber/02_Heat.nc
+-rw-r--r--   0 runner    (1001) docker     (121)   321683 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/amber/02_Heat.parm7
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.042610 dpdata-0.2.9/tests/amber/corr/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:06.994610 dpdata-0.2.9/tests/amber/corr/dataset/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.042610 dpdata-0.2.9/tests/amber/corr/dataset/C6H11HW192O6OW96P1/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/amber/corr/dataset/C6H11HW192O6OW96P1/nopbc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.046610 dpdata-0.2.9/tests/amber/corr/dataset/C6H11HW192O6OW96P1/set.000/
+-rw-r--r--   0 runner    (1001) docker     (121)      164 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/amber/corr/dataset/C6H11HW192O6OW96P1/set.000/box.npy
+-rw-r--r--   0 runner    (1001) docker     (121)     3872 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/amber/corr/dataset/C6H11HW192O6OW96P1/set.000/coord.npy
+-rw-r--r--   0 runner    (1001) docker     (121)      132 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/amber/corr/dataset/C6H11HW192O6OW96P1/set.000/energy.npy
+-rw-r--r--   0 runner    (1001) docker     (121)     3872 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/amber/corr/dataset/C6H11HW192O6OW96P1/set.000/force.npy
+-rw-r--r--   0 runner    (1001) docker     (121)      624 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/amber/corr/dataset/C6H11HW192O6OW96P1/type.raw
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/amber/corr/dataset/C6H11HW192O6OW96P1/type_map.raw
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:06.994610 dpdata-0.2.9/tests/amber/corr/dp_amber_mask/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.046610 dpdata-0.2.9/tests/amber/corr/dp_amber_mask/C6EP0H11HW192O6OW96P1/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/amber/corr/dp_amber_mask/C6EP0H11HW192O6OW96P1/nopbc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.046610 dpdata-0.2.9/tests/amber/corr/dp_amber_mask/C6EP0H11HW192O6OW96P1/set.000/
+-rw-r--r--   0 runner    (1001) docker     (121)      164 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/amber/corr/dp_amber_mask/C6EP0H11HW192O6OW96P1/set.000/box.npy
+-rw-r--r--   0 runner    (1001) docker     (121)     3872 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/amber/corr/dp_amber_mask/C6EP0H11HW192O6OW96P1/set.000/coord.npy
+-rw-r--r--   0 runner    (1001) docker     (121)      132 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/amber/corr/dp_amber_mask/C6EP0H11HW192O6OW96P1/set.000/energy.npy
+-rw-r--r--   0 runner    (1001) docker     (121)     3872 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/amber/corr/dp_amber_mask/C6EP0H11HW192O6OW96P1/set.000/force.npy
+-rw-r--r--   0 runner    (1001) docker     (121)      624 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/amber/corr/dp_amber_mask/C6EP0H11HW192O6OW96P1/type.raw
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/amber/corr/dp_amber_mask/C6EP0H11HW192O6OW96P1/type_map.raw
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.046610 dpdata-0.2.9/tests/amber/corr/dp_corr/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.046610 dpdata-0.2.9/tests/amber/corr/dp_corr/set.000/
+-rw-r--r--   0 runner    (1001) docker     (121)      164 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/amber/corr/dp_corr/set.000/box.npy
+-rw-r--r--   0 runner    (1001) docker     (121)    72896 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/amber/corr/dp_corr/set.000/coord.npy
+-rw-r--r--   0 runner    (1001) docker     (121)      132 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/amber/corr/dp_corr/set.000/energy.npy
+-rw-r--r--   0 runner    (1001) docker     (121)    72896 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/amber/corr/dp_corr/set.000/force.npy
+-rw-r--r--   0 runner    (1001) docker     (121)    12128 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/amber/corr/dp_corr/type.raw
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/amber/corr/dp_corr/type_map.raw
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.046610 dpdata-0.2.9/tests/amber/corr/dp_hl/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.046610 dpdata-0.2.9/tests/amber/corr/dp_hl/set.000/
+-rw-r--r--   0 runner    (1001) docker     (121)      164 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/amber/corr/dp_hl/set.000/box.npy
+-rw-r--r--   0 runner    (1001) docker     (121)    72896 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/amber/corr/dp_hl/set.000/coord.npy
+-rw-r--r--   0 runner    (1001) docker     (121)      132 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/amber/corr/dp_hl/set.000/energy.npy
+-rw-r--r--   0 runner    (1001) docker     (121)    72896 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/amber/corr/dp_hl/set.000/force.npy
+-rw-r--r--   0 runner    (1001) docker     (121)    12128 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/amber/corr/dp_hl/type.raw
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/amber/corr/dp_hl/type_map.raw
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.050610 dpdata-0.2.9/tests/amber/corr/dp_ll/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.050610 dpdata-0.2.9/tests/amber/corr/dp_ll/set.000/
+-rw-r--r--   0 runner    (1001) docker     (121)      164 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/amber/corr/dp_ll/set.000/box.npy
+-rw-r--r--   0 runner    (1001) docker     (121)    72896 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/amber/corr/dp_ll/set.000/coord.npy
+-rw-r--r--   0 runner    (1001) docker     (121)      132 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/amber/corr/dp_ll/set.000/energy.npy
+-rw-r--r--   0 runner    (1001) docker     (121)    72896 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/amber/corr/dp_ll/set.000/force.npy
+-rw-r--r--   0 runner    (1001) docker     (121)    12128 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/amber/corr/dp_ll/type.raw
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/amber/corr/dp_ll/type_map.raw
+-rw-r--r--   0 runner    (1001) docker     (121)    73252 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/amber/corr/high_level.mdfrc
+-rw-r--r--   0 runner    (1001) docker     (121)    27097 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/amber/corr/high_level.mdout
+-rw-r--r--   0 runner    (1001) docker     (121)    73252 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/amber/corr/low_level.mdfrc
+-rw-r--r--   0 runner    (1001) docker     (121)    27017 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/amber/corr/low_level.mdout
+-rw-r--r--   0 runner    (1001) docker     (121)  1036937 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/amber/corr/qmmm.parm7
+-rw-r--r--   0 runner    (1001) docker     (121)    97988 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/amber/corr/rc.nc
+-rw-r--r--   0 runner    (1001) docker     (121)      474 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/amber/methane.mol
+-rw-r--r--   0 runner    (1001) docker     (121)      407 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/amber/sqm.in
+-rw-r--r--   0 runner    (1001) docker     (121)    25413 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/amber/sqm_forces.out
+-rw-r--r--   0 runner    (1001) docker     (121)     6224 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/amber/sqm_no_forces.out
+-rw-r--r--   0 runner    (1001) docker     (121)    46476 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/amber/sqm_opt.out
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.050610 dpdata-0.2.9/tests/ase_traj/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.050610 dpdata-0.2.9/tests/ase_traj/Al0He4O0/
+-rw-r--r--   0 runner    (1001) docker     (121)      228 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/ase_traj/Al0He4O0/box.raw
+-rw-r--r--   0 runner    (1001) docker     (121)      300 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/ase_traj/Al0He4O0/coord.raw
+-rw-r--r--   0 runner    (1001) docker     (121)       25 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/ase_traj/Al0He4O0/energy.raw
+-rw-r--r--   0 runner    (1001) docker     (121)      306 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/ase_traj/Al0He4O0/force.raw
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/ase_traj/Al0He4O0/type.raw
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/ase_traj/Al0He4O0/type_map.raw
+-rw-r--r--   0 runner    (1001) docker     (121)      229 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/ase_traj/Al0He4O0/virial.raw
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.050610 dpdata-0.2.9/tests/ase_traj/Al2He1O3/
+-rw-r--r--   0 runner    (1001) docker     (121)      225 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/ase_traj/Al2He1O3/box.raw
+-rw-r--r--   0 runner    (1001) docker     (121)      450 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/ase_traj/Al2He1O3/coord.raw
+-rw-r--r--   0 runner    (1001) docker     (121)       25 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/ase_traj/Al2He1O3/energy.raw
+-rw-r--r--   0 runner    (1001) docker     (121)      461 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/ase_traj/Al2He1O3/force.raw
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/ase_traj/Al2He1O3/type.raw
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/ase_traj/Al2He1O3/type_map.raw
+-rw-r--r--   0 runner    (1001) docker     (121)      225 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/ase_traj/Al2He1O3/virial.raw
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.050610 dpdata-0.2.9/tests/ase_traj/Al2He2O3/
+-rw-r--r--   0 runner    (1001) docker     (121)      226 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/ase_traj/Al2He2O3/box.raw
+-rw-r--r--   0 runner    (1001) docker     (121)      525 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/ase_traj/Al2He2O3/coord.raw
+-rw-r--r--   0 runner    (1001) docker     (121)       25 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/ase_traj/Al2He2O3/energy.raw
+-rw-r--r--   0 runner    (1001) docker     (121)      536 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/ase_traj/Al2He2O3/force.raw
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/ase_traj/Al2He2O3/type.raw
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/ase_traj/Al2He2O3/type_map.raw
+-rw-r--r--   0 runner    (1001) docker     (121)      227 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/ase_traj/Al2He2O3/virial.raw
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.054610 dpdata-0.2.9/tests/ase_traj/Al4He0O6/
+-rw-r--r--   0 runner    (1001) docker     (121)      227 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/ase_traj/Al4He0O6/box.raw
+-rw-r--r--   0 runner    (1001) docker     (121)      750 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/ase_traj/Al4He0O6/coord.raw
+-rw-r--r--   0 runner    (1001) docker     (121)       25 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/ase_traj/Al4He0O6/energy.raw
+-rw-r--r--   0 runner    (1001) docker     (121)      767 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/ase_traj/Al4He0O6/force.raw
+-rw-r--r--   0 runner    (1001) docker     (121)       20 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/ase_traj/Al4He0O6/type.raw
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/ase_traj/Al4He0O6/type_map.raw
+-rw-r--r--   0 runner    (1001) docker     (121)      225 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/ase_traj/Al4He0O6/virial.raw
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.054610 dpdata-0.2.9/tests/ase_traj/Al4He2O6/
+-rw-r--r--   0 runner    (1001) docker     (121)      225 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/ase_traj/Al4He2O6/box.raw
+-rw-r--r--   0 runner    (1001) docker     (121)      900 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/ase_traj/Al4He2O6/coord.raw
+-rw-r--r--   0 runner    (1001) docker     (121)       25 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/ase_traj/Al4He2O6/energy.raw
+-rw-r--r--   0 runner    (1001) docker     (121)      911 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/ase_traj/Al4He2O6/force.raw
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/ase_traj/Al4He2O6/type.raw
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/ase_traj/Al4He2O6/type_map.raw
+-rw-r--r--   0 runner    (1001) docker     (121)      225 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/ase_traj/Al4He2O6/virial.raw
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.054610 dpdata-0.2.9/tests/ase_traj/Al4He4O6/
+-rw-r--r--   0 runner    (1001) docker     (121)      227 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/ase_traj/Al4He4O6/box.raw
+-rw-r--r--   0 runner    (1001) docker     (121)     1050 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/ase_traj/Al4He4O6/coord.raw
+-rw-r--r--   0 runner    (1001) docker     (121)       25 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/ase_traj/Al4He4O6/energy.raw
+-rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/ase_traj/Al4He4O6/force.raw
+-rw-r--r--   0 runner    (1001) docker     (121)       28 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/ase_traj/Al4He4O6/type.raw
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/ase_traj/Al4He4O6/type_map.raw
+-rw-r--r--   0 runner    (1001) docker     (121)      227 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/ase_traj/Al4He4O6/virial.raw
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.054610 dpdata-0.2.9/tests/ase_traj/Al8He0O12/
+-rw-r--r--   0 runner    (1001) docker     (121)      678 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/ase_traj/Al8He0O12/box.raw
+-rw-r--r--   0 runner    (1001) docker     (121)     4500 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/ase_traj/Al8He0O12/coord.raw
+-rw-r--r--   0 runner    (1001) docker     (121)       75 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/ase_traj/Al8He0O12/energy.raw
+-rw-r--r--   0 runner    (1001) docker     (121)     4593 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/ase_traj/Al8He0O12/force.raw
+-rw-r--r--   0 runner    (1001) docker     (121)       40 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/ase_traj/Al8He0O12/type.raw
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/ase_traj/Al8He0O12/type_map.raw
+-rw-r--r--   0 runner    (1001) docker     (121)      679 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/ase_traj/Al8He0O12/virial.raw
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.058610 dpdata-0.2.9/tests/ase_traj/Al8He4O12/
+-rw-r--r--   0 runner    (1001) docker     (121)      227 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/ase_traj/Al8He4O12/box.raw
+-rw-r--r--   0 runner    (1001) docker     (121)     1800 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/ase_traj/Al8He4O12/coord.raw
+-rw-r--r--   0 runner    (1001) docker     (121)       25 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/ase_traj/Al8He4O12/energy.raw
+-rw-r--r--   0 runner    (1001) docker     (121)     1836 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/ase_traj/Al8He4O12/force.raw
+-rw-r--r--   0 runner    (1001) docker     (121)       48 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/ase_traj/Al8He4O12/type.raw
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/ase_traj/Al8He4O12/type_map.raw
+-rw-r--r--   0 runner    (1001) docker     (121)      227 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/ase_traj/Al8He4O12/virial.raw
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.058610 dpdata-0.2.9/tests/ase_traj/Al8He8O12/
+-rw-r--r--   0 runner    (1001) docker     (121)      225 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/ase_traj/Al8He8O12/box.raw
+-rw-r--r--   0 runner    (1001) docker     (121)     2100 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/ase_traj/Al8He8O12/coord.raw
+-rw-r--r--   0 runner    (1001) docker     (121)       25 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/ase_traj/Al8He8O12/energy.raw
+-rw-r--r--   0 runner    (1001) docker     (121)     2161 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/ase_traj/Al8He8O12/force.raw
+-rw-r--r--   0 runner    (1001) docker     (121)       56 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/ase_traj/Al8He8O12/type.raw
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/ase_traj/Al8He8O12/type_map.raw
+-rw-r--r--   0 runner    (1001) docker     (121)      225 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/ase_traj/Al8He8O12/virial.raw
+-rw-r--r--   0 runner    (1001) docker     (121)    14428 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/ase_traj/HeAlO.traj
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.058610 dpdata-0.2.9/tests/bond_order/
+-rw-r--r--   0 runner    (1001) docker     (121)      806 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/bond_order/BOH4-.mol
+-rw-r--r--   0 runner    (1001) docker     (121)      902 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/bond_order/C5H5-.mol
+-rw-r--r--   0 runner    (1001) docker     (121)      557 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/bond_order/CH3CC-.mol
+-rw-r--r--   0 runner    (1001) docker     (121)      557 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/bond_order/CH3NC.mol
+-rw-r--r--   0 runner    (1001) docker     (121)      723 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/bond_order/CH3NH3+.mol
+-rw-r--r--   0 runner    (1001) docker     (121)      640 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/bond_order/CH3NO2.mol
+-rw-r--r--   0 runner    (1001) docker     (121)      806 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/bond_order/CH3OAsO3_2-.mol
+-rw-r--r--   0 runner    (1001) docker     (121)      557 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/bond_order/CH3OH.mol
+-rw-r--r--   0 runner    (1001) docker     (121)      806 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/bond_order/CH3OPO3_2-.mol
+-rw-r--r--   0 runner    (1001) docker     (121)      723 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/bond_order/CH3PH3+.mol
+-rw-r--r--   0 runner    (1001) docker     (121)      557 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/bond_order/CH3SH.mol
+-rw-r--r--   0 runner    (1001) docker     (121)      723 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/bond_order/CH3SO3-.mol
+-rw-r--r--   0 runner    (1001) docker     (121)      889 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/bond_order/CH3_2SO.mol
+-rw-r--r--   0 runner    (1001) docker     (121)      972 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/bond_order/CH3_2SO2.mol
+-rw-r--r--   0 runner    (1001) docker     (121)     1138 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/bond_order/OCH3+.mol
+-rw-r--r--   0 runner    (1001) docker     (121)     1138 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/bond_order/arg.mol
+-rw-r--r--   0 runner    (1001) docker     (121)     4911 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/bond_order/formal_charge.mol
+-rw-r--r--   0 runner    (1001) docker     (121)      889 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/bond_order/gly.mol
+-rw-r--r--   0 runner    (1001) docker     (121)     1916 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/bond_order/methane.sdf
+-rw-r--r--   0 runner    (1001) docker     (121)     2414 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/bond_order/methane_ethane.sdf
+-rw-r--r--   0 runner    (1001) docker     (121)     1068 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/bond_order/oxpy.mol
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:06.998610 dpdata-0.2.9/tests/bond_order/refined-set-ligands/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.062610 dpdata-0.2.9/tests/bond_order/refined-set-ligands/obabel/
+-rw-r--r--   0 runner    (1001) docker     (121)     4167 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/bond_order/refined-set-ligands/obabel/1a4r_ligand_obabel.sdf
+-rw-r--r--   0 runner    (1001) docker     (121)     2017 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/bond_order/refined-set-ligands/obabel/1ai5_ligand_obabel.sdf
+-rw-r--r--   0 runner    (1001) docker     (121)     2480 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/bond_order/refined-set-ligands/obabel/1f5l_ligand_obabel.sdf
+-rw-r--r--   0 runner    (1001) docker     (121)     1352 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/bond_order/refined-set-ligands/obabel/1m1b_ligand_obabel.sdf
+-rw-r--r--   0 runner    (1001) docker     (121)     4810 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/bond_order/refined-set-ligands/obabel/1mue_ligand_obabel.sdf
+-rw-r--r--   0 runner    (1001) docker     (121)     3130 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/bond_order/refined-set-ligands/obabel/1w4q_ligand_obabel.sdf
+-rw-r--r--   0 runner    (1001) docker     (121)     4439 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/bond_order/refined-set-ligands/obabel/2e94_ligand_obabel.sdf
+-rw-r--r--   0 runner    (1001) docker     (121)     2425 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/bond_order/refined-set-ligands/obabel/4xaq_ligand_obabel.sdf
+-rw-r--r--   0 runner    (1001) docker     (121)     6603 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/bond_order/refined-set-ligands/obabel/4xtw_ligand_obabel.sdf
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.062610 dpdata-0.2.9/tests/bond_order/refined-set-ligands/origin/
+-rw-r--r--   0 runner    (1001) docker     (121)     3213 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/bond_order/refined-set-ligands/origin/1a4r_ligand.sdf
+-rw-r--r--   0 runner    (1001) docker     (121)     1559 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/bond_order/refined-set-ligands/origin/1ai5_ligand.sdf
+-rw-r--r--   0 runner    (1001) docker     (121)     1911 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/bond_order/refined-set-ligands/origin/1f5l_ligand.sdf
+-rw-r--r--   0 runner    (1001) docker     (121)     1050 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/bond_order/refined-set-ligands/origin/1m1b_ligand.sdf
+-rw-r--r--   0 runner    (1001) docker     (121)     3704 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/bond_order/refined-set-ligands/origin/1mue_ligand.sdf
+-rw-r--r--   0 runner    (1001) docker     (121)     2422 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/bond_order/refined-set-ligands/origin/1w4q_ligand.sdf
+-rw-r--r--   0 runner    (1001) docker     (121)     3421 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/bond_order/refined-set-ligands/origin/2e94_ligand.sdf
+-rw-r--r--   0 runner    (1001) docker     (121)     1859 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/bond_order/refined-set-ligands/origin/4xaq_ligand.sdf
+-rw-r--r--   0 runner    (1001) docker     (121)     5071 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/bond_order/refined-set-ligands/origin/4xtw_ligand.sdf
+-rw-r--r--   0 runner    (1001) docker     (121)     4633 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/comp_sys.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5956 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/computed_structure_entry.json
+-rw-r--r--   0 runner    (1001) docker     (121)      222 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/context.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.062610 dpdata-0.2.9/tests/cp2k/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.070610 dpdata-0.2.9/tests/cp2k/aimd/
+-rw-r--r--   0 runner    (1001) docker     (121)     4061 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/cp2k/aimd/DPGEN-1.ener
+-rw-r--r--   0 runner    (1001) docker     (121)  1041450 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/cp2k/aimd/DPGEN-frc-1.xyz
+-rw-r--r--   0 runner    (1001) docker     (121)  1041450 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/cp2k/aimd/DPGEN-pos-1.xyz
+-rw-r--r--   0 runner    (1001) docker     (121)  4621389 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/cp2k/aimd/cp2k.log
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.070610 dpdata-0.2.9/tests/cp2k/aimd/deepmd/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.074610 dpdata-0.2.9/tests/cp2k/aimd/deepmd/set.000/
+-rw-r--r--   0 runner    (1001) docker     (121)     1208 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/cp2k/aimd/deepmd/set.000/box.npy
+-rw-r--r--   0 runner    (1001) docker     (121)   192008 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/cp2k/aimd/deepmd/set.000/coord.npy
+-rw-r--r--   0 runner    (1001) docker     (121)      248 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/cp2k/aimd/deepmd/set.000/energy.npy
+-rw-r--r--   0 runner    (1001) docker     (121)   192008 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/cp2k/aimd/deepmd/set.000/force.npy
+-rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/cp2k/aimd/deepmd/type.raw
+-rw-r--r--   0 runner    (1001) docker     (121)       10 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/cp2k/aimd/deepmd/type_map.raw
+-rw-r--r--   0 runner    (1001) docker     (121)    28510 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/cp2k/aimd/input.inp
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.074610 dpdata-0.2.9/tests/cp2k/aimd_stress/
+-rw-r--r--   0 runner    (1001) docker     (121)      207 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/cp2k/aimd_stress/DPGEN-pos-1.xyz
+-rw-r--r--   0 runner    (1001) docker     (121)   110555 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/cp2k/aimd_stress/cp2k.log
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.074610 dpdata-0.2.9/tests/cp2k/aimd_stress/deepmd/
+-rw-r--r--   0 runner    (1001) docker     (121)      225 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/cp2k/aimd_stress/deepmd/box.raw
+-rw-r--r--   0 runner    (1001) docker     (121)      375 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/cp2k/aimd_stress/deepmd/coord.raw
+-rw-r--r--   0 runner    (1001) docker     (121)       26 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/cp2k/aimd_stress/deepmd/energy.raw
+-rw-r--r--   0 runner    (1001) docker     (121)      382 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/cp2k/aimd_stress/deepmd/force.raw
+-rw-r--r--   0 runner    (1001) docker     (121)       10 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/cp2k/aimd_stress/deepmd/type.raw
+-rw-r--r--   0 runner    (1001) docker     (121)        4 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/cp2k/aimd_stress/deepmd/type_map.raw
+-rw-r--r--   0 runner    (1001) docker     (121)      230 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/cp2k/aimd_stress/deepmd/virial.raw
+-rw-r--r--   0 runner    (1001) docker     (121)     1966 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/cp2k/aimd_stress/input.inp
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.074610 dpdata-0.2.9/tests/cp2k/cp2k_duplicate_header/
+-rw-r--r--   0 runner    (1001) docker     (121)   186887 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/cp2k/cp2k_duplicate_header/cp2k_output_duplicate_header
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.074610 dpdata-0.2.9/tests/cp2k/cp2k_duplicate_header/deepmd/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.074610 dpdata-0.2.9/tests/cp2k/cp2k_duplicate_header/deepmd/set.000/
+-rw-r--r--   0 runner    (1001) docker     (121)      164 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/cp2k/cp2k_duplicate_header/deepmd/set.000/box.npy
+-rw-r--r--   0 runner    (1001) docker     (121)      488 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/cp2k/cp2k_duplicate_header/deepmd/set.000/coord.npy
+-rw-r--r--   0 runner    (1001) docker     (121)      132 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/cp2k/cp2k_duplicate_header/deepmd/set.000/energy.npy
+-rw-r--r--   0 runner    (1001) docker     (121)      488 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/cp2k/cp2k_duplicate_header/deepmd/set.000/force.npy
+-rw-r--r--   0 runner    (1001) docker     (121)      164 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/cp2k/cp2k_duplicate_header/deepmd/set.000/virial.npy
+-rw-r--r--   0 runner    (1001) docker     (121)       60 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/cp2k/cp2k_duplicate_header/deepmd/type.raw
+-rw-r--r--   0 runner    (1001) docker     (121)       10 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/cp2k/cp2k_duplicate_header/deepmd/type_map.raw
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.078610 dpdata-0.2.9/tests/cp2k/cp2k_element_replace/
+-rw-r--r--   0 runner    (1001) docker     (121)   329537 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/cp2k/cp2k_element_replace/cp2k_output_element_replace
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.078610 dpdata-0.2.9/tests/cp2k/cp2k_element_replace/deepmd/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.078610 dpdata-0.2.9/tests/cp2k/cp2k_element_replace/deepmd/set.000/
+-rw-r--r--   0 runner    (1001) docker     (121)      164 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/cp2k/cp2k_element_replace/deepmd/set.000/box.npy
+-rw-r--r--   0 runner    (1001) docker     (121)     7340 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/cp2k/cp2k_element_replace/deepmd/set.000/coord.npy
+-rw-r--r--   0 runner    (1001) docker     (121)      132 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/cp2k/cp2k_element_replace/deepmd/set.000/energy.npy
+-rw-r--r--   0 runner    (1001) docker     (121)     7340 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/cp2k/cp2k_element_replace/deepmd/set.000/force.npy
+-rw-r--r--   0 runner    (1001) docker     (121)      164 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/cp2k/cp2k_element_replace/deepmd/set.000/virial.npy
+-rw-r--r--   0 runner    (1001) docker     (121)     1202 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/cp2k/cp2k_element_replace/deepmd/type.raw
+-rw-r--r--   0 runner    (1001) docker     (121)       10 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/cp2k/cp2k_element_replace/deepmd/type_map.raw
+-rw-r--r--   0 runner    (1001) docker     (121)   303494 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/cp2k/cp2k_nocon_output
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.078610 dpdata-0.2.9/tests/cp2k/cp2k_normal_output/
+-rw-r--r--   0 runner    (1001) docker     (121)   107587 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/cp2k/cp2k_normal_output/cp2k_output
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.078610 dpdata-0.2.9/tests/cp2k/cp2k_normal_output/deepmd/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.078610 dpdata-0.2.9/tests/cp2k/cp2k_normal_output/deepmd/set.000/
+-rw-r--r--   0 runner    (1001) docker     (121)      164 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/cp2k/cp2k_normal_output/deepmd/set.000/box.npy
+-rw-r--r--   0 runner    (1001) docker     (121)      488 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/cp2k/cp2k_normal_output/deepmd/set.000/coord.npy
+-rw-r--r--   0 runner    (1001) docker     (121)      132 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/cp2k/cp2k_normal_output/deepmd/set.000/energy.npy
+-rw-r--r--   0 runner    (1001) docker     (121)      488 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/cp2k/cp2k_normal_output/deepmd/set.000/force.npy
+-rw-r--r--   0 runner    (1001) docker     (121)      164 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/cp2k/cp2k_normal_output/deepmd/set.000/virial.npy
+-rw-r--r--   0 runner    (1001) docker     (121)       60 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/cp2k/cp2k_normal_output/deepmd/type.raw
+-rw-r--r--   0 runner    (1001) docker     (121)       10 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/cp2k/cp2k_normal_output/deepmd/type_map.raw
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.082610 dpdata-0.2.9/tests/fhi_aims/
+-rw-r--r--   0 runner    (1001) docker     (121)    65680 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/fhi_aims/out_md
+-rw-r--r--   0 runner    (1001) docker     (121)   124362 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/fhi_aims/out_scf
+-rw-r--r--   0 runner    (1001) docker     (121)   420506 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/fhi_aims/output_multi_elements
+-rw-r--r--   0 runner    (1001) docker     (121)      141 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/fhi_aims/ref_cell.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      423 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/fhi_aims/ref_cell_md.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      631 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/fhi_aims/ref_cell_md_m.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/fhi_aims/ref_coord.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      516 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/fhi_aims/ref_coord_md.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    31680 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/fhi_aims/ref_coord_md_m.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       99 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/fhi_aims/ref_energy_md.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      204 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/fhi_aims/ref_energy_md_m.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      170 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/fhi_aims/ref_force.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      774 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/fhi_aims/ref_force_md.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    44640 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/fhi_aims/ref_force_md_m.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.086610 dpdata-0.2.9/tests/gaussian/
+-rw-r--r--   0 runner    (1001) docker     (121)   151758 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/gaussian/aimd_gaussian_CH4_output
+-rw-r--r--   0 runner    (1001) docker     (121)  1192096 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/gaussian/largeforce.gaussianlog
+-rw-r--r--   0 runner    (1001) docker     (121)    18377 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/gaussian/methane.gaussianlog
+-rw-r--r--   0 runner    (1001) docker     (121)    18377 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/gaussian/methane_reordered.gaussianlog
+-rw-r--r--   0 runner    (1001) docker     (121)    18166 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/gaussian/methane_sub.gaussianlog
+-rw-r--r--   0 runner    (1001) docker     (121)    15547 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/gaussian/noncoveraged.gaussianlog
+-rw-r--r--   0 runner    (1001) docker     (121)    68303 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/gaussian/oxygen.gaussianlog
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.086610 dpdata-0.2.9/tests/gromacs/
+-rw-r--r--   0 runner    (1001) docker     (121)      469 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/gromacs/1h.gro
+-rw-r--r--   0 runner    (1001) docker     (121)      493 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/gromacs/1h.tri.gro
+-rw-r--r--   0 runner    (1001) docker     (121)     1573 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/gromacs/case_for_format_atom_name.gro
+-rw-r--r--   0 runner    (1001) docker     (121)      952 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/gromacs/multi_frames.gro
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.090610 dpdata-0.2.9/tests/poscars/
+-rw-r--r--   0 runner    (1001) docker     (121)   148662 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/poscars/6362_OUTCAR
+-rw-r--r--   0 runner    (1001) docker     (121)     1950 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/poscars/CONTCAR.h2o.md
+-rw-r--r--   0 runner    (1001) docker     (121)    66878 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/poscars/OUTCAR.Ge.vdw
+-rw-r--r--   0 runner    (1001) docker     (121)    31877 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/poscars/OUTCAR.ch4.1step
+-rw-r--r--   0 runner    (1001) docker     (121)   144560 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/poscars/OUTCAR.ch4.ml
+-rw-r--r--   0 runner    (1001) docker     (121)   130114 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/poscars/OUTCAR.ch4.unconverged
+-rw-r--r--   0 runner    (1001) docker     (121)   122105 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/poscars/OUTCAR.h2o.md
+-rw-r--r--   0 runner    (1001) docker     (121)   262639 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/poscars/OUTCAR.h2o.md.10
+-rw-r--r--   0 runner    (1001) docker     (121)     2931 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/poscars/POSCAR.P42nmc
+-rw-r--r--   0 runner    (1001) docker     (121)     4864 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/poscars/POSCAR.P42nmc.replace
+-rw-r--r--   0 runner    (1001) docker     (121)      627 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/poscars/POSCAR.SiC
+-rw-r--r--   0 runner    (1001) docker     (121)      629 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/poscars/POSCAR.SiC.const
+-rw-r--r--   0 runner    (1001) docker     (121)      628 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/poscars/POSCAR.SiC.normal
+-rw-r--r--   0 runner    (1001) docker     (121)     2742 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/poscars/POSCAR.SiC.replicate123
+-rw-r--r--   0 runner    (1001) docker     (121)      629 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/poscars/POSCAR.SiC.uniform
+-rw-r--r--   0 runner    (1001) docker     (121)      219 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/poscars/POSCAR.h2o.md
+-rw-r--r--   0 runner    (1001) docker     (121)      242 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/poscars/POSCAR.h4o3
+-rw-r--r--   0 runner    (1001) docker     (121)      150 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/poscars/POSCAR.oh.c
+-rw-r--r--   0 runner    (1001) docker     (121)      134 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/poscars/POSCAR.oh.d
+-rw-r--r--   0 runner    (1001) docker     (121)      155 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/poscars/POSCAR.oh.d.dup
+-rw-r--r--   0 runner    (1001) docker     (121)     1120 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/poscars/conf.5.dump
+-rw-r--r--   0 runner    (1001) docker     (121)      448 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/poscars/conf.dump
+-rw-r--r--   0 runner    (1001) docker     (121)      229 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/poscars/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (121)    14032 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/poscars/conf.waterion.lmp
+-rw-r--r--   0 runner    (1001) docker     (121)      475 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/poscars/conf_s_su.dump
+-rw-r--r--   0 runner    (1001) docker     (121)      674 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/poscars/conf_unfold.dump
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.094610 dpdata-0.2.9/tests/poscars/deepmd.h2o.md/
+-rw-r--r--   0 runner    (1001) docker     (121)      681 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/poscars/deepmd.h2o.md/box.raw
+-rw-r--r--   0 runner    (1001) docker     (121)     1350 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/poscars/deepmd.h2o.md/coord.raw
+-rw-r--r--   0 runner    (1001) docker     (121)       78 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/poscars/deepmd.h2o.md/energy.raw
+-rw-r--r--   0 runner    (1001) docker     (121)     1382 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/poscars/deepmd.h2o.md/force.raw
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/poscars/deepmd.h2o.md/type.raw
+-rw-r--r--   0 runner    (1001) docker     (121)      687 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/poscars/deepmd.h2o.md/virial.raw
+-rw-r--r--   0 runner    (1001) docker     (121)    10091 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/poscars/h2o.md.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1539 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/poscars/poscar_ref_oh.py
+-rw-r--r--   0 runner    (1001) docker     (121)      701 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/poscars/shift_origin.dump
+-rw-r--r--   0 runner    (1001) docker     (121)      790 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/poscars/test_lammps_dump_s_su.py
+-rw-r--r--   0 runner    (1001) docker     (121)    58956 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/poscars/vasprun.Ge.vdw.xml
+-rw-r--r--   0 runner    (1001) docker     (121)   108944 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/poscars/vasprun.h2o.md.10.xml
+-rw-r--r--   0 runner    (1001) docker     (121)    83635 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/poscars/vasprun.h2o.md.tribox.lower.xml
+-rw-r--r--   0 runner    (1001) docker     (121)    82151 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/poscars/vasprun.h2o.md.tribox.xml
+-rw-r--r--   0 runner    (1001) docker     (121)    73398 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/poscars/vasprun.h2o.md.xml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.098610 dpdata-0.2.9/tests/pwmat/
+-rw-r--r--   0 runner    (1001) docker     (121)  2137763 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/pwmat/MOVEMENT
+-rw-r--r--   0 runner    (1001) docker     (121)     1354 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/pwmat/OUT.MLMD
+-rw-r--r--   0 runner    (1001) docker     (121)      447 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/pwmat/atom.config
+-rw-r--r--   0 runner    (1001) docker     (121)      279 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/pwmat/atom.config.oh
+-rw-r--r--   0 runner    (1001) docker     (121)      229 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/pwmat/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (121)     1972 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/pwmat/config_ref_ch4.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1506 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/pwmat/config_ref_oh.py
+-rw-r--r--   0 runner    (1001) docker     (121)      174 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/pwmat/mlmd_cell
+-rw-r--r--   0 runner    (1001) docker     (121)      350 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/pwmat/mlmd_coord
+-rw-r--r--   0 runner    (1001) docker     (121)      350 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/pwmat/mlmd_force
+-rw-r--r--   0 runner    (1001) docker     (121)      180 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/pwmat/ref_cell
+-rw-r--r--   0 runner    (1001) docker     (121)      365 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/pwmat/ref_coord
+-rw-r--r--   0 runner    (1001) docker     (121)      364 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/pwmat/ref_force
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.098610 dpdata-0.2.9/tests/pymatgen_data/
+-rw-r--r--   0 runner    (1001) docker     (121)      632 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/pymatgen_data/FA-001.vasp
+-rw-r--r--   0 runner    (1001) docker     (121)      614 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/pymatgen_data/FA-001.xyz
+-rw-r--r--   0 runner    (1001) docker     (121)      348 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/pymatgen_data/mol2-new.vasp
+-rw-r--r--   0 runner    (1001) docker     (121)      823 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/pymatgen_data/mol2.vasp
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.098610 dpdata-0.2.9/tests/qe.scf/
+-rw-r--r--   0 runner    (1001) docker     (121)      576 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/qe.scf/01.in
+-rw-r--r--   0 runner    (1001) docker     (121)    12346 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/qe.scf/01.out
+-rw-r--r--   0 runner    (1001) docker     (121)     6197 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/qe.scf/02.in
+-rw-r--r--   0 runner    (1001) docker     (121)    45800 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/qe.scf/02.out
+-rwxr-xr-x   0 runner    (1001) docker     (121)      829 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/qe.scf/Al.in
+-rw-r--r--   0 runner    (1001) docker     (121)    21583 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/qe.scf/Al.out
+-rw-r--r--   0 runner    (1001) docker     (121)      375 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/qe.scf/ch4_coord
+-rw-r--r--   0 runner    (1001) docker     (121)      381 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/qe.scf/ch4_force
+-rw-r--r--   0 runner    (1001) docker     (121)      228 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/qe.scf/ch4_virial
+-rw-r--r--   0 runner    (1001) docker     (121)      226 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/qe.scf/h2o_cell
+-rw-r--r--   0 runner    (1001) docker     (121)    14402 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/qe.scf/h2o_coord
+-rw-r--r--   0 runner    (1001) docker     (121)    14706 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/qe.scf/h2o_force
+-rw-r--r--   0 runner    (1001) docker     (121)      229 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/qe.scf/h2o_virial
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.102610 dpdata-0.2.9/tests/qe.traj/
+-rw-r--r--   0 runner    (1001) docker     (121)      344 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/qe.traj/oh-md.evp
+-rw-r--r--   0 runner    (1001) docker     (121)    29072 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/qe.traj/oh-md.for
+-rw-r--r--   0 runner    (1001) docker     (121)    10435 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/qe.traj/oh-md.in
+-rw-r--r--   0 runner    (1001) docker     (121)    29072 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/qe.traj/oh-md.pos
+-rw-r--r--   0 runner    (1001) docker     (121)      960 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/qe.traj/traj6.cel
+-rw-r--r--   0 runner    (1001) docker     (121)     1048 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/qe.traj/traj6.evp
+-rw-r--r--   0 runner    (1001) docker     (121)     1020 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/qe.traj/traj6.for
+-rw-r--r--   0 runner    (1001) docker     (121)     1550 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/qe.traj/traj6.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1032 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/qe.traj/traj6.pos
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:06.998610 dpdata-0.2.9/tests/siesta/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.102610 dpdata-0.2.9/tests/siesta/aimd/
+-rw-r--r--   0 runner    (1001) docker     (121)      650 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/siesta/aimd/cell
+-rw-r--r--   0 runner    (1001) docker     (121)    13800 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/siesta/aimd/coord
+-rw-r--r--   0 runner    (1001) docker     (121)       55 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/siesta/aimd/energy
+-rw-r--r--   0 runner    (1001) docker     (121)    11532 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/siesta/aimd/force
+-rw-r--r--   0 runner    (1001) docker     (121)    66496 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/siesta/aimd/output
+-rw-r--r--   0 runner    (1001) docker     (121)      684 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/siesta/aimd/virial
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.102610 dpdata-0.2.9/tests/siesta/scf/
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/siesta/scf/ref_cell
+-rw-r--r--   0 runner    (1001) docker     (121)      215 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/siesta/scf/ref_coord
+-rw-r--r--   0 runner    (1001) docker     (121)       10 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/siesta/scf/ref_energy
+-rw-r--r--   0 runner    (1001) docker     (121)      185 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/siesta/scf/ref_force
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/siesta/scf/ref_virial
+-rw-r--r--   0 runner    (1001) docker     (121)    23640 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/siesta/scf/siesta_output
+-rw-r--r--   0 runner    (1001) docker     (121)     4840 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/test_abacus_md.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4863 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/test_abacus_pw_scf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2694 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/test_abacus_relax.py
+-rw-r--r--   0 runner    (1001) docker     (121)      665 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/test_abacus_stru_dump.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1447 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/test_amber_md.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2550 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/test_amber_sqm.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1539 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/test_ase_traj.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5233 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/test_bond_order_system.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1954 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/test_cell_to_low_triangle.py
+-rw-r--r--   0 runner    (1001) docker     (121)      544 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1616 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/test_corr.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1676 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/test_cp2k_aimd_output.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2151 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/test_cp2k_output.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3535 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/test_deepmd_comp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2761 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/test_deepmd_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8103 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/test_deepmd_raw.py
+-rw-r--r--   0 runner    (1001) docker     (121)      813 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/test_elements_index.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1083 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/test_empty.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1896 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/test_fhi_md_multi_elem_output.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1859 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/test_fhi_md_output.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/test_fhi_output.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4154 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/test_gaussian_driver.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2706 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/test_gaussian_log.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5606 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/test_gromacs_gro.py
+-rw-r--r--   0 runner    (1001) docker     (121)      962 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (121)      453 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/test_lammps_dump_shift_origin.py
+-rw-r--r--   0 runner    (1001) docker     (121)      834 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/test_lammps_dump_skipload.py
+-rw-r--r--   0 runner    (1001) docker     (121)      780 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/test_lammps_dump_to_system.py
+-rw-r--r--   0 runner    (1001) docker     (121)      794 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/test_lammps_dump_unfold.py
+-rw-r--r--   0 runner    (1001) docker     (121)      985 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/test_lammps_lmp_dump.py
+-rw-r--r--   0 runner    (1001) docker     (121)      435 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/test_lammps_lmp_to_system.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1600 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/test_msd.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6138 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/test_multisystems.py
+-rw-r--r--   0 runner    (1001) docker     (121)      772 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/test_periodic_table.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5282 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/test_perturb.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1389 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/test_pick_atom_idx.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3211 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/test_predict.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1887 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/test_pwmat_config_dump.py
+-rw-r--r--   0 runner    (1001) docker     (121)      963 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/test_pwmat_config_to_system.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1870 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/test_pwmat_mlmd.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2061 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/test_pwmat_movement.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1291 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/test_pymatgen_molecule.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2321 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/test_qe_cp_traj.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2636 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/test_qe_cp_traj_skipload.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4767 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/test_qe_pw_scf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      869 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/test_qe_pw_scf_crystal_atomic_positions.py
+-rw-r--r--   0 runner    (1001) docker     (121)      694 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/test_qe_pw_scf_energy_bug.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3979 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/test_quip_gap_xyz.py
+-rw-r--r--   0 runner    (1001) docker     (121)      582 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/test_remove_atom_names.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1410 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/test_remove_pbc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1370 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/test_replace.py
+-rw-r--r--   0 runner    (1001) docker     (121)      817 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/test_replicate.py
+-rw-r--r--   0 runner    (1001) docker     (121)      768 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/test_shuffle.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3090 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/test_siesta_aiMD_output.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3004 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/test_siesta_output.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1055 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/test_sqm_driver.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1137 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/test_stat.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1841 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/test_system_append.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1077 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/test_system_apply_pbc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1387 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/test_system_set_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1478 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/test_to_ase.py
+-rw-r--r--   0 runner    (1001) docker     (121)      570 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/test_to_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)      777 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/test_to_pymatgen.py
+-rw-r--r--   0 runner    (1001) docker     (121)      974 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/test_to_pymatgen_entry.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1292 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/test_type_map.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4172 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/test_vasp_outcar.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1861 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/test_vasp_poscar_dump.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1863 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/test_vasp_poscar_to_system.py
+-rw-r--r--   0 runner    (1001) docker     (121)      761 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/test_vasp_unconverged_outcar.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1639 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/test_vasp_xml.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2206 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/test_water_ions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1406 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/test_xyz.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.102610 dpdata-0.2.9/tests/xyz/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.106610 dpdata-0.2.9/tests/xyz/B1C9/
+-rw-r--r--   0 runner    (1001) docker     (121)      450 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/xyz/B1C9/box.raw
+-rw-r--r--   0 runner    (1001) docker     (121)     1500 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/xyz/B1C9/coord.raw
+-rw-r--r--   0 runner    (1001) docker     (121)       52 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/xyz/B1C9/energy.raw
+-rw-r--r--   0 runner    (1001) docker     (121)     1533 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/xyz/B1C9/force.raw
+-rw-r--r--   0 runner    (1001) docker     (121)       20 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/xyz/B1C9/type.raw
+-rw-r--r--   0 runner    (1001) docker     (121)        4 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/xyz/B1C9/type_map.raw
+-rw-r--r--   0 runner    (1001) docker     (121)      457 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/xyz/B1C9/virial.raw
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.106610 dpdata-0.2.9/tests/xyz/B5C7/
+-rw-r--r--   0 runner    (1001) docker     (121)      225 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/xyz/B5C7/box.raw
+-rw-r--r--   0 runner    (1001) docker     (121)      900 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/xyz/B5C7/coord.raw
+-rw-r--r--   0 runner    (1001) docker     (121)       25 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/xyz/B5C7/energy.raw
+-rw-r--r--   0 runner    (1001) docker     (121)      918 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/xyz/B5C7/force.raw
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/xyz/B5C7/type.raw
+-rw-r--r--   0 runner    (1001) docker     (121)        4 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/xyz/B5C7/type_map.raw
+-rw-r--r--   0 runner    (1001) docker     (121)      225 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/xyz/B5C7/virial.raw
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 02:59:07.106610 dpdata-0.2.9/tests/xyz/B5C7_novirials/
+-rw-r--r--   0 runner    (1001) docker     (121)      225 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/xyz/B5C7_novirials/box.raw
+-rw-r--r--   0 runner    (1001) docker     (121)      900 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/xyz/B5C7_novirials/coord.raw
+-rw-r--r--   0 runner    (1001) docker     (121)       25 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/xyz/B5C7_novirials/energy.raw
+-rw-r--r--   0 runner    (1001) docker     (121)      918 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/xyz/B5C7_novirials/force.raw
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/xyz/B5C7_novirials/type.raw
+-rw-r--r--   0 runner    (1001) docker     (121)        4 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/xyz/B5C7_novirials/type_map.raw
+-rw-r--r--   0 runner    (1001) docker     (121)     1436 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/xyz/xyz_B5C7_novirials.xyz
+-rw-r--r--   0 runner    (1001) docker     (121)     4440 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/xyz/xyz_unittest.field.xyz
+-rw-r--r--   0 runner    (1001) docker     (121)     4413 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/xyz/xyz_unittest.sort.xyz
+-rw-r--r--   0 runner    (1001) docker     (121)     4413 2022-10-03 02:58:54.000000 dpdata-0.2.9/tests/xyz/xyz_unittest.xyz
```

### Comparing `dpdata-0.2.8/.github/ISSUE_TEMPLATE/bug_report.md` & `dpdata-0.2.9/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/.github/ISSUE_TEMPLATE/feature_request.md` & `dpdata-0.2.9/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/.github/ISSUE_TEMPLATE/request-for-help.md` & `dpdata-0.2.9/.github/ISSUE_TEMPLATE/request-for-help.md`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/.github/workflows/mirror_gitee.yml` & `dpdata-0.2.9/.github/workflows/mirror_gitee.yml`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/.github/workflows/pub-pypi.yml` & `dpdata-0.2.9/.github/workflows/pub-pypi.yml`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/.github/workflows/test.yml` & `dpdata-0.2.9/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/LICENSE` & `dpdata-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/PKG-INFO` & `dpdata-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dpdata
-Version: 0.2.8
+Version: 0.2.9
 Summary: Manipulating data formats of DeePMD-kit, VASP, QE, PWmat, and LAMMPS, etc.
 Home-page: https://github.com/deepmodeling/dpdata
 Author: Han Wang
 Author-email: wang_han@iapcm.ac.cn
 Keywords: lammps vasp deepmd-kit
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `dpdata-0.2.8/README.md` & `dpdata-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/docs/Makefile` & `dpdata-0.2.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/docs/conf.py` & `dpdata-0.2.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/docs/make_format.py` & `dpdata-0.2.9/docs/make_format.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/dpdata/__init__.py` & `dpdata-0.2.9/dpdata/__init__.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/dpdata/abacus/md.py` & `dpdata-0.2.9/dpdata/abacus/md.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/dpdata/abacus/relax.py` & `dpdata-0.2.9/dpdata/abacus/relax.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/dpdata/abacus/scf.py` & `dpdata-0.2.9/dpdata/abacus/scf.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/dpdata/amber/mask.py` & `dpdata-0.2.9/dpdata/amber/mask.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/dpdata/amber/md.py` & `dpdata-0.2.9/dpdata/amber/md.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/dpdata/amber/sqm.py` & `dpdata-0.2.9/dpdata/amber/sqm.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/dpdata/ase_calculator.py` & `dpdata-0.2.9/dpdata/ase_calculator.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/dpdata/bond_order_system.py` & `dpdata-0.2.9/dpdata/bond_order_system.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/dpdata/cli.py` & `dpdata-0.2.9/dpdata/cli.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/dpdata/cp2k/cell.py` & `dpdata-0.2.9/dpdata/cp2k/cell.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/dpdata/cp2k/output.py` & `dpdata-0.2.9/dpdata/cp2k/output.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/dpdata/deepmd/comp.py` & `dpdata-0.2.9/dpdata/deepmd/comp.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/dpdata/deepmd/hdf5.py` & `dpdata-0.2.9/dpdata/deepmd/hdf5.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/dpdata/deepmd/raw.py` & `dpdata-0.2.9/dpdata/deepmd/raw.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/dpdata/driver.py` & `dpdata-0.2.9/dpdata/driver.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/dpdata/fhi_aims/output.py` & `dpdata-0.2.9/dpdata/fhi_aims/output.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/dpdata/format.py` & `dpdata-0.2.9/dpdata/format.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/dpdata/gaussian/gjf.py` & `dpdata-0.2.9/dpdata/gaussian/gjf.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/dpdata/gaussian/log.py` & `dpdata-0.2.9/dpdata/gaussian/log.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/dpdata/gromacs/gro.py` & `dpdata-0.2.9/dpdata/gromacs/gro.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/dpdata/lammps/dump.py` & `dpdata-0.2.9/dpdata/lammps/dump.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/dpdata/lammps/lmp.py` & `dpdata-0.2.9/dpdata/lammps/lmp.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/dpdata/md/msd.py` & `dpdata-0.2.9/dpdata/md/msd.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/dpdata/md/pbc.py` & `dpdata-0.2.9/dpdata/md/pbc.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/dpdata/md/rdf.py` & `dpdata-0.2.9/dpdata/md/rdf.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/dpdata/md/water.py` & `dpdata-0.2.9/dpdata/md/water.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/dpdata/periodic_table.json` & `dpdata-0.2.9/dpdata/periodic_table.json`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/dpdata/periodic_table.py` & `dpdata-0.2.9/dpdata/periodic_table.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/dpdata/plugin.py` & `dpdata-0.2.9/dpdata/plugin.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/dpdata/plugins/__init__.py` & `dpdata-0.2.9/dpdata/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/dpdata/plugins/abacus.py` & `dpdata-0.2.9/dpdata/plugins/abacus.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/dpdata/plugins/amber.py` & `dpdata-0.2.9/dpdata/plugins/amber.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/dpdata/plugins/ase.py` & `dpdata-0.2.9/dpdata/plugins/ase.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/dpdata/plugins/cp2k.py` & `dpdata-0.2.9/dpdata/plugins/cp2k.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/dpdata/plugins/deepmd.py` & `dpdata-0.2.9/dpdata/plugins/deepmd.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/dpdata/plugins/fhi_aims.py` & `dpdata-0.2.9/dpdata/plugins/fhi_aims.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/dpdata/plugins/gaussian.py` & `dpdata-0.2.9/dpdata/plugins/gaussian.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/dpdata/plugins/gromacs.py` & `dpdata-0.2.9/dpdata/plugins/gromacs.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/dpdata/plugins/lammps.py` & `dpdata-0.2.9/dpdata/plugins/lammps.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/dpdata/plugins/list.py` & `dpdata-0.2.9/dpdata/plugins/list.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/dpdata/plugins/pwmat.py` & `dpdata-0.2.9/dpdata/plugins/pwmat.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/dpdata/plugins/pymatgen.py` & `dpdata-0.2.9/dpdata/plugins/pymatgen.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/dpdata/plugins/qe.py` & `dpdata-0.2.9/dpdata/plugins/qe.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/dpdata/plugins/rdkit.py` & `dpdata-0.2.9/dpdata/plugins/rdkit.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/dpdata/plugins/siesta.py` & `dpdata-0.2.9/dpdata/plugins/siesta.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/dpdata/plugins/vasp.py` & `dpdata-0.2.9/dpdata/plugins/vasp.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/dpdata/plugins/xyz.py` & `dpdata-0.2.9/dpdata/plugins/xyz.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/dpdata/pwmat/atomconfig.py` & `dpdata-0.2.9/dpdata/pwmat/atomconfig.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/dpdata/pwmat/movement.py` & `dpdata-0.2.9/dpdata/pwmat/movement.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/dpdata/pymatgen/molecule.py` & `dpdata-0.2.9/dpdata/pymatgen/molecule.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/dpdata/qe/scf.py` & `dpdata-0.2.9/dpdata/qe/scf.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/dpdata/qe/traj.py` & `dpdata-0.2.9/dpdata/qe/traj.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/dpdata/rdkit/sanitize.py` & `dpdata-0.2.9/dpdata/rdkit/sanitize.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/dpdata/rdkit/utils.py` & `dpdata-0.2.9/dpdata/rdkit/utils.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/dpdata/siesta/aiMD_output.py` & `dpdata-0.2.9/dpdata/siesta/aiMD_output.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/dpdata/siesta/output.py` & `dpdata-0.2.9/dpdata/siesta/output.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/dpdata/stat.py` & `dpdata-0.2.9/dpdata/stat.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/dpdata/system.py` & `dpdata-0.2.9/dpdata/system.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/dpdata/unit.py` & `dpdata-0.2.9/dpdata/unit.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/dpdata/utils.py` & `dpdata-0.2.9/dpdata/utils.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/dpdata/vasp/outcar.py` & `dpdata-0.2.9/dpdata/vasp/outcar.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/dpdata/vasp/poscar.py` & `dpdata-0.2.9/dpdata/vasp/poscar.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/dpdata/vasp/xml.py` & `dpdata-0.2.9/dpdata/vasp/xml.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/dpdata/xyz/quip_gap_xyz.py` & `dpdata-0.2.9/dpdata/xyz/quip_gap_xyz.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/dpdata/xyz/xyz.py` & `dpdata-0.2.9/dpdata/xyz/xyz.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/dpdata.egg-info/PKG-INFO` & `dpdata-0.2.9/dpdata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dpdata
-Version: 0.2.8
+Version: 0.2.9
 Summary: Manipulating data formats of DeePMD-kit, VASP, QE, PWmat, and LAMMPS, etc.
 Home-page: https://github.com/deepmodeling/dpdata
 Author: Han Wang
 Author-email: wang_han@iapcm.ac.cn
 Keywords: lammps vasp deepmd-kit
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `dpdata-0.2.8/dpdata.egg-info/SOURCES.txt` & `dpdata-0.2.9/dpdata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/plugin_example/dpdata_random/__init__.py` & `dpdata-0.2.9/plugin_example/dpdata_random/__init__.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/setup.py` & `dpdata-0.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/POSCAR` & `dpdata-0.2.9/tests/POSCAR`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/abacus.md/INPUT` & `dpdata-0.2.9/tests/abacus.md/INPUT`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/abacus.md/OUT.abacus/MD_dump` & `dpdata-0.2.9/tests/abacus.md/OUT.abacus/MD_dump`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/abacus.md/OUT.abacus/running_md.log` & `dpdata-0.2.9/tests/abacus.md/OUT.abacus/running_md.log`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/abacus.md/water_coord` & `dpdata-0.2.9/tests/abacus.md/water_coord`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/abacus.md/water_force` & `dpdata-0.2.9/tests/abacus.md/water_force`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/abacus.md/water_virial` & `dpdata-0.2.9/tests/abacus.md/water_virial`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/abacus.md.nostress/OUT.autotest/MD_dump` & `dpdata-0.2.9/tests/abacus.md.nostress/OUT.autotest/MD_dump`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/abacus.md.nostress/OUT.autotest/running_md.log` & `dpdata-0.2.9/tests/abacus.md.nostress/OUT.autotest/running_md.log`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/abacus.relax/INPUT` & `dpdata-0.2.9/tests/abacus.relax/INPUT`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/abacus.relax/OUT.abacus/INPUT` & `dpdata-0.2.9/tests/abacus.relax/OUT.abacus/INPUT`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/abacus.relax/OUT.abacus/running_cell-relax.log` & `dpdata-0.2.9/tests/abacus.relax/OUT.abacus/running_cell-relax.log`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/abacus.relax/coord.ref` & `dpdata-0.2.9/tests/abacus.relax/coord.ref`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/abacus.relax/force.ref` & `dpdata-0.2.9/tests/abacus.relax/force.ref`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/abacus.relax/stress.ref` & `dpdata-0.2.9/tests/abacus.relax/stress.ref`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/abacus.relax/virial.ref` & `dpdata-0.2.9/tests/abacus.relax/virial.ref`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/abacus.scf/OUT.ch4/running_scf.log` & `dpdata-0.2.9/tests/abacus.scf/OUT.ch4/running_scf.log`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/abacus.scf/STRU.ch4` & `dpdata-0.2.9/tests/abacus.scf/STRU.ch4`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/abacus.scf/stru_test` & `dpdata-0.2.9/tests/abacus.scf/stru_test`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/amber/02_Heat.mden` & `dpdata-0.2.9/tests/amber/02_Heat.mden`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/amber/02_Heat.mdfrc` & `dpdata-0.2.9/tests/amber/02_Heat.mdfrc`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/amber/02_Heat.nc` & `dpdata-0.2.9/tests/amber/02_Heat.nc`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/amber/02_Heat.parm7` & `dpdata-0.2.9/tests/amber/02_Heat.parm7`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/amber/corr/dataset/C6H11HW192O6OW96P1/set.000/coord.npy` & `dpdata-0.2.9/tests/amber/corr/dataset/C6H11HW192O6OW96P1/set.000/coord.npy`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/amber/corr/dataset/C6H11HW192O6OW96P1/set.000/force.npy` & `dpdata-0.2.9/tests/amber/corr/dataset/C6H11HW192O6OW96P1/set.000/force.npy`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/amber/corr/dp_amber_mask/C6EP0H11HW192O6OW96P1/set.000/coord.npy` & `dpdata-0.2.9/tests/amber/corr/dp_amber_mask/C6EP0H11HW192O6OW96P1/set.000/coord.npy`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/amber/corr/dp_amber_mask/C6EP0H11HW192O6OW96P1/set.000/force.npy` & `dpdata-0.2.9/tests/amber/corr/dp_amber_mask/C6EP0H11HW192O6OW96P1/set.000/force.npy`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/amber/corr/dp_corr/set.000/coord.npy` & `dpdata-0.2.9/tests/amber/corr/dp_corr/set.000/coord.npy`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/amber/corr/dp_corr/set.000/force.npy` & `dpdata-0.2.9/tests/amber/corr/dp_corr/set.000/force.npy`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/amber/corr/dp_hl/set.000/coord.npy` & `dpdata-0.2.9/tests/amber/corr/dp_hl/set.000/coord.npy`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/amber/corr/dp_hl/set.000/force.npy` & `dpdata-0.2.9/tests/amber/corr/dp_hl/set.000/force.npy`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/amber/corr/dp_ll/set.000/coord.npy` & `dpdata-0.2.9/tests/amber/corr/dp_ll/set.000/coord.npy`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/amber/corr/dp_ll/set.000/force.npy` & `dpdata-0.2.9/tests/amber/corr/dp_ll/set.000/force.npy`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/amber/corr/high_level.mdfrc` & `dpdata-0.2.9/tests/amber/corr/high_level.mdfrc`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/amber/corr/high_level.mdout` & `dpdata-0.2.9/tests/amber/corr/high_level.mdout`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/amber/corr/low_level.mdfrc` & `dpdata-0.2.9/tests/amber/corr/low_level.mdfrc`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/amber/corr/low_level.mdout` & `dpdata-0.2.9/tests/amber/corr/low_level.mdout`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/amber/corr/qmmm.parm7` & `dpdata-0.2.9/tests/amber/corr/qmmm.parm7`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/amber/corr/rc.nc` & `dpdata-0.2.9/tests/amber/corr/rc.nc`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/amber/sqm_forces.out` & `dpdata-0.2.9/tests/amber/sqm_forces.out`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/amber/sqm_no_forces.out` & `dpdata-0.2.9/tests/amber/sqm_no_forces.out`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/amber/sqm_opt.out` & `dpdata-0.2.9/tests/amber/sqm_opt.out`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/ase_traj/Al2He2O3/coord.raw` & `dpdata-0.2.9/tests/ase_traj/Al2He2O3/coord.raw`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/ase_traj/Al2He2O3/force.raw` & `dpdata-0.2.9/tests/ase_traj/Al2He2O3/force.raw`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/ase_traj/Al4He0O6/coord.raw` & `dpdata-0.2.9/tests/ase_traj/Al4He0O6/coord.raw`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/ase_traj/Al4He0O6/force.raw` & `dpdata-0.2.9/tests/ase_traj/Al4He0O6/force.raw`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/ase_traj/Al4He2O6/coord.raw` & `dpdata-0.2.9/tests/ase_traj/Al4He2O6/coord.raw`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/ase_traj/Al4He2O6/force.raw` & `dpdata-0.2.9/tests/ase_traj/Al4He2O6/force.raw`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/ase_traj/Al4He4O6/coord.raw` & `dpdata-0.2.9/tests/ase_traj/Al4He4O6/coord.raw`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/ase_traj/Al4He4O6/force.raw` & `dpdata-0.2.9/tests/ase_traj/Al4He4O6/force.raw`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/ase_traj/Al8He0O12/box.raw` & `dpdata-0.2.9/tests/ase_traj/Al8He0O12/box.raw`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/ase_traj/Al8He0O12/coord.raw` & `dpdata-0.2.9/tests/ase_traj/Al8He0O12/coord.raw`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/ase_traj/Al8He0O12/force.raw` & `dpdata-0.2.9/tests/ase_traj/Al8He0O12/force.raw`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/ase_traj/Al8He0O12/virial.raw` & `dpdata-0.2.9/tests/ase_traj/Al8He0O12/virial.raw`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/ase_traj/Al8He4O12/coord.raw` & `dpdata-0.2.9/tests/ase_traj/Al8He4O12/coord.raw`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/ase_traj/Al8He4O12/force.raw` & `dpdata-0.2.9/tests/ase_traj/Al8He4O12/force.raw`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/ase_traj/Al8He8O12/coord.raw` & `dpdata-0.2.9/tests/ase_traj/Al8He8O12/coord.raw`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/ase_traj/Al8He8O12/force.raw` & `dpdata-0.2.9/tests/ase_traj/Al8He8O12/force.raw`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/ase_traj/HeAlO.traj` & `dpdata-0.2.9/tests/ase_traj/HeAlO.traj`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/bond_order/BOH4-.mol` & `dpdata-0.2.9/tests/bond_order/BOH4-.mol`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/bond_order/C5H5-.mol` & `dpdata-0.2.9/tests/bond_order/C5H5-.mol`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/bond_order/CH3CC-.mol` & `dpdata-0.2.9/tests/bond_order/CH3CC-.mol`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/bond_order/CH3NC.mol` & `dpdata-0.2.9/tests/bond_order/CH3NC.mol`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/bond_order/CH3NH3+.mol` & `dpdata-0.2.9/tests/bond_order/CH3NH3+.mol`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/bond_order/CH3NO2.mol` & `dpdata-0.2.9/tests/bond_order/CH3NO2.mol`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/bond_order/CH3OAsO3_2-.mol` & `dpdata-0.2.9/tests/bond_order/CH3OAsO3_2-.mol`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/bond_order/CH3OH.mol` & `dpdata-0.2.9/tests/bond_order/CH3OH.mol`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/bond_order/CH3OPO3_2-.mol` & `dpdata-0.2.9/tests/bond_order/CH3OPO3_2-.mol`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/bond_order/CH3PH3+.mol` & `dpdata-0.2.9/tests/bond_order/CH3PH3+.mol`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/bond_order/CH3SH.mol` & `dpdata-0.2.9/tests/bond_order/CH3SH.mol`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/bond_order/CH3SO3-.mol` & `dpdata-0.2.9/tests/bond_order/CH3SO3-.mol`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/bond_order/CH3_2SO.mol` & `dpdata-0.2.9/tests/bond_order/CH3_2SO.mol`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/bond_order/CH3_2SO2.mol` & `dpdata-0.2.9/tests/bond_order/CH3_2SO2.mol`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/bond_order/OCH3+.mol` & `dpdata-0.2.9/tests/bond_order/OCH3+.mol`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/bond_order/arg.mol` & `dpdata-0.2.9/tests/bond_order/arg.mol`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/bond_order/formal_charge.mol` & `dpdata-0.2.9/tests/bond_order/formal_charge.mol`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/bond_order/gly.mol` & `dpdata-0.2.9/tests/bond_order/gly.mol`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/bond_order/methane.sdf` & `dpdata-0.2.9/tests/bond_order/methane.sdf`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/bond_order/methane_ethane.sdf` & `dpdata-0.2.9/tests/bond_order/methane_ethane.sdf`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/bond_order/oxpy.mol` & `dpdata-0.2.9/tests/bond_order/oxpy.mol`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/bond_order/refined-set-ligands/obabel/1a4r_ligand_obabel.sdf` & `dpdata-0.2.9/tests/bond_order/refined-set-ligands/obabel/1a4r_ligand_obabel.sdf`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/bond_order/refined-set-ligands/obabel/1ai5_ligand_obabel.sdf` & `dpdata-0.2.9/tests/bond_order/refined-set-ligands/obabel/1ai5_ligand_obabel.sdf`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/bond_order/refined-set-ligands/obabel/1f5l_ligand_obabel.sdf` & `dpdata-0.2.9/tests/bond_order/refined-set-ligands/obabel/1f5l_ligand_obabel.sdf`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/bond_order/refined-set-ligands/obabel/1m1b_ligand_obabel.sdf` & `dpdata-0.2.9/tests/bond_order/refined-set-ligands/obabel/1m1b_ligand_obabel.sdf`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/bond_order/refined-set-ligands/obabel/1mue_ligand_obabel.sdf` & `dpdata-0.2.9/tests/bond_order/refined-set-ligands/obabel/1mue_ligand_obabel.sdf`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/bond_order/refined-set-ligands/obabel/1w4q_ligand_obabel.sdf` & `dpdata-0.2.9/tests/bond_order/refined-set-ligands/obabel/1w4q_ligand_obabel.sdf`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/bond_order/refined-set-ligands/obabel/2e94_ligand_obabel.sdf` & `dpdata-0.2.9/tests/bond_order/refined-set-ligands/obabel/2e94_ligand_obabel.sdf`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/bond_order/refined-set-ligands/obabel/4xaq_ligand_obabel.sdf` & `dpdata-0.2.9/tests/bond_order/refined-set-ligands/obabel/4xaq_ligand_obabel.sdf`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/bond_order/refined-set-ligands/obabel/4xtw_ligand_obabel.sdf` & `dpdata-0.2.9/tests/bond_order/refined-set-ligands/obabel/4xtw_ligand_obabel.sdf`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/bond_order/refined-set-ligands/origin/1a4r_ligand.sdf` & `dpdata-0.2.9/tests/bond_order/refined-set-ligands/origin/1a4r_ligand.sdf`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/bond_order/refined-set-ligands/origin/1ai5_ligand.sdf` & `dpdata-0.2.9/tests/bond_order/refined-set-ligands/origin/1ai5_ligand.sdf`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/bond_order/refined-set-ligands/origin/1f5l_ligand.sdf` & `dpdata-0.2.9/tests/bond_order/refined-set-ligands/origin/1f5l_ligand.sdf`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/bond_order/refined-set-ligands/origin/1m1b_ligand.sdf` & `dpdata-0.2.9/tests/bond_order/refined-set-ligands/origin/1m1b_ligand.sdf`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/bond_order/refined-set-ligands/origin/1mue_ligand.sdf` & `dpdata-0.2.9/tests/bond_order/refined-set-ligands/origin/1mue_ligand.sdf`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/bond_order/refined-set-ligands/origin/1w4q_ligand.sdf` & `dpdata-0.2.9/tests/bond_order/refined-set-ligands/origin/1w4q_ligand.sdf`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/bond_order/refined-set-ligands/origin/2e94_ligand.sdf` & `dpdata-0.2.9/tests/bond_order/refined-set-ligands/origin/2e94_ligand.sdf`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/bond_order/refined-set-ligands/origin/4xaq_ligand.sdf` & `dpdata-0.2.9/tests/bond_order/refined-set-ligands/origin/4xaq_ligand.sdf`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/bond_order/refined-set-ligands/origin/4xtw_ligand.sdf` & `dpdata-0.2.9/tests/bond_order/refined-set-ligands/origin/4xtw_ligand.sdf`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/comp_sys.py` & `dpdata-0.2.9/tests/comp_sys.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/computed_structure_entry.json` & `dpdata-0.2.9/tests/computed_structure_entry.json`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/cp2k/aimd/DPGEN-1.ener` & `dpdata-0.2.9/tests/cp2k/aimd/DPGEN-1.ener`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/cp2k/aimd/DPGEN-frc-1.xyz` & `dpdata-0.2.9/tests/cp2k/aimd/DPGEN-frc-1.xyz`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/cp2k/aimd/DPGEN-pos-1.xyz` & `dpdata-0.2.9/tests/cp2k/aimd/DPGEN-pos-1.xyz`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/cp2k/aimd/cp2k.log` & `dpdata-0.2.9/tests/cp2k/aimd/cp2k.log`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/cp2k/aimd/deepmd/set.000/box.npy` & `dpdata-0.2.9/tests/cp2k/aimd/deepmd/set.000/box.npy`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/cp2k/aimd/deepmd/set.000/coord.npy` & `dpdata-0.2.9/tests/cp2k/aimd/deepmd/set.000/coord.npy`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/cp2k/aimd/deepmd/set.000/force.npy` & `dpdata-0.2.9/tests/cp2k/aimd/deepmd/set.000/force.npy`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/cp2k/aimd/input.inp` & `dpdata-0.2.9/tests/cp2k/aimd/input.inp`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/cp2k/aimd_stress/cp2k.log` & `dpdata-0.2.9/tests/cp2k/aimd_stress/cp2k.log`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/cp2k/aimd_stress/input.inp` & `dpdata-0.2.9/tests/cp2k/aimd_stress/input.inp`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/cp2k/cp2k_duplicate_header/cp2k_output_duplicate_header` & `dpdata-0.2.9/tests/cp2k/cp2k_duplicate_header/cp2k_output_duplicate_header`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/cp2k/cp2k_element_replace/cp2k_output_element_replace` & `dpdata-0.2.9/tests/cp2k/cp2k_element_replace/cp2k_output_element_replace`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/cp2k/cp2k_element_replace/deepmd/set.000/coord.npy` & `dpdata-0.2.9/tests/cp2k/cp2k_element_replace/deepmd/set.000/coord.npy`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/cp2k/cp2k_element_replace/deepmd/set.000/force.npy` & `dpdata-0.2.9/tests/cp2k/cp2k_element_replace/deepmd/set.000/force.npy`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/cp2k/cp2k_nocon_output` & `dpdata-0.2.9/tests/cp2k/cp2k_nocon_output`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/cp2k/cp2k_normal_output/cp2k_output` & `dpdata-0.2.9/tests/cp2k/cp2k_normal_output/cp2k_output`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/fhi_aims/out_md` & `dpdata-0.2.9/tests/fhi_aims/out_md`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/fhi_aims/out_scf` & `dpdata-0.2.9/tests/fhi_aims/out_scf`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/fhi_aims/output_multi_elements` & `dpdata-0.2.9/tests/fhi_aims/output_multi_elements`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/fhi_aims/ref_cell_md_m.txt` & `dpdata-0.2.9/tests/fhi_aims/ref_cell_md_m.txt`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/fhi_aims/ref_coord_md.txt` & `dpdata-0.2.9/tests/fhi_aims/ref_coord_md.txt`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/fhi_aims/ref_coord_md_m.txt` & `dpdata-0.2.9/tests/fhi_aims/ref_coord_md_m.txt`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/fhi_aims/ref_force_md.txt` & `dpdata-0.2.9/tests/fhi_aims/ref_force_md.txt`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/fhi_aims/ref_force_md_m.txt` & `dpdata-0.2.9/tests/fhi_aims/ref_force_md_m.txt`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/gaussian/aimd_gaussian_CH4_output` & `dpdata-0.2.9/tests/gaussian/aimd_gaussian_CH4_output`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/gaussian/largeforce.gaussianlog` & `dpdata-0.2.9/tests/gaussian/largeforce.gaussianlog`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/gaussian/methane.gaussianlog` & `dpdata-0.2.9/tests/gaussian/methane.gaussianlog`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/gaussian/methane_reordered.gaussianlog` & `dpdata-0.2.9/tests/gaussian/methane_reordered.gaussianlog`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/gaussian/methane_sub.gaussianlog` & `dpdata-0.2.9/tests/gaussian/methane_sub.gaussianlog`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/gaussian/noncoveraged.gaussianlog` & `dpdata-0.2.9/tests/gaussian/noncoveraged.gaussianlog`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/gaussian/oxygen.gaussianlog` & `dpdata-0.2.9/tests/gaussian/oxygen.gaussianlog`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/gromacs/case_for_format_atom_name.gro` & `dpdata-0.2.9/tests/gromacs/case_for_format_atom_name.gro`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/gromacs/multi_frames.gro` & `dpdata-0.2.9/tests/gromacs/multi_frames.gro`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/poscars/6362_OUTCAR` & `dpdata-0.2.9/tests/poscars/6362_OUTCAR`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/poscars/CONTCAR.h2o.md` & `dpdata-0.2.9/tests/poscars/CONTCAR.h2o.md`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/poscars/OUTCAR.Ge.vdw` & `dpdata-0.2.9/tests/poscars/OUTCAR.Ge.vdw`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/poscars/OUTCAR.ch4.1step` & `dpdata-0.2.9/tests/poscars/OUTCAR.ch4.1step`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/poscars/OUTCAR.ch4.ml` & `dpdata-0.2.9/tests/poscars/OUTCAR.ch4.ml`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/poscars/OUTCAR.ch4.unconverged` & `dpdata-0.2.9/tests/poscars/OUTCAR.ch4.unconverged`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/poscars/OUTCAR.h2o.md` & `dpdata-0.2.9/tests/poscars/OUTCAR.h2o.md`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/poscars/OUTCAR.h2o.md.10` & `dpdata-0.2.9/tests/poscars/OUTCAR.h2o.md.10`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/poscars/POSCAR.P42nmc` & `dpdata-0.2.9/tests/poscars/POSCAR.P42nmc`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/poscars/POSCAR.P42nmc.replace` & `dpdata-0.2.9/tests/poscars/POSCAR.P42nmc.replace`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/poscars/POSCAR.SiC` & `dpdata-0.2.9/tests/poscars/POSCAR.SiC`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/poscars/POSCAR.SiC.const` & `dpdata-0.2.9/tests/poscars/POSCAR.SiC.const`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/poscars/POSCAR.SiC.normal` & `dpdata-0.2.9/tests/poscars/POSCAR.SiC.normal`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/poscars/POSCAR.SiC.replicate123` & `dpdata-0.2.9/tests/poscars/POSCAR.SiC.replicate123`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/poscars/POSCAR.SiC.uniform` & `dpdata-0.2.9/tests/poscars/POSCAR.SiC.uniform`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/poscars/conf.5.dump` & `dpdata-0.2.9/tests/poscars/conf.5.dump`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/poscars/conf.waterion.lmp` & `dpdata-0.2.9/tests/poscars/conf.waterion.lmp`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/poscars/conf_unfold.dump` & `dpdata-0.2.9/tests/poscars/conf_unfold.dump`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/poscars/deepmd.h2o.md/box.raw` & `dpdata-0.2.9/tests/poscars/deepmd.h2o.md/box.raw`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/poscars/deepmd.h2o.md/coord.raw` & `dpdata-0.2.9/tests/poscars/deepmd.h2o.md/coord.raw`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/poscars/deepmd.h2o.md/force.raw` & `dpdata-0.2.9/tests/poscars/deepmd.h2o.md/force.raw`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/poscars/deepmd.h2o.md/virial.raw` & `dpdata-0.2.9/tests/poscars/deepmd.h2o.md/virial.raw`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/poscars/h2o.md.json` & `dpdata-0.2.9/tests/poscars/h2o.md.json`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/poscars/poscar_ref_oh.py` & `dpdata-0.2.9/tests/poscars/poscar_ref_oh.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/poscars/shift_origin.dump` & `dpdata-0.2.9/tests/poscars/shift_origin.dump`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/poscars/test_lammps_dump_s_su.py` & `dpdata-0.2.9/tests/poscars/test_lammps_dump_s_su.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/poscars/vasprun.Ge.vdw.xml` & `dpdata-0.2.9/tests/poscars/vasprun.Ge.vdw.xml`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/poscars/vasprun.h2o.md.10.xml` & `dpdata-0.2.9/tests/poscars/vasprun.h2o.md.10.xml`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/poscars/vasprun.h2o.md.tribox.lower.xml` & `dpdata-0.2.9/tests/poscars/vasprun.h2o.md.tribox.lower.xml`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/poscars/vasprun.h2o.md.tribox.xml` & `dpdata-0.2.9/tests/poscars/vasprun.h2o.md.tribox.xml`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/poscars/vasprun.h2o.md.xml` & `dpdata-0.2.9/tests/poscars/vasprun.h2o.md.xml`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/pwmat/MOVEMENT` & `dpdata-0.2.9/tests/pwmat/MOVEMENT`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/pwmat/OUT.MLMD` & `dpdata-0.2.9/tests/pwmat/OUT.MLMD`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/pwmat/config_ref_ch4.py` & `dpdata-0.2.9/tests/pwmat/config_ref_ch4.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/pwmat/config_ref_oh.py` & `dpdata-0.2.9/tests/pwmat/config_ref_oh.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/pymatgen_data/FA-001.vasp` & `dpdata-0.2.9/tests/pymatgen_data/FA-001.vasp`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/pymatgen_data/FA-001.xyz` & `dpdata-0.2.9/tests/pymatgen_data/FA-001.xyz`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/pymatgen_data/mol2.vasp` & `dpdata-0.2.9/tests/pymatgen_data/mol2.vasp`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/qe.scf/01.in` & `dpdata-0.2.9/tests/qe.scf/01.in`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/qe.scf/01.out` & `dpdata-0.2.9/tests/qe.scf/01.out`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/qe.scf/02.in` & `dpdata-0.2.9/tests/qe.scf/02.in`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/qe.scf/02.out` & `dpdata-0.2.9/tests/qe.scf/02.out`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/qe.scf/Al.in` & `dpdata-0.2.9/tests/qe.scf/Al.in`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/qe.scf/Al.out` & `dpdata-0.2.9/tests/qe.scf/Al.out`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/qe.scf/h2o_coord` & `dpdata-0.2.9/tests/qe.scf/h2o_coord`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/qe.scf/h2o_force` & `dpdata-0.2.9/tests/qe.scf/h2o_force`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/qe.traj/oh-md.for` & `dpdata-0.2.9/tests/qe.traj/oh-md.for`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/qe.traj/oh-md.in` & `dpdata-0.2.9/tests/qe.traj/oh-md.in`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/qe.traj/oh-md.pos` & `dpdata-0.2.9/tests/qe.traj/oh-md.pos`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/qe.traj/traj6.cel` & `dpdata-0.2.9/tests/qe.traj/traj6.cel`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/qe.traj/traj6.evp` & `dpdata-0.2.9/tests/qe.traj/traj6.evp`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/qe.traj/traj6.for` & `dpdata-0.2.9/tests/qe.traj/traj6.for`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/qe.traj/traj6.in` & `dpdata-0.2.9/tests/qe.traj/traj6.in`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/qe.traj/traj6.pos` & `dpdata-0.2.9/tests/qe.traj/traj6.pos`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/siesta/aimd/coord` & `dpdata-0.2.9/tests/siesta/aimd/coord`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/siesta/aimd/force` & `dpdata-0.2.9/tests/siesta/aimd/force`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/siesta/aimd/output` & `dpdata-0.2.9/tests/siesta/aimd/output`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/siesta/aimd/virial` & `dpdata-0.2.9/tests/siesta/aimd/virial`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/siesta/scf/siesta_output` & `dpdata-0.2.9/tests/siesta/scf/siesta_output`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/test_abacus_md.py` & `dpdata-0.2.9/tests/test_abacus_md.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/test_abacus_pw_scf.py` & `dpdata-0.2.9/tests/test_abacus_pw_scf.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/test_abacus_relax.py` & `dpdata-0.2.9/tests/test_abacus_relax.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/test_abacus_stru_dump.py` & `dpdata-0.2.9/tests/test_abacus_stru_dump.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/test_amber_md.py` & `dpdata-0.2.9/tests/test_amber_md.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/test_amber_sqm.py` & `dpdata-0.2.9/tests/test_amber_sqm.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/test_ase_traj.py` & `dpdata-0.2.9/tests/test_ase_traj.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/test_bond_order_system.py` & `dpdata-0.2.9/tests/test_bond_order_system.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/test_cell_to_low_triangle.py` & `dpdata-0.2.9/tests/test_cell_to_low_triangle.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/test_cli.py` & `dpdata-0.2.9/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/test_corr.py` & `dpdata-0.2.9/tests/test_corr.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/test_cp2k_aimd_output.py` & `dpdata-0.2.9/tests/test_cp2k_aimd_output.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/test_cp2k_output.py` & `dpdata-0.2.9/tests/test_cp2k_output.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/test_deepmd_comp.py` & `dpdata-0.2.9/tests/test_deepmd_comp.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/test_deepmd_hdf5.py` & `dpdata-0.2.9/tests/test_deepmd_hdf5.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/test_deepmd_raw.py` & `dpdata-0.2.9/tests/test_deepmd_raw.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/test_elements_index.py` & `dpdata-0.2.9/tests/test_elements_index.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/test_empty.py` & `dpdata-0.2.9/tests/test_empty.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/test_fhi_md_multi_elem_output.py` & `dpdata-0.2.9/tests/test_fhi_md_multi_elem_output.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/test_fhi_md_output.py` & `dpdata-0.2.9/tests/test_fhi_md_output.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/test_fhi_output.py` & `dpdata-0.2.9/tests/test_fhi_output.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/test_gaussian_driver.py` & `dpdata-0.2.9/tests/test_gaussian_driver.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/test_gaussian_log.py` & `dpdata-0.2.9/tests/test_gaussian_log.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/test_gromacs_gro.py` & `dpdata-0.2.9/tests/test_gromacs_gro.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/test_json.py` & `dpdata-0.2.9/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/test_lammps_dump_skipload.py` & `dpdata-0.2.9/tests/test_lammps_dump_skipload.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/test_lammps_dump_to_system.py` & `dpdata-0.2.9/tests/test_lammps_dump_to_system.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/test_lammps_dump_unfold.py` & `dpdata-0.2.9/tests/test_lammps_dump_unfold.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/test_lammps_lmp_dump.py` & `dpdata-0.2.9/tests/test_lammps_lmp_dump.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/test_msd.py` & `dpdata-0.2.9/tests/test_msd.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/test_multisystems.py` & `dpdata-0.2.9/tests/test_multisystems.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/test_periodic_table.py` & `dpdata-0.2.9/tests/test_periodic_table.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/test_perturb.py` & `dpdata-0.2.9/tests/test_perturb.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/test_pick_atom_idx.py` & `dpdata-0.2.9/tests/test_pick_atom_idx.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/test_predict.py` & `dpdata-0.2.9/tests/test_predict.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/test_pwmat_config_dump.py` & `dpdata-0.2.9/tests/test_pwmat_config_dump.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/test_pwmat_config_to_system.py` & `dpdata-0.2.9/tests/test_pwmat_config_to_system.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/test_pwmat_mlmd.py` & `dpdata-0.2.9/tests/test_pwmat_mlmd.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/test_pwmat_movement.py` & `dpdata-0.2.9/tests/test_pwmat_movement.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/test_pymatgen_molecule.py` & `dpdata-0.2.9/tests/test_pymatgen_molecule.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/test_qe_cp_traj.py` & `dpdata-0.2.9/tests/test_qe_cp_traj.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/test_qe_cp_traj_skipload.py` & `dpdata-0.2.9/tests/test_qe_cp_traj_skipload.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/test_qe_pw_scf.py` & `dpdata-0.2.9/tests/test_qe_pw_scf.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/test_qe_pw_scf_crystal_atomic_positions.py` & `dpdata-0.2.9/tests/test_qe_pw_scf_crystal_atomic_positions.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/test_qe_pw_scf_energy_bug.py` & `dpdata-0.2.9/tests/test_qe_pw_scf_energy_bug.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/test_quip_gap_xyz.py` & `dpdata-0.2.9/tests/test_quip_gap_xyz.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/test_remove_atom_names.py` & `dpdata-0.2.9/tests/test_remove_atom_names.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/test_remove_pbc.py` & `dpdata-0.2.9/tests/test_remove_pbc.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/test_replace.py` & `dpdata-0.2.9/tests/test_replace.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/test_replicate.py` & `dpdata-0.2.9/tests/test_replicate.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/test_shuffle.py` & `dpdata-0.2.9/tests/test_shuffle.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/test_siesta_aiMD_output.py` & `dpdata-0.2.9/tests/test_siesta_aiMD_output.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/test_siesta_output.py` & `dpdata-0.2.9/tests/test_siesta_output.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/test_sqm_driver.py` & `dpdata-0.2.9/tests/test_sqm_driver.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/test_stat.py` & `dpdata-0.2.9/tests/test_stat.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/test_system_append.py` & `dpdata-0.2.9/tests/test_system_append.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/test_system_apply_pbc.py` & `dpdata-0.2.9/tests/test_system_apply_pbc.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/test_system_set_type.py` & `dpdata-0.2.9/tests/test_system_set_type.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/test_to_ase.py` & `dpdata-0.2.9/tests/test_to_ase.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/test_to_list.py` & `dpdata-0.2.9/tests/test_to_list.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/test_to_pymatgen.py` & `dpdata-0.2.9/tests/test_to_pymatgen.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/test_to_pymatgen_entry.py` & `dpdata-0.2.9/tests/test_to_pymatgen_entry.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/test_type_map.py` & `dpdata-0.2.9/tests/test_type_map.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/test_vasp_outcar.py` & `dpdata-0.2.9/tests/test_vasp_outcar.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/test_vasp_poscar_dump.py` & `dpdata-0.2.9/tests/test_vasp_poscar_dump.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/test_vasp_poscar_to_system.py` & `dpdata-0.2.9/tests/test_vasp_poscar_to_system.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/test_vasp_unconverged_outcar.py` & `dpdata-0.2.9/tests/test_vasp_unconverged_outcar.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/test_vasp_xml.py` & `dpdata-0.2.9/tests/test_vasp_xml.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/test_water_ions.py` & `dpdata-0.2.9/tests/test_water_ions.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/test_xyz.py` & `dpdata-0.2.9/tests/test_xyz.py`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/xyz/B1C9/coord.raw` & `dpdata-0.2.9/tests/xyz/B1C9/coord.raw`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/xyz/B1C9/force.raw` & `dpdata-0.2.9/tests/xyz/B1C9/force.raw`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/xyz/B5C7/coord.raw` & `dpdata-0.2.9/tests/xyz/B5C7/coord.raw`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/xyz/B5C7/force.raw` & `dpdata-0.2.9/tests/xyz/B5C7/force.raw`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/xyz/B5C7_novirials/coord.raw` & `dpdata-0.2.9/tests/xyz/B5C7_novirials/coord.raw`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/xyz/B5C7_novirials/force.raw` & `dpdata-0.2.9/tests/xyz/B5C7_novirials/force.raw`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/xyz/xyz_B5C7_novirials.xyz` & `dpdata-0.2.9/tests/xyz/xyz_B5C7_novirials.xyz`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/xyz/xyz_unittest.field.xyz` & `dpdata-0.2.9/tests/xyz/xyz_unittest.field.xyz`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/xyz/xyz_unittest.sort.xyz` & `dpdata-0.2.9/tests/xyz/xyz_unittest.sort.xyz`

 * *Files identical despite different names*

### Comparing `dpdata-0.2.8/tests/xyz/xyz_unittest.xyz` & `dpdata-0.2.9/tests/xyz/xyz_unittest.xyz`

 * *Files identical despite different names*

