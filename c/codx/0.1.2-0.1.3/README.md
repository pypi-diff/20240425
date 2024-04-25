# Comparing `tmp/codx-0.1.2.tar.gz` & `tmp/codx-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codx-0.1.2.tar", max compression
+gzip compressed data, was "codx-0.1.3.tar", max compression
```

## Comparing `codx-0.1.2.tar` & `codx-0.1.3.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0       34 2023-04-03 16:59:53.943376 codx-0.1.2/codx/__init__.py
--rw-r--r--   0        0        0     2183 2023-04-03 16:59:53.949387 codx-0.1.2/codx/cli.py
--rw-r--r--   0        0        0    14309 2023-04-03 16:59:53.946381 codx-0.1.2/codx/components.py
--rw-r--r--   0        0        0      746 2023-04-03 16:10:12.901071 codx-0.1.2/codx/test_cli.py
--rw-r--r--   0        0        0     1451 2023-04-03 15:11:21.152744 codx-0.1.2/codx/test_components.py
--rw-r--r--   0        0        0     1088 2023-03-31 16:07:14.014611 codx-0.1.2/LICENSE
--rw-r--r--   0        0        0      575 2023-04-03 17:00:13.915290 codx-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3523 2023-04-03 15:27:48.063956 codx-0.1.2/README.md
--rw-r--r--   0        0        0     4372 1970-01-01 00:00:00.000000 codx-0.1.2/setup.py
--rw-r--r--   0        0        0     4136 1970-01-01 00:00:00.000000 codx-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       34 2023-04-03 16:59:54.000000 codx-0.1.3/codx/__init__.py
+-rw-r--r--   0        0        0     2183 2023-04-03 16:59:54.000000 codx-0.1.3/codx/cli.py
+-rw-r--r--   0        0        0    14309 2023-04-03 16:59:54.000000 codx-0.1.3/codx/components.py
+-rw-r--r--   0        0        0      746 2023-04-03 16:10:14.000000 codx-0.1.3/codx/test_cli.py
+-rw-r--r--   0        0        0     1451 2023-04-03 15:11:22.000000 codx-0.1.3/codx/test_components.py
+-rw-r--r--   0        0        0     1088 2023-03-31 16:07:16.000000 codx-0.1.3/LICENSE
+-rw-r--r--   0        0        0      606 2024-04-25 12:38:35.776480 codx-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3523 2023-04-03 15:27:50.000000 codx-0.1.3/README.md
+-rw-r--r--   0        0        0     4239 1970-01-01 00:00:00.000000 codx-0.1.3/PKG-INFO
```

### Comparing `codx-0.1.2/codx/cli.py` & `codx-0.1.3/codx/cli.py`

 * *Files identical despite different names*

### Comparing `codx-0.1.2/codx/components.py` & `codx-0.1.3/codx/components.py`

 * *Files identical despite different names*

### Comparing `codx-0.1.2/codx/test_cli.py` & `codx-0.1.3/codx/test_cli.py`

 * *Files identical despite different names*

### Comparing `codx-0.1.2/codx/test_components.py` & `codx-0.1.3/codx/test_components.py`

 * *Files identical despite different names*

### Comparing `codx-0.1.2/LICENSE` & `codx-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `codx-0.1.2/pyproject.toml` & `codx-0.1.3/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [tool.poetry]
 name = "codx"
-version = "0.1.2"
+version = "0.1.3"
 description = "A package used to retrieve exon for protein sequences from RefSeqGene database"
 authors = ["Toan Phung <toan.phungkhoiquoctoan@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 biopython = "^1.81"
-pandas = "^1.5.3"
+pandas = "^2.2.2"
 uniprotparser = "^1.0.9"
 click = "^8.1.3"
+django-admin-tools = "^0.9.3"
 
 [tool.poetry.scripts]
 codx = "codx.cli:main"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.2"
```

