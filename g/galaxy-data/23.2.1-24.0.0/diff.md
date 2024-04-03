# Comparing `tmp/galaxy-data-23.2.1.tar.gz` & `tmp/galaxy-data-24.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/galaxy/galaxy/packages/data/dist/.tmp-onyik87j/galaxy-data-23.2.1.tar", last modified: Thu Feb 22 03:53:47 2024, max compression
+gzip compressed data, was "galaxy-data-24.0.0.tar", last modified: Wed Apr  3 02:45:12 2024, max compression
```

## Comparing `galaxy-data-23.2.1.tar` & `galaxy-data-24.0.0.tar`

### file list

```diff
@@ -1,349 +1,351 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:53:47.000000 galaxy-data-23.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)    24595 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    25976 2024-02-22 03:53:47.000000 galaxy-data-23.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:53:47.000000 galaxy-data-23.2.1/galaxy/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:53:47.000000 galaxy-data-23.2.1/galaxy/datatypes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4682 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/annotation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6769 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/anvio.py
--rw-r--r--   0 runner    (1001) docker     (127)     8962 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/assembly.py
--rw-r--r--   0 runner    (1001) docker     (127)   164205 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/binary.py
--rw-r--r--   0 runner    (1001) docker     (127)    22465 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/blast.py
--rw-r--r--   0 runner    (1001) docker     (127)     4654 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/chain.py
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/checkers.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/chrominfo.py
--rw-r--r--   0 runner    (1001) docker     (127)    33378 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/constructive_solid_geometry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:53:47.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/bam_to_bai.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/bam_to_bigwig_converter.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/bcf_bcf_uncompressed_converter.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/bed_gff_or_vcf_to_bigwig_converter.xml
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/bed_to_fli_converter.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/bed_to_gff_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/bed_to_gff_converter.xml
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/bed_to_interval_index_converter.xml
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/bedgraph_to_bigwig_converter.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/bigwig_to_wig_converter.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/biom.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/bz2_to_uncompressed.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/cml_to_smi_converter.xml
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/cram_to_bam_converter.xml
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/csv_to_tabular.xml
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/fasta_to_2bit.xml
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/fasta_to_bowtie_base_index_converter.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/fasta_to_bowtie_color_index_converter.xml
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/fasta_to_fai.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/fasta_to_len.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/fasta_to_len.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/fasta_to_tabular_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/fasta_to_tabular_converter.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/fastq_to_fqtoc.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/fastq_to_fqtoc.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/fastqsolexa_to_fasta_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/fastqsolexa_to_fasta_converter.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/fastqsolexa_to_qual_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/fastqsolexa_to_qual_converter.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/gff_to_bed_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/gff_to_bed_converter.xml
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/gff_to_fli_converter.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/gff_to_interval_index_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/gff_to_interval_index_converter.xml
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/gro_to_pdb.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/gz_to_uncompressed.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/inchi_to_mol_converter.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/interval_to_bed12_converter.xml
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/interval_to_bed6_converter.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/interval_to_bed_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/interval_to_bed_converter.xml
--rw-r--r--   0 runner    (1001) docker     (127)     9402 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/interval_to_bedstrict_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/interval_to_bedstrict_converter.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/interval_to_bgzip_converter.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/interval_to_bigwig_converter.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/interval_to_fli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/interval_to_interval_index_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/interval_to_interval_index_converter.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4590 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/interval_to_tabix_converter.xml
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/len_to_linecount.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/lped_to_fped_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/lped_to_fped_converter.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/lped_to_pbed_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/lped_to_pbed_converter.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/maf_to_fasta_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/maf_to_fasta_converter.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/maf_to_interval_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/maf_to_interval_converter.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/mdconvert.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/mol2_to_mol_converter.xml
--rw-r--r--   0 runner    (1001) docker     (127)    11846 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/molecules_converter.xml
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/neostorezip_to_neostore_converter.xml
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/parquet_to_csv_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/parquet_to_csv_converter.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/pbed_ldreduced_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/pbed_ldreduced_converter.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/pbed_to_lped_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/pbed_to_lped_converter.xml
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/pdb_to_gro.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/picard_interval_list_to_bed6_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/picard_interval_list_to_bed6_converter.xml
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/pileup_to_interval_index_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/pileup_to_interval_index_converter.xml
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/ref_to_seq_taxonomy_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/ref_to_seq_taxonomy_converter.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/sam_to_bigwig_converter.xml
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/sam_to_unsorted_bam.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/smi_to_mol_converter.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/smi_to_smi_converter.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/tabular_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/tabular_to_csv.xml
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/tabular_to_dbnsfp.xml
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/tar_to_directory.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/to_coordinate_sorted_bam.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/to_qname_sorted_bam.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/uncompressed_to_gz.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/vcf_bgzip_to_tabix_converter.xml
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/vcf_to_interval_index_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/vcf_to_interval_index_converter.xml
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/vcf_to_vcf_bgzip_converter.xml
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/wig_to_bigwig_converter.xml
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/wiggle_to_simple_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/converters/wiggle_to_simple_converter.xml
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/coverage.py
--rw-r--r--   0 runner    (1001) docker     (127)    54942 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:53:47.000000 galaxy-data-23.2.1/galaxy/datatypes/dataproviders/
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/dataproviders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12033 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/dataproviders/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/dataproviders/chunk.py
--rw-r--r--   0 runner    (1001) docker     (127)    13755 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/dataproviders/column.py
--rw-r--r--   0 runner    (1001) docker     (127)    29823 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/dataproviders/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     6614 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/dataproviders/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/dataproviders/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5868 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/dataproviders/external.py
--rw-r--r--   0 runner    (1001) docker     (127)     5233 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/dataproviders/hierarchy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9450 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/dataproviders/line.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:53:47.000000 galaxy-data-23.2.1/galaxy/datatypes/display_applications/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/display_applications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15530 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/display_applications/application.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:53:47.000000 galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:53:47.000000 galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/biom/
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/biom/biom_simple.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:53:47.000000 galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/ensembl/
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/ensembl/ensembl_bam.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/ensembl/ensembl_gff.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/ensembl/ensembl_interval_as_bed.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:53:47.000000 galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/gbrowse/
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/gbrowse/gbrowse_gff.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/gbrowse/gbrowse_interval_as_bed.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/gbrowse/gbrowse_wig.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:53:47.000000 galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/icn3d/
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/icn3d/icn3d_simple.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:53:47.000000 galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/igb/
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/igb/bam.xml
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/igb/bb.xml
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/igb/bed.xml
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/igb/bedgraph.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/igb/bigwig.xml
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/igb/gtf.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/igb/wig.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:53:47.000000 galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/igv/
--rw-r--r--   0 runner    (1001) docker     (127)     5123 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/igv/bam.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/igv/bigwig.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/igv/genbank.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/igv/genome_fasta.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/igv/gff.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4965 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/igv/interval_as_bed.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5383 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/igv/vcf.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:53:47.000000 galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/image/
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/image/avivator.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:53:47.000000 galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/intermine/
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/intermine/intermine_simple.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:53:47.000000 galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/iobio/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/iobio/bam.xml
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/iobio/vcf.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:53:47.000000 galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/minerva/
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/minerva/tabular.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:53:47.000000 galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/qiime/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:53:47.000000 galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/qiime/qiime2/
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/qiime/qiime2/q2view.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:53:47.000000 galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/rviewer/
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/rviewer/bed.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/rviewer/vcf.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:53:47.000000 galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/ucsc/
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/ucsc/bam.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/ucsc/bigbed.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/ucsc/bigwig.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/ucsc/interval_as_bed.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/ucsc/maf_customtrack.xml
--rwxr-xr-x   0 runner    (1001) docker     (127)      436 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/ucsc/trackhub.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/ucsc/vcf.xml
--rw-r--r--   0 runner    (1001) docker     (127)    13628 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/display_applications/parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/display_applications/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:53:47.000000 galaxy-data-23.2.1/galaxy/datatypes/display_applications/xsd/
--rw-r--r--   0 runner    (1001) docker     (127)    16714 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/display_applications/xsd/geda.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/flow.py
--rw-r--r--   0 runner    (1001) docker     (127)    44070 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/genetics.py
--rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/gis.py
--rw-r--r--   0 runner    (1001) docker     (127)    21206 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/goldenpath.py
--rw-r--r--   0 runner    (1001) docker     (127)     6087 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)    15597 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/images.py
--rw-r--r--   0 runner    (1001) docker     (127)    83478 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/interval.py
--rw-r--r--   0 runner    (1001) docker     (127)    15589 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/isa.py
--rw-r--r--   0 runner    (1001) docker     (127)     6736 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/larch.py
--rw-r--r--   0 runner    (1001) docker     (127)     8419 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/media.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/metacyto.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/microarrays.py
--rw-r--r--   0 runner    (1001) docker     (127)    55369 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/molecules.py
--rw-r--r--   0 runner    (1001) docker     (127)    37916 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/mothur.py
--rw-r--r--   0 runner    (1001) docker     (127)     9861 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/msa.py
--rw-r--r--   0 runner    (1001) docker     (127)     5675 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/neo4j.py
--rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/ngsindex.py
--rw-r--r--   0 runner    (1001) docker     (127)     6423 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/phylip.py
--rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/plant_tribes.py
--rw-r--r--   0 runner    (1001) docker     (127)    36665 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/proteomics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/protocols.py
--rw-r--r--   0 runner    (1001) docker     (127)    10662 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/qiime2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/qualityscore.py
--rw-r--r--   0 runner    (1001) docker     (127)    52243 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    61099 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/set_metadata_tool.xml
--rw-r--r--   0 runner    (1001) docker     (127)    35782 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/sniff.py
--rw-r--r--   0 runner    (1001) docker     (127)     7289 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/spaln.py
--rw-r--r--   0 runner    (1001) docker     (127)     3910 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/speech.py
--rw-r--r--   0 runner    (1001) docker     (127)    77912 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/tabular.py
--rw-r--r--   0 runner    (1001) docker     (127)    49829 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/tracks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6157 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/triples.py
--rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/upload_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:53:47.000000 galaxy-data-23.2.1/galaxy/datatypes/util/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/util/generic_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    19188 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/util/gff_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    30760 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/util/maf_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     9606 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/datatypes/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:53:47.000000 galaxy-data-23.2.1/galaxy/model/
--rw-r--r--   0 runner    (1001) docker     (127)   439490 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6079 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    12466 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/custom_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/database_heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/database_object_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     5988 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/database_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:53:47.000000 galaxy-data-23.2.1/galaxy/model/dataset_collections/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/dataset_collections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5787 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/dataset_collections/builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4617 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/dataset_collections/matching.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/dataset_collections/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     7789 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/dataset_collections/structure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/dataset_collections/subcollections.py
--rw-r--r--   0 runner    (1001) docker     (127)     6601 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/dataset_collections/type_description.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:53:47.000000 galaxy-data-23.2.1/galaxy/model/dataset_collections/types/
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/dataset_collections/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/dataset_collections/types/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/dataset_collections/types/paired.py
--rw-r--r--   0 runner    (1001) docker     (127)    12279 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/deferred.py
--rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/index_filter_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     8543 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/item_attrs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)    28981 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:53:47.000000 galaxy-data-23.2.1/galaxy/model/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/migrations/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    13199 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:53:47.000000 galaxy-data-23.2.1/galaxy/model/migrations/alembic/
--rw-r--r--   0 runner    (1001) docker     (127)     4498 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/migrations/alembic/env.py
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/migrations/alembic/script.py.mako
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:53:47.000000 galaxy-data-23.2.1/galaxy/model/migrations/alembic/versions_gxy/
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/migrations/alembic/versions_gxy/186d4835587b_drop_job_state_history_update_time_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/migrations/alembic/versions_gxy/2d749563e1fe_add_notification_system_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/migrations/alembic/versions_gxy/3100452fa030_add_workflow_invocation_message_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/migrations/alembic/versions_gxy/3356bc2ecfc4_drop_view.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/migrations/alembic/versions_gxy/3a2914d703ca_add_index_wf_r_s_s__workflow_invocation_.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/migrations/alembic/versions_gxy/460d0ecd1dd8_.py
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/migrations/alembic/versions_gxy/518c8438a91b_add_when_expression_column.py
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/migrations/alembic/versions_gxy/59e024ceaca1_add_export_association_table.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/migrations/alembic/versions_gxy/6a67bf27e6a6_deferred_data_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/migrations/alembic/versions_gxy/8a19186a6ee7_add_columns_to_interactivetool_entry_point.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/migrations/alembic/versions_gxy/92fb564c7095_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/migrations/alembic/versions_gxy/9540a051226e_preferred_object_store_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/migrations/alembic/versions_gxy/987ce9839ecb_create_celery_user_rate_limit_table.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/migrations/alembic/versions_gxy/b182f655505f_add_workflow_source_metadata_column.py
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/migrations/alembic/versions_gxy/b855b714e8b8_make_api_keys_deleted_non_nullable.py
--rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/migrations/alembic/versions_gxy/c39f1de47a04_add_skipped_state_to_collection_job_.py
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/migrations/alembic/versions_gxy/caa7742f7bca_add_index_wf_r_i_p__workflow_invocation_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/migrations/alembic/versions_gxy/d0583094c8cd_add_quota_source_labels.py
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/migrations/alembic/versions_gxy/ddbdbc40bdc1_add_workflow_comment_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/migrations/alembic/versions_gxy/e0561d5fc8c7_add_archived_columns_to_history.py
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/migrations/alembic/versions_gxy/e0e3bb173ee6_add_column_deleted_to_api_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/migrations/alembic/versions_gxy/e7b6dcb09efd_create_gxy_branch.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/migrations/alembic/versions_gxy/e93c5d0b47a9_alter_column_external_user_id.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:53:47.000000 galaxy-data-23.2.1/galaxy/model/migrations/alembic/versions_tsi/
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/migrations/alembic/versions_tsi/d4a650f47a3c_create_tsi_branch.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/migrations/alembic.ini
--rw-r--r--   0 runner    (1001) docker     (127)    15662 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/migrations/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/migrations/dbscript.py
--rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/migrations/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9120 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/migrations/scripts.py
--rw-r--r--   0 runner    (1001) docker     (127)    14878 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/migrations/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/none_like.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:53:47.000000 galaxy-data-23.2.1/galaxy/model/orm/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/orm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4834 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/orm/engine_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/orm/now.py
--rw-r--r--   0 runner    (1001) docker     (127)     6154 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/orm/scripts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/orm/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/scoped_session.py
--rw-r--r--   0 runner    (1001) docker     (127)    82210 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/security.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:53:47.000000 galaxy-data-23.2.1/galaxy/model/store/
--rw-r--r--   0 runner    (1001) docker     (127)   139905 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/store/_bco_convert_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/store/build_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)    41412 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/store/discover.py
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/store/load_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)    17526 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/store/ro_crate_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    20976 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/tags.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:53:47.000000 galaxy-data-23.2.1/galaxy/model/tool_shed_install/
--rw-r--r--   0 runner    (1001) docker     (127)    33197 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/tool_shed_install/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/tool_shed_install/mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:53:47.000000 galaxy-data-23.2.1/galaxy/model/triggers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/triggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5558 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/triggers/history_update_time_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     6135 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/triggers/update_audit_table.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/triggers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:53:47.000000 galaxy-data-23.2.1/galaxy/model/unittest_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/unittest_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/unittest_utils/beaker_testing_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/unittest_utils/data_app.py
--rw-r--r--   0 runner    (1001) docker     (127)    29112 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/unittest_utils/gxy_model_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/unittest_utils/mapping_testing_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/unittest_utils/migration_scripts_testing_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8070 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/unittest_utils/model_testing_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10637 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/unittest_utils/store_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/model/unittest_utils/tsi_model_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:53:47.000000 galaxy-data-23.2.1/galaxy/quota/
--rw-r--r--   0 runner    (1001) docker     (127)    12545 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/quota/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7762 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/quota/_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:53:47.000000 galaxy-data-23.2.1/galaxy/security/
--rw-r--r--   0 runner    (1001) docker     (127)     6309 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/security/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6327 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/security/idencoding.py
--rw-r--r--   0 runner    (1001) docker     (127)    18691 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/security/object_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/security/passwords.py
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/security/ssh_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     6689 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/security/validate_user_input.py
--rw-r--r--   0 runner    (1001) docker     (127)    10115 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/galaxy/security/vault.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:53:47.000000 galaxy-data-23.2.1/galaxy_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    25976 2024-02-22 03:53:47.000000 galaxy-data-23.2.1/galaxy_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14941 2024-02-22 03:53:47.000000 galaxy-data-23.2.1/galaxy_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 03:53:47.000000 galaxy-data-23.2.1/galaxy_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-02-22 03:53:47.000000 galaxy-data-23.2.1/galaxy_data.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-02-22 03:53:47.000000 galaxy-data-23.2.1/galaxy_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-22 03:53:47.000000 galaxy-data-23.2.1/galaxy_data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-02-22 03:53:47.000000 galaxy-data-23.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-22 03:50:43.000000 galaxy-data-23.2.1/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:12.931122 galaxy-data-24.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    33710 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    35958 2024-04-03 02:45:12.931122 galaxy-data-24.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:12.875121 galaxy-data-24.0.0/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:12.883122 galaxy-data-24.0.0/galaxy/datatypes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6770 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/anvio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8962 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/assembly.py
+-rw-r--r--   0 runner    (1001) docker     (127)   166979 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/binary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22475 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/blast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4654 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/checkers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/chrominfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33379 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/constructive_solid_geometry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:12.899122 galaxy-data-24.0.0/galaxy/datatypes/converters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/bam_to_bai.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/bam_to_bigwig_converter.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/bcf_bcf_uncompressed_converter.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/bed_gff_or_vcf_to_bigwig_converter.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/bed_to_fli_converter.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/bed_to_gff_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/bed_to_gff_converter.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/bed_to_interval_index_converter.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/bedgraph_to_bigwig_converter.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/bigwig_to_wig_converter.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/biom.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/bz2_to_uncompressed.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/cml_to_smi_converter.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/cram_to_bam_converter.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/csv_to_tabular.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/fasta_to_2bit.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/fasta_to_bowtie_base_index_converter.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/fasta_to_bowtie_color_index_converter.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/fasta_to_fai.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/fasta_to_len.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/fasta_to_len.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/fasta_to_tabular_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/fasta_to_tabular_converter.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/fastq_to_fqtoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/fastq_to_fqtoc.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/fastqsolexa_to_fasta_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/fastqsolexa_to_fasta_converter.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/fastqsolexa_to_qual_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/fastqsolexa_to_qual_converter.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/gff_to_bed_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/gff_to_bed_converter.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/gff_to_fli_converter.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/gff_to_interval_index_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/gff_to_interval_index_converter.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/gro_to_pdb.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/gz_to_uncompressed.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/inchi_to_mol_converter.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/interval_to_bed12_converter.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/interval_to_bed6_converter.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/interval_to_bed_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/interval_to_bed_converter.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     9402 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/interval_to_bedstrict_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/interval_to_bedstrict_converter.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/interval_to_bgzip_converter.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/interval_to_bigwig_converter.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/interval_to_fli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/interval_to_interval_index_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/interval_to_interval_index_converter.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4590 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/interval_to_tabix_converter.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/len_to_linecount.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/lped_to_fped_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/lped_to_fped_converter.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/lped_to_pbed_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/lped_to_pbed_converter.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/maf_to_fasta_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/maf_to_fasta_converter.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/maf_to_interval_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/maf_to_interval_converter.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/mdconvert.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/mol2_to_mol_converter.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    11846 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/molecules_converter.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/neostorezip_to_neostore_converter.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/parquet_to_csv_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/parquet_to_csv_converter.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/pbed_ldreduced_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/pbed_ldreduced_converter.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/pbed_to_lped_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/pbed_to_lped_converter.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/pdb_to_gro.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/picard_interval_list_to_bed6_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/picard_interval_list_to_bed6_converter.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/pileup_to_interval_index_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/pileup_to_interval_index_converter.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/ref_to_seq_taxonomy_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/ref_to_seq_taxonomy_converter.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/sam_to_bigwig_converter.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/sam_to_unsorted_bam.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/smi_to_mol_converter.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/smi_to_smi_converter.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/tabular_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/tabular_to_csv.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/tabular_to_dbnsfp.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/tar_to_directory.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/to_coordinate_sorted_bam.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/to_qname_sorted_bam.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/uncompressed_to_gz.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/vcf_bgzip_to_tabix_converter.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/vcf_to_interval_index_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/vcf_to_interval_index_converter.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/vcf_to_vcf_bgzip_converter.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/wig_to_bigwig_converter.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/wiggle_to_simple_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/converters/wiggle_to_simple_converter.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/coverage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54956 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:12.899122 galaxy-data-24.0.0/galaxy/datatypes/dataproviders/
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/dataproviders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12014 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/dataproviders/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/dataproviders/chunk.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13756 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/dataproviders/column.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29824 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/dataproviders/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6614 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/dataproviders/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/dataproviders/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5869 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/dataproviders/external.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5196 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/dataproviders/hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9435 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/dataproviders/line.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:12.903122 galaxy-data-24.0.0/galaxy/datatypes/display_applications/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/display_applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15530 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/display_applications/application.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:12.867121 galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:12.903122 galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/biom/
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/biom/biom_simple.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:12.903122 galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/ensembl/
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/ensembl/ensembl_bam.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/ensembl/ensembl_gff.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/ensembl/ensembl_interval_as_bed.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:12.903122 galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/gbrowse/
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/gbrowse/gbrowse_gff.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/gbrowse/gbrowse_interval_as_bed.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/gbrowse/gbrowse_wig.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:12.903122 galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/icn3d/
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/icn3d/icn3d_simple.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:12.903122 galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/igb/
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/igb/bam.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/igb/bb.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/igb/bed.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/igb/bedgraph.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/igb/bigwig.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/igb/gtf.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/igb/wig.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:12.907122 galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/igv/
+-rw-r--r--   0 runner    (1001) docker     (127)     5123 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/igv/bam.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/igv/bigwig.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/igv/genbank.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/igv/genome_fasta.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/igv/gff.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4965 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/igv/interval_as_bed.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5383 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/igv/vcf.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:12.907122 galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/image/avivator.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:12.907122 galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/intermine/
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/intermine/intermine_simple.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:12.907122 galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/iobio/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/iobio/bam.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/iobio/vcf.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:12.907122 galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/minerva/
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/minerva/tabular.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:12.867121 galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/qiime/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:12.907122 galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/qiime/qiime2/
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/qiime/qiime2/q2view.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:12.907122 galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/rviewer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/rviewer/bed.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/rviewer/vcf.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:12.907122 galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/ucsc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/ucsc/bam.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/ucsc/bigbed.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/ucsc/bigwig.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/ucsc/interval_as_bed.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/ucsc/maf_customtrack.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      436 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/ucsc/trackhub.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/ucsc/vcf.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    13603 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/display_applications/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/display_applications/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:12.907122 galaxy-data-24.0.0/galaxy/datatypes/display_applications/xsd/
+-rw-r--r--   0 runner    (1001) docker     (127)    16714 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/display_applications/xsd/geda.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44071 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/genetics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/gis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21204 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/goldenpath.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6088 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15598 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83479 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/interval.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15574 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/isa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6736 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/larch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8420 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/metacyto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/microarrays.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55535 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/molecules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37917 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/mothur.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9885 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/msa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5676 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/neo4j.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/ngsindex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6424 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/phylip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/plant_tribes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36666 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/proteomics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10662 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/qiime2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/qualityscore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52231 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61232 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/set_metadata_tool.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    35867 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/sniff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7299 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/spaln.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3910 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/speech.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77880 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/tabular.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50320 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/tracks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7534 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/triples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/upload_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:12.911122 galaxy-data-24.0.0/galaxy/datatypes/util/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/util/generic_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19189 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/util/gff_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30671 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/util/maf_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9607 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/datatypes/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:12.911122 galaxy-data-24.0.0/galaxy/model/
+-rw-r--r--   0 runner    (1001) docker     (127)   446817 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7480 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12551 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/custom_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/database_heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/database_object_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7227 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/database_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:12.915122 galaxy-data-24.0.0/galaxy/model/dataset_collections/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/dataset_collections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5787 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/dataset_collections/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4617 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/dataset_collections/matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/dataset_collections/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7790 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/dataset_collections/structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/dataset_collections/subcollections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6601 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/dataset_collections/type_description.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:12.915122 galaxy-data-24.0.0/galaxy/model/dataset_collections/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/dataset_collections/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/dataset_collections/types/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/dataset_collections/types/paired.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12279 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/deferred.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/index_filter_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8519 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/item_attrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28981 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:12.915122 galaxy-data-24.0.0/galaxy/model/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/migrations/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13225 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:12.915122 galaxy-data-24.0.0/galaxy/model/migrations/alembic/
+-rw-r--r--   0 runner    (1001) docker     (127)     4511 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/migrations/alembic/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/migrations/alembic/script.py.mako
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:12.919122 galaxy-data-24.0.0/galaxy/model/migrations/alembic/versions_gxy/
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/migrations/alembic/versions_gxy/186d4835587b_drop_job_state_history_update_time_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/migrations/alembic/versions_gxy/2d749563e1fe_add_notification_system_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/migrations/alembic/versions_gxy/2dc3386d091f_add_indexes_for_workflow_comment_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/migrations/alembic/versions_gxy/3100452fa030_add_workflow_invocation_message_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/migrations/alembic/versions_gxy/3356bc2ecfc4_drop_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/migrations/alembic/versions_gxy/3a2914d703ca_add_index_wf_r_s_s__workflow_invocation_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/migrations/alembic/versions_gxy/460d0ecd1dd8_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/migrations/alembic/versions_gxy/518c8438a91b_add_when_expression_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/migrations/alembic/versions_gxy/55f02fd8ab6c_add_index_on_hda_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/migrations/alembic/versions_gxy/59e024ceaca1_add_export_association_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/migrations/alembic/versions_gxy/6a67bf27e6a6_deferred_data_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/migrations/alembic/versions_gxy/8a19186a6ee7_add_columns_to_interactivetool_entry_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/migrations/alembic/versions_gxy/92fb564c7095_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/migrations/alembic/versions_gxy/9540a051226e_preferred_object_store_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/migrations/alembic/versions_gxy/987ce9839ecb_create_celery_user_rate_limit_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/migrations/alembic/versions_gxy/b182f655505f_add_workflow_source_metadata_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/migrations/alembic/versions_gxy/b855b714e8b8_make_api_keys_deleted_non_nullable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/migrations/alembic/versions_gxy/c39f1de47a04_add_skipped_state_to_collection_job_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/migrations/alembic/versions_gxy/caa7742f7bca_add_index_wf_r_i_p__workflow_invocation_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/migrations/alembic/versions_gxy/d0583094c8cd_add_quota_source_labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/migrations/alembic/versions_gxy/ddbdbc40bdc1_add_workflow_comment_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/migrations/alembic/versions_gxy/e0561d5fc8c7_add_archived_columns_to_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/migrations/alembic/versions_gxy/e0e3bb173ee6_add_column_deleted_to_api_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/migrations/alembic/versions_gxy/e7b6dcb09efd_create_gxy_branch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/migrations/alembic/versions_gxy/e93c5d0b47a9_alter_column_external_user_id.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:12.919122 galaxy-data-24.0.0/galaxy/model/migrations/alembic/versions_tsi/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/migrations/alembic/versions_tsi/d4a650f47a3c_create_tsi_branch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/migrations/alembic.ini
+-rw-r--r--   0 runner    (1001) docker     (127)    15613 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/migrations/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/migrations/dbscript.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/migrations/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9159 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/migrations/scripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14838 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/migrations/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/none_like.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:12.923122 galaxy-data-24.0.0/galaxy/model/orm/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/orm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4847 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/orm/engine_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/orm/now.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6155 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/orm/scripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/orm/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/scoped_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83103 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/security.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:12.923122 galaxy-data-24.0.0/galaxy/model/store/
+-rw-r--r--   0 runner    (1001) docker     (127)   140517 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/store/_bco_convert_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/store/build_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41755 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/store/discover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/store/load_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17526 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/store/ro_crate_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20954 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/tags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:12.923122 galaxy-data-24.0.0/galaxy/model/tool_shed_install/
+-rw-r--r--   0 runner    (1001) docker     (127)    33142 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/tool_shed_install/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/tool_shed_install/mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:12.923122 galaxy-data-24.0.0/galaxy/model/triggers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/triggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5558 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/triggers/history_update_time_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6135 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/triggers/update_audit_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/triggers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:12.927122 galaxy-data-24.0.0/galaxy/model/unittest_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/unittest_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/unittest_utils/beaker_testing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/unittest_utils/data_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29112 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/unittest_utils/gxy_model_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/unittest_utils/mapping_testing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/unittest_utils/migration_scripts_testing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8105 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/unittest_utils/model_testing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10638 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/unittest_utils/store_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/model/unittest_utils/tsi_model_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:12.927122 galaxy-data-24.0.0/galaxy/quota/
+-rw-r--r--   0 runner    (1001) docker     (127)    16856 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/quota/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7995 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/quota/_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:12.927122 galaxy-data-24.0.0/galaxy/security/
+-rw-r--r--   0 runner    (1001) docker     (127)     6421 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/security/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6327 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/security/idencoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18674 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/security/object_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/security/passwords.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/security/ssh_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6679 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/security/validate_user_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10115 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/galaxy/security/vault.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:12.931122 galaxy-data-24.0.0/galaxy_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    35958 2024-04-03 02:45:12.000000 galaxy-data-24.0.0/galaxy_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15124 2024-04-03 02:45:12.000000 galaxy-data-24.0.0/galaxy_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 02:45:12.000000 galaxy-data-24.0.0/galaxy_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-03 02:45:12.000000 galaxy-data-24.0.0/galaxy_data.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-03 02:45:12.000000 galaxy-data-24.0.0/galaxy_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 02:45:12.000000 galaxy-data-24.0.0/galaxy_data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-03 02:45:12.931122 galaxy-data-24.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 02:43:42.000000 galaxy-data-24.0.0/test-requirements.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `galaxy-data-23.2.1/HISTORY.rst` & `galaxy-data-24.0.0/HISTORY.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,83 @@
 History
 -------
 
 .. to_doc
 
 -------------------
+24.0.0 (2024-04-02)
+-------------------
+
+
+=========
+Bug fixes
+=========
+
+* Fix for converter tests by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#17188 <https://github.com/galaxyproject/galaxy/pull/17188>`_
+* correct dbkey for minerva display app by `@hexylena <https://github.com/hexylena>`_ in `#17196 <https://github.com/galaxyproject/galaxy/pull/17196>`_
+* Fix invocation serialization if no state was set by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17278 <https://github.com/galaxyproject/galaxy/pull/17278>`_
+* Fix quotas ID encoding by `@davelopez <https://github.com/davelopez>`_ in `#17335 <https://github.com/galaxyproject/galaxy/pull/17335>`_
+* Fix model store exports that include implicit conversions.  by `@jmchilton <https://github.com/jmchilton>`_ in `#17346 <https://github.com/galaxyproject/galaxy/pull/17346>`_
+* Fix bug: create new PSAAssociation if not in database by `@jdavcs <https://github.com/jdavcs>`_ in `#17516 <https://github.com/galaxyproject/galaxy/pull/17516>`_
+* Fix social_core methods by `@jdavcs <https://github.com/jdavcs>`_ in `#17530 <https://github.com/galaxyproject/galaxy/pull/17530>`_
+* Fix ancient bug: incorrect usage of func.coalesce in User model by `@jdavcs <https://github.com/jdavcs>`_ in `#17577 <https://github.com/galaxyproject/galaxy/pull/17577>`_
+* Account for newlines in CIF Datatype sniffer by `@patrick-austin <https://github.com/patrick-austin>`_ in `#17582 <https://github.com/galaxyproject/galaxy/pull/17582>`_
+* Anticipate PendingRollbackError in ``check_database_connection`` by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17598 <https://github.com/galaxyproject/galaxy/pull/17598>`_
+* Add basic model import attribute validation by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17628 <https://github.com/galaxyproject/galaxy/pull/17628>`_
+* More efficient change_state queries, maybe fix deadlock by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17632 <https://github.com/galaxyproject/galaxy/pull/17632>`_
+* Npz sniffing: do not read the whole file by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#17672 <https://github.com/galaxyproject/galaxy/pull/17672>`_
+* Assert that at least one file in npz zipfile ends with .npy by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17679 <https://github.com/galaxyproject/galaxy/pull/17679>`_
+* Workflow Comment Indexing by `@ElectronicBlueberry <https://github.com/ElectronicBlueberry>`_ in `#17700 <https://github.com/galaxyproject/galaxy/pull/17700>`_
+* Fix source history update_time being updated when importing a public history by `@jmchilton <https://github.com/jmchilton>`_ in `#17728 <https://github.com/galaxyproject/galaxy/pull/17728>`_
+* Also set extension and metadata on copies of job outputs when finishing job by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17777 <https://github.com/galaxyproject/galaxy/pull/17777>`_
+* Defer job attributes that are usually not needed by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17795 <https://github.com/galaxyproject/galaxy/pull/17795>`_
+* Fix change_datatype PJA for dynamic collections  by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17803 <https://github.com/galaxyproject/galaxy/pull/17803>`_
+* Simplify nested collection joins by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17817 <https://github.com/galaxyproject/galaxy/pull/17817>`_
+* Fix very slow user data table query by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17830 <https://github.com/galaxyproject/galaxy/pull/17830>`_
+* Update db revision 24.0 release tags by `@jdavcs <https://github.com/jdavcs>`_ in `#17834 <https://github.com/galaxyproject/galaxy/pull/17834>`_
+* Minor refactor of query building logic for readability by `@jdavcs <https://github.com/jdavcs>`_ in `#17835 <https://github.com/galaxyproject/galaxy/pull/17835>`_
+* Fix user login when duplicate UserRoleAssociation exists by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17854 <https://github.com/galaxyproject/galaxy/pull/17854>`_
+
+============
+Enhancements
+============
+
+* Make columns types an empty list for empty tabular data  by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#13918 <https://github.com/galaxyproject/galaxy/pull/13918>`_
+* port invocation API to fastapi by `@martenson <https://github.com/martenson>`_ in `#16707 <https://github.com/galaxyproject/galaxy/pull/16707>`_
+* SQLAlchemy 2.0 upgrades (part 5) by `@jdavcs <https://github.com/jdavcs>`_ in `#16932 <https://github.com/galaxyproject/galaxy/pull/16932>`_
+* Python 3.8 as minimum by `@mr-c <https://github.com/mr-c>`_ in `#16954 <https://github.com/galaxyproject/galaxy/pull/16954>`_
+*  Expose more tool information / navigability in UI. by `@jmchilton <https://github.com/jmchilton>`_ in `#17105 <https://github.com/galaxyproject/galaxy/pull/17105>`_
+* Add support for (fast5.tar).xz binary compressed files by `@tuncK <https://github.com/tuncK>`_ in `#17106 <https://github.com/galaxyproject/galaxy/pull/17106>`_
+* SA2.0 updates: handling "object is being merged into a Session along the backref cascade path" by `@jdavcs <https://github.com/jdavcs>`_ in `#17122 <https://github.com/galaxyproject/galaxy/pull/17122>`_
+* Towards SQLAlchemy 2.0: fix last cases of RemovedIn20Warning by `@jdavcs <https://github.com/jdavcs>`_ in `#17132 <https://github.com/galaxyproject/galaxy/pull/17132>`_
+* Create pydantic model for the return of show operation -  get: `/api/jobs/{job_id}`  by `@heisner-tillman <https://github.com/heisner-tillman>`_ in `#17153 <https://github.com/galaxyproject/galaxy/pull/17153>`_
+* Much simpler default dataset permissions for typical users. by `@jmchilton <https://github.com/jmchilton>`_ in `#17166 <https://github.com/galaxyproject/galaxy/pull/17166>`_
+* Add future=True flag to SA engine by `@jdavcs <https://github.com/jdavcs>`_ in `#17174 <https://github.com/galaxyproject/galaxy/pull/17174>`_
+* Add future=True flag to SA session by `@jdavcs <https://github.com/jdavcs>`_ in `#17179 <https://github.com/galaxyproject/galaxy/pull/17179>`_
+* Vueifiy History Grids by `@guerler <https://github.com/guerler>`_ in `#17219 <https://github.com/galaxyproject/galaxy/pull/17219>`_
+* Convert sample object store configuration to YAML and support configuring inline by `@natefoo <https://github.com/natefoo>`_ in `#17222 <https://github.com/galaxyproject/galaxy/pull/17222>`_
+* Migrate models to pydantic 2 by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17262 <https://github.com/galaxyproject/galaxy/pull/17262>`_
+* API endpoint that allows "changing" the objectstore for "safe" scenarios.  by `@jmchilton <https://github.com/jmchilton>`_ in `#17329 <https://github.com/galaxyproject/galaxy/pull/17329>`_
+* Enable ``warn_unreachable`` mypy option by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17365 <https://github.com/galaxyproject/galaxy/pull/17365>`_
+* Fix type annotation of code using XML etree by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17367 <https://github.com/galaxyproject/galaxy/pull/17367>`_
+* Add explicit cache_ok attribute to JSONType subclass by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17376 <https://github.com/galaxyproject/galaxy/pull/17376>`_
+* More specific type annotation for ``BaseJobExec.parse_status()`` by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17381 <https://github.com/galaxyproject/galaxy/pull/17381>`_
+* Update to black 2024 stable style by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17391 <https://github.com/galaxyproject/galaxy/pull/17391>`_
+* Allow using tool data bundles as inputs to reference data select parameters by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17435 <https://github.com/galaxyproject/galaxy/pull/17435>`_
+* UI for "relocating" a dataset to a new object store (when safe) by `@jmchilton <https://github.com/jmchilton>`_ in `#17437 <https://github.com/galaxyproject/galaxy/pull/17437>`_
+* Allow filtering history datasets by object store ID and quota source. by `@jmchilton <https://github.com/jmchilton>`_ in `#17460 <https://github.com/galaxyproject/galaxy/pull/17460>`_
+* Faster FASTA and FASTQ metadata setting by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#17462 <https://github.com/galaxyproject/galaxy/pull/17462>`_
+* Feature SBOL datatypes by `@guillaume-gricourt <https://github.com/guillaume-gricourt>`_ in `#17482 <https://github.com/galaxyproject/galaxy/pull/17482>`_
+* Display workflow invocation counts. by `@jmchilton <https://github.com/jmchilton>`_ in `#17488 <https://github.com/galaxyproject/galaxy/pull/17488>`_
+* add npy datatype by `@astrovsky01 <https://github.com/astrovsky01>`_ in `#17517 <https://github.com/galaxyproject/galaxy/pull/17517>`_
+* Enhance Avivator display app to support regular Tiffs by `@davelopez <https://github.com/davelopez>`_ in `#17554 <https://github.com/galaxyproject/galaxy/pull/17554>`_
+* Update Python dependencies by `@galaxybot <https://github.com/galaxybot>`_ in `#17580 <https://github.com/galaxyproject/galaxy/pull/17580>`_
+* Add migrations revision identifier for 24.0 by `@jdavcs <https://github.com/jdavcs>`_ in `#17589 <https://github.com/galaxyproject/galaxy/pull/17589>`_
+
+-------------------
 23.2.1 (2024-02-21)
 -------------------
 
 
 =========
 Bug fixes
 =========
