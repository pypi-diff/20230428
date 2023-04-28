# Comparing `tmp/cutadapt-4.3.tar.gz` & `tmp/cutadapt-4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cutadapt-4.3.tar", last modified: Fri Mar 17 13:22:02 2023, max compression
+gzip compressed data, was "cutadapt-4.4.tar", last modified: Fri Apr 28 08:35:29 2023, max compression
```

## Comparing `cutadapt-4.3.tar` & `cutadapt-4.4.tar`

### file list

```diff
@@ -1,320 +1,324 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 13:22:02.350044 cutadapt-4.3/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-03-17 13:21:51.000000 cutadapt-4.3/.codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-17 13:21:51.000000 cutadapt-4.3/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 13:22:02.318044 cutadapt-4.3/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-03-17 13:21:51.000000 cutadapt-4.3/.github/issue_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 13:22:02.318044 cutadapt-4.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-03-17 13:21:51.000000 cutadapt-4.3/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-03-17 13:21:51.000000 cutadapt-4.3/.github/workflows/pyinstaller.yml
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-03-17 13:21:51.000000 cutadapt-4.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-03-17 13:21:51.000000 cutadapt-4.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-17 13:21:51.000000 cutadapt-4.3/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    43456 2023-03-17 13:21:51.000000 cutadapt-4.3/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-03-17 13:21:51.000000 cutadapt-4.3/CITATION
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-03-17 13:21:51.000000 cutadapt-4.3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-03-17 13:21:51.000000 cutadapt-4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-03-17 13:21:51.000000 cutadapt-4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-03-17 13:22:02.350044 cutadapt-4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-03-17 13:21:51.000000 cutadapt-4.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 13:22:02.322044 cutadapt-4.3/doc/
--rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-03-17 13:21:51.000000 cutadapt-4.3/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 13:22:02.322044 cutadapt-4.3/doc/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    18174 2023-03-17 13:21:51.000000 cutadapt-4.3/doc/_static/adapters.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-03-17 13:21:51.000000 cutadapt-4.3/doc/_static/cutadapt-logo.inkscape.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-03-17 13:21:51.000000 cutadapt-4.3/doc/_static/cutadapt-logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-03-17 13:21:51.000000 cutadapt-4.3/doc/_static/cutadapt-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8689 2023-03-17 13:21:51.000000 cutadapt-4.3/doc/algorithms.rst
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-17 13:21:51.000000 cutadapt-4.3/doc/changes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-03-17 13:21:51.000000 cutadapt-4.3/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-03-17 13:21:51.000000 cutadapt-4.3/doc/develop.rst
--rw-r--r--   0 runner    (1001) docker     (123)    98493 2023-03-17 13:21:51.000000 cutadapt-4.3/doc/guide.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-03-17 13:21:51.000000 cutadapt-4.3/doc/ideas.rst
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-03-17 13:21:51.000000 cutadapt-4.3/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8686 2023-03-17 13:21:51.000000 cutadapt-4.3/doc/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13168 2023-03-17 13:21:51.000000 cutadapt-4.3/doc/recipes.rst
--rw-r--r--   0 runner    (1001) docker     (123)    29450 2023-03-17 13:21:51.000000 cutadapt-4.3/doc/reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-17 13:21:51.000000 cutadapt-4.3/doc/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-03-17 13:21:51.000000 cutadapt-4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-17 13:22:02.350044 cutadapt-4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-03-17 13:21:51.000000 cutadapt-4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 13:22:02.318044 cutadapt-4.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 13:22:02.326044 cutadapt-4.3/src/cutadapt/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-17 13:21:51.000000 cutadapt-4.3/src/cutadapt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49213 2023-03-17 13:21:51.000000 cutadapt-4.3/src/cutadapt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-03-17 13:21:51.000000 cutadapt-4.3/src/cutadapt/_align.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    26578 2023-03-17 13:21:51.000000 cutadapt-4.3/src/cutadapt/_align.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-03-17 13:21:51.000000 cutadapt-4.3/src/cutadapt/_kmer_finder.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11028 2023-03-17 13:21:51.000000 cutadapt-4.3/src/cutadapt/_kmer_finder.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-03-17 13:21:51.000000 cutadapt-4.3/src/cutadapt/_match_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-03-17 13:22:02.000000 cutadapt-4.3/src/cutadapt/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    47562 2023-03-17 13:21:51.000000 cutadapt-4.3/src/cutadapt/adapters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-03-17 13:21:51.000000 cutadapt-4.3/src/cutadapt/align.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-03-17 13:21:51.000000 cutadapt-4.3/src/cutadapt/info.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-03-17 13:21:51.000000 cutadapt-4.3/src/cutadapt/info.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-03-17 13:21:51.000000 cutadapt-4.3/src/cutadapt/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     8936 2023-03-17 13:21:51.000000 cutadapt-4.3/src/cutadapt/kmer_heuristic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-03-17 13:21:51.000000 cutadapt-4.3/src/cutadapt/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    28147 2023-03-17 13:21:51.000000 cutadapt-4.3/src/cutadapt/modifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)    19159 2023-03-17 13:21:51.000000 cutadapt-4.3/src/cutadapt/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    36567 2023-03-17 13:21:51.000000 cutadapt-4.3/src/cutadapt/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-03-17 13:21:51.000000 cutadapt-4.3/src/cutadapt/predicates.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-03-17 13:21:51.000000 cutadapt-4.3/src/cutadapt/qualtrim.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-03-17 13:21:51.000000 cutadapt-4.3/src/cutadapt/qualtrim.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    29600 2023-03-17 13:21:51.000000 cutadapt-4.3/src/cutadapt/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-03-17 13:21:51.000000 cutadapt-4.3/src/cutadapt/statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)    14534 2023-03-17 13:21:51.000000 cutadapt-4.3/src/cutadapt/steps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-03-17 13:21:51.000000 cutadapt-4.3/src/cutadapt/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-03-17 13:21:51.000000 cutadapt-4.3/src/cutadapt/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 13:22:02.326044 cutadapt-4.3/src/cutadapt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-03-17 13:22:02.000000 cutadapt-4.3/src/cutadapt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8491 2023-03-17 13:22:02.000000 cutadapt-4.3/src/cutadapt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 13:22:02.000000 cutadapt-4.3/src/cutadapt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-17 13:22:02.000000 cutadapt-4.3/src/cutadapt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-03-17 13:22:02.000000 cutadapt-4.3/src/cutadapt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-17 13:22:02.000000 cutadapt-4.3/src/cutadapt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 13:22:02.326044 cutadapt-4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 13:22:02.342044 cutadapt-4.3/tests/cut/
--rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/454.fa
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/SRR2040271_1.fastq
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/action_lowercase.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/action_retain.fasta
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/adapterorder-ag.fasta
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/adapterorder-ga.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/adapterx.fasta
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/anchored-back.fasta
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/anchored.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/anchored_no_indels.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/anchored_no_indels_wildcard.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/anywhere_repeat.fastq
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/casava.fastq
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 13:22:02.342044 cutadapt-4.3/tests/cut/combinatorial/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/combinatorial/combinatorial.A_G.1.fastq
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/combinatorial/combinatorial.A_G.2.fastq
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/combinatorial/combinatorial.A_T.1.fastq
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/combinatorial/combinatorial.A_T.2.fastq
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/combinatorial/combinatorial.A_unknown.1.fastq
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/combinatorial/combinatorial.A_unknown.2.fastq
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/combinatorial/combinatorial.C_G.1.fastq
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/combinatorial/combinatorial.C_G.2.fastq
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/combinatorial/combinatorial.C_T.1.fastq
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/combinatorial/combinatorial.C_T.2.fastq
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/combinatorial/combinatorial.C_unknown.1.fastq
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/combinatorial/combinatorial.C_unknown.2.fastq
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/combinatorial/combinatorial.unknown_G.1.fastq
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/combinatorial/combinatorial.unknown_G.2.fastq
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/combinatorial/combinatorial.unknown_T.1.fastq
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/combinatorial/combinatorial.unknown_T.2.fastq
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/combinatorial/combinatorial.unknown_unknown.1.fastq
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/combinatorial/combinatorial.unknown_unknown.2.fastq
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/demultiplexed.first.1.fastq
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/demultiplexed.first.2.fastq
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/demultiplexed.second.1.fastq
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/demultiplexed.second.2.fastq
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/demultiplexed.unknown.1.fastq
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/demultiplexed.unknown.2.fastq
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/discard-untrimmed.fastq
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/discard.fastq
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/dos.fastq
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/dual-i1.1.fastq
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/dual-i1.2.fastq
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/dual-i2.1.fastq
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/dual-i2.2.fastq
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/dual-unknown.1.fastq
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/dual-unknown.2.fastq
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/empty.fasta
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/empty.fastq
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/example.fa
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/examplefront.fa
--rw-r--r--   0 runner    (1001) docker     (123)    17780 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/illumina.fastq
--rw-r--r--   0 runner    (1001) docker     (123)    25093 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/illumina.info.txt
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/illumina5.fastq
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/illumina5.info.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/illumina64.fastq
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/info-rc.txt
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/interleaved.fastq
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/issue46.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/linked-anchored.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/linked-discard-g.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/linked-discard.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/linked-info.txt
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/linked-lowercase.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/linked-not-anchored.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/linked.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/lowercase.fastq
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/lowqual.fastq
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/lowqual.unchanged.fastq
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/maxee.fastq
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/maxlen.fa
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/maxn0.2.fasta
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/maxn0.4.fasta
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/maxn0.fasta
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/maxn1.fasta
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/maxn2.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/minlen.fa
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/minlen.noprimer.fa
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/multiprefix.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/multisuffix.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/nextseq.fastq
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/no-trim.fastq
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/no_indels.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/overlapb.fa
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/pair-adapters.1.fastq
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/pair-adapters.2.fastq
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/paired-filterboth.1.fastq
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/paired-filterboth.2.fastq
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/paired-filterfirst.1.fastq
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/paired-filterfirst.2.fastq
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/paired-m27.1.fastq
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/paired-m27.2.fastq
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/paired-onlyA.1.fastq
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/paired-onlyA.2.fastq
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/paired-separate.1.fastq
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/paired-separate.2.fastq
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/paired-too-short.1.fastq
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/paired-too-short.2.fastq
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/paired-trimmed.1.fastq
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/paired-trimmed.2.fastq
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/paired-untrimmed.1.fastq
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/paired-untrimmed.2.fastq
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/paired.1.fastq
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/paired.2.fastq
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/paired.m14.1.fastq
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/paired.m14.2.fastq
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/pairedq.1.fastq
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/pairedq.2.fastq
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/pairedu.1.fastq
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/pairedu.2.fastq
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/plus.fastq
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/polya.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/rename.1.fastq
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/rename.2.fastq
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/rename.fastq
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/rest.fa
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/restfront.fa
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/revcomp-single-normalize.fastq
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/revcomp-single.fastq
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/s_1_sequence.txt
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/shortened-negative.fastq
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/shortened.fastq
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/simple.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/small-no-trim.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/small.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/small.fastq
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/small.trimmed.fastq
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/small.untrimmed.fastq
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/solid-no-zerocap.fastq
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/solidqual.fastq
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/sra.fastq
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/stripped.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/suffix.fastq
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/trim-n.fasta
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/trimN3.fasta
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/trimN5.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/twoadapters.fasta
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/twoadapters.first.fasta
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/twoadapters.second.fasta
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/twoadapters.unknown.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/unconditional-back.fastq
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/unconditional-both.fastq
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/unconditional-front.fastq
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/wildcard.fa
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/wildcardN.fa
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/wildcard_adapter.fa
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/wildcard_adapter_anywhere.fa
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/cut/xadapter.fasta
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 13:22:02.350044 cutadapt-4.3/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/data/454.fa
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/data/E3M.fasta
--rw-r--r--   0 runner    (1001) docker     (123)     8630 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/data/E3M.qual
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/data/action_lowercase.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/data/action_retain.fasta
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/data/adapter-empty-name.fasta
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/data/adapter.fasta
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/data/adapterorder.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/data/anchored-back.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/data/anchored.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/data/anchored_no_indels.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/data/anywhere_repeat.fastq
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/data/casava.fastq
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/data/combinatorial.1.fastq
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/data/combinatorial.2.fastq
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/data/dos.fastq
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/data/dual-index.1.fastq
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/data/dual-index.2.fastq
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/data/empty.fasta
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/data/empty.fastq
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/data/example.fa
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/data/format-error.fastq
--rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/data/illumina.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/data/illumina5.fastq
--rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/data/illumina64.fastq
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/data/info-rc.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/data/interleaved.fastq
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/data/issue46.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/data/lengths.fa
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/data/linked.fasta
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/data/lowqual.fastq
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/data/maxee.fastq
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/data/maxn.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/data/multi.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/data/multiblock.fastq.bz2
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/data/multiblock.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/data/nextseq.fastq
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/data/no_indels.fasta
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/data/onlycomment.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/data/overlapb.fa
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/data/paired.1.fastq
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/data/paired.2.fastq
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/data/polya.fasta
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/data/prefix-adapter.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/data/rest.fa
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/data/rest.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/data/restfront.txt
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/data/revcomp.1.fastq
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/data/revcomp.2.fastq
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/data/s_1_sequence.txt.gz
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/data/simple.fasta
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/data/simple.fasta.gz
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/data/simple.fastq
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/data/small.fastq
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/data/small.fastq.bz2
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/data/small.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/data/small.fastq.xz
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/data/suffix-adapter.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/data/suffix.fastq
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/data/toolong.fa
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/data/tooshort.fa
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/data/tooshort.noprimer.fa
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/data/trim-n.fasta
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/data/trimN3.fasta
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/data/trimN5.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/data/twoadapters.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/data/underscore_fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/data/wildcard.fa
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/data/wildcardN.fa
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/data/wildcard_adapter.fa
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/data/withplus.fastq
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/data/xadapterx.fasta
--rw-r--r--   0 runner    (1001) docker     (123)    17680 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/test_adapters.py
--rw-r--r--   0 runner    (1001) docker     (123)    14561 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/test_align.py
--rw-r--r--   0 runner    (1001) docker     (123)     5942 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/test_command.py
--rw-r--r--   0 runner    (1001) docker     (123)    29970 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/test_commandline.py
--rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/test_kmer_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/test_kmer_heuristic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)    15242 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/test_modifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)    23199 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/test_paired.py
--rw-r--r--   0 runner    (1001) docker     (123)    15643 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/test_predicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/test_qualtrim.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/test_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/test_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/test_testutils.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/test_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/test_trim.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-03-17 13:21:51.000000 cutadapt-4.3/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-03-17 13:21:51.000000 cutadapt-4.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:35:29.195059 cutadapt-4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-28 08:35:19.000000 cutadapt-4.4/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-28 08:35:19.000000 cutadapt-4.4/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:35:29.163059 cutadapt-4.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-28 08:35:19.000000 cutadapt-4.4/.github/issue_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:35:29.163059 cutadapt-4.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-04-28 08:35:19.000000 cutadapt-4.4/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-28 08:35:19.000000 cutadapt-4.4/.github/workflows/pyinstaller.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-28 08:35:19.000000 cutadapt-4.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-28 08:35:19.000000 cutadapt-4.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-28 08:35:19.000000 cutadapt-4.4/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    44609 2023-04-28 08:35:19.000000 cutadapt-4.4/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-28 08:35:19.000000 cutadapt-4.4/CITATION
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-04-28 08:35:19.000000 cutadapt-4.4/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-28 08:35:19.000000 cutadapt-4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-28 08:35:19.000000 cutadapt-4.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-04-28 08:35:29.195059 cutadapt-4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-04-28 08:35:19.000000 cutadapt-4.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:35:29.163059 cutadapt-4.4/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-04-28 08:35:19.000000 cutadapt-4.4/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:35:29.167059 cutadapt-4.4/doc/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    18174 2023-04-28 08:35:19.000000 cutadapt-4.4/doc/_static/adapters.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-04-28 08:35:19.000000 cutadapt-4.4/doc/_static/cutadapt-logo.inkscape.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-04-28 08:35:19.000000 cutadapt-4.4/doc/_static/cutadapt-logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-04-28 08:35:19.000000 cutadapt-4.4/doc/_static/cutadapt-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     9420 2023-04-28 08:35:19.000000 cutadapt-4.4/doc/algorithms.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-28 08:35:19.000000 cutadapt-4.4/doc/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-04-28 08:35:19.000000 cutadapt-4.4/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-04-28 08:35:19.000000 cutadapt-4.4/doc/develop.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    98417 2023-04-28 08:35:19.000000 cutadapt-4.4/doc/guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-28 08:35:19.000000 cutadapt-4.4/doc/ideas.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-28 08:35:19.000000 cutadapt-4.4/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8686 2023-04-28 08:35:19.000000 cutadapt-4.4/doc/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12226 2023-04-28 08:35:19.000000 cutadapt-4.4/doc/recipes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    30125 2023-04-28 08:35:19.000000 cutadapt-4.4/doc/reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-28 08:35:19.000000 cutadapt-4.4/doc/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-04-28 08:35:19.000000 cutadapt-4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 08:35:29.195059 cutadapt-4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-28 08:35:19.000000 cutadapt-4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:35:29.163059 cutadapt-4.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:35:29.167059 cutadapt-4.4/src/cutadapt/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-28 08:35:19.000000 cutadapt-4.4/src/cutadapt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-28 08:35:19.000000 cutadapt-4.4/src/cutadapt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-04-28 08:35:19.000000 cutadapt-4.4/src/cutadapt/_align.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    32244 2023-04-28 08:35:19.000000 cutadapt-4.4/src/cutadapt/_align.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-28 08:35:19.000000 cutadapt-4.4/src/cutadapt/_kmer_finder.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11028 2023-04-28 08:35:19.000000 cutadapt-4.4/src/cutadapt/_kmer_finder.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-04-28 08:35:19.000000 cutadapt-4.4/src/cutadapt/_match_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-28 08:35:28.000000 cutadapt-4.4/src/cutadapt/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49367 2023-04-28 08:35:19.000000 cutadapt-4.4/src/cutadapt/adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5824 2023-04-28 08:35:19.000000 cutadapt-4.4/src/cutadapt/align.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51094 2023-04-28 08:35:19.000000 cutadapt-4.4/src/cutadapt/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7668 2023-04-28 08:35:19.000000 cutadapt-4.4/src/cutadapt/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-28 08:35:19.000000 cutadapt-4.4/src/cutadapt/info.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-28 08:35:19.000000 cutadapt-4.4/src/cutadapt/info.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-04-28 08:35:19.000000 cutadapt-4.4/src/cutadapt/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9241 2023-04-28 08:35:19.000000 cutadapt-4.4/src/cutadapt/kmer_heuristic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-04-28 08:35:19.000000 cutadapt-4.4/src/cutadapt/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28523 2023-04-28 08:35:19.000000 cutadapt-4.4/src/cutadapt/modifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19159 2023-04-28 08:35:19.000000 cutadapt-4.4/src/cutadapt/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16225 2023-04-28 08:35:19.000000 cutadapt-4.4/src/cutadapt/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-04-28 08:35:19.000000 cutadapt-4.4/src/cutadapt/predicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-28 08:35:19.000000 cutadapt-4.4/src/cutadapt/qualtrim.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-04-28 08:35:19.000000 cutadapt-4.4/src/cutadapt/qualtrim.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    30716 2023-04-28 08:35:19.000000 cutadapt-4.4/src/cutadapt/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15926 2023-04-28 08:35:19.000000 cutadapt-4.4/src/cutadapt/runners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-04-28 08:35:19.000000 cutadapt-4.4/src/cutadapt/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14885 2023-04-28 08:35:19.000000 cutadapt-4.4/src/cutadapt/steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-28 08:35:19.000000 cutadapt-4.4/src/cutadapt/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-04-28 08:35:19.000000 cutadapt-4.4/src/cutadapt/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:35:29.171059 cutadapt-4.4/src/cutadapt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-04-28 08:35:29.000000 cutadapt-4.4/src/cutadapt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8580 2023-04-28 08:35:29.000000 cutadapt-4.4/src/cutadapt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 08:35:29.000000 cutadapt-4.4/src/cutadapt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-28 08:35:29.000000 cutadapt-4.4/src/cutadapt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-28 08:35:29.000000 cutadapt-4.4/src/cutadapt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-28 08:35:29.000000 cutadapt-4.4/src/cutadapt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:35:29.171059 cutadapt-4.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:35:29.183059 cutadapt-4.4/tests/cut/
+-rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/454.fa
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/SRR2040271_1.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/action_lowercase.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/action_retain.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/adapterorder-ag.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/adapterorder-ga.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/adapterx.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/anchored-back.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/anchored.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/anchored_no_indels.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/anchored_no_indels_wildcard.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/anywhere_repeat.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/casava.fastq
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:35:29.187059 cutadapt-4.4/tests/cut/combinatorial/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/combinatorial/combinatorial.A_G.1.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/combinatorial/combinatorial.A_G.2.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/combinatorial/combinatorial.A_T.1.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/combinatorial/combinatorial.A_T.2.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/combinatorial/combinatorial.A_unknown.1.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/combinatorial/combinatorial.A_unknown.2.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/combinatorial/combinatorial.C_G.1.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/combinatorial/combinatorial.C_G.2.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/combinatorial/combinatorial.C_T.1.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/combinatorial/combinatorial.C_T.2.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/combinatorial/combinatorial.C_unknown.1.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/combinatorial/combinatorial.C_unknown.2.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/combinatorial/combinatorial.unknown_G.1.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/combinatorial/combinatorial.unknown_G.2.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/combinatorial/combinatorial.unknown_T.1.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/combinatorial/combinatorial.unknown_T.2.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/combinatorial/combinatorial.unknown_unknown.1.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/combinatorial/combinatorial.unknown_unknown.2.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/demultiplexed.first.1.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/demultiplexed.first.2.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/demultiplexed.second.1.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/demultiplexed.second.2.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/demultiplexed.unknown.1.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/demultiplexed.unknown.2.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/discard-untrimmed.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/discard.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/dos.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/dual-i1.1.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/dual-i1.2.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/dual-i2.1.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/dual-i2.2.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/dual-unknown.1.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/dual-unknown.2.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/empty.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/empty.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/example.fa
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/examplefront.fa
+-rw-r--r--   0 runner    (1001) docker     (123)    17780 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/illumina.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)    25093 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/illumina.info.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/illumina5.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/illumina5.info.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/illumina64.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/info-rc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/interleaved.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/issue46.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/linked-anchored.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/linked-discard-g.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/linked-discard.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/linked-info.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/linked-lowercase.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/linked-not-anchored.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/linked.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/lowercase.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/lowqual.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/lowqual.unchanged.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/maxee.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/maxlen.fa
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/maxn0.2.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/maxn0.4.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/maxn0.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/maxn1.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/maxn2.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/minlen.fa
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/minlen.noprimer.fa
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/multiprefix.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/multisuffix.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/nextseq.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/no-trim.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/no_indels.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/overlapb.fa
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/pair-adapters.1.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/pair-adapters.2.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/paired-filterboth.1.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/paired-filterboth.2.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/paired-filterfirst.1.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/paired-filterfirst.2.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/paired-m27.1.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/paired-m27.2.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/paired-onlyA.1.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/paired-onlyA.2.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/paired-separate.1.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/paired-separate.2.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/paired-too-short.1.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/paired-too-short.2.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/paired-trimmed.1.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/paired-trimmed.2.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/paired-untrimmed.1.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/paired-untrimmed.2.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/paired.1.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/paired.2.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/paired.m14.1.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/paired.m14.2.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/pairedq.1.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/pairedq.2.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/pairedu.1.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/pairedu.2.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/plus.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/poly-a.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/polya.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/rename.1.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/rename.2.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/rename.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/rest.fa
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/restfront.fa
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/revcomp-single-normalize.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/revcomp-single.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/s_1_sequence.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/shortened-negative.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/shortened.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/simple.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/small-no-trim.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/small.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/small.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/small.trimmed.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/small.untrimmed.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/solid-no-zerocap.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/solidqual.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/sra.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/stripped.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/suffix.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/trim-n.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/trimN3.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/trimN5.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/twoadapters.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/twoadapters.first.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/twoadapters.second.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/twoadapters.unknown.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/unconditional-back.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/unconditional-both.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/unconditional-front.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/wildcard.fa
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/wildcardN.fa
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/wildcard_adapter.fa
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/wildcard_adapter_anywhere.fa
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/cut/xadapter.fasta
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:35:29.195059 cutadapt-4.4/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/data/454.fa
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/data/E3M.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)     8630 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/data/E3M.qual
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/data/action_lowercase.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/data/action_retain.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/data/adapter-empty-name.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/data/adapter.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/data/adapterorder.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/data/anchored-back.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/data/anchored.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/data/anchored_no_indels.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/data/anywhere_repeat.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/data/casava.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/data/combinatorial.1.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/data/combinatorial.2.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/data/dos.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/data/dual-index.1.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/data/dual-index.2.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/data/empty.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/data/empty.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/data/example.fa
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/data/format-error.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/data/illumina.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/data/illumina5.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/data/illumina64.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/data/info-rc.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/data/interleaved.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/data/issue46.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/data/lengths.fa
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/data/linked.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/data/lowqual.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/data/maxee.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/data/maxn.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/data/multi.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/data/multiblock.fastq.bz2
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/data/multiblock.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/data/nextseq.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/data/no_indels.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/data/onlycomment.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/data/overlapb.fa
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/data/paired.1.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/data/paired.2.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/data/polya.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/data/prefix-adapter.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/data/rest.fa
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/data/rest.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/data/restfront.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/data/revcomp.1.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/data/revcomp.2.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/data/s_1_sequence.txt.gz
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/data/simple.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/data/simple.fasta.gz
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/data/simple.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/data/small.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/data/small.fastq.bz2
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/data/small.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/data/small.fastq.xz
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/data/suffix-adapter.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/data/suffix.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/data/toolong.fa
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/data/tooshort.fa
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/data/tooshort.noprimer.fa
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/data/trim-n.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/data/trimN3.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/data/trimN5.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/data/twoadapters.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/data/underscore_fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/data/wildcard.fa
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/data/wildcardN.fa
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/data/wildcard_adapter.fa
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/data/withplus.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/data/xadapterx.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    17698 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/test_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14621 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/test_align.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/test_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30056 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/test_commandline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/test_kmer_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/test_kmer_heuristic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15546 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/test_modifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23194 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/test_paired.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15661 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/test_predicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/test_qualtrim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/test_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/test_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/test_testutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/test_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/test_trim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-28 08:35:19.000000 cutadapt-4.4/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-04-28 08:35:19.000000 cutadapt-4.4/tox.ini
```

### Comparing `cutadapt-4.3/.github/workflows/ci.yml` & `cutadapt-4.4/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `cutadapt-4.3/.github/workflows/pyinstaller.yml` & `cutadapt-4.4/.github/workflows/pyinstaller.yml`

 * *Files identical despite different names*

