# Comparing `tmp/biobear-0.19.6.tar.gz` & `tmp/biobear-0.20.0.tar.gz`

## Comparing `biobear-0.19.6.tar` & `biobear-0.20.0.tar`

### file list

```diff
@@ -1,101 +1,103 @@
--rw-r--r--   0        0        0      413 1970-01-01 00:00:00.000000 biobear-0.19.6/Cargo.toml
--rw-r--r--   0     1001      127       18 2024-04-24 17:01:59.000000 biobear-0.19.6/.github/FUNDING.yml
--rw-r--r--   0     1001      127     3295 2024-04-24 17:01:59.000000 biobear-0.19.6/.github/biobear.svg
--rw-r--r--   0     1001      127      100 2024-04-24 17:01:59.000000 biobear-0.19.6/.github/dependabot.yml
--rw-r--r--   0     1001      127     4104 2024-04-24 17:01:59.000000 biobear-0.19.6/.github/workflows/release.yml
--rw-r--r--   0     1001      127     1517 2024-04-24 17:01:59.000000 biobear-0.19.6/.github/workflows/smoke-test.yml
--rw-r--r--   0     1001      127      143 2024-04-24 17:01:59.000000 biobear-0.19.6/.github/workflows/smoketest.py
--rw-r--r--   0     1001      127     1160 2024-04-24 17:01:59.000000 biobear-0.19.6/.github/workflows/test.yml
--rw-r--r--   0     1001      127     4135 2024-04-24 17:01:59.000000 biobear-0.19.6/.gitignore
--rw-r--r--   0     1001      127     4395 2024-04-24 17:01:59.000000 biobear-0.19.6/CHANGELOG.md
--rw-r--r--   0     1001      127     1055 2024-04-24 17:01:59.000000 biobear-0.19.6/LICENSE
--rw-r--r--   0     1001      127      207 2024-04-24 17:01:59.000000 biobear-0.19.6/Makefile
--rw-r--r--   0     1001      127     7956 2024-04-24 17:01:59.000000 biobear-0.19.6/README.md
--rw-r--r--   0     1001      127      393 2024-04-24 17:01:59.000000 biobear-0.19.6/benchmarks/biobear-scan.py
--rw-r--r--   0     1001      127      467 2024-04-24 17:01:59.000000 biobear-0.19.6/benchmarks/biopython-scan.py
--rw-r--r--   0     1001      127      979 2024-04-24 17:01:59.000000 biobear-0.19.6/benchmarks/results.json
--rw-r--r--   0     1001      127     1569 2024-04-24 17:01:59.000000 biobear-0.19.6/bin/test.sh
--rw-r--r--   0     1001      127      285 2024-04-24 17:01:59.000000 biobear-0.19.6/cz.json
--rw-r--r--   0     1001      127      252 2024-04-24 17:01:59.000000 biobear-0.19.6/docs.bash
--rw-r--r--   0     1001      127     2587 2024-04-24 17:01:59.000000 biobear-0.19.6/python/biobear/__init__.py
--rw-r--r--   0     1001      127     2304 2024-04-24 17:01:59.000000 biobear-0.19.6/python/biobear/bam_reader.py
--rw-r--r--   0     1001      127     2087 2024-04-24 17:01:59.000000 biobear-0.19.6/python/biobear/bcf_reader.py
--rw-r--r--   0     1001      127     7914 2024-04-24 17:01:59.000000 biobear-0.19.6/python/biobear/biobear.pyi
--rw-r--r--   0     1001      127     1309 2024-04-24 17:01:59.000000 biobear-0.19.6/python/biobear/compression.py
--rw-r--r--   0     1001      127     1762 2024-04-24 17:01:59.000000 biobear-0.19.6/python/biobear/fasta_reader.py
--rw-r--r--   0     1001      127     1756 2024-04-24 17:01:59.000000 biobear-0.19.6/python/biobear/fastq_reader.py
--rw-r--r--   0     1001      127      858 2024-04-24 17:01:59.000000 biobear-0.19.6/python/biobear/genbank_reader.py
--rw-r--r--   0     1001      127     1564 2024-04-24 17:01:59.000000 biobear-0.19.6/python/biobear/gff_reader.py
--rw-r--r--   0     1001      127     1566 2024-04-24 17:01:59.000000 biobear-0.19.6/python/biobear/gtf_reader.py
--rw-r--r--   0     1001      127     1050 2024-04-24 17:01:59.000000 biobear-0.19.6/python/biobear/mzml_reader.py
--rw-r--r--   0     1001      127        0 2024-04-24 17:01:59.000000 biobear-0.19.6/python/biobear/py.typed
--rw-r--r--   0     1001      127     2910 2024-04-24 17:01:59.000000 biobear-0.19.6/python/biobear/reader.py
--rw-r--r--   0     1001      127     2129 2024-04-24 17:01:59.000000 biobear-0.19.6/python/biobear/vcf_reader.py
--rw-r--r--   0     1001      127   124562 2024-04-24 17:01:59.000000 biobear-0.19.6/python/tests/data/BGC0000404.gbk
--rw-r--r--   0     1001      127     6152 2024-04-24 17:01:59.000000 biobear-0.19.6/python/tests/data/bedcov.bam
--rw-r--r--   0     1001      127     7608 2024-04-24 17:01:59.000000 biobear-0.19.6/python/tests/data/bedcov.bam.bai
--rw-r--r--   0     1001      127      939 2024-04-24 17:01:59.000000 biobear-0.19.6/python/tests/data/cram/0500_mapped.cram
--rw-r--r--   0     1001      127     7275 2024-04-24 17:01:59.000000 biobear-0.19.6/python/tests/data/cram/1404_index_multislice.cram
--rw-r--r--   0     1001      127      156 2024-04-24 17:01:59.000000 biobear-0.19.6/python/tests/data/cram/1404_index_multislice.cram.crai
--rw-r--r--   0     1001      127  1060702 2024-04-24 17:01:59.000000 biobear-0.19.6/python/tests/data/cram/ce.fa
--rw-r--r--   0     1001      127      230 2024-04-24 17:01:59.000000 biobear-0.19.6/python/tests/data/cram/ce.fa.fai
--rw-r--r--   0     1001      127     3178 2024-04-24 17:01:59.000000 biobear-0.19.6/python/tests/data/cram/test_input_1_a.cram
--rw-r--r--   0     1001      127   339527 2024-04-24 17:01:59.000000 biobear-0.19.6/python/tests/data/fake_fastq_file.fastq.gz
--rw-r--r--   0     1001      127     1749 2024-04-24 17:01:59.000000 biobear-0.19.6/python/tests/data/file.vcf
--rw-r--r--   0     1001      127     9521 2024-04-24 17:01:59.000000 biobear-0.19.6/python/tests/data/index.bcf
--rw-r--r--   0     1001      127      143 2024-04-24 17:01:59.000000 biobear-0.19.6/python/tests/data/index.bcf.csi
--rw-r--r--   0     1001      127     8638 2024-04-24 17:01:59.000000 biobear-0.19.6/python/tests/data/index.vcf.gz
--rw-r--r--   0     1001      127      213 2024-04-24 17:01:59.000000 biobear-0.19.6/python/tests/data/index.vcf.gz.tbi
--rw-r--r--   0     1001      127       41 2024-04-24 17:01:59.000000 biobear-0.19.6/python/tests/data/test.fa
--rw-r--r--   0     1001      127       55 2024-04-24 17:01:59.000000 biobear-0.19.6/python/tests/data/test.fa.gz
--rw-r--r--   0     1001      127       41 2024-04-24 17:01:59.000000 biobear-0.19.6/python/tests/data/test.fasta
--rw-r--r--   0     1001      127       22 2024-04-24 17:01:59.000000 biobear-0.19.6/python/tests/data/test.fasta.fai
--rw-r--r--   0     1001      127       58 2024-04-24 17:01:59.000000 biobear-0.19.6/python/tests/data/test.fasta.gz
--rw-r--r--   0     1001      127      286 2024-04-24 17:01:59.000000 biobear-0.19.6/python/tests/data/test.fastq
--rw-r--r--   0     1001      127      134 2024-04-24 17:01:59.000000 biobear-0.19.6/python/tests/data/test.fastq.gz
--rw-r--r--   0     1001      127      286 2024-04-24 17:01:59.000000 biobear-0.19.6/python/tests/data/test.fq
--rw-r--r--   0     1001      127      156 2024-04-24 17:01:59.000000 biobear-0.19.6/python/tests/data/test.fq.gz
--rw-r--r--   0     1001      127      112 2024-04-24 17:01:59.000000 biobear-0.19.6/python/tests/data/test.gff
--rw-r--r--   0     1001      127       91 2024-04-24 17:01:59.000000 biobear-0.19.6/python/tests/data/test.gff.gz
--rw-r--r--   0     1001      127    17994 2024-04-24 17:01:59.000000 biobear-0.19.6/python/tests/data/test.gtf
--rw-r--r--   0     1001      127     1478 2024-04-24 17:01:59.000000 biobear-0.19.6/python/tests/data/test.gtf.gz
--rw-r--r--   0     1001      127    17171 2024-04-24 17:01:59.000000 biobear-0.19.6/python/tests/data/test.mzML
--rw-r--r--   0     1001      127     2845 2024-04-24 17:01:59.000000 biobear-0.19.6/python/tests/data/test.mzML.gz
--rw-r--r--   0     1001      127     1025 2024-04-24 17:01:59.000000 biobear-0.19.6/python/tests/data/two-cram/rand1k.fa
--rw-r--r--   0     1001      127       20 2024-04-24 17:01:59.000000 biobear-0.19.6/python/tests/data/two-cram/rand1k.fa.fai
--rw-r--r--   0     1001      127     1029 2024-04-24 17:01:59.000000 biobear-0.19.6/python/tests/data/two-cram/twolib.sorted.cram
--rw-r--r--   0     1001      127       42 2024-04-24 17:01:59.000000 biobear-0.19.6/python/tests/data/two-cram/twolib.sorted.cram.crai
--rw-r--r--   0     1001      127     4302 2024-04-24 17:01:59.000000 biobear-0.19.6/python/tests/data/vcf_file.vcf
--rw-r--r--   0     1001      127     1669 2024-04-24 17:01:59.000000 biobear-0.19.6/python/tests/data/vcf_file.vcf.gz
--rw-r--r--   0     1001      127      254 2024-04-24 17:01:59.000000 biobear-0.19.6/python/tests/data/vcf_file.vcf.gz.tbi
--rw-r--r--   0     1001      127    13705 2024-04-24 17:01:59.000000 biobear-0.19.6/python/tests/test_session.py
--rw-r--r--   0     1001      127       47 2024-04-24 17:01:59.000000 biobear-0.19.6/requirements-dev.txt
--rw-r--r--   0     1001      127     3705 2024-04-24 17:01:59.000000 biobear-0.19.6/src/bam_reader.rs
--rw-r--r--   0     1001      127     3590 2024-04-24 17:01:59.000000 biobear-0.19.6/src/bcf_reader.rs
--rw-r--r--   0     1001      127     1397 2024-04-24 17:01:59.000000 biobear-0.19.6/src/datasources/bam.rs
--rw-r--r--   0     1001      127     1631 2024-04-24 17:01:59.000000 biobear-0.19.6/src/datasources/bcf.rs
--rw-r--r--   0     1001      127     1561 2024-04-24 17:01:59.000000 biobear-0.19.6/src/datasources/bed.rs
--rw-r--r--   0     1001      127     2572 2024-04-24 17:01:59.000000 biobear-0.19.6/src/datasources/bigwig.rs
--rw-r--r--   0     1001      127     1548 2024-04-24 17:01:59.000000 biobear-0.19.6/src/datasources/cram.rs
--rw-r--r--   0     1001      127     3265 2024-04-24 17:01:59.000000 biobear-0.19.6/src/datasources/fasta.rs
--rw-r--r--   0     1001      127     3322 2024-04-24 17:01:59.000000 biobear-0.19.6/src/datasources/fastq.rs
--rw-r--r--   0     1001      127     1353 2024-04-24 17:01:59.000000 biobear-0.19.6/src/datasources/fcs.rs
--rw-r--r--   0     1001      127     1380 2024-04-24 17:01:59.000000 biobear-0.19.6/src/datasources/genbank.rs
--rw-r--r--   0     1001      127     1913 2024-04-24 17:01:59.000000 biobear-0.19.6/src/datasources/gff.rs
--rw-r--r--   0     1001      127     1476 2024-04-24 17:01:59.000000 biobear-0.19.6/src/datasources/gtf.rs
--rw-r--r--   0     1001      127     1322 2024-04-24 17:01:59.000000 biobear-0.19.6/src/datasources/hmm_dom_tab.rs
--rw-r--r--   0     1001      127     1224 2024-04-24 17:01:59.000000 biobear-0.19.6/src/datasources/mod.rs
--rw-r--r--   0     1001      127     1517 2024-04-24 17:01:59.000000 biobear-0.19.6/src/datasources/mzml.rs
--rw-r--r--   0     1001      127     1071 2024-04-24 17:01:59.000000 biobear-0.19.6/src/datasources/sam.rs
--rw-r--r--   0     1001      127     2036 2024-04-24 17:01:59.000000 biobear-0.19.6/src/datasources/vcf.rs
--rw-r--r--   0     1001      127     2618 2024-04-24 17:01:59.000000 biobear-0.19.6/src/error.rs
--rw-r--r--   0     1001      127     4174 2024-04-24 17:01:59.000000 biobear-0.19.6/src/execution_result.rs
--rw-r--r--   0     1001      127     3784 2024-04-24 17:01:59.000000 biobear-0.19.6/src/exon_reader.rs
--rw-r--r--   0     1001      127     3225 2024-04-24 17:01:59.000000 biobear-0.19.6/src/file_compression_type.rs
--rw-r--r--   0     1001      127     2706 2024-04-24 17:01:59.000000 biobear-0.19.6/src/lib.rs
--rw-r--r--   0     1001      127     1253 2024-04-24 17:01:59.000000 biobear-0.19.6/src/runtime.rs
--rw-r--r--   0     1001      127     9978 2024-04-24 17:01:59.000000 biobear-0.19.6/src/session_context.rs
--rw-r--r--   0     1001      127     3752 2024-04-24 17:01:59.000000 biobear-0.19.6/src/vcf_reader.rs
--rw-r--r--   0     1001      127   110055 2024-04-24 17:02:05.000000 biobear-0.19.6/Cargo.lock
--rw-r--r--   0     1001      127      725 2024-04-24 17:01:59.000000 biobear-0.19.6/pyproject.toml
--rw-r--r--   0        0        0     8469 1970-01-01 00:00:00.000000 biobear-0.19.6/PKG-INFO
+-rw-r--r--   0        0        0      411 1970-01-01 00:00:00.000000 biobear-0.20.0/Cargo.toml
+-rw-r--r--   0     1001      127       18 2024-04-24 22:21:12.000000 biobear-0.20.0/.github/FUNDING.yml
+-rw-r--r--   0     1001      127     3295 2024-04-24 22:21:12.000000 biobear-0.20.0/.github/biobear.svg
+-rw-r--r--   0     1001      127      100 2024-04-24 22:21:12.000000 biobear-0.20.0/.github/dependabot.yml
+-rw-r--r--   0     1001      127     4104 2024-04-24 22:21:12.000000 biobear-0.20.0/.github/workflows/release.yml
+-rw-r--r--   0     1001      127     1517 2024-04-24 22:21:12.000000 biobear-0.20.0/.github/workflows/smoke-test.yml
+-rw-r--r--   0     1001      127      143 2024-04-24 22:21:12.000000 biobear-0.20.0/.github/workflows/smoketest.py
+-rw-r--r--   0     1001      127     1160 2024-04-24 22:21:12.000000 biobear-0.20.0/.github/workflows/test.yml
+-rw-r--r--   0     1001      127     4135 2024-04-24 22:21:12.000000 biobear-0.20.0/.gitignore
+-rw-r--r--   0     1001      127     4466 2024-04-24 22:21:12.000000 biobear-0.20.0/CHANGELOG.md
+-rw-r--r--   0     1001      127     1055 2024-04-24 22:21:12.000000 biobear-0.20.0/LICENSE
+-rw-r--r--   0     1001      127      207 2024-04-24 22:21:12.000000 biobear-0.20.0/Makefile
+-rw-r--r--   0     1001      127     7956 2024-04-24 22:21:12.000000 biobear-0.20.0/README.md
+-rw-r--r--   0     1001      127      393 2024-04-24 22:21:12.000000 biobear-0.20.0/benchmarks/biobear-scan.py
+-rw-r--r--   0     1001      127      467 2024-04-24 22:21:12.000000 biobear-0.20.0/benchmarks/biopython-scan.py
+-rw-r--r--   0     1001      127      979 2024-04-24 22:21:12.000000 biobear-0.20.0/benchmarks/results.json
+-rw-r--r--   0     1001      127     1569 2024-04-24 22:21:12.000000 biobear-0.20.0/bin/test.sh
+-rw-r--r--   0     1001      127      285 2024-04-24 22:21:12.000000 biobear-0.20.0/cz.json
+-rw-r--r--   0     1001      127      252 2024-04-24 22:21:12.000000 biobear-0.20.0/docs.bash
+-rw-r--r--   0     1001      127     2587 2024-04-24 22:21:12.000000 biobear-0.20.0/python/biobear/__init__.py
+-rw-r--r--   0     1001      127     2304 2024-04-24 22:21:12.000000 biobear-0.20.0/python/biobear/bam_reader.py
+-rw-r--r--   0     1001      127     2087 2024-04-24 22:21:12.000000 biobear-0.20.0/python/biobear/bcf_reader.py
+-rw-r--r--   0     1001      127     7988 2024-04-24 22:21:12.000000 biobear-0.20.0/python/biobear/biobear.pyi
+-rw-r--r--   0     1001      127     1309 2024-04-24 22:21:12.000000 biobear-0.20.0/python/biobear/compression.py
+-rw-r--r--   0     1001      127     1762 2024-04-24 22:21:12.000000 biobear-0.20.0/python/biobear/fasta_reader.py
+-rw-r--r--   0     1001      127     1756 2024-04-24 22:21:12.000000 biobear-0.20.0/python/biobear/fastq_reader.py
+-rw-r--r--   0     1001      127      858 2024-04-24 22:21:12.000000 biobear-0.20.0/python/biobear/genbank_reader.py
+-rw-r--r--   0     1001      127     1564 2024-04-24 22:21:12.000000 biobear-0.20.0/python/biobear/gff_reader.py
+-rw-r--r--   0     1001      127     1566 2024-04-24 22:21:12.000000 biobear-0.20.0/python/biobear/gtf_reader.py
+-rw-r--r--   0     1001      127     1050 2024-04-24 22:21:12.000000 biobear-0.20.0/python/biobear/mzml_reader.py
+-rw-r--r--   0     1001      127        0 2024-04-24 22:21:12.000000 biobear-0.20.0/python/biobear/py.typed
+-rw-r--r--   0     1001      127     2910 2024-04-24 22:21:12.000000 biobear-0.20.0/python/biobear/reader.py
+-rw-r--r--   0     1001      127     2129 2024-04-24 22:21:12.000000 biobear-0.20.0/python/biobear/vcf_reader.py
+-rw-r--r--   0     1001      127   124562 2024-04-24 22:21:12.000000 biobear-0.20.0/python/tests/data/BGC0000404.gbk
+-rw-r--r--   0     1001      127     6152 2024-04-24 22:21:12.000000 biobear-0.20.0/python/tests/data/bedcov.bam
+-rw-r--r--   0     1001      127     7608 2024-04-24 22:21:12.000000 biobear-0.20.0/python/tests/data/bedcov.bam.bai
+-rw-r--r--   0     1001      127      939 2024-04-24 22:21:12.000000 biobear-0.20.0/python/tests/data/cram/0500_mapped.cram
+-rw-r--r--   0     1001      127     7275 2024-04-24 22:21:12.000000 biobear-0.20.0/python/tests/data/cram/1404_index_multislice.cram
+-rw-r--r--   0     1001      127      156 2024-04-24 22:21:12.000000 biobear-0.20.0/python/tests/data/cram/1404_index_multislice.cram.crai
+-rw-r--r--   0     1001      127  1060702 2024-04-24 22:21:12.000000 biobear-0.20.0/python/tests/data/cram/ce.fa
+-rw-r--r--   0     1001      127      230 2024-04-24 22:21:12.000000 biobear-0.20.0/python/tests/data/cram/ce.fa.fai
+-rw-r--r--   0     1001      127     3178 2024-04-24 22:21:12.000000 biobear-0.20.0/python/tests/data/cram/test_input_1_a.cram
+-rw-r--r--   0     1001      127   339527 2024-04-24 22:21:12.000000 biobear-0.20.0/python/tests/data/fake_fastq_file.fastq.gz
+-rw-r--r--   0     1001      127     1749 2024-04-24 22:21:12.000000 biobear-0.20.0/python/tests/data/file.vcf
+-rw-r--r--   0     1001      127     9521 2024-04-24 22:21:12.000000 biobear-0.20.0/python/tests/data/index.bcf
+-rw-r--r--   0     1001      127      143 2024-04-24 22:21:12.000000 biobear-0.20.0/python/tests/data/index.bcf.csi
+-rw-r--r--   0     1001      127     8638 2024-04-24 22:21:12.000000 biobear-0.20.0/python/tests/data/index.vcf.gz
+-rw-r--r--   0     1001      127      213 2024-04-24 22:21:12.000000 biobear-0.20.0/python/tests/data/index.vcf.gz.tbi
+-rw-r--r--   0     1001      127       41 2024-04-24 22:21:12.000000 biobear-0.20.0/python/tests/data/test.fa
+-rw-r--r--   0     1001      127       55 2024-04-24 22:21:12.000000 biobear-0.20.0/python/tests/data/test.fa.gz
+-rw-r--r--   0     1001      127       41 2024-04-24 22:21:12.000000 biobear-0.20.0/python/tests/data/test.fasta
+-rw-r--r--   0     1001      127       22 2024-04-24 22:21:12.000000 biobear-0.20.0/python/tests/data/test.fasta.fai
+-rw-r--r--   0     1001      127       58 2024-04-24 22:21:12.000000 biobear-0.20.0/python/tests/data/test.fasta.gz
+-rw-r--r--   0     1001      127      286 2024-04-24 22:21:12.000000 biobear-0.20.0/python/tests/data/test.fastq
+-rw-r--r--   0     1001      127      134 2024-04-24 22:21:12.000000 biobear-0.20.0/python/tests/data/test.fastq.gz
+-rw-r--r--   0     1001      127      286 2024-04-24 22:21:12.000000 biobear-0.20.0/python/tests/data/test.fq
+-rw-r--r--   0     1001      127      156 2024-04-24 22:21:12.000000 biobear-0.20.0/python/tests/data/test.fq.gz
+-rw-r--r--   0     1001      127      112 2024-04-24 22:21:12.000000 biobear-0.20.0/python/tests/data/test.gff
+-rw-r--r--   0     1001      127       91 2024-04-24 22:21:12.000000 biobear-0.20.0/python/tests/data/test.gff.gz
+-rw-r--r--   0     1001      127    17994 2024-04-24 22:21:12.000000 biobear-0.20.0/python/tests/data/test.gtf
+-rw-r--r--   0     1001      127     1478 2024-04-24 22:21:12.000000 biobear-0.20.0/python/tests/data/test.gtf.gz
+-rw-r--r--   0     1001      127    17171 2024-04-24 22:21:12.000000 biobear-0.20.0/python/tests/data/test.mzML
+-rw-r--r--   0     1001      127     2845 2024-04-24 22:21:12.000000 biobear-0.20.0/python/tests/data/test.mzML.gz
+-rw-r--r--   0     1001      127     1025 2024-04-24 22:21:12.000000 biobear-0.20.0/python/tests/data/two-cram/rand1k.fa
+-rw-r--r--   0     1001      127       20 2024-04-24 22:21:12.000000 biobear-0.20.0/python/tests/data/two-cram/rand1k.fa.fai
+-rw-r--r--   0     1001      127     1029 2024-04-24 22:21:12.000000 biobear-0.20.0/python/tests/data/two-cram/twolib.sorted.cram
+-rw-r--r--   0     1001      127       42 2024-04-24 22:21:12.000000 biobear-0.20.0/python/tests/data/two-cram/twolib.sorted.cram.crai
+-rw-r--r--   0     1001      127     1669 2024-04-24 22:21:12.000000 biobear-0.20.0/python/tests/data/vcf-partition/sample=1/vcf_file.vcf.gz
+-rw-r--r--   0     1001      127      254 2024-04-24 22:21:12.000000 biobear-0.20.0/python/tests/data/vcf-partition/sample=1/vcf_file.vcf.gz.tbi
+-rw-r--r--   0     1001      127     4302 2024-04-24 22:21:12.000000 biobear-0.20.0/python/tests/data/vcf_file.vcf
+-rw-r--r--   0     1001      127     1669 2024-04-24 22:21:12.000000 biobear-0.20.0/python/tests/data/vcf_file.vcf.gz
+-rw-r--r--   0     1001      127      254 2024-04-24 22:21:12.000000 biobear-0.20.0/python/tests/data/vcf_file.vcf.gz.tbi
+-rw-r--r--   0     1001      127    14881 2024-04-24 22:21:12.000000 biobear-0.20.0/python/tests/test_session.py
+-rw-r--r--   0     1001      127       47 2024-04-24 22:21:12.000000 biobear-0.20.0/requirements-dev.txt
+-rw-r--r--   0     1001      127     3705 2024-04-24 22:21:12.000000 biobear-0.20.0/src/bam_reader.rs
+-rw-r--r--   0     1001      127     3590 2024-04-24 22:21:12.000000 biobear-0.20.0/src/bcf_reader.rs
+-rw-r--r--   0     1001      127     1397 2024-04-24 22:21:12.000000 biobear-0.20.0/src/datasources/bam.rs
+-rw-r--r--   0     1001      127     1631 2024-04-24 22:21:12.000000 biobear-0.20.0/src/datasources/bcf.rs
+-rw-r--r--   0     1001      127     1561 2024-04-24 22:21:12.000000 biobear-0.20.0/src/datasources/bed.rs
+-rw-r--r--   0     1001      127     2572 2024-04-24 22:21:12.000000 biobear-0.20.0/src/datasources/bigwig.rs
+-rw-r--r--   0     1001      127     1548 2024-04-24 22:21:12.000000 biobear-0.20.0/src/datasources/cram.rs
+-rw-r--r--   0     1001      127     3265 2024-04-24 22:21:12.000000 biobear-0.20.0/src/datasources/fasta.rs
+-rw-r--r--   0     1001      127     3322 2024-04-24 22:21:12.000000 biobear-0.20.0/src/datasources/fastq.rs
+-rw-r--r--   0     1001      127     1353 2024-04-24 22:21:12.000000 biobear-0.20.0/src/datasources/fcs.rs
+-rw-r--r--   0     1001      127     1380 2024-04-24 22:21:12.000000 biobear-0.20.0/src/datasources/genbank.rs
+-rw-r--r--   0     1001      127     1913 2024-04-24 22:21:12.000000 biobear-0.20.0/src/datasources/gff.rs
+-rw-r--r--   0     1001      127     1476 2024-04-24 22:21:12.000000 biobear-0.20.0/src/datasources/gtf.rs
+-rw-r--r--   0     1001      127     1322 2024-04-24 22:21:12.000000 biobear-0.20.0/src/datasources/hmm_dom_tab.rs
+-rw-r--r--   0     1001      127     1224 2024-04-24 22:21:12.000000 biobear-0.20.0/src/datasources/mod.rs
+-rw-r--r--   0     1001      127     1517 2024-04-24 22:21:12.000000 biobear-0.20.0/src/datasources/mzml.rs
+-rw-r--r--   0     1001      127     1071 2024-04-24 22:21:12.000000 biobear-0.20.0/src/datasources/sam.rs
+-rw-r--r--   0     1001      127     2839 2024-04-24 22:21:12.000000 biobear-0.20.0/src/datasources/vcf.rs
+-rw-r--r--   0     1001      127     2618 2024-04-24 22:21:12.000000 biobear-0.20.0/src/error.rs
+-rw-r--r--   0     1001      127     4185 2024-04-24 22:21:12.000000 biobear-0.20.0/src/execution_result.rs
+-rw-r--r--   0     1001      127     3784 2024-04-24 22:21:12.000000 biobear-0.20.0/src/exon_reader.rs
+-rw-r--r--   0     1001      127     3225 2024-04-24 22:21:12.000000 biobear-0.20.0/src/file_compression_type.rs
+-rw-r--r--   0     1001      127     2706 2024-04-24 22:21:12.000000 biobear-0.20.0/src/lib.rs
+-rw-r--r--   0     1001      127     1253 2024-04-24 22:21:12.000000 biobear-0.20.0/src/runtime.rs
+-rw-r--r--   0     1001      127     9978 2024-04-24 22:21:12.000000 biobear-0.20.0/src/session_context.rs
+-rw-r--r--   0     1001      127     3752 2024-04-24 22:21:12.000000 biobear-0.20.0/src/vcf_reader.rs
+-rw-r--r--   0     1001      127   110055 2024-04-24 22:21:18.000000 biobear-0.20.0/Cargo.lock
+-rw-r--r--   0     1001      127      725 2024-04-24 22:21:12.000000 biobear-0.20.0/pyproject.toml
+-rw-r--r--   0        0        0     8469 1970-01-01 00:00:00.000000 biobear-0.20.0/PKG-INFO
```