```

### Comparing `galaxy-data-23.2.1/LICENSE` & `galaxy-data-24.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/PKG-INFO` & `galaxy-data-24.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,64 @@
 Metadata-Version: 2.1
 Name: galaxy-data
-Version: 23.2.1
+Version: 24.0.0
 Summary: Galaxy datatype framework and datatypes
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Academic Free License (AFL)
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Software Development :: Testing
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: galaxy-files
+Requires-Dist: galaxy-objectstore
+Requires-Dist: galaxy-tool-util
+Requires-Dist: galaxy-util[template]
+Requires-Dist: alembic
+Requires-Dist: alembic-utils
+Requires-Dist: bdbag>=1.6.3
+Requires-Dist: bx-python
+Requires-Dist: dnspython
+Requires-Dist: galaxy-sequence-utils
+Requires-Dist: h5grove>=1.2.1
+Requires-Dist: h5py
+Requires-Dist: isa-rwval>=0.10.10
+Requires-Dist: isal
+Requires-Dist: MarkupSafe
+Requires-Dist: msal
+Requires-Dist: mrcfile
+Requires-Dist: numpy
+Requires-Dist: parsley
+Requires-Dist: pycryptodome
+Requires-Dist: pydantic[email]!=2.6.0,!=2.6.1,>=2
+Requires-Dist: pylibmagic
+Requires-Dist: python-magic
+Requires-Dist: pysam>=0.21
+Requires-Dist: rocrate
+Requires-Dist: social-auth-core[openidconnect]==4.0.3
+Requires-Dist: SQLAlchemy<2,>=1.4.25
+Requires-Dist: tifffile
+Requires-Dist: typing-extensions
+Requires-Dist: WebOb
 
 
 .. image:: https://badge.fury.io/py/galaxy-data.svg
    :target: https://pypi.org/project/galaxy-data/
 
 
 Overview
@@ -42,14 +72,84 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+24.0.0 (2024-04-02)
+-------------------
+
+
+=========
+Bug fixes
+=========
+
+* Fix for converter tests by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#17188 <https://github.com/galaxyproject/galaxy/pull/17188>`_
+* correct dbkey for minerva display app by `@hexylena <https://github.com/hexylena>`_ in `#17196 <https://github.com/galaxyproject/galaxy/pull/17196>`_
+* Fix invocation serialization if no state was set by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17278 <https://github.com/galaxyproject/galaxy/pull/17278>`_
+* Fix quotas ID encoding by `@davelopez <https://github.com/davelopez>`_ in `#17335 <https://github.com/galaxyproject/galaxy/pull/17335>`_
+* Fix model store exports that include implicit conversions.  by `@jmchilton <https://github.com/jmchilton>`_ in `#17346 <https://github.com/galaxyproject/galaxy/pull/17346>`_
+* Fix bug: create new PSAAssociation if not in database by `@jdavcs <https://github.com/jdavcs>`_ in `#17516 <https://github.com/galaxyproject/galaxy/pull/17516>`_
+* Fix social_core methods by `@jdavcs <https://github.com/jdavcs>`_ in `#17530 <https://github.com/galaxyproject/galaxy/pull/17530>`_
+* Fix ancient bug: incorrect usage of func.coalesce in User model by `@jdavcs <https://github.com/jdavcs>`_ in `#17577 <https://github.com/galaxyproject/galaxy/pull/17577>`_
+* Account for newlines in CIF Datatype sniffer by `@patrick-austin <https://github.com/patrick-austin>`_ in `#17582 <https://github.com/galaxyproject/galaxy/pull/17582>`_
+* Anticipate PendingRollbackError in ``check_database_connection`` by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17598 <https://github.com/galaxyproject/galaxy/pull/17598>`_
+* Add basic model import attribute validation by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17628 <https://github.com/galaxyproject/galaxy/pull/17628>`_
+* More efficient change_state queries, maybe fix deadlock by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17632 <https://github.com/galaxyproject/galaxy/pull/17632>`_
+* Npz sniffing: do not read the whole file by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#17672 <https://github.com/galaxyproject/galaxy/pull/17672>`_
+* Assert that at least one file in npz zipfile ends with .npy by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17679 <https://github.com/galaxyproject/galaxy/pull/17679>`_
+* Workflow Comment Indexing by `@ElectronicBlueberry <https://github.com/ElectronicBlueberry>`_ in `#17700 <https://github.com/galaxyproject/galaxy/pull/17700>`_
+* Fix source history update_time being updated when importing a public history by `@jmchilton <https://github.com/jmchilton>`_ in `#17728 <https://github.com/galaxyproject/galaxy/pull/17728>`_
+* Also set extension and metadata on copies of job outputs when finishing job by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17777 <https://github.com/galaxyproject/galaxy/pull/17777>`_
+* Defer job attributes that are usually not needed by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17795 <https://github.com/galaxyproject/galaxy/pull/17795>`_
+* Fix change_datatype PJA for dynamic collections  by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17803 <https://github.com/galaxyproject/galaxy/pull/17803>`_
+* Simplify nested collection joins by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17817 <https://github.com/galaxyproject/galaxy/pull/17817>`_
+* Fix very slow user data table query by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17830 <https://github.com/galaxyproject/galaxy/pull/17830>`_
+* Update db revision 24.0 release tags by `@jdavcs <https://github.com/jdavcs>`_ in `#17834 <https://github.com/galaxyproject/galaxy/pull/17834>`_
+* Minor refactor of query building logic for readability by `@jdavcs <https://github.com/jdavcs>`_ in `#17835 <https://github.com/galaxyproject/galaxy/pull/17835>`_
+* Fix user login when duplicate UserRoleAssociation exists by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17854 <https://github.com/galaxyproject/galaxy/pull/17854>`_
+
+============
+Enhancements
+============
+
+* Make columns types an empty list for empty tabular data  by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#13918 <https://github.com/galaxyproject/galaxy/pull/13918>`_
+* port invocation API to fastapi by `@martenson <https://github.com/martenson>`_ in `#16707 <https://github.com/galaxyproject/galaxy/pull/16707>`_
+* SQLAlchemy 2.0 upgrades (part 5) by `@jdavcs <https://github.com/jdavcs>`_ in `#16932 <https://github.com/galaxyproject/galaxy/pull/16932>`_
+* Python 3.8 as minimum by `@mr-c <https://github.com/mr-c>`_ in `#16954 <https://github.com/galaxyproject/galaxy/pull/16954>`_
+*  Expose more tool information / navigability in UI. by `@jmchilton <https://github.com/jmchilton>`_ in `#17105 <https://github.com/galaxyproject/galaxy/pull/17105>`_
+* Add support for (fast5.tar).xz binary compressed files by `@tuncK <https://github.com/tuncK>`_ in `#17106 <https://github.com/galaxyproject/galaxy/pull/17106>`_
+* SA2.0 updates: handling "object is being merged into a Session along the backref cascade path" by `@jdavcs <https://github.com/jdavcs>`_ in `#17122 <https://github.com/galaxyproject/galaxy/pull/17122>`_
+* Towards SQLAlchemy 2.0: fix last cases of RemovedIn20Warning by `@jdavcs <https://github.com/jdavcs>`_ in `#17132 <https://github.com/galaxyproject/galaxy/pull/17132>`_
+* Create pydantic model for the return of show operation -  get: `/api/jobs/{job_id}`  by `@heisner-tillman <https://github.com/heisner-tillman>`_ in `#17153 <https://github.com/galaxyproject/galaxy/pull/17153>`_
+* Much simpler default dataset permissions for typical users. by `@jmchilton <https://github.com/jmchilton>`_ in `#17166 <https://github.com/galaxyproject/galaxy/pull/17166>`_
+* Add future=True flag to SA engine by `@jdavcs <https://github.com/jdavcs>`_ in `#17174 <https://github.com/galaxyproject/galaxy/pull/17174>`_
+* Add future=True flag to SA session by `@jdavcs <https://github.com/jdavcs>`_ in `#17179 <https://github.com/galaxyproject/galaxy/pull/17179>`_
+* Vueifiy History Grids by `@guerler <https://github.com/guerler>`_ in `#17219 <https://github.com/galaxyproject/galaxy/pull/17219>`_
+* Convert sample object store configuration to YAML and support configuring inline by `@natefoo <https://github.com/natefoo>`_ in `#17222 <https://github.com/galaxyproject/galaxy/pull/17222>`_
+* Migrate models to pydantic 2 by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17262 <https://github.com/galaxyproject/galaxy/pull/17262>`_
+* API endpoint that allows "changing" the objectstore for "safe" scenarios.  by `@jmchilton <https://github.com/jmchilton>`_ in `#17329 <https://github.com/galaxyproject/galaxy/pull/17329>`_
+* Enable ``warn_unreachable`` mypy option by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17365 <https://github.com/galaxyproject/galaxy/pull/17365>`_
+* Fix type annotation of code using XML etree by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17367 <https://github.com/galaxyproject/galaxy/pull/17367>`_
+* Add explicit cache_ok attribute to JSONType subclass by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17376 <https://github.com/galaxyproject/galaxy/pull/17376>`_
+* More specific type annotation for ``BaseJobExec.parse_status()`` by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17381 <https://github.com/galaxyproject/galaxy/pull/17381>`_
+* Update to black 2024 stable style by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17391 <https://github.com/galaxyproject/galaxy/pull/17391>`_
+* Allow using tool data bundles as inputs to reference data select parameters by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17435 <https://github.com/galaxyproject/galaxy/pull/17435>`_
+* UI for "relocating" a dataset to a new object store (when safe) by `@jmchilton <https://github.com/jmchilton>`_ in `#17437 <https://github.com/galaxyproject/galaxy/pull/17437>`_
+* Allow filtering history datasets by object store ID and quota source. by `@jmchilton <https://github.com/jmchilton>`_ in `#17460 <https://github.com/galaxyproject/galaxy/pull/17460>`_
+* Faster FASTA and FASTQ metadata setting by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#17462 <https://github.com/galaxyproject/galaxy/pull/17462>`_
+* Feature SBOL datatypes by `@guillaume-gricourt <https://github.com/guillaume-gricourt>`_ in `#17482 <https://github.com/galaxyproject/galaxy/pull/17482>`_
+* Display workflow invocation counts. by `@jmchilton <https://github.com/jmchilton>`_ in `#17488 <https://github.com/galaxyproject/galaxy/pull/17488>`_
+* add npy datatype by `@astrovsky01 <https://github.com/astrovsky01>`_ in `#17517 <https://github.com/galaxyproject/galaxy/pull/17517>`_
+* Enhance Avivator display app to support regular Tiffs by `@davelopez <https://github.com/davelopez>`_ in `#17554 <https://github.com/galaxyproject/galaxy/pull/17554>`_
+* Update Python dependencies by `@galaxybot <https://github.com/galaxybot>`_ in `#17580 <https://github.com/galaxyproject/galaxy/pull/17580>`_
+* Add migrations revision identifier for 24.0 by `@jdavcs <https://github.com/jdavcs>`_ in `#17589 <https://github.com/galaxyproject/galaxy/pull/17589>`_
+
+-------------------
 23.2.1 (2024-02-21)
 -------------------
 
 
 =========
 Bug fixes
 =========
```

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/_schema.py` & `galaxy-data-24.0.0/galaxy/datatypes/_schema.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,15 @@
     Optional,
 )
 
 from pydantic import (
     BaseModel,
     Field,
     HttpUrl,
+    RootModel,
 )
 
 
 class CompositeFileInfo(BaseModel):
     name: str = Field(..., title="Name", description="The name of this composite file")  # Mark this field as required
     optional: bool = Field(title="Optional", description="")  # TODO add description
     mimetype: Optional[str] = Field(title="MIME type", description="The MIME type of this file")
@@ -27,21 +28,21 @@
 
 
 class DatatypeDetails(BaseModel):
     extension: str = Field(
         ...,  # Mark this field as required
         title="Extension",
         description="The data type’s Dataset file extension",
-        example="bed",
+        examples=["bed"],
     )
     description: Optional[str] = Field(title="Description", description="A summary description for this data type")
     description_url: Optional[HttpUrl] = Field(
         title="Description URL",
         description="The URL to a detailed description for this datatype",
-        example="https://wiki.galaxyproject.org/Learn/Datatypes#Bed",
+        examples=["https://wiki.galaxyproject.org/Learn/Datatypes#Bed"],
     )
     display_in_upload: bool = Field(
         default=False,
         title="Display in upload",
         description="If True, the associated file extension will be displayed in the `File Format` select list in the `Upload File from your computer` tool in the `Get Data` tool section of the tool panel",
     )
     composite_files: Optional[List[CompositeFileInfo]] = Field(
@@ -81,51 +82,51 @@
 
 
 class DatatypeConverter(BaseModel):
     source: str = Field(
         ...,  # Mark this field as required
         title="Source",
         description="Source type for conversion",
-        example="bam",
+        examples=["bam"],
     )
     target: str = Field(
         ...,  # Mark this field as required
         title="Target",
         description="Target type for conversion",
-        example="bai",
+        examples=["bai"],
     )
     tool_id: str = Field(
         ...,  # Mark this field as required
         title="Tool identifier",
         description="The converter tool identifier",
-        example="CONVERTER_Bam_Bai_0",
+        examples=["CONVERTER_Bam_Bai_0"],
     )
 
 
-class DatatypeConverterList(BaseModel):
-    __root__: List[DatatypeConverter] = Field(title="List of data type converters", default=[])
+class DatatypeConverterList(RootModel):
+    root: List[DatatypeConverter] = Field(title="List of data type converters", default=[])
 
 
 class DatatypeEDAMDetails(BaseModel):
     prefix_IRI: str = Field(
         ...,  # Mark this field as required
         title="Prefix IRI",
         description="The EDAM prefixed Resource Identifier",
-        example="format_1782",
+        examples=["format_1782"],
     )
     label: Optional[str] = Field(
         title="Label",
         description="The EDAM label",
-        example="NCBI gene report format",
+        examples=["NCBI gene report format"],
     )
     definition: Optional[str] = Field(
         title="Definition",
         description="The EDAM definition",
-        example="Entry (gene) format of the NCBI database.",
+        examples=["Entry (gene) format of the NCBI database."],
     )
 
 
-class DatatypesEDAMDetailsDict(BaseModel):
-    __root__: Dict[str, DatatypeEDAMDetails] = Field(
+class DatatypesEDAMDetailsDict(RootModel):
+    root: Dict[str, DatatypeEDAMDetails] = Field(
         title="Dict of EDAM details for formats",
         default={},
     )
```

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/annotation.py` & `galaxy-data-24.0.0/galaxy/datatypes/annotation.py`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/anvio.py` & `galaxy-data-24.0.0/galaxy/datatypes/anvio.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Datatypes for Anvi'o
 https://github.com/merenlab/anvio
 """
+
 import glob
 import logging
 import os
 from typing import Optional
 
 from galaxy.datatypes.metadata import MetadataElement
 from galaxy.datatypes.protocols import (
```

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/assembly.py` & `galaxy-data-24.0.0/galaxy/datatypes/assembly.py`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/binary.py` & `galaxy-data-24.0.0/galaxy/datatypes/binary.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,14 +85,15 @@
     nice_size,
     sqlite,
     UNKNOWN,
 )
 from galaxy.util.checkers import (
     is_bz2,
     is_gzip,
+    is_xz,
 )
 from . import (
     data,
     dataproviders,
 )
 
 # Optional dependency to enable better metadata support in FITS datatype
@@ -1487,19 +1488,17 @@
                 if isinstance(tmp, (h5py.Dataset, h5py.Datatype)):
                     if "index" in tmp.dtype.names:
                         return tmp["index"]
                     if "_index" in tmp.dtype.names:
                         return tmp["_index"]
                     return None
                 else:
-                    index_var = tmp.attrs.get("index")
-                    if index_var is not None:
+                    if (index_var := tmp.attrs.get("index")) is not None:
                         return tmp[index_var]
-                    index_var = tmp.attrs.get("_index")
-                    if index_var is not None:
+                    if (index_var := tmp.attrs.get("_index")) is not None:
                         return tmp[index_var]
                     return None
 
             def _layercountsize(tmp, lennames=0):
                 "From TMP and LENNAMES, return layers, their number, and the length of one of the layers (all equal)."
                 if hasattr(tmp, "dtype"):
                     layers = list(tmp.dtype.names)
@@ -3683,14 +3682,17 @@
     """
     Class describing a gzip-compressed FAST5 archive
 
     >>> from galaxy.datatypes.sniff import get_test_fname
     >>> fname = get_test_fname('test.fast5.tar.gz')
     >>> Fast5ArchiveGz().sniff(fname)
     True
+    >>> fname = get_test_fname('test.fast5.tar.xz')
+    >>> Fast5ArchiveGz().sniff(fname)
+    False
     >>> fname = get_test_fname('test.fast5.tar.bz2')
     >>> Fast5ArchiveGz().sniff(fname)
     False
     >>> fname = get_test_fname('test.fast5.tar')
     >>> Fast5ArchiveGz().sniff(fname)
     False
     """
@@ -3699,22 +3701,52 @@
 
     def sniff(self, filename: str) -> bool:
         if not is_gzip(filename):
             return False
         return Fast5Archive.sniff(self, filename)
 
 
+class Fast5ArchiveXz(Fast5Archive):
+    """
+    Class describing a xz-compressed FAST5 archive
+
+    >>> from galaxy.datatypes.sniff import get_test_fname
+    >>> fname = get_test_fname('test.fast5.tar.gz')
+    >>> Fast5ArchiveXz().sniff(fname)
+    False
+    >>> fname = get_test_fname('test.fast5.tar.xz')
+    >>> Fast5ArchiveXz().sniff(fname)
+    True
+    >>> fname = get_test_fname('test.fast5.tar.bz2')
+    >>> Fast5ArchiveXz().sniff(fname)
+    False
+    >>> fname = get_test_fname('test.fast5.tar')
+    >>> Fast5ArchiveXz().sniff(fname)
+    False
+    """
+
+    file_ext = "fast5.tar.xz"
+
+    def sniff(self, filename: str) -> bool:
+        if not is_xz(filename):
+            return False
+        return Fast5Archive.sniff(self, filename)
+
+
 class Fast5ArchiveBz2(Fast5Archive):
     """
     Class describing a bzip2-compressed FAST5 archive
 
     >>> from galaxy.datatypes.sniff import get_test_fname
     >>> fname = get_test_fname('test.fast5.tar.bz2')
     >>> Fast5ArchiveBz2().sniff(fname)
     True
+    >>> fname = get_test_fname('test.fast5.tar.xz')
+    >>> Fast5ArchiveBz2().sniff(fname)
+    False
     >>> fname = get_test_fname('test.fast5.tar.gz')
     >>> Fast5ArchiveBz2().sniff(fname)
     False
     >>> fname = get_test_fname('test.fast5.tar')
     >>> Fast5ArchiveBz2().sniff(fname)
     False
     """
@@ -4293,19 +4325,17 @@
     MetadataElement(name="files", default=[], desc="files", readonly=True, visible=True, no_value=[])
 
     def __init__(self, **kwd):
         super().__init__(**kwd)
 
     def sniff(self, filename: str) -> bool:
         try:
-            npz = np.load(filename)
-            if isinstance(npz, np.lib.npyio.NpzFile):
-                for f in npz.files:
-                    if isinstance(npz[f], np.ndarray):
-                        return True
+            with np.load(filename) as npz:
+                if isinstance(npz, np.lib.npyio.NpzFile) and any(f.filename.endswith(".npy") for f in npz.zip.filelist):
+                    return True
         except Exception:
             return False
         return False
 
     def set_meta(self, dataset: DatasetProtocol, overwrite: bool = True, **kwd) -> None:
         try:
             with np.load(dataset.get_file_name()) as npz:
@@ -4536,7 +4566,62 @@
             dataset.blurb = "file purged from disk"
 
     def display_peek(self, dataset: DatasetProtocol) -> str:
         try:
             return dataset.peek
         except Exception:
             return f"Binary FITS file size ({nice_size(dataset.get_size())})"
+
+
+@build_sniff_from_prefix
+class Numpy(Binary):
+    """
+    Class defining a numpy data file
+
+    >>> from galaxy.datatypes.sniff import get_test_fname
+    >>> fname = get_test_fname('test.npy')
+    >>> Numpy().sniff(fname)
+    True
+    """
+
+    file_ext = "npy"
+
+    MetadataElement(
+        name="version_str",
+        default="",
+        param=MetadataParameter,
+        desc="Version string for the numpy file format",
+        readonly=True,
+        visible=True,
+        no_value=0,
+        optional=True,
+    )
+
+    def _numpy_version_string(self, filename):
+        magic_string = open(filename, "rb").read(8)
+        version_str = f"{magic_string[6]}.{magic_string[7]}"
+        return version_str
+
+    def set_meta(self, dataset: DatasetProtocol, overwrite: bool = True, **kwd) -> None:
+        try:
+            dataset.metadata.version_str = self._numpy_version_string(dataset.get_file_name())
+        except Exception as e:
+            log.warning("%s, set_meta Exception: %s", self, e)
+
+    def sniff_prefix(self, file_prefix: FilePrefix) -> bool:
+        # The first 6 bytes of any numpy file is '\x93NUMPY', with following bytes for version
+        # number of file formats, and info about header data. The rest of the file contains binary data.
+        return file_prefix.startswith_bytes(b"\x93NUMPY")
+
+    def set_peek(self, dataset: DatasetProtocol, **kwd) -> None:
+        if not dataset.dataset.purged:
+            dataset.peek = f"Binary numpy file version {dataset.metadata.version_str}"
+            dataset.blurb = nice_size(dataset.get_size())
+        else:
+            dataset.peek = "file does not exist"
+            dataset.blurb = "file purged from disk"
+
+    def display_peek(self, dataset: DatasetProtocol) -> str:
+        try:
+            return dataset.peek
+        except Exception:
+            return "Binary numpy file (%s)" % (nice_size(dataset.get_size()))
```

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/blast.py` & `galaxy-data-24.0.0/galaxy/datatypes/blast.py`

 * *Files 0% similar despite different names*

```diff
@@ -257,15 +257,15 @@
 
     @staticmethod
     def merge(split_files: List[str], output_file: str) -> None:
         """Merge BLAST databases (not implemented for now)."""
         raise NotImplementedError("Merging BLAST databases is non-trivial (do this via makeblastdb?)")
 
     @classmethod
-    def split(cls, input_datasets: List, subdir_generator_function: Callable, split_params: Dict) -> None:
+    def split(cls, input_datasets: List, subdir_generator_function: Callable, split_params: Optional[Dict]) -> None:
         """Split a BLAST database (not implemented for now)."""
         if split_params is None:
             return None
         raise NotImplementedError("Can't split BLAST databases")
 
 
 class BlastNucDb(_BlastDb):
```

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/chain.py` & `galaxy-data-24.0.0/galaxy/datatypes/chain.py`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/constructive_solid_geometry.py` & `galaxy-data-24.0.0/galaxy/datatypes/constructive_solid_geometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,14 +189,15 @@
 
     Binary data must be placed into the file immediately after the newline
     ('\\n') character from the previous ASCII keyword and parameter sequence.
 
     TODO: only legacy formats are currently supported and support for XML formats
     should be added.
     """
+
     subtype = ""
     # Add metadata elements.
     MetadataElement(name="vtk_version", default=None, desc="Vtk version", readonly=True, optional=True, visible=True)
     MetadataElement(name="file_format", default=None, desc="File format", readonly=True, optional=True, visible=True)
     MetadataElement(name="dataset_type", default=None, desc="Dataset type", readonly=True, optional=True, visible=True)
 
     # STRUCTURED_GRID data_type.
```

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/bam_to_bai.xml` & `galaxy-data-24.0.0/galaxy/datatypes/converters/bam_to_bai.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/bam_to_bigwig_converter.xml` & `galaxy-data-24.0.0/galaxy/datatypes/converters/bam_to_bigwig_converter.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/bcf_bcf_uncompressed_converter.xml` & `galaxy-data-24.0.0/galaxy/datatypes/converters/bcf_bcf_uncompressed_converter.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/bed_gff_or_vcf_to_bigwig_converter.xml` & `galaxy-data-24.0.0/galaxy/datatypes/converters/bed_gff_or_vcf_to_bigwig_converter.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/bed_to_fli_converter.xml` & `galaxy-data-24.0.0/galaxy/datatypes/converters/bed_to_fli_converter.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/bed_to_gff_converter.py` & `galaxy-data-24.0.0/galaxy/datatypes/converters/bed_to_gff_converter.py`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/bed_to_gff_converter.xml` & `galaxy-data-24.0.0/galaxy/datatypes/converters/bed_to_gff_converter.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/bed_to_interval_index_converter.xml` & `galaxy-data-24.0.0/galaxy/datatypes/converters/bed_to_interval_index_converter.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/bedgraph_to_bigwig_converter.xml` & `galaxy-data-24.0.0/galaxy/datatypes/converters/bedgraph_to_bigwig_converter.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/bigwig_to_wig_converter.xml` & `galaxy-data-24.0.0/galaxy/datatypes/converters/bigwig_to_wig_converter.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/biom.xml` & `galaxy-data-24.0.0/galaxy/datatypes/converters/biom.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/bz2_to_uncompressed.xml` & `galaxy-data-24.0.0/galaxy/datatypes/converters/bz2_to_uncompressed.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/cml_to_smi_converter.xml` & `galaxy-data-24.0.0/galaxy/datatypes/converters/cml_to_smi_converter.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/cram_to_bam_converter.xml` & `galaxy-data-24.0.0/galaxy/datatypes/converters/cram_to_bam_converter.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/csv_to_tabular.xml` & `galaxy-data-24.0.0/galaxy/datatypes/converters/csv_to_tabular.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/fasta_to_2bit.xml` & `galaxy-data-24.0.0/galaxy/datatypes/converters/fasta_to_2bit.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/fasta_to_bowtie_base_index_converter.xml` & `galaxy-data-24.0.0/galaxy/datatypes/converters/fasta_to_bowtie_base_index_converter.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/fasta_to_bowtie_color_index_converter.xml` & `galaxy-data-24.0.0/galaxy/datatypes/converters/fasta_to_bowtie_color_index_converter.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/fasta_to_fai.xml` & `galaxy-data-24.0.0/galaxy/datatypes/converters/fasta_to_fai.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/fasta_to_len.py` & `galaxy-data-24.0.0/galaxy/datatypes/converters/fasta_to_len.py`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/fasta_to_len.xml` & `galaxy-data-24.0.0/galaxy/datatypes/converters/fasta_to_len.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/fasta_to_tabular_converter.py` & `galaxy-data-24.0.0/galaxy/datatypes/converters/fasta_to_tabular_converter.py`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/fasta_to_tabular_converter.xml` & `galaxy-data-24.0.0/galaxy/datatypes/converters/fasta_to_tabular_converter.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/fastq_to_fqtoc.py` & `galaxy-data-24.0.0/galaxy/datatypes/converters/fastq_to_fqtoc.py`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/fastq_to_fqtoc.xml` & `galaxy-data-24.0.0/galaxy/datatypes/converters/fastq_to_fqtoc.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/fastqsolexa_to_fasta_converter.py` & `galaxy-data-24.0.0/galaxy/datatypes/converters/fastqsolexa_to_fasta_converter.py`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/fastqsolexa_to_fasta_converter.xml` & `galaxy-data-24.0.0/galaxy/datatypes/converters/fastqsolexa_to_fasta_converter.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/fastqsolexa_to_qual_converter.py` & `galaxy-data-24.0.0/galaxy/datatypes/converters/fastqsolexa_to_qual_converter.py`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/fastqsolexa_to_qual_converter.xml` & `galaxy-data-24.0.0/galaxy/datatypes/converters/fastqsolexa_to_qual_converter.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/gff_to_bed_converter.py` & `galaxy-data-24.0.0/galaxy/datatypes/converters/gff_to_bed_converter.py`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/gff_to_bed_converter.xml` & `galaxy-data-24.0.0/galaxy/datatypes/converters/gff_to_bed_converter.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/gff_to_fli_converter.xml` & `galaxy-data-24.0.0/galaxy/datatypes/converters/gff_to_fli_converter.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/gff_to_interval_index_converter.py` & `galaxy-data-24.0.0/galaxy/datatypes/converters/gff_to_interval_index_converter.py`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/gff_to_interval_index_converter.xml` & `galaxy-data-24.0.0/galaxy/datatypes/converters/gff_to_interval_index_converter.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/gro_to_pdb.xml` & `galaxy-data-24.0.0/galaxy/datatypes/converters/gro_to_pdb.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/gz_to_uncompressed.xml` & `galaxy-data-24.0.0/galaxy/datatypes/converters/gz_to_uncompressed.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/inchi_to_mol_converter.xml` & `galaxy-data-24.0.0/galaxy/datatypes/converters/inchi_to_mol_converter.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/interval_to_bed12_converter.xml` & `galaxy-data-24.0.0/galaxy/datatypes/converters/interval_to_bed12_converter.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/interval_to_bed6_converter.xml` & `galaxy-data-24.0.0/galaxy/datatypes/converters/interval_to_bed6_converter.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/interval_to_bed_converter.py` & `galaxy-data-24.0.0/galaxy/datatypes/converters/interval_to_bed_converter.py`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/interval_to_bed_converter.xml` & `galaxy-data-24.0.0/galaxy/datatypes/converters/interval_to_bed_converter.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/interval_to_bedstrict_converter.py` & `galaxy-data-24.0.0/galaxy/datatypes/converters/interval_to_bedstrict_converter.py`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/interval_to_bedstrict_converter.xml` & `galaxy-data-24.0.0/galaxy/datatypes/converters/interval_to_bedstrict_converter.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/interval_to_bgzip_converter.xml` & `galaxy-data-24.0.0/galaxy/datatypes/converters/interval_to_bgzip_converter.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/interval_to_bigwig_converter.xml` & `galaxy-data-24.0.0/galaxy/datatypes/converters/interval_to_bigwig_converter.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/interval_to_fli.py` & `galaxy-data-24.0.0/galaxy/datatypes/converters/interval_to_fli.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 where location is formatted as:
 
     contig:start-end
 
 and symbols are sorted in lexigraphical order.
 """
+
 import optparse
 
 from bx.tabular.io import (
     Comment,
     Header,
 )
```

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/interval_to_interval_index_converter.py` & `galaxy-data-24.0.0/galaxy/datatypes/converters/interval_to_interval_index_converter.py`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/interval_to_interval_index_converter.xml` & `galaxy-data-24.0.0/galaxy/datatypes/converters/interval_to_interval_index_converter.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/interval_to_tabix_converter.xml` & `galaxy-data-24.0.0/galaxy/datatypes/converters/interval_to_tabix_converter.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/len_to_linecount.xml` & `galaxy-data-24.0.0/galaxy/datatypes/converters/len_to_linecount.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/lped_to_fped_converter.py` & `galaxy-data-24.0.0/galaxy/datatypes/converters/lped_to_fped_converter.py`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/lped_to_fped_converter.xml` & `galaxy-data-24.0.0/galaxy/datatypes/converters/lped_to_fped_converter.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/lped_to_pbed_converter.py` & `galaxy-data-24.0.0/galaxy/datatypes/converters/lped_to_pbed_converter.py`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/lped_to_pbed_converter.xml` & `galaxy-data-24.0.0/galaxy/datatypes/converters/lped_to_pbed_converter.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/maf_to_fasta_converter.py` & `galaxy-data-24.0.0/galaxy/datatypes/converters/maf_to_fasta_converter.py`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/maf_to_fasta_converter.xml` & `galaxy-data-24.0.0/galaxy/datatypes/converters/maf_to_fasta_converter.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/maf_to_interval_converter.py` & `galaxy-data-24.0.0/galaxy/datatypes/converters/maf_to_interval_converter.py`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/maf_to_interval_converter.xml` & `galaxy-data-24.0.0/galaxy/datatypes/converters/maf_to_interval_converter.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/mdconvert.xml` & `galaxy-data-24.0.0/galaxy/datatypes/converters/mdconvert.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/mol2_to_mol_converter.xml` & `galaxy-data-24.0.0/galaxy/datatypes/converters/mol2_to_mol_converter.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/molecules_converter.xml` & `galaxy-data-24.0.0/galaxy/datatypes/converters/molecules_converter.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/neostorezip_to_neostore_converter.xml` & `galaxy-data-24.0.0/galaxy/datatypes/converters/neostorezip_to_neostore_converter.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/parquet_to_csv_converter.py` & `galaxy-data-24.0.0/galaxy/datatypes/converters/parquet_to_csv_converter.py`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/parquet_to_csv_converter.xml` & `galaxy-data-24.0.0/galaxy/datatypes/converters/parquet_to_csv_converter.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/pbed_ldreduced_converter.py` & `galaxy-data-24.0.0/galaxy/datatypes/converters/pbed_ldreduced_converter.py`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/pbed_ldreduced_converter.xml` & `galaxy-data-24.0.0/galaxy/datatypes/converters/pbed_ldreduced_converter.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/pbed_to_lped_converter.py` & `galaxy-data-24.0.0/galaxy/datatypes/converters/pbed_to_lped_converter.py`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/pbed_to_lped_converter.xml` & `galaxy-data-24.0.0/galaxy/datatypes/converters/pbed_to_lped_converter.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/pdb_to_gro.xml` & `galaxy-data-24.0.0/galaxy/datatypes/converters/pdb_to_gro.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/picard_interval_list_to_bed6_converter.py` & `galaxy-data-24.0.0/galaxy/datatypes/converters/picard_interval_list_to_bed6_converter.py`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/picard_interval_list_to_bed6_converter.xml` & `galaxy-data-24.0.0/galaxy/datatypes/converters/picard_interval_list_to_bed6_converter.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/pileup_to_interval_index_converter.py` & `galaxy-data-24.0.0/galaxy/datatypes/converters/pileup_to_interval_index_converter.py`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/pileup_to_interval_index_converter.xml` & `galaxy-data-24.0.0/galaxy/datatypes/converters/pileup_to_interval_index_converter.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/ref_to_seq_taxonomy_converter.py` & `galaxy-data-24.0.0/galaxy/datatypes/converters/ref_to_seq_taxonomy_converter.py`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/ref_to_seq_taxonomy_converter.xml` & `galaxy-data-24.0.0/galaxy/datatypes/converters/ref_to_seq_taxonomy_converter.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/sam_to_bigwig_converter.xml` & `galaxy-data-24.0.0/galaxy/datatypes/converters/sam_to_bigwig_converter.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/sam_to_unsorted_bam.xml` & `galaxy-data-24.0.0/galaxy/datatypes/converters/sam_to_unsorted_bam.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/smi_to_mol_converter.xml` & `galaxy-data-24.0.0/galaxy/datatypes/converters/smi_to_mol_converter.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/smi_to_smi_converter.xml` & `galaxy-data-24.0.0/galaxy/datatypes/converters/smi_to_smi_converter.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/tabular_csv.py` & `galaxy-data-24.0.0/galaxy/datatypes/converters/tabular_csv.py`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/tabular_to_csv.xml` & `galaxy-data-24.0.0/galaxy/datatypes/converters/tabular_to_csv.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/tabular_to_dbnsfp.xml` & `galaxy-data-24.0.0/galaxy/datatypes/converters/tabular_to_dbnsfp.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/tar_to_directory.xml` & `galaxy-data-24.0.0/galaxy/datatypes/converters/tar_to_directory.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/to_coordinate_sorted_bam.xml` & `galaxy-data-24.0.0/galaxy/datatypes/converters/to_coordinate_sorted_bam.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/to_qname_sorted_bam.xml` & `galaxy-data-24.0.0/galaxy/datatypes/converters/to_qname_sorted_bam.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/uncompressed_to_gz.xml` & `galaxy-data-24.0.0/galaxy/datatypes/converters/uncompressed_to_gz.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/vcf_bgzip_to_tabix_converter.xml` & `galaxy-data-24.0.0/galaxy/datatypes/converters/vcf_bgzip_to_tabix_converter.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/vcf_to_interval_index_converter.py` & `galaxy-data-24.0.0/galaxy/datatypes/converters/vcf_to_interval_index_converter.py`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/vcf_to_interval_index_converter.xml` & `galaxy-data-24.0.0/galaxy/datatypes/converters/vcf_to_interval_index_converter.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/vcf_to_vcf_bgzip_converter.xml` & `galaxy-data-24.0.0/galaxy/datatypes/converters/vcf_to_vcf_bgzip_converter.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/wig_to_bigwig_converter.xml` & `galaxy-data-24.0.0/galaxy/datatypes/converters/wig_to_bigwig_converter.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/wiggle_to_simple_converter.py` & `galaxy-data-24.0.0/galaxy/datatypes/converters/wiggle_to_simple_converter.py`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/converters/wiggle_to_simple_converter.xml` & `galaxy-data-24.0.0/galaxy/datatypes/converters/wiggle_to_simple_converter.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/coverage.py` & `galaxy-data-24.0.0/galaxy/datatypes/coverage.py`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/data.py` & `galaxy-data-24.0.0/galaxy/datatypes/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -421,17 +421,17 @@
                 rpath = os.path.relpath(fpath, extra_files_path)
                 yield fpath, rpath
 
     def _serve_raw(
         self, dataset: DatasetHasHidProtocol, to_ext: Optional[str], headers: Headers, **kwd
     ) -> Tuple[IO, Headers]:
         headers["Content-Length"] = str(os.stat(dataset.get_file_name()).st_size)