### Comparing `cutadapt-4.3/CHANGES.rst` & `cutadapt-4.4/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,33 @@
 
 =========
 Changelog
 =========
 
+v4.4 (2023-04-28)
+-----------------
+
+* :issue:`695`: Fixed very slow k-mer heuristic initialization (hours instead
+  of seconds) for degenerate adapter sequences such as ``A{100}`` as used
+  when doing poly-A trimming.
+* :issue:`696`: Added option ``--poly-a`` for trimming poly-A tails. This is
+  more accurate and multiple times faster than using ``-a A{100}`` as previously
+  recommended. This is currently experimental (that is, the algorithm may change
+  in the next one or two releases).
+* :issue:`685`: Sped up index generation somewhat. This is most noticable when
+  demultiplexing using thousands or more adapters. The speedup is
+  different depending on whether indels are allowed or not because
+  different algorithms are used.
+* :issue:`685`: Sped up demultiplexing (when using an index) for the case when
+  the read contains ``N`` bases within the region where the adapter matches.
+  Previously, any ``N`` would disable the index for that read and trigger a
+  fallback to the slow method of matching each adapter one-by-one. Now the index
+  is used even in those cases.
+* :pr:`700`: Sped up ``--max-expected-errors``. Thanks @rhpvorderman.
+
 v4.3 (2023-03-17)
 -----------------
 
 * :pr:`663`: Cutadapt became significantly faster due to an added runtime
   heuristic that avoids running the full alignment algorithm if it can be
   proven that it cannot succeed. Thanks to @rhpvorderman for this great
   improvement!
@@ -211,15 +232,15 @@
 v2.9 (2020-03-18)
 -----------------
 
 * :issue:`441`: Add a ``--max-ee`` (or ``--max-expected-errors``) option
   for filtering reads whose number of expected errors exceeds the given
   threshold. The idea comes from
   `Edgar et al. (2015) <https://academic.oup.com/bioinformatics/article/31/21/3476/194979>`_.
-* :issue:`438`: The info file now contains the `` rc`` suffix that is added to
+* :issue:`438`: The info file now contains the ``rc`` suffix that is added to
   the names of reverse-complemented reads (with ``--revcomp``).
 * :issue:`448`: ``.bz2`` and ``.xz`` output wasn’t possible in multi-core mode.
 
 v2.8 (2020-01-13)
 -----------------
 
 * :issue:`220`: With option ``--revcomp``, Cutadapt now searches both the read
```

### Comparing `cutadapt-4.3/CITATION` & `cutadapt-4.4/CITATION`

 * *Files identical despite different names*

### Comparing `cutadapt-4.3/CONTRIBUTING.rst` & `cutadapt-4.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `cutadapt-4.3/LICENSE` & `cutadapt-4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cutadapt-4.3/PKG-INFO` & `cutadapt-4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cutadapt
-Version: 4.3
+Version: 4.4
 Summary: Adapter trimming and other preprocessing of high-throughput sequencing reads
 Author-email: Marcel Martin <marcel.martin@scilifelab.se>
 License: MIT
 Project-URL: Homepage, https://cutadapt.readthedocs.io/
 Project-URL: Changelog, https://cutadapt.readthedocs.io/en/stable/changes.html
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `cutadapt-4.3/README.rst` & `cutadapt-4.4/README.rst`

 * *Files identical despite different names*

### Comparing `cutadapt-4.3/doc/Makefile` & `cutadapt-4.4/doc/Makefile`

 * *Files identical despite different names*

### Comparing `cutadapt-4.3/doc/_static/adapters.svg` & `cutadapt-4.4/doc/_static/adapters.svg`

 * *Files identical despite different names*

### Comparing `cutadapt-4.3/doc/_static/cutadapt-logo.inkscape.svg` & `cutadapt-4.4/doc/_static/cutadapt-logo.inkscape.svg`

 * *Files identical despite different names*

### Comparing `cutadapt-4.3/doc/_static/cutadapt-logo.png` & `cutadapt-4.4/doc/_static/cutadapt-logo.png`

 * *Files identical despite different names*

### Comparing `cutadapt-4.3/doc/_static/cutadapt-logo.svg` & `cutadapt-4.4/doc/_static/cutadapt-logo.svg`

 * *Files identical despite different names*

### Comparing `cutadapt-4.3/doc/algorithms.rst` & `cutadapt-4.4/doc/algorithms.rst`

 * *Files 7% similar despite different names*

```diff
@@ -184,7 +184,26 @@
 
 (70), (38), 8, -8, -25, -23, -20, -21, -15, -7
 
 The numbers in parentheses are not computed (because 8 is greater than zero),
 but shown here for completeness. The position of the minimum (-25) is used as
 the trimming position. Therefore, the read is trimmed to the first four bases,
 which have quality values 42, 40, 26, 27.
+
+
+.. _expected-errors:
+
+Expected errors
+===============
+
+The ``--max-expected-errors`` (short version: ``--max-ee``) option discards a
+read if its number of expected errors exceeds the specified threshold.
+
+This emulates a filtering option originally implemented in
+`USEARCH <https://www.drive5.com/usearch/>`_. The number of expected errors is
+computed from the quality scores as described in the USEARCH paper by
+`Edgar et al. (2015) <https://academic.oup.com/bioinformatics/article/31/21/3476/194979>`_,
+(Section 2.2). That is, it is the sum of the error probabilities.
+
+The USEARCH manual page `has a lot more background on expected
+errors <https://www.drive5.com/usearch/manual/exp_errs.html>`_ and how to choose
+a threshold.
```

### Comparing `cutadapt-4.3/doc/conf.py` & `cutadapt-4.4/doc/conf.py`

 * *Files identical despite different names*

### Comparing `cutadapt-4.3/doc/develop.rst` & `cutadapt-4.4/doc/develop.rst`

 * *Files identical despite different names*

### Comparing `cutadapt-4.3/doc/guide.rst` & `cutadapt-4.4/doc/guide.rst`

 * *Files 0% similar despite different names*

```diff
@@ -974,17 +974,15 @@
 If you have many repeated bases in the adapter sequence, such as many ``N`` s or
 many ``A`` s, you do not have to spell them out. For example, instead of writing
 ten ``A`` in a row (``AAAAAAAAAA``), write ``A{10}`` instead. The number within
 the curly braces specifies how often the character that preceeds it will be
 repeated. This works also for IUPAC wildcard characters, as in ``N{5}``.
 
 It is recommended that you use quotation marks around your adapter sequence if
-you use this feature. For poly-A trimming, for example, you would write::
-
-    cutadapt -a "A{100}" -o output.fastq input.fastq
+you use this feature, as in ``-a "N{5}ACGT"``.
 
 
 .. _modifying-reads:
 
 Modifying reads
 ===============
 
@@ -1126,14 +1124,24 @@
 
 This works like regular quality trimming (where one would use ``-q 20``
 instead), except that the qualities of ``G`` bases are ignored.
 
 .. versionadded:: 1.10
 
 
+.. _poly-a:
+
+Poly-A trimming
+~~~~~~~~~~~~~~~
+
+Use `--poly-a`` to trim poly-A tails. Poly-A trimming is done after adapter trimming.
+
+.. versionadded:: 4.4
+
+
 Shortening reads to a fixed length
 ----------------------------------
 
 To shorten each read down to a certain length, use the ``--length`` option or
 the short version ``-l``::
 
     cutadapt -l 10 -o output.fastq.gz input.fastq.gz
@@ -1399,18 +1407,15 @@
 reads. They always discard those reads for which the filtering criterion applies.
 
 ``--max-n COUNT_or_FRACTION``
     Discard reads with more than COUNT ``N`` bases. If ``COUNT_or_FRACTION`` is
     a number between 0 and 1, it is interpreted as a fraction of the read length
 
 ``--max-expected-errors ERRORS`` or ``--max-ee ERRORS``
-    Discard reads with more than ERRORS expected errors. The number of expected
-    errors is computed as described in
-    `Edgar et al. (2015) <https://academic.oup.com/bioinformatics/article/31/21/3476/194979>`_,
-    (Section 2.2).
+    Discard reads with more than ERRORS :ref:`expected errors <expected-errors>`.
 
 ``--discard-casava``
     Discard reads that did not pass CASAVA filtering. Illumina’s CASAVA pipeline in
     version 1.8 adds an *is_filtered* header field to each read. Specifying this
     option, the reads that did not pass filtering (these are the reads that have
     a ``Y`` for *is_filtered*) will be discarded. Reads for which the header cannot
     be recognized are kept.
```

### Comparing `cutadapt-4.3/doc/ideas.rst` & `cutadapt-4.4/doc/ideas.rst`

 * *Files identical despite different names*

### Comparing `cutadapt-4.3/doc/installation.rst` & `cutadapt-4.4/doc/installation.rst`

 * *Files identical despite different names*

### Comparing `cutadapt-4.3/doc/recipes.rst` & `cutadapt-4.4/doc/recipes.rst`

 * *Files 3% similar despite different names*

```diff
@@ -52,42 +52,19 @@
       input.1.fastq.gz \
       input.2.fastq.gz
 
 
 Trim poly-A tails
 -----------------
 
-If you want to trim a poly-A tail from the 3' end of your reads, use the 3'
-adapter type (``-a``) with an adapter sequence of many repeated ``A``
-nucleotides. Use the
-following notation to specify a sequence that consists of 100 ``A``::
+Use ``--poly-a``, see :ref:`poly-A trimming <poly-a>`.
 
-    cutadapt -a "A{100}" -o output.fastq input.fastq
-
-This also works when there are sequencing errors in the poly-A tail. So this
-read ::
-
-    TACGTACGTACGTACGAAATAAAAAAAAAAA
-
-will be trimmed to::
-
-    TACGTACGTACGTACG
-
-If for some reason you would like to use a shorter sequence of ``A``, you can
-do so: The matching algorithm always picks the leftmost match that it can find,
-so Cutadapt will do the right thing even when the tail has more ``A`` than you
-used in the adapter sequence. However, sequencing errors may result in shorter
-matches than desired. For example, using ``-a "A{10}"``, the read above (where
-the ``AAAT`` is followed by eleven ``A``) would be trimmed to::
-
-    TACGTACGTACGTACGAAAT
-
-Depending on your application, perhaps a variant of ``-a A{10}N{90}`` is an
-alternative, forcing the match to be located as much to the left as possible,
-while still allowing for non-``A`` bases towards the end of the read.
+In versions of Cutadapt earlier than 4.4, the recommendation was to use
+``-a "A{100}"`` for poly-A-trimming, but the ``--poly-a`` option is more
+accurate and much faster.
 
 
 Trim a fixed number of bases preceding each adapter
 ---------------------------------------------------
 
 If the adapters you want to remove are preceded by some unknown sequence (such
 as a random tag/molecular identifier), you can specify this as part of the
```

### Comparing `cutadapt-4.3/doc/reference.rst` & `cutadapt-4.4/doc/reference.rst`

 * *Files 2% similar despite different names*

```diff
@@ -114,14 +114,17 @@
     :ref:`NextSeq-specific quality trimming <nextseq-trim>` that
     also trims dark cycles appearing as high-quality G bases.
 
 ``--quality-base N`` (default: 33)
     Assume that quality values in the FASTQ file are encoded as ascii(quality + N).
     This needs to be set to 64 for some very old Illumina FASTQ files.
 
+``--poly-a``
+    :ref:`Trim poly-A tails <poly-A>`.
+
 ``--length LENGTH``, ``-l LENGTH``
     Shorten reads to LENGTH, where LENGTH is an integer. Positive values remove bases at
     the end while negative ones remove bases at the beginning.
 
 ``--trim-n``
     Trim N's from 5' and 3' ends of reads. See: :ref:`Dealing with N bases <n-bases>`.
 
@@ -161,17 +164,16 @@
     Discard reads longer than LEN. If LEN2 is given for paired-end data, it is applied to R2.
 
 ``--max-n COUNT``
     Discard reads with more than COUNT 'N' bases.
     If COUNT is a number between 0 and 1,
     it is interpreted as a fraction of the read length. See :ref:`Dealing with N bases <n-bases>`.
 