### Comparing `codx-0.1.2/README.md` & `codx-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `codx-0.1.2/setup.py` & `codx-0.1.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,107 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
-
-packages = \
-['codx']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['biopython>=1.81,<2.0',
- 'click>=8.1.3,<9.0.0',
- 'pandas>=1.5.3,<2.0.0',
- 'uniprotparser>=1.0.9,<2.0.0']
-
-entry_points = \
-{'console_scripts': ['codx = codx.cli:main']}
-
-setup_kwargs = {
-    'name': 'codx',
-    'version': '0.1.2',
-    'description': 'A package used to retrieve exon for protein sequences from RefSeqGene database',
-    'long_description': '# CODX\n---\n\n`codx` is a python package that allow retrieval of exons data from NCBI RefSeqGene database.\n\n## Installation\n\n```bash\npip install codx\n```\n\n## Usage Python Package\n---\nThe package uses gene id in order to retrieve exons data from NCBI RefSeqGene database. The gene id can be obtained from the Uniprot database using the accession id of the gene. The `get_geneids_from_uniprot` function can be used to obtain the gene id from RefSeqGene database of NCBI.\n\n\n```python\n# if you only have accession id, you must first use the get_geneids_from_uniprot function to get the gene id from Uniprot\nfrom codx.components import get_geneids_from_uniprot\n\ngene_ids = get_geneids_from_uniprot(["P35568", "P05019", "Q99490", "Q8NEJ0", "Q13322", "Q15323"])\n# the result will be a set of gene ids that can be obtained from the Uniprot database using the list of Uniprot accession above\n```\n\n\n\n```python\n# Import the create_db function to create a sqlite3 database with gene and exon data from NCBI\nfrom codx.components import create_db\n\n\n# 120892 is the gene id for LRRK2 gene\ndb = create_db(["120892"], entrez_email="your@email.com") # You need to provide an email address to use the NCBI API\n\n# From the database object, you can retrieve a gene object using its gene name\ngene = db.get_gene("LRRK2")\n\n# From the gene objects you can retrieve exons data from the blocks attribute each exon object has its start and end location as well as the associated sequence\nfor exon in gene.blocks:\n    print(exon.start, exon.end, exon.sequence)\n\n# Using the gene object it is also possible to create all possible ordered combinations of exons\n# This will be a generator object that yield a SeqRecord object for each combination\n# There however may be a lot of combinations so depending on the gene, you may not want to use this with a very large gene unless there are no other options\nfor exon_combination in gene.shuffle_blocks():\n    print(exon_combination)\n\n# To create six frame translation of any sequence, you can use the three_frame_translation function twice, one with and one without the reverse complement option enable\n# Each output is a dictionary with the translatable sequence as value and the frame as key\nfrom codx.components import three_frame_translation\nfor exon_combination in gene.shuffle_blocks():\n    three_frame = three_frame_translation(exon_combination.seq, only_start_at_atg=True)\n    three_frame_complement = three_frame_translation(exon_combination.seq, only_start_at_atg=True, reverse_complement=True)\n\n```\n\n## Usage Command Line\n---\nIn addition to the python API, installation also provide a cli interface that can be used for the same purpose\n\n\n```bash\nUsage: codx [OPTIONS] IDS\n\nOptions:\n  -o, --output TEXT              Output file\n  -i, --include-intron           Include intron\n  -u, --uniprot                  Input is Uniprot accession ids\n  -t, --translate                Translate to protein\n  -3, --three-frame-translation  Translate to protein in 3 frames\n  -6, --six-frame-translation    Translate to protein in 6 frames (3 forward\n                                 and 3 reverse complement)\n  --help                         Show this message and exit.\n```\n\nHere IDS positional argument are a list of gene ids or uniprot accession ids delimited by `,`.\n\nExample usage can be seen below\n\n```bash\ncodx -o output.fasta -u P35568,P05019,Q99490,Q8NEJ0,Q13322,Q15323\n```\n\n```bash\ncodx -o output.fasta 1190,120892\n```',
-    'author': 'Toan Phung',
-    'author_email': 'toan.phungkhoiquoctoan@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.9,<4.0',
-}
-
-
-setup(**setup_kwargs)
+Metadata-Version: 2.1
+Name: codx
+Version: 0.1.3
+Summary: A package used to retrieve exon for protein sequences from RefSeqGene database
+License: MIT
+Author: Toan Phung
+Author-email: toan.phungkhoiquoctoan@gmail.com
+Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: biopython (>=1.81,<2.0)
+Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: django-admin-tools (>=0.9.3,<0.10.0)
+Requires-Dist: pandas (>=2.2.2,<3.0.0)
+Requires-Dist: uniprotparser (>=1.0.9,<2.0.0)
+Description-Content-Type: text/markdown
+
+# CODX
+---
+
+`codx` is a python package that allow retrieval of exons data from NCBI RefSeqGene database.
+
+## Installation
+
+```bash
+pip install codx
+```
+
+## Usage Python Package
+---
+The package uses gene id in order to retrieve exons data from NCBI RefSeqGene database. The gene id can be obtained from the Uniprot database using the accession id of the gene. The `get_geneids_from_uniprot` function can be used to obtain the gene id from RefSeqGene database of NCBI.
+
+
+```python
+# if you only have accession id, you must first use the get_geneids_from_uniprot function to get the gene id from Uniprot
+from codx.components import get_geneids_from_uniprot
+
+gene_ids = get_geneids_from_uniprot(["P35568", "P05019", "Q99490", "Q8NEJ0", "Q13322", "Q15323"])
+# the result will be a set of gene ids that can be obtained from the Uniprot database using the list of Uniprot accession above
+```
+
+
+
+```python
+# Import the create_db function to create a sqlite3 database with gene and exon data from NCBI
+from codx.components import create_db
+
+
+# 120892 is the gene id for LRRK2 gene
+db = create_db(["120892"], entrez_email="your@email.com") # You need to provide an email address to use the NCBI API
+
+# From the database object, you can retrieve a gene object using its gene name
+gene = db.get_gene("LRRK2")
+
+# From the gene objects you can retrieve exons data from the blocks attribute each exon object has its start and end location as well as the associated sequence
+for exon in gene.blocks:
+    print(exon.start, exon.end, exon.sequence)
+
+# Using the gene object it is also possible to create all possible ordered combinations of exons
+# This will be a generator object that yield a SeqRecord object for each combination
+# There however may be a lot of combinations so depending on the gene, you may not want to use this with a very large gene unless there are no other options
+for exon_combination in gene.shuffle_blocks():
+    print(exon_combination)
+
+# To create six frame translation of any sequence, you can use the three_frame_translation function twice, one with and one without the reverse complement option enable
+# Each output is a dictionary with the translatable sequence as value and the frame as key
+from codx.components import three_frame_translation
+for exon_combination in gene.shuffle_blocks():
+    three_frame = three_frame_translation(exon_combination.seq, only_start_at_atg=True)
+    three_frame_complement = three_frame_translation(exon_combination.seq, only_start_at_atg=True, reverse_complement=True)
+
+```
+
+## Usage Command Line
+---
+In addition to the python API, installation also provide a cli interface that can be used for the same purpose
+
+
+```bash
+Usage: codx [OPTIONS] IDS
+
+Options:
+  -o, --output TEXT              Output file
+  -i, --include-intron           Include intron
+  -u, --uniprot                  Input is Uniprot accession ids
+  -t, --translate                Translate to protein
+  -3, --three-frame-translation  Translate to protein in 3 frames
+  -6, --six-frame-translation    Translate to protein in 6 frames (3 forward
+                                 and 3 reverse complement)
+  --help                         Show this message and exit.
+```
+
+Here IDS positional argument are a list of gene ids or uniprot accession ids delimited by `,`.
+
+Example usage can be seen below
+
+```bash
+codx -o output.fasta -u P35568,P05019,Q99490,Q8NEJ0,Q13322,Q15323
+```
+
+```bash
+codx -o output.fasta 1190,120892
+```
```