### Comparing `biobear-0.19.6/.github/biobear.svg` & `biobear-0.20.0/.github/biobear.svg`

 * *Files identical despite different names*

### Comparing `biobear-0.19.6/.github/workflows/release.yml` & `biobear-0.20.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `biobear-0.19.6/.github/workflows/smoke-test.yml` & `biobear-0.20.0/.github/workflows/smoke-test.yml`

 * *Files identical despite different names*

### Comparing `biobear-0.19.6/.github/workflows/test.yml` & `biobear-0.20.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `biobear-0.19.6/.gitignore` & `biobear-0.20.0/.gitignore`

 * *Files identical despite different names*

### Comparing `biobear-0.19.6/CHANGELOG.md` & `biobear-0.20.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## v0.20.0 (2024-04-24)
+
+### Feat
+
+- improve vcf table options (#128)
+
 ## v0.19.6 (2024-04-24)
 
 ### Fix
 
 - better annotations
 
 ## v0.19.5 (2024-04-23)
```

### Comparing `biobear-0.19.6/LICENSE` & `biobear-0.20.0/LICENSE`

 * *Files identical despite different names*

### Comparing `biobear-0.19.6/README.md` & `biobear-0.20.0/README.md`

 * *Files identical despite different names*

### Comparing `biobear-0.19.6/benchmarks/results.json` & `biobear-0.20.0/benchmarks/results.json`

 * *Files identical despite different names*

### Comparing `biobear-0.19.6/bin/test.sh` & `biobear-0.20.0/bin/test.sh`

 * *Files identical despite different names*

### Comparing `biobear-0.19.6/python/biobear/__init__.py` & `biobear-0.20.0/python/biobear/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 from .biobear import FCSReadOptions
 from .biobear import CRAMReadOptions
 from .biobear import connect
 from .biobear import new_session
 from .biobear import __runtime
 
 
-__version__ = "0.19.6"
+__version__ = "0.20.0"
 
 __all__ = [
     "FastaReader",
     "FastqReader",
     "VCFReader",
     "VCFIndexedReader",
     "BamReader",
```

### Comparing `biobear-0.19.6/python/biobear/bam_reader.py` & `biobear-0.20.0/python/biobear/bam_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.19.6/python/biobear/bcf_reader.py` & `biobear-0.20.0/python/biobear/bcf_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.19.6/python/biobear/biobear.pyi` & `biobear-0.20.0/python/biobear/biobear.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -100,16 +100,18 @@
 
 class VCFReadOptions:
     """Options for reading VCF data."""
     def __init__(
         self,
         /,
         region: Optional[str] = None,
-        file_extension: Optional[str] = None,
         file_compression_type: Optional[FileCompressionType] = None,
+        parse_info: bool = False,
+        parse_formats: bool = False,
+        partition_cols: list[str | None] = None,
     ) -> None: ...
 
 class BCFReadOptions:
     """Options for reading BCF data."""
     def __init__(
         self,
         /,
```

### Comparing `biobear-0.19.6/python/biobear/compression.py` & `biobear-0.20.0/python/biobear/compression.py`

 * *Files identical despite different names*

### Comparing `biobear-0.19.6/python/biobear/fasta_reader.py` & `biobear-0.20.0/python/biobear/fasta_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.19.6/python/biobear/fastq_reader.py` & `biobear-0.20.0/python/biobear/fastq_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.19.6/python/biobear/genbank_reader.py` & `biobear-0.20.0/python/biobear/genbank_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.19.6/python/biobear/gff_reader.py` & `biobear-0.20.0/python/biobear/gff_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.19.6/python/biobear/gtf_reader.py` & `biobear-0.20.0/python/biobear/gtf_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.19.6/python/biobear/mzml_reader.py` & `biobear-0.20.0/python/biobear/mzml_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.19.6/python/biobear/reader.py` & `biobear-0.20.0/python/biobear/reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.19.6/python/biobear/vcf_reader.py` & `biobear-0.20.0/python/biobear/vcf_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.19.6/python/tests/data/BGC0000404.gbk` & `biobear-0.20.0/python/tests/data/BGC0000404.gbk`

 * *Files identical despite different names*

### Comparing `biobear-0.19.6/python/tests/data/bedcov.bam` & `biobear-0.20.0/python/tests/data/bedcov.bam`

 * *Files identical despite different names*

### Comparing `biobear-0.19.6/python/tests/data/bedcov.bam.bai` & `biobear-0.20.0/python/tests/data/bedcov.bam.bai`

 * *Files identical despite different names*

### Comparing `biobear-0.19.6/python/tests/data/cram/0500_mapped.cram` & `biobear-0.20.0/python/tests/data/cram/0500_mapped.cram`

 * *Files identical despite different names*

### Comparing `biobear-0.19.6/python/tests/data/cram/1404_index_multislice.cram` & `biobear-0.20.0/python/tests/data/cram/1404_index_multislice.cram`

 * *Files identical despite different names*

### Comparing `biobear-0.19.6/python/tests/data/cram/ce.fa` & `biobear-0.20.0/python/tests/data/cram/ce.fa`

 * *Files identical despite different names*

### Comparing `biobear-0.19.6/python/tests/data/cram/test_input_1_a.cram` & `biobear-0.20.0/python/tests/data/cram/test_input_1_a.cram`

 * *Files identical despite different names*

### Comparing `biobear-0.19.6/python/tests/data/fake_fastq_file.fastq.gz` & `biobear-0.20.0/python/tests/data/fake_fastq_file.fastq.gz`

 * *Files identical despite different names*

### Comparing `biobear-0.19.6/python/tests/data/file.vcf` & `biobear-0.20.0/python/tests/data/file.vcf`

 * *Files identical despite different names*

### Comparing `biobear-0.19.6/python/tests/data/index.bcf` & `biobear-0.20.0/python/tests/data/index.bcf`

 * *Files identical despite different names*

### Comparing `biobear-0.19.6/python/tests/data/index.vcf.gz` & `biobear-0.20.0/python/tests/data/index.vcf.gz`

 * *Files identical despite different names*

### Comparing `biobear-0.19.6/python/tests/data/test.gtf` & `biobear-0.20.0/python/tests/data/test.gtf`

 * *Files identical despite different names*

### Comparing `biobear-0.19.6/python/tests/data/test.gtf.gz` & `biobear-0.20.0/python/tests/data/test.gtf.gz`

 * *Files identical despite different names*

### Comparing `biobear-0.19.6/python/tests/data/test.mzML` & `biobear-0.20.0/python/tests/data/test.mzML`

 * *Files identical despite different names*

### Comparing `biobear-0.19.6/python/tests/data/test.mzML.gz` & `biobear-0.20.0/python/tests/data/test.mzML.gz`

 * *Files identical despite different names*

### Comparing `biobear-0.19.6/python/tests/data/two-cram/rand1k.fa` & `biobear-0.20.0/python/tests/data/two-cram/rand1k.fa`

 * *Files identical despite different names*

### Comparing `biobear-0.19.6/python/tests/data/two-cram/twolib.sorted.cram` & `biobear-0.20.0/python/tests/data/two-cram/twolib.sorted.cram`

 * *Files identical despite different names*

### Comparing `biobear-0.19.6/python/tests/data/vcf_file.vcf` & `biobear-0.20.0/python/tests/data/vcf_file.vcf`

 * *Files identical despite different names*

### Comparing `biobear-0.19.6/python/tests/data/vcf_file.vcf.gz` & `biobear-0.20.0/python/tests/data/vcf-partition/sample=1/vcf_file.vcf.gz`

 * *Files identical despite different names*

### Comparing `biobear-0.19.6/python/tests/test_session.py` & `biobear-0.20.0/python/tests/test_session.py`

 * *Files 5% similar despite different names*

```diff
@@ -337,14 +337,64 @@
     df = session.read_vcf_file(
         (DATA / "vcf_file.vcf").as_posix(), options=options
     ).to_polars()
 
     assert len(df) == 15
 
 
+@pytest.mark.skipif(
+    not importlib.util.find_spec("polars"), reason="polars not installed"
+)
+def test_vcf_reader_with_parsing():
+    session = new_session()
+    options = VCFReadOptions(parse_formats=True, parse_info=True)
+
+    df = session.read_vcf_file(
+        (DATA / "vcf_file.vcf").as_posix(), options=options
+    ).to_polars()
+
+    # Check that this is a struct, with three fields
+    assert len(df.get_column("info").dtype.fields) == 6
+    assert len(df) == 15
+
+
+def test_vcf_query_with_region_and_partition():
+    session = connect()
+    options = VCFReadOptions(
+        region="1",
+        file_compression_type=FileCompressionType.GZIP,
+        parse_formats=True,
+        parse_info=True,
+        partition_cols=["sample"],
+    )
+
+    rbr = session.read_vcf_file(
+        (DATA / "vcf-partition").as_posix(), options=options
+    ).to_arrow_record_batch_reader()
+
+    batch = next(rbr)
+
+    assert batch.column_names == [
+        "chrom",
+        "pos",
+        "id",
+        "ref",
+        "alt",
+        "qual",
+        "filter",
+        "info",
+        "formats",
+        "sample",
+    ]
+
+    batch.schema.field("sample")
+
+    assert 11 == batch.num_rows
+
+
 def test_vcf_query():
     session = connect()
     options = VCFReadOptions(region="1", file_compression_type=FileCompressionType.GZIP)
 
     rbr = session.read_vcf_file(
         (DATA / "vcf_file.vcf.gz").as_posix(), options=options
     ).to_arrow_record_batch_reader()
```

### Comparing `biobear-0.19.6/src/bam_reader.rs` & `biobear-0.20.0/src/bam_reader.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.19.6/src/bcf_reader.rs` & `biobear-0.20.0/src/bcf_reader.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.19.6/src/datasources/bam.rs` & `biobear-0.20.0/src/datasources/bam.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.19.6/src/datasources/bcf.rs` & `biobear-0.20.0/src/datasources/bcf.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.19.6/src/datasources/bed.rs` & `biobear-0.20.0/src/datasources/bed.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.19.6/src/datasources/bigwig.rs` & `biobear-0.20.0/src/datasources/bigwig.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.19.6/src/datasources/cram.rs` & `biobear-0.20.0/src/datasources/cram.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.19.6/src/datasources/fasta.rs` & `biobear-0.20.0/src/datasources/fasta.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.19.6/src/datasources/fastq.rs` & `biobear-0.20.0/src/datasources/fastq.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.19.6/src/datasources/fcs.rs` & `biobear-0.20.0/src/datasources/fcs.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.19.6/src/datasources/genbank.rs` & `biobear-0.20.0/src/datasources/genbank.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.19.6/src/datasources/gff.rs` & `biobear-0.20.0/src/datasources/gff.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.19.6/src/datasources/gtf.rs` & `biobear-0.20.0/src/datasources/gtf.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.19.6/src/datasources/hmm_dom_tab.rs` & `biobear-0.20.0/src/datasources/hmm_dom_tab.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.19.6/src/datasources/mod.rs` & `biobear-0.20.0/src/datasources/mod.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.19.6/src/datasources/mzml.rs` & `biobear-0.20.0/src/datasources/mzml.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.19.6/src/datasources/sam.rs` & `biobear-0.20.0/src/datasources/sam.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.19.6/src/datasources/vcf.rs` & `biobear-0.20.0/src/datasources/vcf.rs`

 * *Files 16% similar despite different names*

```diff
@@ -8,65 +8,81 @@
 //
 // Unless required by applicable law or agreed to in writing, software
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
+use arrow::datatypes::{DataType, Field};
 use exon::datasources::vcf::ListingVCFTableOptions;
 use noodles::core::Region;
 use pyo3::{pyclass, pymethods, PyResult};
 
 use crate::FileCompressionType;
 
 use super::parse_region;
 
 #[pyclass]
-#[derive(Debug, Clone)]
+#[derive(Debug, Clone, Default)]
 /// Options for reading VCF files.
 pub struct VCFReadOptions {
+    /// The region to read.
     region: Option<Region>,
+    /// The file compression type.
     file_compression_type: FileCompressionType,
-}
-
-impl Default for VCFReadOptions {
-    fn default() -> Self {
-        Self {
-            region: None,
-            file_compression_type: FileCompressionType::UNCOMPRESSED,
-        }
-    }
+    /// True if the INFO column should be parsed.
+    parse_info: bool,
+    /// True if the FORMAT column should be parsed.
+    parse_formats: bool,
+    /// The partition fields.
+    partition_cols: Option<Vec<String>>,
 }
 
 #[pymethods]
 impl VCFReadOptions {
     #[new]
-    #[pyo3(signature = (/, region = None, file_compression_type = None))]
+    #[pyo3(signature = (*, region = None, file_compression_type = None, parse_info = false, parse_formats = false, partition_cols = None))]
     fn try_new(
         region: Option<String>,
         file_compression_type: Option<FileCompressionType>,
+        parse_info: bool,
+        parse_formats: bool,
+        partition_cols: Option<Vec<String>>,
     ) -> PyResult<Self> {
         let region = parse_region(region)?;
 
         let file_compression_type =
             file_compression_type.unwrap_or(FileCompressionType::UNCOMPRESSED);
 
         Ok(Self {
             region,
             file_compression_type,
+            parse_info,
+            parse_formats,
+            partition_cols,
         })
     }
 }
 
 impl From<VCFReadOptions> for ListingVCFTableOptions {
     fn from(options: VCFReadOptions) -> Self {
+        let mut o = ListingVCFTableOptions::new(options.file_compression_type.into(), false)
+            .with_parse_info(options.parse_info)
+            .with_parse_formats(options.parse_formats);
+
         let regions = options.region.map(|r| vec![r]).unwrap_or_default();
+        if !regions.is_empty() {
+            o = o.with_regions(regions);
+        }
 
-        let mut t = ListingVCFTableOptions::new(options.file_compression_type.into(), false);
+        if let Some(partition_cols) = options.partition_cols {
+            let partition_fields = partition_cols
+                .iter()
+                .map(|s| Field::new(s, DataType::Utf8, false))
+                .collect::<Vec<_>>();
 
-        if !regions.is_empty() {
-            t = t.with_regions(regions);
+            o = o.with_table_partition_cols(partition_fields);
         }
 
-        t
+        o
     }
 }
```

### Comparing `biobear-0.19.6/src/error.rs` & `biobear-0.20.0/src/error.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.19.6/src/execution_result.rs` & `biobear-0.20.0/src/execution_result.rs`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     error::{self, BioBearError},
     runtime::wait_for_future,
 };
 
 #[pyclass(name = "ExecutionResult", subclass)]
 #[derive(Clone)]
 pub(crate) struct ExecutionResult {
-    df: Arc<DataFrame>,
+    pub(super) df: Arc<DataFrame>,
 }
 
 impl ExecutionResult {
     pub(crate) fn new(df: DataFrame) -> Self {
         Self { df: Arc::new(df) }
     }
 }
```

### Comparing `biobear-0.19.6/src/exon_reader.rs` & `biobear-0.20.0/src/exon_reader.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.19.6/src/file_compression_type.rs` & `biobear-0.20.0/src/file_compression_type.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.19.6/src/lib.rs` & `biobear-0.20.0/src/lib.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.19.6/src/runtime.rs` & `biobear-0.20.0/src/runtime.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.19.6/src/session_context.rs` & `biobear-0.20.0/src/session_context.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.19.6/src/vcf_reader.rs` & `biobear-0.20.0/src/vcf_reader.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.19.6/Cargo.lock` & `biobear-0.20.0/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -782,15 +782,15 @@
 checksum = "b1f45e9417d87227c7a56d22e471c6206462cba514c7590c09aff4cf6d1ddcad"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "biobear"
-version = "0.19.6"
+version = "0.20.0"
 dependencies = [
  "arrow",
  "datafusion",
  "exon",
  "noodles",
  "pyo3",
  "tokio",
@@ -1513,17 +1513,17 @@
 dependencies = [
  "libc",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "exon"
-version = "0.19.1"
+version = "0.20.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6fa0bc4dd82d6ec6f8953d209f6d114d61ac9cbfc9d401306e1d052deae68f97"
+checksum = "f12d411c682725f817f372df500db33d3faeb062ae27bc1219cecb772d917915"
 dependencies = [
  "arrow",
  "async-trait",
  "bytes",
  "coitrees",
  "datafusion",
  "exon-bam",
@@ -1557,211 +1557,211 @@
  "tracing",
  "tracing-subscriber",
  "url",
 ]
 
 [[package]]
 name = "exon-bam"
-version = "0.19.1"
+version = "0.20.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "36c3dd44c11b39a6f687aef3b183c3b041cf11e548842812cd454828a4210f0d"
+checksum = "3462f703bcd000d6cbb99f7190b5ae643aa25e9724abd228d7526b45e4da811d"
 dependencies = [
  "arrow",
  "exon-common",
  "exon-sam",
  "futures",
  "itertools 0.12.1",
  "noodles",
  "object_store",
  "tokio",
 ]
 
 [[package]]
 name = "exon-bcf"
-version = "0.19.1"
+version = "0.20.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "37bac04538dce4ecf6a9896b95ce94b9c890d6d241f6c667698241b48939935b"
+checksum = "7ab4713826c8c1f227aa97f4635bf32925a2f46633255cba9be4d808dd3a7a12"
 dependencies = [
  "arrow",
  "exon-common",
  "exon-vcf",
  "futures",
  "noodles",
  "object_store",
  "tokio",
 ]
 
 [[package]]
 name = "exon-bed"
-version = "0.19.1"
+version = "0.20.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6ddef33fe52445d563cbdca3a29decf0c09b340e32046be5865c5fffb263dde8"
+checksum = "b39c5e9b78850fb321258d639a9b378071a00c7ddbe76816914ab3c9c02c0690"
 dependencies = [
  "arrow",
  "exon-common",
  "futures",
  "noodles",
  "object_store",
  "tokio",
  "tokio-util",
 ]
 
 [[package]]
 name = "exon-bigwig"
-version = "0.19.1"
+version = "0.20.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4672edb009c25f9e21ee477da20afc9df18693839dab7b56e1ca7cb3d9053886"
+checksum = "584019c71d19153df9d04ff407ef530707dafbdaa2c50518c15b089276ffd512"
 dependencies = [
  "arrow",
  "bigtools",
  "exon-common",
  "futures",
  "noodles",
  "object_store",
  "tokio",
  "tokio-util",
 ]
 
 [[package]]
 name = "exon-common"
-version = "0.19.1"
+version = "0.20.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9a937e7a0b277eda0ff02d7aaf2d0da883d3aedbc39c0c5e6e2a1bd43a373bac"
+checksum = "0e53da36a207408fe4b2c101f7ca74de80bae8695141b332d470fb6759008f67"
 dependencies = [
  "arrow",
  "datafusion",
  "futures",
  "glob",
  "object_store",
  "url",
 ]
 
 [[package]]
 name = "exon-cram"
-version = "0.19.1"
+version = "0.20.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "586985a4a2d623e0f65005ffb0e82e5e3387e1f32649646434cca0376e213a7c"
+checksum = "0dd5a8e5c6dd20123f5d4abf159ff92b3e68d33f42f2f27b6f636790a435c558"
 dependencies = [
  "arrow",
  "coitrees",
  "exon-common",
  "exon-sam",
  "futures",
  "noodles",
  "object_store",
  "tokio",
  "tracing",
 ]
 
 [[package]]
 name = "exon-fasta"
-version = "0.19.1"
+version = "0.20.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c3617480f7c8d671099cc96f2e2353aecbb3c98cd75c24d6205655a90630cc67"
+checksum = "4114a749ab07caff8400418afc1b9646d9ac9f24ca78155f0e7b2c335d2fc5c0"
 dependencies = [
  "arrow",
  "exon-common",
  "futures",
  "noodles",
  "object_store",
  "tokio",
  "tokio-util",
 ]
 
 [[package]]
 name = "exon-fastq"
-version = "0.19.1"
+version = "0.20.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "eb694d477d75dd5fdd0518ad3f94872d9e8ec8d2ca46a0b27f3c06eadafc4fcc"
+checksum = "8ef531a509a4d062e2a83d4ccb137da3ad23f2d075c664716136037574b3c4ef"
 dependencies = [
  "arrow",
  "exon-common",
  "futures",
  "noodles",
  "object_store",
  "tokio",
  "tokio-util",
 ]
 
 [[package]]
 name = "exon-fcs"
-version = "0.19.1"
+version = "0.20.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "75936579cf7d9ea383e05fcb0753d71d770d86436b30c0a1c1348207829a474d"
+checksum = "245c7d95bcd1a571e4f9e6437cc258a7c6af7677525a3a0c8af742bb6b6675fd"
 dependencies = [
  "arrow",
  "byteorder",
  "exon-common",
  "futures",
  "object_store",
  "tokio",
 ]
 
 [[package]]
 name = "exon-genbank"
-version = "0.19.1"
+version = "0.20.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8501cc2951e7547d1be6d16d39332c0e0d41872092ae38034c2810e3e1bc8342"
+checksum = "c23008e079cba06c24d5df23bf47d132c4ec6892e556cb8fbb75898e2ea207fc"
 dependencies = [
  "arrow",
  "exon-common",
  "futures",
  "gb-io",
  "object_store",
  "tokio",
 ]
 
 [[package]]
 name = "exon-gff"
-version = "0.19.1"
+version = "0.20.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "647d164a26a3c070bbe9a560f7101a34f41894356d331d43fd33c0e1740f16ed"
+checksum = "e5984c5326179f676df8c0d09313790dd73c4968dced821f7a5c21707d6326fb"
 dependencies = [
  "arrow",
  "exon-common",
  "futures",
  "noodles",
  "object_store",
  "tokio",
  "tokio-util",
 ]
 
 [[package]]
 name = "exon-gtf"
-version = "0.19.1"
+version = "0.20.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "955bc3d05bbbb5d59efe5b6da25c0e123d577e7002472512c38befe2c764d097"
+checksum = "e85b77f1f7f243f05b76bc50670e5b380de1eb2a140949e2bb4926afa62eefcc"
 dependencies = [
  "arrow",
  "exon-common",
  "futures",
  "noodles",
  "object_store",
  "tokio",
 ]
 
 [[package]]
 name = "exon-io"
-version = "0.19.1"
+version = "0.20.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9a925701c2da63b34e529206a8f4e64fa7fe35ec80b54580eb1f83754fb6745d"
+checksum = "9dcf8bdc69a6bea45d011091a6d7b7396facb9f0fa858819dfa5ee89ce77e92d"
 dependencies = [
  "async-trait",
  "aws-config",
  "aws-credential-types",
  "object_store",
  "tokio",
  "url",
 ]
 
 [[package]]
 name = "exon-mzml"
-version = "0.19.1"
+version = "0.20.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d38acb5706f38f2d55ddc98382bae052a09e89043368ec94cbffa6bed3e182e6"
+checksum = "dde77be5b7b22832bcffb41ae6f12efdc02576d66d5f3dd7e619ea7cf7a1e3d0"
 dependencies = [
  "arrow",
  "base64 0.22.0",
  "byteorder",
  "exon-common",
  "flate2",
  "futures",
@@ -1769,32 +1769,32 @@
  "quick-xml",
  "serde",
  "tokio",
 ]
 
 [[package]]
 name = "exon-sam"
-version = "0.19.1"
+version = "0.20.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "88ce1dc3243e1c3b9683680bdfaebd9130089c915275679340508c752209afbc"
+checksum = "3b3e598adaef273d4075ab8b6408f84b67c50601978c87996279d93d0a47a331"
 dependencies = [
  "arrow",
  "exon-common",
  "futures",
  "itertools 0.12.1",
  "noodles",
  "object_store",
  "tokio",
 ]
 
 [[package]]
 name = "exon-vcf"
-version = "0.19.1"
+version = "0.20.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d36092b522a08122746c5ca19fed73d2f16674a8b4b7670f5267679ffd009cc3"
+checksum = "9093381751971ad0a463bf87d675188bee95e263dbb29e9399dcaed4a4eddbd6"
 dependencies = [
  "arrow",
  "exon-common",
  "futures",
  "noodles",
  "object_store",
  "tokio",
```

### Comparing `biobear-0.19.6/pyproject.toml` & `biobear-0.20.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -12,12 +12,12 @@
 dependencies = ["pyarrow>=15"]
 license = { file = "LICENSE" }
 name = "biobear"
 readme = "README.md"
 requires-python = ">=3.8"
 description = "A package for working with Bioinformatics data with SQL and Arrow"
 summary = "A package for working with Bioinformatics data with SQL and Arrow"
-version = "0.19.6"
+version = "0.20.0"
 
 [tool.maturin]
 features = ["pyo3/extension-module"]
 python-source = "python"
```

### Comparing `biobear-0.19.6/PKG-INFO` & `biobear-0.20.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: biobear
-Version: 0.19.6
+Version: 0.20.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: pyarrow >=15
 License-File: LICENSE
 Summary: A package for working with Bioinformatics data with SQL and Arrow
 Author-email: WHERE TRUE devs <thauck+biobear@wheretrue.com>
```