-``--max-expected-errors ERRORS``, ``--max-ee ERRORS``
-    Discard reads whose expected number of errors (computed
-    from quality values) exceeds ERRORS.
+``--max-expected-errors E``, ``--max-ee E``
+    Discard reads whose :ref:`expected number of errors <expected-errors>` exceeds the value *E*.
 
 ``--discard-trimmed``, ``--discard``
     Discard reads in which an adapter match was found.
     Use also ``-O`` to avoid discarding too many randomly matching reads.
 
 ``--discard-untrimmed``, ``--trimmed-only``
     Discard reads in which no adapter match was found.
@@ -306,14 +308,17 @@
       "basepair_counts": {
         "input": 10100000,
         "input_read1": 10100000,
         "input_read2": null,
         "quality_trimmed": 842048,
         "quality_trimmed_read1": 842048,
         "quality_trimmed_read2": null,
+        "poly_a_trimmed": null,
+        "poly_a_trimmed_read1": null,
+        "poly_a_trimmed_read2": null,
         "output": 9038081,
         "output_read1": 9038081,
         "output_read2": null
       },
       "adapters_read1": [
         {
           "name": "1",
@@ -381,20 +386,20 @@
    If backwards incompatible changes are made, the major version is increased.
 
    Example: ``[0, 1]``
 
 cutadapt_version : str
    The version of Cutadapt that generated the report.
 
-   Example: ``"3.5"``
+   Example: ``"4.4"``
 
 python_version : str
    The Python version used to run Cutadapt.
 
-   Example: ``"3.9"``
+   Example: ``"3.10"``
 
 command_line_arguments : list of strings
    The command-line arguments for this invocation. Only for information, do not parse this.
 
    Example: ``["-a", "ACGT", "-o", "out.fastq", "input.fastq"]```
 
 cores : int
@@ -471,22 +476,33 @@
 basepair_counts.input_read1 : int
    Number of basepairs in the input, read 1 only.
 
 basepair_counts.input_read2 : int | null
    If paired-end, number of basepairs in the input counting read 2 only, null otherwise.
 
 basepair_counts.quality_trimmed : int | null
-   Total number of basepairs removed due to quality trimming, null if no quality trimming was done.
+   Total number of basepairs removed due to quality trimming or null if no quality trimming was done.
 
 basepair_counts.quality_trimmed_read1 : int | null
-   Number of basepairs removed from read 1 due to quality trimming, null if no quality trimming
+   Number of basepairs removed from read 1 due to quality trimming or null if no quality trimming
    was done.
 
 basepair_counts.quality_trimmed_read2 : int
-   Number of basepairs removed from read 2 due to quality trimming, null if no quality trimming was
+   Number of basepairs removed from read 2 due to quality trimming or null if no quality trimming was
+   done or if input was single end.
+
+basepair_counts.poly_a_trimmed : int | null
+   Total number of basepairs removed due to poly-A trimming or null if no poly-A trimming was done.
+
+basepair_counts.poly_a_trimmed_read1 : int | null
+   Number of basepairs removed from read 1 due to poly-A trimming or null if no poly-A trimming was
+   done.
+
+basepair_counts.poly_a_trimmed_read2 : int
+   Number of basepairs removed from read 2 due to poly-A trimming or null if no poly-A trimming was
    done or if input was single end.
 
 basepair_counts.output : int
    Total number of basepairs in the final output.
 
 basepair_counts.output_read1 : int
    Number of basepairs written to the read 1 final output.
@@ -753,14 +769,15 @@
 
 Read modifications are applied in the following order to each read.
 Steps not requested on the command-line are skipped.
 
 1. Unconditional base removal with ``--cut``
 2. Quality trimming (``-q``)
 3. Adapter trimming (``-a``, ``-b``, ``-g`` and uppercase versions)
-4. Read shortening (``--length``)
-5. N-end trimming (``--trim-n``)
-6. Length tag modification (``--length-tag``)
-7. Read name suffix removal (``--strip-suffix``)
-8. Addition of prefix and suffix to read name (``-x``/``--prefix`` and ``-y``/``--suffix``)
-9. Read renaming according to ``--rename``
-10. Replacing of negative quality values with zero (zero capping)
+4. Poly-A trimming (``--poly-a``)
+5. Read shortening (``--length``)
+6. N-end trimming (``--trim-n``)
+7. Length tag modification (``--length-tag``)
+8. Read name suffix removal (``--strip-suffix``)
+9. Addition of prefix and suffix to read name (``-x``/``--prefix`` and ``-y``/``--suffix``)
+10. Read renaming according to ``--rename``
+11. Replacing of negative quality values with zero (zero capping)
```

### Comparing `cutadapt-4.3/pyproject.toml` & `cutadapt-4.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 ]
 
 [project.urls]
 "Homepage" = "https://cutadapt.readthedocs.io/"
 "Changelog" = "https://cutadapt.readthedocs.io/en/stable/changes.html"
 
 [project.scripts]
-cutadapt = "cutadapt.__main__:main_cli"
+cutadapt = "cutadapt.cli:main_cli"
 
 [project.optional-dependencies]
 dev = [
     "Cython",
     "pytest",
     "pytest-timeout",
     "pytest-mock",
@@ -57,7 +57,10 @@
 [tool.mypy]
 warn_unused_configs = true
 
 [tool.cibuildwheel]
 environment = "CFLAGS=-g0"
 test-extras = ["dev"]
 test-command = ["pytest {project}"]
+
+[tool.ruff]
+line-length = 130
```

### Comparing `cutadapt-4.3/src/cutadapt/__main__.py` & `cutadapt-4.4/src/cutadapt/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -85,24 +85,24 @@
     PairedAdapterCutter,
     NextseqQualityTrimmer,
     Shortener,
     ReverseComplementer,
     PairedEndRenamer,
     Renamer,
     InvalidTemplate,
+    PolyATrimmer,
 )
 from cutadapt.report import full_report, minimal_report, Statistics
 from cutadapt.pipeline import (
-    Pipeline,
     SingleEndPipeline,
     PairedEndPipeline,
-    InputPaths,
-    OutputFiles,
 )
-from cutadapt.utils import available_cpu_count, Progress, DummyProgress, FileOpener
+from cutadapt.runners import Pipeline, run_pipeline
+from cutadapt.files import InputPaths, OutputFiles, FileOpener
+from cutadapt.utils import available_cpu_count, Progress, DummyProgress
 from cutadapt.log import setup_logging, REPORT
 from cutadapt.qualtrim import HasNoQualities
 
 logger = logging.getLogger()
 
 
 class CutadaptArgumentParser(ArgumentParser):
@@ -251,14 +251,16 @@
             "value is given, only the 3' end is trimmed. If two "
             "comma-separated cutoffs are given, the 5' end is trimmed with "
             "the first cutoff, the 3' end with the second.")
     group.add_argument("--quality-base", type=int, default=33, metavar='N',
         help="Assume that quality values in FASTQ are encoded as ascii(quality "
             "+ N). This needs to be set to 64 for some old Illumina "
             "FASTQ files. Default: %(default)s")
+    group.add_argument("--poly-a", action="store_true", default=False,
+        help="Trim poly-A tails")
     group.add_argument("--length", "-l", type=int, default=None, metavar="LENGTH",
             help="Shorten reads to LENGTH. Positive values remove bases at the end "
             "while negative ones remove bases at the beginning. This and the "
             "following modifications are applied after adapter trimming.")
     group.add_argument("--trim-n", action='store_true', default=False,
         help="Trim N's on ends of reads.")
     group.add_argument("--length-tag", metavar="TAG",
@@ -483,27 +485,38 @@
         > 1
     ):
         raise CommandLineError(
             "Only one of the --discard-trimmed, --discard-untrimmed "
             "and --untrimmed-output options can be used at the same time."
         )
 
-    demultiplex_mode = determine_demultiplex_mode(args)
+    demultiplex_mode = determine_demultiplex_mode(args.output, args.paired_output)
     if demultiplex_mode and args.discard_trimmed:
         raise CommandLineError("Do not use --discard-trimmed when demultiplexing.")
     if demultiplex_mode == "combinatorial" and args.pair_adapters:
         raise CommandLineError(
             "With --pair-adapters, you can only use {name} in your output file name template, "
             "not {name1} and {name2} (no combinatorial demultiplexing)."
         )
     if demultiplex_mode == "normal":
         out = out2 = None
         combinatorial_out = combinatorial_out2 = None
-        demultiplex_out, demultiplex_out2, untrimmed, untrimmed2 = open_demultiplex_out(
-            adapter_names, args, file_opener  # type: ignore
+        (
+            demultiplex_out,
+            demultiplex_out2,
+            untrimmed,
+            untrimmed2,
+        ) = open_demultiplex_out(
+            adapter_names,  # type: ignore
+            args.output,
+            args.paired_output,
+            args.untrimmed_output,
+            args.untrimmed_paired_output,
+            args.discard_untrimmed,
+            file_opener,
         )
     elif demultiplex_mode == "combinatorial":
         assert "{name1}" in args.output and "{name2}" in args.output
         assert "{name1}" in args.paired_output and "{name2}" in args.paired_output
         if args.untrimmed_output or args.untrimmed_paired_output:
             raise CommandLineError(
                 "Combinatorial demultiplexing (with {name1} and {name2})"
@@ -595,65 +608,74 @@
             "{name2}", fname2
         )
         combinatorial_out[(name1, name2)] = file_opener.xopen(path1, "wb")
         combinatorial_out2[(name1, name2)] = file_opener.xopen(path2, "wb")
     return combinatorial_out, combinatorial_out2
 
 
-def open_demultiplex_out(adapter_names: Sequence[str], args, file_opener):
+def open_demultiplex_out(
+    adapter_names: Sequence[str],
+    template1: str,
+    template2: Optional[str],
+    untrimmed_output: Optional[str],
+    untrimmed_paired_output: Optional[str],
+    discard_untrimmed: bool,
+    file_opener,
+):
     demultiplex_out = dict()
     demultiplex_out2: Optional[Dict[str, Any]] = (
-        dict() if args.paired_output is not None else None
+        dict() if template2 is not None else None
     )
     for name in adapter_names:
-        path1 = args.output.replace("{name}", name)
+        path1 = template1.replace("{name}", name)
         demultiplex_out[name] = file_opener.xopen(path1, "wb")
         if demultiplex_out2 is not None:
-            path2 = args.paired_output.replace("{name}", name)
+            assert template2 is not None
+            path2 = template2.replace("{name}", name)
             demultiplex_out2[name] = file_opener.xopen(path2, "wb")
-    untrimmed_path = args.output.replace("{name}", "unknown")
-    if args.untrimmed_output:
-        untrimmed_path = args.untrimmed_output
-    if args.discard_untrimmed:
+    untrimmed_path: Optional[str] = template1.replace("{name}", "unknown")
+    if untrimmed_output:
+        untrimmed_path = untrimmed_output
+    if discard_untrimmed:
         untrimmed = None
     else:
         untrimmed = file_opener.xopen(untrimmed_path, "wb")
-    if args.paired_output is not None:
-        untrimmed2_path = args.paired_output.replace("{name}", "unknown")
-        if args.untrimmed_paired_output:
-            untrimmed2_path = args.untrimmed_paired_output
-        if args.discard_untrimmed:
+    if template2 is not None:
+        untrimmed2_path = template2.replace("{name}", "unknown")
+        if untrimmed_paired_output:
+            untrimmed2_path = untrimmed_paired_output
+        if discard_untrimmed:
             untrimmed2 = None
         else:
             untrimmed2 = file_opener.xopen(untrimmed2_path, "wb")
     else:
         untrimmed2 = None
     return demultiplex_out, demultiplex_out2, untrimmed, untrimmed2
 
 
-def determine_demultiplex_mode(args) -> Union[str, bool]:
+def determine_demultiplex_mode(
+    output: Optional[str], paired_output: Optional[str]
+) -> Union[str, bool]:
     """Return one of "normal", "combinatorial" or False"""
 
-    demultiplex = args.output is not None and "{name}" in args.output
+    demultiplex = output is not None and "{name}" in output
 
-    if args.paired_output is not None and (
-        demultiplex != ("{name}" in args.paired_output)
-    ):
+    if paired_output is not None and (demultiplex != ("{name}" in paired_output)):
         raise CommandLineError(
             'When demultiplexing paired-end data, "{name}" must appear in '
             "both output file names (-o and -p)"
         )
 
     demultiplex_combinatorial = (
-        args.output is not None
-        and args.paired_output is not None
-        and "{name1}" in args.output
-        and "{name2}" in args.output
-        and "{name1}" in args.paired_output
-        and "{name2}" in args.paired_output
+        output is not None
+        and paired_output is not None
+        and "{name1}" in output
+        and "{name2}" in output
+        and "{name1}" in paired_output
+        and "{name2}" in paired_output
     )
     if demultiplex and demultiplex_combinatorial:
         raise CommandLineError("You cannot combine {name} with {name1} and {name2}")
 
     if demultiplex:
         return "normal"
     elif demultiplex_combinatorial:
@@ -768,111 +790,129 @@
             "GC content must be given as percentage between 0 and 100"
         )
 
     if args.pair_adapters and args.times != 1:
         raise CommandLineError("--pair-adapters cannot be used with --times")
 
 
-def pipeline_from_parsed_args(args, paired, adapters, adapters2) -> Pipeline:
-    """
-    Set up a processing pipeline from parsed command-line arguments.
+class PipelineMaker:
+    def __init__(self, args, paired, adapters, adapters2):
+        self.args = args
+        self.action = None if args.action == "none" else args.action
+        self.paired = paired
+        self.adapters = adapters
+        self.adapters2 = adapters2
 
-    If there are any problems parsing the arguments, a CommandLineError is raised.
+    def make(self) -> Pipeline:
+        """
+        Set up a processing pipeline from parsed command-line arguments.
 
-    Return an instance of Pipeline (SingleEndPipeline or PairedEndPipeline)
-    """
-    if args.action == "none":
-        args.action = None
+        If there are any problems parsing the arguments, a CommandLineError is raised.
 
-    modifiers = []
-    modifiers.extend(make_unconditional_cutters(args.cut, args.cut2, paired))
+        Return an instance of Pipeline (SingleEndPipeline or PairedEndPipeline)
+        """
+        modifiers = []
+        modifiers.extend(
+            make_unconditional_cutters(self.args.cut, self.args.cut2, self.paired)
+        )
 
-    if args.nextseq_trim is not None:
-        trimmer = NextseqQualityTrimmer(args.nextseq_trim, args.quality_base)
-        if paired:
-            modifiers.append((trimmer, copy.copy(trimmer)))
-        else:
-            modifiers.append(trimmer)
+        if self.args.nextseq_trim is not None:
+            trimmer = NextseqQualityTrimmer(
+                self.args.nextseq_trim, self.args.quality_base
+            )
+            if self.paired:
+                modifiers.append((trimmer, copy.copy(trimmer)))
+            else:
+                modifiers.append(trimmer)
 
-    modifiers.extend(
-        make_quality_trimmers(
-            args.quality_cutoff, args.quality_cutoff2, args.quality_base, paired
+        modifiers.extend(
+            make_quality_trimmers(
+                self.args.quality_cutoff,
+                self.args.quality_cutoff2,
+                self.args.quality_base,
+                self.paired,
+            )
         )
-    )
-    modifiers.extend(
-        make_adapter_cutter(
-            adapters,
-            adapters2,
-            paired,
-            args.pair_adapters,
-            args.action,
-            args.times,
-            args.reverse_complement,
-            not args.rename,  # no "rc" suffix if --rename is used
-            args.index,
+        modifiers.extend(
+            make_adapter_cutter(
+                self.adapters,
+                self.adapters2,
+                self.paired,
+                self.args.pair_adapters,
+                self.action,
+                self.args.times,
+                self.args.reverse_complement,
+                not self.args.rename,  # no "rc" suffix if --rename is used
+                self.args.index,
+            )
         )
-    )
-
-    for modifier in modifiers_applying_to_both_ends_if_paired(args):
-        if paired:
-            modifiers.append((modifier, copy.copy(modifier)))
-        else:
-            modifiers.append(modifier)
 
-    if args.rename and (args.prefix or args.suffix):
-        raise CommandLineError(
-            "Option --rename cannot be combined with --prefix (-x) or --suffix (-y)"
-        )
-    if args.rename and args.rename != "{header}":
-        try:
-            renamer = PairedEndRenamer(args.rename) if paired else Renamer(args.rename)
-            modifiers.append(renamer)
-        except InvalidTemplate as e:
-            raise CommandLineError(e)
+        for modifier in modifiers_applying_to_both_ends_if_paired(self.args):
+            if self.paired:
+                modifiers.append((modifier, copy.copy(modifier)))
+            else:
+                modifiers.append(modifier)
 
-    # Create the processing pipeline
-    if paired:
-        pair_filter_mode = "any" if args.pair_filter is None else args.pair_filter
-        pipeline = PairedEndPipeline(modifiers, pair_filter_mode)  # type: Any
-    else:
-        pipeline = SingleEndPipeline(modifiers)
+        if self.args.rename and (self.args.prefix or self.args.suffix):
+            raise CommandLineError(
+                "Option --rename cannot be combined with --prefix (-x) or --suffix (-y)"
+            )
+        if self.args.rename and self.args.rename != "{header}":
+            try:
+                renamer = (
+                    PairedEndRenamer(self.args.rename)
+                    if self.paired
+                    else Renamer(self.args.rename)
+                )
+                modifiers.append(renamer)
+            except InvalidTemplate as e:
+                raise CommandLineError(e)
+
+        # Create the processing pipeline
+        if self.paired:
+            pair_filter_mode = (
+                "any" if self.args.pair_filter is None else self.args.pair_filter
+            )
+            pipeline = PairedEndPipeline(modifiers, pair_filter_mode)  # type: Any
+        else:
+            pipeline = SingleEndPipeline(modifiers)
 
-    # When adapters are being trimmed only in R1 or R2, override the pair filter mode
-    # as using the default of 'any' would regard all read pairs as untrimmed.
-    if (
-        isinstance(pipeline, PairedEndPipeline)
-        and (not adapters2 or not adapters)
-        and (
-            args.discard_untrimmed
-            or args.untrimmed_output
-            or args.untrimmed_paired_output
-        )
-    ):
-        pipeline.override_untrimmed_pair_filter = True
+        # When adapters are being trimmed only in R1 or R2, override the pair filter mode
+        # as using the default of 'any' would regard all read pairs as untrimmed.
+        if (
+            isinstance(pipeline, PairedEndPipeline)
+            and (not self.adapters2 or not self.adapters)
+            and (
+                self.args.discard_untrimmed
+                or self.args.untrimmed_output
+                or self.args.untrimmed_paired_output
+            )
+        ):
+            pipeline.override_untrimmed_pair_filter = True
 
-    # Set filtering parameters
-    # Minimum/maximum length
-    for attr in "minimum_length", "maximum_length":
-        param = getattr(args, attr)
-        if param is not None:
-            lengths = parse_lengths(param)
-            if not paired and len(lengths) == 2:
-                raise CommandLineError(
-                    "Two minimum or maximum lengths given for single-end data"
-                )
-            if paired and len(lengths) == 1:
-                lengths = (lengths[0], lengths[0])
-            setattr(pipeline, attr, lengths)
-    pipeline.max_n = args.max_n
-    pipeline.max_expected_errors = args.max_expected_errors
-    pipeline.discard_casava = args.discard_casava
-    pipeline.discard_trimmed = args.discard_trimmed
-    pipeline.discard_untrimmed = args.discard_untrimmed
+        # Set filtering parameters
+        # Minimum/maximum length
+        for attr in "minimum_length", "maximum_length":
+            param = getattr(self.args, attr)
+            if param is not None:
+                lengths = parse_lengths(param)
+                if not self.paired and len(lengths) == 2:
+                    raise CommandLineError(
+                        "Two minimum or maximum lengths given for single-end data"
+                    )
+                if self.paired and len(lengths) == 1:
+                    lengths = (lengths[0], lengths[0])
+                setattr(pipeline, attr, lengths)
+        pipeline.max_n = self.args.max_n
+        pipeline.max_expected_errors = self.args.max_expected_errors
+        pipeline.discard_casava = self.args.discard_casava
+        pipeline.discard_trimmed = self.args.discard_trimmed
+        pipeline.discard_untrimmed = self.args.discard_untrimmed
 
-    return pipeline
+        return pipeline
 
 
 def adapters_from_args(args) -> Tuple[List[Adapter], List[Adapter]]:
     search_parameters = dict(
         max_errors=args.error_rate,
         min_overlap=args.overlap,
         read_wildcards=args.match_read_wildcards,
@@ -981,14 +1021,16 @@
                     rc_suffix=" rc" if add_rc_suffix else None,
                 )
             else:
                 yield adapter_cutter
 
 
 def modifiers_applying_to_both_ends_if_paired(args) -> Iterator[SingleEndModifier]:
+    if args.poly_a:
+        yield PolyATrimmer()
     if args.length is not None:
         yield Shortener(args.length)
     if args.trim_n:
         yield NEndTrimmer()
     if args.length_tag:
         yield LengthTagModifier(args.length_tag)
     for suffix in args.strip_suffix:
@@ -1069,32 +1111,37 @@
     try:
         is_interleaved_input = args.interleaved and len(args.inputs) == 1
         input_paths = setup_input_files(args.inputs, paired, is_interleaved_input)
         check_arguments(args, paired)
         adapters, adapters2 = adapters_from_args(args)
         log_adapters(adapters, adapters2 if paired else None)
 
-        pipeline = pipeline_from_parsed_args(args, paired, adapters, adapters2)
+        pipeline = PipelineMaker(args, paired, adapters, adapters2).make()
         adapter_names: List[Optional[str]] = [a.name for a in adapters]
         adapter_names2: List[Optional[str]] = [a.name for a in adapters2]
         outfiles = open_output_files(
             args, default_outfile, file_opener, adapter_names, adapter_names2
         )
         inpaths = InputPaths(*input_paths, interleaved=is_interleaved_input)
         logger.info(
             "Processing %s reads on %d core%s ...",
             {False: "single-end", True: "paired-end"}[pipeline.paired],
             cores,
             "s" if cores > 1 else "",
         )
-        stats = pipeline.run(inpaths, outfiles, cores, progress, args.buffer_size)
+        stats = run_pipeline(
+            pipeline, inpaths, outfiles, cores, progress, args.buffer_size
+        )
 
     except KeyboardInterrupt:
-        print("Interrupted", file=sys.stderr)
-        sys.exit(130)
+        if args.debug:
+            raise
+        else:
+            print("Interrupted", file=sys.stderr)
+            sys.exit(130)
     except BrokenPipeError:
         sys.exit(1)
     except (
         OSError,
         EOFError,
         HasNoQualities,
         dnaio.UnknownFileFormat,
@@ -1138,20 +1185,24 @@
     logger.debug("dnaio version: %s", dnaio.__version__)
     logger.debug("xopen version: %s", xopen.__version__)
 
 
 def log_adapters(adapters, adapters2):
     paired = adapters2 is not None
     logger.debug("R1 adapters (%d):" if paired else "Adapters (%d):", len(adapters))
-    for a in adapters:
+    for a in itertools.islice(adapters, 20):
         logger.debug("- %s", a)
+    if len(adapters) > 20:
+        logger.debug("- (%d more)", len(adapters) - 20)
     if paired:
         logger.debug("R2 adapters (%d):", len(adapters2))
-        for a in adapters2:
+        for a in itertools.islice(adapters2, 20):
             logger.debug("- %s", a)
+        if len(adapters2) > 20:
+            logger.debug("- (%d more)", len(adapters2) - 20)
 
 
 def setup_profiler_if_requested(requested):
     if requested:
         import cProfile
 
         profiler = cProfile.Profile()
@@ -1202,15 +1253,15 @@
     path2: Optional[str],
     cores: int,
     paired: bool,
     gc_content: float,
 ) -> Dict:
     d = {
         "tag": "Cutadapt report",
-        "schema_version": OneLine([0, 1]),
+        "schema_version": OneLine([0, 2]),
         "cutadapt_version": __version__,
         "python_version": platform.python_version(),
         "command_line_arguments": cmdlineargs,
         "cores": cores,
         "input": {
             "path1": path1,
             "path2": path2,
```

### Comparing `cutadapt-4.3/src/cutadapt/_align.pyi` & `cutadapt-4.4/src/cutadapt/_align.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional, Tuple
+from typing import Optional, Tuple, Iterable
 
 class DPMatrix:
     m: int
     n: int
     def __init__(self, reference: str, query: str): ...
     def set_entry(self, i: int, j: int, cost: int) -> None: ...
     def __str__(self) -> str: ...
@@ -36,7 +36,10 @@
         wildcard_query: bool = False,
         min_overlap: int = 1,
     ): ...
     def __repr__(self) -> str: ...
     def locate(self, query: str) -> Optional[Tuple[int, int, int, int, int, int]]: ...
 
 class SuffixComparer(PrefixComparer): ...
+
+def hamming_sphere(s: str, k: int) -> Iterable[str]: ...
+def edit_environment(t: str, k: int) -> Iterable[Tuple[str, int, int]]: ...
```

### Comparing `cutadapt-4.3/src/cutadapt/_align.pyx` & `cutadapt-4.4/src/cutadapt/_align.pyx`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 # cython: profile=False, emit_code_comments=False, language_level=3
+from cpython.ref cimport PyObject
 from cpython.bytes cimport PyBytes_FromStringAndSize, PyBytes_AS_STRING
 from cpython.mem cimport PyMem_Malloc, PyMem_Free, PyMem_Realloc
 from cpython.unicode cimport PyUnicode_GET_LENGTH
+from libc.string cimport memcpy, memset
 
 from ._match_tables import _upper_table, _acgt_table, _iupac_table
 
 cdef extern from "Python.h":
+    unsigned char * PyUnicode_1BYTE_DATA(object o)
     void * PyUnicode_DATA(object o)
     bint PyUnicode_IS_COMPACT_ASCII(object o)
+    object PyUnicode_New(Py_ssize_t size, Py_UCS4 maxchar)
 
 DEF MATCH_SCORE = +1
 DEF MISMATCH_SCORE = -1
 DEF INSERTION_SCORE = -2
 DEF DELETION_SCORE = -2
 
 
@@ -394,32 +398,32 @@
             int cost_insertion
             int origin, cost, score
             int length
             int ref_start
             int cur_effective_length
             int last_filled_i = 0
             int best_length
+            int origin_increment = 1 if self.start_in_query else 0
+            int insertion_cost_increment = self._insertion_cost if not self.start_in_query else 0
             bint characters_equal
             bint is_acceptable
             # We keep only a single column of the DP matrix in memory.
             # To access the diagonal cell to the upper left,
             # we store it here before overwriting it.
             _Entry diag_entry
 
         with nogil:
             # iterate over columns
             for j in range(min_n + 1, max_n + 1):
                 # remember first entry before overwriting
                 diag_entry = column[0]
 
                 # fill in first entry in this column
-                if self.start_in_query:
-                    column[0].origin = j
-                else:
-                    column[0].cost = j * self._insertion_cost
+                column[0].origin += origin_increment
+                column[0].cost += insertion_cost_increment
                 for i in range(1, last + 1):
                     if compare_ascii:
                         characters_equal = (s1[i-1] == s2[j-1])
                     else:
                         characters_equal = (s1[i-1] & s2[j-1]) != 0
                     if characters_equal:
                         # If the characters match, we can skip computing costs for
@@ -685,7 +689,175 @@
     def locate(self, str query):
         cdef int n = len(query)
         result = super().locate(query[::-1])
         if result is None:
             return None
         _, length, _, _, score, errors = result
         return (self.m - length, self.m, n - length, n, score, errors)
+
+
+def hamming_sphere(str s, int k):
+    """
+    Yield all strings t for which the hamming distance between s and t is exactly k,
+    assuming the alphabet is A, C, G, T.
+    """
+    if k == 0:
+        yield s
+        return
+
+    if not PyUnicode_IS_COMPACT_ASCII(s):
+        raise ValueError("String must contain only ASCII characters")
+
+    cdef:
+        Py_ssize_t n = PyUnicode_GET_LENGTH(s)
+        unsigned char* s_ptr = <unsigned char*>PyUnicode_DATA(s)
+        Py_ssize_t i, j
+        #str prefix, prefix2
+        unsigned char ch, ch1, ch2
+        unsigned char* result_ptr
+
+    if k == 1:
+        for i in range(n):
+            for ch in "ACGT":
+                if s_ptr[i] == ch:
+                    continue
+                result = PyUnicode_New(n, 255)
+                if <PyObject*>result == NULL:
+                    raise MemoryError()
+                result_ptr = <unsigned char*>PyUnicode_1BYTE_DATA(result)
+                memcpy(result_ptr, s_ptr, n)
+                result_ptr[i] = ch
+                yield result
+        return
+
+    if k == 2:
+        for i in range(n):
+            for ch1 in "ACGT":
+                if s_ptr[i] == ch1:
+                    continue
+
+                for j in range(i + 1, n):
+                    for ch2 in "ACGT":
+                        if s[j] == ch2:
+                            continue
+
+                        result = PyUnicode_New(n, 255)
+                        if <PyObject*>result == NULL:
+                            raise MemoryError()
+                        result_ptr = <unsigned char*>PyUnicode_1BYTE_DATA(result)
+                        memcpy(result_ptr, s_ptr, n)
+                        result_ptr[i] = ch1
+                        result_ptr[j] = ch2
+                        yield result
+        return
+
+    # Recursive solution for k > 2
+    # i is the first position that is varied
+    for i in range(n - k + 1):
+        prefix = s[:i]
+        c = s[i]
+        suffix = s[i + 1 :]
+        for pch in "ACGT":
+            if pch == c:
+                continue
+            for t in hamming_sphere(suffix, k - 1):
+                yield prefix + pch + t
+
+
+def edit_environment(str t_str, int k):
+    """
+    Find all strings s for which the edit distance between s and t is at most k,
+    assuming the alphabet is A, C, G, T.
+
+    Yield tuples (s, e, m), where e is the edit distance between s and t and
+    m is the number of matches in the optimal alignment.
+    """
+
+    cdef bytes t = t_str.encode().translate(bytes.maketrans(b"ACGTacgt", b"\0\1\2\3\0\1\2\3"))
+    cdef unsigned char* t_ptr = t
+
+    # len(s) = m, indexed by i
+    # len(t) = n, indexed by j
+    cdef:
+        int j, match, diag, left, up, c, m
+        int i = 0
+        int n = len(t)
+        char ch
+        int min_cost
+
+    cdef int* costs = <int*> PyMem_Malloc((n + 1) * (n + k + 1) * sizeof(int))
+
+    if not costs:
+        raise MemoryError()
+    memset(costs, k+1, (n+1) * (n+k+1) * sizeof(int))
+    for i in range(n + k + 1):
+        costs[i*(n+1)] = i
+    for j in range(n + 1):
+        costs[j] = j
+
+    cdef int* matches = <int*> PyMem_Malloc((n + 1) * (n + k + 1) * sizeof(int))
+    if not matches:
+        raise MemoryError()
+    memset(matches, 0, (n+1) * (n+k+1) * sizeof(int))
+
+    trans = bytes.maketrans(b"\0\1\2\3", b"ACGT")
+
+    cdef char* s = <char*>PyMem_Malloc((n + k + 1) * sizeof(char))
+    i = 0
+    if not s:
+        raise MemoryError()
+    while True:
+        # Fill in row i (unless it is row 0, which is already filled in)
+        if i > 0:
+            ch = s[i - 1]
+            min_cost = 999999999
+            for j in range(max(1, i - k), min(n + 1, i + k + 1)):
+                match = 0 if t_ptr[j - 1] == ch else 1
+
+                diag = costs[(i - 1) * (n+1) + j - 1] + match
+                left = costs[i * (n+1) + j - 1] + 1
+                up = costs[(i - 1) * (n+1) + j] + 1
+                if diag <= left and diag <= up:
+                    c = diag
+                    m = matches[(i - 1) * (n+1) + j - 1] + (1 - match)
+                elif left <= up:
+                    c = left
+                    m = matches[i * (n+1) + j - 1]
+                else:
+                    c = up
+                    m = matches[(i - 1) * (n+1) + j]
+                costs[i*(n+1) + j] = c
+                matches[i*(n+1) + j] = m
+                min_cost = min(min_cost, c)
+        else:
+            min_cost = 0
+
+        if costs[i * (n+1) + n] <= k:
+            # The costs of an optimal alignment of t against s are at most k,
+            # so s is within the edit environment.
+            result = PyBytes_FromStringAndSize(s, i)
+            if <PyObject*>result == NULL:
+                raise MemoryError()
+
+            yield result.translate(trans).decode(), costs[i * (n+1) + n], matches[i * (n+1) + n]
+
+        # Next string
+        if min_cost <= k and i < n + k:
+            # When all entries are greater than k, we can skip remaining prefixes since costs in
+            # subsequent rows cannot get lower
+            s[i] = 0
+            i += 1
+        else:
+            while True:
+                if i == 0:
+                    PyMem_Free(costs)
+                    PyMem_Free(matches)
+                    return
+                i -= 1
+                ch = s[i]
+                if ch < 3:
+                    break
+
+            s[i] = ch + 1
+            i += 1
+
+    assert False
```

### Comparing `cutadapt-4.3/src/cutadapt/_kmer_finder.pyx` & `cutadapt-4.4/src/cutadapt/_kmer_finder.pyx`

 * *Files identical despite different names*

### Comparing `cutadapt-4.3/src/cutadapt/_match_tables.py` & `cutadapt-4.4/src/cutadapt/_match_tables.py`

 * *Files identical despite different names*

### Comparing `cutadapt-4.3/src/cutadapt/adapters.py` & `cutadapt-4.4/src/cutadapt/adapters.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,23 +5,24 @@
 The ...Match classes trim the reads.
 """
 import logging
 from enum import IntFlag
 from collections import defaultdict
 from typing import Optional, Tuple, Sequence, Dict, Any, List, Union
 from abc import ABC, abstractmethod
+import time
 
 from ._kmer_finder import KmerFinder
 from .align import (
     EndSkip,
     Aligner,
     PrefixComparer,
     SuffixComparer,
     edit_environment,
-    hamming_environment,
+    hamming_sphere,
 )
 from .kmer_heuristic import create_positions_and_kmers, kmer_probability_analysis
 
 logger = logging.getLogger()
 
 
 class MockKmerFinder:
@@ -1289,102 +1290,153 @@
         try:
             cls._accept(adapter)
         except ValueError:
             return False
         return True
 
     def _make_index(self) -> Tuple[List[int], "AdapterIndex"]:
+        start_time = time.time()
         logger.info("Building index of %s adapters ...", len(self._adapters))
         index: Dict[str, Tuple[SingleAdapter, int, int]] = dict()
         lengths = set()
         has_warned = False
         for adapter in self._adapters:
             sequence = adapter.sequence
             k = int(adapter.max_error_rate * len(sequence))
-            environment = edit_environment if adapter.indels else hamming_environment
-            for s, errors, matches in environment(sequence, k):
-                if s in index:
-                    other_adapter, other_errors, other_matches = index[s]
-                    if matches < other_matches:
-                        continue
-                    if other_matches == matches and not has_warned:
-                        logger.warning(
-                            "Adapters %s %r and %s %r are very similar. At %s allowed errors, "
-                            "the sequence %r cannot be assigned uniquely because the number of "
-                            "matches is %s compared to both adapters.",
-                            other_adapter.name,
-                            other_adapter.sequence,
-                            adapter.name,
-                            adapter.sequence,
-                            k,
-                            s,
-                            matches,
-                        )
-                        has_warned = True
-                else:
-                    index[s] = (adapter, errors, matches)
-                lengths.add(len(s))
-        logger.info("Built an index containing %s strings.", len(index))
+
+            if adapter.indels:
+                for s, errors, matches in edit_environment(sequence, k):
+                    if s in index:
+                        other_adapter, other_errors, other_matches = index[s]
+                        if matches < other_matches:
+                            continue
+                        if other_matches == matches and not has_warned:
+                            self._warn_similar(adapter, other_adapter, k, s, matches)
+                            has_warned = True
+                    else:
+                        index[s] = (adapter, errors, matches)
+                    lengths.add(len(s))
+            else:
+                n = len(sequence)
+                for errors in range(k + 1):
+                    for s in hamming_sphere(sequence, errors):
+                        matches = n - errors
+                        if s in index:
+                            other_adapter, other_errors, other_matches = index[s]
+                            if matches < other_matches:
+                                continue
+                            if other_matches == matches and not has_warned:
+                                self._warn_similar(
+                                    adapter, other_adapter, k, s, matches
+                                )
+                                has_warned = True
+                        else:
+                            index[s] = (adapter, errors, matches)
+                lengths.add(n)
+        elapsed = time.time() - start_time
+        logger.info(
+            "Built an index containing %s strings in %.1f s.", len(index), elapsed
+        )
 
         return sorted(lengths, reverse=True), index
 
+    @staticmethod
+    def _warn_similar(adapter, other_adapter, k, s, matches):
+        logger.warning(
+            "Adapters %s %r and %s %r are very similar. At %s allowed errors, "
+            "the sequence %r cannot be assigned uniquely because the number of "
+            "matches is %s compared to both adapters.",
+            other_adapter.name,
+            other_adapter.sequence,
+            adapter.name,
+            adapter.sequence,
+            k,
+            s,
+            matches,
+        )
+
     def _match_to_one_length(self, sequence: str):
         """
-        Match the adapters against a string and return a Match that represents
+        Match a query string against all adapters and return a Match that represents
         the best match or None if no match was found
         """
         affix = self._make_affix(sequence.upper(), self._length)
         if "N" in affix:
-            # Fall back to non-indexed matching
-            return self._multiple_adapters.match_to(sequence)
-        try:
-            adapter, e, m = self._index[affix]
-        except KeyError:
-            return None
+            result = self._lookup_with_n(affix)
+            if result is None:
+                return None
+            adapter, e, m = result
+        else:
+            try:
+                adapter, e, m = self._index[affix]
+            except KeyError:
+                return None
         return self._make_match(adapter, self._length, m, e, sequence)
 
     def _match_to_multiple_lengths(self, sequence: str):
         """
         Match the adapters against a string and return a Match that represents
         the best match or None if no match was found
         """
         affix = sequence.upper()
 
         # Check all the prefixes or suffixes (affixes) that could match
         best_adapter: Optional[SingleAdapter] = None
         best_length = 0
         best_m = -1
         best_e = 1000
-        check_n = True
+
+        # Check successively shorter affixes
         for length in self._lengths:
             if length < best_m:
                 # No chance of getting the same or a higher number of matches, so we can stop early
                 break
             affix = self._make_affix(affix, length)
-            if check_n:
-                if "N" in affix:
-                    return self._multiple_adapters.match_to(sequence)
-                check_n = False
-            try:
-                adapter, e, m = self._index[affix]
-            except KeyError:
-                continue
+            if "N" in affix:
+                result = self._lookup_with_n(affix)
+                if result is None:
+                    continue
+                adapter, e, m = result
+            else:
+                try:
+                    adapter, e, m = self._index[affix]
+                except KeyError:
+                    continue
+
             if m > best_m or (m == best_m and e < best_e):
                 # TODO this could be made to work:
                 # assert best_m == -1
                 best_adapter = adapter
                 best_e = e
                 best_m = m
                 best_length = length
 
         if best_m == -1:
             return None
         else:
             return self._make_match(best_adapter, best_length, best_m, best_e, sequence)
 
+    def _lookup_with_n(self, affix):
+        # N wildcards need to be counted as mismatches (read wildcards aren’t allowed).
+        # We can thus look up an affix where we replace N with an arbitrary nucleotide.
+        affix_without_n = affix.replace("N", "A")
+        try:
+            result = self._index[affix_without_n]
+        except KeyError:
+            return None
+
+        # The looked up number of matches and errors is too low if
+        # the adapter actually has an A where the N is in the query.
+        # Fix this by re-doing the alignment.
+        adapter = result[0]
+        match = adapter.match_to(affix)
+        if match is None:
+            return None
+        return adapter, match.errors, match.score
+
     def enable_debug(self):
         pass
 
 
 class IndexedPrefixAdapters(IndexedAdapters):
     @classmethod
     def _accept(cls, adapter):
```

### Comparing `cutadapt-4.3/src/cutadapt/align.py` & `cutadapt-4.4/src/cutadapt/align.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,21 @@
     "edit_environment",
     "edit_distance",
 ]
 
 from enum import IntFlag
 from typing import Iterator, Tuple
 
-from cutadapt._align import Aligner, PrefixComparer, SuffixComparer
+from cutadapt._align import (
+    Aligner,
+    PrefixComparer,
+    SuffixComparer,
+    hamming_sphere,
+    edit_environment,
+)
 
 
 class EndSkip(IntFlag):
     """
     Flags for the Aligner that indicate which ends of reference or query may be skipped at
     no cost. Setting all four flags at the same time results in semiglobal alignment.
     """
@@ -50,39 +56,14 @@
                 costs[i - 1] + 1,
             )
             prev = costs[i]
             costs[i] = c
     return costs[-1]
 
 
-def hamming_sphere(s: str, k: int) -> Iterator[str]:
-    """
-    Yield all strings t for which the hamming distance between s and t is exactly k,
-    assuming the alphabet is A, C, G, T.
-    """
-    assert k >= 0
-    if k == 0:
-        yield s
-        return
-    n = len(s)
-
-    # i is the first position that is varied
-    for i in range(n - k + 1):
-        prefix = s[:i]
-        c = s[i]
-        suffix = s[i + 1 :]
-        for ch in "ACGT":
-            if ch == c:
-                continue
-            for t in hamming_sphere(suffix, k - 1):
-                y = prefix + ch + t
-                assert len(y) == n
-                yield y
-
-
 def hamming_environment(s: str, k: int) -> Iterator[Tuple[str, int, int]]:
     """
     Find all strings t for which the hamming distance between s and t is at most k,
     assuming the alphabet is A, C, G, T.
 
     Yield tuples (t, e, m), where e is the hamming distance between s and t and
     m is the number of matches (equal to len(t) - e).
@@ -111,15 +92,15 @@
                 yield prefix + s[i + 1 :]  # substitution
             yield s + ch  # insertion into final position
         # all deletions
         for i in range(n):
             yield s[:i] + s[i + 1 :]
 
 
-def edit_environment(s: str, k: int) -> Iterator[Tuple[str, int, int]]:
+def py_edit_environment(s: str, k: int) -> Iterator[Tuple[str, int, int]]:
     """
     Find all strings t for which the edit distance between s and t is at most k,
     assuming the alphabet is A, C, G, T.
 
     Yield tuples (t, e, score), where e is the edit distance between s and t and
     score is the score of the optimal alignment.
     """
```

### Comparing `cutadapt-4.3/src/cutadapt/info.pyx` & `cutadapt-4.4/src/cutadapt/info.pyx`

 * *Files identical despite different names*

### Comparing `cutadapt-4.3/src/cutadapt/json.py` & `cutadapt-4.4/src/cutadapt/json.py`

 * *Files identical despite different names*

### Comparing `cutadapt-4.3/src/cutadapt/kmer_heuristic.py` & `cutadapt-4.4/src/cutadapt/kmer_heuristic.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,43 +1,33 @@
 import io
-import itertools
-import sys
 from typing import List, Optional, Set, Tuple
 from collections import defaultdict
 
 
-def kmer_possibilities(sequence: str, chunks: int) -> List[Set[str]]:
+def kmer_chunks(sequence: str, chunks: int) -> Set[str]:
     """
-    Partition a sequence in almost equal sized chunks. Return all possibilities.
-
-    Example sequence ABCDEFGH with 3 chunks. Possibilities:
-    ["ABC", "DEF", "GH"]; ["ABC", "DE", "FGH"]; ["AB", "CDE", "FGH"]
+    Partition a sequence in almost equal sized chunks. Returns the shortest
+    possibility. AABCABCABC, 3 returns {"AABC", "ABC"}
     """
     chunk_size = len(sequence) // (chunks)
     remainder = len(sequence) % (chunks)
     chunk_sizes: List[int] = remainder * [chunk_size + 1] + (chunks - remainder) * [
         chunk_size
     ]
-    possible_orderings = set(itertools.permutations(chunk_sizes))
-    kmer_sets = []
-    for chunk_list in possible_orderings:
-        offset = 0
-        chunk_set = set()
-        for size in chunk_list:
-            chunk_set.add(sequence[offset : offset + size])
-            offset += size
-        kmer_sets.append(chunk_set)
-    return kmer_sets
-
-
-# A SearchSet is a start and stop combined with a list of possible kmer sets
-# which should appear between this start and stop. Start and stop follow python
-# indexing rules. (Negative start is a position relative to the end. None end
-# is to the end of the sequence)
-SearchSet = Tuple[int, Optional[int], List[Set[str]]]
+    offset = 0
+    chunk_set = set()
+    for size in chunk_sizes:
+        chunk_set.add(sequence[offset : offset + size])
+        offset += size
+    return chunk_set
+
+
+# A SearchSet is a start and stop combined with a set of strings to search
+# for at that position
+SearchSet = Tuple[int, Optional[int], Set[str]]
 
 
 def minimize_kmer_search_list(
     kmer_search_list: List[Tuple[str, int, Optional[int]]]
 ) -> List[Tuple[str, int, Optional[int]]]:
     kmer_and_offsets_dict = defaultdict(list)
     for kmer, start, stop in kmer_search_list:  # type: ignore
@@ -70,32 +60,30 @@
         if back_searches:
             kmers_and_positions.append(
                 (kmer, min(start for start, stop in back_searches), None)
             )
     return kmers_and_positions
 
 
-def find_optimal_kmers(
+def remove_redundant_kmers(
     search_sets: List[SearchSet],
 ) -> List[Tuple[int, Optional[int], List[str]]]:
-    minimal_score = sys.maxsize
-    best_combination = []
-    positions = [(start, stop) for start, stop, kmer_set_list in search_sets]
-    kmer_set_lists = [kmer_set_list for start, stop, kmer_set_list in search_sets]
-    for kmer_sets in itertools.product(*kmer_set_lists):
-        kmer_search_list = []
-        for kmer_set, (start, stop) in zip(kmer_sets, positions):
-            for kmer in kmer_set:
-                kmer_search_list.append((kmer, start, stop))
-        minimized_search_list = minimize_kmer_search_list(kmer_search_list)
-        if len(minimized_search_list) < minimal_score:
-            best_combination = minimized_search_list
-            minimal_score = len(minimized_search_list)
+    """
+    This removes kmers that are searched in multiple search sets and makes
+    sure they are only searched in the larger search set. This reduces the
+    amount of searched patterns and therefore the number of false positives.
+    """
+
+    kmer_search_list = []
+    for start, stop, kmer_set in search_sets:
+        for kmer in kmer_set:
+            kmer_search_list.append((kmer, start, stop))
+    minimized_search_list = minimize_kmer_search_list(kmer_search_list)
     result_dict = defaultdict(list)
-    for kmer, start, stop in best_combination:
+    for kmer, start, stop in minimized_search_list:
         result_dict[(start, stop)].append(kmer)
     return [(start, stop, kmers) for (start, stop), kmers in result_dict.items()]
 
 
 def create_back_overlap_searchsets(
     adapter: str, min_overlap: int, error_rate: float
 ) -> List[SearchSet]:
@@ -116,18 +104,18 @@
         if max_errors == 0:
             # Add a couple of directly matching 1, 2, 3 and 4-mer searches.
             # The probability of a false positive is just to high when for
             # example a 3-mer is evaluated in more than one position.
             min_overlap_kmer_length = 5
             if minimum_length < min_overlap_kmer_length:
                 for i in range(minimum_length, min_overlap_kmer_length):
-                    search_set = (-i, None, [{adapter[:i]}])
+                    search_set = (-i, None, {adapter[:i]})
                     search_sets.append(search_set)
                 minimum_length = min_overlap_kmer_length
-        kmer_sets = kmer_possibilities(adapter[:minimum_length], max_errors + 1)
+        kmer_sets = kmer_chunks(adapter[:minimum_length], max_errors + 1)
         search_sets.append((-length, None, kmer_sets))
         minimum_length = length + 1
     return search_sets
 
 
 def create_positions_and_kmers(
     adapter: str,
@@ -162,24 +150,22 @@
         # with some parameters set differently. Reversing the adapter, running
         # the back adapter code and reversing all the kmers and positions has
         # the same effect without needing to duplicate the code.
         reversed_back_search_sets = create_back_overlap_searchsets(
             adapter[::-1], min_overlap, error_rate
         )
         front_search_sets = []
-        for start, stop, kmer_sets in reversed_back_search_sets:
-            new_kmer_sets = [
-                {kmer[::-1] for kmer in kmer_set} for kmer_set in kmer_sets
-            ]
-            front_search_sets.append((0, -start, new_kmer_sets))
+        for start, stop, kmer_set in reversed_back_search_sets:
+            new_kmer_set = {kmer[::-1] for kmer in kmer_set}
+            front_search_sets.append((0, -start, new_kmer_set))
         search_sets.extend(front_search_sets)
     if internal:
-        kmer_sets = kmer_possibilities(adapter, max_errors + 1)
+        kmer_sets = kmer_chunks(adapter, max_errors + 1)
         search_sets.append((0, None, kmer_sets))
-    return find_optimal_kmers(search_sets)
+    return remove_redundant_kmers(search_sets)
 
 
 def kmer_probability_analysis(
     kmers_and_offsets: List[Tuple[int, Optional[int], List[str]]],
     default_length: int = 150,
 ) -> str:  # pragma: no cover  # only for debugging use
     """
@@ -211,7 +197,35 @@
             out.write(
                 f"{kmer:10}\t{start}\t{stop}\t{considered_sites}\t{(1 - not_hit_chance) * 100:.2f}\n"
             )
     out.write(
         f"Chance for profile hit by random sequence: {(1 - accumulated_not_hit_chance) * 100:.2f}%\n"
     )
     return out.getvalue()
+
+
+if __name__ == "__main__":
+    # This allows for easy debugging and benchmarking of the kmer heuristic code.
+    import argparse
+    from ._kmer_finder import KmerFinder
+    import dnaio
+
+    parser = argparse.ArgumentParser()
+    parser.add_argument("--adapter")
+    parser.add_argument("--anywhere", action="store_true")
+    parser.add_argument("fastq")
+    args = parser.parse_args()
+    kmers_and_offsets = create_positions_and_kmers(
+        args.adapter, 3, 0.1, back_adapter=True, front_adapter=args.anywhere
+    )
+    kmer_finder = KmerFinder(kmers_and_offsets)
+    print(kmer_probability_analysis(kmers_and_offsets))
+    with dnaio.open(args.fastq, mode="r", open_threads=0) as reader:  # type: ignore
+        number_of_records = 0
+        possible_adapters_found = 0
+        for number_of_records, record in enumerate(reader, start=1):
+            if kmer_finder.kmers_present(record.sequence):
+                possible_adapters_found += 1
+    print(
+        f"Percentage possible adapters: "
+        f"{possible_adapters_found * 100 / number_of_records:.2f}%"
+    )
```

### Comparing `cutadapt-4.3/src/cutadapt/log.py` & `cutadapt-4.4/src/cutadapt/log.py`

 * *Files identical despite different names*

### Comparing `cutadapt-4.3/src/cutadapt/modifiers.py` & `cutadapt-4.4/src/cutadapt/modifiers.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import logging
 from types import SimpleNamespace
 from typing import Sequence, List, Tuple, Optional, Set
 from abc import ABC, abstractmethod
 
 from dnaio import record_names_match, SequenceRecord
 
-from .qualtrim import quality_trim_index, nextseq_trim_index
+from .qualtrim import quality_trim_index, nextseq_trim_index, poly_a_trim_index
 from .adapters import (
     MultipleAdapters,
     SingleAdapter,
     IndexedPrefixAdapters,
     IndexedSuffixAdapters,
     Match,
     remainder,
@@ -748,14 +748,27 @@
         start, stop = quality_trim_index(
             read.qualities, self.cutoff_front, self.cutoff_back, self.base
         )
         self.trimmed_bases += len(read) - (stop - start)
         return read[start:stop]
 
 
+class PolyATrimmer(SingleEndModifier):
+    def __init__(self):
+        self.trimmed_bases = 0
+
+    def __repr__(self):
+        return "PolyATrimmer()"
+
+    def __call__(self, record: SequenceRecord, info: ModificationInfo):
+        index = poly_a_trim_index(record.sequence)
+        self.trimmed_bases += len(record) - index
+        return record[:index]
+
+
 class Shortener(SingleEndModifier):
     """Unconditionally shorten a read to the given length
 
     If the length is positive, the bases are removed from the end of the read.
     If the length is negative, the bases are removed from the beginning of the read.
     """
```

### Comparing `cutadapt-4.3/src/cutadapt/parser.py` & `cutadapt-4.4/src/cutadapt/parser.py`

 * *Files identical despite different names*

### Comparing `cutadapt-4.3/src/cutadapt/predicates.py` & `cutadapt-4.4/src/cutadapt/predicates.py`

 * *Files identical despite different names*

### Comparing `cutadapt-4.3/src/cutadapt/qualtrim.pyx` & `cutadapt-4.4/src/cutadapt/qualtrim.pyx`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 # cython: profile=False, emit_code_comments=False, language_level=3
 """
 Quality trimming.
 """
+from cpython.unicode cimport PyUnicode_GET_LENGTH
+from libc.stdint cimport uint8_t
 
 cdef extern from *:
     unsigned char * PyUnicode_1BYTE_DATA(object o)
+    void *PyUnicode_DATA(object o)
+    bint PyUnicode_IS_COMPACT_ASCII(object o)
     int PyUnicode_KIND(object o)
     int PyUnicode_1BYTE_KIND
 
 
 cdef class HasNoQualities(Exception):
     pass
 
@@ -105,27 +109,67 @@
             break
         if s > max_qual:
             max_qual = s
             max_i = i
     return max_i
 
 
-def expected_errors(str qualities, int base=33):
+def poly_a_trim_index(str s):
+    """
+    Return start index of poly-A tail
+    """
+    if not PyUnicode_KIND(s) == PyUnicode_1BYTE_KIND:
+        raise ValueError("Sequence is not ASCII")
+    cdef:
+        char* s_ptr = <char *>PyUnicode_1BYTE_DATA(s)
+        int n = len(s)
+        int best_score = 0
+        int best_index = n
+        int score = 0
+        int i
+        char c
+        int errors = 0
+
+    for i in reversed(range(n)):
+        if s_ptr[i] == b"A":
+            score += 1
+        else:
+            score -= 2
+            errors += 1
+
+        if score > best_score and errors * 5 <= n - i:  # max error rate 0.2
+            best_score = score
+            best_index = i
+
+    return best_index
+
+
+# A lookup table is faster than recalculating the very expensive exponent
+# calculation every time.
+cdef double[94]  QUAL_TO_ERROR_RATE = [10 ** (-q / 10) for q in range(94)]
+
+def expected_errors(str qualities, uint8_t base=33):
     """
     Return the number of expected errors (as double) from a read’s
     qualities.
 
     This uses the formula in Edgar et al. (2015),
     see Section 2.2 in <https://academic.oup.com/bioinformatics/article/31/21/3476/194979>.
 
     qualities -- ASCII-encoded qualities (chr(qual + base))
     """
+    if not PyUnicode_IS_COMPACT_ASCII(qualities):
+        raise ValueError(f"Quality string contains non-ASCII values: {qualities}")
     cdef:
-        int i, q
-        bytes quals = qualities.encode()
-        char* cq = quals
+        size_t i
+        uint8_t phred, q
+        uint8_t *quals = <uint8_t *>PyUnicode_DATA(qualities)
+        size_t qual_length = PyUnicode_GET_LENGTH(qualities)
         double e = 0.0
 
-    for i in range(len(qualities)):
-        q = cq[i] - base
-        e += 10 ** (-q / 10)
+    for i in range(qual_length):
+        phred = quals[i]
+        q = phred - base
+        if q > 93:
+            raise ValueError(f"Not a valid phred value {q} for character {ord(q)}")
+        e += QUAL_TO_ERROR_RATE[q]
     return e
```

### Comparing `cutadapt-4.3/src/cutadapt/report.py` & `cutadapt-4.4/src/cutadapt/report.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 from .modifiers import (
     QualityTrimmer,
     NextseqQualityTrimmer,
     AdapterCutter,
     PairedAdapterCutter,
     ReverseComplementer,
     PairedEndModifierWrapper,
+    PolyATrimmer,
 )
 from .statistics import ReadLengthStatistics
 from .steps import HasStatistics, HasFilterStatistics
 
 FILTERS = {
     "too_short": "that were too short",
     "too_long": "that were too long",
@@ -66,14 +67,15 @@
         self.filtered: Dict[str, int] = defaultdict(int)
         self.reverse_complemented: Optional[int] = None
         self.n = 0
         self.total_bp = [0, 0]
         self.read_length_statistics = ReadLengthStatistics()
         self.with_adapters: List[Optional[int]] = [None, None]
         self.quality_trimmed_bp: List[Optional[int]] = [None, None]
+        self.poly_a_trimmed_bp: List[Optional[int]] = [None, None]
         self.adapter_stats: List[List[AdapterStatistics]] = [[], []]
         self._collected: bool = False
 
     def __iadd__(self, other: Any):
         if not isinstance(other, Statistics):
             raise ValueError(f"Cannot add {other.__type__.__name__}")
         self.n += other.n
@@ -156,14 +158,18 @@
         else:
             modifiers_list = [(0, m)]
         for i, modifier in modifiers_list:
             if isinstance(modifier, (QualityTrimmer, NextseqQualityTrimmer)):
                 self.quality_trimmed_bp[i] = add_if_not_none(
                     self.quality_trimmed_bp[i], modifier.trimmed_bases
                 )
+            if isinstance(modifier, PolyATrimmer):
+                self.poly_a_trimmed_bp[i] = add_if_not_none(
+                    self.poly_a_trimmed_bp[i], modifier.trimmed_bases
+                )
             elif isinstance(modifier, AdapterCutter):
                 assert self.with_adapters[i] is None
                 self.with_adapters[i] = modifier.with_adapters
                 self.adapter_stats[i] = list(modifier.adapter_statistics.values())
             elif isinstance(modifier, ReverseComplementer):
                 assert self.with_adapters[i] is None
                 self.with_adapters[i] = modifier.adapter_cutter.with_adapters
@@ -197,14 +203,17 @@
             "basepair_counts": {
                 "input": self.total,
                 "input_read1": self.total_bp[0],
                 "input_read2": self.total_bp[1] if self.paired else None,
                 "quality_trimmed": self.quality_trimmed,
                 "quality_trimmed_read1": self.quality_trimmed_bp[0],
                 "quality_trimmed_read2": self.quality_trimmed_bp[1],
+                "poly_a_trimmed": self.poly_a_trimmed,
+                "poly_a_trimmed_read1": self.poly_a_trimmed_bp[0],
+                "poly_a_trimmed_read2": self.poly_a_trimmed_bp[1],
                 "output": self.total_written_bp,
                 "output_read1": written_bp[0],
                 "output_read2": written_bp[1] if self.paired else None,
             },
             "adapters_read1": [
                 self._adapter_statistics_as_json(
                     astats, self.n, gc_content, one_line=one_line
@@ -289,14 +298,18 @@
         return sum(self.total_bp)
 
     @property
     def quality_trimmed(self) -> Optional[int]:
         return add_if_not_none(*self.quality_trimmed_bp)
 
     @property
+    def poly_a_trimmed(self) -> Optional[int]:
+        return add_if_not_none(*self.poly_a_trimmed_bp)
+
+    @property
     def total_written_bp(self) -> int:
         return sum(self.read_length_statistics.written_bp())
 
     @property
     def written(self) -> int:
         return self.read_length_statistics.written_reads()
 
@@ -323,14 +336,18 @@
     @property
     def reverse_complemented_fraction(self) -> float:
         return safe_divide(self.reverse_complemented, self.n)
 
     def filtered_fraction(self, filter_name: str) -> float:
         return safe_divide(self.filtered.get(filter_name), self.n)
 
+    @property
+    def poly_a_trimmed_fraction(self) -> float:
+        return safe_divide(self.poly_a_trimmed, self.total)
+
 
 class ErrorRanges:
     """
     Representation of the lengths up to which a number of errors is allowed
     for partial adapter matches.
 
     >>> ErrorRanges(length=8, error_rate=0.1).lengths()
@@ -604,14 +621,24 @@
             f"{stats.quality_trimmed:13,d} bp ({stats.quality_trimmed_fraction:.1%})\n"
         )
         if stats.paired:
             for i in (0, 1):
                 if stats.quality_trimmed_bp[i] is not None:
                     report += f"  Read {i + 1}: {stats.quality_trimmed_bp[i]:13,d} bp\n"
 
+    if stats.poly_a_trimmed is not None:
+        report += (
+            "Poly-A-trimmed:            "
+            f"{stats.poly_a_trimmed:13,d} bp ({stats.poly_a_trimmed_fraction:.1%})\n"
+        )
+        if stats.paired:
+            for i in (0, 1):
+                if stats.poly_a_trimmed_bp[i] is not None:
+                    report += f"  Read {i + 1}: {stats.poly_a_trimmed_bp[i]:13,d} bp\n"
+
     report += (
         "Total written (filtered):  "
         "{o.total_written_bp:13,d} bp ({o.total_written_bp_fraction:.1%})\n"
     )
     if stats.paired:
         report += "  Read 1: {o.written_bp[0]:13,d} bp\n"
         report += "  Read 2: {o.written_bp[1]:13,d} bp\n"
```

### Comparing `cutadapt-4.3/src/cutadapt/statistics.py` & `cutadapt-4.4/src/cutadapt/statistics.py`

 * *Files identical despite different names*

### Comparing `cutadapt-4.3/src/cutadapt/steps.py` & `cutadapt-4.4/src/cutadapt/steps.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,41 +16,42 @@
 3. The last pipeline step should be one of the "Sinks", which consume all reads.
    Demultiplexers are sinks, for example.
 """
 
 from abc import ABC, abstractmethod
 from typing import Tuple, Dict, Optional, Any
 
+from dnaio import SequenceRecord
+
 from .predicates import Predicate
 from .modifiers import ModificationInfo
 from .statistics import ReadLengthStatistics
 
-# Constants used when returning from a step’s __call__ method to improve
-# readability (it is unintuitive that "return True" means "discard the read").
-DISCARD = True
-KEEP = False
+RecordPair = Tuple[SequenceRecord, SequenceRecord]
 
 
 class SingleEndStep(ABC):
     @abstractmethod
-    def __call__(self, read, info: ModificationInfo) -> bool:
+    def __call__(self, read, info: ModificationInfo) -> Optional[SequenceRecord]:
         """
-        Process a single read. Return True if the read has been consumed
-        (and should thus not be passed on to subsequent steps).
+        Process a single read. Return the processed read or None to indicate that
+        the read has been consumed and should thus not be passed on to subsequent
+        steps.
         """
 
 
 class PairedEndStep(ABC):
     @abstractmethod
     def __call__(
         self, read1, read2, info1: ModificationInfo, info2: ModificationInfo
-    ) -> bool:
+    ) -> Optional[RecordPair]:
         """
-        Process read pair (read1, read2). Return True if the read pair
-        has been consumed (and should thus not be passed on to subsequent steps).
+        Process (read1, read2). Return the processed read pair or None if
+        the read pair has been "consumed" (filtered or written to an output file)
+        and should thus not be passed on to subsequent steps.
         """
 
 
 class HasStatistics(ABC):
     """
     Used for the final steps (sinks), which need to keep track of read length statistics
     """
@@ -87,21 +88,21 @@
 
     def descriptive_identifier(self) -> str:
         return self._predicate.descriptive_identifier()
 
     def filtered(self) -> int:
         return self._filtered
 
-    def __call__(self, read, info: ModificationInfo) -> bool:
+    def __call__(self, read, info: ModificationInfo) -> Optional[SequenceRecord]:
         if self._predicate.test(read, info):
             self._filtered += 1
             if self._writer is not None:
                 self._writer.write(read)
-            return DISCARD
-        return KEEP
+            return None
+        return read
 
 
 class PairedEndFilter(PairedEndStep, HasFilterStatistics):
     """
     A pipeline step that can filter paired-end reads, redirect them to a file, and counts
     how many read pairs were filtered.
 
@@ -176,63 +177,63 @@
     def _is_filtered_second(
         self, read1, read2, info1: ModificationInfo, info2: ModificationInfo
     ) -> bool:
         return self.predicate2.test(read2, info2)  # type: ignore
 
     def __call__(
         self, read1, read2, info1: ModificationInfo, info2: ModificationInfo
-    ) -> bool:
+    ) -> Optional[RecordPair]:
         if self._is_filtered(read1, read2, info1, info2):
             self._filtered += 1
             if self.writer is not None:
                 self.writer.write(read1, read2)
-            return DISCARD
-        return KEEP
+            return None
+        return (read1, read2)
 
 
 class RestFileWriter(SingleEndStep):
     def __init__(self, file):
         self._file = file
 
     def __repr__(self):
         return f"RestFileWriter(file={self._file})"
 
-    def __call__(self, read, info):
+    def __call__(self, read, info) -> Optional[SequenceRecord]:
         # TODO this fails with linked adapters
         if info.matches:
             rest = info.matches[-1].rest()
             if len(rest) > 0:
                 print(rest, read.name, file=self._file)
-        return KEEP
+        return read
 
 
 class WildcardFileWriter(SingleEndStep):
     def __init__(self, file):
         self._file = file
 
     def __repr__(self):
         return f"WildcardFileWriter(file={self._file})"
 
-    def __call__(self, read, info) -> bool:
+    def __call__(self, read, info) -> Optional[SequenceRecord]:
         # TODO this fails with linked adapters
         if info.matches:
             print(info.matches[-1].wildcards(), read.name, file=self._file)
-        return KEEP
+        return read
 
 
 class InfoFileWriter(SingleEndStep):
     RC_MAP = {None: "", True: "1", False: "0"}
 
     def __init__(self, file):
         self._file = file
 
     def __repr__(self):
         return f"InfoFileWriter(file={self._file})"
 
-    def __call__(self, read, info: ModificationInfo):
+    def __call__(self, read, info: ModificationInfo) -> Optional[SequenceRecord]:
         current_read = info.original_read
         if info.is_rc:
             current_read = current_read.reverse_complement()
         if info.matches:
             for match in info.matches:
                 for info_record in match.get_info_records(current_read):
                     # info_record[0] is the read name suffix
@@ -245,15 +246,15 @@
                     )
                 current_read = match.trimmed(current_read)
         else:
             seq = read.sequence
             qualities = read.qualities if read.qualities is not None else ""
             print(read.name, -1, seq, qualities, sep="\t", file=self._file)
 
-        return KEEP
+        return read
 
 
 class PairedSingleEndStep(PairedEndStep):
     """
     Wrap a SingleEndStep as a PairedEndStep
 
     The wrapped step is called with the first read
@@ -261,18 +262,21 @@
 
     def __init__(self, step: SingleEndStep):
         self._step = step
 
     def __repr__(self):
         return f"PairedSingleEndStep(step={self._step})"
 
-    def __call__(self, read1, read2, info1, info2):
+    def __call__(self, read1, read2, info1, info2) -> Optional[RecordPair]:
         _ = read2  # intentionally ignored
         _ = info2
-        return self._step(read1, info1)
+        result = self._step(read1, info1)
+        if result is None:
+            return None
+        return (result, read2)
 
 
 # The following steps are used as final step in a pipeline.
 # They send each read or read pair to the final intended output file,
 # and they all track the lengths of written reads.
 
 
@@ -286,18 +290,18 @@
         super().__init__()
         self.writer = writer
         self._statistics = ReadLengthStatistics()
 
     def __repr__(self):
         return f"NoFilter({self.writer})"
 
-    def __call__(self, read, info: ModificationInfo) -> bool:
+    def __call__(self, read, info: ModificationInfo) -> Optional[SequenceRecord]:
         self.writer.write(read)
         self._statistics.update(read)
-        return DISCARD
+        return None
 
     def get_statistics(self) -> ReadLengthStatistics:
         return self._statistics
 
 
 class PairedEndSink(PairedEndStep, HasStatistics):
     """
@@ -311,18 +315,18 @@
         self._statistics = ReadLengthStatistics()
 
     def __repr__(self):
         return f"PairedNoFilter({self.writer})"
 
     def __call__(
         self, read1, read2, info1: ModificationInfo, info2: ModificationInfo
-    ) -> bool:
+    ) -> Optional[RecordPair]:
         self.writer.write(read1, read2)
         self._statistics.update2(read1, read2)
-        return DISCARD
+        return None
 
     def get_statistics(self) -> ReadLengthStatistics:
         return self._statistics
 
 
 class Demultiplexer(SingleEndStep, HasStatistics, HasFilterStatistics):
     """
@@ -341,28 +345,28 @@
         self._untrimmed_writer = self._writers.get(None, None)
         self._statistics = ReadLengthStatistics()
         self._filtered = 0
 
     def __repr__(self):
         return f"<Demultiplexer len(writers)={len(self._writers)}>"
 
-    def __call__(self, read, info):
+    def __call__(self, read, info) -> Optional[SequenceRecord]:
         """
         Write the read to the proper output file according to the most recent match
         """
         if info.matches:
             name = info.matches[-1].adapter.name
             self._statistics.update(read)
             self._writers[name].write(read)
         elif self._untrimmed_writer is not None:
             self._statistics.update(read)
             self._untrimmed_writer.write(read)
         else:
             self._filtered += 1
-        return DISCARD
+        return None
 
     def descriptive_identifier(self) -> str:
         return "discard_untrimmed"
 
     def get_statistics(self) -> ReadLengthStatistics:
         return self._statistics
 
@@ -381,26 +385,26 @@
         self._writers = writers
         self._untrimmed_writer = self._writers.get(None, None)
         self._statistics = ReadLengthStatistics()
         self._filtered = 0
 
     def __call__(
         self, read1, read2, info1: ModificationInfo, info2: ModificationInfo
-    ) -> bool:
+    ) -> Optional[RecordPair]:
         assert read2 is not None
         if info1.matches:
             name = info1.matches[-1].adapter.name  # type: ignore
             self._statistics.update2(read1, read2)
             self._writers[name].write(read1, read2)
         elif self._untrimmed_writer is not None:
             self._statistics.update2(read1, read2)
             self._untrimmed_writer.write(read1, read2)
         else:
             self._filtered += 1
-        return DISCARD
+        return None
 
     def descriptive_identifier(self) -> str:
         return "discard_untrimmed"
 
     def get_statistics(self) -> ReadLengthStatistics:
         return self._statistics
 
@@ -421,23 +425,23 @@
         of the name. Missing dictionary keys are ignored and can be used to discard
         read pairs.
         """
         super().__init__()
         self._writers = writers
         self._statistics = ReadLengthStatistics()
 
-    def __call__(self, read1, read2, info1, info2) -> bool:
+    def __call__(self, read1, read2, info1, info2) -> Optional[RecordPair]:
         """
         Write the read to the proper output file according to the most recent matches both on
         R1 and R2
         """
         assert read2 is not None
         name1 = info1.matches[-1].adapter.name if info1.matches else None
         name2 = info2.matches[-1].adapter.name if info2.matches else None
         key = (name1, name2)
         if key in self._writers:
             self._statistics.update2(read1, read2)
             self._writers[key].write(read1, read2)
-        return DISCARD
+        return None
 
     def get_statistics(self) -> ReadLengthStatistics:
         return self._statistics
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `cutadapt-4.3/src/cutadapt/tokenizer.py` & `cutadapt-4.4/src/cutadapt/tokenizer.py`

 * *Files identical despite different names*

### Comparing `cutadapt-4.3/src/cutadapt.egg-info/PKG-INFO` & `cutadapt-4.4/src/cutadapt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cutadapt
-Version: 4.3
+Version: 4.4
 Summary: Adapter trimming and other preprocessing of high-throughput sequencing reads
 Author-email: Marcel Martin <marcel.martin@scilifelab.se>
 License: MIT
 Project-URL: Homepage, https://cutadapt.readthedocs.io/
 Project-URL: Changelog, https://cutadapt.readthedocs.io/en/stable/changes.html
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `cutadapt-4.3/src/cutadapt.egg-info/SOURCES.txt` & `cutadapt-4.4/src/cutadapt.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -37,26 +37,29 @@
 src/cutadapt/_align.pyx
 src/cutadapt/_kmer_finder.pyi
 src/cutadapt/_kmer_finder.pyx
 src/cutadapt/_match_tables.py
 src/cutadapt/_version.py
 src/cutadapt/adapters.py
 src/cutadapt/align.py
+src/cutadapt/cli.py
+src/cutadapt/files.py
 src/cutadapt/info.pyi
 src/cutadapt/info.pyx
 src/cutadapt/json.py
 src/cutadapt/kmer_heuristic.py
 src/cutadapt/log.py
 src/cutadapt/modifiers.py
 src/cutadapt/parser.py
 src/cutadapt/pipeline.py
 src/cutadapt/predicates.py
 src/cutadapt/qualtrim.pyi
 src/cutadapt/qualtrim.pyx
 src/cutadapt/report.py
+src/cutadapt/runners.py
 src/cutadapt/statistics.py
 src/cutadapt/steps.py
 src/cutadapt/tokenizer.py
 src/cutadapt/utils.py
 src/cutadapt.egg-info/PKG-INFO
 src/cutadapt.egg-info/SOURCES.txt
 src/cutadapt.egg-info/dependency_links.txt
@@ -173,14 +176,15 @@
 tests/cut/paired.m14.1.fastq
 tests/cut/paired.m14.2.fastq
 tests/cut/pairedq.1.fastq
 tests/cut/pairedq.2.fastq
 tests/cut/pairedu.1.fastq
 tests/cut/pairedu.2.fastq
 tests/cut/plus.fastq
+tests/cut/poly-a.fasta
 tests/cut/polya.fasta
 tests/cut/rename.1.fastq
 tests/cut/rename.2.fastq
 tests/cut/rename.fastq
 tests/cut/rest.fa
 tests/cut/restfront.fa
 tests/cut/revcomp-single-normalize.fastq
```

### Comparing `cutadapt-4.3/tests/conftest.py` & `cutadapt-4.4/tests/conftest.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 import pytest
 from utils import assert_files_equal, datapath, cutpath
-from cutadapt.__main__ import main
+from cutadapt.cli import main
 from cutadapt.report import Statistics
 
 
 @pytest.fixture(params=[1, 2])
 def cores(request):
     return request.param
```

### Comparing `cutadapt-4.3/tests/cut/454.fa` & `cutadapt-4.4/tests/cut/454.fa`

 * *Files identical despite different names*

### Comparing `cutadapt-4.3/tests/cut/anywhere_repeat.fastq` & `cutadapt-4.4/tests/cut/anywhere_repeat.fastq`

 * *Files identical despite different names*

### Comparing `cutadapt-4.3/tests/cut/illumina.fastq` & `cutadapt-4.4/tests/cut/illumina.fastq`

 * *Files identical despite different names*

### Comparing `cutadapt-4.3/tests/cut/illumina.info.txt` & `cutadapt-4.4/tests/cut/illumina.info.txt`

 * *Files identical despite different names*

### Comparing `cutadapt-4.3/tests/cut/illumina5.fastq` & `cutadapt-4.4/tests/cut/illumina5.fastq`

 * *Files identical despite different names*

### Comparing `cutadapt-4.3/tests/cut/illumina5.info.txt` & `cutadapt-4.4/tests/cut/illumina5.info.txt`

 * *Files identical despite different names*

### Comparing `cutadapt-4.3/tests/cut/illumina64.fastq` & `cutadapt-4.4/tests/cut/illumina64.fastq`

 * *Files identical despite different names*

### Comparing `cutadapt-4.3/tests/cut/linked-info.txt` & `cutadapt-4.4/tests/cut/linked-info.txt`

 * *Files identical despite different names*

### Comparing `cutadapt-4.3/tests/cut/overlapb.fa` & `cutadapt-4.4/tests/cut/overlapb.fa`

 * *Files identical despite different names*

### Comparing `cutadapt-4.3/tests/cut/solid-no-zerocap.fastq` & `cutadapt-4.4/tests/cut/solid-no-zerocap.fastq`

 * *Files identical despite different names*

### Comparing `cutadapt-4.3/tests/cut/solidqual.fastq` & `cutadapt-4.4/tests/cut/solidqual.fastq`

 * *Files identical despite different names*

### Comparing `cutadapt-4.3/tests/data/454.fa` & `cutadapt-4.4/tests/data/454.fa`

 * *Files identical despite different names*

### Comparing `cutadapt-4.3/tests/data/E3M.fasta` & `cutadapt-4.4/tests/data/E3M.fasta`

 * *Files identical despite different names*

### Comparing `cutadapt-4.3/tests/data/E3M.qual` & `cutadapt-4.4/tests/data/E3M.qual`

 * *Files identical despite different names*

### Comparing `cutadapt-4.3/tests/data/anywhere_repeat.fastq` & `cutadapt-4.4/tests/data/anywhere_repeat.fastq`

 * *Files identical despite different names*

### Comparing `cutadapt-4.3/tests/data/illumina.fastq.gz` & `cutadapt-4.4/tests/data/illumina.fastq.gz`

 * *Files identical despite different names*

### Comparing `cutadapt-4.3/tests/data/illumina5.fastq` & `cutadapt-4.4/tests/data/illumina5.fastq`

 * *Files identical despite different names*

### Comparing `cutadapt-4.3/tests/data/illumina64.fastq` & `cutadapt-4.4/tests/data/illumina64.fastq`

 * *Files identical despite different names*

### Comparing `cutadapt-4.3/tests/data/interleaved.fastq` & `cutadapt-4.4/tests/data/interleaved.fastq`

 * *Files identical despite different names*

### Comparing `cutadapt-4.3/tests/data/nextseq.fastq` & `cutadapt-4.4/tests/data/nextseq.fastq`

 * *Files identical despite different names*

### Comparing `cutadapt-4.3/tests/data/overlapb.fa` & `cutadapt-4.4/tests/data/overlapb.fa`

 * *Files identical despite different names*

### Comparing `cutadapt-4.3/tests/test_adapters.py` & `cutadapt-4.4/tests/test_adapters.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pytest
 
-from dnaio import Sequence
+from dnaio import SequenceRecord
 from cutadapt.adapters import (
     RemoveAfterMatch,
     RemoveBeforeMatch,
     FrontAdapter,
     BackAdapter,
     PrefixAdapter,
     SuffixAdapter,
@@ -275,15 +275,15 @@
         front_required=True,
         back_required=False,
         name="name",
     )
     assert linked_adapter.front_adapter.min_overlap == 4
     assert linked_adapter.back_adapter.min_overlap == 3
 
-    read = Sequence(name="seq", sequence="AAAACCCCCTTTT")
+    read = SequenceRecord(name="seq", sequence="AAAACCCCCTTTT")
     trimmed = linked_adapter.match_to(read.sequence).trimmed(read)
     assert trimmed.name == "seq"
     assert trimmed.sequence == "CCCCC"
 
 
 def test_linked_adapter_statistics():
     # Issue #615
@@ -325,15 +325,15 @@
         sequence="GAACTCCAGTCACNNNNN",
         max_errors=0.12,
         min_overlap=5,
         read_wildcards=False,
         adapter_wildcards=True,
         name="Foo",
     )
-    read = Sequence(name="abc", sequence="CCCCAGAACTACAGTCCCGGC")
+    read = SequenceRecord(name="abc", sequence="CCCCAGAACTACAGTCCCGGC")
     am = RemoveAfterMatch(
         astart=0,
         astop=17,
         rstart=5,
         rstop=21,
         score=15,
         errors=2,
```

### Comparing `cutadapt-4.3/tests/test_align.py` & `cutadapt-4.4/tests/test_align.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     PrefixComparer,
     SuffixComparer,
     hamming_sphere,
     edit_environment,
     edit_distance,
     naive_edit_environment,
     slow_edit_environment,
+    py_edit_environment,
 )
 from cutadapt.adapters import Where
 
 from utils import binomial
 
 
 class AlignmentResult(NamedTuple):
@@ -464,15 +465,18 @@
         (1, "AAA"),
         (1, "TCATTAGA"),
         (2, "ACC"),
         (2, "A" * 10),
         (3, "TCATTA"),
     ],
 )