-        headers[
-            "content-type"
-        ] = "application/octet-stream"  # force octet-stream so Safari doesn't append mime extensions to filename
+        headers["content-type"] = (
+            "application/octet-stream"  # force octet-stream so Safari doesn't append mime extensions to filename
+        )
         filename = self._download_filename(
             dataset,
             to_ext,
             hdca=kwd.get("hdca"),
             element_identifier=kwd.get("element_identifier"),
             filename_pattern=kwd.get("filename_pattern"),
         )
@@ -472,17 +472,17 @@
             filename = self._download_filename(
                 data,
                 to_ext,
                 hdca=kwd.get("hdca"),
                 element_identifier=kwd.get("element_identifier"),
                 filename_pattern=kwd.get("filename_pattern"),
             )
-            headers[
-                "content-type"
-            ] = "application/octet-stream"  # force octet-stream so Safari doesn't append mime extensions to filename
+            headers["content-type"] = (
+                "application/octet-stream"  # force octet-stream so Safari doesn't append mime extensions to filename
+            )
             headers["Content-Disposition"] = f'attachment; filename="{filename}"'
             return open(data.get_file_name(), "rb"), headers
 
     def _serve_binary_file_contents_as_text(self, trans, data, headers, file_size, max_peek_size):
         headers["content-type"] = "text/html"
         return (
             trans.fill_template_mako(
@@ -1106,15 +1106,15 @@
             else:
                 dataset.blurb = f"{util.commaify(str(line_count))} {inflector.cond_plural(line_count, self.line_class)}"
         else:
             dataset.peek = "file does not exist"
             dataset.blurb = "file purged from disk"
 
     @classmethod
-    def split(cls, input_datasets: List, subdir_generator_function: Callable, split_params: Dict) -> None:
+    def split(cls, input_datasets: List, subdir_generator_function: Callable, split_params: Optional[Dict]) -> None:
         """
         Split the input files by line.
         """
         if split_params is None:
             return
 
         if len(input_datasets) > 1:
```

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/dataproviders/__init__.py` & `galaxy-data-24.0.0/galaxy/datatypes/dataproviders/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/dataproviders/base.py` & `galaxy-data-24.0.0/galaxy/datatypes/dataproviders/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Base class(es) for all DataProviders.
 """
+
 # there's a blurry line between functionality here and functionality in datatypes module
 # attempting to keep parsing to a minimum here and focus on chopping/pagination/reformat(/filtering-maybe?)
 #   and using as much pre-computed info/metadata from the datatypes module as possible
 # also, this shouldn't be a replacement/re-implementation of the tool layer
 #   (which provides traceability/versioning/reproducibility)
 
 import logging
@@ -52,16 +53,15 @@
         settings = {}
         # get settings defined in base classes
         for base_class in base_classes:
             base_settings = getattr(base_class, "settings", None)
             if base_settings:
                 settings.update(base_settings)
         # get settings defined in this class
-        new_settings = attributes.pop("settings", None)
-        if new_settings:
+        if new_settings := attributes.pop("settings", None):
             settings.update(new_settings)
         attributes["settings"] = settings
         return type.__new__(cls, name, base_classes, attributes)
 
 
 # ----------------------------------------------------------------------------- base classes
 class DataProvider(metaclass=HasSettings):
```

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/dataproviders/chunk.py` & `galaxy-data-24.0.0/galaxy/datatypes/dataproviders/chunk.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Chunk (N number of bytes at M offset to a source's beginning) provider.
 
 Primarily for file sources but usable by any iterator that has both
 seek and read( N ).
 """
+
 import base64
 import logging
 import os
 
 from . import (
     base,
     exceptions,
```

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/dataproviders/column.py` & `galaxy-data-24.0.0/galaxy/datatypes/dataproviders/column.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Providers that provide lists of lists generally where each line of a source
 is further subdivided into multiple data (e.g. columns from a line).
 """
+
 import logging
 import re
 from urllib.parse import unquote_plus
 
 from . import line
 
 _TODO = """
```

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/dataproviders/dataset.py` & `galaxy-data-24.0.0/galaxy/datatypes/dataproviders/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Dataproviders that use either:
     - the file contents and/or metadata from a Galaxy DatasetInstance as
         their source.
     - or provide data in some way relevant to bioinformatic data
         (e.g. parsing genomic regions from their source)
 """
+
 import logging
 import sys
 
 from bx import (
     seq as bx_seq,
     wiggle as bx_wig,
 )
```

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/dataproviders/decorators.py` & `galaxy-data-24.0.0/galaxy/datatypes/dataproviders/decorators.py`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/dataproviders/exceptions.py` & `galaxy-data-24.0.0/galaxy/datatypes/dataproviders/exceptions.py`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/dataproviders/external.py` & `galaxy-data-24.0.0/galaxy/datatypes/dataproviders/external.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Data providers that iterate over a source that is not in memory
 or not in a file.
 """
+
 import gzip
 import logging
 import subprocess
 import tempfile
 from urllib.parse import (
     urlencode,
     urlparse,
```

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/dataproviders/hierarchy.py` & `galaxy-data-24.0.0/galaxy/datatypes/dataproviders/hierarchy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 """
 Dataproviders that iterate over lines from their sources.
 """
+
 import logging
 
-from galaxy.util import etree
+from galaxy.util import (
+    Element,
+    etree,
+)
 from . import line
 
 _TODO = """
 """
 
 log = logging.getLogger(__name__)
 
@@ -61,15 +65,14 @@
 
         Change point for more sophisticated selectors.
         """
         # search for partial match of selector to the element tag
         # TODO: add more flexibility here w/o re-implementing xpath
         # TODO: fails with '#' - browser thinks it's an anchor - use urlencode
         # TODO: need removal/replacement of etree namespacing here - then move to string match
-        Element = getattr(etree, "_Element", etree.Element)
         return bool((selector is None) or (isinstance(element, Element) and selector in element.tag))
 
     def element_as_dict(self, element):
         """
         Converts an XML element (its text, tag, and attributes) to dictionary form.
 
         :param  element:    an XML ``Element``
```

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/dataproviders/line.py` & `galaxy-data-24.0.0/galaxy/datatypes/dataproviders/line.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Dataproviders that iterate over lines from their sources.
 """
+
 import collections
 import logging
 import re
 
 from . import base
 
 log = logging.getLogger(__name__)
@@ -180,16 +181,15 @@
     def __iter__(self):
         """
         Overridden to provide last block.
         """
         parent_gen = super().__iter__()
         yield from parent_gen
 
-        last_block = self.handle_last_block()
-        if last_block is not None:
+        if (last_block := self.handle_last_block()) is not None:
             self.num_data_returned += 1
             yield last_block
 
     def filter(self, line):
         """
         Line filter here being used to aggregate/assemble lines into a block
         and determine whether the line indicates a new block.
```

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/display_applications/application.py` & `galaxy-data-24.0.0/galaxy/datatypes/display_applications/application.py`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/ensembl/ensembl_bam.xml` & `galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/ensembl/ensembl_bam.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/ensembl/ensembl_gff.xml` & `galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/ensembl/ensembl_gff.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/ensembl/ensembl_interval_as_bed.xml` & `galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/ensembl/ensembl_interval_as_bed.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/gbrowse/gbrowse_gff.xml` & `galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/gbrowse/gbrowse_gff.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/gbrowse/gbrowse_interval_as_bed.xml` & `galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/gbrowse/gbrowse_interval_as_bed.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/gbrowse/gbrowse_wig.xml` & `galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/gbrowse/gbrowse_wig.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/igb/bam.xml` & `galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/igb/bam.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/igb/bb.xml` & `galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/igb/bb.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/igb/bed.xml` & `galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/igb/bed.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/igb/bedgraph.xml` & `galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/igb/bedgraph.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/igb/bigwig.xml` & `galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/igb/bigwig.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/igb/gtf.xml` & `galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/igb/gtf.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/igb/wig.xml` & `galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/igb/wig.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/igv/bam.xml` & `galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/igv/bam.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/igv/bigwig.xml` & `galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/igv/bigwig.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/igv/genbank.xml` & `galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/igv/genbank.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/igv/genome_fasta.xml` & `galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/igv/genome_fasta.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/igv/gff.xml` & `galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/igv/gff.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/igv/interval_as_bed.xml` & `galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/igv/interval_as_bed.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/igv/vcf.xml` & `galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/igv/vcf.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/rviewer/bed.xml` & `galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/rviewer/bed.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/rviewer/vcf.xml` & `galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/rviewer/vcf.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/ucsc/bam.xml` & `galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/ucsc/bam.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/ucsc/bigbed.xml` & `galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/ucsc/bigbed.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/ucsc/bigwig.xml` & `galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/ucsc/bigwig.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/ucsc/interval_as_bed.xml` & `galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/ucsc/interval_as_bed.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/ucsc/maf_customtrack.xml` & `galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/ucsc/maf_customtrack.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/display_applications/configs/ucsc/vcf.xml` & `galaxy-data-24.0.0/galaxy/datatypes/display_applications/configs/ucsc/vcf.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/display_applications/parameters.py` & `galaxy-data-24.0.0/galaxy/datatypes/display_applications/parameters.py`

 * *Files 0% similar despite different names*

```diff
@@ -156,16 +156,15 @@
                 data.extension, self.extensions
             )
             assert direct_match or target_ext is not None, f"No conversion path found for data param: {self.name}"
             return None
         return data
 
     def get_value(self, other_values, dataset_hash, user_hash, trans):
-        data = self._get_dataset_like_object(other_values)
-        if data:
+        if data := self._get_dataset_like_object(other_values):
             return DisplayDataValueWrapper(data, self, other_values, dataset_hash, user_hash, trans)
         return None
 
     def prepare(self, other_values, dataset_hash, user_hash, trans):
         data = self._get_dataset_like_object(other_values)
         if not data and self.formats:
             data = other_values.get(self.dataset, None)
@@ -206,16 +205,15 @@
     def is_preparing(self, other_values):
         value = self._get_dataset_like_object(other_values)
         if value and value.state in (DatasetState.NEW, DatasetState.UPLOAD, DatasetState.QUEUED, DatasetState.RUNNING):
             return True
         return False
 
     def ready(self, other_values):
-        value = self._get_dataset_like_object(other_values)
-        if value:
+        if value := self._get_dataset_like_object(other_values):
             if value.state == DatasetState.OK:
                 return True
             elif value.state == DatasetState.ERROR:
                 raise Exception(f"A data display parameter is in the error state: {self.name}")
         return False
```

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/display_applications/util.py` & `galaxy-data-24.0.0/galaxy/datatypes/display_applications/util.py`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/display_applications/xsd/geda.xsd` & `galaxy-data-24.0.0/galaxy/datatypes/display_applications/xsd/geda.xsd`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/flow.py` & `galaxy-data-24.0.0/galaxy/datatypes/flow.py`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/genetics.py` & `galaxy-data-24.0.0/galaxy/datatypes/genetics.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 genome graphs datatypes derived from Interval datatypes
 genome graphs datasets have a header row with appropriate columnames
 The first column is always the marker - eg columname = rs, first row= rs12345 if the rows are snps
 subsequent row values are all numeric ! Will fail if any non numeric (eg '+' or 'NA') values
 ross lazarus for rgenetics
 august 20 2007
 """
+
 import logging
 import os
 import re
 import sys
 from typing import (
     Dict,
     IO,
```

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/gis.py` & `galaxy-data-24.0.0/galaxy/datatypes/gis.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 GIS classes
 """
+
 from galaxy.datatypes.binary import Binary
 from galaxy.datatypes.protocols import (
     DatasetProtocol,
     HasExtraFilesAndMetadata,
 )
```

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/goldenpath.py` & `galaxy-data-24.0.0/galaxy/datatypes/goldenpath.py`

 * *Files 0% similar despite different names*

```diff
@@ -361,15 +361,14 @@
 
     @abc.abstractmethod
     def _validate_line(self):
         """Final remaining validations specific to the gap or sequence AGP lines."""
 
 
 class AGPSeqLine(AGPLine):
-
     """
     A subclass of AGPLine specifically for AGP lines that represent sequences.
     """
 
     allowed_comp_types = {"A", "D", "F", "G", "O", "P", "W"}
     allowed_orientations = {"+", "-", "?", "0", "na"}
 
@@ -458,15 +457,14 @@
 
     def _validate_line(self):
         if self.orientation not in AGPSeqLine.allowed_orientations:
             raise AGPError(self.fname, self.line_number, f"invalid orientation: {self.orientation}")
 
 
 class AGPGapLine(AGPLine):
-
     """
     A subclass of AGPLine specifically for AGP lines that represent sequence gaps.
     """
 
     allowed_comp_types = {"N", "U"}
     allowed_linkage_types = {"yes", "no"}
     allowed_gap_types = {
```

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/graph.py` & `galaxy-data-24.0.0/galaxy/datatypes/graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Graph content classes.
 """
+
 import logging
 from typing import List
 
 from galaxy.datatypes.dataproviders.column import ColumnarDataProvider
 from galaxy.datatypes.dataproviders.dataset import DatasetDataProvider
 from galaxy.datatypes.dataproviders.hierarchy import XMLDataProvider
 from galaxy.datatypes.protocols import DatasetProtocol
```

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/hdf5.py` & `galaxy-data-24.0.0/galaxy/datatypes/hdf5.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Composite datatype for the HDF5SummarizedExperiment R data object.
 
 This datatype was created for use with the iSEE interactive tool.
 """
+
 from typing import Optional
 
 from galaxy.datatypes.data import Data
 from galaxy.datatypes.metadata import MetadataElement
 from galaxy.datatypes.protocols import (
     HasExtraFilesAndMetadata,
     HasMetadata,
```

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/images.py` & `galaxy-data-24.0.0/galaxy/datatypes/images.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Image classes
 """
+
 import base64
 import json
 import logging
 from typing import Optional
 
 import mrcfile
 import numpy as np
@@ -86,18 +87,14 @@
     edam_format = "format_3603"
     file_ext = "png"
 
 
 class Tiff(Image):
     edam_format = "format_3591"
     file_ext = "tiff"
-
-
-class OMETiff(Tiff):
-    file_ext = "ome.tiff"
     MetadataElement(
         name="offsets",
         desc="Offsets File",
         param=FileParameter,
         file_ext="json",
         readonly=True,
         visible=False,
@@ -115,14 +112,18 @@
             )
         with tifffile.TiffFile(dataset.get_file_name()) as tif:
             offsets = [page.offset for page in tif.pages]
         with open(offsets_file.get_file_name(), "w") as f:
             json.dump(offsets, f)
         dataset.metadata.offsets = offsets_file
 
+
+class OMETiff(Tiff):
+    file_ext = "ome.tiff"
+
     def sniff(self, filename: str) -> bool:
         with tifffile.TiffFile(filename) as tif:
             if tif.is_ome:
                 return True
         return False
```

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/interval.py` & `galaxy-data-24.0.0/galaxy/datatypes/interval.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Interval datatypes
 """
+
 import logging
 import sys
 import tempfile
 from typing import (
     cast,
     List,
     Optional,
```

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/isa.py` & `galaxy-data-24.0.0/galaxy/datatypes/isa.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,16 +125,15 @@
     ################################################################
 
     def _get_investigation(self, dataset: HasExtraFilesPath) -> Optional["Investigation"]:
         """Create a contained instance specific to the exact ISA type (Tab or Json).
         We will use it to parse and access information from the archive."""
 
         investigation = None
-        main_file = self._get_main_file(dataset)
-        if main_file is not None:
+        if (main_file := self._get_main_file(dataset)) is not None:
             investigation = self._make_investigation_instance(main_file)
 
         return investigation
 
     # Find main file in archive {{{2
     ################################################################
```

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/larch.py` & `galaxy-data-24.0.0/galaxy/datatypes/larch.py`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/media.py` & `galaxy-data-24.0.0/galaxy/datatypes/media.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Video classes"""
+
 import json
 import subprocess
 import wave
 from functools import lru_cache
 from typing import (
     List,
     Tuple,
```

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/metacyto.py` & `galaxy-data-24.0.0/galaxy/datatypes/metacyto.py`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/metadata.py` & `galaxy-data-24.0.0/galaxy/datatypes/metadata.py`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/microarrays.py` & `galaxy-data-24.0.0/galaxy/datatypes/microarrays.py`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/molecules.py` & `galaxy-data-24.0.0/galaxy/datatypes/molecules.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
 import os
 import re
 from typing import (
     Callable,
     Dict,
     List,
+    Optional,
 )
 
 from galaxy.datatypes import metadata
 from galaxy.datatypes.binary import Binary
 from galaxy.datatypes.data import (
     get_file_peek,
     Text,
@@ -387,15 +388,15 @@
     def set_meta(self, dataset: DatasetProtocol, overwrite: bool = True, **kwd) -> None:
         """
         Set the number of molecules in dataset.
         """
         dataset.metadata.number_of_molecules = count_special_lines(r"^\$\$\$\$$", dataset.get_file_name())
 
     @classmethod
-    def split(cls, input_datasets: List, subdir_generator_function: Callable, split_params: Dict) -> None:
+    def split(cls, input_datasets: List, subdir_generator_function: Callable, split_params: Optional[Dict]) -> None:
         """
         Split the input files by molecule records.
         """
         if split_params is None:
             return None
 
         if len(input_datasets) > 1:
@@ -470,15 +471,15 @@
     def set_meta(self, dataset: DatasetProtocol, overwrite: bool = True, **kwd) -> None:
         """
         Set the number of lines of data in dataset.
         """
         dataset.metadata.number_of_molecules = count_special_lines("@<TRIPOS>MOLECULE", dataset.get_file_name())
 
     @classmethod
-    def split(cls, input_datasets: List, subdir_generator_function: Callable, split_params: Dict) -> None:
+    def split(cls, input_datasets: List, subdir_generator_function: Callable, split_params: Optional[Dict]) -> None:
         """
         Split the input files by molecule records.
         """
         if split_params is None:
             return None
 
         if len(input_datasets) > 1:
@@ -556,15 +557,15 @@
     def set_meta(self, dataset: DatasetProtocol, overwrite: bool = True, **kwd) -> None:
         """
         Set the number of lines of data in dataset.
         """
         dataset.metadata.number_of_molecules = count_special_lines("^#", dataset.get_file_name(), invert=True)
 
     @classmethod
-    def split(cls, input_datasets: List, subdir_generator_function: Callable, split_params: Dict) -> None:
+    def split(cls, input_datasets: List, subdir_generator_function: Callable, split_params: Optional[Dict]) -> None:
         """
         Split the input files by fingerprint records.
         """
         if split_params is None:
             return None
 
         if len(input_datasets) > 1:
@@ -680,15 +681,15 @@
 
     @staticmethod
     def merge(split_files: List[str], output_file: str) -> None:
         """Merging Fastsearch indices is not supported."""
         raise NotImplementedError("Merging Fastsearch indices is not supported.")
 
     @classmethod
-    def split(cls, input_datasets: List, subdir_generator_function: Callable, split_params: Dict) -> None:
+    def split(cls, input_datasets: List, subdir_generator_function: Callable, split_params: Optional[Dict]) -> None:
         """Splitting Fastsearch indices is not supported."""
         if split_params is None:
             return None
         raise NotImplementedError("Splitting Fastsearch indices is not possible.")
 
 
 class DRF(GenericMolFile):
@@ -1005,25 +1006,28 @@
         True
         >>> fname = get_test_fname('Si_lowercase.cell')
         >>> CIF().sniff(fname)
         False
         >>> fname = get_test_fname('1.star')
         >>> CIF().sniff(fname)
         False
+        >>> fname = get_test_fname('LaMnO3.cif')
+        >>> CIF().sniff(fname)
+        True
         """
 
         # check for optional CIF version marker '#\#CIF_<version>' at start of file
         if file_prefix.startswith("#\\#CIF_"):
             return True
 
         # no version marker, search for mandatory CIF keywords
         # first non-comment line must begin with 'data_'
         # and '_atom_site_fract_(x|y|z)' must be specified somewhere in the file
         for line in file_prefix.line_iterator():
-            if not line:
+            if not line.rstrip():
                 continue
             elif line[0] == "#":  # comment so skip
                 continue
             elif line.startswith("data_"):
                 return file_prefix.search_str("_atom_site_fract_")
             else:  # line has some other content
                 return False
@@ -1407,15 +1411,15 @@
         for expected_string in ['<?xml version="1.0"?>', "http://www.xml-cml.org/schema"]:
             if expected_string not in file_prefix.contents_header:
                 return False
 
         return True
 
     @classmethod
-    def split(cls, input_datasets: List, subdir_generator_function: Callable, split_params: Dict) -> None:
+    def split(cls, input_datasets: List, subdir_generator_function: Callable, split_params: Optional[Dict]) -> None:
         """
         Split the input files by molecule records.
         """
         if split_params is None:
             return None
 
         if len(input_datasets) > 1:
```

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/mothur.py` & `galaxy-data-24.0.0/galaxy/datatypes/mothur.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Mothur Metagenomics Datatypes
 """
+
 import logging
 import re
 from typing import (
     List,
     Optional,
 )
```

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/msa.py` & `galaxy-data-24.0.0/galaxy/datatypes/msa.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import logging
 import os
 import re
 from typing import (
     Callable,
     Dict,
     List,
+    Optional,
 )
 
 from galaxy.datatypes.binary import Binary
 from galaxy.datatypes.data import (
     get_file_peek,
     Text,
 )
@@ -201,15 +202,15 @@
         Set the number of models in dataset.
         """
         dataset.metadata.number_of_models = generic_util.count_special_lines(
             "^#[[:space:]+]STOCKHOLM[[:space:]+]1.0", dataset.get_file_name()
         )
 
     @classmethod
-    def split(cls, input_datasets: List, subdir_generator_function: Callable, split_params: Dict) -> None:
+    def split(cls, input_datasets: List, subdir_generator_function: Callable, split_params: Optional[Dict]) -> None:
         """
 
         Split the input files by model records.
         """
         if split_params is None:
             return None
```

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/neo4j.py` & `galaxy-data-24.0.0/galaxy/datatypes/neo4j.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Neo4j Composite Dataset
 """
+
 import logging
 
 from galaxy.datatypes.data import Data
 from galaxy.datatypes.images import Html
 from galaxy.datatypes.metadata import MetadataElement
 from galaxy.datatypes.protocols import (
     DatasetProtocol,
```

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/ngsindex.py` & `galaxy-data-24.0.0/galaxy/datatypes/ngsindex.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 NGS indexes
 """
+
 import logging
 import os
 
 from galaxy.datatypes.protocols import (
     DatasetProtocol,
     HasExtraFilesAndMetadata,
 )
```

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/phylip.py` & `galaxy-data-24.0.0/galaxy/datatypes/phylip.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 @authors: Kenzo-Hugo Hillion and Fabien Mareuil, Institut Pasteur, Paris
 @contacts: kehillio@pasteur.fr and fabien.mareuil@pasteur.fr
 @project: galaxy
 @githuborganization: C3BI
 Phylip datatype sniffer
 """
+
 from typing import TYPE_CHECKING
 
 from galaxy import util
 from galaxy.datatypes.data import (
     get_file_peek,
     Text,
 )
```

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/plant_tribes.py` & `galaxy-data-24.0.0/galaxy/datatypes/plant_tribes.py`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/proteomics.py` & `galaxy-data-24.0.0/galaxy/datatypes/proteomics.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Proteomics Datatypes
 """
+
 import logging
 import re
 from typing import (
     IO,
     List,
     Optional,
 )
```

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/protocols.py` & `galaxy-data-24.0.0/galaxy/datatypes/protocols.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,37 @@
 """
 Location of protocols used in datatypes
 """
+
 from typing import Any
 
 from typing_extensions import Protocol
 
 
 class HasClearAssociatedFiles(Protocol):
-    def clear_associated_files(self, metadata_safe: bool = False, purge: bool = False) -> None:
-        ...
+    def clear_associated_files(self, metadata_safe: bool = False, purge: bool = False) -> None: ...
 
 
 class HasCreatingJob(Protocol):
     @property
-    def creating_job(self):
-        ...
+    def creating_job(self): ...
 
 
 class HasExt(Protocol):
     @property
-    def ext(self):
-        ...
+    def ext(self): ...
 
 
 class HasExtraFilesPath(Protocol):
     @property
-    def extra_files_path(self):
-        ...
+    def extra_files_path(self): ...
 
 
 class HasFileName(Protocol):
-    def get_file_name(self, sync_cache=True) -> str:
-        ...
+    def get_file_name(self, sync_cache=True) -> str: ...
 
 
 class HasHid(Protocol):
     hid: str
 
 
 class HasId(Protocol):
@@ -50,16 +46,15 @@
     metadata: Any
 
 
 class HasName(Protocol):
     name: str
 
 
-class HasExtraFilesAndMetadata(HasExtraFilesPath, HasMetadata, Protocol):
-    ...
+class HasExtraFilesAndMetadata(HasExtraFilesPath, HasMetadata, Protocol): ...
 
 
 class DatasetProtocol(
     HasCreatingJob,
     HasExt,
     HasExtraFilesPath,
     HasFileName,
@@ -74,28 +69,21 @@
     dbkey: Any
     extension: str
     peek: Any
     state: Any
     states: Any
 
     @property
-    def datatype(self):
-        ...
+    def datatype(self): ...
 
-    def get_converted_files_by_type(self, file_type):
-        ...
+    def get_converted_files_by_type(self, file_type): ...
 
-    def get_mime(self) -> str:
-        ...
+    def get_mime(self) -> str: ...
 
-    def get_size(self) -> int:
-        ...
+    def get_size(self) -> int: ...
 
-    def has_data(self) -> bool:
-        ...
+    def has_data(self) -> bool: ...
 
-    def set_peek(self) -> None:
-        ...
+    def set_peek(self) -> None: ...
 
 
-class DatasetHasHidProtocol(DatasetProtocol, HasHid, Protocol):
-    ...
+class DatasetHasHidProtocol(DatasetProtocol, HasHid, Protocol): ...
```

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/qiime2.py` & `galaxy-data-24.0.0/galaxy/datatypes/qiime2.py`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/qualityscore.py` & `galaxy-data-24.0.0/galaxy/datatypes/qualityscore.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Qualityscore class
 """
+
 import logging
 
 from galaxy.datatypes.protocols import DatasetProtocol
 from galaxy.datatypes.sniff import (
     build_sniff_from_prefix,
     FilePrefix,
 )
```

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/registry.py` & `galaxy-data-24.0.0/galaxy/datatypes/registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -352,17 +352,17 @@
                             if edam_format:
                                 compressed_datatype_class.edam_format = edam_format
                             if edam_data:
                                 compressed_datatype_class.edam_data = edam_data
                             compressed_datatype_instance = compressed_datatype_class()
                             self.datatypes_by_extension[compressed_extension] = compressed_datatype_instance
                             for suffix in infer_from_suffixes:
-                                self.datatypes_by_suffix_inferences[
-                                    f"{suffix}.{auto_compressed_type}"
-                                ] = compressed_datatype_instance
+                                self.datatypes_by_suffix_inferences[f"{suffix}.{auto_compressed_type}"] = (
+                                    compressed_datatype_instance
+                                )
                             if display_in_upload and compressed_extension not in self.upload_file_formats:
                                 self.upload_file_formats.append(compressed_extension)
                             self.datatype_info_dicts.append(
                                 {
                                     "display_in_upload": display_in_upload,
                                     "extension": compressed_extension,
                                     "description": description,
@@ -484,16 +484,15 @@
 
     def load_datatype_sniffers(self, root, override=False, compressed_sniffers=None):
         """
         Process the sniffers element from a parsed a datatypes XML file located at root_dir/config (if processing the Galaxy
         distributed config) or contained within an installed Tool Shed repository.
         """
         sniffer_elem_classes = [e.attrib["type"] for e in self.sniffer_elems]
-        sniffers = root.find("sniffers")
-        if sniffers is not None:
+        if (sniffers := root.find("sniffers")) is not None:
             for elem in sniffers.findall("sniffer"):
                 # Keep a status of the process steps to enable stopping the process of handling the sniffer if necessary.
                 ok = True
                 dtype = elem.get("type", None)
                 if dtype is not None:
                     try:
                         fields = dtype.split(":")
```

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/sequence.py` & `galaxy-data-24.0.0/galaxy/datatypes/sequence.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,15 +213,15 @@
                     split_data["args"]["toc_file"] = toc.get_file_name()
                 with open(os.path.join(dir, f"split_info_{base_name}.json"), "w") as f:
                     json.dump(split_data, f)
             start_sequence += sequences_per_file[part_no]
         return directories
 
     @classmethod
-    def split(cls, input_datasets: List, subdir_generator_function: Callable, split_params: Dict) -> None:
+    def split(cls, input_datasets: List, subdir_generator_function: Callable, split_params: Optional[Dict]) -> None:
         """Split a generic sequence file (not sensible or possible, see subclasses)."""
         if split_params is None:
             return None
         raise NotImplementedError("Can't split generic sequence files")
 
     @staticmethod
     def get_split_commands_with_toc(
@@ -254,16 +254,16 @@
             current_sequence += int(sections[i]["sequences"])
             i += 1
         if i == len(sections):  # bad input data!
             raise Exception(f"No FQTOC section contains starting sequence {start_sequence}")
 
         # These two variables act as an accumulator for consecutive entire blocks that
         # can be copied verbatim (without decompressing)
-        start_chunk = int(-1)
-        end_chunk = int(-1)
+        start_chunk = -1
+        end_chunk = -1
         copy_chunk_cmd = "dd bs=1 skip=%s count=%s if=%s 2> /dev/null >> %s"
 
         while sequence_count > 0 and i < len(sections):
             # we need to extract partial data. So, find the byte offsets of the chunks that contain the data we need
             # use a combination of dd (to pull just the right sections out) tail (to skip lines) and head (to get the
             # right number of lines
             sequences = int(sections[i]["sequences"])
@@ -331,28 +331,46 @@
     edam_data = "data_0863"
 
     MetadataElement(
         name="species", desc="Species", default=[], param=metadata.SelectParameter, multiple=True, readonly=True
     )
 
     @classmethod
-    def split(cls, input_datasets: List, subdir_generator_function: Callable, split_params: Dict) -> None:
+    def split(cls, input_datasets: List, subdir_generator_function: Callable, split_params: Optional[Dict]) -> None:
         """Split a generic alignment file (not sensible or possible, see subclasses)."""
         if split_params is None:
             return None
         raise NotImplementedError("Can't split generic alignment files")
 
 
 @build_sniff_from_prefix
 class Fasta(Sequence):
     """Class representing a FASTA sequence"""
 
     edam_format = "format_1929"
     file_ext = "fasta"
 
+    def set_meta(self, dataset: DatasetProtocol, overwrite: bool = True, **kwd) -> None:
+        """
+        Set the number of sequences and the number of data lines in a FASTA dataset.
+        """
+        data_lines = 0
+        sequences = 0
+        with compression_utils.get_fileobj(dataset.get_file_name()) as fh:
+            for line in fh:
+                if not line:
+                    continue
+                elif line[0] == ">":
+                    sequences += 1
+                    data_lines += 1
+                else:
+                    data_lines += 1
+            dataset.metadata.data_lines = data_lines
+            dataset.metadata.sequences = sequences
+
     def sniff_prefix(self, file_prefix: FilePrefix) -> bool:
         """
         Determines whether the file is in fasta format
 
         A sequence in FASTA format consists of a single-line description, followed by lines of sequence data.
         The first character of the description line is a greater-than (">") symbol in the first column.
         All lines should be shorter than 80 characters
@@ -401,15 +419,15 @@
                         return False
                     return True
                 else:
                     return False
         return False
 
     @classmethod
-    def split(cls, input_datasets: List, subdir_generator_function: Callable, split_params: Dict) -> None:
+    def split(cls, input_datasets: List, subdir_generator_function: Callable, split_params: Optional[Dict]) -> None:
         """Split a FASTA file sequence by sequence.
 
         Note that even if split_mode="number_of_parts", the actual number of
         sub-files produced may not match that requested by split_size.
 
         If split_mode="to_size" then split_size is treated as the number of
         FASTA records to put in each sub-file (not size in bytes).
@@ -695,32 +713,19 @@
         """
         if self.max_optional_metadata_filesize >= 0 and dataset.get_size() > self.max_optional_metadata_filesize:
             dataset.metadata.data_lines = None
             dataset.metadata.sequences = None
             return
         data_lines = 0
         sequences = 0
-        seq_counter = 0  # blocks should be 4 lines long
         with compression_utils.get_fileobj(dataset.get_file_name()) as in_file:
             for line in in_file:
-                line = line.strip()
-                if line and line.startswith("#") and not data_lines:
-                    # We don't count comment lines for sequence data types
-                    continue
-                seq_counter += 1
+                if line.startswith("@") and data_lines % 4 == 0:
+                    sequences += 1
                 data_lines += 1
-                if line and line.startswith("@"):
-                    if seq_counter >= 4:
-                        # count previous block
-                        # blocks should be 4 lines long
-                        sequences += 1
-                        seq_counter = 1
-            if seq_counter >= 4:
-                # count final block
-                sequences += 1
             dataset.metadata.data_lines = data_lines
             dataset.metadata.sequences = sequences
 
     def sniff_prefix(self, file_prefix: FilePrefix) -> bool:
         """
         Determines whether the file is in generic fastq format
         For details, see http://maq.sourceforge.net/fastq.shtml
@@ -788,15 +793,15 @@
                     ),
                     headers,
                 )
         else:
             return Sequence.display_data(self, trans, dataset, preview, filename, to_ext, **kwd)
 
     @classmethod
-    def split(cls, input_datasets: List, subdir_generator_function: Callable, split_params: Dict) -> None:
+    def split(cls, input_datasets: List, subdir_generator_function: Callable, split_params: Optional[Dict]) -> None:
         """
         FASTQ files are split on cluster boundaries, in increments of 4 lines
         """
         if split_params is None:
             return None
 
         # first, see if there are any associated FQTOC files that will give us the split locations
```

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/set_metadata_tool.xml` & `galaxy-data-24.0.0/galaxy/datatypes/set_metadata_tool.xml`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/sniff.py` & `galaxy-data-24.0.0/galaxy/datatypes/sniff.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,16 +87,15 @@
     converted_newlines: bool
     converted_regex: bool
 
 
 class ConvertFunction(Protocol):
     def __call__(
         self, fname: str, in_place: bool = True, tmp_dir: Optional[str] = None, tmp_prefix: Optional[str] = "gxupload"
-    ) -> ConvertResult:
-        ...
+    ) -> ConvertResult: ...
 
 
 def convert_newlines(
     fname: str,
     in_place: bool = True,
     tmp_dir: Optional[str] = None,
     tmp_prefix: Optional[str] = "gxupload",
@@ -395,14 +394,17 @@
     'cell'
     >>> fname = get_test_fname('Si_lowercase.cell')
     >>> guess_ext(fname, sniff_order)
     'cell'
     >>> fname = get_test_fname('Si.cif')
     >>> guess_ext(fname, sniff_order)
     'cif'
+    >>> fname = get_test_fname('LaMnO3.cif')
+    >>> guess_ext(fname, sniff_order)
+    'cif'
     >>> fname = get_test_fname('Si.xyz')
     >>> guess_ext(fname, sniff_order)
     'xyz'
     >>> fname = get_test_fname('Si_multi.xyz')
     >>> guess_ext(fname, sniff_order)
     'xyz'
     >>> fname = get_test_fname('Si.extxyz')
```

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/spaln.py` & `galaxy-data-24.0.0/galaxy/datatypes/spaln.py`

 * *Files 0% similar despite different names*

```diff
@@ -168,15 +168,15 @@
 
     @staticmethod
     def merge(split_files: List[str], output_file: str) -> None:
         """Merge spaln databases (not implemented)."""
         raise NotImplementedError("Merging spaln databases is not possible")
 
     @classmethod
-    def split(cls, input_datasets: List, subdir_generator_function: Callable, split_params: Dict) -> None:
+    def split(cls, input_datasets: List, subdir_generator_function: Callable, split_params: Optional[Dict]) -> None:
         """Split a spaln database (not implemented)."""
         if split_params is None:
             return None
         raise NotImplementedError("Can't split spaln database")
 
     def set_meta(self, dataset: DatasetProtocol, overwrite: bool = True, **kwd) -> None:
         super().set_meta(dataset, overwrite=overwrite, **kwd)
```

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/speech.py` & `galaxy-data-24.0.0/galaxy/datatypes/speech.py`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/tabular.py` & `galaxy-data-24.0.0/galaxy/datatypes/tabular.py`

 * *Files 1% similar despite different names*

```diff
@@ -446,26 +446,26 @@
         if skip is None:
             skip = 0
         column_type_set_order = ["int", "float", "list", "str"]  # Order to set column types in
         default_column_type = column_type_set_order[-1]  # Default column type is lowest in list
         column_type_compare_order = list(column_type_set_order)  # Order to compare column types
         column_type_compare_order.reverse()
 
-        def type_overrules_type(column_type1, column_type2):
-            if column_type1 is None or column_type1 == column_type2:
+        def type_overrules_type(new_column_type, old_column_type):
+            if new_column_type is None or new_column_type == old_column_type:
                 return False
-            if column_type2 is None:
+            if old_column_type is None:
                 return True
             for column_type in column_type_compare_order:
-                if column_type1 == column_type:
+                if new_column_type == column_type:
                     return True
-                if column_type2 == column_type:
+                if old_column_type == column_type:
                     return False
             # neither column type was found in our ordered list, this cannot happen
-            raise ValueError(f"Tried to compare unknown column types: {column_type1} and {column_type2}")
+            raise ValueError(f"Tried to compare unknown column types: {new_column_type} and {old_column_type}")
 
         def is_int(column_text):
             # Don't allow underscores in numeric literals (PEP 515)
             if "_" in column_text:
                 return False
             try:
                 int(column_text)
@@ -504,15 +504,15 @@
                     return column_type
             return None
 
         data_lines = 0
         comment_lines = 0
         column_names = None
         column_types: List = []
-        first_line_column_types = [default_column_type]  # default value is one column of type str
+        first_line_column_types = []
         if dataset.has_data():
             # NOTE: if skip > num_check_lines, we won't detect any metadata, and will use default
             with compression_utils.get_fileobj(dataset.get_file_name()) as dataset_fh:
                 i = 0
                 for line in iter(dataset_fh.readline, ""):
                     line = line.rstrip("\r\n")
                     if i == 0:
```

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/text.py` & `galaxy-data-24.0.0/galaxy/datatypes/text.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 """
 
 import gzip
 import json
 import logging
 import os
 import re
+import shlex
 import subprocess
 import tempfile
 from typing import (
     IO,
     Optional,
     Tuple,
 )
@@ -34,15 +35,14 @@
 from galaxy.datatypes.sniff import (
     build_sniff_from_prefix,
     FilePrefix,
     iter_headers,
 )
 from galaxy.util import (
     nice_size,
-    shlex_join,
     string_as_bool,
     unicodify,
 )
 
 log = logging.getLogger(__name__)
 
 
@@ -129,14 +129,27 @@
     def display_peek(self, dataset: DatasetProtocol) -> str:
         try:
             return dataset.peek
         except Exception:
             return f"JSON file ({nice_size(dataset.get_size())})"
 
 
+class DataManagerJson(Json):
+    file_ext = "data_manager_json"
+    MetadataElement(
+        name="data_tables", default=None, desc="Data tables represented by this dataset", readonly=True, visible=True
+    )
+
+    def set_meta(self, dataset: DatasetProtocol, overwrite: bool = True, **kwd):
+        super().set_meta(dataset=dataset, overwrite=overwrite, **kwd)
+        with open(dataset.get_file_name()) as fh:
+            data_tables = json.load(fh)["data_tables"]
+        dataset.metadata.data_tables = data_tables
+
+
 class ExpressionJson(Json):
     """Represents the non-data input or output to a tool or workflow."""
 
     file_ext = "json"
     MetadataElement(
         name="json_type", default=None, desc="JavaScript or JSON type of expression", readonly=True, visible=True
     )
@@ -238,15 +251,15 @@
                 ]
                 subprocess.check_call(cmd)
                 ofilename = f"{ofilename}.html"
             except subprocess.CalledProcessError:
                 ofilename = dataset.get_file_name()
                 log.exception(
                     'Command "%s" failed. Could not convert the Jupyter Notebook to HTML, defaulting to plain text.',
-                    shlex_join(cmd),
+                    shlex.join(cmd),
                 )
             return open(ofilename, mode="rb"), headers
 
     def set_meta(self, dataset: DatasetProtocol, overwrite: bool = True, **kwd) -> None:
         """
         Set the number of models in dataset.
         """
@@ -1109,15 +1122,14 @@
             file_start = file_prefix.string_io().read(50000).strip().rsplit("\n", 1)[0]
             try:
                 item = yaml.safe_load(file_start)
                 assert isinstance(item, (list, dict))
                 return True
             except yaml.YAMLError:
                 return False
-            return False
 
 
 @build_sniff_from_prefix
 class BCSLmodel(Text):
     """BioChemical Space Language model file"""
 
     file_ext = "bcsl.model"
```

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/tracks.py` & `galaxy-data-24.0.0/galaxy/datatypes/tracks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Datatype classes for tracks/track views within galaxy.
 """
+
 import logging
 
 from galaxy.datatypes.protocols import (
     DatasetProtocol,
     HasExtraFilesAndMetadata,
 )
 from galaxy.datatypes.text import Html
```

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/triples.py` & `galaxy-data-24.0.0/galaxy/datatypes/triples.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """
 Triple format classes
 """
+
 import logging
 import re
 
+from galaxy.datatypes.metadata import MetadataElement
 from galaxy.datatypes.protocols import DatasetProtocol
 from galaxy.datatypes.sniff import (
     build_sniff_from_prefix,
     FilePrefix,
 )
 from . import (
     binary,
@@ -16,14 +18,15 @@
     xml,
 )
 
 log = logging.getLogger(__name__)
 
 TURTLE_PREFIX_PATTERN = re.compile(r"@prefix\s+[^:]*:\s+<[^>]*>\s\.")
 TURTLE_BASE_PATTERN = re.compile(r"@base\s+<[^>]*>\s\.")
+SBOL_PATTERN = re.compile(r"http[s]?://[w\.]*sbol[s]?.org/v(\d{1})#")
 
 
 class Triples(data.Data):
     """
     The abstract base class for the file format that can contain triples
     """
 
@@ -197,7 +200,42 @@
         """Set the peek and blurb text"""
         if not dataset.dataset.purged:
             dataset.peek = data.get_file_peek(dataset.get_file_name())
             dataset.blurb = "HDT triple data"
         else:
             dataset.peek = "file does not exist"
             dataset.blurb = "file purged from disk"
+
+
+@build_sniff_from_prefix
+class Sbol(data.Text, Triples):
+    """
+    The SBOL data format (https://sbolstandard.org).
+    """
+
+    MetadataElement(name="version", default="", readonly=True, visible=True, optional=True)
+    edam_format = "format_3725"
+    file_ext = "sbol"
+
+    def set_meta(self, dataset: DatasetProtocol, overwrite: bool = True, **kwd) -> None:
+        file_prefix = FilePrefix(filename=dataset.get_file_name())
+        match = file_prefix.search(SBOL_PATTERN)
+        if match and match.group(1):
+            dataset.metadata.version = match.group(1)
+
+    def sniff_prefix(self, file_prefix: FilePrefix) -> bool:
+        # http://sbols.org/v2#
+        if file_prefix.search(SBOL_PATTERN):
+            return True
+        return False
+
+    def set_peek(self, dataset: DatasetProtocol, **kwd) -> None:
+        """Set the peek and blurb text"""
+        if not dataset.dataset.purged:
+            dataset.peek = data.get_file_peek(dataset.get_file_name())
+            msg = "SBOL data"
+            if dataset.metadata.version != "":
+                msg += " v" + dataset.metadata.version
+            dataset.blurb = msg
+        else:
+            dataset.peek = "file does not exist"
+            dataset.blurb = "file purged from disk"
```

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/upload_util.py` & `galaxy-data-24.0.0/galaxy/datatypes/upload_util.py`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/util/gff_util.py` & `galaxy-data-24.0.0/galaxy/datatypes/util/gff_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Provides utilities for working with GFF files.
 """
+
 import copy
 
 from bx.intervals.io import (
     GenomicInterval,
     GenomicIntervalReader,
     MissingFieldError,
     NiceReaderWrapper,
```

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/util/maf_utilities.py` & `galaxy-data-24.0.0/galaxy/datatypes/util/maf_utilities.py`

 * *Files 0% similar despite different names*

```diff
@@ -654,17 +654,14 @@
     ends = []
 
     fields = line.split()
     # Requires atleast 12 BED columns
     if len(fields) < 12:
         raise Exception(f"Not a proper 12 column BED line ({line}).")
     tx_start = int(fields[1])
-    strand = fields[5]
-    if strand != "-":
-        strand = "+"  # Default strand is +
     cds_start = int(fields[6])
     cds_end = int(fields[7])
 
     # Calculate and store starts and ends of coding exons
     region_start, region_end = cds_start, cds_end
     exon_starts = list(map(int, fields[11].rstrip(",\n").split(",")))
     exon_starts = [x + tx_start for x in exon_starts]
```

### Comparing `galaxy-data-23.2.1/galaxy/datatypes/xml.py` & `galaxy-data-24.0.0/galaxy/datatypes/xml.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 XML format classes
 """
+
 import logging
 import re
 from typing import List
 
 from galaxy import util
 from galaxy.datatypes.dataproviders.dataset import DatasetDataProvider
 from galaxy.datatypes.dataproviders.hierarchy import XMLDataProvider
```

### Comparing `galaxy-data-23.2.1/galaxy/model/__init__.py` & `galaxy-data-24.0.0/galaxy/model/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Galaxy data model classes
 
 Naming: try to use class names that have a distinct plural form so that
 the relationship cardinalities are obvious (e.g. prefer Dataset to Data)
 """
+
 import abc
 import base64
 import errno
 import json
 import logging
 import numbers
 import operator
@@ -107,23 +108,27 @@
 )
 from sqlalchemy.orm.attributes import flag_modified
 from sqlalchemy.orm.collections import attribute_mapped_collection
 from sqlalchemy.sql import exists
 from typing_extensions import (
     Literal,
     Protocol,
+    TypeAlias,
     TypedDict,
 )
 
 import galaxy.exceptions
 import galaxy.model.metadata
 import galaxy.model.tags
 import galaxy.security.passwords
 import galaxy.util
-from galaxy.model.base import transaction
+from galaxy.model.base import (
+    ensure_object_added_to_session,
+    transaction,
+)
 from galaxy.model.custom_types import (
     DoubleEncodedJsonType,
     JSONType,
     MetadataType,
     MutableJSONType,
     TrimmedString,
     UUIDType,
@@ -132,19 +137,24 @@
 from galaxy.model.item_attrs import (
     get_item_annotation_str,
     UsesAnnotations,
 )
 from galaxy.model.orm.now import now
 from galaxy.model.orm.util import add_object_to_object_session
 from galaxy.objectstore import ObjectStore
-from galaxy.schema.invocation import InvocationCancellationUserRequest
+from galaxy.schema.invocation import (
+    InvocationCancellationUserRequest,
+    InvocationState,
+    InvocationStepState,
+)
 from galaxy.schema.schema import (
     DatasetCollectionPopulatedState,
     DatasetState,
     DatasetValidatedState,
+    InvocationsStateCounts,
     JobState,
 )
 from galaxy.schema.workflow.comments import WorkflowCommentModel
 from galaxy.security import get_permitted_actions
 from galaxy.security.idencoding import IdEncodingHelper
 from galaxy.security.validate_user_input import validate_password_str
 from galaxy.util import (
@@ -518,16 +528,15 @@
             self.job_stderr = None
 
         if job_messages is not None:
             self.job_messages = job_messages
 
     def log_str(self):
         extra = ""
-        safe_id = getattr(self, "id", None)
-        if safe_id is not None:
+        if (safe_id := getattr(self, "id", None)) is not None:
             extra += f"id={safe_id}"
         else:
             extra += "unflushed"
 
         return f"{self.__class__.__name__}[{extra},tool_id={self.tool_id}]"
 
     @property
@@ -647,22 +656,22 @@
     statements.append((clean_old_statement, params))
     return statements
 
 
 # move these to galaxy.schema.schema once galaxy-data depends on
 # galaxy-schema.
 class UserQuotaBasicUsage(BaseModel):
-    quota_source_label: Optional[str]
+    quota_source_label: Optional[str] = None
     total_disk_usage: float
 
 
 class UserQuotaUsage(UserQuotaBasicUsage):
-    quota_percent: Optional[float]
-    quota_bytes: Optional[int]
-    quota: Optional[str]
+    quota_percent: Optional[float] = None
+    quota_bytes: Optional[int] = None
+    quota: Optional[str] = None
 
 
 class User(Base, Dictifiable, RepresentById):
     """
     Data for a Galaxy user or admin and relations to their
     histories, credentials, and roles.
     """
@@ -686,30 +695,32 @@
     deleted = Column(Boolean, index=True, default=False)
     purged = Column(Boolean, index=True, default=False)
     disk_usage = Column(Numeric(15, 0), index=True)
     # Column("person_metadata", JSONType),  # TODO: add persistent, configurable metadata rep for workflow creator
     active = Column(Boolean, index=True, default=True, nullable=False)
     activation_token = Column(TrimmedString(64), nullable=True, index=True)
 
-    addresses = relationship("UserAddress", back_populates="user", order_by=lambda: desc(UserAddress.update_time))
+    addresses = relationship(
+        "UserAddress", back_populates="user", order_by=lambda: desc(UserAddress.update_time), cascade_backrefs=False
+    )
     cloudauthz = relationship("CloudAuthz", back_populates="user")
     custos_auth = relationship("CustosAuthnzToken", back_populates="user")
     default_permissions = relationship("DefaultUserPermissions", back_populates="user")
     groups = relationship("UserGroupAssociation", back_populates="user")
     histories = relationship(
-        "History", back_populates="user", order_by=lambda: desc(History.update_time)  # type: ignore[has-type]
+        "History", back_populates="user", order_by=lambda: desc(History.update_time), cascade_backrefs=False  # type: ignore[has-type]
     )
     active_histories = relationship(
         "History",
         primaryjoin=(lambda: (History.user_id == User.id) & (not_(History.deleted)) & (not_(History.archived))),  # type: ignore[has-type]
         viewonly=True,
         order_by=lambda: desc(History.update_time),  # type: ignore[has-type]
     )
     galaxy_sessions = relationship(
-        "GalaxySession", back_populates="user", order_by=lambda: desc(GalaxySession.update_time)  # type: ignore[has-type]
+        "GalaxySession", back_populates="user", order_by=lambda: desc(GalaxySession.update_time), cascade_backrefs=False  # type: ignore[has-type]
     )
     quotas = relationship("UserQuotaAssociation", back_populates="user")
     quota_source_usages = relationship("UserQuotaSourceUsage", back_populates="user")
     social_auth = relationship("UserAuthnzToken", back_populates="user")
     stored_workflow_menu_entries = relationship(
         "StoredWorkflowMenuEntry",
         primaryjoin=(
@@ -736,17 +747,20 @@
                 not_(APIKeys.deleted == true()),  # type: ignore[has-type]
             )
         ),
     )
     data_manager_histories = relationship("DataManagerHistoryAssociation", back_populates="user")
     roles = relationship("UserRoleAssociation", back_populates="user")
     stored_workflows = relationship(
-        "StoredWorkflow", back_populates="user", primaryjoin=(lambda: User.id == StoredWorkflow.user_id)  # type: ignore[has-type]
+        "StoredWorkflow",
+        back_populates="user",
+        primaryjoin=(lambda: User.id == StoredWorkflow.user_id),  # type: ignore[has-type]
+        cascade_backrefs=False,
     )
-    all_notifications = relationship("UserNotificationAssociation", back_populates="user")
+    all_notifications = relationship("UserNotificationAssociation", back_populates="user", cascade_backrefs=False)
     non_private_roles = relationship(
         "UserRoleAssociation",
         viewonly=True,
         primaryjoin=(
             lambda: (User.id == UserRoleAssociation.user_id)  # type: ignore[has-type]
             & (UserRoleAssociation.role_id == Role.id)  # type: ignore[has-type]
             & not_(Role.name == User.email)  # type: ignore[has-type]
@@ -775,31 +789,50 @@
         self.password = password
         self.external = False
         self.deleted = False
         self.purged = False
         self.active = False
         self.username = username
 
+    def get_user_data_tables(self, data_table: str):
+        session = object_session(self)
+        assert session
+        metadata_select = (
+            select(HistoryDatasetAssociation)
+            .join(Dataset)
+            .join(History)
+            .where(
+                HistoryDatasetAssociation.deleted == false(),
+                HistoryDatasetAssociation.extension == "data_manager_json",
+                History.user_id == self.id,
+                Dataset.state == "ok",
+                # excludes data manager runs that actually populated tables.
+                # maybe track this formally by creating a different datatype for bundles ?
+                Dataset.total_size != Dataset.file_size,
+                HistoryDatasetAssociation._metadata.contains(data_table),
+            )
+            .order_by(HistoryDatasetAssociation.id)
+        )
+        return session.execute(metadata_select).scalars().all()
+
     @property
     def extra_preferences(self):
         data = defaultdict(lambda: None)
-        extra_user_preferences = self.preferences.get("extra_user_preferences")
-        if extra_user_preferences:
+        if extra_user_preferences := self.preferences.get("extra_user_preferences"):
             try:
                 data.update(json.loads(extra_user_preferences))
             except Exception:
                 pass
         return data
 
     def set_password_cleartext(self, cleartext):
         """
         Set user password to the digest of `cleartext`.
         """
-        message = validate_password_str(cleartext)
-        if message:
+        if message := validate_password_str(cleartext):
             raise Exception(f"Invalid password: {message}")
         if User.use_pbkdf2:
             self.password = galaxy.security.passwords.hash_password(cleartext)
         else:
             self.password = new_insecure_hash(text_type=cleartext)
         self.last_password_change = now()
 
@@ -912,15 +945,15 @@
 
     total_disk_usage = property(get_disk_usage, set_disk_usage)
 
     def adjust_total_disk_usage(self, amount, quota_source_label):
         assert amount is not None
         if amount != 0:
             if quota_source_label is None:
-                self.disk_usage = func.coalesce(self.table.c.disk_usage, 0) + amount
+                self.disk_usage = (self.disk_usage or 0) + amount
             else:
                 # else would work on newer sqlite - 3.24.0
                 engine = object_session(self).bind
                 if "sqlite" in engine.dialect.name:
                     # hacky alternative for older sqlite
                     statement = """
 WITH new (user_id, quota_source_label) AS ( VALUES(:user_id, :label) )
@@ -1327,31 +1360,35 @@
     input_datasets = relationship("JobToInputDatasetAssociation", back_populates="job")
     input_dataset_collections = relationship("JobToInputDatasetCollectionAssociation", back_populates="job")
     input_dataset_collection_elements = relationship(
         "JobToInputDatasetCollectionElementAssociation", back_populates="job"
     )
     output_dataset_collection_instances = relationship("JobToOutputDatasetCollectionAssociation", back_populates="job")
     output_dataset_collections = relationship("JobToImplicitOutputDatasetCollectionAssociation", back_populates="job")
-    post_job_actions = relationship("PostJobActionAssociation", back_populates="job")
+    post_job_actions = relationship("PostJobActionAssociation", back_populates="job", cascade_backrefs=False)
     input_library_datasets = relationship("JobToInputLibraryDatasetAssociation", back_populates="job")
     output_library_datasets = relationship("JobToOutputLibraryDatasetAssociation", back_populates="job")
     external_output_metadata = relationship("JobExternalOutputMetadata", back_populates="job")
     tasks = relationship("Task", back_populates="job")
     output_datasets = relationship("JobToOutputDatasetAssociation", back_populates="job")
     state_history = relationship("JobStateHistory")
     text_metrics = relationship("JobMetricText")
     numeric_metrics = relationship("JobMetricNumeric")
     interactivetool_entry_points = relationship("InteractiveToolEntryPoint", back_populates="job", uselist=True)
     implicit_collection_jobs_association = relationship(
-        "ImplicitCollectionJobsJobAssociation", back_populates="job", uselist=False
+        "ImplicitCollectionJobsJobAssociation", back_populates="job", uselist=False, cascade_backrefs=False
     )
     container = relationship("JobContainerAssociation", back_populates="job", uselist=False)
-    data_manager_association = relationship("DataManagerJobAssociation", back_populates="job", uselist=False)
+    data_manager_association = relationship(
+        "DataManagerJobAssociation", back_populates="job", uselist=False, cascade_backrefs=False
+    )
     history_dataset_collection_associations = relationship("HistoryDatasetCollectionAssociation", back_populates="job")
-    workflow_invocation_step = relationship("WorkflowInvocationStep", back_populates="job", uselist=False)
+    workflow_invocation_step = relationship(
+        "WorkflowInvocationStep", back_populates="job", uselist=False, cascade_backrefs=False
+    )
 
     any_output_dataset_collection_instances_deleted: column_property  # defined at the end of this module
     any_output_dataset_deleted: column_property  # defined at the end of this module
 
     dict_collection_visible_keys = ["id", "state", "exit_code", "update_time", "create_time", "galaxy_version"]
     dict_element_visible_keys = [
         "id",
@@ -1363,15 +1400,15 @@
         "command_version",
         "copied_from_job_id",
     ]
 
     _numeric_metric = JobMetricNumeric
     _text_metric = JobMetricText
 
-    states = JobState
+    states: TypeAlias = JobState
 
     # states that are not expected to change, except through admin action or re-scheduling
     terminal_states = [states.OK, states.ERROR, states.DELETED]
     # deleting state should not turn back into any of the non-ready states
     finished_states = terminal_states + [states.DELETING]
     #: job states where the job hasn't finished and the model may still change
     non_ready_states = [
@@ -1592,14 +1629,18 @@
         if dataset is None and dataset_id is not None:
             assoc.dataset_id = dataset_id
         add_object_to_object_session(self, assoc)
         self.input_datasets.append(assoc)
 
     def add_output_dataset(self, name, dataset):
         joda = JobToOutputDatasetAssociation(name, dataset)
+        if dataset.dataset.job is None:
+            # Only set job if dataset doesn't already have associated job.
+            # database operation tools that make copies should not modify the job here.
+            dataset.dataset.job = self
         add_object_to_object_session(self, joda)
         self.output_datasets.append(joda)
 
     def add_input_dataset_collection(self, name, dataset_collection):
         self.input_dataset_collections.append(JobToInputDatasetCollectionAssociation(name, dataset_collection))
 
     def add_input_dataset_collection_element(self, name, dataset_collection_element):
@@ -1622,14 +1663,21 @@
 
     def add_output_library_dataset(self, name, dataset):
         self.output_library_datasets.append(JobToOutputLibraryDatasetAssociation(name, dataset))
 
     def add_post_job_action(self, pja):
         self.post_job_actions.append(PostJobActionAssociation(pja, self))
 
+    def get_change_datatype_actions(self):
+        return {
+            pja.post_job_action.output_name: pja.post_job_action.action_arguments["newtype"]
+            for pja in self.post_job_actions
+            if pja.post_job_action.action_type == "ChangeDatatypeAction"
+        }
+
     @property
     def all_entry_points_configured(self):
         # consider an actual DB attribute for this.
         all_configured = True
         for ep in self.interactivetool_entry_points:
             all_configured = ep.configured and all_configured
         return all_configured
@@ -1809,14 +1857,15 @@
 
     def to_dict(self, view="collection", system_details=False):
         if view == "admin_job_list":
             rval = super().to_dict(view="collection")
         else:
             rval = super().to_dict(view=view)
         rval["tool_id"] = self.tool_id
+        rval["tool_version"] = self.tool_version
         rval["history_id"] = self.history_id
         if system_details or view == "admin_job_list":
             # System level details that only admins should have.
             rval["external_id"] = self.job_runner_external_id
             rval["command_line"] = self.command_line
             rval["traceback"] = self.traceback
         if view == "admin_job_list":
@@ -1954,58 +2003,40 @@
         statements = [
             text(
                 """
             UPDATE dataset
             SET
                 state = :state,
                 update_time = :update_time
-            WHERE id IN (
-                SELECT hda.dataset_id FROM history_dataset_association hda
-                INNER JOIN job_to_output_dataset jtod
-                ON jtod.dataset_id = hda.id AND jtod.job_id = :job_id
-            );
-        """
-            ),
-            text(
-                """
-            UPDATE dataset
-            SET
-                state = :state,
-                update_time = :update_time
-            WHERE id IN (
-                SELECT ldda.dataset_id FROM library_dataset_dataset_association ldda
-                INNER JOIN job_to_output_library_dataset jtold
-                ON jtold.ldda_id = ldda.id AND jtold.job_id = :job_id
-            );
+            WHERE
+                dataset.job_id = :job_id
         """
             ),
             text(
                 """
             UPDATE history_dataset_association
             SET
                 info = :info,
                 update_time = :update_time
-            WHERE id IN (
-                SELECT jtod.dataset_id
-                FROM job_to_output_dataset jtod
-                WHERE jtod.job_id = :job_id
-            );
+            FROM dataset
+            WHERE
+                history_dataset_association.dataset_id = dataset.id
+                AND dataset.job_id = :job_id;
         """
             ),
             text(
                 """
             UPDATE library_dataset_dataset_association
             SET
                 info = :info,
                 update_time = :update_time
-            WHERE id IN (
-                SELECT jtold.ldda_id
-                FROM job_to_output_library_dataset jtold
-                WHERE jtold.job_id = :job_id
-            );
+            FROM dataset
+            WHERE
+                library_dataset_dataset_association.dataset_id = dataset.id
+                AND dataset.job_id = :job_id;
         """
             ),
         ]
         sa_session = object_session(self)
         update_time = now()
         self.update_hdca_update_time_for_job(
             update_time=update_time, sa_session=sa_session, supports_skip_locked=supports_skip_locked
@@ -2407,15 +2438,17 @@
 
 
 class ImplicitCollectionJobs(Base, Serializable):
     __tablename__ = "implicit_collection_jobs"
 
     id = Column(Integer, primary_key=True)
     populated_state = Column(TrimmedString(64), default="new", nullable=False)
-    jobs = relationship("ImplicitCollectionJobsJobAssociation", back_populates="implicit_collection_jobs")
+    jobs = relationship(
+        "ImplicitCollectionJobsJobAssociation", back_populates="implicit_collection_jobs", cascade_backrefs=False
+    )
 
     class populated_states(str, Enum):
         NEW = "new"  # New implicit jobs object, unpopulated job associations
         OK = "ok"  # Job associations are set and fixed.
         FAILED = "failed"  # There were issues populating job associations, object is in error.
 
     def __init__(self, populated_state=None):
@@ -2461,28 +2494,30 @@
     )
 
     def __init__(self, action_type, workflow_step=None, output_name=None, action_arguments=None):
         self.action_type = action_type
         self.output_name = output_name
         self.action_arguments = action_arguments
         self.workflow_step = workflow_step
+        ensure_object_added_to_session(self, object_in_session=workflow_step)
 
 
 class PostJobActionAssociation(Base, RepresentById):
     __tablename__ = "post_job_action_association"
 
     id = Column(Integer, primary_key=True)
     job_id = Column(Integer, ForeignKey("job.id"), index=True, nullable=False)
     post_job_action_id = Column(Integer, ForeignKey("post_job_action.id"), index=True, nullable=False)
     post_job_action = relationship("PostJobAction")
     job = relationship("Job", back_populates="post_job_actions")
 
     def __init__(self, pja, job=None, job_id=None):
         if job is not None:
             self.job = job
+            ensure_object_added_to_session(self, object_in_session=job)
         elif job_id is not None:
             self.job_id = job_id
         else:
             raise Exception("PostJobActionAssociation must be created with a job or a job_id.")
         self.post_job_action = pja
 
 
@@ -2770,15 +2805,15 @@
 
     id = Column(Integer, primary_key=True)
     create_time = Column(DateTime, default=now)
     update_time = Column(DateTime, default=now, onupdate=now)
     name = Column(String(255), index=True, unique=True)
     deleted = Column(Boolean, index=True, default=False)
     quotas = relationship("GroupQuotaAssociation", back_populates="group")
-    roles = relationship("GroupRoleAssociation", back_populates="group")
+    roles = relationship("GroupRoleAssociation", back_populates="group", cascade_backrefs=False)
     users = relationship("UserGroupAssociation", back_populates="group")
 
     dict_collection_visible_keys = ["id", "name"]
     dict_element_visible_keys = ["id", "name"]
 
     def __init__(self, name=None):
         self.name = name
@@ -2845,14 +2880,15 @@
     update_time = Column(DateTime, default=now, onupdate=now)
 
     user = relationship("User", back_populates="all_notifications")
     notification = relationship("Notification", back_populates="user_notification_associations")
 
     def __init__(self, user, notification):
         self.user = user
+        ensure_object_added_to_session(self, object_in_session=user)
         self.notification = notification
 
 
 def is_hda(d):
     return isinstance(d, HistoryDatasetAssociation)
 
 
@@ -2978,17 +3014,17 @@
         "HistoryRatingAssociation",
         order_by=lambda: HistoryRatingAssociation.id,  # type: ignore[has-type]
         back_populates="history",
     )
     default_permissions = relationship("DefaultHistoryPermissions", back_populates="history")
     users_shared_with = relationship("HistoryUserShareAssociation", back_populates="history")
     galaxy_sessions = relationship("GalaxySessionToHistoryAssociation", back_populates="history")
-    workflow_invocations = relationship("WorkflowInvocation", back_populates="history")
+    workflow_invocations = relationship("WorkflowInvocation", back_populates="history", cascade_backrefs=False)
     user = relationship("User", back_populates="histories")
-    jobs = relationship("Job", back_populates="history")
+    jobs = relationship("Job", back_populates="history", cascade_backrefs=False)
 
     update_time = column_property(
         select(func.max(HistoryAudit.update_time)).where(HistoryAudit.history_id == id).scalar_subquery(),
     )
     users_shared_with_count: column_property  # defined at the end of this module
     average_rating: column_property  # defined at the end of this module
 
@@ -2997,24 +3033,28 @@
     # returns a list of users that history is shared with.
     users_shared_with_dot_users = association_proxy("users_shared_with", "user")
 
     dict_collection_visible_keys = ["id", "name", "published", "deleted"]
     dict_element_visible_keys = [
         "id",
         "name",
-        "genome_build",
+        "archived",
+        "create_time",
         "deleted",
+        "empty",
+        "genome_build",
+        "hid_counter",
+        "importable",
+        "preferred_object_store_id",
         "purged",
-        "archived",
-        "update_time",
         "published",
-        "importable",
         "slug",
-        "empty",
-        "preferred_object_store_id",
+        "tags",
+        "update_time",
+        "username",
     ]
     default_name = "Unnamed history"
 
     def __init__(self, id=None, name=None, user=None):
         self.id = id
         self.name = name or History.default_name
         self.deleted = False
@@ -3041,14 +3081,20 @@
             self._pending_additions.append(item)
 
     @property
     def empty(self):
         return self.hid_counter is None or self.hid_counter == 1
 
     @property
+    def username(self):
+        if user := self.user:
+            return user.username
+        return None
+
+    @property
     def count(self):
         return self.hid_counter - 1
 
     def add_pending_items(self, set_output_hid=True):
         # These are assumed to be either copies of existing datasets or new, empty datasets,
         # so we don't need to set the quota.
         self.add_datasets(
@@ -3498,14 +3544,15 @@
     create_time = Column(DateTime, default=now)
     update_time = Column(DateTime, default=now, onupdate=now)
     group = relationship("Group", back_populates="roles")
     role = relationship("Role", back_populates="groups")
 
     def __init__(self, group, role):
         self.group = group
+        ensure_object_added_to_session(self, object_in_session=group)
         self.role = role
 
 
 class Role(Base, Dictifiable, RepresentById):
     __tablename__ = "role"
 
     id = Column(Integer, primary_key=True)
@@ -3598,15 +3645,15 @@
     update_time = Column(DateTime, default=now, onupdate=now)
     name = Column(String(255), index=True, unique=True)
     description = Column(TEXT)
     bytes = Column(BigInteger)
     operation = Column(String(8))
     deleted = Column(Boolean, index=True, default=False)
     quota_source_label = Column(String(32), default=None)
-    default = relationship("DefaultQuotaAssociation", back_populates="quota")
+    default = relationship("DefaultQuotaAssociation", back_populates="quota", cascade_backrefs=False)
     groups = relationship("GroupQuotaAssociation", back_populates="quota")
     users = relationship("UserQuotaAssociation", back_populates="quota")
 
     dict_collection_visible_keys = ["id", "name", "quota_source_label"]
     dict_element_visible_keys = [
         "id",
         "name",
@@ -3668,14 +3715,15 @@
         UNREGISTERED = "unregistered"
         REGISTERED = "registered"
 
     def __init__(self, type, quota):
         assert type in self.types.__members__.values(), "Invalid type"
         self.type = type
         self.quota = quota
+        ensure_object_added_to_session(self, object_in_session=quota)
 
 
 class DatasetPermissions(Base, RepresentById):
     __tablename__ = "dataset_permissions"
 
     id = Column(Integer, primary_key=True)
     create_time = Column(DateTime, default=now)
@@ -3708,14 +3756,15 @@
     library = relationship("Library", back_populates="actions")
     role = relationship("Role")
 
     def __init__(self, action, library_item, role):
         self.action = action
         if isinstance(library_item, Library):
             self.library = library_item
+            ensure_object_added_to_session(self, object_in_session=library_item)
         else:
             raise Exception(f"Invalid Library specified: {library_item.__class__.__name__}")
         self.role = role
 
 
 class LibraryFolderPermissions(Base, RepresentById):
     __tablename__ = "library_folder_permissions"
@@ -3729,14 +3778,15 @@
     folder = relationship("LibraryFolder", back_populates="actions")
     role = relationship("Role")
 
     def __init__(self, action, library_item, role):
         self.action = action
         if isinstance(library_item, LibraryFolder):
             self.folder = library_item
+            ensure_object_added_to_session(self, object_in_session=library_item)
         else:
             raise Exception(f"Invalid LibraryFolder specified: {library_item.__class__.__name__}")
         self.role = role
 
 
 class LibraryDatasetPermissions(Base, RepresentById):
     __tablename__ = "library_dataset_permissions"
@@ -3750,14 +3800,15 @@
     library_dataset = relationship("LibraryDataset", back_populates="actions")
     role = relationship("Role")
 
     def __init__(self, action, library_item, role):
         self.action = action
         if isinstance(library_item, LibraryDataset):
             self.library_dataset = library_item
+            ensure_object_added_to_session(self, object_in_session=library_item)
         else:
             raise Exception(f"Invalid LibraryDataset specified: {library_item.__class__.__name__}")
         self.role = role
 
 
 class LibraryDatasetDatasetAssociationPermissions(Base, RepresentById):
     __tablename__ = "library_dataset_dataset_association_permissions"
@@ -3815,16 +3866,15 @@
         self.history = history
         self.action = action
         self.role = role
 
 
 class StorableObject:
     def flush(self):
-        sa_session = object_session(self)
-        if sa_session:
+        if sa_session := object_session(self):
             with transaction(sa_session):
                 sa_session.commit()
 
 
 class Dataset(Base, StorableObject, Serializable):
     __tablename__ = "dataset"
 
@@ -3873,21 +3923,22 @@
             lambda: and_(
                 Dataset.id == LibraryDatasetDatasetAssociation.dataset_id,  # type: ignore[attr-defined]
                 LibraryDatasetDatasetAssociation.deleted == false(),  # type: ignore[has-type]
             )
         ),
         viewonly=True,
     )
-    hashes = relationship("DatasetHash", back_populates="dataset")
+    hashes = relationship("DatasetHash", back_populates="dataset", cascade_backrefs=False)
     sources = relationship("DatasetSource", back_populates="dataset")
-    history_associations = relationship("HistoryDatasetAssociation", back_populates="dataset")
+    history_associations = relationship("HistoryDatasetAssociation", back_populates="dataset", cascade_backrefs=False)
     library_associations = relationship(
         "LibraryDatasetDatasetAssociation",
         primaryjoin=(lambda: LibraryDatasetDatasetAssociation.table.c.dataset_id == Dataset.id),
         back_populates="dataset",
+        cascade_backrefs=False,
     )
 
     # failed_metadata is only valid as DatasetInstance state currently
     states = DatasetState
 
     non_ready_states = (states.NEW, states.UPLOAD, states.QUEUED, states.RUNNING, states.SETTING_METADATA)
     ready_states = tuple(set(states.__members__.values()) - set(non_ready_states))
@@ -3986,14 +4037,24 @@
 
     @property
     def quota_source_info(self):
         object_store_id = self.object_store_id
         quota_source_map = self.object_store.get_quota_source_map()
         return quota_source_map.get_quota_source_info(object_store_id)
 
+    @property
+    def device_source_label(self):
+        return self.device_source_info.label
+
+    @property
+    def device_source_info(self):
+        object_store_id = self.object_store_id
+        device_source_map = self.object_store.get_quota_source_map()
+        return device_source_map.get_device_source_info(object_store_id)
+
     def set_file_name(self, filename):
         if not filename:
             self.external_filename = None
         else:
             self.external_filename = filename
 
     def _assert_object_store_set(self):
@@ -4030,16 +4091,15 @@
 
     @property
     def store_by(self):
         store_by = self.object_store.get_store_by(self)
         return store_by
 
     def extra_files_path_name_from(self, object_store):
-        store_by = self.store_by
-        if store_by is not None:
+        if (store_by := self.store_by) is not None:
             return f"dataset_{getattr(self, store_by)}_files"
         else:
             return None
 
     @property
     def extra_files_path_name(self):
         return self.extra_files_path_name_from(self.object_store)
@@ -4054,20 +4114,18 @@
                 return os.path.getsize(self.external_filename)
             except OSError:
                 return 0
         assert self.object_store
         return self.object_store.size(self)
 
     @overload
-    def get_size(self, nice_size: Literal[False], calculate_size: bool = True) -> int:
-        ...
+    def get_size(self, nice_size: Literal[False], calculate_size: bool = True) -> int: ...
 
     @overload
-    def get_size(self, nice_size: Literal[True], calculate_size: bool = True) -> str:
-        ...
+    def get_size(self, nice_size: Literal[True], calculate_size: bool = True) -> str: ...
 
     def get_size(self, nice_size: bool = False, calculate_size: bool = True) -> Union[int, str]:
         """Returns the size of the data on disk"""
         if self.file_size:
             if nice_size:
                 return galaxy.util.nice_size(self.file_size)
             else:
@@ -4103,16 +4161,15 @@
             db_session.commit()
         return self.total_size
 
     def set_total_size(self):
         if self.file_size is None:
             self.set_size()
         self.total_size = self.file_size or 0
-        rel_path = self._extra_files_rel_path
-        if rel_path is not None:
+        if (rel_path := self._extra_files_rel_path) is not None:
             if self.object_store.exists(self, extra_dir=rel_path, dir_only=True):
                 for root, _, files in os.walk(self.extra_files_path):
                     self.total_size += sum(
                         os.path.getsize(os.path.join(root, file))
                         for file in files
                         if os.path.exists(os.path.join(root, file))
                     )
@@ -4141,16 +4198,15 @@
     def full_delete(self):
         """Remove the file and extra files, marks deleted and purged"""
         # os.unlink( self.file_name )
         try:
             self.object_store.delete(self)
         except galaxy.exceptions.ObjectNotFound:
             pass
-        rel_path = self._extra_files_rel_path
-        if rel_path is not None:
+        if (rel_path := self._extra_files_rel_path) is not None:
             if self.object_store.exists(self, extra_dir=rel_path, dir_only=True):
                 self.object_store.delete(self, entire_dir=True, extra_dir=rel_path, dir_only=True)
         # TODO: purge metadata files
         self.deleted = True
         self.purged = True
 
     def get_access_roles(self, security_agent):
@@ -4311,14 +4367,16 @@
 
     states = Dataset.states
     _state: Optional[str]
     conversion_messages = Dataset.conversion_messages
     permitted_actions = Dataset.permitted_actions
     purged: bool
     creating_job_associations: List[Union[JobToOutputDatasetCollectionAssociation, JobToOutputDatasetAssociation]]
+    copied_from_history_dataset_association: Optional["HistoryDatasetAssociation"]
+    copied_from_library_dataset_dataset_association: Optional["LibraryDatasetDatasetAssociation"]
 
     validated_states = DatasetValidatedState
 
     def __init__(
         self,
         id=None,
         hid=None,
@@ -4340,14 +4398,16 @@
         visible=True,
         create_dataset=False,
         sa_session=None,
         extended_metadata=None,
         flush=True,
         metadata_deferred=False,
         creating_job_id=None,
+        copied_from_history_dataset_association=None,
+        copied_from_library_dataset_dataset_association=None,
     ):
         self.name = name or "Unnamed dataset"
         self.id = id
         self.info = info
         self.blurb = blurb
         self.peek = peek
         self.tool_version = tool_version
@@ -4363,25 +4423,30 @@
         ):  # dbkey is stored in metadata, only set if non-zero, or else we could clobber one supplied by input 'metadata'
             self._metadata["dbkey"] = listify(dbkey)
         self.deleted = deleted
         self.visible = visible
         self.validated_state = validated_state
         self.validated_state_message = validated_state_message
         # Relationships
+        if copied_from_history_dataset_association:
+            self.copied_from_history_dataset_association_id = copied_from_history_dataset_association.id
+        if copied_from_library_dataset_dataset_association:
+            self.copied_from_library_dataset_dataset_association_id = copied_from_library_dataset_dataset_association.id
         if not dataset and create_dataset:
             # Had to pass the sqlalchemy session in order to create a new dataset
             dataset = Dataset(state=Dataset.states.NEW)
             dataset.job_id = creating_job_id
             if flush:
                 sa_session.add(dataset)
                 with transaction(sa_session):
                     sa_session.commit()
         elif dataset:
             add_object_to_object_session(self, dataset)
         self.dataset = dataset
+        ensure_object_added_to_session(self, object_in_session=dataset)
         self.parent_id = parent_id
 
     @property
     def peek(self):
         return self._peek
 
     @peek.setter
@@ -4414,14 +4479,24 @@
                 if sa_session:
                     sa_session.add(self.dataset)
                 self.dataset.state = state
 
     def set_metadata_success_state(self):
         self._state = None
 
+    def get_object_store_id(self):
+        return self.dataset.object_store_id
+
+    object_store_id = property(get_object_store_id)
+
+    def get_quota_source_label(self):
+        return self.dataset.quota_source_label
+
+    quota_source_label = property(get_quota_source_label)
+
     def get_file_name(self, sync_cache=True) -> str:
         if self.dataset.purged:
             return ""
         return self.dataset.get_file_name(sync_cache=sync_cache)
 
     def set_file_name(self, filename: str):
         return self.dataset.set_file_name(filename)
@@ -4793,15 +4868,15 @@
             except Exception as e:
                 log.warning(e)
             return lst
 
         return _source_dataset_chain(self, [])
 
     @property
-    def creating_job(self):
+    def creating_job(self) -> Optional[Job]:
         # TODO this should work with `return self.dataset.job` (revise failing unit tests)
         creating_job_associations = None
         if self.creating_job_associations:
             creating_job_associations = self.creating_job_associations
         else:
             inherit_chain = self.source_dataset_chain
             if inherit_chain:
@@ -4921,30 +4996,26 @@
     Resource class that creates a relation between a dataset and a user history.
     """
 
     def __init__(
         self,
         hid=None,
         history=None,
-        copied_from_history_dataset_association=None,
-        copied_from_library_dataset_dataset_association=None,
         sa_session=None,
         **kwd,
     ):
         """
         Create a a new HDA and associate it with the given history.
         """
         # FIXME: sa_session is must be passed to DataSetInstance if the create_dataset
         # parameter is True so that the new object can be flushed.  Is there a better way?
         DatasetInstance.__init__(self, sa_session=sa_session, **kwd)
         self.hid = hid
         # Relationships
         self.history = history
-        self.copied_from_history_dataset_association = copied_from_history_dataset_association
-        self.copied_from_library_dataset_dataset_association = copied_from_library_dataset_dataset_association
 
     def __strict_check_before_flush__(self):
         if self.extension != "len":
             # TODO: Custom builds (with .len extension) do not get a history or a HID.
             # These should get some other type of permanent storage, perhaps UserDatasetAssociation ?
             # Everything else needs to have a hid and a history
             if not self.history and not getattr(self, "history_id", None):
@@ -4970,15 +5041,15 @@
             hist = state.get_history(attr.key, True)
 
             if not hist.has_changes():
                 continue
 
             # hist.deleted holds old value(s)
             changes[attr.key] = hist.deleted
-        if self.update_time and self.state == self.states.OK and not self.deleted:
+        if changes and self.update_time and self.state == self.states.OK and not self.deleted:
             # We only record changes to HDAs that exist in the database and have a update_time
             new_values = {}
             new_values["name"] = changes.get("name", self.name)
             new_values["dbkey"] = changes.get("dbkey", self.dbkey)
             new_values["extension"] = changes.get("extension", self.extension)
             new_values["extended_metadata_id"] = changes.get("extended_metadata_id", self.extended_metadata_id)
             for k, v in new_values.items():
@@ -5370,15 +5441,15 @@
     update_time = Column(DateTime, default=now, onupdate=now)
     name = Column(String(255), index=True)
     deleted = Column(Boolean, index=True, default=False)
     purged = Column(Boolean, index=True, default=False)
     description = Column(TEXT)
     synopsis = Column(TEXT)
     root_folder = relationship("LibraryFolder", back_populates="library_root")
-    actions = relationship("LibraryPermissions", back_populates="library")
+    actions = relationship("LibraryPermissions", back_populates="library", cascade_backrefs=False)
 
     permitted_actions = get_permitted_actions(filter="LIBRARY")
     dict_collection_visible_keys = ["id", "name"]
     dict_element_visible_keys = ["id", "deleted", "name", "description", "synopsis", "root_folder_id", "create_time"]
 
     def __init__(self, name=None, description=None, synopsis=None, root_folder=None):
         self.name = name or "Unnamed library"
@@ -5489,15 +5560,15 @@
             "and_(LibraryDataset.folder_id == LibraryFolder.id, not_(LibraryDataset.deleted), LibraryDataset.library_dataset_dataset_association_id.isnot(None))"
         ),
         order_by=(lambda: asc(LibraryDataset._name)),
         viewonly=True,
     )
 
     library_root = relationship("Library", back_populates="root_folder")
-    actions = relationship("LibraryFolderPermissions", back_populates="folder")
+    actions = relationship("LibraryFolderPermissions", back_populates="folder", cascade_backrefs=False)
 
     dict_element_visible_keys = [
         "id",
         "parent_id",
         "name",
         "description",
         "item_count",
@@ -5614,15 +5685,15 @@
         primaryjoin=(
             "and_(LibraryDataset.id == LibraryDatasetDatasetAssociation.library_dataset_id, \
              not_(LibraryDataset.library_dataset_dataset_association_id == LibraryDatasetDatasetAssociation.id))"
         ),
         viewonly=True,
         uselist=True,
     )
-    actions = relationship("LibraryDatasetPermissions", back_populates="library_dataset")
+    actions = relationship("LibraryDatasetPermissions", back_populates="library_dataset", cascade_backrefs=False)
 
     # This class acts as a proxy to the currently selected LDDA
     upload_options = [
         ("upload_file", "Upload files"),
         ("upload_directory", "Upload directory of files"),
         ("upload_paths", "Upload files from filesystem paths"),
         ("import_from_history", "Import datasets from your current history"),
@@ -5706,30 +5777,25 @@
             elif isinstance(val, list):
                 val = ", ".join(str(v) for v in val)
             rval[f"metadata_{name}"] = val
         return rval
 
 
 class LibraryDatasetDatasetAssociation(DatasetInstance, HasName, Serializable):
+
     def __init__(
         self,
-        copied_from_history_dataset_association=None,
-        copied_from_library_dataset_dataset_association=None,
         library_dataset=None,
         user=None,
         sa_session=None,
         **kwd,
     ):
         # FIXME: sa_session is must be passed to DataSetInstance if the create_dataset
         # parameter in kwd is True so that the new object can be flushed.  Is there a better way?
         DatasetInstance.__init__(self, sa_session=sa_session, **kwd)
-        if copied_from_history_dataset_association:
-            self.copied_from_history_dataset_association_id = copied_from_history_dataset_association.id
-        if copied_from_library_dataset_dataset_association:
-            self.copied_from_library_dataset_dataset_association_id = copied_from_library_dataset_dataset_association.id
         self.library_dataset = library_dataset
         self.user = user
 
     def to_history_dataset_association(self, target_history, parent_id=None, add_to_history=False, visible=None):
         sa_session = object_session(self)
         hda = HistoryDatasetAssociation(
             name=self.name,
@@ -5873,15 +5939,15 @@
                 SET update_time =
                     (SELECT update_time
                     FROM library_dataset_dataset_association
                     WHERE id = :ldda_id)
                 WHERE exists (SELECT 1 FROM parent_folders_of
                     WHERE library_folder.id = parent_folders_of.folder_id)
             """
-        ).execution_options(autocommit=True)
+        )
 
         with object_session(self).bind.connect() as conn, conn.begin():
             ret = conn.execute(sql, {"library_dataset_id": ldda.library_dataset_id, "ldda_id": ldda.id})
 
         if ret.rowcount < 1:
             log.warning(f"Attempt to updated parent folder times failed: {ret.rowcount} records updated.")
 
@@ -6151,15 +6217,15 @@
     def __init__(self, id=None, collection_type=None, populated=True, element_count=None):
         self.id = id
         self.collection_type = collection_type
         if not populated:
             self.populated_state = DatasetCollection.populated_states.NEW
         self.element_count = element_count
 
-    def _get_nested_collection_attributes(
+    def _build_nested_collection_attributes_stmt(
         self,
         collection_attributes: Optional[Iterable[str]] = None,
         element_attributes: Optional[Iterable[str]] = None,
         hda_attributes: Optional[Iterable[str]] = None,
         dataset_attributes: Optional[Iterable[str]] = None,
         dataset_permission_attributes: Optional[Iterable[str]] = None,
         return_entities: Optional[
@@ -6178,47 +6244,46 @@
         collection_attributes = collection_attributes or ()
         element_attributes = element_attributes or ()
         hda_attributes = hda_attributes or ()
         dataset_attributes = dataset_attributes or ()
         dataset_permission_attributes = dataset_permission_attributes or ()
         return_entities = return_entities or ()
         dataset_collection = self
-        db_session = object_session(self)
         dc = alias(DatasetCollection)
         dce = alias(DatasetCollectionElement)
-
         depth_collection_type = dataset_collection.collection_type
         order_by_columns = [dce.c.element_index]
         nesting_level = 0
 
         def attribute_columns(column_collection, attributes, nesting_level=None):
             label_fragment = f"_{nesting_level}" if nesting_level is not None else ""
             return [getattr(column_collection, a).label(f"{a}{label_fragment}") for a in attributes]
 
         q = (
-            db_session.query(
+            select(
                 *attribute_columns(dce.c, element_attributes, nesting_level),
                 *attribute_columns(dc.c, collection_attributes, nesting_level),
             )
             .select_from(dce, dc)
             .join(dce, dce.c.dataset_collection_id == dc.c.id)
             .filter(dc.c.id == dataset_collection.id)
         )
+
         while ":" in depth_collection_type:
             nesting_level += 1
-            inner_dc = alias(DatasetCollection)
             inner_dce = alias(DatasetCollectionElement)
+            inner_dc = alias(DatasetCollection)
             order_by_columns.append(inner_dce.c.element_index)
-            q = q.join(
-                inner_dc, and_(inner_dc.c.id == dce.c.child_collection_id, dce.c.dataset_collection_id == dc.c.id)
-            ).outerjoin(inner_dce, inner_dce.c.dataset_collection_id == inner_dc.c.id)
-            q = q.add_columns(
-                *attribute_columns(inner_dce.c, element_attributes, nesting_level),
-                *attribute_columns(inner_dc.c, collection_attributes, nesting_level),
-            )
+            q = q.outerjoin(inner_dce, inner_dce.c.dataset_collection_id == dce.c.child_collection_id)
+            if collection_attributes:
+                q = q.join(inner_dc, inner_dc.c.id == dce.c.child_collection_id)
+                q = q.add_columns(
+                    *attribute_columns(inner_dc.c, collection_attributes, nesting_level),
+                )
+            q = q.add_columns(*attribute_columns(inner_dce.c, element_attributes, nesting_level))
             dce = inner_dce
             dc = inner_dc
             depth_collection_type = depth_collection_type.split(":", 1)[1]
         if inner_filter:
             q = q.filter(inner_filter.produce_filter(dc.c))
 
         if (
@@ -6233,41 +6298,52 @@
             q = q.join(DatasetPermissions)
         q = (
             q.add_columns(*attribute_columns(HistoryDatasetAssociation, hda_attributes))
             .add_columns(*attribute_columns(Dataset, dataset_attributes))
             .add_columns(*attribute_columns(DatasetPermissions, dataset_permission_attributes))
         )
         for entity in return_entities:
-            q = q.add_entity(entity)
+            q = q.add_columns(entity)
             if entity == DatasetCollectionElement:
                 q = q.filter(entity.id == dce.c.id)
-        return q.distinct().order_by(*order_by_columns)
+
+        q = q.order_by(*order_by_columns)
+        return q
 
     @property
     def dataset_states_and_extensions_summary(self):
         if not hasattr(self, "_dataset_states_and_extensions_summary"):
-            q = self._get_nested_collection_attributes(hda_attributes=("extension",), dataset_attributes=("state",))
+            stmt = self._build_nested_collection_attributes_stmt(
+                hda_attributes=("extension",), dataset_attributes=("state",)
+            )
+            # With DISTINCT, all columns that appear in the ORDER BY clause must appear in the SELECT clause.
+            stmt = stmt.add_columns(*stmt._order_by_clauses)
+            stmt = stmt.distinct()
+
+            tuples = object_session(self).execute(stmt)
+
             extensions = set()
             states = set()
-            for extension, state in q:
+            for extension, state, *_ in tuples:  # we discard the added columns from the order-by clause
                 states.add(state)
                 extensions.add(extension)
 
             self._dataset_states_and_extensions_summary = (states, extensions)
 
         return self._dataset_states_and_extensions_summary
 
     @property
     def has_deferred_data(self):
         if not hasattr(self, "_has_deferred_data"):
             has_deferred_data = False
             if object_session(self):
                 # TODO: Optimize by just querying without returning the states...
-                q = self._get_nested_collection_attributes(dataset_attributes=("state",))
-                for (state,) in q:
+                stmt = self._build_nested_collection_attributes_stmt(dataset_attributes=("state",))
+                tuples = object_session(self).execute(stmt)
+                for (state,) in tuples:
                     if state == Dataset.states.DEFERRED:
                         has_deferred_data = True
                         break
             else:
                 # This will be in a remote tool evaluation context, so can't query database
                 for dataset_element in self.dataset_elements_and_identifiers():
                     if dataset_element.hda.state == Dataset.states.DEFERRED:
@@ -6280,21 +6356,24 @@
     @property
     def populated_optimized(self):
         if not hasattr(self, "_populated_optimized"):
             _populated_optimized = True
             if ":" not in self.collection_type:
                 _populated_optimized = self.populated_state == DatasetCollection.populated_states.OK
             else:
-                q = self._get_nested_collection_attributes(
+                stmt = self._build_nested_collection_attributes_stmt(
                     collection_attributes=("populated_state",),
                     inner_filter=InnerCollectionFilter(
                         "populated_state", operator.__ne__, DatasetCollection.populated_states.OK
                     ),
                 )
-                _populated_optimized = q.session.query(~exists(q.subquery())).scalar()
+                stmt = stmt.subquery()
+                stmt = select(~exists(stmt))
+                session = object_session(self)
+                _populated_optimized = session.scalar(stmt)
 
             self._populated_optimized = _populated_optimized
 
         return self._populated_optimized
 
     @property
     def populated(self):
@@ -6302,45 +6381,33 @@
         if top_level_populated and self.has_subcollections:
             return all(e.child_collection and e.child_collection.populated for e in self.elements)
         return top_level_populated
 
     @property
     def dataset_action_tuples(self):
         if not hasattr(self, "_dataset_action_tuples"):
-            q = self._get_nested_collection_attributes(dataset_permission_attributes=("action", "role_id"))
-            _dataset_action_tuples = []
-            for _dataset_action_tuple in q:
-                if _dataset_action_tuple[0] is None:
-                    continue
-                _dataset_action_tuples.append(_dataset_action_tuple)
-
-            self._dataset_action_tuples = _dataset_action_tuples
-
+            stmt = self._build_nested_collection_attributes_stmt(dataset_permission_attributes=("action", "role_id"))
+            tuples = object_session(self).execute(stmt)
+            self._dataset_action_tuples = [(action, role_id) for action, role_id in tuples if action is not None]
         return self._dataset_action_tuples
 
     @property
-    def element_identifiers_extensions_and_paths(self):
-        q = self._get_nested_collection_attributes(
-            element_attributes=("element_identifier",), hda_attributes=("extension",), return_entities=(Dataset,)
-        )
-        return [(row[:-2], row.extension, row.Dataset.get_file_name()) for row in q]
-
-    @property
     def element_identifiers_extensions_paths_and_metadata_files(
         self,
     ) -> List[List[Any]]:
         results = []
         if object_session(self):
-            q = self._get_nested_collection_attributes(
+            stmt = self._build_nested_collection_attributes_stmt(
                 element_attributes=("element_identifier",),
                 hda_attributes=("extension",),
                 return_entities=(HistoryDatasetAssociation, Dataset),
             )
+            tuples = object_session(self).execute(stmt)
             # element_identifiers, extension, path
-            for row in q:
+            for row in tuples:
                 result = [row[:-3], row.extension, row.Dataset.get_file_name()]
                 hda = row.HistoryDatasetAssociation
                 result.append(hda.get_metadata_file_paths_and_extensions())
                 results.append(result)
         else:
             # This will be in a remote tool evaluation context, so can't query database
             for dataset_element in self.dataset_elements_and_identifiers():
@@ -6377,15 +6444,17 @@
             for element in self.elements:
                 element.child_collection.finalize(collection_type_description.child_collection_type_description())
 
     @property
     def dataset_instances(self):
         db_session = object_session(self)
         if db_session and self.id:
-            return self._get_nested_collection_attributes(return_entities=(HistoryDatasetAssociation,)).all()
+            stmt = self._build_nested_collection_attributes_stmt(return_entities=(HistoryDatasetAssociation,))
+            tuples = db_session.execute(stmt).all()
+            return [tuple[0] for tuple in tuples]
         else:
             # Sessionless context
             instances = []
             for element in self.elements:
                 if element.is_collection:
                     instances.extend(element.child_collection.dataset_instances)
                 else:
@@ -6393,15 +6462,17 @@
                     instances.append(instance)
             return instances
 
     @property
     def dataset_elements(self):
         db_session = object_session(self)
         if db_session and self.id:
-            return self._get_nested_collection_attributes(return_entities=(DatasetCollectionElement,)).all()
+            stmt = self._build_nested_collection_attributes_stmt(return_entities=(DatasetCollectionElement,))
+            tuples = db_session.execute(stmt).all()
+            return [tuple[0] for tuple in tuples]
         elements = []
         for element in self.elements:
             if element.is_collection:
                 elements.extend(element.child_collection.dataset_elements)
             else:
                 elements.append(element)
         return elements
@@ -6478,17 +6549,19 @@
         if flush:
             session = object_session(self)
             with transaction(session):
                 session.commit()
         return new_collection
 
     def replace_failed_elements(self, replacements):
-        hda_id_to_element = dict(
-            self._get_nested_collection_attributes(return_entities=[DatasetCollectionElement], hda_attributes=["id"])
+        stmt = self._build_nested_collection_attributes_stmt(
+            return_entities=[DatasetCollectionElement], hda_attributes=["id"]
         )
+        tuples = object_session(self).execute(stmt).all()
+        hda_id_to_element = dict(tuples)
         for failed, replacement in replacements.items():
             element = hda_id_to_element.get(failed.id)
             if element:
                 element.hda = replacement
 
     def set_from_dict(self, new_data):
         # Nothing currently editable in this class.
@@ -6745,18 +6818,20 @@
     def job_state_summary_dict(self):
         if self.job_state_summary:
             return self.job_state_summary._asdict()
 
     @property
     def dataset_dbkeys_and_extensions_summary(self):
         if not hasattr(self, "_dataset_dbkeys_and_extensions_summary"):
-            rows = self.collection._get_nested_collection_attributes(hda_attributes=("_metadata", "extension"))
+            stmt = self.collection._build_nested_collection_attributes_stmt(hda_attributes=("_metadata", "extension"))
+            tuples = object_session(self).execute(stmt)
+
             extensions = set()
             dbkeys = set()
-            for row in rows:
+            for row in tuples:
                 if row is not None:
                     dbkey_field = row._metadata.get("dbkey")
                     if isinstance(dbkey_field, list):
                         for dbkey in dbkey_field:
                             dbkeys.add(dbkey)
                     else:
                         dbkeys.add(dbkey_field)
@@ -6814,17 +6889,17 @@
         copied_from_history_dataset_collection_association_chain = []
         src_hdca = self
         while src_hdca.copied_from_history_dataset_collection_association:
             src_hdca = src_hdca.copied_from_history_dataset_collection_association
             copied_from_history_dataset_collection_association_chain.append(
                 serialization_options.get_identifier(id_encoder, src_hdca)
             )
-        rval[
-            "copied_from_history_dataset_collection_association_id_chain"
-        ] = copied_from_history_dataset_collection_association_chain
+        rval["copied_from_history_dataset_collection_association_id_chain"] = (
+            copied_from_history_dataset_collection_association_chain
+        )
         serialization_options.attach_identifier(id_encoder, self, rval)
         return rval
 
     def to_dict(self, view="collection"):
         original_dict_value = super().to_dict(view=view)
         if view == "dbkeysandextensions":
             (dbkeys, extensions) = self.dataset_dbkeys_and_extensions_summary
@@ -6942,15 +7017,15 @@
             dce.child_collection_id == ep.c.dataset_collection_id
         )
         parents_cte = parents_cte.union(rec)
 
         # join parents to hdca, look for matching hdca_id
         hdca = aliased(HDCA, name="hdca")
         jointohdca = parents_cte.join(hdca, hdca.collection_id == parents_cte.c.dataset_collection_id)
-        qry = Query(hdca.id).select_entity_from(jointohdca).filter(hdca.id == self.id)
+        qry = Query(hdca.id).select_from(jointohdca).filter(hdca.id == self.id)
 
         results = qry.with_session(sa_session).all()
         return len(results) > 0
 
 
 class LibraryDatasetCollectionAssociation(Base, DatasetCollectionInstance, RepresentById):
     """Associates a DatasetCollection with a library folder."""
@@ -7218,15 +7293,17 @@
     session_key = Column(TrimmedString(255), index=True, unique=True)
     is_valid = Column(Boolean, default=False)
     # saves a reference to the previous session so we have a way to chain them together
     prev_session_id = Column(Integer)
     disk_usage = Column(Numeric(15, 0), index=True)
     last_action = Column(DateTime)
     current_history = relationship("History")
-    histories = relationship("GalaxySessionToHistoryAssociation", back_populates="galaxy_session")
+    histories = relationship(
+        "GalaxySessionToHistoryAssociation", back_populates="galaxy_session", cascade_backrefs=False
+    )
     user = relationship("User", back_populates="galaxy_sessions")
 
     def __init__(self, is_valid=False, **kwd):
         super().__init__(**kwd)
         self.is_valid = is_valid
         self.last_action = self.last_action or now()
 
@@ -7255,14 +7332,15 @@
     session_id = Column(Integer, ForeignKey("galaxy_session.id"), index=True)
     history_id = Column(Integer, ForeignKey("history.id"), index=True)
     galaxy_session = relationship("GalaxySession", back_populates="histories")
     history = relationship("History", back_populates="galaxy_sessions")
 
     def __init__(self, galaxy_session, history):
         self.galaxy_session = galaxy_session
+        ensure_object_added_to_session(self, object_in_session=galaxy_session)
         add_object_to_object_session(self, history)
         self.history = history
 
 
 class UCI:
     def __init__(self):
         self.id = None
@@ -7301,14 +7379,15 @@
     )
     workflows = relationship(
         "Workflow",
         back_populates="stored_workflow",
         cascade="all, delete-orphan",
         primaryjoin=(lambda: StoredWorkflow.id == Workflow.stored_workflow_id),  # type: ignore[has-type]
         order_by=lambda: -Workflow.id,  # type: ignore[has-type]
+        cascade_backrefs=False,
     )
     latest_workflow = relationship(
         "Workflow",
         post_update=True,
         primaryjoin=(lambda: StoredWorkflow.latest_workflow_id == Workflow.id),  # type: ignore[has-type]
         lazy=False,
     )
@@ -7417,14 +7496,28 @@
     def copy_tags_from(self, target_user, source_workflow):
         # Override to only copy owner tags.
         for src_swta in source_workflow.owner_tags:
             new_swta = src_swta.copy()
             new_swta.user = target_user
             self.tags.append(new_swta)
 
+    def invocation_counts(self) -> InvocationsStateCounts:
+        sa_session = object_session(self)
+        stmt = (
+            select([WorkflowInvocation.state, func.count(WorkflowInvocation.state)])
+            .select_from(StoredWorkflow)
+            .join(Workflow, Workflow.stored_workflow_id == StoredWorkflow.id)
+            .join(WorkflowInvocation, WorkflowInvocation.workflow_id == Workflow.id)
+            .group_by(WorkflowInvocation.state)
+            .where(StoredWorkflow.id == self.id)
+        )
+        rows = sa_session.execute(stmt).all()
+        rows_as_dict = dict(r for r in rows if r[0] is not None)
+        return InvocationsStateCounts(rows_as_dict)
+
     def to_dict(self, view="collection", value_mapper=None):
         rval = super().to_dict(view=view, value_mapper=value_mapper)
         rval["latest_workflow_uuid"] = (lambda uuid: str(uuid) if self.latest_workflow.uuid else None)(
             self.latest_workflow.uuid
         )
         return rval
 
@@ -7469,14 +7562,15 @@
         cascade="all, delete-orphan",
         lazy=False,
     )
     parent_workflow_steps = relationship(
         "WorkflowStep",
         primaryjoin=(lambda: Workflow.id == WorkflowStep.subworkflow_id),  # type: ignore[has-type]
         back_populates="subworkflow",
+        cascade_backrefs=False,
     )
     stored_workflow = relationship(
         "StoredWorkflow",
         primaryjoin=(lambda: StoredWorkflow.id == Workflow.stored_workflow_id),
         back_populates="workflows",
     )
 
@@ -7635,15 +7729,15 @@
     position = Column(MutableJSONType)
     config = Column(JSONType)
     order_index: int = Column(Integer)
     when_expression = Column(JSONType)
     uuid = Column(UUIDType)
     label = Column(Unicode(255))
     temp_input_connections: Optional[InputConnDictType]
-    parent_comment_id = Column(Integer, ForeignKey("workflow_comment.id"), nullable=True)
+    parent_comment_id = Column(Integer, ForeignKey("workflow_comment.id"), index=True, nullable=True)
 
     parent_comment = relationship(
         "WorkflowComment",
         primaryjoin=(lambda: WorkflowComment.id == WorkflowStep.parent_comment_id),
         back_populates="child_steps",
     )
 
@@ -7657,22 +7751,25 @@
         "WorkflowStepTagAssociation", order_by=lambda: WorkflowStepTagAssociation.id, back_populates="workflow_step"
     )
     annotations = relationship(
         "WorkflowStepAnnotationAssociation",
         order_by=lambda: WorkflowStepAnnotationAssociation.id,
         back_populates="workflow_step",
     )
-    post_job_actions = relationship("PostJobAction", back_populates="workflow_step")
+    post_job_actions = relationship("PostJobAction", back_populates="workflow_step", cascade_backrefs=False)
     inputs = relationship("WorkflowStepInput", back_populates="workflow_step")
-    workflow_outputs = relationship("WorkflowOutput", back_populates="workflow_step")
+    workflow_outputs = relationship("WorkflowOutput", back_populates="workflow_step", cascade_backrefs=False)
     output_connections = relationship(
         "WorkflowStepConnection", primaryjoin=(lambda: WorkflowStepConnection.output_step_id == WorkflowStep.id)
     )
     workflow = relationship(
-        "Workflow", primaryjoin=(lambda: Workflow.id == WorkflowStep.workflow_id), back_populates="steps"
+        "Workflow",
+        primaryjoin=(lambda: Workflow.id == WorkflowStep.workflow_id),
+        back_populates="steps",
+        cascade_backrefs=False,
     )
 
     # Injected attributes
     # TODO: code using these should be refactored to not depend on these non-persistent fields
     module: Optional["WorkflowModule"]
     state: Optional["DefaultToolState"]
     upgrade_messages: Optional[Dict]
@@ -7761,14 +7858,15 @@
         return step_input
 
     def add_connection(self, input_name, output_name, output_step, input_subworkflow_step_index=None):
         step_input = self.get_or_add_input(input_name)
 
         conn = WorkflowStepConnection()
         conn.input_step_input = step_input
+        ensure_object_added_to_session(conn, object_in_session=step_input)
         conn.output_name = output_name
         add_object_to_object_session(conn, output_step)
         conn.output_step = output_step
         if self.subworkflow:
             if input_subworkflow_step_index is not None:
                 input_subworkflow_step = self.subworkflow.step_by_index(input_subworkflow_step_index)
             else:
@@ -7882,16 +7980,15 @@
                 association = WorkflowStepAnnotationAssociation()
                 association.user = user
                 association.workflow_step = copied_step
                 association.annotation = annotation.annotation
                 annotations.append(association)
             copied_step.annotations = annotations
 
-        subworkflow = self.subworkflow
-        if subworkflow:
+        if subworkflow := self.subworkflow:
             copied_subworkflow = subworkflow.copy()
             copied_step.subworkflow = copied_subworkflow
             for subworkflow_step, copied_subworkflow_step in zip(subworkflow.steps, copied_subworkflow.steps):
                 subworkflow_step_mapping[subworkflow_step.id] = copied_subworkflow_step
 
         for old_conn, new_conn in zip(self.input_connections, copied_step.input_connections):
             new_conn.input_step_input = copied_step.get_or_add_input(old_conn.input_name)
@@ -7951,14 +8048,15 @@
         cascade="all",
         primaryjoin=(lambda: WorkflowStepInput.workflow_step_id == WorkflowStep.id),
     )
     connections = relationship(
         "WorkflowStepConnection",
         back_populates="input_step_input",
         primaryjoin=(lambda: WorkflowStepConnection.input_step_input_id == WorkflowStepInput.id),
+        cascade_backrefs=False,
     )
 
     def __init__(self, workflow_step):
         add_object_to_object_session(self, workflow_step)
         self.workflow_step = workflow_step
         self.default_value_set = False
 
@@ -8042,14 +8140,15 @@
         "WorkflowStep",
         back_populates="workflow_outputs",
         primaryjoin=(lambda: WorkflowStep.id == WorkflowOutput.workflow_step_id),
     )
 
     def __init__(self, workflow_step, output_name=None, label=None, uuid=None):
         self.workflow_step = workflow_step
+        ensure_object_added_to_session(self, object_in_session=workflow_step)
         self.output_name = output_name
         self.label = label
         self.uuid = get_uuid(uuid)
 
     def copy(self, copied_step):
         copied_output = WorkflowOutput(copied_step)
         copied_output.output_name = self.output_name
@@ -8077,15 +8176,15 @@
     order_index: int = Column(Integer)
     workflow_id = Column(Integer, ForeignKey("workflow.id"), index=True, nullable=False)
     position = Column(MutableJSONType)
     size = Column(JSONType)
     type = Column(String(16))
     color = Column(String(16))
     data = Column(JSONType)
-    parent_comment_id = Column(Integer, ForeignKey("workflow_comment.id"), nullable=True)
+    parent_comment_id = Column(Integer, ForeignKey("workflow_comment.id"), index=True, nullable=True)
 
     workflow = relationship(
         "Workflow",
         primaryjoin=(lambda: Workflow.id == WorkflowComment.workflow_id),
         back_populates="comments",
     )
 
@@ -8120,20 +8219,20 @@
 
         if self.child_steps:
             comment_dict["child_steps"] = [step.order_index for step in self.child_steps]
 
         if self.child_comments:
             comment_dict["child_comments"] = [comment.order_index for comment in self.child_comments]
 
-        WorkflowCommentModel(__root__=comment_dict)
+        WorkflowCommentModel(root=comment_dict)
 
         return comment_dict
 
     def from_dict(dict):
-        WorkflowCommentModel(__root__=dict)
+        WorkflowCommentModel(root=dict)
 
         comment = WorkflowComment()
         comment.order_index = dict.get("id", 0)
         comment.type = dict.get("type", "text")
         comment.position = dict.get("position", None)
         comment.size = dict.get("size", None)
         comment.color = dict.get("color", "none")
@@ -8181,40 +8280,55 @@
     state = Column(TrimmedString(64), index=True)
     scheduler = Column(TrimmedString(255), index=True)
     handler = Column(TrimmedString(255), index=True)
     uuid = Column(UUIDType())
     history_id = Column(Integer, ForeignKey("history.id"), index=True)
 
     history = relationship("History", back_populates="workflow_invocations")
-    input_parameters = relationship("WorkflowRequestInputParameter", back_populates="workflow_invocation")
-    step_states = relationship("WorkflowRequestStepState", back_populates="workflow_invocation")
-    input_step_parameters = relationship("WorkflowRequestInputStepParameter", back_populates="workflow_invocation")
-    input_datasets = relationship("WorkflowRequestToInputDatasetAssociation", back_populates="workflow_invocation")
+    input_parameters = relationship(
+        "WorkflowRequestInputParameter", back_populates="workflow_invocation", cascade_backrefs=False
+    )
+    step_states = relationship("WorkflowRequestStepState", back_populates="workflow_invocation", cascade_backrefs=False)
+    input_step_parameters = relationship(
+        "WorkflowRequestInputStepParameter", back_populates="workflow_invocation", cascade_backrefs=False
+    )
+    input_datasets = relationship(
+        "WorkflowRequestToInputDatasetAssociation", back_populates="workflow_invocation", cascade_backrefs=False
+    )
     input_dataset_collections = relationship(
-        "WorkflowRequestToInputDatasetCollectionAssociation", back_populates="workflow_invocation"
+        "WorkflowRequestToInputDatasetCollectionAssociation",
+        back_populates="workflow_invocation",
+        cascade_backrefs=False,
     )
     subworkflow_invocations = relationship(
         "WorkflowInvocationToSubworkflowInvocationAssociation",
         primaryjoin=(
             lambda: WorkflowInvocationToSubworkflowInvocationAssociation.workflow_invocation_id == WorkflowInvocation.id
         ),
         back_populates="parent_workflow_invocation",
         uselist=True,
     )
     steps = relationship(
         "WorkflowInvocationStep",
         back_populates="workflow_invocation",
         order_by=lambda: WorkflowInvocationStep.order_index,
+        cascade_backrefs=False,
     )
     workflow: Workflow = relationship("Workflow")
     output_dataset_collections = relationship(
-        "WorkflowInvocationOutputDatasetCollectionAssociation", back_populates="workflow_invocation"
+        "WorkflowInvocationOutputDatasetCollectionAssociation",
+        back_populates="workflow_invocation",
+        cascade_backrefs=False,
+    )
+    output_datasets = relationship(
+        "WorkflowInvocationOutputDatasetAssociation", back_populates="workflow_invocation", cascade_backrefs=False
+    )
+    output_values = relationship(
+        "WorkflowInvocationOutputValue", back_populates="workflow_invocation", cascade_backrefs=False
     )
-    output_datasets = relationship("WorkflowInvocationOutputDatasetAssociation", back_populates="workflow_invocation")
-    output_values = relationship("WorkflowInvocationOutputValue", back_populates="workflow_invocation")
     messages = relationship("WorkflowInvocationMessage", back_populates="workflow_invocation")
 
     dict_collection_visible_keys = [
         "id",
         "update_time",
         "create_time",
         "workflow_id",
@@ -8228,22 +8342,15 @@
         "create_time",
         "workflow_id",
         "history_id",
         "uuid",
         "state",
     ]
 
-    class states(str, Enum):
-        NEW = "new"  # Brand new workflow invocation... maybe this should be same as READY
-        READY = "ready"  # Workflow ready for another iteration of scheduling.
-        SCHEDULED = "scheduled"  # Workflow has been scheduled.
-        CANCELLED = "cancelled"
-        CANCELLING = "cancelling"  # invocation scheduler will cancel job in next iteration
-        FAILED = "failed"
-
+    states = InvocationState
     non_terminal_states = [states.NEW, states.READY]
 
     def create_subworkflow_invocation_for_step(self, step):
         assert step.type == "subworkflow"
         subworkflow_invocation = WorkflowInvocation()
         self.attach_subworkflow_invocation_for_step(step, subworkflow_invocation)
         return subworkflow_invocation
@@ -8278,15 +8385,15 @@
         """Indicates the workflow invocation is somehow active - and in
         particular valid actions may be performed on its
         WorkflowInvocationSteps.
         """
         states = WorkflowInvocation.states
         return self.state in [states.NEW, states.READY]
 
-    def set_state(self, state: "WorkflowInvocation.states"):
+    def set_state(self, state: InvocationState):
         session = object_session(self)
         priority_states = (WorkflowInvocation.states.CANCELLING, WorkflowInvocation.states.CANCELLED)
         if session and self.id and state not in priority_states:
             # generate statement that will not revert CANCELLING or CANCELLED back to anything non-terminal
             session.execute(
                 update(WorkflowInvocation.table)
                 .where(
@@ -8414,28 +8521,31 @@
     def add_output(self, workflow_output, step, output_object):
         if not hasattr(output_object, "history_content_type"):
             # assuming this is a simple type, just JSON-ify it and stick in the database. In the future
             # I'd like parameter_inputs to have datasets and collections as valid parameter types so
             # dispatch on actual object and not step type.
             output_assoc = WorkflowInvocationOutputValue()
             output_assoc.workflow_invocation = self
+            ensure_object_added_to_session(output_assoc, object_in_session=self)
             output_assoc.workflow_output = workflow_output
             output_assoc.workflow_step = step
             output_assoc.value = output_object
             self.output_values.append(output_assoc)
         elif output_object.history_content_type == "dataset":
             output_assoc = WorkflowInvocationOutputDatasetAssociation()
             output_assoc.workflow_invocation = self
+            ensure_object_added_to_session(output_assoc, object_in_session=self)
             output_assoc.workflow_output = workflow_output
             output_assoc.workflow_step = step
             output_assoc.dataset = output_object
             self.output_datasets.append(output_assoc)
         elif output_object.history_content_type == "dataset_collection":
             output_assoc = WorkflowInvocationOutputDatasetCollectionAssociation()
             output_assoc.workflow_invocation = self
+            ensure_object_added_to_session(output_assoc, object_in_session=self)
             output_assoc.workflow_output = workflow_output
             output_assoc.workflow_step = step
             output_assoc.dataset_collection = output_object
             self.output_dataset_collections.append(output_assoc)
         else:
             raise Exception("Unknown output type encountered")
 
@@ -8536,14 +8646,17 @@
         invocation_attrs["output_values"] = output_values
 
         serialization_options.attach_identifier(id_encoder, self, invocation_attrs)
         return invocation_attrs
 
     def to_dict(self, view="collection", value_mapper=None, step_details=False, legacy_job_state=False):
         rval = super().to_dict(view=view, value_mapper=value_mapper)
+        if rval["state"] is None:
+            # bugs could result in no state being set
+            rval["state"] = self.states.FAILED
         if view == "element":
             steps = []
             for step in self.steps:
                 if step_details:
                     v = step.to_dict(view="element")
                 else:
                     v = step.to_dict(view="collection")
@@ -8608,17 +8721,15 @@
                     "workflow_step_id": output_assoc.workflow_step_id,
                 }
 
             output_collections = {}
             for output_assoc in self.output_dataset_collections:
                 label = output_assoc.workflow_output.label
                 if not label:
-                    label = (
-                        label
-                    ) = f"{output_assoc.workflow_output.output_name} (Step {output_assoc.workflow_output.workflow_step.order_index + 1})"
+                    label = f"{output_assoc.workflow_output.output_name} (Step {output_assoc.workflow_output.workflow_step.order_index + 1})"
 
                 output_collections[label] = {
                     "src": "hdca",
                     "id": output_assoc.dataset_collection_id,
                     "workflow_step_id": output_assoc.workflow_step_id,
                 }
 
@@ -8694,16 +8805,15 @@
         return False
 
     def set_handler(self, handler):
         self.handler = handler
 
     def log_str(self):
         extra = ""
-        safe_id = getattr(self, "id", None)
-        if safe_id is not None:
+        if (safe_id := getattr(self, "id", None)) is not None:
             extra += f"id={safe_id}"
         else:
             extra += "unflushed"
         return f"{self.__class__.__name__}[{extra}]"
 
 
 class WorkflowInvocationToSubworkflowInvocationAssociation(Base, Dictifiable, RepresentById):
@@ -8820,18 +8930,22 @@
     implicit_collection_jobs_id = Column(Integer, ForeignKey("implicit_collection_jobs.id"), index=True, nullable=True)
     action = Column(MutableJSONType, nullable=True)
 
     workflow_step = relationship("WorkflowStep")
     job = relationship("Job", back_populates="workflow_invocation_step", uselist=False)
     implicit_collection_jobs = relationship("ImplicitCollectionJobs", uselist=False)
     output_dataset_collections = relationship(
-        "WorkflowInvocationStepOutputDatasetCollectionAssociation", back_populates="workflow_invocation_step"
+        "WorkflowInvocationStepOutputDatasetCollectionAssociation",
+        back_populates="workflow_invocation_step",
+        cascade_backrefs=False,
     )
     output_datasets = relationship(
-        "WorkflowInvocationStepOutputDatasetAssociation", back_populates="workflow_invocation_step"
+        "WorkflowInvocationStepOutputDatasetAssociation",
+        back_populates="workflow_invocation_step",
+        cascade_backrefs=False,
     )
     workflow_invocation = relationship("WorkflowInvocation", back_populates="steps")
     output_value = relationship(
         "WorkflowInvocationOutputValue",
         foreign_keys="[WorkflowInvocationStep.workflow_invocation_id, WorkflowInvocationStep.workflow_step_id]",
         primaryjoin=(
             lambda: and_(
@@ -8863,35 +8977,32 @@
         "job_id",
         "workflow_step_id",
         "subworkflow_invocation_id",
         "state",
         "action",
     ]
 
-    class states(str, Enum):
-        NEW = "new"  # Brand new workflow invocation step
-        READY = "ready"  # Workflow invocation step ready for another iteration of scheduling.
-        SCHEDULED = "scheduled"  # Workflow invocation step has been scheduled.
-        # CANCELLED = 'cancelled',  TODO: implement and expose
-        # FAILED = 'failed',  TODO: implement and expose
+    states = InvocationStepState
 
     @property
     def is_new(self):
         return self.state == self.states.NEW
 
     def add_output(self, output_name, output_object):
         if output_object.history_content_type == "dataset":
             output_assoc = WorkflowInvocationStepOutputDatasetAssociation()
             output_assoc.workflow_invocation_step = self
+            ensure_object_added_to_session(output_assoc, object_in_session=self)
             output_assoc.dataset = output_object
             output_assoc.output_name = output_name
             self.output_datasets.append(output_assoc)
         elif output_object.history_content_type == "dataset_collection":
             output_assoc = WorkflowInvocationStepOutputDatasetCollectionAssociation()
             output_assoc.workflow_invocation_step = self
+            ensure_object_added_to_session(output_assoc, object_in_session=self)
             output_assoc.dataset_collection = output_object
             output_assoc.output_name = output_name
             self.output_dataset_collections.append(output_assoc)
         else:
             raise Exception("Unknown output type encountered")
 
     @property
@@ -8987,17 +9098,19 @@
 
             outputs = {}
             for output_assoc in self.output_datasets:
                 name = output_assoc.output_name
                 outputs[name] = {
                     "src": "hda",
                     "id": output_assoc.dataset.id,
-                    "uuid": str(output_assoc.dataset.dataset.uuid)
-                    if output_assoc.dataset.dataset.uuid is not None
-                    else None,
+                    "uuid": (
+                        str(output_assoc.dataset.dataset.uuid)
+                        if output_assoc.dataset.dataset.uuid is not None
+                        else None
+                    ),
                 }
 
             output_collections = {}
             for output_assoc in self.output_dataset_collections:
                 name = output_assoc.output_name
                 output_collections[name] = {
                     "src": "hdca",
@@ -9522,34 +9635,48 @@
     def save(self):
         self.sa_session.add(self)
         with transaction(self.sa_session):
             self.sa_session.commit()
 
     @classmethod
     def store(cls, server_url, association):
-        try:
+        """
+        Create an Association instance
+        (Required by social_core.storage.AssociationMixin interface)
+        """
+
+        def get_or_create():
             stmt = select(PSAAssociation).filter_by(server_url=server_url, handle=association.handle).limit(1)
             assoc = cls.sa_session.scalars(stmt).first()
-        except IndexError:
-            assoc = cls(server_url=server_url, handle=association.handle)
+            return assoc or cls(server_url=server_url, handle=association.handle)
+
+        assoc = get_or_create()
         assoc.secret = base64.encodebytes(association.secret).decode()
         assoc.issued = association.issued
         assoc.lifetime = association.lifetime
         assoc.assoc_type = association.assoc_type
         cls.sa_session.add(assoc)
         with transaction(cls.sa_session):
             cls.sa_session.commit()
 
     @classmethod
     def get(cls, *args, **kwargs):
+        """
+        Get an Association instance
+        (Required by social_core.storage.AssociationMixin interface)
+        """
         stmt = select(PSAAssociation).filter_by(*args, **kwargs)
-        return cls.sa_session.scalars(stmt)
+        return cls.sa_session.scalars(stmt).all()
 
     @classmethod
     def remove(cls, ids_to_delete):
+        """
+        Remove an Association instance
+        (Required by social_core.storage.AssociationMixin interface)
+        """
         stmt = (
             delete(PSAAssociation)
             .where(PSAAssociation.id.in_(ids_to_delete))
             .execution_options(synchronize_session="fetch")
         )
         PSAAssociation.sa_session.execute(stmt)
 
@@ -9572,14 +9699,17 @@
     def save(self):
         self.sa_session.add(self)
         with transaction(self.sa_session):
             self.sa_session.commit()
 
     @classmethod
     def get_code(cls, code):
+        """
+        (Required by social_core.storage.CodeMixin interface)
+        """
         stmt = select(PSACode).where(PSACode.code == code).limit(1)
         return cls.sa_session.scalars(stmt).first()
 
 
 class PSANonce(Base, NonceMixin, RepresentById):
     __tablename__ = "psa_nonce"
 
@@ -9599,14 +9729,18 @@
     def save(self):
         self.sa_session.add(self)
         with transaction(self.sa_session):
             self.sa_session.commit()
 
     @classmethod
     def use(cls, server_url, timestamp, salt):
+        """
+        Create a Nonce instance
+        (Required by social_core.storage.NonceMixin interface)
+        """
         try:
             stmt = select(PSANonce).where(server_url=server_url, timestamp=timestamp, salt=salt).limit(1)
             return cls.sa_session.scalars(stmt).first()
         except IndexError:
             instance = cls(server_url=server_url, timestamp=timestamp, salt=salt)
             cls.sa_session.add(instance)
             with transaction(cls.sa_session):
@@ -9635,21 +9769,26 @@
     def save(self):
         self.sa_session.add(self)
         with transaction(self.sa_session):
             self.sa_session.commit()
 
     @classmethod
     def load(cls, token):
+        """
+        (Required by social_core.storage.PartialMixin interface)
+        """
         stmt = select(PSAPartial).where(PSAPartial.token == token).limit(1)
         return cls.sa_session.scalars(stmt).first()
 
     @classmethod
     def destroy(cls, token):
-        partial = cls.load(token)
-        if partial:
+        """
+        (Required by social_core.storage.PartialMixin interface)
+        """
+        if partial := cls.load(token):
             session = cls.sa_session
             session.execute(delete(partial))
             with transaction(session):
                 session.commit()
 
 
 class UserAuthnzToken(Base, UserMixin, RepresentById):
@@ -9691,73 +9830,123 @@
 
     def save(self):
         self.sa_session.add(self)
         with transaction(self.sa_session):
             self.sa_session.commit()
 
     @classmethod
-    def username_max_length(cls):
-        # Note: This is the maximum field length set for the username column of the galaxy_user table.
-        # A better alternative is to retrieve this number from the table, instead of this const value.
-        return 255
-
-    @classmethod
     def changed(cls, user):
+        """
+        The given user instance is ready to be saved
+        (Required by social_core.storage.UserMixin interface)
+        """
         cls.sa_session.add(user)
         with transaction(cls.sa_session):
             cls.sa_session.commit()
 
     @classmethod
     def get_username(cls, user):
+        """
+        Return the username for given user
+        (Required by social_core.storage.UserMixin interface)
+        """
         return getattr(user, "username", None)
 
     @classmethod
+    def user_model(cls):
+        """
+        Return the user model
+        (Required by social_core.storage.UserMixin interface)
+        """
+        return User
+
+    @classmethod
+    def username_max_length(cls):
+        """
+        Return the max length for username
+        (Required by social_core.storage.UserMixin interface)
+        """
+        # Note: This is the maximum field length set for the username column of the galaxy_user table.
+        # A better alternative is to retrieve this number from the table, instead of this const value.
+        return 255
+
+    @classmethod
+    def user_exists(cls, *args, **kwargs):
+        """
+        Return True/False if a User instance exists with the given arguments.
+        Arguments are directly passed to filter() manager method.
+        (Required by social_core.storage.UserMixin interface)
+        """
+        stmt_user = select(User).filter_by(*args, **kwargs)
+        stmt_count = select(func.count()).select_from(stmt_user)
+        return cls.sa_session.scalar(stmt_count) > 0
+
+    @classmethod
     def create_user(cls, *args, **kwargs):
         """
         This is used by PSA authnz, do not use directly.
         Prefer using the user manager.
+        (Required by social_core.storage.UserMixin interface)
         """
-        instance = User(*args, **kwargs)
-        if cls.email_exists(instance.email):
+        model = cls.user_model()
+        instance = model(*args, **kwargs)
+        if cls.get_users_by_email(instance.email):
             raise Exception(f"User with this email '{instance.email}' already exists.")
         instance.set_random_password()
         cls.sa_session.add(instance)
         with transaction(cls.sa_session):
             cls.sa_session.commit()
         return instance
 
     @classmethod
     def get_user(cls, pk):
-        return UserAuthnzToken.sa_session.get(User, pk)
+        """
+        Return user instance for given id
+        (Required by social_core.storage.UserMixin interface)
+        """
+        return cls.sa_session.get(User, pk)
 
     @classmethod
-    def email_exists(cls, email):
-        stmt = select(User).where(func.lower(User.email) == email.lower()).limit(1)
-        return bool(cls.sa_session.scalars(stmt).first())
+    def get_users_by_email(cls, email):
+        """
+        Return users instances for given email address
+        (Required by social_core.storage.UserMixin interface)
+        """
+        stmt = select(User).where(func.lower(User.email) == email.lower())
+        return cls.sa_session.scalars(stmt).all()
 
     @classmethod
     def get_social_auth(cls, provider, uid):
+        """
+        Return UserSocialAuth for given provider and uid
+        (Required by social_core.storage.UserMixin interface)
+        """
         uid = str(uid)
-        try:
-            stmt = select(UserAuthnzToken).filter_by(provider=provider, uid=uid).limit(1)
-            return cls.sa_session.scalars(stmt).first()
-        except IndexError:
-            return None
+        stmt = select(cls).filter_by(provider=provider, uid=uid).limit(1)
+        return cls.sa_session.scalars(stmt).first()
 
     @classmethod
     def get_social_auth_for_user(cls, user, provider=None, id=None):
-        stmt = select(UserAuthnzToken).filter_by(user_id=user.id)
+        """
+        Return all the UserSocialAuth instances for given user
+        (Required by social_core.storage.UserMixin interface)
+        """
+        stmt = select(cls).filter_by(user_id=user.id)
         if provider:
             stmt = stmt.filter_by(provider=provider)
         if id:
             stmt = stmt.filter_by(id=id)
-        return cls.sa_session.scalars(stmt)
+        return cls.sa_session.scalars(stmt).all()
 
     @classmethod
     def create_social_auth(cls, user, uid, provider):
+        """
+        Create a UserSocialAuth instance for given user
+        (Required by social_core.storage.UserMixin interface)
+        """
         uid = str(uid)
         instance = cls(user=user, uid=uid, provider=provider)
         cls.sa_session.add(instance)
         with transaction(cls.sa_session):
             cls.sa_session.commit()
         return instance
 
@@ -9870,14 +10059,15 @@
         "latest_revision_id",
         "slug",
         "published",
         "importable",
         "deleted",
         "username",
         "email_hash",
+        "create_time",
         "update_time",
     ]
 
     def to_dict(self, view="element"):
         rval = super().to_dict(view=view)
         rev = []
         for a in self.revisions:
@@ -9956,14 +10146,15 @@
 
     user = relationship("User")
     revisions = relationship(
         "VisualizationRevision",
         back_populates="visualization",
         cascade="all, delete-orphan",
         primaryjoin=(lambda: Visualization.id == VisualizationRevision.visualization_id),
+        cascade_backrefs=False,
     )
     latest_revision = relationship(
         "VisualizationRevision",
         post_update=True,
         primaryjoin=(lambda: Visualization.latest_revision_id == VisualizationRevision.id),
         lazy=False,
     )
@@ -10714,15 +10905,15 @@
         nullable=True,
     ),
     Column("name", TrimmedString(255)),
     Column("info", TrimmedString(255)),
     Column("blurb", TrimmedString(255)),
     Column("peek", TEXT, key="_peek"),
     Column("tool_version", TEXT),
-    Column("extension", TrimmedString(64)),
+    Column("extension", TrimmedString(64), index=True),
     Column("metadata", MetadataType, key="_metadata"),
     Column("metadata_deferred", Boolean, key="metadata_deferred"),
     Column("parent_id", Integer, ForeignKey("history_dataset_association.id"), nullable=True),
     Column("designation", TrimmedString(255)),
     Column("deleted", Boolean, index=True, default=False),
     Column("visible", Boolean),
     Column("extended_metadata_id", Integer, ForeignKey("extended_metadata.id"), index=True),
@@ -10945,31 +11136,35 @@
         ),
     ),
 )
 
 # ----------------------------------------------------------------------------------------
 # The following statements must not precede the mapped models defined above.
 
-Job.any_output_dataset_collection_instances_deleted = column_property(
-    exists(HistoryDatasetCollectionAssociation.id).where(
-        and_(
-            Job.id == JobToOutputDatasetCollectionAssociation.job_id,
-            HistoryDatasetCollectionAssociation.id == JobToOutputDatasetCollectionAssociation.dataset_collection_id,
-            HistoryDatasetCollectionAssociation.deleted == true(),
-        )
+Job.any_output_dataset_collection_instances_deleted = deferred(
+    column_property(
+        exists(HistoryDatasetCollectionAssociation.id).where(
+            and_(
+                Job.id == JobToOutputDatasetCollectionAssociation.job_id,
+                HistoryDatasetCollectionAssociation.id == JobToOutputDatasetCollectionAssociation.dataset_collection_id,
+                HistoryDatasetCollectionAssociation.deleted == true(),
+            )
+        ),
     )
 )
 
-Job.any_output_dataset_deleted = column_property(
-    exists(HistoryDatasetAssociation.id).where(
-        and_(
-            Job.id == JobToOutputDatasetAssociation.job_id,
-            HistoryDatasetAssociation.table.c.id == JobToOutputDatasetAssociation.dataset_id,
-            HistoryDatasetAssociation.table.c.deleted == true(),
-        )
+Job.any_output_dataset_deleted = deferred(
+    column_property(
+        exists(HistoryDatasetAssociation.id).where(
+            and_(
+                Job.id == JobToOutputDatasetAssociation.job_id,
+                HistoryDatasetAssociation.table.c.id == JobToOutputDatasetAssociation.dataset_id,
+                HistoryDatasetAssociation.table.c.deleted == true(),
+            )
+        ),
     )
 )
 
 History.average_rating = column_property(
     select(func.avg(HistoryRatingAssociation.rating))
     .where(HistoryRatingAssociation.history_id == History.id)
     .scalar_subquery(),
```

### Comparing `galaxy-data-23.2.1/galaxy/model/base.py` & `galaxy-data-24.0.0/galaxy/model/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Shared model and mapping code between Galaxy and Tool Shed, trying to
 generalize to generic database connections.
 """
+
 import contextlib
 import logging
 import os
 import threading
 from contextvars import ContextVar
 from inspect import (
     getmembers,
@@ -16,14 +17,15 @@
     Type,
     TYPE_CHECKING,
     Union,
 )
 
 from sqlalchemy import event
 from sqlalchemy.orm import (
+    object_session,
     scoped_session,
     Session,
     sessionmaker,
 )
 
 from galaxy.util.bunch import Bunch
 
@@ -62,24 +64,28 @@
     """
     In the event of a database disconnect, if there exists an active database
     transaction, that transaction becomes invalidated. Accessing the database
     will raise sqlalchemy.exc.PendingRollbackError. This handles this situation
     by rolling back the invalidated transaction.
     Ref: https://docs.sqlalchemy.org/en/14/errors.html#can-t-reconnect-until-invalid-transaction-is-rolled-back
     """
-    if session and session.connection().invalidated:
-        log.error("Database transaction rolled back due to invalid state.")
+    assert session
+    if isinstance(session, scoped_session):
+        session = session()
+    trans = session.get_transaction()
+    if (trans and not trans.is_active) or session.connection().invalidated:
         session.rollback()
+        log.error("Database transaction rolled back due to inactive session transaction or invalid connection state.")
 
 
 # TODO: Refactor this to be a proper class, not a bunch.
 class ModelMapping(Bunch):
     def __init__(self, model_modules, engine):
         self.engine = engine
-        self._SessionLocal = sessionmaker(autoflush=False, autocommit=False)
+        self._SessionLocal = sessionmaker(autoflush=False, autocommit=False, future=True)
         versioned_session(self._SessionLocal)
         context = scoped_session(self._SessionLocal, scopefunc=self.request_scopefunc)
         # For backward compatibility with "context.current"
         # deprecated?
         context.current = context
         self.session = context
         self.scoped_registry = context.registry
@@ -176,7 +182,26 @@
 def versioned_session(session):
     @event.listens_for(session, "before_flush")
     def before_flush(session, flush_context, instances):
         for obj in versioned_objects(session.dirty):
             obj.__create_version__(session)
         for obj in versioned_objects(session.deleted):
             obj.__create_version__(session, deleted=True)
+
+
+def ensure_object_added_to_session(object_to_add, *, object_in_session=None, session=None) -> bool:
+    """
+    This function is intended as a safeguard to mimic pre-SQLAlchemy 2.0 behavior.
+    `object_to_add` was implicitly merged into a Session prior to SQLAlchemy 2.0, which was indicated
+    by `RemovedIn20Warning` warnings logged while running Galaxy's tests. (See https://github.com/galaxyproject/galaxy/issues/12541)
+    As part of the upgrade to 2.0, the `cascade_backrefs=False` argument was added to the relevant relationships that turned off this behavior.
+    This function is called from the code that triggered these warnings, thus emulating the cascading behavior.
+    The intention is to remove all such calls, as well as this function definition, after the move to SQLAlchemy 2.0.
+    # Ref: https://docs.sqlalchemy.org/en/14/changelog/migration_14.html#cascade-backrefs-behavior-deprecated-for-removal-in-2-0
+    """
+    if session:
+        session.add(object_to_add)
+        return True
+    if object_in_session and object_session(object_in_session):
+        object_session(object_in_session).add(object_to_add)
+        return True
+    return False
```

### Comparing `galaxy-data-23.2.1/galaxy/model/custom_types.py` & `galaxy-data-24.0.0/galaxy/model/custom_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,14 +113,16 @@
         return copy.deepcopy(value)
 
     def compare_values(self, x, y):
         return x == y
 
 
 class DoubleEncodedJsonType(JSONType):
+    cache_ok = True
+
     def process_result_value(self, value, dialect):
         value = super().process_result_value(value, dialect)
         if isinstance(value, str):
             try:
                 return json.loads(value)
             except ValueError:
                 return value
@@ -337,19 +339,20 @@
     """
 
     cache_ok = True
 
     def process_bind_param(self, value, dialect):
         if value is not None:
             if MAX_METADATA_VALUE_SIZE is not None:
-                for k, v in list(value.items()):
-                    sz = total_size(v)
-                    if sz > MAX_METADATA_VALUE_SIZE:
-                        del value[k]
-                        log.warning(f"Refusing to bind metadata key {k} due to size ({sz})")
+                if hasattr(value, "items"):
+                    for k, v in list(value.items()):
+                        sz = total_size(v)
+                        if sz > MAX_METADATA_VALUE_SIZE:
+                            del value[k]
+                            log.warning(f"Refusing to bind metadata key {k} due to size ({sz})")
             value = json_encoder.encode(value).encode()
         return value
 
     def process_result_value(self, value, dialect):
         if value is None:
             return None
         ret = None
```

### Comparing `galaxy-data-23.2.1/galaxy/model/database_heartbeat.py` & `galaxy-data-24.0.0/galaxy/model/database_heartbeat.py`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/model/database_object_names.py` & `galaxy-data-24.0.0/galaxy/model/database_object_names.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Naming convention and helper functions for generating names of database
 constraints and indexes.
 """
+
 from typing import (
     List,
     Union,
 )
 
 from galaxy.util import listify
```

### Comparing `galaxy-data-23.2.1/galaxy/model/database_utils.py` & `galaxy-data-24.0.0/galaxy/model/database_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from sqlalchemy import (
     create_engine,
     select,
     update,
 )
 from sqlalchemy.engine import Engine
 from sqlalchemy.engine.url import make_url
+from sqlalchemy.orm import object_session
 from sqlalchemy.sql.compiler import IdentifierPreparer
 from sqlalchemy.sql.expression import (
     ClauseElement,
     text,
 )
 
 from galaxy.exceptions import ConfigurationError
@@ -40,15 +41,15 @@
     """
     dbm = DatabaseManager.make_manager(db_url, database)
     dbm.create(encoding, template)
 
 
 @contextmanager
 def sqlalchemy_engine(url):
-    engine = create_engine(url)
+    engine = create_engine(url, future=True)
     try:
         yield engine
     finally:
         engine.dispose()
 
 
 class DatabaseManager:
@@ -83,15 +84,15 @@
                 return bool(conn.scalar(stmt))
 
     def create(self, encoding, template):
         with sqlalchemy_engine(self.url) as engine:
             preparer = IdentifierPreparer(engine.dialect)
             template = template or "template1"
             database, template = preparer.quote(self.database), preparer.quote(template)
-            stmt = f"CREATE DATABASE {database} ENCODING '{encoding}' TEMPLATE {template}"
+            stmt = text(f"CREATE DATABASE {database} ENCODING '{encoding}' TEMPLATE {template}")
             with engine.connect().execution_options(isolation_level="AUTOCOMMIT") as conn:
                 conn.execute(stmt)
 
 
 class SqliteDatabaseManager(DatabaseManager):
     def _handle_no_database(self):
         self.database = self.url.database  # use database from db_url
@@ -126,15 +127,15 @@
                 return bool(conn.scalar(stmt))
 
     def create(self, encoding, *arg):
         # Ignore any args (template)
         with sqlalchemy_engine(self.url) as engine:
             preparer = IdentifierPreparer(engine.dialect)
             database = preparer.quote(self.database)
-            stmt = f"CREATE DATABASE {database} CHARACTER SET = '{encoding}'"
+            stmt = text(f"CREATE DATABASE {database} CHARACTER SET = '{encoding}'")
             with engine.connect().execution_options(isolation_level="AUTOCOMMIT") as conn:
                 conn.execute(stmt)
 
 
 def is_one_database(db1_url: str, db2_url: Optional[str]):
     """
     Check if the arguments refer to one database. This will be true
@@ -171,7 +172,26 @@
             return True
     except Exception:
         return False
 
 
 def is_postgres(url: DbUrl) -> bool:
     return url.startswith("postgres")
+
+
+def ensure_object_added_to_session(object_to_add, *, object_in_session=None, session=None) -> bool:
+    """
+    This function is intended as a safeguard to mimic pre-SQLAlchemy 2.0 behavior.
+    `object_to_add` was implicitly merged into a Session prior to SQLAlchemy 2.0, which was indicated
+    by `RemovedIn20Warning` warnings logged while running Galaxy's tests. (See https://github.com/galaxyproject/galaxy/issues/12541)
+    As part of the upgrade to 2.0, the `cascade_backrefs=False` argument was added to the relevant relationships that turned off this behavior.
+    This function is called from the code that triggered these warnings, thus emulating the cascading behavior.
+    The intention is to remove all such calls, as well as this function definition, after the move to SQLAlchemy 2.0.
+    # Ref: https://docs.sqlalchemy.org/en/14/changelog/migration_14.html#cascade-backrefs-behavior-deprecated-for-removal-in-2-0
+    """
+    if session:
+        session.add(object_to_add)
+        return True
+    if object_in_session and object_session(object_in_session):
+        object_session(object_in_session).add(object_to_add)
+        return True
+    return False
```

### Comparing `galaxy-data-23.2.1/galaxy/model/dataset_collections/builder.py` & `galaxy-data-24.0.0/galaxy/model/dataset_collections/builder.py`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/model/dataset_collections/matching.py` & `galaxy-data-24.0.0/galaxy/model/dataset_collections/matching.py`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/model/dataset_collections/registry.py` & `galaxy-data-24.0.0/galaxy/model/dataset_collections/registry.py`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/model/dataset_collections/structure.py` & `galaxy-data-24.0.0/galaxy/model/dataset_collections/structure.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """ Module for reasoning about structure of and matching hierarchical collections of data.
 """
+
 import logging
 
 log = logging.getLogger(__name__)
 
 
 class Leaf:
     children_known = True
```

### Comparing `galaxy-data-23.2.1/galaxy/model/dataset_collections/subcollections.py` & `galaxy-data-24.0.0/galaxy/model/dataset_collections/subcollections.py`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/model/dataset_collections/type_description.py` & `galaxy-data-24.0.0/galaxy/model/dataset_collections/type_description.py`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/model/dataset_collections/types/__init__.py` & `galaxy-data-24.0.0/galaxy/model/dataset_collections/types/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/model/dataset_collections/types/list.py` & `galaxy-data-24.0.0/galaxy/model/dataset_collections/types/list.py`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/model/dataset_collections/types/paired.py` & `galaxy-data-24.0.0/galaxy/model/dataset_collections/types/paired.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,23 +15,21 @@
 
     collection_type = "paired"
 
     def __init__(self):
         pass
 
     def generate_elements(self, elements):
-        forward_dataset = elements.get(FORWARD_IDENTIFIER)
-        reverse_dataset = elements.get(REVERSE_IDENTIFIER)
-        if forward_dataset:
+        if forward_dataset := elements.get(FORWARD_IDENTIFIER):
             left_association = DatasetCollectionElement(
                 element=forward_dataset,
                 element_identifier=FORWARD_IDENTIFIER,
             )
             yield left_association
-        if reverse_dataset:
+        if reverse_dataset := elements.get(REVERSE_IDENTIFIER):
             right_association = DatasetCollectionElement(
                 element=reverse_dataset,
                 element_identifier=REVERSE_IDENTIFIER,
             )
             yield right_association
 
     def prototype_elements(self):
```

### Comparing `galaxy-data-23.2.1/galaxy/model/deferred.py` & `galaxy-data-24.0.0/galaxy/model/deferred.py`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/model/index_filter_util.py` & `galaxy-data-24.0.0/galaxy/model/index_filter_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Utility functions used to adapt galaxy.util.search to Galaxy model index queries."""
+
 from typing import (
     List,
     Union,
 )
 
 from sqlalchemy import (
     and_,
```

### Comparing `galaxy-data-23.2.1/galaxy/model/item_attrs.py` & `galaxy-data-24.0.0/galaxy/model/item_attrs.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,16 +92,15 @@
     def get_item_annotation_obj(self, db_session, user, item):
         return get_item_annotation_obj(db_session, user, item)
 
     def add_item_annotation(self, db_session, user, item, annotation):
         return add_item_annotation(db_session, user, item, annotation)
 
     def delete_item_annotation(self, db_session, user, item):
-        annotation_assoc = get_item_annotation_obj(db_session, user, item)
-        if annotation_assoc:
+        if annotation_assoc := get_item_annotation_obj(db_session, user, item):
             db_session.delete(annotation_assoc)
             with transaction(db_session):
                 db_session.commit()
 
     def copy_item_annotation(self, db_session, source_user, source_item, target_user, target_item):
         """Copy an annotation from a user/item source to a user/item target."""
         if source_user and target_user:
```

### Comparing `galaxy-data-23.2.1/galaxy/model/mapping.py` & `galaxy-data-24.0.0/galaxy/model/mapping.py`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/model/metadata.py` & `galaxy-data-24.0.0/galaxy/model/metadata.py`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/model/migrations/__init__.py` & `galaxy-data-24.0.0/galaxy/model/migrations/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,18 +120,18 @@
 def verify_databases_via_script(
     gxy_config: DatabaseConfig,
     tsi_config: DatabaseConfig,
     is_auto_migrate: bool = False,
 ) -> None:
     # This function serves a use case when an engine has not been created yet
     # (e.g. when called from a script).
-    gxy_engine = create_engine(gxy_config.url)
+    gxy_engine = create_engine(gxy_config.url, future=True)
     tsi_engine = None
     if tsi_config.url and tsi_config.url != gxy_config.url:
-        tsi_engine = create_engine(tsi_config.url)
+        tsi_engine = create_engine(tsi_config.url, future=True)
 
     verify_databases(
         gxy_engine,
         gxy_config.template,
         gxy_config.encoding,
         tsi_engine,
         tsi_config.template,
```

### Comparing `galaxy-data-23.2.1/galaxy/model/migrations/alembic/env.py` & `galaxy-data-24.0.0/galaxy/model/migrations/alembic/env.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,15 +112,15 @@
         dialect_opts={"paramstyle": "named"},
     )
     with context.begin_transaction():
         context.run_migrations()
 
 
 def _configure_and_run_migrations_online(url) -> None:
-    engine = create_engine(url)
+    engine = create_engine(url, future=True)
     with engine.connect() as connection:
         context.configure(connection=connection, target_metadata=target_metadata)
         with context.begin_transaction():
             context.run_migrations()
     engine.dispose()
```

### Comparing `galaxy-data-23.2.1/galaxy/model/migrations/alembic/versions_gxy/186d4835587b_drop_job_state_history_update_time_.py` & `galaxy-data-24.0.0/galaxy/model/migrations/alembic/versions_gxy/186d4835587b_drop_job_state_history_update_time_.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """drop job_state_history.update_time column
 
 Revision ID: 186d4835587b
 Revises: 6a67bf27e6a6
 Create Date: 2022-06-01 17:50:22.629894
 
 """
+
 from sqlalchemy import (
     Column,
     DateTime,
 )
 
 from galaxy.model.migrations.util import (
     add_column,
```

### Comparing `galaxy-data-23.2.1/galaxy/model/migrations/alembic/versions_gxy/2d749563e1fe_add_notification_system_tables.py` & `galaxy-data-24.0.0/galaxy/model/migrations/alembic/versions_gxy/2d749563e1fe_add_notification_system_tables.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Add Notification System tables
 
 Revision ID: 2d749563e1fe
 Revises: b855b714e8b8
 Create Date: 2023-03-02 15:16:36.737075
 
 """
+
 import sqlalchemy as sa
 
 from galaxy.model.custom_types import JSONType
 from galaxy.model.migrations.util import (
     create_table,
     drop_table,
     transaction,
```

### Comparing `galaxy-data-23.2.1/galaxy/model/migrations/alembic/versions_gxy/3100452fa030_add_workflow_invocation_message_table.py` & `galaxy-data-24.0.0/galaxy/model/migrations/alembic/versions_gxy/3100452fa030_add_workflow_invocation_message_table.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Add reason column on invocation table
 
 Revision ID: 3100452fa030
 Revises: 518c8438a91b
 Create Date: 2023-01-13 16:13:09.578391
 
 """
+
 from sqlalchemy import (
     Column,
     ForeignKey,
     Integer,
     String,
 )
```

### Comparing `galaxy-data-23.2.1/galaxy/model/migrations/alembic/versions_gxy/3356bc2ecfc4_drop_view.py` & `galaxy-data-24.0.0/galaxy/model/migrations/alembic/versions_gxy/3356bc2ecfc4_drop_view.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """drop view
 
 Revision ID: 3356bc2ecfc4
 Revises: 460d0ecd1dd8
 Create Date: 2023-04-10 15:06:01.037416
 
 """
+
 from alembic import op
 
 # revision identifiers, used by Alembic.
 revision = "3356bc2ecfc4"
 down_revision = "460d0ecd1dd8"
 branch_labels = None
 depends_on = None
```

### Comparing `galaxy-data-23.2.1/galaxy/model/migrations/alembic/versions_gxy/3a2914d703ca_add_index_wf_r_s_s__workflow_invocation_.py` & `galaxy-data-24.0.0/galaxy/model/migrations/alembic/versions_gxy/3a2914d703ca_add_index_wf_r_s_s__workflow_invocation_.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """add index workflow_request_step_states__workflow_invocation_id
 
 Revision ID: 3a2914d703ca
 Revises: c39f1de47a04
 Create Date: 2023-03-07 15:06:55.682273
 
 """
+
 from galaxy.model.database_object_names import build_index_name
 from galaxy.model.migrations.util import (
     create_index,
     drop_index,
 )
 
 # revision identifiers, used by Alembic.
```

### Comparing `galaxy-data-23.2.1/galaxy/model/migrations/alembic/versions_gxy/460d0ecd1dd8_.py` & `galaxy-data-24.0.0/galaxy/model/migrations/alembic/versions_gxy/460d0ecd1dd8_.py`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/model/migrations/alembic/versions_gxy/518c8438a91b_add_when_expression_column.py` & `galaxy-data-24.0.0/galaxy/model/migrations/alembic/versions_gxy/518c8438a91b_add_when_expression_column.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Add when_expression column
 
 Revision ID: 518c8438a91b
 Revises: 59e024ceaca1
 Create Date: 2022-10-24 16:43:39.565871
 
 """
+
 from sqlalchemy import Column
 
 from galaxy.model.custom_types import JSONType
 from galaxy.model.migrations.util import (
     add_column,
     drop_column,
 )
```

### Comparing `galaxy-data-23.2.1/galaxy/model/migrations/alembic/versions_gxy/59e024ceaca1_add_export_association_table.py` & `galaxy-data-24.0.0/galaxy/model/migrations/alembic/versions_gxy/59e024ceaca1_add_export_association_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """add export association table
 
 Revision ID: 59e024ceaca1
 Revises: e0e3bb173ee6
 Create Date: 2022-10-12 18:02:34.659770
 
 """
+
 from sqlalchemy import (
     Column,
     DateTime,
     Integer,
 )
 
 from galaxy.model.custom_types import (
```

### Comparing `galaxy-data-23.2.1/galaxy/model/migrations/alembic/versions_gxy/6a67bf27e6a6_deferred_data_tables.py` & `galaxy-data-24.0.0/galaxy/model/migrations/alembic/versions_gxy/6a67bf27e6a6_deferred_data_tables.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """deferred data tables
 
 Revision ID: 6a67bf27e6a6
 Revises: b182f655505f
 Create Date: 2022-03-14 12:17:55.313830
 
 """
+
 from sqlalchemy import (
     Boolean,
     Column,
 )
 
 from galaxy.model.migrations.util import (
     add_column,
```

### Comparing `galaxy-data-23.2.1/galaxy/model/migrations/alembic/versions_gxy/8a19186a6ee7_add_columns_to_interactivetool_entry_point.py` & `galaxy-data-24.0.0/galaxy/model/migrations/alembic/versions_gxy/8a19186a6ee7_add_columns_to_interactivetool_entry_point.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """add label, requires_path_in_url and requires_path_in_header_named columns to interactivetool_entry_point
 
 Revision ID: 8a19186a6ee7
 Revises: ddbdbc40bdc1
 Create Date: 2023-11-15 12:53:32.888292
 
 """
+
 from sqlalchemy import (
     Boolean,
     Column,
     Text,
 )
 
 from galaxy.model.migrations.util import (
```

### Comparing `galaxy-data-23.2.1/galaxy/model/migrations/alembic/versions_gxy/9540a051226e_preferred_object_store_ids.py` & `galaxy-data-24.0.0/galaxy/model/migrations/alembic/versions_gxy/9540a051226e_preferred_object_store_ids.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """preferred_object_store_ids
 
 Revision ID: 9540a051226e
 Revises: d0583094c8cd
 Create Date: 2022-06-10 10:38:25.212102
 
 """
+
 from sqlalchemy import (
     Column,
     String,
 )
 
 from galaxy.model.custom_types import JSONType
 from galaxy.model.migrations.util import (
```

### Comparing `galaxy-data-23.2.1/galaxy/model/migrations/alembic/versions_gxy/987ce9839ecb_create_celery_user_rate_limit_table.py` & `galaxy-data-24.0.0/galaxy/model/migrations/alembic/versions_gxy/987ce9839ecb_create_celery_user_rate_limit_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """create celery_user_rate_limit_table
 
 Revision ID: 987ce9839ecb
 Revises: b855b714e8b8
 Create Date: 2023-05-17 15:08:28.467938
 
 """
+
 import sqlalchemy as sa
 
 from galaxy.model.migrations.util import (
     create_table,
     drop_table,
 )
```

### Comparing `galaxy-data-23.2.1/galaxy/model/migrations/alembic/versions_gxy/b182f655505f_add_workflow_source_metadata_column.py` & `galaxy-data-24.0.0/galaxy/model/migrations/alembic/versions_gxy/b182f655505f_add_workflow_source_metadata_column.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """add workflow.source_metadata column
 
 Revision ID: b182f655505f
 Revises: e7b6dcb09efd
 Create Date: 2022-03-14 12:56:57.067748
 
 """
+
 from sqlalchemy import Column
 
 from galaxy.model.custom_types import JSONType
 from galaxy.model.migrations.util import (
     add_column,
     drop_column,
 )
```

### Comparing `galaxy-data-23.2.1/galaxy/model/migrations/alembic/versions_gxy/b855b714e8b8_make_api_keys_deleted_non_nullable.py` & `galaxy-data-24.0.0/galaxy/model/migrations/alembic/versions_gxy/b855b714e8b8_make_api_keys_deleted_non_nullable.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """make api_keys deleted non nullable
 
 Revision ID: b855b714e8b8
 Revises: 3356bc2ecfc4
 Create Date: 2023-04-19 18:41:13.500332
 
 """
+
 import sqlalchemy as sa
 from alembic import op
 
 from galaxy.model.migrations.util import (
     alter_column,
     transaction,
 )
```

### Comparing `galaxy-data-23.2.1/galaxy/model/migrations/alembic/versions_gxy/c39f1de47a04_add_skipped_state_to_collection_job_.py` & `galaxy-data-24.0.0/galaxy/model/migrations/alembic/versions_gxy/c39f1de47a04_add_skipped_state_to_collection_job_.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Add skipped state to collection_job_state_summary_view
 
 Revision ID: c39f1de47a04
 Revises: 3100452fa030
 Create Date: 2023-01-16 11:53:59.783836
 
 """
+
 from alembic import op
 
 from galaxy.model.migrations.util import transaction
 
 # revision identifiers, used by Alembic.
 revision = "c39f1de47a04"
 down_revision = "3100452fa030"
```

### Comparing `galaxy-data-23.2.1/galaxy/model/migrations/alembic/versions_gxy/caa7742f7bca_add_index_wf_r_i_p__workflow_invocation_.py` & `galaxy-data-24.0.0/galaxy/model/migrations/alembic/versions_gxy/caa7742f7bca_add_index_wf_r_i_p__workflow_invocation_.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """add index workflow_request_input_parameters__workflow_invocation_id
 
 Revision ID: caa7742f7bca
 Revises: 3a2914d703ca
 Create Date: 2023-03-07 15:10:44.943542
 
 """
+
 from galaxy.model.database_object_names import build_index_name
 from galaxy.model.migrations.util import (
     create_index,
     drop_index,
 )
 
 # revision identifiers, used by Alembic.
```

### Comparing `galaxy-data-23.2.1/galaxy/model/migrations/alembic/versions_gxy/d0583094c8cd_add_quota_source_labels.py` & `galaxy-data-24.0.0/galaxy/model/migrations/alembic/versions_gxy/d0583094c8cd_add_quota_source_labels.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """add quota source labels
 
 Revision ID: d0583094c8cd
 Revises: c39f1de47a04
 Create Date: 2022-06-09 12:24:44.329038
 
 """
+
 from sqlalchemy import (
     Column,
     ForeignKey,
     Integer,
     Numeric,
     String,
 )
```

### Comparing `galaxy-data-23.2.1/galaxy/model/migrations/alembic/versions_gxy/ddbdbc40bdc1_add_workflow_comment_table.py` & `galaxy-data-24.0.0/galaxy/model/migrations/alembic/versions_gxy/ddbdbc40bdc1_add_workflow_comment_table.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """add workflow_comment table
 Revision ID: ddbdbc40bdc1
 Revises: 92fb564c7095
 Create Date: 2023-08-14 13:41:59.442243
 """
+
 import sqlalchemy as sa
 
 from galaxy.model.custom_types import (
     JSONType,
     MutableJSONType,
 )
 from galaxy.model.migrations.util import (
```

### Comparing `galaxy-data-23.2.1/galaxy/model/migrations/alembic/versions_gxy/e0561d5fc8c7_add_archived_columns_to_history.py` & `galaxy-data-24.0.0/galaxy/model/migrations/alembic/versions_gxy/e0561d5fc8c7_add_archived_columns_to_history.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """add archived columns to history
 
 Revision ID: e0561d5fc8c7
 Revises: 2d749563e1fe
 Create Date: 2023-05-03 11:57:58.710098
 
 """
+
 import sqlalchemy as sa
 
 from galaxy.model.database_object_names import (
     build_foreign_key_name,
     build_index_name,
 )
 from galaxy.model.migrations.util import (
```

### Comparing `galaxy-data-23.2.1/galaxy/model/migrations/alembic/versions_gxy/e0e3bb173ee6_add_column_deleted_to_api_keys.py` & `galaxy-data-24.0.0/galaxy/model/migrations/alembic/versions_gxy/e0e3bb173ee6_add_column_deleted_to_api_keys.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """add column deleted to API keys
 
 Revision ID: e0e3bb173ee6
 Revises: 186d4835587b
 Create Date: 2022-09-27 14:09:05.890227
 
 """
+
 from sqlalchemy import (
     Boolean,
     Column,
 )
 
 from galaxy.model.database_object_names import build_index_name
 from galaxy.model.migrations.util import (
```

### Comparing `galaxy-data-23.2.1/galaxy/model/migrations/alembic/versions_gxy/e93c5d0b47a9_alter_column_external_user_id.py` & `galaxy-data-24.0.0/galaxy/model/migrations/alembic/versions_gxy/e93c5d0b47a9_alter_column_external_user_id.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """alter column CustosAuthnzToken.external_user_id to increase length
 
 Revision ID: e93c5d0b47a9
 Revises: e0561d5fc8c7
 Create Date: 2023-10-08 12:11:02.024669
 
 """
+
 import sqlalchemy as sa
 
 from galaxy.model.migrations.util import alter_column
 
 # revision identifiers, used by Alembic.
 revision = "e93c5d0b47a9"
 down_revision = "e0561d5fc8c7"
```

### Comparing `galaxy-data-23.2.1/galaxy/model/migrations/alembic.ini` & `galaxy-data-24.0.0/galaxy/model/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/model/migrations/base.py` & `galaxy-data-24.0.0/galaxy/model/migrations/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Shared code for galaxy and tool shed migrations.
 """
+
 import abc
 import logging
 import os
 import sys
 import urllib.parse
 from argparse import (
     ArgumentParser,
@@ -45,16 +46,15 @@
 
 class BaseParserBuilder(abc.ABC):
     """
     Assembler object that simplifies the construction of an argument parser for database migration scripts.
     """
 
     @abc.abstractmethod
-    def _get_command_object(self):
-        ...
+    def _get_command_object(self): ...
 
     def __init__(self, parser, subcommand_required=True):
         self._cmd = self._get_command_object()
         self.parser = parser
         self.subparsers = parser.add_subparsers(required=subcommand_required)
         self._init_arg_parsers()
 
@@ -177,20 +177,18 @@
         return parser
 
 
 class BaseDbScript(abc.ABC):
     """Facade for common database schema migration operations."""
 
     @abc.abstractmethod
-    def _set_dburl(self, config_file: Optional[str] = None) -> None:
-        ...
+    def _set_dburl(self, config_file: Optional[str] = None) -> None: ...
 
     @abc.abstractmethod
-    def _upgrade_to_head(self, is_sql_mode: bool):
-        ...
+    def _upgrade_to_head(self, is_sql_mode: bool): ...
 
     def __init__(self, config_file: Optional[str] = None) -> None:
         self.alembic_config = self._get_alembic_cfg()
         self._set_dburl(config_file)
 
     def revision(self, args: Namespace) -> None:
         head = self._add_branch_label("head")
@@ -255,20 +253,18 @@
     def _process_repair_arg(self, args: Namespace) -> None:
         if "repair" in args and args.repair:
             self.alembic_config.set_main_option("repair", "1")
 
 
 class BaseCommand(abc.ABC):
     @abc.abstractmethod
-    def init(self, args: Namespace) -> None:
-        ...
+    def init(self, args: Namespace) -> None: ...
 
     @abc.abstractmethod
-    def _get_dbscript(self, config_file: str) -> BaseDbScript:
-        ...
+    def _get_dbscript(self, config_file: str) -> BaseDbScript: ...
 
     def upgrade(self, args: Namespace) -> None:
         self._exec_command("upgrade", args)
 
     def downgrade(self, args: Namespace) -> None:
         self._exec_command("downgrade", args)
 
@@ -303,16 +299,15 @@
 
 class BaseAlembicManager(abc.ABC):
     """
     Alembic operations on one database.
     """
 
     @abc.abstractmethod
-    def _get_alembic_root(self):
-        ...
+    def _get_alembic_root(self): ...
 
     @staticmethod
     def is_at_revision(engine: Engine, revision: Union[str, Iterable[str]]) -> bool:
         """
         True if revision is a subset of the set of version heads stored in the database.
         """
         revision = listify(revision)
@@ -430,15 +425,15 @@
 
 def get_url_string(engine: Engine) -> str:
     db_url = engine.url.render_as_string(hide_password=False)
     return urllib.parse.unquote(db_url)
 
 
 def load_metadata(metadata: MetaData, engine: Engine) -> None:
-    with engine.connect() as conn:
+    with engine.begin() as conn:
         metadata.create_all(bind=conn)
 
 
 def listify(data: Union[str, Iterable[str]]) -> Iterable[str]:
     if not isinstance(data, (list, tuple)):
         return [cast(str, data)]
     return data
```

### Comparing `galaxy-data-23.2.1/galaxy/model/migrations/dbscript.py` & `galaxy-data-24.0.0/galaxy/model/migrations/dbscript.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,14 +36,16 @@
     "22.05": "186d4835587b",
     "release_23.0": "caa7742f7bca",
     "23.0": "caa7742f7bca",
     "release_23.1": "e93c5d0b47a9",
     "23.1": "e93c5d0b47a9",
     "release_23.2": "8a19186a6ee7",
     "23.2": "8a19186a6ee7",
+    "release_24.0": "55f02fd8ab6c",
+    "24.0": "55f02fd8ab6c",
 }
 
 
 class ParserBuilder(BaseParserBuilder):
     def _get_command_object(self):
         return Command()
```

### Comparing `galaxy-data-23.2.1/galaxy/model/migrations/exceptions.py` & `galaxy-data-24.0.0/galaxy/model/migrations/exceptions.py`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/model/migrations/scripts.py` & `galaxy-data-24.0.0/galaxy/model/migrations/scripts.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
     *NOTE: this function cannot determine whether a database has been properly
     initialized; it can only tell when a database has *not* been initialized.
     """
     if not database_exists(db_url):
         raise DatabaseDoesNotExistError(db_url)
 
-    engine = create_engine(db_url)
+    engine = create_engine(db_url, future=True)
     try:
         db_state = DatabaseStateCache(engine=engine)
         if db_state.is_database_empty() or db_state.contains_only_kombu_tables():
             raise DatabaseNotInitializedError(db_url)
     finally:
         engine.dispose()
 
@@ -157,15 +157,15 @@
         Get the head revision for the gxy branch from the galaxy database. If there
         is no alembic_version table, get the sqlalchemy migrate version. Raise error
         if that version is not the latest.
         (previously referred to as "database version")
         """
         db_url = gxy_db_url or self.gxy_db_url
         try:
-            engine = create_engine(db_url)
+            engine = create_engine(db_url, future=True)
             version = self._get_gxy_alembic_db_version(engine)
             if not version:
                 version = self._get_gxy_sam_db_version(engine)
                 if version is None:
                     raise NoVersionTableError(GXY)
                 elif version != SQLALCHEMYMIGRATE_LAST_VERSION_GXY:
                     raise IncorrectSAMigrateVersionError(GXY, SQLALCHEMYMIGRATE_LAST_VERSION_GXY)
@@ -193,15 +193,15 @@
 
     def _rename_arg(self, argv, old_name, new_name) -> None:
         pos = argv.index(old_name)
         argv[pos] = new_name
 
     def _upgrade(self, db_url, model):
         try:
-            engine = create_engine(db_url)
+            engine = create_engine(db_url, future=True)
             am = get_alembic_manager(engine)
             am.upgrade(model)
         finally:
             engine.dispose()
 
     def _set_db_urls(self):
         self.rename_config_argument(sys.argv)
```

### Comparing `galaxy-data-23.2.1/galaxy/model/migrations/util.py` & `galaxy-data-24.0.0/galaxy/model/migrations/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,24 +31,21 @@
             if self.pre_execute_check():
                 return self.execute()
             else:
                 self.log_check_not_passed()
                 return None
 
     @abstractmethod
-    def execute(self) -> Optional[Any]:
-        ...
+    def execute(self) -> Optional[Any]: ...
 
     @abstractmethod
-    def pre_execute_check(self) -> bool:
-        ...
+    def pre_execute_check(self) -> bool: ...
 
     @abstractmethod
-    def log_check_not_passed(self) -> None:
-        ...
+    def log_check_not_passed(self) -> None: ...
 
     def _is_repair_mode(self) -> bool:
         """`--repair` option has been passed to the command."""
         return bool(context.config.get_main_option("repair"))
 
     def _log_object_exists_message(self, object_name: str) -> None:
         log.info(f"{object_name} already exists. Skipping revision.")
@@ -78,20 +75,18 @@
         if _is_sqlite():
             with legacy_alter_table(), op.batch_alter_table(self.table_name) as batch_op:
                 return self.batch_execute(batch_op)
         else:
             return self.non_batch_execute()  # use regular op context for non-sqlite db
 
     @abstractmethod
-    def batch_execute(self, batch_op) -> Optional[Any]:
-        ...
+    def batch_execute(self, batch_op) -> Optional[Any]: ...
 
     @abstractmethod
-    def non_batch_execute(self) -> Optional[Any]:
-        ...
+    def non_batch_execute(self) -> Optional[Any]: ...
 
 
 class CreateTable(DDLOperation):
     """Wraps alembic's create_table directive."""
 
     def __init__(self, table_name: str, *columns: sa.schema.SchemaItem) -> None:
         self.table_name = table_name
```

### Comparing `galaxy-data-23.2.1/galaxy/model/none_like.py` & `galaxy-data-24.0.0/galaxy/model/none_like.py`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/model/orm/engine_factory.py` & `galaxy-data-24.0.0/galaxy/model/orm/engine_factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,15 @@
                     if thread_local_log.log:
                         log.debug(f"Request query: {total:f}(s)\n{statement}\nParameters: {parameters}")
                 except AttributeError:
                     pass
 
     engine_options = engine_options or {}
     engine_options = set_sqlite_connect_args(engine_options, url)
-    engine = create_engine(url, **engine_options)
+    engine = create_engine(url, **engine_options, future=True)
 
     # Prevent sharing connection across fork: https://docs.sqlalchemy.org/en/14/core/pooling.html#using-connection-pools-with-multiprocessing-or-os-fork
     register_after_fork(engine, lambda e: e.dispose())
 
     @event.listens_for(engine, "connect")
     def connect(dbapi_connection, connection_record):
         connection_record.info["pid"] = os.getpid()
```

### Comparing `galaxy-data-23.2.1/galaxy/model/orm/scripts.py` & `galaxy-data-24.0.0/galaxy/model/orm/scripts.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Code to support database helper scripts (create_toolshed_db.py, migrate_toolshed_db.py, etc...).
 """
+
 import argparse
 import logging
 import os
 import sys
 
 import alembic.config
```

### Comparing `galaxy-data-23.2.1/galaxy/model/orm/util.py` & `galaxy-data-24.0.0/galaxy/model/orm/util.py`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/model/scoped_session.py` & `galaxy-data-24.0.0/galaxy/model/scoped_session.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 These classes are used for registering different scoped_session objects with
 the DI framework. This type distinction is necessary because we need to store
 scoped_session objects that produce sessions that may have different binds
 (i.e., if the tool_shed_install model uses a different database).
 """
+
 from sqlalchemy.orm import scoped_session
 
 
 class galaxy_scoped_session(scoped_session):
     """scoped_session used for galaxy model."""
```

### Comparing `galaxy-data-23.2.1/galaxy/model/security.py` & `galaxy-data-24.0.0/galaxy/model/security.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     false,
     func,
     not_,
     or_,
     select,
 )
 from sqlalchemy.orm import joinedload
+from sqlalchemy.sql import text
 
 import galaxy.model
 from galaxy.model import (
     Dataset,
     DatasetPermissions,
     Group,
     GroupRoleAssociation,
@@ -630,14 +631,32 @@
 
     def can_modify_library_item(self, roles, item):
         return self.allow_action(roles, self.permitted_actions.LIBRARY_MODIFY, item)
 
     def can_manage_library_item(self, roles, item):
         return self.allow_action(roles, self.permitted_actions.LIBRARY_MANAGE, item)
 
+    def can_change_object_store_id(self, user, dataset):
+        # prevent update if dataset shared with anyone but the current user
+        # private object stores would prevent this but if something has been
+        # kept private in a sharable object store still allow the swap
+        if dataset.library_associations:
+            return False
+        else:
+            query = text(
+                """
+SELECT COUNT(*)
+FROM history
+INNER JOIN
+    history_dataset_association on history_dataset_association.history_id = history.id
+WHERE history.user_id != :user_id and history_dataset_association.dataset_id = :dataset_id
+"""
+            ).bindparams(dataset_id=dataset.id, user_id=user.id if user else None)
+            return self.sa_session.scalars(query).first() == 0
+
     def get_item_actions(self, action, item):
         # item must be one of: Dataset, Library, LibraryFolder, LibraryDataset, LibraryDatasetDatasetAssociation
         # SM: Accessing item.actions emits a query to Library_Dataset_Permissions
         # if the item is a LibraryDataset:
         # TODO: Pass in the item's actions - the item isn't needed
         return [permission for permission in item.actions if permission.action == action.action]
 
@@ -742,20 +761,24 @@
                 self.user_set_default_permissions(user, history=True, dataset=True)
 
     def create_private_user_role(self, user):
         user.attempt_create_private_role()
         return self.get_private_user_role(user)
 
     def get_private_user_role(self, user, auto_create=False):
-        stmt = select(Role).where(
-            and_(
-                UserRoleAssociation.user_id == user.id,
-                Role.id == UserRoleAssociation.role_id,
-                Role.type == Role.types.PRIVATE,
+        stmt = (
+            select(Role)
+            .where(
+                and_(
+                    UserRoleAssociation.user_id == user.id,
+                    Role.id == UserRoleAssociation.role_id,
+                    Role.type == Role.types.PRIVATE,
+                )
             )
+            .distinct()
         )
         role = self.sa_session.execute(stmt).scalar_one_or_none()
         if not role:
             if auto_create:
                 return self.create_private_user_role(user)
             else:
                 return None
```

### Comparing `galaxy-data-23.2.1/galaxy/model/store/__init__.py` & `galaxy-data-24.0.0/galaxy/model/store/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,18 @@
     Type,
     TYPE_CHECKING,
     Union,
 )
 
 from bdbag import bdbag_api as bdb
 from boltons.iterutils import remap
+from pydantic import (
+    BaseModel,
+    ConfigDict,
+)
 from rocrate.model.computationalworkflow import (
     ComputationalWorkflow,
     WorkflowDescription,
 )
 from rocrate.rocrate import ROCrate
 from sqlalchemy import select
 from sqlalchemy.orm import joinedload
@@ -52,15 +56,18 @@
     RequestParameterInvalidException,
 )
 from galaxy.files import (
     ConfiguredFileSources,
     ProvidesUserFileSourcesUserContext,
 )
 from galaxy.files.uris import stream_url_to_file
-from galaxy.model.base import transaction
+from galaxy.model.base import (
+    ensure_object_added_to_session,
+    transaction,
+)
 from galaxy.model.mapping import GalaxyModelMapping
 from galaxy.model.metadata import MetadataCollection
 from galaxy.model.orm.util import (
     add_object_to_object_session,
     add_object_to_session,
     get_object_session,
 )
@@ -89,15 +96,18 @@
 from galaxy.schema.bco.io_domain import Uri
 from galaxy.schema.bco.util import (
     extension_domains,
     galaxy_execution_domain,
     get_contributors,
     write_to_file,
 )
-from galaxy.schema.schema import ModelStoreFormat
+from galaxy.schema.schema import (
+    DatasetStateField,
+    ModelStoreFormat,
+)
 from galaxy.security.idencoding import IdEncodingHelper
 from galaxy.util import (
     FILENAME_VALID_CHARS,
     in_directory,
     safe_makedirs,
 )
 from galaxy.util.bunch import Bunch
@@ -167,14 +177,28 @@
     FORBID = "forbid"
     # Allow datasets to be imported as experimental DISCARDED datasets that are not deleted if file data unavailable.
     ALLOW = "allow"
     # Import all datasets as discarded regardless of whether file data is available in the store.
     FORCE = "force"
 
 
+class DatasetAttributeImportModel(BaseModel):
+    state: Optional[DatasetStateField] = None
+    deleted: Optional[bool] = None
+    purged: Optional[bool] = None
+    external_filename: Optional[str] = None
+    _extra_files_path: Optional[str] = None
+    file_size: Optional[int] = None
+    object_store_id: Optional[str] = None
+    total_size: Optional[int] = None
+    created_from_basename: Optional[str] = None
+    uuid: Optional[str] = None
+    model_config = ConfigDict(extra="ignore")
+
+
 DEFAULT_DISCARDED_DATA_TYPE = ImportDiscardedDataType.FORBID
 
 
 class ImportOptions:
     allow_edit: bool
     allow_library_creation: bool
     allow_dataset_object_edit: bool
@@ -267,16 +291,15 @@
         self.tag_handler = tag_handler
         if self.defines_new_history():
             self.import_history_encoded_id = self.new_history_properties().get("encoded_id")
         else:
             self.import_history_encoded_id = None
 
     @abc.abstractmethod
-    def workflow_paths(self) -> Iterator[Tuple[str, str]]:
-        ...
+    def workflow_paths(self) -> Iterator[Tuple[str, str]]: ...
 
     @abc.abstractmethod
     def defines_new_history(self) -> bool:
         """Does this store define a new history to create."""
 
     @abc.abstractmethod
     def new_history_properties(self) -> Dict[str, Any]:
@@ -287,32 +310,30 @@
         """Return a list of HDA properties."""
 
     def library_properties(self) -> List[Dict[str, Any]]:
         """Return a list of library properties."""
         return []
 
     @abc.abstractmethod
-    def invocations_properties(self) -> List[Dict[str, Any]]:
-        ...
+    def invocations_properties(self) -> List[Dict[str, Any]]: ...
 
     @abc.abstractmethod
     def collections_properties(self) -> List[Dict[str, Any]]:
         """Return a list of HDCA properties."""
 
     @abc.abstractmethod
     def implicit_dataset_conversion_properties(self) -> List[Dict[str, Any]]:
         """Return a list of ImplicitlyConvertedDatasetAssociation properties."""
 
     @abc.abstractmethod
     def jobs_properties(self) -> List[Dict[str, Any]]:
         """Return a list of jobs properties."""
 
     @abc.abstractmethod
-    def implicit_collection_jobs_properties(self) -> List[Dict[str, Any]]:
-        ...
+    def implicit_collection_jobs_properties(self) -> List[Dict[str, Any]]: ...
 
     @property
     @abc.abstractmethod
     def object_key(self) -> str:
         """Key used to connect objects in metadata.
 
         Legacy exports used 'hid' but associated objects may not be from the same history
@@ -440,44 +461,32 @@
         job: Optional[model.Job],
     ) -> None:
         object_key = self.object_key
 
         def handle_dataset_object_edit(dataset_instance, dataset_attrs):
             if "dataset" in dataset_attrs:
                 assert self.import_options.allow_dataset_object_edit
-                dataset_attributes = [
-                    "state",
-                    "deleted",
-                    "purged",
-                    "external_filename",
-                    "_extra_files_path",
-                    "file_size",
-                    "object_store_id",
-                    "total_size",
-                    "created_from_basename",
-                    "uuid",
-                ]
-
-                for attribute in dataset_attributes:
-                    if attribute in dataset_attrs["dataset"]:
-                        setattr(dataset_instance.dataset, attribute, dataset_attrs["dataset"][attribute])
+                dataset_attributes = DatasetAttributeImportModel(**dataset_attrs["dataset"]).model_dump(
+                    exclude_unset=True,
+                )
+                for attribute, value in dataset_attributes.items():
+                    setattr(dataset_instance.dataset, attribute, value)
                 self._attach_dataset_hashes(dataset_attrs["dataset"], dataset_instance)
                 self._attach_dataset_sources(dataset_attrs["dataset"], dataset_instance)
                 if "id" in dataset_attrs["dataset"] and self.import_options.allow_edit:
                     dataset_instance.dataset.id = dataset_attrs["dataset"]["id"]
                     for dataset_association in dataset_instance.dataset.history_associations:
                         if (
                             dataset_association is not dataset_instance
                             and dataset_association.extension == dataset_instance.extension
+                            or dataset_association.extension == "auto"
                         ):
-                            dataset_association.metadata = dataset_instance.metadata
-                            dataset_association.blurb = dataset_instance.blurb
-                            dataset_association.peek = dataset_instance.peek
-                            dataset_association.info = dataset_instance.info
-                            dataset_association.tool_version = dataset_instance.tool_version
+                            copy_dataset_instance_metadata_attributes(
+                                source=dataset_instance, target=dataset_association
+                            )
                 if job:
                     dataset_instance.dataset.job_id = job.id
 
         for dataset_attrs in datasets_attrs:
             if "state" not in dataset_attrs:
                 self.dataset_state_serialized = False
 
@@ -1033,14 +1042,15 @@
 
         invocations_attrs = self.invocations_properties()
         for invocation_attrs in invocations_attrs:
             assert not self.import_options.allow_edit
             imported_invocation = model.WorkflowInvocation()
             imported_invocation.user = self.user
             imported_invocation.history = history
+            ensure_object_added_to_session(imported_invocation, object_in_session=history)
             workflow_key = invocation_attrs["workflow"]
             if workflow_key not in object_import_tracker.workflows_by_key:
                 raise Exception(f"Failed to find key {workflow_key} in {object_import_tracker.workflows_by_key.keys()}")
             workflow = object_import_tracker.workflows_by_key[workflow_key]
             imported_invocation.workflow = workflow
             state = invocation_attrs["state"]
             if state in model.WorkflowInvocation.non_terminal_states:
@@ -1054,24 +1064,26 @@
             def attach_workflow_step(imported_object, attrs):
                 order_index = attrs["order_index"]
                 imported_object.workflow_step = workflow.step_by_index(order_index)  # noqa: B023
 
             for step_attrs in invocation_attrs["steps"]:
                 imported_invocation_step = model.WorkflowInvocationStep()
                 imported_invocation_step.workflow_invocation = imported_invocation
+                ensure_object_added_to_session(imported_invocation, session=self.sa_session)
                 attach_workflow_step(imported_invocation_step, step_attrs)
                 restore_times(imported_invocation_step, step_attrs)
                 imported_invocation_step.action = step_attrs["action"]
 
                 # TODO: ensure terminal...
                 imported_invocation_step.state = step_attrs["state"]
 
                 if "job" in step_attrs:
                     job = object_import_tracker.jobs_by_key[step_attrs["job"][object_key]]
                     imported_invocation_step.job = job
+                    ensure_object_added_to_session(imported_invocation_step, object_in_session=job)
                 elif "implicit_collection_jobs" in step_attrs:
                     icj = object_import_tracker.implicit_collection_jobs_by_key[
                         step_attrs["implicit_collection_jobs"][object_key]
                     ]
                     imported_invocation_step.implicit_collection_jobs = icj
 
                 # TODO: handle step outputs...
@@ -1493,27 +1505,25 @@
     def _normalize_job_parameters(
         self,
         imported_job: model.Job,
         job_attrs: Dict[str, Any],
         _find_hda: Callable,
         _find_hdca: Callable,
         _find_dce: Callable,
-    ) -> Dict[str, Any]:
-        ...
+    ) -> Dict[str, Any]: ...
 
     @abc.abstractmethod
     def _connect_job_io(
         self,
         imported_job: model.Job,
         job_attrs: Dict[str, Any],
         _find_hda: Callable,
         _find_hdca: Callable,
         _find_dce: Callable,
-    ) -> None:
-        ...
+    ) -> None: ...
 
     @property
     def file_source_root(self) -> str:
         return self.archive_dir
 
     def defines_new_history(self) -> bool:
         new_history_attributes = os.path.join(self.archive_dir, ATTRS_FILENAME_HISTORY)
@@ -1587,14 +1597,15 @@
             "exit_code",
             "traceback",
             "job_messages",
             "tool_stdout",
             "tool_stderr",
             "job_stdout",
             "job_stderr",
+            "galaxy_version",
         )
         for attribute in ATTRIBUTES:
             value = job_attrs.get(attribute)
             if value is not None:
                 setattr(imported_job, attribute, value)
         if "stdout" in job_attrs:
             imported_job.tool_stdout = job_attrs.get("stdout")
@@ -2020,16 +2031,15 @@
         for dataset in self.included_datasets:
             for metadata_element in dataset.metadata.values():
                 if isinstance(metadata_element, model.MetadataFile):
                     metadata_element.update_from_file(metadata_element.get_file_name())
 
     def export_job(self, job: model.Job, tool=None, include_job_data=True):
         self.export_jobs([job], include_job_data=include_job_data)
-        tool_source = getattr(tool, "tool_source", None)
-        if tool_source:
+        if tool_source := getattr(tool, "tool_source", None):
             with open(os.path.join(self.export_directory, "tool.xml"), "w") as out:
                 out.write(tool_source.to_string())
 
     def export_jobs(
         self,
         jobs: Iterable[model.Job],
         jobs_attrs: Optional[List[Dict[str, Any]]] = None,
@@ -2359,16 +2369,15 @@
 
             def record_job(job):
                 if not job:
                     # No viable job.
                     return
 
                 jobs_dict[job.id] = job
-                icja = job.implicit_collection_jobs_association
-                if icja:
+                if icja := job.implicit_collection_jobs_association:
                     implicit_collection_jobs = icja.implicit_collection_jobs
                     implicit_collection_jobs_dict[implicit_collection_jobs.id] = implicit_collection_jobs
 
             def record_associated_jobs(obj):
                 # Get the job object.
                 job = None
                 for assoc in getattr(obj, "creating_job_associations", []):
@@ -2381,18 +2390,16 @@
                 # Get the associated job, if any. If this hda was copied from another,
                 # we need to find the job that created the original hda
                 if not isinstance(hda, (model.HistoryDatasetAssociation, model.LibraryDatasetDatasetAssociation)):
                     raise Exception(
                         f"Expected a HistoryDatasetAssociation or LibraryDatasetDatasetAssociation, but got a {type(hda)}: {hda}"
                     )
                 job_hda = hda
-                while getattr(
-                    job_hda, "copied_from_history_dataset_association", None
-                ):  # should this check library datasets as well?
-                    job_hda = job_hda.copied_from_history_dataset_association  # type: ignore[union-attr]
+                while job_hda.copied_from_history_dataset_association:  # should this check library datasets as well?
+                    job_hda = job_hda.copied_from_history_dataset_association
                 if not job_hda.creating_job_associations:
                     # No viable HDA found.
                     continue
 
                 record_associated_jobs(job_hda)
 
             for hdca in self.included_collections:
@@ -2463,16 +2470,15 @@
     export_directory: StrPath
     included_datasets: Dict[model.DatasetInstance, Tuple[model.DatasetInstance, bool]]
     dataset_implicit_conversions: Dict[model.DatasetInstance, model.ImplicitlyConvertedDatasetAssociation]
     dataset_id_to_path: Dict[int, Tuple[Optional[str], Optional[str]]]
 
     @property
     @abc.abstractmethod
-    def workflows_directory(self) -> str:
-        ...
+    def workflows_directory(self) -> str: ...
 
     def _generate_markdown_readme(self) -> str:
         markdown_parts: List[str] = []
         if self._is_single_invocation_export():
             invocation = self.included_invocations[0]
             name = invocation.workflow.name
             create_time = invocation.create_time
@@ -2761,22 +2767,22 @@
             export_options.override_environment_variables,
         )
         extension_domain = extension_domains(export_options.galaxy_url, export_options.galaxy_version)
         error_domain = ErrorDomain(
             empirical_error=export_options.override_empirical_error or {},
             algorithmic_error=export_options.override_algorithmic_error or {},
         )
-        usability_domain = UsabilityDomain(__root__=usability_domain_str)
+        usability_domain = UsabilityDomain(root=usability_domain_str)
         description_domain = DescriptionDomain(
             keywords=keywords,
             xref=export_options.override_xref or [],
             platform=["Galaxy"],
             pipeline_steps=pipeline_steps,
         )
-        parametric_domain = ParametricDomain(__root__=parametric_domain_items)
+        parametric_domain = ParametricDomain(root=parametric_domain_items)
         io_domain = InputAndOutputDomain(
             input_subdomain=input_subdomain_items,
             output_subdomain=output_subdomain_items,
         )
         core = BioComputeObjectCore(
             description_domain=description_domain,
             error_domain=error_domain,
@@ -3072,7 +3078,16 @@
         assert isinstance(store_dict, dict)
         temp_dir = mkdtemp()
         import_json = os.path.join(temp_dir, "import_store.json")
         with open(import_json, "w") as f:
             dump(store_dict, f)
         source_uri = f"file://{import_json}"
     return source_uri
+
+
+def copy_dataset_instance_metadata_attributes(source: model.DatasetInstance, target: model.DatasetInstance) -> None:
+    target.metadata = source.metadata
+    target.blurb = source.blurb
+    target.peek = source.peek
+    target.info = source.info
+    target.tool_version = source.tool_version
+    target.extension = source.extension
```

### Comparing `galaxy-data-23.2.1/galaxy/model/store/_bco_convert_utils.py` & `galaxy-data-24.0.0/galaxy/model/store/_bco_convert_utils.py`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/model/store/build_objects.py` & `galaxy-data-24.0.0/galaxy/model/store/build_objects.py`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/model/store/discover.py` & `galaxy-data-24.0.0/galaxy/model/store/discover.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Utilities for discovering files to add to a model store.
 
 Working with input "JSON" format used for Fetch API, galaxy.json
 imports, etc... High-level utilities in this file can be used during
 job output discovery or for persisting Galaxy model objects
 corresponding to files in other contexts.
 """
+
 import abc
 import logging
 import os
 from typing import (
     Any,
     Callable,
     Dict,
@@ -274,63 +275,71 @@
         self,
         collection,
         root_collection_builder,
         discovered_files,
         name=None,
         metadata_source_name=None,
         final_job_state="ok",
+        change_datatype_actions=None,
     ):
         # TODO: allow configurable sorting.
         #    <sort by="lexical" /> <!-- default -->
         #    <sort by="reverse_lexical" />
         #    <sort regex="example.(\d+).fastq" by="1:numerical" />
         #    <sort regex="part_(\d+)_sample_([^_]+).fastq" by="2:lexical,1:numerical" />
         if name is None:
             name = "unnamed output"
+        if change_datatype_actions is None:
+            change_datatype_actions = {}
         if self.flush_per_n_datasets and self.flush_per_n_datasets > 0:
             for chunk in chunk_iterable(discovered_files, size=self.flush_per_n_datasets):
                 self._populate_elements(
                     chunk=chunk,
                     name=name,
                     root_collection_builder=root_collection_builder,
                     metadata_source_name=metadata_source_name,
                     final_job_state=final_job_state,
+                    change_datatype_actions=change_datatype_actions,
                 )
                 if len(chunk) == self.flush_per_n_datasets:
                     # In most cases we don't need to flush, that happens in the caller.
                     # Only flush here for saving memory.
                     root_collection_builder.populate_partial()
                     self.flush()
         else:
             self._populate_elements(
                 chunk=discovered_files,
                 name=name,
                 root_collection_builder=root_collection_builder,
                 metadata_source_name=metadata_source_name,
                 final_job_state=final_job_state,
+                change_datatype_actions=change_datatype_actions,
             )
 
-    def _populate_elements(self, chunk, name, root_collection_builder, metadata_source_name, final_job_state):
+    def _populate_elements(
+        self, chunk, name, root_collection_builder, metadata_source_name, final_job_state, change_datatype_actions
+    ):
         element_datasets: Dict[str, List[Any]] = {
             "element_identifiers": [],
             "datasets": [],
             "tag_lists": [],
             "paths": [],
             "extra_files": [],
         }
+        ext_override = change_datatype_actions.get(name)
         for discovered_file in chunk:
             filename = discovered_file.path
             create_dataset_timer = ExecutionTimer()
             fields_match = discovered_file.match
             if not fields_match:
                 raise Exception(f"Problem parsing metadata fields for file {filename}")
             element_identifiers = fields_match.element_identifiers
             designation = fields_match.designation
             visible = fields_match.visible
-            ext = fields_match.ext
+            ext = ext_override or fields_match.ext
             dbkey = fields_match.dbkey
             extra_files = fields_match.extra_files
             # galaxy.tools.parser.output_collection_def.INPUT_DBKEY_TOKEN
             if dbkey == "__input__":
                 dbkey = self.input_dbkey
 
             # Create new primary dataset
@@ -1000,16 +1009,15 @@
         self.path = path
         self._parent_identifiers = parent_identifiers
 
     @property
     def designation(self):
         # If collecting nested collection, grab identifier_0,
         # identifier_1, etc... and join on : to build designation.
-        element_identifiers = self.raw_element_identifiers
-        if element_identifiers:
+        if element_identifiers := self.raw_element_identifiers:
             return ":".join(element_identifiers)
         elif "designation" in self.as_dict:
             return self.as_dict.get("designation")
         elif "name" in self.as_dict:
             return self.as_dict.get("name")
         else:
             return None
```

### Comparing `galaxy-data-23.2.1/galaxy/model/store/load_objects.py` & `galaxy-data-24.0.0/galaxy/model/store/load_objects.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,16 +31,15 @@
         argv = sys.argv[1:]
     args = _arg_parser().parse_args(argv)
 
     galaxy_url = args.galaxy_url
     api_url = f"{galaxy_url.rstrip('/')}/api"
     api_key = args.key
     assert api_key
-    history_id = args.history_id
-    if history_id:
+    if history_id := args.history_id:
         create_url = f"{api_url}/histories/{history_id}/contents_from_store?key={api_key}"
     else:
         create_url = f"{api_url}/histories/from_store?key={api_key}"
 
     store_path = args.store
     assert os.path.exists(store_path)
     is_json = False
```

### Comparing `galaxy-data-23.2.1/galaxy/model/store/ro_crate_utils.py` & `galaxy-data-24.0.0/galaxy/model/store/ro_crate_utils.py`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/model/tags.py` & `galaxy-data-24.0.0/galaxy/model/tags.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,17 +143,16 @@
             tags.append(self.get_tag_by_id(tag_id))
         return tags
 
     def remove_item_tag(self, user: "User", item, tag_name: str):
         """Remove a tag from an item."""
         self._ensure_user_owns_item(user, item)
         # Get item tag association.
-        item_tag_assoc = self._get_item_tag_assoc(user, item, tag_name)
         # Remove association.
-        if item_tag_assoc:
+        if item_tag_assoc := self._get_item_tag_assoc(user, item, tag_name):
             # Delete association.
             self.sa_session.delete(item_tag_assoc)
             item.tags.remove(item_tag_assoc)
             return True
         return False
 
     def delete_item_tags(self, user: Optional["User"], item):
```

### Comparing `galaxy-data-23.2.1/galaxy/model/tool_shed_install/__init__.py` & `galaxy-data-24.0.0/galaxy/model/tool_shed_install/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,20 +51,18 @@
 
 else:
     from sqlalchemy.orm.decl_api import DeclarativeMeta
 
 
 class HasToolBox(common_util.HasToolShedRegistry, Protocol):
     @property
-    def tool_dependency_dir(self) -> Optional[str]:
-        ...
+    def tool_dependency_dir(self) -> Optional[str]: ...
 
     @property
-    def toolbox(self) -> AbstractToolBox:
-        ...
+    def toolbox(self) -> AbstractToolBox: ...
 
 
 class Base(metaclass=DeclarativeMeta):
     __abstract__ = True
     registry = mapper_registry
     metadata = mapper_registry.metadata
     __init__ = mapper_registry.constructor
@@ -238,18 +236,17 @@
             shed_config_dict = app.toolbox.get_shed_config_dict_by_filename(self.shed_config_filename)
             if shed_config_dict:
                 return shed_config_dict
         return self.guess_shed_config(app)
 
     def get_tool_relative_path(self, app: HasToolBox):
         # This is a somewhat public function, used by data_manager_manual for instance
-        shed_conf_dict = self.get_shed_config_dict(app)
         tool_path = None
         relative_path = None
-        if shed_conf_dict:
+        if shed_conf_dict := self.get_shed_config_dict(app):
             tool_path = shed_conf_dict["tool_path"]
             relative_path = os.path.join(
                 self.tool_shed_path_name, "repos", self.owner, self.name, self.installed_changeset_revision
             )
         return tool_path, relative_path
 
     def guess_shed_config(self, app: HasToolBox):
@@ -407,16 +404,15 @@
         missing_dependencies = []
         for tool_dependency in self.tool_dependencies:
             if tool_dependency.status not in [ToolDependency.installation_status.INSTALLED]:
                 missing_dependencies.append(tool_dependency)
         return missing_dependencies
 
     def repo_files_directory(self, app: HasToolBox):
-        repo_path = self.repo_path(app)
-        if repo_path:
+        if repo_path := self.repo_path(app):
             return os.path.join(repo_path, self.name)
         return None
 
     def repo_path(self, app: HasToolBox):
         tool_shed = common_util.remove_protocol_and_port_from_tool_shed_url(self.tool_shed)
         for shed_tool_conf_dict in app.toolbox.dynamic_confs(include_migrated_tool_conf=True):
             tool_path = shed_tool_conf_dict["tool_path"]
```

### Comparing `galaxy-data-23.2.1/galaxy/model/tool_shed_install/mapping.py` & `galaxy-data-24.0.0/galaxy/model/tool_shed_install/mapping.py`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/model/triggers/history_update_time_field.py` & `galaxy-data-24.0.0/galaxy/model/triggers/history_update_time_field.py`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/model/triggers/update_audit_table.py` & `galaxy-data-24.0.0/galaxy/model/triggers/update_audit_table.py`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/model/unittest_utils/beaker_testing_utils.py` & `galaxy-data-24.0.0/galaxy/model/unittest_utils/beaker_testing_utils.py`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/model/unittest_utils/data_app.py` & `galaxy-data-24.0.0/galaxy/model/unittest_utils/data_app.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Mock GalaxyApp exposing config + functionality required for galaxy-data package.
 
 There is a more expansive MockApp in test/unit/unittest_utils - but it isn't packaged
 and it has dependencies from across the app. This mock application and config is
 more appropriate for testing galaxy-data functionality and will be included with
 galaxy-data.
 """
+
 import os
 import shutil
 import tempfile
 from typing import Optional
 
 from galaxy import (
     model,
@@ -52,14 +53,15 @@
         self.data_dir = os.path.join(root, "database")
 
         self.security = IdEncodingHelper(id_secret=GALAXY_TEST_UNITTEST_SECRET)
         self.database_connection = kwd.get("database_connection", GALAXY_TEST_IN_MEMORY_DB_CONNECTION)
 
         # objectstore config values...
         self.object_store_config_file = ""
+        self.object_store_config = None
         self.object_store = "disk"
         self.object_store_check_old_style = False
         self.object_store_cache_path = "/tmp/cache"
         self.object_store_store_by = "uuid"
 
         self.umask = os.umask(0o77)
         self.gid = os.getgid()
```

### Comparing `galaxy-data-23.2.1/galaxy/model/unittest_utils/gxy_model_fixtures.py` & `galaxy-data-24.0.0/galaxy/model/unittest_utils/gxy_model_fixtures.py`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/model/unittest_utils/mapping_testing_utils.py` & `galaxy-data-24.0.0/galaxy/model/unittest_utils/mapping_testing_utils.py`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/model/unittest_utils/migration_scripts_testing_utils.py` & `galaxy-data-24.0.0/galaxy/model/unittest_utils/migration_scripts_testing_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,13 +71,13 @@
     args = ["sh", cmd_path] + cmd_args
     return subprocess.run(args, capture_output=True, text=True)
 
 
 def get_db_heads(config: Config) -> Tuple[str, ...]:
     """Return revision ids (version heads) stored in the database."""
     dburl = config.get_main_option("sqlalchemy.url")
-    engine = create_engine(dburl)
+    engine = create_engine(dburl, future=True)
     with engine.connect() as conn:
         context = MigrationContext.configure(conn)
         heads = context.get_current_heads()
     engine.dispose()
     return heads
```

### Comparing `galaxy-data-23.2.1/galaxy/model/unittest_utils/model_testing_utils.py` & `galaxy-data-24.0.0/galaxy/model/unittest_utils/model_testing_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     select,
 )
 from sqlalchemy.engine import (
     Engine,
     make_url,
 )
 from sqlalchemy.sql.compiler import IdentifierPreparer
+from sqlalchemy.sql.expression import text
 
 from galaxy.model.database_utils import (
     create_database,
     DbUrl,
     is_postgres,
 )
 
@@ -62,15 +63,15 @@
         if is_postgres(url):
             _drop_postgres_database(url)
 
 
 @contextmanager
 def disposing_engine(url: DbUrl) -> Iterator[Engine]:
     """Context manager for engine that disposes of its connection pool on exit."""
-    engine = create_engine(url)
+    engine = create_engine(url, future=True)
     try:
         yield engine
     finally:
         engine.dispose()
 
 
 @pytest.fixture
@@ -93,16 +94,15 @@
     Return a factory function that produces a database url with a unique database name.
     If _get_connection_url() returns a value, the database is postgresql; otherwise, it's
     sqlite (referring to a location witin the /tmp directory).
     """
 
     def url() -> DbUrl:
         database = _generate_unique_database_name()
-        connection_url = _get_connection_url()
-        if connection_url:
+        if connection_url := _get_connection_url():
             return _make_postgres_db_url(DbUrl(connection_url), database)
         else:
             return _make_sqlite_db_url(tmp_directory, database)
 
     return url
 
 
@@ -111,16 +111,15 @@
     """
     Return a database url with a unique database name.
     If _get_connection_url() returns a value, the database is postgresql; otherwise, it's
     sqlite (referring to a location witin the /tmp directory).
     """
     # TODO this duplication should be removed (see url_factory).
     database = _generate_unique_database_name()
-    connection_url = _get_connection_url()
-    if connection_url:
+    if connection_url := _get_connection_url():
         return _make_postgres_db_url(DbUrl(connection_url), database)
     else:
         return _make_sqlite_db_url(tmp_directory, database)
 
 
 def initialize_model(mapper_registry, engine):
     mapper_registry.metadata.create_all(engine)
@@ -230,18 +229,18 @@
     db_url = make_url(url)
     database = db_url.database
     connection_url = db_url.set(database="postgres")
     _drop_database(connection_url, database)
 
 
 def _drop_database(connection_url, database_name):
-    engine = create_engine(connection_url, isolation_level="AUTOCOMMIT")
+    engine = create_engine(connection_url, isolation_level="AUTOCOMMIT", future=True)
     preparer = IdentifierPreparer(engine.dialect)
     database_name = preparer.quote(database_name)
-    stmt = f"DROP DATABASE IF EXISTS {database_name}"
+    stmt = text(f"DROP DATABASE IF EXISTS {database_name}")
     with engine.connect() as conn:
         conn.execute(stmt)
     engine.dispose()
 
 
 def _get_default_where_clause(cls, obj_id):
     where_clause = cls.__table__.c.id == obj_id
```

### Comparing `galaxy-data-23.2.1/galaxy/model/unittest_utils/store_fixtures.py` & `galaxy-data-24.0.0/galaxy/model/unittest_utils/store_fixtures.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Fixtures for populating model stores."""
+
 from typing import (
     Any,
     Dict,
 )
 from uuid import uuid4
 
 from galaxy.model.orm.now import now
```

### Comparing `galaxy-data-23.2.1/galaxy/model/unittest_utils/tsi_model_fixtures.py` & `galaxy-data-24.0.0/galaxy/model/unittest_utils/tsi_model_fixtures.py`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/quota/_schema.py` & `galaxy-data-24.0.0/galaxy/quota/_schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 from enum import Enum
 from typing import (
     List,
     Optional,
 )
 
-from pydantic import Field
+from pydantic import (
+    Field,
+    RootModel,
+)
 from typing_extensions import Literal
 
 from galaxy.schema.fields import (
-    DecodedDatabaseIdField,
+    EncodedDatabaseIdField,
     ModelClassField,
 )
 from galaxy.schema.schema import (
     GroupModel,
     Model,
     UserModel,
+    WithModelClass,
 )
 
 QUOTA = Literal["Quota"]
 USER_QUOTA_ASSOCIATION = Literal["UserQuotaAssociation"]
 GROUP_QUOTA_ASSOCIATION = Literal["GroupQuotaAssociation"]
 DEFAULT_QUOTA_ASSOCIATION = Literal["DefaultQuotaAssociation"]
 
@@ -62,50 +66,52 @@
         "- `=` : The quota is exactly the amount specified"
         "- `+` : The amount specified will be added to the amounts of the user's other associated quota definitions"
         "- `-` : The amount specified will be subtracted from the amounts of the user's other associated quota definitions"
     ),
 )
 
 
-class DefaultQuota(Model):  # TODO: should this replace lib.galaxy.model.DefaultQuotaAssociation at some point?
+class DefaultQuota(
+    Model, WithModelClass
+):  # TODO: should this replace lib.galaxy.model.DefaultQuotaAssociation at some point?
     model_class: DEFAULT_QUOTA_ASSOCIATION = ModelClassField(DEFAULT_QUOTA_ASSOCIATION)
     type: DefaultQuotaTypes = Field(
         ...,
         title="Type",
         description=(
             "The type of the default quota. Either one of:\n"
             " - `registered`: the associated quota will affect registered users.\n"
             " - `unregistered`: the associated quota will affect unregistered users.\n"
         ),
     )
 
 
-class UserQuota(Model):
+class UserQuota(Model, WithModelClass):
     model_class: USER_QUOTA_ASSOCIATION = ModelClassField(USER_QUOTA_ASSOCIATION)
     user: UserModel = Field(
         ...,
         title="User",
         description="Information about a user associated with a quota.",
     )
 
 
-class GroupQuota(Model):
+class GroupQuota(Model, WithModelClass):
     model_class: GROUP_QUOTA_ASSOCIATION = ModelClassField(GROUP_QUOTA_ASSOCIATION)
     group: GroupModel = Field(
         ...,
         title="Group",
         description="Information about a user group associated with a quota.",
     )
 
 
-class QuotaBase(Model):
+class QuotaBase(Model, WithModelClass):
     """Base model containing common fields for Quotas."""
 
     model_class: QUOTA = ModelClassField(QUOTA)
-    id: DecodedDatabaseIdField = Field(
+    id: EncodedDatabaseIdField = Field(
         ...,
         title="ID",
         description="The `encoded identifier` of the quota.",
     )
     name: str = QuotaNameField
     quota_source_label: Optional[str] = Field(
         None,
@@ -117,20 +123,21 @@
 class QuotaSummary(QuotaBase):
     """Contains basic information about a Quota"""
 
     url: str = Field(
         ...,
         title="URL",
         description="The relative URL to get this particular Quota details from the rest API.",
-        deprecated=True,
+        # TODO: also deprecate on python side, https://github.com/pydantic/pydantic/issues/2255
+        json_schema_extra={"deprecated": True},
     )
 
 
-class QuotaSummaryList(Model):
-    __root__: List[QuotaSummary] = Field(
+class QuotaSummaryList(RootModel):
+    root: List[QuotaSummary] = Field(
         default=[],
         title="List with summary information of Quotas.",
     )
 
 
 class QuotaDetails(QuotaBase):
     description: str = QuotaDescriptionField
```

### Comparing `galaxy-data-23.2.1/galaxy/security/__init__.py` & `galaxy-data-24.0.0/galaxy/security/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Galaxy Security
 
 """
+
 from typing import (
     List,
     Optional,
 )
 
 from typing_extensions import Literal
 
@@ -32,15 +33,15 @@
         DATASET_MANAGE_PERMISSIONS=Action(
             "manage permissions",
             "Users having associated role can manage the roles associated with permissions on this dataset.",
             "grant",
         ),
         DATASET_ACCESS=Action(
             "access",
-            "Users having associated role can import this dataset into their history for analysis.",
+            "Users having all associated roles can import this dataset into their history for analysis.",
             "restrict",
         ),
         LIBRARY_ACCESS=Action(
             "access library", "Restrict access to this library to only users having associated role", "restrict"
         ),
         LIBRARY_ADD=Action(
             "add library item", "Users having associated role can add library items to this library item", "grant"
@@ -84,14 +85,17 @@
 
     def can_add_library_item(self, roles, item):
         raise Exception("Unimplemented Method")
 
     def can_modify_library_item(self, roles, item):
         raise Exception("Unimplemented Method")
 
+    def can_change_object_store_id(self, user, dataset):
+        raise Exception("Unimplemented Method")
+
     def can_manage_library_item(self, roles, item):
         raise Exception("Unimplemented Method")
 
     def associate_components(self, **kwd):
         raise Exception(f"No valid method of associating provided components: {kwd}")
 
     def create_private_user_role(self, user):
```

### Comparing `galaxy-data-23.2.1/galaxy/security/idencoding.py` & `galaxy-data-24.0.0/galaxy/security/idencoding.py`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/security/object_wrapper.py` & `galaxy-data-24.0.0/galaxy/security/object_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,16 +161,15 @@
         # This allows e.g. isinstance to continue to work.
         try:
             wrapped_class_name = value.__name__
             wrapped_class = value
         except Exception:
             wrapped_class_name = value.__class__.__name__
             wrapped_class = value.__class__
-        value_mod = inspect.getmodule(value)
-        if value_mod:
+        if value_mod := inspect.getmodule(value):
             wrapped_class_name = f"{value_mod.__name__}.{wrapped_class_name}"
         wrapped_class_name = (
             f"SafeStringWrapper__{wrapped_class_name}__{'__'.join(sorted(c.__name__ for c in no_wrap_classes))}"
         )
         do_wrap_func_name = f"__do_wrap_{wrapped_class_name}"
         do_wrap_func = __do_wrap
         global_dict = globals()
```

### Comparing `galaxy-data-23.2.1/galaxy/security/passwords.py` & `galaxy-data-24.0.0/galaxy/security/passwords.py`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/security/ssh_util.py` & `galaxy-data-24.0.0/galaxy/security/ssh_util.py`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy/security/validate_user_input.py` & `galaxy-data-24.0.0/galaxy/security/validate_user_input.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Utilities for validating inputs related to user objects.
 
 The validate_* methods in this file return simple messages that do not contain
 user inputs - so these methods do not need to be escaped.
 """
+
 import logging
 import re
 from typing import Optional
 
 import dns.resolver
 from dns.exception import DNSException
 from sqlalchemy import (
@@ -125,16 +126,15 @@
 def validate_publicname(trans, publicname, user=None):
     """
     Check that publicname respects the minimum and maximum string length, the
     allowed characters, and that the username is not taken already.
     """
     if user and user.username == publicname:
         return ""
-    message = validate_publicname_str(publicname)
-    if message:
+    if message := validate_publicname_str(publicname):
         return message
 
     stmt = select(trans.app.model.User).filter_by(username=publicname).limit(1)
     if trans.sa_session.scalars(stmt).first():
         return "Public name is taken; please choose another."
     return ""
```

### Comparing `galaxy-data-23.2.1/galaxy/security/vault.py` & `galaxy-data-24.0.0/galaxy/security/vault.py`

 * *Files identical despite different names*

### Comparing `galaxy-data-23.2.1/galaxy_data.egg-info/PKG-INFO` & `galaxy-data-24.0.0/galaxy_data.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,64 @@
 Metadata-Version: 2.1
 Name: galaxy-data
-Version: 23.2.1
+Version: 24.0.0
 Summary: Galaxy datatype framework and datatypes
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Academic Free License (AFL)
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Software Development :: Testing
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: galaxy-files
+Requires-Dist: galaxy-objectstore
+Requires-Dist: galaxy-tool-util
+Requires-Dist: galaxy-util[template]
+Requires-Dist: alembic
+Requires-Dist: alembic-utils
+Requires-Dist: bdbag>=1.6.3
+Requires-Dist: bx-python
+Requires-Dist: dnspython
+Requires-Dist: galaxy-sequence-utils
+Requires-Dist: h5grove>=1.2.1
+Requires-Dist: h5py
+Requires-Dist: isa-rwval>=0.10.10
+Requires-Dist: isal
+Requires-Dist: MarkupSafe
+Requires-Dist: msal
+Requires-Dist: mrcfile
+Requires-Dist: numpy
+Requires-Dist: parsley
+Requires-Dist: pycryptodome
+Requires-Dist: pydantic[email]!=2.6.0,!=2.6.1,>=2
+Requires-Dist: pylibmagic
+Requires-Dist: python-magic
+Requires-Dist: pysam>=0.21
+Requires-Dist: rocrate
+Requires-Dist: social-auth-core[openidconnect]==4.0.3
+Requires-Dist: SQLAlchemy<2,>=1.4.25
+Requires-Dist: tifffile
+Requires-Dist: typing-extensions
+Requires-Dist: WebOb
 
 
 .. image:: https://badge.fury.io/py/galaxy-data.svg
    :target: https://pypi.org/project/galaxy-data/
 
 
 Overview
@@ -42,14 +72,84 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+24.0.0 (2024-04-02)
+-------------------
+
+
+=========
+Bug fixes
+=========
+
+* Fix for converter tests by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#17188 <https://github.com/galaxyproject/galaxy/pull/17188>`_
+* correct dbkey for minerva display app by `@hexylena <https://github.com/hexylena>`_ in `#17196 <https://github.com/galaxyproject/galaxy/pull/17196>`_
+* Fix invocation serialization if no state was set by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17278 <https://github.com/galaxyproject/galaxy/pull/17278>`_
+* Fix quotas ID encoding by `@davelopez <https://github.com/davelopez>`_ in `#17335 <https://github.com/galaxyproject/galaxy/pull/17335>`_
+* Fix model store exports that include implicit conversions.  by `@jmchilton <https://github.com/jmchilton>`_ in `#17346 <https://github.com/galaxyproject/galaxy/pull/17346>`_
+* Fix bug: create new PSAAssociation if not in database by `@jdavcs <https://github.com/jdavcs>`_ in `#17516 <https://github.com/galaxyproject/galaxy/pull/17516>`_
+* Fix social_core methods by `@jdavcs <https://github.com/jdavcs>`_ in `#17530 <https://github.com/galaxyproject/galaxy/pull/17530>`_
+* Fix ancient bug: incorrect usage of func.coalesce in User model by `@jdavcs <https://github.com/jdavcs>`_ in `#17577 <https://github.com/galaxyproject/galaxy/pull/17577>`_
+* Account for newlines in CIF Datatype sniffer by `@patrick-austin <https://github.com/patrick-austin>`_ in `#17582 <https://github.com/galaxyproject/galaxy/pull/17582>`_
+* Anticipate PendingRollbackError in ``check_database_connection`` by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17598 <https://github.com/galaxyproject/galaxy/pull/17598>`_
+* Add basic model import attribute validation by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17628 <https://github.com/galaxyproject/galaxy/pull/17628>`_
+* More efficient change_state queries, maybe fix deadlock by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17632 <https://github.com/galaxyproject/galaxy/pull/17632>`_
+* Npz sniffing: do not read the whole file by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#17672 <https://github.com/galaxyproject/galaxy/pull/17672>`_
+* Assert that at least one file in npz zipfile ends with .npy by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17679 <https://github.com/galaxyproject/galaxy/pull/17679>`_
+* Workflow Comment Indexing by `@ElectronicBlueberry <https://github.com/ElectronicBlueberry>`_ in `#17700 <https://github.com/galaxyproject/galaxy/pull/17700>`_
+* Fix source history update_time being updated when importing a public history by `@jmchilton <https://github.com/jmchilton>`_ in `#17728 <https://github.com/galaxyproject/galaxy/pull/17728>`_
+* Also set extension and metadata on copies of job outputs when finishing job by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17777 <https://github.com/galaxyproject/galaxy/pull/17777>`_
+* Defer job attributes that are usually not needed by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17795 <https://github.com/galaxyproject/galaxy/pull/17795>`_
+* Fix change_datatype PJA for dynamic collections  by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17803 <https://github.com/galaxyproject/galaxy/pull/17803>`_
+* Simplify nested collection joins by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17817 <https://github.com/galaxyproject/galaxy/pull/17817>`_
+* Fix very slow user data table query by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17830 <https://github.com/galaxyproject/galaxy/pull/17830>`_
+* Update db revision 24.0 release tags by `@jdavcs <https://github.com/jdavcs>`_ in `#17834 <https://github.com/galaxyproject/galaxy/pull/17834>`_
+* Minor refactor of query building logic for readability by `@jdavcs <https://github.com/jdavcs>`_ in `#17835 <https://github.com/galaxyproject/galaxy/pull/17835>`_
+* Fix user login when duplicate UserRoleAssociation exists by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17854 <https://github.com/galaxyproject/galaxy/pull/17854>`_
+
+============
+Enhancements
+============
+
+* Make columns types an empty list for empty tabular data  by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#13918 <https://github.com/galaxyproject/galaxy/pull/13918>`_
+* port invocation API to fastapi by `@martenson <https://github.com/martenson>`_ in `#16707 <https://github.com/galaxyproject/galaxy/pull/16707>`_
+* SQLAlchemy 2.0 upgrades (part 5) by `@jdavcs <https://github.com/jdavcs>`_ in `#16932 <https://github.com/galaxyproject/galaxy/pull/16932>`_
+* Python 3.8 as minimum by `@mr-c <https://github.com/mr-c>`_ in `#16954 <https://github.com/galaxyproject/galaxy/pull/16954>`_
+*  Expose more tool information / navigability in UI. by `@jmchilton <https://github.com/jmchilton>`_ in `#17105 <https://github.com/galaxyproject/galaxy/pull/17105>`_
+* Add support for (fast5.tar).xz binary compressed files by `@tuncK <https://github.com/tuncK>`_ in `#17106 <https://github.com/galaxyproject/galaxy/pull/17106>`_
+* SA2.0 updates: handling "object is being merged into a Session along the backref cascade path" by `@jdavcs <https://github.com/jdavcs>`_ in `#17122 <https://github.com/galaxyproject/galaxy/pull/17122>`_
+* Towards SQLAlchemy 2.0: fix last cases of RemovedIn20Warning by `@jdavcs <https://github.com/jdavcs>`_ in `#17132 <https://github.com/galaxyproject/galaxy/pull/17132>`_
+* Create pydantic model for the return of show operation -  get: `/api/jobs/{job_id}`  by `@heisner-tillman <https://github.com/heisner-tillman>`_ in `#17153 <https://github.com/galaxyproject/galaxy/pull/17153>`_
+* Much simpler default dataset permissions for typical users. by `@jmchilton <https://github.com/jmchilton>`_ in `#17166 <https://github.com/galaxyproject/galaxy/pull/17166>`_
+* Add future=True flag to SA engine by `@jdavcs <https://github.com/jdavcs>`_ in `#17174 <https://github.com/galaxyproject/galaxy/pull/17174>`_
+* Add future=True flag to SA session by `@jdavcs <https://github.com/jdavcs>`_ in `#17179 <https://github.com/galaxyproject/galaxy/pull/17179>`_
+* Vueifiy History Grids by `@guerler <https://github.com/guerler>`_ in `#17219 <https://github.com/galaxyproject/galaxy/pull/17219>`_
+* Convert sample object store configuration to YAML and support configuring inline by `@natefoo <https://github.com/natefoo>`_ in `#17222 <https://github.com/galaxyproject/galaxy/pull/17222>`_
+* Migrate models to pydantic 2 by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17262 <https://github.com/galaxyproject/galaxy/pull/17262>`_
+* API endpoint that allows "changing" the objectstore for "safe" scenarios.  by `@jmchilton <https://github.com/jmchilton>`_ in `#17329 <https://github.com/galaxyproject/galaxy/pull/17329>`_
+* Enable ``warn_unreachable`` mypy option by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17365 <https://github.com/galaxyproject/galaxy/pull/17365>`_
+* Fix type annotation of code using XML etree by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17367 <https://github.com/galaxyproject/galaxy/pull/17367>`_
+* Add explicit cache_ok attribute to JSONType subclass by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17376 <https://github.com/galaxyproject/galaxy/pull/17376>`_
+* More specific type annotation for ``BaseJobExec.parse_status()`` by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17381 <https://github.com/galaxyproject/galaxy/pull/17381>`_
+* Update to black 2024 stable style by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17391 <https://github.com/galaxyproject/galaxy/pull/17391>`_
+* Allow using tool data bundles as inputs to reference data select parameters by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17435 <https://github.com/galaxyproject/galaxy/pull/17435>`_
+* UI for "relocating" a dataset to a new object store (when safe) by `@jmchilton <https://github.com/jmchilton>`_ in `#17437 <https://github.com/galaxyproject/galaxy/pull/17437>`_
+* Allow filtering history datasets by object store ID and quota source. by `@jmchilton <https://github.com/jmchilton>`_ in `#17460 <https://github.com/galaxyproject/galaxy/pull/17460>`_
+* Faster FASTA and FASTQ metadata setting by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#17462 <https://github.com/galaxyproject/galaxy/pull/17462>`_
+* Feature SBOL datatypes by `@guillaume-gricourt <https://github.com/guillaume-gricourt>`_ in `#17482 <https://github.com/galaxyproject/galaxy/pull/17482>`_
+* Display workflow invocation counts. by `@jmchilton <https://github.com/jmchilton>`_ in `#17488 <https://github.com/galaxyproject/galaxy/pull/17488>`_
+* add npy datatype by `@astrovsky01 <https://github.com/astrovsky01>`_ in `#17517 <https://github.com/galaxyproject/galaxy/pull/17517>`_
+* Enhance Avivator display app to support regular Tiffs by `@davelopez <https://github.com/davelopez>`_ in `#17554 <https://github.com/galaxyproject/galaxy/pull/17554>`_
+* Update Python dependencies by `@galaxybot <https://github.com/galaxybot>`_ in `#17580 <https://github.com/galaxyproject/galaxy/pull/17580>`_
+* Add migrations revision identifier for 24.0 by `@jdavcs <https://github.com/jdavcs>`_ in `#17589 <https://github.com/galaxyproject/galaxy/pull/17589>`_
+
+-------------------
 23.2.1 (2024-02-21)
 -------------------
 
 
 =========
 Bug fixes
 =========
```

### Comparing `galaxy-data-23.2.1/galaxy_data.egg-info/SOURCES.txt` & `galaxy-data-24.0.0/galaxy_data.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -241,19 +241,21 @@
 galaxy/model/migrations/exceptions.py
 galaxy/model/migrations/scripts.py
 galaxy/model/migrations/util.py
 galaxy/model/migrations/alembic/env.py
 galaxy/model/migrations/alembic/script.py.mako
 galaxy/model/migrations/alembic/versions_gxy/186d4835587b_drop_job_state_history_update_time_.py
 galaxy/model/migrations/alembic/versions_gxy/2d749563e1fe_add_notification_system_tables.py
+galaxy/model/migrations/alembic/versions_gxy/2dc3386d091f_add_indexes_for_workflow_comment_.py
 galaxy/model/migrations/alembic/versions_gxy/3100452fa030_add_workflow_invocation_message_table.py
 galaxy/model/migrations/alembic/versions_gxy/3356bc2ecfc4_drop_view.py
 galaxy/model/migrations/alembic/versions_gxy/3a2914d703ca_add_index_wf_r_s_s__workflow_invocation_.py
 galaxy/model/migrations/alembic/versions_gxy/460d0ecd1dd8_.py
 galaxy/model/migrations/alembic/versions_gxy/518c8438a91b_add_when_expression_column.py
+galaxy/model/migrations/alembic/versions_gxy/55f02fd8ab6c_add_index_on_hda_extension.py
 galaxy/model/migrations/alembic/versions_gxy/59e024ceaca1_add_export_association_table.py
 galaxy/model/migrations/alembic/versions_gxy/6a67bf27e6a6_deferred_data_tables.py
 galaxy/model/migrations/alembic/versions_gxy/8a19186a6ee7_add_columns_to_interactivetool_entry_point.py
 galaxy/model/migrations/alembic/versions_gxy/92fb564c7095_.py
 galaxy/model/migrations/alembic/versions_gxy/9540a051226e_preferred_object_store_ids.py
 galaxy/model/migrations/alembic/versions_gxy/987ce9839ecb_create_celery_user_rate_limit_table.py
 galaxy/model/migrations/alembic/versions_gxy/b182f655505f_add_workflow_source_metadata_column.py
```

### Comparing `galaxy-data-23.2.1/setup.cfg` & `galaxy-data-24.0.0/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -5,68 +5,69 @@
 	Development Status :: 5 - Production/Stable
 	Environment :: Console
 	Intended Audience :: Developers
 	License :: OSI Approved :: Academic Free License (AFL)
 	Natural Language :: English
 	Operating System :: POSIX
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Topic :: Software Development
 	Topic :: Software Development :: Code Generators
 	Topic :: Software Development :: Testing
 description = Galaxy datatype framework and datatypes
 keywords = 
 	Galaxy
 license = AFL
 license_files = 
 	LICENSE
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 name = galaxy-data
 url = https://github.com/galaxyproject/galaxy
-version = 23.2.1
+version = 24.0.0
 
 [options]
 include_package_data = True
 install_requires = 
 	galaxy-files
 	galaxy-objectstore
+	galaxy-tool-util
 	galaxy-util[template]
 	alembic
 	alembic-utils
-	bdbag
+	bdbag>=1.6.3
 	bx-python
 	dnspython
 	galaxy-sequence-utils
-	h5grove
+	h5grove>=1.2.1
 	h5py
-	isa-rwval
+	isa-rwval>=0.10.10
 	isal
 	MarkupSafe
 	msal
 	mrcfile
 	numpy
 	parsley
 	pycryptodome
-	pydantic[email]<2
+	pydantic[email]>=2,!=2.6.0,!=2.6.1
 	pylibmagic
 	python-magic
 	pysam>=0.21
 	rocrate
 	social-auth-core[openidconnect]==4.0.3
 	SQLAlchemy>=1.4.25,<2
 	tifffile
 	typing-extensions
 	WebOb
 packages = find:
-python_requires = >=3.7
+python_requires = >=3.8
 
 [options.entry_points]
 console_scripts = 
 	galaxy-build-objects = galaxy.model.store.build_objects:main
 	galaxy-load-objects = galaxy.model.store.load_objects:main
 	galaxy-manage-db = galaxy.model.orm.scripts:manage_db
```