-@pytest.mark.parametrize("environment_func", [edit_environment, slow_edit_environment])
+@pytest.mark.parametrize(
+    "environment_func",
+    [edit_environment, slow_edit_environment, py_edit_environment],
+)
 def test_edit_environment(k, s, environment_func):
     result = list(environment_func(s, k))
     strings, distances, matches = zip(*result)
     naive = set(naive_edit_environment(s, k))
     assert len(set(strings)) == len(strings)
     assert set(strings) == naive
 
@@ -483,11 +487,11 @@
         start1, stop1, start2, stop2, score, errors = result
         assert errors == dist
         assert start1 == 0
         assert stop1 == len(s)
         assert start2 == 0
         assert stop2 == len(t)
         assert edit_distance(s, t) == dist
-        if environment_func is edit_environment:
+        if environment_func is py_edit_environment:
             assert m == score
             assert m <= len(s), (s, t, dist)
             assert m <= len(t), (s, t, dist)
```

### Comparing `cutadapt-4.3/tests/test_api.py` & `cutadapt-4.4/tests/test_api.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,23 +6,24 @@
 The tests in this module do not check results, they are just here to
 ensure that the code as shown can be executed.
 """
 import copy
 import json
 import os
 
+from cutadapt.runners import run_pipeline
 from utils import datapath
 
 
 def test_command_line():
     # Call Cutadapt from Python, but pass parameters as a list of strings
     # the same way we would in the shell. The difference is that this is
     # not in a separate process, errors cause a CommandLineError instead
     # of SystemExit, and we get back a Statistics object.
-    from cutadapt.__main__ import main
+    from cutadapt.cli import main
 
     stats = main(["-q", "10", "-o", os.devnull, datapath("small.fastq")])
     assert stats is not None
     json.dumps(stats.as_json())
 
     # TODO
     # - Should not set up logging
@@ -34,18 +35,17 @@
 
 def test_pipeline_single(tmp_path):
     # The following is roughly equivalent to:
     # cutadapt -u 5 -a GATCGGAAGA -q 0,15 -m 10
     #   --discard-untrimmed --info-file=info.txt -o ... small.fastq
     import json
     from cutadapt.pipeline import SingleEndPipeline
-    from cutadapt.utils import FileOpener
+    from cutadapt.files import FileOpener, OutputFiles, InputPaths
     from cutadapt.modifiers import UnconditionalCutter, QualityTrimmer, AdapterCutter
     from cutadapt.adapters import BackAdapter
-    from cutadapt.pipeline import InputPaths, OutputFiles
 
     file_opener = FileOpener()
     adapter = BackAdapter(
         sequence="GATCGGAAGA",
         max_errors=1,
         min_overlap=3,
     )
@@ -57,33 +57,32 @@
     pipeline = SingleEndPipeline(modifiers)
     pipeline.minimum_length = (10,)
     pipeline.discard_untrimmed = True
     inpaths = InputPaths(datapath("small.fastq"))
     info_file = file_opener.xopen_or_none(tmp_path / "info.txt", "wb")
     out = file_opener.xopen(tmp_path / "out.fastq", "wb")
     outfiles = OutputFiles(info=info_file, out=out)
-    stats = pipeline.run(inpaths, outfiles, cores=1)
+    stats = run_pipeline(pipeline, inpaths, outfiles, cores=1)
     assert stats is not None
     json.dumps(stats.as_json())
     outfiles.close()
     # TODO
     # - info file isn’t written, what is missing?
     # - see next function for more TODOs that also apply here
 
 
 def test_pipeline_paired(tmp_path):
     # cutadapt -u 5 -U 7 -a GATCGGAAGA -q 0,15 -m 10:0
     #   --discard-untrimmed --info-file=info.txt
     #   -o ... -p ...
     #   paired.1.fastq paired.2.fastq
     from cutadapt.pipeline import PairedEndPipeline
-    from cutadapt.utils import FileOpener
     from cutadapt.modifiers import UnconditionalCutter, QualityTrimmer, AdapterCutter
     from cutadapt.adapters import BackAdapter
-    from cutadapt.pipeline import InputPaths, OutputFiles
+    from cutadapt.files import OutputFiles, InputPaths, FileOpener
 
     trimmer = QualityTrimmer(cutoff_front=0, cutoff_back=15)
     adapter = BackAdapter(
         sequence="GATCGGAAGA",
         max_errors=1,
         min_overlap=3,
     )
@@ -105,15 +104,15 @@
         tmp_path / "out.1.fastq", tmp_path / "out.2.fastq", "wb"
     )
     outfiles = OutputFiles(
         info=info_file,
         out=out,
         out2=out2,
     )
-    stats = pipeline.run(inpaths, outfiles, cores=1, progress=True)
+    stats = run_pipeline(pipeline, inpaths, outfiles, cores=1, progress=True)
     assert stats is not None
     _ = stats.as_json()
     outfiles.close()
 
     # TODO
     # - could use += for adding modifiers
     # - allow using adapter specification strings?
```

### Comparing `cutadapt-4.3/tests/test_command.py` & `cutadapt-4.4/tests/test_command.py`

 * *Files identical despite different names*

### Comparing `cutadapt-4.3/tests/test_commandline.py` & `cutadapt-4.4/tests/test_commandline.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import sys
 import os
 from io import StringIO, BytesIO
 
 import dnaio
 import pytest
 
-from cutadapt.__main__ import main
+from cutadapt.cli import main
 from utils import assert_files_equal, datapath, cutpath
 
 # pytest.mark.timeout will not fail even if pytest-timeout is not installed
 try:
     import pytest_timeout as _unused
 except ImportError:  # pragma: no cover
     raise ImportError("pytest_timeout needs to be installed")
@@ -260,28 +260,32 @@
 
 
 def test_twoadapters(run):
     """two adapters"""
     run("-a AATTTCAGGAATT -a GTTCTCTAGTTCT", "twoadapters.fasta", "twoadapters.fasta")
 
 
-def test_polya(run):
+def test_poly_a_legacy(run):
     """poly-A tails"""
     run(
         "-m 24 -O 10 -a AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA",
         "polya.fasta",
         "polya.fasta",
     )
 
 
-def test_polya_brace_notation(run):
+def test_poly_a_legacy_brace_notation(run):
     """poly-A tails"""
     run("-m 24 -O 10 -a A{35}", "polya.fasta", "polya.fasta")
 
 
+def test_poly_a(run):
+    run("--poly-a", "poly-a.fasta", "polya.fasta")
+
+
 # the same as --action=none
 def test_no_trim(run):
     run("--no-trim --discard-untrimmed -a CCCTAGTTAAAC", "no-trim.fastq", "small.fastq")
 
 
 def test_action_none(run):
     run(
```

### Comparing `cutadapt-4.3/tests/test_kmer_finder.py` & `cutadapt-4.4/tests/test_kmer_finder.py`

 * *Files identical despite different names*

### Comparing `cutadapt-4.3/tests/test_kmer_heuristic.py` & `cutadapt-4.4/tests/test_kmer_heuristic.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 import pytest
 
 from cutadapt.kmer_heuristic import (
-    kmer_possibilities,
+    kmer_chunks,
     minimize_kmer_search_list,
     create_back_overlap_searchsets,
     create_positions_and_kmers,
 )
 
 
 @pytest.mark.parametrize(
     ["sequence", "chunks", "expected"],
     [
-        ("ABC", 3, [{"A", "B", "C"}]),
-        ("ABCD", 3, [{"A", "B", "CD"}, {"A", "BC", "D"}, {"AB", "C", "D"}]),
+        ("ABC", 3, {"A", "B", "C"}),
+        ("ABCD", 3, {"AB", "C", "D"}),
     ],
 )
-def test_kmer_possibilities(sequence, chunks, expected):
-    frozen_expected = set(frozenset(s) for s in expected)
-    result = kmer_possibilities(sequence, chunks)
-    frozen_result = set(frozenset(s) for s in result)
-    assert frozen_expected == frozen_result
+def test_kmer_chunks(sequence, chunks, expected):
+    assert kmer_chunks(sequence, chunks) == expected
 
 
 @pytest.mark.parametrize(
     ["kmer_search_list", "expected"],
     [
         ([("ABC", -33, None), ("ABC", -19, None)], [("ABC", -33, None)]),
         (
@@ -41,19 +38,19 @@
     assert set(result) == set(expected)
 
 
 def test_create_back_overlap_searchsets():
     adapter = "ABCDEFGHIJ0123456789"
     searchsets = create_back_overlap_searchsets(adapter, 3, 0.1)
     assert len(searchsets) == 5
-    assert (-3, None, [{"ABC"}]) in searchsets
-    assert (-4, None, [{"ABCD"}]) in searchsets
-    assert (-9, None, [{"ABCDE"}]) in searchsets
-    assert (-19, None, kmer_possibilities(adapter[:10], 2)) in searchsets
-    assert (-20, None, kmer_possibilities(adapter, 3)) in searchsets
+    assert (-3, None, {"ABC"}) in searchsets
+    assert (-4, None, {"ABCD"}) in searchsets
+    assert (-9, None, {"ABCDE"}) in searchsets
+    assert (-19, None, kmer_chunks(adapter[:10], 2)) in searchsets
+    assert (-20, None, kmer_chunks(adapter, 3)) in searchsets
 
 
 @pytest.mark.parametrize(
     ["kwargs", "expected"],
     [
         (
             dict(back_adapter=True, front_adapter=False, internal=True, min_overlap=3),
@@ -102,7 +99,21 @@
         adapter,
         error_rate=0.1,
         **kwargs,
     )
     assert {(start, stop): frozenset(kmers) for start, stop, kmers in result} == {
         (start, stop): frozenset(kmers) for start, stop, kmers in expected
     }
+
+
+@pytest.mark.timeout(0.5)
+def test_create_positions_and_kmers_slow():
+    create_positions_and_kmers(
+        # Ridiculous size to check if there aren't any quadratic or exponential
+        # algorithms in the code.
+        "A" * 1000,
+        min_overlap=3,
+        error_rate=0.1,
+        back_adapter=True,
+        front_adapter=False,
+        internal=True,
+    )
```

### Comparing `cutadapt-4.3/tests/test_main.py` & `cutadapt-4.4/tests/test_main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pytest
 
-from cutadapt.__main__ import (
+from cutadapt.cli import (
     main,
     parse_cutoffs,
     parse_lengths,
     CommandLineError,
     setup_logging,
 )
```

### Comparing `cutadapt-4.3/tests/test_modifiers.py` & `cutadapt-4.4/tests/test_modifiers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import List
 
 import pytest
-from dnaio import Sequence
+from dnaio import SequenceRecord
 from cutadapt.adapters import (
     BackAdapter,
     PrefixAdapter,
     IndexedPrefixAdapters,
     LinkedAdapter,
     FrontAdapter,
     Adapter,
@@ -27,15 +27,15 @@
     InvalidTemplate,
     PairedEndRenamer,
 )
 
 
 def test_unconditional_cutter():
     UnconditionalCutter(length=5)
-    read = Sequence("r1", "abcdefg")
+    read = SequenceRecord("r1", "abcdefg")
 
     info = ModificationInfo(read)
     assert UnconditionalCutter(length=2)(read, info).sequence == "cdefg"
     assert info.cut_prefix == "ab"
     assert info.cut_suffix is None
 
     info = ModificationInfo(read)
@@ -51,71 +51,75 @@
     adapters = [
         PrefixAdapter("TTATTTGTCT"),
         PrefixAdapter("TCCGCACTGG"),
     ]
     adapter_cutter = AdapterCutter(adapters, index=False)
     reverse_complementer = ReverseComplementer(adapter_cutter)
 
-    read = Sequence("r", "ttatttgtctCCAGCTTAGACATATCGCCT")
+    read = SequenceRecord("r", "ttatttgtctCCAGCTTAGACATATCGCCT")
     info = ModificationInfo(read)
     trimmed = reverse_complementer(read, info)
     assert trimmed.sequence == "CCAGCTTAGACATATCGCCT"
     assert not info.is_rc
 
-    read = Sequence("r", "CAACAGGCCACATTAGACATATCGGATGGTagacaaataa")
+    read = SequenceRecord("r", "CAACAGGCCACATTAGACATATCGGATGGTagacaaataa")
     info = ModificationInfo(read)
     trimmed = reverse_complementer(read, info)
     assert trimmed.sequence == "ACCATCCGATATGTCTAATGTGGCCTGTTG"
     assert info.is_rc
 
 
 def test_zero_capper():
     zc = ZeroCapper()
-    read = Sequence("r1", "ACGT", "# !%")
+    read = SequenceRecord("r1", "ACGT", "# !%")
     result = zc(read, ModificationInfo(read))
     assert result.sequence == "ACGT"
     assert result.qualities == "#!!%"
 
 
 def test_nend_trimmer():
     trimmer = NEndTrimmer()
     seqs = ["NNNNAAACCTTGGNNN", "NNNNAAACNNNCTTGGNNN", "NNNNNN"]
     trims = ["AAACCTTGG", "AAACNNNCTTGG", ""]
     for seq, trimmed in zip(seqs, trims):
-        _seq = Sequence("read1", seq, qualities="#" * len(seq))
-        _trimmed = Sequence("read1", trimmed, qualities="#" * len(trimmed))
+        _seq = SequenceRecord("read1", seq, qualities="#" * len(seq))
+        _trimmed = SequenceRecord("read1", trimmed, qualities="#" * len(trimmed))
         assert trimmer(_seq, ModificationInfo(_seq)) == _trimmed
 
 
 def test_quality_trimmer():
-    read = Sequence("read1", "ACGTTTACGTA", "##456789###")
+    read = SequenceRecord("read1", "ACGTTTACGTA", "##456789###")
 
     qt = QualityTrimmer(10, 10, 33)
-    assert qt(read, ModificationInfo(read)) == Sequence("read1", "GTTTAC", "456789")
+    assert qt(read, ModificationInfo(read)) == SequenceRecord(
+        "read1", "GTTTAC", "456789"
+    )
 
     qt = QualityTrimmer(0, 10, 33)
-    assert qt(read, ModificationInfo(read)) == Sequence("read1", "ACGTTTAC", "##456789")
+    assert qt(read, ModificationInfo(read)) == SequenceRecord(
+        "read1", "ACGTTTAC", "##456789"
+    )
 
     qt = QualityTrimmer(10, 0, 33)
-    assert qt(read, ModificationInfo(read)) == Sequence(
+    assert qt(read, ModificationInfo(read)) == SequenceRecord(
         "read1", "GTTTACGTA", "456789###"
     )
 
 
 def test_shortener():
-    read = Sequence("read1", "ACGTTTACGTA", "##456789###")
+    read = SequenceRecord("read1", "ACGTTTACGTA", "##456789###")
 
     shortener = Shortener(0)
-    assert shortener(read, ModificationInfo(read)) == Sequence("read1", "", "")
+    assert shortener(read, ModificationInfo(read)) == SequenceRecord("read1", "", "")
 
     shortener = Shortener(1)
-    assert shortener(read, ModificationInfo(read)) == Sequence("read1", "A", "#")
+    assert shortener(read, ModificationInfo(read)) == SequenceRecord("read1", "A", "#")
 
     shortener = Shortener(5)
-    assert shortener(read, ModificationInfo(read)) == Sequence(
+    assert shortener(read, ModificationInfo(read)) == SequenceRecord(
         "read1", "ACGTT", "##456"
     )
 
     shortener = Shortener(100)
     assert shortener(read, ModificationInfo(read)) == read
 
 
@@ -142,30 +146,30 @@
             ("mask", "CCCCNNNNNNNNNN", "TTTTNNNNNNNNNN"),
             ("retain", "CCCCGGTTAA", "TTTTAACCGG"),
         ],
     )
     def test_actions(self, action, expected_trimmed1, expected_trimmed2):
         a1 = BackAdapter("GGTTAA")
         a2 = BackAdapter("AACCGG")
-        s1 = Sequence("name", "CCCCGGTTAACCCC")
-        s2 = Sequence("name", "TTTTAACCGGTTTT")
+        s1 = SequenceRecord("name", "CCCCGGTTAACCCC")
+        s2 = SequenceRecord("name", "TTTTAACCGGTTTT")
         pac = PairedAdapterCutter([a1], [a2], action=action)
         info1 = ModificationInfo(s1)
         info2 = ModificationInfo(s2)
         trimmed1, trimmed2 = pac(s1, s2, info1, info2)
         assert expected_trimmed1 == trimmed1.sequence
         assert expected_trimmed2 == trimmed2.sequence
 
     def test_multiple_occurrences(self):
         r1_a1 = BackAdapter("AAAAAA")
         r1_a2 = BackAdapter("CCCC")
         r2_a1 = BackAdapter("GGGG")
         r2_a2 = BackAdapter("TTTT")
-        s1 = Sequence("name", "TTAAAAAATTCCCCTT")
-        s2 = Sequence("name", "ACACTTTTACAC")
+        s1 = SequenceRecord("name", "TTAAAAAATTCCCCTT")
+        s2 = SequenceRecord("name", "ACACTTTTACAC")
         pac = PairedAdapterCutter([r1_a1, r1_a2], [r2_a1, r2_a2], action="lowercase")
         info1 = ModificationInfo(s1)
         info2 = ModificationInfo(s2)
         trimmed1, trimmed2 = pac(s1, s2, info1, info2)
         assert len(info1.matches) == 1 and info1.matches[0].adapter is r1_a2
         assert len(info2.matches) == 1 and info2.matches[0].adapter is r2_a2
         assert "TTAAAAAATTcccctt" == trimmed1.sequence
@@ -177,15 +181,15 @@
         AdapterCutter([BackAdapter("ACGT")], times=2, action="retain")
     assert "cannot be combined with times" in e.value.args[0]
 
 
 def test_action_retain():
     back = BackAdapter("AACCGG")
     ac = AdapterCutter([back], action="retain")
-    seq = Sequence("r1", "ATTGCCAACCGGTATATAT")
+    seq = SequenceRecord("r1", "ATTGCCAACCGGTATATAT")
     info = ModificationInfo(seq)
     trimmed = ac(seq, info)
     assert "ATTGCCAACCGG" == trimmed.sequence
 
 
 @pytest.mark.parametrize(
     "s,expected",
@@ -201,82 +205,82 @@
     back = BackAdapter("AACCGG")
     adapters: List[Adapter] = [
         LinkedAdapter(
             front, back, front_required=False, back_required=False, name="linked"
         )
     ]
     ac = AdapterCutter(adapters, action="retain")
-    seq = Sequence("r1", s)
+    seq = SequenceRecord("r1", s)
     info = ModificationInfo(seq)
     trimmed = ac(seq, info)
     assert expected == trimmed.sequence
 
 
 class TestRenamer:
     def test_invalid_template_variable(self):
         with pytest.raises(InvalidTemplate):
             Renamer("{id} {invalid}")
 
     def test_header_template_variable(self):
         renamer = Renamer("{header} extra")
-        read = Sequence("theid thecomment", "ACGT")
+        read = SequenceRecord("theid thecomment", "ACGT")
         info = ModificationInfo(read)
         assert renamer(read, info).name == "theid thecomment extra"
 
     def test_id_template_variable(self):
         renamer = Renamer("{id} extra")
-        read = Sequence("theid thecomment", "ACGT")
+        read = SequenceRecord("theid thecomment", "ACGT")
         info = ModificationInfo(read)
         assert renamer(read, info).name == "theid extra"
 
     def test_tab_escape(self):
         renamer = Renamer(r"{id} extra\tand a tab")
-        read = Sequence("theid thecomment", "ACGT")
+        read = SequenceRecord("theid thecomment", "ACGT")
         info = ModificationInfo(read)
         assert renamer(read, info).name == "theid extra\tand a tab"
 
     def test_comment_template_variable(self):
         renamer = Renamer("{id}_extra {comment}")
-        read = Sequence("theid thecomment", "ACGT")
+        read = SequenceRecord("theid thecomment", "ACGT")
         info = ModificationInfo(read)
         assert renamer(read, info).name == "theid_extra thecomment"
 
     def test_comment_template_variable_missing_comment(self):
         renamer = Renamer("{id}_extra {comment}")
-        read = Sequence("theid", "ACGT")
+        read = SequenceRecord("theid", "ACGT")
         info = ModificationInfo(read)
         assert renamer(read, info).name == "theid_extra "
 
     def test_cut_prefix_template_variable(self):
         renamer = Renamer("{id}_{cut_prefix} {comment}")
-        read = Sequence("theid thecomment", "ACGT")
+        read = SequenceRecord("theid thecomment", "ACGT")
         info = ModificationInfo(read)
         info.cut_prefix = "TTAAGG"
         assert renamer(read, info).name == "theid_TTAAGG thecomment"
 
     def test_cut_suffix_template_variable(self):
         renamer = Renamer("{id}_{cut_suffix} {comment}")
-        read = Sequence("theid thecomment", "ACGT")
+        read = SequenceRecord("theid thecomment", "ACGT")
         info = ModificationInfo(read)
         info.cut_suffix = "TTAAGG"
         assert renamer(read, info).name == "theid_TTAAGG thecomment"
 
     def test_rc_template_variable(self):
         renamer = Renamer("{id} rc={rc} {comment}")
-        read = Sequence("theid thecomment", "ACGT")
+        read = SequenceRecord("theid thecomment", "ACGT")
         info = ModificationInfo(read)
         assert renamer(read, info).name == "theid rc= thecomment"
 
-        read = Sequence("theid thecomment", "ACGT")
+        read = SequenceRecord("theid thecomment", "ACGT")
         info.is_rc = True
         assert renamer(read, info).name == "theid rc=rc thecomment"
 
     def test_match_sequence(self):
         sequence = "TTTTCCCCACGTGGGG"
-        read = Sequence("theid thecomment", sequence)
+        read = SequenceRecord("theid thecomment", sequence)
         adapter = BackAdapter("AGGT")
         info = ModificationInfo(read)
         info.matches.append(
             RemoveBeforeMatch(
                 astart=0,
                 astop=4,
                 rstart=8,
@@ -291,15 +295,15 @@
 
         renamer(read, info)
 
         assert read.name == "theid thecomment match=ACGT"
 
     def test_match_sequence_linked_match(self):
         sequence = "TATTCCCCACGTGGGG"
-        read = Sequence("theid thecomment", sequence)
+        read = SequenceRecord("theid thecomment", sequence)
         adapter1 = PrefixAdapter("TTTT")
         adapter2 = BackAdapter("AGGT")
         linked_adapter = LinkedAdapter(
             adapter1,
             adapter2,
             front_required=True,
             back_required=False,
@@ -337,88 +341,88 @@
 class TestPairedEndRenamer:
     def test_invalid_template_variable(self):
         with pytest.raises(InvalidTemplate):
             PairedEndRenamer("{id} {invalid}")
 
     def test_tab_escape(self):
         renamer = PairedEndRenamer(r"{id} {comment}\tand a tab")
-        r1 = Sequence("theid comment1", "ACGT")
-        r2 = Sequence("theid comment2", "ACGT")
+        r1 = SequenceRecord("theid comment1", "ACGT")
+        r2 = SequenceRecord("theid comment2", "ACGT")
         info1 = ModificationInfo(r1)
         info2 = ModificationInfo(r2)
         renamed1, renamed2 = renamer(r1, r2, info1, info2)
         assert renamed1.name == "theid comment1\tand a tab"
         assert renamed2.name == "theid comment2\tand a tab"
 
     def test_ids_not_identical(self):
         renamer = PairedEndRenamer("{id} abc {comment} xyz")
-        r1 = Sequence("theid_a cmtx", "ACGT")
-        r2 = Sequence("theid_b cmty", "ACGT")
+        r1 = SequenceRecord("theid_a cmtx", "ACGT")
+        r2 = SequenceRecord("theid_b cmty", "ACGT")
         info1 = ModificationInfo(r1)
         info2 = ModificationInfo(r2)
         with pytest.raises(ValueError) as e:
             renamer(r1, r2, info1, info2)
         assert "not identical" in e.value.args[0]
 
     def test_comment(self):
         renamer = PairedEndRenamer("{id} abc {comment} xyz")
-        r1 = Sequence("theid cmtx", "ACGT")
-        r2 = Sequence("theid cmty", "ACGT")
+        r1 = SequenceRecord("theid cmtx", "ACGT")
+        r2 = SequenceRecord("theid cmty", "ACGT")
         info1 = ModificationInfo(r1)
         info2 = ModificationInfo(r2)
         renamed1, renamed2 = renamer(r1, r2, info1, info2)
         assert renamed1.name == "theid abc cmtx xyz"
         assert renamed2.name == "theid abc cmty xyz"
 
     def test_r1_comment(self):
         renamer = PairedEndRenamer("{id} abc {r1.comment} xyz")
-        r1 = Sequence("theid cmtx", "ACGT")
-        r2 = Sequence("theid cmty", "ACGT")
+        r1 = SequenceRecord("theid cmtx", "ACGT")
+        r2 = SequenceRecord("theid cmty", "ACGT")
         info1 = ModificationInfo(r1)
         info2 = ModificationInfo(r2)
         renamed1, renamed2 = renamer(r1, r2, info1, info2)
         assert renamed1.name == "theid abc cmtx xyz"
         assert renamed2.name == "theid abc cmtx xyz"
 
     def test_r2_comment(self):
         renamer = PairedEndRenamer("{id} abc {r2.comment} xyz")
-        r1 = Sequence("theid cmtx", "ACGT")
-        r2 = Sequence("theid cmty", "ACGT")
+        r1 = SequenceRecord("theid cmtx", "ACGT")
+        r2 = SequenceRecord("theid cmty", "ACGT")
         info1 = ModificationInfo(r1)
         info2 = ModificationInfo(r2)
         renamed1, renamed2 = renamer(r1, r2, info1, info2)
         assert renamed1.name == "theid abc cmty xyz"
         assert renamed2.name == "theid abc cmty xyz"
 
     def test_read_number(self):
         renamer = PairedEndRenamer("{id} read no. is: {rn}")
-        r1 = Sequence("theid cmtx", "ACGT")
-        r2 = Sequence("theid cmty", "ACGT")
+        r1 = SequenceRecord("theid cmtx", "ACGT")
+        r2 = SequenceRecord("theid cmty", "ACGT")
         info1 = ModificationInfo(r1)
         info2 = ModificationInfo(r2)
         renamed1, renamed2 = renamer(r1, r2, info1, info2)
         assert renamed1.name == "theid read no. is: 1"
         assert renamed2.name == "theid read no. is: 2"
 
     def test_match_sequence(self):
-        r1 = Sequence("theid first", "AACC")
+        r1 = SequenceRecord("theid first", "AACC")
         info1 = ModificationInfo(r1)
         info1.matches.append(
             RemoveBeforeMatch(
                 astart=2,
                 astop=4,
                 rstart=1,
                 rstop=3,
                 score=1,
                 errors=1,
                 adapter=FrontAdapter("AT"),
                 sequence="AACC",
             )
         )
-        r2 = Sequence("theid second", "GGTT")
+        r2 = SequenceRecord("theid second", "GGTT")
         info2 = ModificationInfo(r2)
         info2.matches.append(
             RemoveBeforeMatch(
                 astart=2,
                 astop=4,
                 rstart=1,
                 rstop=3,
```

### Comparing `cutadapt-4.3/tests/test_paired.py` & `cutadapt-4.4/tests/test_paired.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import os.path
 import shutil
 from itertools import product
 
 import pytest
 
-from cutadapt.__main__ import main
+from cutadapt.cli import main
 from utils import assert_files_equal, datapath, cutpath
 
 
 @pytest.fixture
 def run_paired(tmp_path):
     def _run(params, in1, in2, expected1, expected2, cores):
         if type(params) is str:
```

### Comparing `cutadapt-4.3/tests/test_parser.py` & `cutadapt-4.4/tests/test_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 from textwrap import dedent
 import pytest
 
-from dnaio import Sequence
+from dnaio import SequenceRecord
 from cutadapt.adapters import (
     LinkedAdapter,
     BackAdapter,
     FrontAdapter,
     InvalidCharacter,
     PrefixAdapter,
     RightmostFrontAdapter,
@@ -472,15 +472,15 @@
 
 def test_anywhere_parameter_back():
     adapter = make_adapter("CTGAAGTGAAGTACACGGTT;anywhere", "back", dict())
     assert isinstance(adapter, BackAdapter)
     assert adapter._force_anywhere
 
     # TODO move the rest to a separate test
-    read = Sequence("foo1", "TGAAGTACACGGTTAAAAAAAAAA")
+    read = SequenceRecord("foo1", "TGAAGTACACGGTTAAAAAAAAAA")
     from cutadapt.modifiers import AdapterCutter
 
     cutter = AdapterCutter([adapter])
     trimmed_read = cutter(read, ModificationInfo(read))
     assert trimmed_read.sequence == ""
 
 
@@ -492,15 +492,15 @@
 
 def test_anywhere_parameter_front():
     adapter = make_adapter("CTGAAGTGAAGTACACGGTT;anywhere", "front", dict())
     assert isinstance(adapter, FrontAdapter)
     assert adapter._force_anywhere
 
     # TODO move the rest to a separate test
-    read = Sequence("foo1", "AAAAAAAAAACTGAAGTGAA")
+    read = SequenceRecord("foo1", "AAAAAAAAAACTGAAGTGAA")
     from cutadapt.modifiers import AdapterCutter
 
     cutter = AdapterCutter([adapter])
     trimmed_read = cutter(read, ModificationInfo(read))
     assert trimmed_read.sequence == ""
```

### Comparing `cutadapt-4.3/tests/test_predicates.py` & `cutadapt-4.4/tests/test_predicates.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Tests write output (should it return True or False or write)
 """
 import pytest
-from dnaio import Sequence
+from dnaio import SequenceRecord
 
 from cutadapt.predicates import TooManyN
 from cutadapt.steps import PairedEndFilter
 
 
 @pytest.mark.parametrize(
     "seq,count,expected",
@@ -19,15 +19,15 @@
         ("ANAAAA", 1 / 6, False),
         ("ANAAAA", 0, True),
     ],
 )
 def test_too_many_n(seq, count, expected):
     # third parameter is True if read should be Trueed
     predicate = TooManyN(count=count)
-    _seq = Sequence("read1", seq, qualities="#" * len(seq))
+    _seq = SequenceRecord("read1", seq, qualities="#" * len(seq))
     assert predicate.test(_seq, []) == expected
 
 
 @pytest.mark.parametrize(
     "seq1,seq2,count,expected",
     [
         ("AAA", "AAA", 0, False),
@@ -38,18 +38,18 @@
 )
 def test_too_many_n_paired(seq1, seq2, count, expected):
     predicate = TooManyN(count=count)
     filter_legacy = PairedEndFilter(
         predicate, predicate, None, pair_filter_mode="first"
     )
     filter_any = PairedEndFilter(predicate, predicate, None, pair_filter_mode="any")
-    read1 = Sequence("read1", seq1, qualities="#" * len(seq1))
-    read2 = Sequence("read1", seq2, qualities="#" * len(seq2))
-    assert filter_legacy(read1, read2, [], []) == predicate.test(read1, [])
+    read1 = SequenceRecord("read1", seq1, qualities="#" * len(seq1))
+    read2 = SequenceRecord("read1", seq2, qualities="#" * len(seq2))
+    assert (filter_legacy(read1, read2, [], []) is None) == predicate.test(read1, [])
     # True entire pair if one of the reads fulfills criteria
-    assert filter_any(read1, read2, [], []) == expected
+    assert (filter_any(read1, read2, [], []) is None) == expected
 
 
 def test_invalid_pair_filter_mode():
     with pytest.raises(ValueError) as e:
         PairedEndFilter(None, None, None, "invalidmode")
     assert "pair_filter_mode must be" in e.value.args[0]
```

### Comparing `cutadapt-4.3/tests/test_stats.py` & `cutadapt-4.4/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `cutadapt-4.3/tests/test_tokenizer.py` & `cutadapt-4.4/tests/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `cutadapt-4.3/tests/test_trim.py` & `cutadapt-4.4/tests/test_trim.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import typing
 
-from dnaio import Sequence
+from dnaio import SequenceRecord
 from cutadapt.adapters import (
     BackAdapter,
     AnywhereAdapter,
     BackAdapterStatistics,
     Adapter,
 )
 from cutadapt.modifiers import AdapterCutter, ModificationInfo
 
 
 def test_statistics() -> None:
-    read = Sequence("name", "AAAACCCCAAAA")
-    adapters: typing.Sequence[Adapter] = [BackAdapter("CCCC", max_errors=0.1)]
+    read = SequenceRecord("name", "AAAACCCCAAAA")
+    adapters: typing.SequenceRecord[Adapter] = [BackAdapter("CCCC", max_errors=0.1)]
     cutter = AdapterCutter(adapters, times=3)
     cutter(read, ModificationInfo(read))
     assert isinstance(cutter.adapter_statistics[adapters[0]], BackAdapterStatistics)
     lengths = cutter.adapter_statistics[adapters[0]].end.lengths
     trimmed_bp = sum(seqlen * count for (seqlen, count) in lengths.items())
     assert trimmed_bp <= len(read), trimmed_bp
 
@@ -27,25 +27,25 @@
     the end of a sequence with overlap 9 and there is one deletion.
     In this case the algorithm starts with 10 bases of the adapter to get
     the hit and so the match is considered good. An insertion or substitution
     at the same spot is not a match.
     """
     adapter = BackAdapter("TCGATCGATCGAT", max_errors=0.1)
 
-    read = Sequence("foo1", "AAAAAAAAAAATCGTCGATC")
+    read = SequenceRecord("foo1", "AAAAAAAAAAATCGTCGATC")
     cutter = AdapterCutter([adapter], times=1)
     trimmed_read = cutter(read, ModificationInfo(read))
 
     assert trimmed_read.sequence == "AAAAAAAAAAA"
     assert cutter.adapter_statistics[adapter].end.lengths == {9: 1}
     # We see 1 error at length 9 even though the number of allowed mismatches at
     # length 9 is 0.
     assert cutter.adapter_statistics[adapter].end.errors[9][1] == 1
 
-    read = Sequence("foo2", "AAAAAAAAAAATCGAACGA")
+    read = SequenceRecord("foo2", "AAAAAAAAAAATCGAACGA")
     cutter = AdapterCutter([adapter], times=1)
     trimmed_read = cutter(read, ModificationInfo(read))
 
     assert trimmed_read.sequence == read.sequence
     assert cutter.adapter_statistics[adapter].end.lengths == {}
 
 
@@ -55,11 +55,11 @@
         ("AACCGGTTccgcatttagGATC", "AACCGGTT"),
         ("AACCGGTTccgcgtttagGATC", "AACCGGTT"),  # one mismatch
         ("AACCGGTTccgcatttag", "AACCGGTT"),
         ("ccgcatttagAACCGGTT", "AACCGGTT"),
         ("ccgtatttagAACCGGTT", "AACCGGTT"),  # one mismatch
         ("ccgatttagAACCGGTT", "AACCGGTT"),  # one deletion
     ):
-        read = Sequence("foo", seq)
+        read = SequenceRecord("foo", seq)
         cutter = AdapterCutter([adapter], times=1)
         trimmed_read = cutter(read, ModificationInfo(read))
         assert trimmed_read.sequence == expected_trimmed
```

### Comparing `cutadapt-4.3/tests/utils.py` & `cutadapt-4.4/tests/utils.py`

 * *Files identical despite different names*

### Comparing `cutadapt-4.3/tox.ini` & `cutadapt-4.4/tox.ini`

 * *Files identical despite different names*

