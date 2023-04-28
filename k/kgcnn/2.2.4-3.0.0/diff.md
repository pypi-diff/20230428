# Comparing `tmp/kgcnn-2.2.4.tar.gz` & `tmp/kgcnn-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kgcnn-2.2.4.tar", last modified: Fri Apr 28 07:23:56 2023, max compression
+gzip compressed data, was "kgcnn-3.0.0.tar", last modified: Fri Apr 28 07:25:09 2023, max compression
```

## Comparing `kgcnn-2.2.4.tar` & `kgcnn-3.0.0.tar`

### file list

```diff
@@ -1,242 +1,333 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 07:23:56.237417 kgcnn-2.2.4/
--rw-rw-rw-   0        0        0       76 2023-04-28 07:07:45.000000 kgcnn-2.2.4/AUTHORS
--rw-rw-rw-   0        0        0     1066 2023-04-28 07:07:45.000000 kgcnn-2.2.4/LICENSE
--rw-rw-rw-   0        0        0       47 2023-04-28 07:07:45.000000 kgcnn-2.2.4/MANIFEST.in
--rw-rw-rw-   0        0        0    18659 2023-04-28 07:23:56.236418 kgcnn-2.2.4/PKG-INFO
--rw-rw-rw-   0        0        0    17783 2023-04-28 07:07:45.000000 kgcnn-2.2.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-28 07:23:54.423745 kgcnn-2.2.4/kgcnn/
--rw-rw-rw-   0        0        0       42 2023-04-28 07:07:46.000000 kgcnn-2.2.4/kgcnn/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:23:54.566705 kgcnn-2.2.4/kgcnn/crystal/
--rw-rw-rw-   0        0        0        0 2023-04-28 07:07:46.000000 kgcnn-2.2.4/kgcnn/crystal/__init__.py
--rw-rw-rw-   0        0        0      801 2023-04-28 07:07:46.000000 kgcnn-2.2.4/kgcnn/crystal/base.py
--rw-rw-rw-   0        0        0    16129 2023-04-28 07:07:46.000000 kgcnn-2.2.4/kgcnn/crystal/graph_builder.py
--rw-rw-rw-   0        0        0     5945 2023-04-28 07:07:46.000000 kgcnn-2.2.4/kgcnn/crystal/preprocessor.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:23:54.654176 kgcnn-2.2.4/kgcnn/data/
--rw-rw-rw-   0        0        0        1 2023-04-28 07:07:46.000000 kgcnn-2.2.4/kgcnn/data/__init__.py
--rw-rw-rw-   0        0        0    34079 2023-04-28 07:07:46.000000 kgcnn-2.2.4/kgcnn/data/base.py
--rw-rw-rw-   0        0        0    12792 2023-04-28 07:07:46.000000 kgcnn-2.2.4/kgcnn/data/crystal.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:23:54.951606 kgcnn-2.2.4/kgcnn/data/datasets/
--rw-rw-rw-   0        0        0     3036 2023-04-28 07:07:47.000000 kgcnn-2.2.4/kgcnn/data/datasets/ClinToxDataset.py
--rw-rw-rw-   0        0        0     3182 2023-04-28 07:07:47.000000 kgcnn-2.2.4/kgcnn/data/datasets/CoraDataset.py
--rw-rw-rw-   0        0        0     4761 2023-04-28 07:07:47.000000 kgcnn-2.2.4/kgcnn/data/datasets/CoraLuDataset.py
--rw-rw-rw-   0        0        0     1559 2023-04-28 07:07:47.000000 kgcnn-2.2.4/kgcnn/data/datasets/ESOLDataset.py
--rw-rw-rw-   0        0        0     1727 2023-04-28 07:07:47.000000 kgcnn-2.2.4/kgcnn/data/datasets/FreeSolvDataset.py
--rw-rw-rw-   0        0        0     5398 2023-04-28 07:07:47.000000 kgcnn-2.2.4/kgcnn/data/datasets/GraphTUDataset2020.py
--rw-rw-rw-   0        0        0     7113 2023-04-28 07:07:47.000000 kgcnn-2.2.4/kgcnn/data/datasets/ISO17Dataset.py
--rw-rw-rw-   0        0        0     1471 2023-04-28 07:07:47.000000 kgcnn-2.2.4/kgcnn/data/datasets/LipopDataset.py
--rw-rw-rw-   0        0        0     8792 2023-04-28 07:07:47.000000 kgcnn-2.2.4/kgcnn/data/datasets/MD17Dataset.py
--rw-rw-rw-   0        0        0     6574 2023-04-28 07:07:47.000000 kgcnn-2.2.4/kgcnn/data/datasets/MD17RevisedDataset.py
--rw-rw-rw-   0        0        0     3158 2023-04-28 07:07:47.000000 kgcnn-2.2.4/kgcnn/data/datasets/MUTAGDataset.py
--rw-rw-rw-   0        0        0    11255 2023-04-28 07:07:47.000000 kgcnn-2.2.4/kgcnn/data/datasets/MatBenchDataset2020.py
--rw-rw-rw-   0        0        0     1469 2023-04-28 07:07:47.000000 kgcnn-2.2.4/kgcnn/data/datasets/MatProjectDielectricDataset.py
--rw-rw-rw-   0        0        0     1388 2023-04-28 07:07:47.000000 kgcnn-2.2.4/kgcnn/data/datasets/MatProjectEFormDataset.py
--rw-rw-rw-   0        0        0     1398 2023-04-28 07:07:47.000000 kgcnn-2.2.4/kgcnn/data/datasets/MatProjectGapDataset.py
--rw-rw-rw-   0        0        0     1424 2023-04-28 07:07:47.000000 kgcnn-2.2.4/kgcnn/data/datasets/MatProjectIsMetalDataset.py
--rw-rw-rw-   0        0        0     1325 2023-04-28 07:07:47.000000 kgcnn-2.2.4/kgcnn/data/datasets/MatProjectJdft2dDataset.py
--rw-rw-rw-   0        0        0     1605 2023-04-28 07:07:47.000000 kgcnn-2.2.4/kgcnn/data/datasets/MatProjectLogGVRHDataset.py
--rw-rw-rw-   0        0        0     1604 2023-04-28 07:07:47.000000 kgcnn-2.2.4/kgcnn/data/datasets/MatProjectLogKVRHDataset.py
--rw-rw-rw-   0        0        0     1316 2023-04-28 07:07:47.000000 kgcnn-2.2.4/kgcnn/data/datasets/MatProjectPerovskitesDataset.py
--rw-rw-rw-   0        0        0     1693 2023-04-28 07:07:47.000000 kgcnn-2.2.4/kgcnn/data/datasets/MatProjectPhononsDataset.py
--rw-rw-rw-   0        0        0     8589 2023-04-28 07:07:47.000000 kgcnn-2.2.4/kgcnn/data/datasets/MoleculeNetDataset2018.py
--rw-rw-rw-   0        0        0     4834 2023-04-28 07:07:47.000000 kgcnn-2.2.4/kgcnn/data/datasets/MutagenicityDataset.py
--rw-rw-rw-   0        0        0     3046 2023-04-28 07:07:47.000000 kgcnn-2.2.4/kgcnn/data/datasets/PROTEINSDataset.py
--rw-rw-rw-   0        0        0     6558 2023-04-28 07:07:47.000000 kgcnn-2.2.4/kgcnn/data/datasets/QM7Dataset.py
--rw-rw-rw-   0        0        0     5516 2023-04-28 07:07:47.000000 kgcnn-2.2.4/kgcnn/data/datasets/QM7bDataset.py
--rw-rw-rw-   0        0        0     3922 2023-04-28 07:07:47.000000 kgcnn-2.2.4/kgcnn/data/datasets/QM8Dataset.py
--rw-rw-rw-   0        0        0    12250 2023-04-28 07:07:47.000000 kgcnn-2.2.4/kgcnn/data/datasets/QM9Dataset.py
--rw-rw-rw-   0        0        0     2952 2023-04-28 07:07:47.000000 kgcnn-2.2.4/kgcnn/data/datasets/QM9MolNetDataset.py
--rw-rw-rw-   0        0        0     2160 2023-04-28 07:07:47.000000 kgcnn-2.2.4/kgcnn/data/datasets/SIDERDataset.py
--rw-rw-rw-   0        0        0     2194 2023-04-28 07:07:47.000000 kgcnn-2.2.4/kgcnn/data/datasets/Tox21MolNetDataset.py
--rw-rw-rw-   0        0        0      426 2023-04-28 07:07:47.000000 kgcnn-2.2.4/kgcnn/data/datasets/VgdMockDataset.py
--rw-rw-rw-   0        0        0      597 2023-04-28 07:07:47.000000 kgcnn-2.2.4/kgcnn/data/datasets/VgdRbMotifsDataset.py
--rw-rw-rw-   0        0        0        1 2023-04-28 07:07:47.000000 kgcnn-2.2.4/kgcnn/data/datasets/__init__.py
--rw-rw-rw-   0        0        0    12525 2023-04-28 07:07:46.000000 kgcnn-2.2.4/kgcnn/data/download.py
--rw-rw-rw-   0        0        0    22963 2023-04-28 07:07:47.000000 kgcnn-2.2.4/kgcnn/data/moleculenet.py
--rw-rw-rw-   0        0        0    17746 2023-04-28 07:15:12.000000 kgcnn-2.2.4/kgcnn/data/qm.py
--rw-rw-rw-   0        0        0     2851 2023-04-28 07:07:47.000000 kgcnn-2.2.4/kgcnn/data/serial.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:23:54.953613 kgcnn-2.2.4/kgcnn/data/transform/
--rw-rw-rw-   0        0        0        0 2023-04-28 07:07:47.000000 kgcnn-2.2.4/kgcnn/data/transform/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:23:54.996608 kgcnn-2.2.4/kgcnn/data/transform/scaler/
--rw-rw-rw-   0        0        0        0 2023-04-28 07:07:47.000000 kgcnn-2.2.4/kgcnn/data/transform/scaler/__init__.py
--rw-rw-rw-   0        0        0    19614 2023-04-28 07:07:48.000000 kgcnn-2.2.4/kgcnn/data/transform/scaler/force.py
--rw-rw-rw-   0        0        0    53863 2023-04-28 07:07:48.000000 kgcnn-2.2.4/kgcnn/data/transform/scaler/mol.py
--rw-rw-rw-   0        0        0    27716 2023-04-28 07:07:48.000000 kgcnn-2.2.4/kgcnn/data/transform/scaler/scaler.py
--rw-rw-rw-   0        0        0     1908 2023-04-28 07:07:48.000000 kgcnn-2.2.4/kgcnn/data/transform/scaler/serial.py
--rw-rw-rw-   0        0        0     9367 2023-04-28 07:07:47.000000 kgcnn-2.2.4/kgcnn/data/tudataset.py
--rw-rw-rw-   0        0        0     5298 2023-04-28 07:07:47.000000 kgcnn-2.2.4/kgcnn/data/utils.py
--rw-rw-rw-   0        0        0     8860 2023-04-28 07:07:47.000000 kgcnn-2.2.4/kgcnn/data/visual_graph.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:23:55.060606 kgcnn-2.2.4/kgcnn/graph/
--rw-rw-rw-   0        0        0        0 2023-04-28 07:07:48.000000 kgcnn-2.2.4/kgcnn/graph/__init__.py
--rw-rw-rw-   0        0        0    28421 2023-04-28 07:07:48.000000 kgcnn-2.2.4/kgcnn/graph/adj.py
--rw-rw-rw-   0        0        0    25764 2023-04-28 07:07:48.000000 kgcnn-2.2.4/kgcnn/graph/base.py
--rw-rw-rw-   0        0        0    23582 2023-04-28 07:07:48.000000 kgcnn-2.2.4/kgcnn/graph/geom.py
--rw-rw-rw-   0        0        0     1864 2023-04-28 07:07:48.000000 kgcnn-2.2.4/kgcnn/graph/postprocessor.py
--rw-rw-rw-   0        0        0    31815 2023-04-28 07:07:48.000000 kgcnn-2.2.4/kgcnn/graph/preprocessor.py
--rw-rw-rw-   0        0        0     2468 2023-04-28 07:07:48.000000 kgcnn-2.2.4/kgcnn/graph/serial.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:23:55.074605 kgcnn-2.2.4/kgcnn/hyper/
--rw-rw-rw-   0        0        0        0 2023-04-28 07:07:48.000000 kgcnn-2.2.4/kgcnn/hyper/__init__.py
--rw-rw-rw-   0        0        0    14935 2023-04-28 07:07:48.000000 kgcnn-2.2.4/kgcnn/hyper/hyper.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:23:55.077607 kgcnn-2.2.4/kgcnn/io/
--rw-rw-rw-   0        0        0        0 2023-04-28 07:07:48.000000 kgcnn-2.2.4/kgcnn/io/__init__.py
--rw-rw-rw-   0        0        0     4054 2023-04-28 07:07:48.000000 kgcnn-2.2.4/kgcnn/io/loader.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:23:55.192606 kgcnn-2.2.4/kgcnn/layers/
--rw-rw-rw-   0        0        0     1322 2023-04-28 07:07:48.000000 kgcnn-2.2.4/kgcnn/layers/README.md
--rw-rw-rw-   0        0        0        1 2023-04-28 07:07:48.000000 kgcnn-2.2.4/kgcnn/layers/__init__.py
--rw-rw-rw-   0        0        0     7693 2023-04-28 07:07:48.000000 kgcnn-2.2.4/kgcnn/layers/base.py
--rw-rw-rw-   0        0        0    12507 2023-04-28 07:07:48.000000 kgcnn-2.2.4/kgcnn/layers/casting.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:23:55.409627 kgcnn-2.2.4/kgcnn/layers/conv/
--rw-rw-rw-   0        0        0      101 2023-04-28 07:07:48.000000 kgcnn-2.2.4/kgcnn/layers/conv/__init__.py
--rw-rw-rw-   0        0        0    25733 2023-04-28 07:07:48.000000 kgcnn-2.2.4/kgcnn/layers/conv/acsf_conv.py
--rw-rw-rw-   0        0        0    12186 2023-04-28 07:07:48.000000 kgcnn-2.2.4/kgcnn/layers/conv/attentivefp_conv.py
--rw-rw-rw-   0        0        0     6468 2023-04-28 07:07:48.000000 kgcnn-2.2.4/kgcnn/layers/conv/cgcnn_conv.py
--rw-rw-rw-   0        0        0    22252 2023-04-28 07:07:48.000000 kgcnn-2.2.4/kgcnn/layers/conv/dimenet_conv.py
--rw-rw-rw-   0        0        0     3939 2023-04-28 07:07:48.000000 kgcnn-2.2.4/kgcnn/layers/conv/dmpnn_conv.py
--rw-rw-rw-   0        0        0    15540 2023-04-28 07:07:48.000000 kgcnn-2.2.4/kgcnn/layers/conv/gat_conv.py
--rw-rw-rw-   0        0        0     7112 2023-04-28 07:07:48.000000 kgcnn-2.2.4/kgcnn/layers/conv/gcn_conv.py
--rw-rw-rw-   0        0        0     6634 2023-04-28 07:07:48.000000 kgcnn-2.2.4/kgcnn/layers/conv/gin_conv.py
--rw-rw-rw-   0        0        0    30822 2023-04-28 07:07:48.000000 kgcnn-2.2.4/kgcnn/layers/conv/hamnet_conv.py
--rw-rw-rw-   0        0        0    25834 2023-04-28 07:07:48.000000 kgcnn-2.2.4/kgcnn/layers/conv/hdnnp_conv.py
--rw-rw-rw-   0        0        0     8987 2023-04-28 07:07:48.000000 kgcnn-2.2.4/kgcnn/layers/conv/mat_conv.py
--rw-rw-rw-   0        0        0     7153 2023-04-28 07:07:48.000000 kgcnn-2.2.4/kgcnn/layers/conv/megnet_conv.py
--rw-rw-rw-   0        0        0    10529 2023-04-28 07:07:48.000000 kgcnn-2.2.4/kgcnn/layers/conv/mpnn_conv.py
--rw-rw-rw-   0        0        0     8501 2023-04-28 07:07:49.000000 kgcnn-2.2.4/kgcnn/layers/conv/mxmnet_conv.py
--rw-rw-rw-   0        0        0    15451 2023-04-28 07:07:49.000000 kgcnn-2.2.4/kgcnn/layers/conv/painn_conv.py
--rw-rw-rw-   0        0        0        0 2023-04-28 07:07:49.000000 kgcnn-2.2.4/kgcnn/layers/conv/rgcn_conv.py
--rw-rw-rw-   0        0        0     9857 2023-04-28 07:07:49.000000 kgcnn-2.2.4/kgcnn/layers/conv/sage_conv.py
--rw-rw-rw-   0        0        0     8444 2023-04-28 07:07:49.000000 kgcnn-2.2.4/kgcnn/layers/conv/schnet_conv.py
--rw-rw-rw-   0        0        0        3 2023-04-28 07:07:49.000000 kgcnn-2.2.4/kgcnn/layers/conv/vgae_conv.py
--rw-rw-rw-   0        0        0    21072 2023-04-28 07:07:49.000000 kgcnn-2.2.4/kgcnn/layers/conv/wacsf_conv.py
--rw-rw-rw-   0        0        0    17264 2023-04-28 07:07:48.000000 kgcnn-2.2.4/kgcnn/layers/gather.py
--rw-rw-rw-   0        0        0    43155 2023-04-28 07:07:48.000000 kgcnn-2.2.4/kgcnn/layers/geom.py
--rw-rw-rw-   0        0        0     4735 2023-04-28 07:07:48.000000 kgcnn-2.2.4/kgcnn/layers/message.py
--rw-rw-rw-   0        0        0    18206 2023-04-28 07:07:48.000000 kgcnn-2.2.4/kgcnn/layers/mlp.py
--rw-rw-rw-   0        0        0    23450 2023-04-28 07:07:48.000000 kgcnn-2.2.4/kgcnn/layers/modules.py
--rw-rw-rw-   0        0        0    28771 2023-04-28 07:07:48.000000 kgcnn-2.2.4/kgcnn/layers/norm.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:23:55.437627 kgcnn-2.2.4/kgcnn/layers/pool/
--rw-rw-rw-   0        0        0        1 2023-04-28 07:07:49.000000 kgcnn-2.2.4/kgcnn/layers/pool/__init__.py
--rw-rw-rw-   0        0        0    13924 2023-04-28 07:07:49.000000 kgcnn-2.2.4/kgcnn/layers/pool/set2set.py
--rw-rw-rw-   0        0        0    19993 2023-04-28 07:07:49.000000 kgcnn-2.2.4/kgcnn/layers/pool/topk.py
--rw-rw-rw-   0        0        0    35807 2023-04-28 07:07:48.000000 kgcnn-2.2.4/kgcnn/layers/pooling.py
--rw-rw-rw-   0        0        0    11852 2023-04-28 07:07:48.000000 kgcnn-2.2.4/kgcnn/layers/relational.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:23:55.715627 kgcnn-2.2.4/kgcnn/literature/
--rw-rw-rw-   0        0        0     5926 2023-04-28 07:07:49.000000 kgcnn-2.2.4/kgcnn/literature/AttentiveFP.py
--rw-rw-rw-   0        0        0     9374 2023-04-28 07:07:49.000000 kgcnn-2.2.4/kgcnn/literature/CGCNN.py
--rw-rw-rw-   0        0        0     8176 2023-04-28 07:07:49.000000 kgcnn-2.2.4/kgcnn/literature/CMPNN.py
--rw-rw-rw-   0        0        0     8382 2023-04-28 07:07:49.000000 kgcnn-2.2.4/kgcnn/literature/DMPNN.py
--rw-rw-rw-   0        0        0    18292 2023-04-28 07:07:49.000000 kgcnn-2.2.4/kgcnn/literature/DimeNetPP.py
--rw-rw-rw-   0        0        0    10063 2023-04-28 07:07:49.000000 kgcnn-2.2.4/kgcnn/literature/EGNN.py
--rw-rw-rw-   0        0        0     5929 2023-04-28 07:07:49.000000 kgcnn-2.2.4/kgcnn/literature/GAT.py
--rw-rw-rw-   0        0        0     6283 2023-04-28 07:07:49.000000 kgcnn-2.2.4/kgcnn/literature/GATv2.py
--rw-rw-rw-   0        0        0    10429 2023-04-28 07:07:49.000000 kgcnn-2.2.4/kgcnn/literature/GCN.py
--rw-rw-rw-   0        0        0    10915 2023-04-28 07:07:49.000000 kgcnn-2.2.4/kgcnn/literature/GIN.py
--rw-rw-rw-   0        0        0    30112 2023-04-28 07:07:49.000000 kgcnn-2.2.4/kgcnn/literature/GNNExplain.py
--rw-rw-rw-   0        0        0     5613 2023-04-28 07:07:49.000000 kgcnn-2.2.4/kgcnn/literature/GNNFilm.py
--rw-rw-rw-   0        0        0     6852 2023-04-28 07:07:49.000000 kgcnn-2.2.4/kgcnn/literature/GraphSAGE.py
--rw-rw-rw-   0        0        0    15732 2023-04-28 07:07:49.000000 kgcnn-2.2.4/kgcnn/literature/HDNNP2nd.py
--rw-rw-rw-   0        0        0     8177 2023-04-28 07:07:49.000000 kgcnn-2.2.4/kgcnn/literature/HDNNP4th.py
--rw-rw-rw-   0        0        0     8249 2023-04-28 07:07:49.000000 kgcnn-2.2.4/kgcnn/literature/HamNet.py
--rw-rw-rw-   0        0        0     8214 2023-04-28 07:07:49.000000 kgcnn-2.2.4/kgcnn/literature/INorp.py
--rw-rw-rw-   0        0        0     9740 2023-04-28 07:07:49.000000 kgcnn-2.2.4/kgcnn/literature/MAT.py
--rw-rw-rw-   0        0        0    23677 2023-04-28 07:07:49.000000 kgcnn-2.2.4/kgcnn/literature/MEGAN.py
--rw-rw-rw-   0        0        0    10177 2023-04-28 07:07:49.000000 kgcnn-2.2.4/kgcnn/literature/MXMNet.py
--rw-rw-rw-   0        0        0    18841 2023-04-28 07:07:49.000000 kgcnn-2.2.4/kgcnn/literature/Megnet.py
--rw-rw-rw-   0        0        0    17476 2023-04-28 07:07:49.000000 kgcnn-2.2.4/kgcnn/literature/NMPN.py
--rw-rw-rw-   0        0        0    14418 2023-04-28 07:07:49.000000 kgcnn-2.2.4/kgcnn/literature/PAiNN.py
--rw-rw-rw-   0        0        0     5668 2023-04-28 07:07:49.000000 kgcnn-2.2.4/kgcnn/literature/RGCN.py
--rw-rw-rw-   0        0        0    14558 2023-04-28 07:07:49.000000 kgcnn-2.2.4/kgcnn/literature/Schnet.py
--rw-rw-rw-   0        0        0     7330 2023-04-28 07:07:49.000000 kgcnn-2.2.4/kgcnn/literature/Unet.py
--rw-rw-rw-   0        0        0        1 2023-04-28 07:07:49.000000 kgcnn-2.2.4/kgcnn/literature/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:23:55.738628 kgcnn-2.2.4/kgcnn/metrics/
--rw-rw-rw-   0        0        0        0 2023-04-28 07:07:49.000000 kgcnn-2.2.4/kgcnn/metrics/__init__.py
--rw-rw-rw-   0        0        0      972 2023-04-28 07:07:49.000000 kgcnn-2.2.4/kgcnn/metrics/loss.py
--rw-rw-rw-   0        0        0    10804 2023-04-28 07:07:50.000000 kgcnn-2.2.4/kgcnn/metrics/metrics.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:23:55.774627 kgcnn-2.2.4/kgcnn/model/
--rw-rw-rw-   0        0        0        0 2023-04-28 07:07:50.000000 kgcnn-2.2.4/kgcnn/model/README.md
--rw-rw-rw-   0        0        0        0 2023-04-28 07:07:50.000000 kgcnn-2.2.4/kgcnn/model/__init__.py
--rw-rw-rw-   0        0        0     8946 2023-04-28 07:07:50.000000 kgcnn-2.2.4/kgcnn/model/force.py
--rw-rw-rw-   0        0        0       18 2023-04-28 07:07:50.000000 kgcnn-2.2.4/kgcnn/model/serial.py
--rw-rw-rw-   0        0        0     5430 2023-04-28 07:07:50.000000 kgcnn-2.2.4/kgcnn/model/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:23:55.874629 kgcnn-2.2.4/kgcnn/mol/
--rw-rw-rw-   0        0        0        0 2023-04-28 07:07:50.000000 kgcnn-2.2.4/kgcnn/mol/__init__.py
--rw-rw-rw-   0        0        0    10056 2023-04-28 07:07:50.000000 kgcnn-2.2.4/kgcnn/mol/base.py
--rw-rw-rw-   0        0        0    12151 2023-04-28 07:07:50.000000 kgcnn-2.2.4/kgcnn/mol/convert.py
--rw-rw-rw-   0        0        0     2556 2023-04-28 07:07:50.000000 kgcnn-2.2.4/kgcnn/mol/encoder.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:23:55.892627 kgcnn-2.2.4/kgcnn/mol/external/
--rw-rw-rw-   0        0        0        1 2023-04-28 07:07:50.000000 kgcnn-2.2.4/kgcnn/mol/external/__init__.py
--rw-rw-rw-   0        0        0    20790 2023-04-28 07:07:50.000000 kgcnn-2.2.4/kgcnn/mol/external/ballloon.py
--rw-rw-rw-   0        0        0    17887 2023-04-28 07:07:50.000000 kgcnn-2.2.4/kgcnn/mol/graph_babel.py
--rw-rw-rw-   0        0        0    20209 2023-04-28 07:07:50.000000 kgcnn-2.2.4/kgcnn/mol/graph_rdkit.py
--rw-rw-rw-   0        0        0     8959 2023-04-28 07:07:50.000000 kgcnn-2.2.4/kgcnn/mol/io.py
--rw-rw-rw-   0        0        0     5100 2023-04-28 07:07:50.000000 kgcnn-2.2.4/kgcnn/mol/methods.py
--rw-rw-rw-   0        0        0      697 2023-04-28 07:07:50.000000 kgcnn-2.2.4/kgcnn/mol/serial.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:23:55.910628 kgcnn-2.2.4/kgcnn/moldyn/
--rw-rw-rw-   0        0        0        0 2023-04-28 07:07:50.000000 kgcnn-2.2.4/kgcnn/moldyn/__init__.py
--rw-rw-rw-   0        0        0     3911 2023-04-28 07:07:50.000000 kgcnn-2.2.4/kgcnn/moldyn/ase_calc.py
--rw-rw-rw-   0        0        0     8386 2023-04-28 07:07:50.000000 kgcnn-2.2.4/kgcnn/moldyn/base.py
--rw-rw-rw-   0        0        0        0 2023-04-28 07:07:50.000000 kgcnn-2.2.4/kgcnn/moldyn/newx_calc.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:23:55.972040 kgcnn-2.2.4/kgcnn/ops/
--rw-rw-rw-   0        0        0        0 2023-04-28 07:07:50.000000 kgcnn-2.2.4/kgcnn/ops/__init__.py
--rw-rw-rw-   0        0        0     3851 2023-04-28 07:07:50.000000 kgcnn-2.2.4/kgcnn/ops/activ.py
--rw-rw-rw-   0        0        0     1483 2023-04-28 07:07:50.000000 kgcnn-2.2.4/kgcnn/ops/axis.py
--rw-rw-rw-   0        0        0        0 2023-04-28 07:07:50.000000 kgcnn-2.2.4/kgcnn/ops/casting.py
--rw-rw-rw-   0        0        0     2169 2023-04-28 07:07:50.000000 kgcnn-2.2.4/kgcnn/ops/initializer.py
--rw-rw-rw-   0        0        0     8290 2023-04-28 07:07:50.000000 kgcnn-2.2.4/kgcnn/ops/partition.py
--rw-rw-rw-   0        0        0    10223 2023-04-28 07:07:50.000000 kgcnn-2.2.4/kgcnn/ops/polynom.py
--rw-rw-rw-   0        0        0     3181 2023-04-28 07:07:50.000000 kgcnn-2.2.4/kgcnn/ops/ragged.py
--rw-rw-rw-   0        0        0     1148 2023-04-28 07:07:50.000000 kgcnn-2.2.4/kgcnn/ops/scatter.py
--rw-rw-rw-   0        0        0     2046 2023-04-28 07:07:50.000000 kgcnn-2.2.4/kgcnn/ops/segment.py
--rw-rw-rw-   0        0        0        0 2023-04-28 07:07:50.000000 kgcnn-2.2.4/kgcnn/ops/sorting.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:23:55.978473 kgcnn-2.2.4/kgcnn/scaler/
--rw-rw-rw-   0        0        0        0 2023-04-28 07:07:50.000000 kgcnn-2.2.4/kgcnn/scaler/__init__.py
--rw-rw-rw-   0        0        0      229 2023-04-28 07:07:50.000000 kgcnn-2.2.4/kgcnn/scaler/force.py
--rw-rw-rw-   0        0        0      227 2023-04-28 07:07:50.000000 kgcnn-2.2.4/kgcnn/scaler/mol.py
--rw-rw-rw-   0        0        0      230 2023-04-28 07:07:50.000000 kgcnn-2.2.4/kgcnn/scaler/scaler.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:23:56.031417 kgcnn-2.2.4/kgcnn/training/
--rw-rw-rw-   0        0        0        0 2023-04-28 07:07:50.000000 kgcnn-2.2.4/kgcnn/training/__init__.py
--rw-rw-rw-   0        0        0     1220 2023-04-28 07:07:50.000000 kgcnn-2.2.4/kgcnn/training/callbacks.py
--rw-rw-rw-   0        0        0     4643 2023-04-28 07:07:50.000000 kgcnn-2.2.4/kgcnn/training/history.py
--rw-rw-rw-   0        0        0     8691 2023-04-28 07:07:50.000000 kgcnn-2.2.4/kgcnn/training/optimizer.py
--rw-rw-rw-   0        0        0     2092 2023-04-28 07:07:50.000000 kgcnn-2.2.4/kgcnn/training/schedule.py
--rw-rw-rw-   0        0        0    16405 2023-04-28 07:07:50.000000 kgcnn-2.2.4/kgcnn/training/scheduler.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:23:56.062418 kgcnn-2.2.4/kgcnn/utils/
--rw-rw-rw-   0        0        0        1 2023-04-28 07:07:50.000000 kgcnn-2.2.4/kgcnn/utils/__init__.py
--rw-rw-rw-   0        0        0      501 2023-04-28 07:07:50.000000 kgcnn-2.2.4/kgcnn/utils/cli.py
--rw-rw-rw-   0        0        0     2248 2023-04-28 07:07:50.000000 kgcnn-2.2.4/kgcnn/utils/devices.py
--rw-rw-rw-   0        0        0      204 2023-04-28 07:07:51.000000 kgcnn-2.2.4/kgcnn/utils/models.py
--rw-rw-rw-   0        0        0     7356 2023-04-28 07:07:51.000000 kgcnn-2.2.4/kgcnn/utils/plots.py
--rw-rw-rw-   0        0        0     2307 2023-04-28 07:07:51.000000 kgcnn-2.2.4/kgcnn/utils/serial.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:23:56.071417 kgcnn-2.2.4/kgcnn/xai/
--rw-rw-rw-   0        0        0        0 2023-04-28 07:07:51.000000 kgcnn-2.2.4/kgcnn/xai/__init__.py
--rw-rw-rw-   0        0        0     2456 2023-04-28 07:07:51.000000 kgcnn-2.2.4/kgcnn/xai/base.py
--rw-rw-rw-   0        0        0     4480 2023-04-28 07:07:51.000000 kgcnn-2.2.4/kgcnn/xai/testing.py
--rw-rw-rw-   0        0        0      774 2023-04-28 07:07:51.000000 kgcnn-2.2.4/kgcnn/xai/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:23:54.500760 kgcnn-2.2.4/kgcnn.egg-info/
--rw-rw-rw-   0        0        0    18659 2023-04-28 07:23:54.000000 kgcnn-2.2.4/kgcnn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5864 2023-04-28 07:23:54.000000 kgcnn-2.2.4/kgcnn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 07:23:54.000000 kgcnn-2.2.4/kgcnn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      328 2023-04-28 07:23:54.000000 kgcnn-2.2.4/kgcnn.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-28 07:23:54.000000 kgcnn-2.2.4/kgcnn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-28 07:23:56.237417 kgcnn-2.2.4/setup.cfg
--rw-rw-rw-   0        0        0     1931 2023-04-28 07:07:45.000000 kgcnn-2.2.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:23:56.226416 kgcnn-2.2.4/test/
--rw-rw-rw-   0        0        0        0 2023-04-28 07:07:51.000000 kgcnn-2.2.4/test/__init__.py
--rw-rw-rw-   0        0        0     4141 2023-04-28 07:07:51.000000 kgcnn-2.2.4/test/test_adj.py
--rw-rw-rw-   0        0        0     1134 2023-04-28 07:07:51.000000 kgcnn-2.2.4/test/test_connect.py
--rw-rw-rw-   0        0        0     5172 2023-04-28 07:07:51.000000 kgcnn-2.2.4/test/test_conv_attention.py
--rw-rw-rw-   0        0        0     1272 2023-04-28 07:07:51.000000 kgcnn-2.2.4/test/test_conv_dmpnn.py
--rw-rw-rw-   0        0        0     4986 2023-04-28 07:07:51.000000 kgcnn-2.2.4/test/test_data_base.py
--rw-rw-rw-   0        0        0     7921 2023-04-28 07:07:51.000000 kgcnn-2.2.4/test/test_data_moleculenet.py
--rw-rw-rw-   0        0        0     1444 2023-04-28 07:07:51.000000 kgcnn-2.2.4/test/test_data_visual_graph.py
--rw-rw-rw-   0        0        0     2972 2023-04-28 07:07:51.000000 kgcnn-2.2.4/test/test_gather.py
--rw-rw-rw-   0        0        0     7473 2023-04-28 07:07:51.000000 kgcnn-2.2.4/test/test_geom.py
--rw-rw-rw-   0        0        0     1255 2023-04-28 07:07:51.000000 kgcnn-2.2.4/test/test_graph_base.py
--rw-rw-rw-   0        0        0     9433 2023-04-28 07:07:51.000000 kgcnn-2.2.4/test/test_hdnnp.py
--rw-rw-rw-   0        0        0     1265 2023-04-28 07:07:51.000000 kgcnn-2.2.4/test/test_literature_gnnexplain.py
--rw-rw-rw-   0        0        0     6865 2023-04-28 07:07:51.000000 kgcnn-2.2.4/test/test_literature_megan.py
--rw-rw-rw-   0        0        0     2338 2023-04-28 07:07:51.000000 kgcnn-2.2.4/test/test_pool_pooling.py
--rw-rw-rw-   0        0        0     8075 2023-04-28 07:07:51.000000 kgcnn-2.2.4/test/test_range_periodic.py
--rw-rw-rw-   0        0        0     4109 2023-04-28 07:07:51.000000 kgcnn-2.2.4/test/test_topk.py
--rw-rw-rw-   0        0        0     1140 2023-04-28 07:07:51.000000 kgcnn-2.2.4/test/test_xai_base.py
--rw-rw-rw-   0        0        0      936 2023-04-28 07:07:52.000000 kgcnn-2.2.4/test/test_xai_testing.py
--rw-rw-rw-   0        0        0      568 2023-04-28 07:07:52.000000 kgcnn-2.2.4/test/test_xai_utils.py
--rw-rw-rw-   0        0        0      118 2023-04-28 07:07:52.000000 kgcnn-2.2.4/test/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-28 07:25:09.578677 kgcnn-3.0.0/
+-rw-rw-rw-   0        0        0       76 2023-04-28 07:07:15.000000 kgcnn-3.0.0/AUTHORS
+-rw-rw-rw-   0        0        0     1066 2023-04-28 07:07:15.000000 kgcnn-3.0.0/LICENSE
+-rw-rw-rw-   0        0        0       47 2023-04-28 07:07:15.000000 kgcnn-3.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    19415 2023-04-28 07:25:09.577678 kgcnn-3.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0    18539 2023-04-28 07:07:15.000000 kgcnn-3.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-28 07:25:07.497322 kgcnn-3.0.0/kgcnn/
+-rw-rw-rw-   0        0        0       43 2023-04-28 07:07:17.000000 kgcnn-3.0.0/kgcnn/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 07:25:07.564322 kgcnn-3.0.0/kgcnn/crystal/
+-rw-rw-rw-   0        0        0        0 2023-04-28 07:07:17.000000 kgcnn-3.0.0/kgcnn/crystal/__init__.py
+-rw-rw-rw-   0        0        0     2814 2023-04-28 07:07:17.000000 kgcnn-3.0.0/kgcnn/crystal/base.py
+-rw-rw-rw-   0        0        0    32196 2023-04-28 07:07:17.000000 kgcnn-3.0.0/kgcnn/crystal/graph_builder.py
+drwxrwxrwx   0        0        0        0 2023-04-28 07:25:07.577323 kgcnn-3.0.0/kgcnn/crystal/periodic_table/
+-rw-rw-rw-   0        0        0        0 2023-04-28 07:07:17.000000 kgcnn-3.0.0/kgcnn/crystal/periodic_table/__init__.py
+-rw-rw-rw-   0        0        0     4029 2023-04-28 07:07:17.000000 kgcnn-3.0.0/kgcnn/crystal/periodic_table/periodic_table.py
+-rw-rw-rw-   0        0        0    21221 2023-04-28 07:07:17.000000 kgcnn-3.0.0/kgcnn/crystal/preprocessor.py
+drwxrwxrwx   0        0        0        0 2023-04-28 07:25:07.658321 kgcnn-3.0.0/kgcnn/data/
+-rw-rw-rw-   0        0        0        1 2023-04-28 07:07:17.000000 kgcnn-3.0.0/kgcnn/data/__init__.py
+-rw-rw-rw-   0        0        0    34079 2023-04-28 07:07:17.000000 kgcnn-3.0.0/kgcnn/data/base.py
+-rw-rw-rw-   0        0        0    12744 2023-04-28 07:07:17.000000 kgcnn-3.0.0/kgcnn/data/crystal.py
+drwxrwxrwx   0        0        0        0 2023-04-28 07:25:07.863324 kgcnn-3.0.0/kgcnn/data/datasets/
+-rw-rw-rw-   0        0        0     3036 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/datasets/ClinToxDataset.py
+-rw-rw-rw-   0        0        0     3186 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/datasets/CoraDataset.py
+-rw-rw-rw-   0        0        0     4761 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/datasets/CoraLuDataset.py
+-rw-rw-rw-   0        0        0     1559 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/datasets/ESOLDataset.py
+-rw-rw-rw-   0        0        0     1727 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/datasets/FreeSolvDataset.py
+-rw-rw-rw-   0        0        0     5398 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/datasets/GraphTUDataset2020.py
+-rw-rw-rw-   0        0        0     7113 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/datasets/ISO17Dataset.py
+-rw-rw-rw-   0        0        0     1471 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/datasets/LipopDataset.py
+-rw-rw-rw-   0        0        0     8792 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/datasets/MD17Dataset.py
+-rw-rw-rw-   0        0        0     6574 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/datasets/MD17RevisedDataset.py
+-rw-rw-rw-   0        0        0     3158 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/datasets/MUTAGDataset.py
+-rw-rw-rw-   0        0        0    11255 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/datasets/MatBenchDataset2020.py
+-rw-rw-rw-   0        0        0     1469 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/datasets/MatProjectDielectricDataset.py
+-rw-rw-rw-   0        0        0     1388 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/datasets/MatProjectEFormDataset.py
+-rw-rw-rw-   0        0        0     1398 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/datasets/MatProjectGapDataset.py
+-rw-rw-rw-   0        0        0     1424 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/datasets/MatProjectIsMetalDataset.py
+-rw-rw-rw-   0        0        0     1325 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/datasets/MatProjectJdft2dDataset.py
+-rw-rw-rw-   0        0        0     1605 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/datasets/MatProjectLogGVRHDataset.py
+-rw-rw-rw-   0        0        0     1604 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/datasets/MatProjectLogKVRHDataset.py
+-rw-rw-rw-   0        0        0     1316 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/datasets/MatProjectPerovskitesDataset.py
+-rw-rw-rw-   0        0        0     1693 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/datasets/MatProjectPhononsDataset.py
+-rw-rw-rw-   0        0        0     8589 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/datasets/MoleculeNetDataset2018.py
+-rw-rw-rw-   0        0        0     4834 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/datasets/MutagenicityDataset.py
+-rw-rw-rw-   0        0        0     3051 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/datasets/PROTEINSDataset.py
+-rw-rw-rw-   0        0        0     6575 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/datasets/QM7Dataset.py
+-rw-rw-rw-   0        0        0     5533 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/datasets/QM7bDataset.py
+-rw-rw-rw-   0        0        0     3922 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/datasets/QM8Dataset.py
+-rw-rw-rw-   0        0        0    12255 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/datasets/QM9Dataset.py
+-rw-rw-rw-   0        0        0     2952 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/datasets/QM9MolNetDataset.py
+-rw-rw-rw-   0        0        0     2160 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/datasets/SIDERDataset.py
+-rw-rw-rw-   0        0        0     2194 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/datasets/Tox21MolNetDataset.py
+-rw-rw-rw-   0        0        0        1 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/datasets/__init__.py
+-rw-rw-rw-   0        0        0    12525 2023-04-28 07:07:17.000000 kgcnn-3.0.0/kgcnn/data/download.py
+-rw-rw-rw-   0        0        0    22993 2023-04-28 07:07:17.000000 kgcnn-3.0.0/kgcnn/data/moleculenet.py
+-rw-rw-rw-   0        0        0    17786 2023-04-28 07:15:56.000000 kgcnn-3.0.0/kgcnn/data/qm.py
+-rw-rw-rw-   0        0        0     2851 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/serial.py
+drwxrwxrwx   0        0        0        0 2023-04-28 07:25:07.866324 kgcnn-3.0.0/kgcnn/data/transform/
+-rw-rw-rw-   0        0        0        0 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/transform/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/transform/base.py
+drwxrwxrwx   0        0        0        0 2023-04-28 07:25:07.918321 kgcnn-3.0.0/kgcnn/data/transform/scaler/
+-rw-rw-rw-   0        0        0        0 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/transform/scaler/__init__.py
+-rw-rw-rw-   0        0        0    19619 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/transform/scaler/force.py
+-rw-rw-rw-   0        0        0    53863 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/transform/scaler/molecule.py
+-rw-rw-rw-   0        0        0     1816 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/transform/scaler/serial.py
+-rw-rw-rw-   0        0        0    27716 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/data/transform/scaler/standard.py
+-rw-rw-rw-   0        0        0     9408 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/tudataset.py
+-rw-rw-rw-   0        0        0     5311 2023-04-28 07:07:18.000000 kgcnn-3.0.0/kgcnn/data/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-28 07:25:07.959323 kgcnn-3.0.0/kgcnn/graph/
+-rw-rw-rw-   0        0        0        0 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/graph/__init__.py
+-rw-rw-rw-   0        0        0    26596 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/graph/base.py
+drwxrwxrwx   0        0        0        0 2023-04-28 07:25:07.987324 kgcnn-3.0.0/kgcnn/graph/methods/
+-rw-rw-rw-   0        0        0     1246 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/graph/methods/__init__.py
+-rw-rw-rw-   0        0        0    28421 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/graph/methods/_adj.py
+-rw-rw-rw-   0        0        0    23582 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/graph/methods/_geom.py
+-rw-rw-rw-   0        0        0     1864 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/graph/postprocessor.py
+-rw-rw-rw-   0        0        0    31335 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/graph/preprocessor.py
+-rw-rw-rw-   0        0        0     2468 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/graph/serial.py
+drwxrwxrwx   0        0        0        0 2023-04-28 07:25:07.998321 kgcnn-3.0.0/kgcnn/hyper/
+-rw-rw-rw-   0        0        0        0 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/hyper/__init__.py
+-rw-rw-rw-   0        0        0      209 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/hyper/hyper.py
+drwxrwxrwx   0        0        0        0 2023-04-28 07:25:08.010321 kgcnn-3.0.0/kgcnn/io/
+-rw-rw-rw-   0        0        0        0 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/io/__init__.py
+-rw-rw-rw-   0        0        0     4055 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/io/loader.py
+drwxrwxrwx   0        0        0        0 2023-04-28 07:25:08.217322 kgcnn-3.0.0/kgcnn/layers/
+-rw-rw-rw-   0        0        0     1095 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/layers/README.md
+-rw-rw-rw-   0        0        0        1 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/layers/__init__.py
+-rw-rw-rw-   0        0        0    15544 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/layers/attention.py
+-rw-rw-rw-   0        0        0     7693 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/layers/base.py
+-rw-rw-rw-   0        0        0    12507 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/layers/casting.py
+-rw-rw-rw-   0        0        0    15115 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/layers/conv.py
+-rw-rw-rw-   0        0        0    19063 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/layers/gather.py
+-rw-rw-rw-   0        0        0    43155 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/layers/geom.py
+-rw-rw-rw-   0        0        0     4735 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/layers/message.py
+-rw-rw-rw-   0        0        0    18206 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/layers/mlp.py
+-rw-rw-rw-   0        0        0    23450 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/layers/modules.py
+-rw-rw-rw-   0        0        0    28771 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/layers/norm.py
+-rw-rw-rw-   0        0        0    35808 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/layers/pooling.py
+-rw-rw-rw-   0        0        0    11853 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/layers/relational.py
+-rw-rw-rw-   0        0        0    13549 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/layers/set2set.py
+-rw-rw-rw-   0        0        0     8702 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/layers/update.py
+drwxrwxrwx   0        0        0        0 2023-04-28 07:25:08.219323 kgcnn-3.0.0/kgcnn/literature/
+drwxrwxrwx   0        0        0        0 2023-04-28 07:25:08.279322 kgcnn-3.0.0/kgcnn/literature/AttentiveFP/
+-rw-rw-rw-   0        0        0       99 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/literature/AttentiveFP/__init__.py
+-rw-rw-rw-   0        0        0    12186 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/literature/AttentiveFP/_attentivefp_conv.py
+-rw-rw-rw-   0        0        0     5902 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/literature/AttentiveFP/_make.py
+drwxrwxrwx   0        0        0        0 2023-04-28 07:25:08.368674 kgcnn-3.0.0/kgcnn/literature/CGCNN/
+-rw-rw-rw-   0        0        0      130 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/literature/CGCNN/__init__.py
+-rw-rw-rw-   0        0        0     6471 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/literature/CGCNN/_cgcnn_conv.py
+-rw-rw-rw-   0        0        0     9358 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/literature/CGCNN/_make.py
+drwxrwxrwx   0        0        0        0 2023-04-28 07:25:08.382928 kgcnn-3.0.0/kgcnn/literature/CMPNN/
+-rw-rw-rw-   0        0        0       98 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/literature/CMPNN/__init__.py
+-rw-rw-rw-   0        0        0     8126 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/literature/CMPNN/_make.py
+drwxrwxrwx   0        0        0        0 2023-04-28 07:25:08.407928 kgcnn-3.0.0/kgcnn/literature/DGIN/
+-rw-rw-rw-   0        0        0      100 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/literature/DGIN/__init__.py
+-rw-rw-rw-   0        0        0     4927 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/literature/DGIN/_dgin_conv.py
+-rw-rw-rw-   0        0        0    10250 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/literature/DGIN/_make.py
+drwxrwxrwx   0        0        0        0 2023-04-28 07:25:08.433548 kgcnn-3.0.0/kgcnn/literature/DMPNN/
+-rw-rw-rw-   0        0        0       98 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/DMPNN/__init__.py
+-rw-rw-rw-   0        0        0     2117 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/DMPNN/_dmpnn_conv.py
+-rw-rw-rw-   0        0        0     8366 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/DMPNN/_make.py
+drwxrwxrwx   0        0        0        0 2023-04-28 07:25:08.468547 kgcnn-3.0.0/kgcnn/literature/DimeNetPP/
+-rw-rw-rw-   0        0        0      215 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/DimeNetPP/__init__.py
+-rw-rw-rw-   0        0        0    19372 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/DimeNetPP/_dimenet_conv.py
+-rw-rw-rw-   0        0        0    18270 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/DimeNetPP/_make.py
+drwxrwxrwx   0        0        0        0 2023-04-28 07:25:08.482548 kgcnn-3.0.0/kgcnn/literature/EGNN/
+-rw-rw-rw-   0        0        0       98 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/EGNN/__init__.py
+-rw-rw-rw-   0        0        0    10063 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/EGNN/_make.py
+drwxrwxrwx   0        0        0        0 2023-04-28 07:25:08.496548 kgcnn-3.0.0/kgcnn/literature/GAT/
+-rw-rw-rw-   0        0        0       98 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/GAT/__init__.py
+-rw-rw-rw-   0        0        0     5925 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/GAT/_make.py
+drwxrwxrwx   0        0        0        0 2023-04-28 07:25:08.502550 kgcnn-3.0.0/kgcnn/literature/GATv2/
+-rw-rw-rw-   0        0        0       98 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/GATv2/__init__.py
+-rw-rw-rw-   0        0        0     6279 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/GATv2/_make.py
+drwxrwxrwx   0        0        0        0 2023-04-28 07:25:08.536548 kgcnn-3.0.0/kgcnn/literature/GCN/
+-rw-rw-rw-   0        0        0      218 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/GCN/__init__.py
+-rw-rw-rw-   0        0        0     1874 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/GCN/_gcn_conv.py
+-rw-rw-rw-   0        0        0    10192 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/GCN/_make.py
+drwxrwxrwx   0        0        0        0 2023-04-28 07:25:08.563550 kgcnn-3.0.0/kgcnn/literature/GIN/
+-rw-rw-rw-   0        0        0      202 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/GIN/__init__.py
+-rw-rw-rw-   0        0        0     6634 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/GIN/_gin_conv.py
+-rw-rw-rw-   0        0        0    10899 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/GIN/_make.py
+drwxrwxrwx   0        0        0        0 2023-04-28 07:25:08.616549 kgcnn-3.0.0/kgcnn/literature/GNNExplain/
+-rw-rw-rw-   0        0        0      187 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/GNNExplain/__init__.py
+-rw-rw-rw-   0        0        0    30109 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/GNNExplain/_model.py
+-rw-rw-rw-   0        0        0     1262 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/GNNExplain/_test_literature_gnnexplain.py
+-rw-rw-rw-   0        0        0     1134 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/GNNExplain/_test_xai_base.py
+-rw-rw-rw-   0        0        0      933 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/GNNExplain/_test_xai_testing.py
+-rw-rw-rw-   0        0        0      565 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/GNNExplain/_test_xai_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-28 07:25:08.634551 kgcnn-3.0.0/kgcnn/literature/GNNExplain/_xai/
+-rw-rw-rw-   0        0        0        0 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/GNNExplain/_xai/__init__.py
+-rw-rw-rw-   0        0        0     2456 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/GNNExplain/_xai/_base.py
+-rw-rw-rw-   0        0        0     4459 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/GNNExplain/_xai/_testing.py
+-rw-rw-rw-   0        0        0      774 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/GNNExplain/_xai/_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-28 07:25:08.641550 kgcnn-3.0.0/kgcnn/literature/GNNFilm/
+-rw-rw-rw-   0        0        0       99 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/GNNFilm/__init__.py
+-rw-rw-rw-   0        0        0     5606 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/GNNFilm/_make.py
+drwxrwxrwx   0        0        0        0 2023-04-28 07:25:08.643550 kgcnn-3.0.0/kgcnn/literature/GemNet/
+-rw-rw-rw-   0        0        0        0 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/GemNet/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 07:25:08.647550 kgcnn-3.0.0/kgcnn/literature/GraphSAGE/
+-rw-rw-rw-   0        0        0       99 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/GraphSAGE/__init__.py
+-rw-rw-rw-   0        0        0     6836 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/GraphSAGE/_make.py
+drwxrwxrwx   0        0        0        0 2023-04-28 07:25:08.688549 kgcnn-3.0.0/kgcnn/literature/HDNNP2nd/
+-rw-rw-rw-   0        0        0      454 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/HDNNP2nd/__init__.py
+-rw-rw-rw-   0        0        0    25733 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/HDNNP2nd/_acsf_conv.py
+-rw-rw-rw-   0        0        0    15739 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/HDNNP2nd/_make.py
+-rw-rw-rw-   0        0        0    21072 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/HDNNP2nd/_wacsf_conv.py
+drwxrwxrwx   0        0        0        0 2023-04-28 07:25:08.748549 kgcnn-3.0.0/kgcnn/literature/HDNNP4th/
+-rw-rw-rw-   0        0        0      127 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/HDNNP4th/__init__.py
+-rw-rw-rw-   0        0        0    25834 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/HDNNP4th/_hdnnp_conv.py
+-rw-rw-rw-   0        0        0     8160 2023-04-28 07:07:20.000000 kgcnn-3.0.0/kgcnn/literature/HDNNP4th/_make.py
+-rw-rw-rw-   0        0        0     9442 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/HDNNP4th/_test_hdnnp.py
+drwxrwxrwx   0        0        0        0 2023-04-28 07:25:08.777550 kgcnn-3.0.0/kgcnn/literature/HamNet/
+-rw-rw-rw-   0        0        0       99 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/HamNet/__init__.py
+-rw-rw-rw-   0        0        0    28565 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/HamNet/_hamnet_conv.py
+-rw-rw-rw-   0        0        0     8210 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/HamNet/_make.py
+drwxrwxrwx   0        0        0        0 2023-04-28 07:25:08.782552 kgcnn-3.0.0/kgcnn/literature/INorp/
+-rw-rw-rw-   0        0        0       99 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/INorp/__init__.py
+-rw-rw-rw-   0        0        0     7954 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/INorp/_make.py
+drwxrwxrwx   0        0        0        0 2023-04-28 07:25:08.809548 kgcnn-3.0.0/kgcnn/literature/MAT/
+-rw-rw-rw-   0        0        0       99 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/MAT/__init__.py
+-rw-rw-rw-   0        0        0     9724 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/MAT/_make.py
+-rw-rw-rw-   0        0        0     8758 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/MAT/_mat_conv.py
+drwxrwxrwx   0        0        0        0 2023-04-28 07:25:08.836547 kgcnn-3.0.0/kgcnn/literature/MEGAN/
+-rw-rw-rw-   0        0        0      218 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/MEGAN/__init__.py
+-rw-rw-rw-   0        0        0     1068 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/MEGAN/_make.py
+-rw-rw-rw-   0        0        0    22759 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/MEGAN/_model.py
+-rw-rw-rw-   0        0        0     6903 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/MEGAN/_test_literature_megan.py
+drwxrwxrwx   0        0        0        0 2023-04-28 07:25:08.863565 kgcnn-3.0.0/kgcnn/literature/MXMNet/
+-rw-rw-rw-   0        0        0       99 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/MXMNet/__init__.py
+-rw-rw-rw-   0        0        0    10142 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/MXMNet/_make.py
+-rw-rw-rw-   0        0        0     8490 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/MXMNet/_mxmnet_conv.py
+drwxrwxrwx   0        0        0        0 2023-04-28 07:25:08.882571 kgcnn-3.0.0/kgcnn/literature/Megnet/
+-rw-rw-rw-   0        0        0      215 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/Megnet/__init__.py
+-rw-rw-rw-   0        0        0    18509 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/Megnet/_make.py
+-rw-rw-rw-   0        0        0     7153 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/Megnet/_megnet_conv.py
+drwxrwxrwx   0        0        0        0 2023-04-28 07:25:08.901567 kgcnn-3.0.0/kgcnn/literature/MoGAT/
+-rw-rw-rw-   0        0        0       99 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/MoGAT/__init__.py
+-rw-rw-rw-   0        0        0     6679 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/MoGAT/_make.py
+-rw-rw-rw-   0        0        0    12206 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/MoGAT/_mogat_conv.py
+drwxrwxrwx   0        0        0        0 2023-04-28 07:25:08.921568 kgcnn-3.0.0/kgcnn/literature/NMPN/
+-rw-rw-rw-   0        0        0      215 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/NMPN/__init__.py
+-rw-rw-rw-   0        0        0    17202 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/NMPN/_make.py
+-rw-rw-rw-   0        0        0     4753 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/NMPN/_mpnn_conv.py
+drwxrwxrwx   0        0        0        0 2023-04-28 07:25:08.947566 kgcnn-3.0.0/kgcnn/literature/PAiNN/
+-rw-rw-rw-   0        0        0      215 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/PAiNN/__init__.py
+-rw-rw-rw-   0        0        0    14386 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/PAiNN/_make.py
+-rw-rw-rw-   0        0        0    15451 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/PAiNN/_painn_conv.py
+drwxrwxrwx   0        0        0        0 2023-04-28 07:25:08.952567 kgcnn-3.0.0/kgcnn/literature/RGCN/
+-rw-rw-rw-   0        0        0       99 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/RGCN/__init__.py
+-rw-rw-rw-   0        0        0     5668 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/RGCN/_make.py
+drwxrwxrwx   0        0        0        0 2023-04-28 07:25:08.978566 kgcnn-3.0.0/kgcnn/literature/Schnet/
+-rw-rw-rw-   0        0        0      215 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/Schnet/__init__.py
+-rw-rw-rw-   0        0        0    14260 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/Schnet/_make.py
+-rw-rw-rw-   0        0        0     8445 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/Schnet/_schnet_conv.py
+drwxrwxrwx   0        0        0        0 2023-04-28 07:25:09.019565 kgcnn-3.0.0/kgcnn/literature/Unet/
+-rw-rw-rw-   0        0        0       99 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/Unet/__init__.py
+-rw-rw-rw-   0        0        0     7194 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/Unet/_make.py
+-rw-rw-rw-   0        0        0     1138 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/Unet/_test_connect.py
+-rw-rw-rw-   0        0        0     4157 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/Unet/_test_topk.py
+-rw-rw-rw-   0        0        0    19977 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/Unet/_topk.py
+-rw-rw-rw-   0        0        0       51 2023-04-28 07:07:19.000000 kgcnn-3.0.0/kgcnn/literature/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 07:25:09.074566 kgcnn-3.0.0/kgcnn/literature/coGN/
+-rw-rw-rw-   0        0        0     2872 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/coGN/__init__.py
+-rw-rw-rw-   0        0        0     7416 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/coGN/_coGN_config.py
+-rw-rw-rw-   0        0        0     6429 2023-04-28 07:07:21.000000 kgcnn-3.0.0/kgcnn/literature/coGN/_coNGN_config.py
+drwxrwxrwx   0        0        0        0 2023-04-28 07:25:09.099565 kgcnn-3.0.0/kgcnn/literature/coGN/_embedding_layers/
+-rw-rw-rw-   0        0        0        0 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/literature/coGN/_embedding_layers/__init__.py
+-rw-rw-rw-   0        0        0     4218 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/literature/coGN/_embedding_layers/_atom_embedding.py
+-rw-rw-rw-   0        0        0     6719 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/literature/coGN/_embedding_layers/_edge_embedding.py
+-rw-rw-rw-   0        0        0      891 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/literature/coGN/_gates.py
+drwxrwxrwx   0        0        0        0 2023-04-28 07:25:09.125875 kgcnn-3.0.0/kgcnn/literature/coGN/_graph_network/
+-rw-rw-rw-   0        0        0        0 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/literature/coGN/_graph_network/__init__.py
+-rw-rw-rw-   0        0        0    16183 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/literature/coGN/_graph_network/graph_network_base.py
+-rw-rw-rw-   0        0        0    23817 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/literature/coGN/_graph_network/graph_networks.py
+-rw-rw-rw-   0        0        0    27686 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/literature/coGN/_make.py
+-rw-rw-rw-   0        0        0     2266 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/literature/coGN/_multiplicity_readout.py
+-rw-rw-rw-   0        0        0     3945 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/literature/coGN/_preprocessing_layers.py
+-rw-rw-rw-   0        0        0      372 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/literature/coGN/_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-28 07:25:09.149593 kgcnn-3.0.0/kgcnn/literature/rGIN/
+-rw-rw-rw-   0        0        0       99 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/literature/rGIN/__init__.py
+-rw-rw-rw-   0        0        0     5438 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/literature/rGIN/_make.py
+-rw-rw-rw-   0        0        0     3500 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/literature/rGIN/_rgin_conv.py
+drwxrwxrwx   0        0        0        0 2023-04-28 07:25:09.164678 kgcnn-3.0.0/kgcnn/metrics/
+-rw-rw-rw-   0        0        0        0 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/metrics/__init__.py
+-rw-rw-rw-   0        0        0      972 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/metrics/loss.py
+-rw-rw-rw-   0        0        0    10804 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/metrics/metrics.py
+drwxrwxrwx   0        0        0        0 2023-04-28 07:25:09.191679 kgcnn-3.0.0/kgcnn/model/
+-rw-rw-rw-   0        0        0        0 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/model/README.md
+-rw-rw-rw-   0        0        0        0 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/model/__init__.py
+-rw-rw-rw-   0        0        0     8946 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/model/force.py
+-rw-rw-rw-   0        0        0       18 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/model/serial.py
+-rw-rw-rw-   0        0        0     5430 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/model/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-28 07:25:09.255679 kgcnn-3.0.0/kgcnn/mol/
+-rw-rw-rw-   0        0        0      165 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/mol/__init__.py
+-rw-rw-rw-   0        0        0       33 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/mol/base.py
+-rw-rw-rw-   0        0        0       36 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/mol/convert.py
+-rw-rw-rw-   0        0        0       36 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/mol/encoder.py
+drwxrwxrwx   0        0        0        0 2023-04-28 07:25:09.260679 kgcnn-3.0.0/kgcnn/mol/external/
+-rw-rw-rw-   0        0        0        1 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/mol/external/__init__.py
+-rw-rw-rw-   0        0        0       46 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/mol/external/ballloon.py
+-rw-rw-rw-   0        0        0       40 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/mol/graph_babel.py
+-rw-rw-rw-   0        0        0       40 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/mol/graph_rdkit.py
+-rw-rw-rw-   0        0        0       31 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/mol/io.py
+-rw-rw-rw-   0        0        0       36 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/mol/methods.py
+-rw-rw-rw-   0        0        0       35 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/mol/serial.py
+drwxrwxrwx   0        0        0        0 2023-04-28 07:25:09.282677 kgcnn-3.0.0/kgcnn/moldyn/
+-rw-rw-rw-   0        0        0      177 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/moldyn/__init__.py
+-rw-rw-rw-   0        0        0       46 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/moldyn/ase_calc.py
+-rw-rw-rw-   0        0        0       42 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/moldyn/base.py
+drwxrwxrwx   0        0        0        0 2023-04-28 07:25:09.358677 kgcnn-3.0.0/kgcnn/molecule/
+-rw-rw-rw-   0        0        0        0 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/molecule/__init__.py
+-rw-rw-rw-   0        0        0    10057 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/molecule/base.py
+-rw-rw-rw-   0        0        0    12161 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/molecule/convert.py
+drwxrwxrwx   0        0        0        0 2023-04-28 07:25:09.373677 kgcnn-3.0.0/kgcnn/molecule/dynamics/
+-rw-rw-rw-   0        0        0        0 2023-04-28 07:07:23.000000 kgcnn-3.0.0/kgcnn/molecule/dynamics/__init__.py
+-rw-rw-rw-   0        0        0     3911 2023-04-28 07:07:23.000000 kgcnn-3.0.0/kgcnn/molecule/dynamics/ase_calc.py
+-rw-rw-rw-   0        0        0     8386 2023-04-28 07:07:23.000000 kgcnn-3.0.0/kgcnn/molecule/dynamics/base.py
+-rw-rw-rw-   0        0        0     2556 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/molecule/encoder.py
+drwxrwxrwx   0        0        0        0 2023-04-28 07:25:09.399676 kgcnn-3.0.0/kgcnn/molecule/external/
+-rw-rw-rw-   0        0        0      159 2023-04-28 07:07:23.000000 kgcnn-3.0.0/kgcnn/molecule/external/__init__.py
+-rw-rw-rw-   0        0        0    20790 2023-04-28 07:07:23.000000 kgcnn-3.0.0/kgcnn/molecule/external/ballloon.py
+-rw-rw-rw-   0        0        0    17892 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/molecule/graph_babel.py
+-rw-rw-rw-   0        0        0    20750 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/molecule/graph_rdkit.py
+-rw-rw-rw-   0        0        0     8960 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/molecule/io.py
+-rw-rw-rw-   0        0        0     5105 2023-04-28 07:07:22.000000 kgcnn-3.0.0/kgcnn/molecule/methods.py
+-rw-rw-rw-   0        0        0      702 2023-04-28 07:07:23.000000 kgcnn-3.0.0/kgcnn/molecule/serial.py
+drwxrwxrwx   0        0        0        0 2023-04-28 07:25:09.452678 kgcnn-3.0.0/kgcnn/ops/
+-rw-rw-rw-   0        0        0        0 2023-04-28 07:07:23.000000 kgcnn-3.0.0/kgcnn/ops/__init__.py
+-rw-rw-rw-   0        0        0     3853 2023-04-28 07:07:23.000000 kgcnn-3.0.0/kgcnn/ops/activ.py
+-rw-rw-rw-   0        0        0     1483 2023-04-28 07:07:23.000000 kgcnn-3.0.0/kgcnn/ops/axis.py
+-rw-rw-rw-   0        0        0        0 2023-04-28 07:07:23.000000 kgcnn-3.0.0/kgcnn/ops/casting.py
+-rw-rw-rw-   0        0        0     6991 2023-04-28 07:07:23.000000 kgcnn-3.0.0/kgcnn/ops/initializer.py
+-rw-rw-rw-   0        0        0        0 2023-04-28 07:07:23.000000 kgcnn-3.0.0/kgcnn/ops/numpy.py
+-rw-rw-rw-   0        0        0     8292 2023-04-28 07:07:23.000000 kgcnn-3.0.0/kgcnn/ops/partition.py
+-rw-rw-rw-   0        0        0    10223 2023-04-28 07:07:23.000000 kgcnn-3.0.0/kgcnn/ops/polynom.py
+-rw-rw-rw-   0        0        0     3181 2023-04-28 07:07:23.000000 kgcnn-3.0.0/kgcnn/ops/ragged.py
+-rw-rw-rw-   0        0        0     1148 2023-04-28 07:07:23.000000 kgcnn-3.0.0/kgcnn/ops/scatter.py
+-rw-rw-rw-   0        0        0     2046 2023-04-28 07:07:23.000000 kgcnn-3.0.0/kgcnn/ops/segment.py
+-rw-rw-rw-   0        0        0        0 2023-04-28 07:07:23.000000 kgcnn-3.0.0/kgcnn/ops/sorting.py
+drwxrwxrwx   0        0        0        0 2023-04-28 07:25:09.497678 kgcnn-3.0.0/kgcnn/training/
+-rw-rw-rw-   0        0        0        0 2023-04-28 07:07:23.000000 kgcnn-3.0.0/kgcnn/training/__init__.py
+-rw-rw-rw-   0        0        0     1220 2023-04-28 07:07:23.000000 kgcnn-3.0.0/kgcnn/training/callbacks.py
+-rw-rw-rw-   0        0        0     4643 2023-04-28 07:07:23.000000 kgcnn-3.0.0/kgcnn/training/history.py
+-rw-rw-rw-   0        0        0    14935 2023-04-28 07:07:23.000000 kgcnn-3.0.0/kgcnn/training/hyper.py
+-rw-rw-rw-   0        0        0     8691 2023-04-28 07:07:23.000000 kgcnn-3.0.0/kgcnn/training/optimizer.py
+-rw-rw-rw-   0        0        0     2656 2023-04-28 07:07:23.000000 kgcnn-3.0.0/kgcnn/training/schedule.py
+-rw-rw-rw-   0        0        0    16405 2023-04-28 07:07:23.000000 kgcnn-3.0.0/kgcnn/training/scheduler.py
+drwxrwxrwx   0        0        0        0 2023-04-28 07:25:09.506678 kgcnn-3.0.0/kgcnn/utils/
+-rw-rw-rw-   0        0        0        1 2023-04-28 07:07:23.000000 kgcnn-3.0.0/kgcnn/utils/__init__.py
+-rw-rw-rw-   0        0        0     2248 2023-04-28 07:07:23.000000 kgcnn-3.0.0/kgcnn/utils/devices.py
+-rw-rw-rw-   0        0        0     7356 2023-04-28 07:07:23.000000 kgcnn-3.0.0/kgcnn/utils/plots.py
+-rw-rw-rw-   0        0        0     2307 2023-04-28 07:07:23.000000 kgcnn-3.0.0/kgcnn/utils/serial.py
+drwxrwxrwx   0        0        0        0 2023-04-28 07:25:07.526324 kgcnn-3.0.0/kgcnn.egg-info/
+-rw-rw-rw-   0        0        0    19415 2023-04-28 07:25:07.000000 kgcnn-3.0.0/kgcnn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     8562 2023-04-28 07:25:07.000000 kgcnn-3.0.0/kgcnn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 07:25:07.000000 kgcnn-3.0.0/kgcnn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      313 2023-04-28 07:25:07.000000 kgcnn-3.0.0/kgcnn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-28 07:25:07.000000 kgcnn-3.0.0/kgcnn.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-28 07:25:09.579678 kgcnn-3.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1855 2023-04-28 07:07:15.000000 kgcnn-3.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 07:25:09.576678 kgcnn-3.0.0/test/
+-rw-rw-rw-   0        0        0        0 2023-04-28 07:07:24.000000 kgcnn-3.0.0/test/__init__.py
+-rw-rw-rw-   0        0        0     4986 2023-04-28 07:07:24.000000 kgcnn-3.0.0/test/test_data_base.py
+-rw-rw-rw-   0        0        0     7931 2023-04-28 07:07:24.000000 kgcnn-3.0.0/test/test_data_moleculenet.py
+-rw-rw-rw-   0        0        0     1255 2023-04-28 07:07:24.000000 kgcnn-3.0.0/test/test_graph_base.py
+-rw-rw-rw-   0        0        0     4149 2023-04-28 07:07:24.000000 kgcnn-3.0.0/test/test_graph_methods.py
+-rw-rw-rw-   0        0        0     5135 2023-04-28 07:07:24.000000 kgcnn-3.0.0/test/test_layers_attention.py
+-rw-rw-rw-   0        0        0     4211 2023-04-28 07:07:24.000000 kgcnn-3.0.0/test/test_layers_gather.py
+-rw-rw-rw-   0        0        0     7647 2023-04-28 07:07:24.000000 kgcnn-3.0.0/test/test_layers_geom.py
+-rw-rw-rw-   0        0        0     2338 2023-04-28 07:07:24.000000 kgcnn-3.0.0/test/test_layers_pooling.py
+-rw-rw-rw-   0        0        0     8078 2023-04-28 07:07:24.000000 kgcnn-3.0.0/test/test_range_periodic.py
+-rw-rw-rw-   0        0        0      118 2023-04-28 07:07:24.000000 kgcnn-3.0.0/test/utils.py
```

### Comparing `kgcnn-2.2.4/LICENSE` & `kgcnn-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kgcnn-2.2.4/PKG-INFO` & `kgcnn-3.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kgcnn
-Version: 2.2.4
+Version: 3.0.0
 Summary: General Base Layers for Graph Convolutions with tensorflow.keras
 Home-page: https://github.com/aimat-lab/gcnn_keras
 Author: Patrick Reiser
 Author-email: patrick.reiser@kit.edu
 License: UNKNOWN
 Keywords: materials,science,machine,learning,deep,graph,networks,neural
 Platform: UNKNOWN
@@ -43,15 +43,15 @@
 
 <a name="general"></a>
 # General
 
 The package in [kgcnn](kgcnn) contains several layer classes to build up graph convolution models. 
 Some models are given as an example.
 A [documentation](https://kgcnn.readthedocs.io/en/latest/index.html) is generated in [docs](docs).
-Focus of [kgcnn](kgcnn) is (batched) graph learning for molecules [kgcnn.mol](kgcnn/mol) and materials [kgcnn.crystal](kgcnn/crystal).
+Focus of [kgcnn](kgcnn) is (batched) graph learning for molecules [kgcnn.molecule](kgcnn/molecule) and materials [kgcnn.crystal](kgcnn/crystal).
 If you want to get in contact, feel free to [discuss](https://github.com/aimat-lab/gcnn_keras/discussions). 
 
 <a name="requirements"></a>
 # Requirements
 
 
 Standard python package requirements are placed in the `setup.py` and are installed automatically ([kgcnn](https://github.com/aimat-lab/gcnn_keras) >=2.2). 
@@ -157,44 +157,50 @@
     def update_nodes(self, inputs, **kwargs):
         nodes, nodes_update = inputs
         return self.add([nodes, nodes_update])
 ```
 
 <a name="literature"></a>
 # Literature
-A version of the following models and variants thereof are implemented in [literature](kgcnn/literature):
-* **[GCN](kgcnn/literature/GCN.py)**: [Semi-Supervised Classification with Graph Convolutional Networks](https://arxiv.org/abs/1609.02907) by Kipf et al. (2016)
-* **[Schnet](kgcnn/literature/Schnet.py)**: [SchNet – A deep learning architecture for molecules and materials ](https://aip.scitation.org/doi/10.1063/1.5019779) by Schütt et al. (2017)
-* **[GAT](kgcnn/literature/GAT.py)**: [Graph Attention Networks](https://arxiv.org/abs/1710.10903) by Veličković et al. (2018)
-* **[GraphSAGE](kgcnn/literature/GraphSAGE.py)**: [Inductive Representation Learning on Large Graphs](http://arxiv.org/abs/1706.02216) by Hamilton et al. (2017)
-* **[DimeNetPP](kgcnn/literature/DimeNetPP.py)**: [Fast and Uncertainty-Aware Directional Message Passing for Non-Equilibrium Molecules](https://arxiv.org/abs/2011.14115) by Klicpera et al. (2020)
-* **[GNNExplainer](kgcnn/literature/GNNExplain.py)**: [GNNExplainer: Generating Explanations for Graph Neural Networks](https://arxiv.org/abs/1903.03894) by Ying et al. (2019)
-* **[AttentiveFP](kgcnn/literature/AttentiveFP.py)**: [Pushing the Boundaries of Molecular Representation for Drug Discovery with the Graph Attention Mechanism](https://pubs.acs.org/doi/10.1021/acs.jmedchem.9b00959) by Xiong et al. (2019)
+The following models, proposed in literature, have a module in [literature](kgcnn/literature). The module usually exposes a `make_model` function
+to create a ``tf.keras.models.Model``, which features ragged tensor in- or output. The models can but must not be build completely from `kgcnn.layers` and can for example include
+original implementations (with proper licencing).
+
+* **[GCN](kgcnn/literature/GCN)**: [Semi-Supervised Classification with Graph Convolutional Networks](https://arxiv.org/abs/1609.02907) by Kipf et al. (2016)
+* **[Schnet](kgcnn/literature/Schnet)**: [SchNet – A deep learning architecture for molecules and materials ](https://aip.scitation.org/doi/10.1063/1.5019779) by Schütt et al. (2017)
+* **[GAT](kgcnn/literature/GAT)**: [Graph Attention Networks](https://arxiv.org/abs/1710.10903) by Veličković et al. (2018)
+* **[GraphSAGE](kgcnn/literature/GraphSAGE)**: [Inductive Representation Learning on Large Graphs](http://arxiv.org/abs/1706.02216) by Hamilton et al. (2017)
+* **[DimeNetPP](kgcnn/literature/DimeNetPP)**: [Fast and Uncertainty-Aware Directional Message Passing for Non-Equilibrium Molecules](https://arxiv.org/abs/2011.14115) by Klicpera et al. (2020)
+* **[GNNExplainer](kgcnn/literature/GNNExplain)**: [GNNExplainer: Generating Explanations for Graph Neural Networks](https://arxiv.org/abs/1903.03894) by Ying et al. (2019)
+* **[AttentiveFP](kgcnn/literature/AttentiveFP)**: [Pushing the Boundaries of Molecular Representation for Drug Discovery with the Graph Attention Mechanism](https://pubs.acs.org/doi/10.1021/acs.jmedchem.9b00959) by Xiong et al. (2019)
 
 <details>
 <summary> ... and many more <b>(click to expand)</b>.</summary>
 
-* **[INorp](kgcnn/literature/INorp.py)**: [Interaction Networks for Learning about Objects,Relations and Physics](https://arxiv.org/abs/1612.00222) by Battaglia et al. (2016)
-* **[Megnet](kgcnn/literature/Megnet.py)**: [Graph Networks as a Universal Machine Learning Framework for Molecules and Crystals](https://doi.org/10.1021/acs.chemmater.9b01294) by Chen et al. (2019)
-* **[NMPN](kgcnn/literature/NMPN.py)**: [Neural Message Passing for Quantum Chemistry](http://arxiv.org/abs/1704.01212) by Gilmer et al. (2017)
-* **[Unet](kgcnn/literature/Unet.py)**: [Graph U-Nets](http://proceedings.mlr.press/v97/gao19a/gao19a.pdf) by H. Gao and S. Ji (2019)
-* **[GATv2](kgcnn/literature/GATv2.py)**: [How Attentive are Graph Attention Networks?](https://arxiv.org/abs/2105.14491) by Brody et al. (2021)
-* **[GIN](kgcnn/literature/GIN.py)**: [How Powerful are Graph Neural Networks?](https://arxiv.org/abs/1810.00826) by Xu et al. (2019)
-* **[PAiNN](kgcnn/literature/PAiNN.py)**: [Equivariant message passing for the prediction of tensorial properties and molecular spectra](https://arxiv.org/pdf/2102.03150.pdf) by Schütt et al. (2020)
-* **[DMPNN](kgcnn/literature/DMPNN.py)**: [Analyzing Learned Molecular Representations for Property Prediction](https://pubs.acs.org/doi/abs/10.1021/acs.jcim.9b00237) by Yang et al. (2019)
-* **[HamNet](kgcnn/literature/HamNet.py)**: [HamNet: Conformation-Guided Molecular Representation with Hamiltonian Neural Networks](https://arxiv.org/abs/2105.03688) by Li et al. (2021)
-* **[CGCNN](kgcnn/literature/CGCNN.py)**: [Crystal Graph Convolutional Neural Networks for an Accurate and Interpretable Prediction of Material Properties](https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.120.145301) by Xie et al. (2018)
-* **[CMPNN](kgcnn/literature/CMPNN.py)**: [Communicative Representation Learning on Attributed Molecular Graphs](https://www.ijcai.org/proceedings/2020/0392.pdf) by Song et al. (2020)
-* **[EGNN](kgcnn/literature/EGNN.py)**: [E(n) Equivariant Graph Neural Networks](https://arxiv.org/abs/2102.09844) by Satorras et al. (2021)
-* **[MAT](kgcnn/literature/MAT.py)**: [Molecule Attention Transformer](https://arxiv.org/abs/2002.08264) by Maziarka et al. (2020)
-* **[MXMNet](kgcnn/literature/MXMNet.py)**: [Molecular Mechanics-Driven Graph Neural Network with Multiplex Graph for Molecular Structures](https://arxiv.org/abs/2011.07457) by Zhang et al. (2020)
-* **[RGCN](kgcnn/literature/RGCN.py)**: [Modeling Relational Data with Graph Convolutional Networks](https://arxiv.org/abs/1703.06103) by Schlichtkrull et al. (2017)
-* **[GNNFilm](kgcnn/literature/GNNFilm.py)**: [GNN-FiLM: Graph Neural Networks with Feature-wise Linear Modulation](https://arxiv.org/abs/1906.12192) by Marc Brockschmidt (2020)
-* **[HDNNP2nd](kgcnn/literature/HDNNP2nd.py)**: [Atom-centered symmetry functions for constructing high-dimensional neural network potentials](https://aip.scitation.org/doi/abs/10.1063/1.3553717) by Jörg Behler (2011)
-* **[HDNNP4th](kgcnn/literature/HDNNP4th.py)**: [A fourth-generation high-dimensional neural network potential with accurate electrostatics including non-local charge transfer](https://www.nature.com/articles/s41467-020-20427-2) by Ko et al. (2021)
+* **[INorp](kgcnn/literature/INorp)**: [Interaction Networks for Learning about Objects,Relations and Physics](https://arxiv.org/abs/1612.00222) by Battaglia et al. (2016)
+* **[Megnet](kgcnn/literature/Megnet)**: [Graph Networks as a Universal Machine Learning Framework for Molecules and Crystals](https://doi.org/10.1021/acs.chemmater.9b01294) by Chen et al. (2019)
+* **[NMPN](kgcnn/literature/NMPN)**: [Neural Message Passing for Quantum Chemistry](http://arxiv.org/abs/1704.01212) by Gilmer et al. (2017)
+* **[Unet](kgcnn/literature/Unet)**: [Graph U-Nets](http://proceedings.mlr.press/v97/gao19a/gao19a.pdf) by H. Gao and S. Ji (2019)
+* **[GATv2](kgcnn/literature/GATv2)**: [How Attentive are Graph Attention Networks?](https://arxiv.org/abs/2105.14491) by Brody et al. (2021)
+* **[GIN](kgcnn/literature/GIN)**: [How Powerful are Graph Neural Networks?](https://arxiv.org/abs/1810.00826) by Xu et al. (2019)
+* **[PAiNN](kgcnn/literature/PAiNN)**: [Equivariant message passing for the prediction of tensorial properties and molecular spectra](https://arxiv.org/pdf/2102.03150.pdf) by Schütt et al. (2020)
+* **[DMPNN](kgcnn/literature/DMPNN)**: [Analyzing Learned Molecular Representations for Property Prediction](https://pubs.acs.org/doi/abs/10.1021/acs.jcim.9b00237) by Yang et al. (2019)
+* **[HamNet](kgcnn/literature/HamNet)**: [HamNet: Conformation-Guided Molecular Representation with Hamiltonian Neural Networks](https://arxiv.org/abs/2105.03688) by Li et al. (2021)
+* **[CGCNN](kgcnn/literature/CGCNN)**: [Crystal Graph Convolutional Neural Networks for an Accurate and Interpretable Prediction of Material Properties](https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.120.145301) by Xie et al. (2018)
+* **[CMPNN](kgcnn/literature/CMPNN)**: [Communicative Representation Learning on Attributed Molecular Graphs](https://www.ijcai.org/proceedings/2020/0392.pdf) by Song et al. (2020)
+* **[EGNN](kgcnn/literature/EGNN)**: [E(n) Equivariant Graph Neural Networks](https://arxiv.org/abs/2102.09844) by Satorras et al. (2021)
+* **[MAT](kgcnn/literature/MAT)**: [Molecule Attention Transformer](https://arxiv.org/abs/2002.08264) by Maziarka et al. (2020)
+* **[MXMNet](kgcnn/literature/MXMNet)**: [Molecular Mechanics-Driven Graph Neural Network with Multiplex Graph for Molecular Structures](https://arxiv.org/abs/2011.07457) by Zhang et al. (2020)
+* **[RGCN](kgcnn/literature/RGCN)**: [Modeling Relational Data with Graph Convolutional Networks](https://arxiv.org/abs/1703.06103) by Schlichtkrull et al. (2017)
+* **[GNNFilm](kgcnn/literature/GNNFilm)**: [GNN-FiLM: Graph Neural Networks with Feature-wise Linear Modulation](https://arxiv.org/abs/1906.12192) by Marc Brockschmidt (2020)
+* **[HDNNP2nd](kgcnn/literature/HDNNP2nd)**: [Atom-centered symmetry functions for constructing high-dimensional neural network potentials](https://aip.scitation.org/doi/abs/10.1063/1.3553717) by Jörg Behler (2011)
+* **[HDNNP4th](kgcnn/literature/HDNNP4th)**: [A fourth-generation high-dimensional neural network potential with accurate electrostatics including non-local charge transfer](https://www.nature.com/articles/s41467-020-20427-2) by Ko et al. (2021)
+* **[DGIN](kgcnn/literature/DGIN)**: [Improved Lipophilicity and Aqueous Solubility Prediction with Composite Graph Neural Networks ](https://pubmed.ncbi.nlm.nih.gov/34684766/) by Wieder et al. (2021)
+* **[MoGAT](kgcnn/literature/MoGAT)**: [Multi-order graph attention network for water solubility prediction and interpretation](https://www.nature.com/articles/s41598-022-25701-5) by Lee et al. (2023)
+* **[rGIN](kgcnn/literature/rGIN)** [Random Features Strengthen Graph Neural Networks](https://arxiv.org/abs/2002.03155) by Sato et al. (2020)
 </details>
 
 
 <a name="data"></a>
 # Data
 
 How to construct ragged tensors is shown [above](#implementation-details-input).
```

### Comparing `kgcnn-2.2.4/README.md` & `kgcnn-3.0.0/kgcnn.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: kgcnn
+Version: 3.0.0
+Summary: General Base Layers for Graph Convolutions with tensorflow.keras
+Home-page: https://github.com/aimat-lab/gcnn_keras
+Author: Patrick Reiser
+Author-email: patrick.reiser@kit.edu
+License: UNKNOWN
+Keywords: materials,science,machine,learning,deep,graph,networks,neural
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Topic :: Scientific/Engineering :: Physics
+Classifier: Topic :: Scientific/Engineering :: Chemistry
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Description-Content-Type: text/markdown
+Provides-Extra: openbabel
+License-File: LICENSE
+License-File: AUTHORS
+
 ![GitHub release (latest by date)](https://img.shields.io/github/v/release/aimat-lab/gcnn_keras)
 [![Documentation Status](https://readthedocs.org/projects/kgcnn/badge/?version=latest)](https://kgcnn.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/kgcnn.svg)](https://badge.fury.io/py/kgcnn)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/kgcnn)
 [![kgcnn_unit_tests](https://github.com/aimat-lab/gcnn_keras/actions/workflows/unittests.yml/badge.svg)](https://github.com/aimat-lab/gcnn_keras/actions/workflows/unittests.yml)
 [![DOI](https://img.shields.io/badge/DOI-10.1016%2Fj.simpa.2021.100095%20-blue)](https://doi.org/10.1016/j.simpa.2021.100095)
 ![GitHub](https://img.shields.io/github/license/aimat-lab/gcnn_keras)
@@ -21,15 +43,15 @@
 
 <a name="general"></a>
 # General
 
 The package in [kgcnn](kgcnn) contains several layer classes to build up graph convolution models. 
 Some models are given as an example.
 A [documentation](https://kgcnn.readthedocs.io/en/latest/index.html) is generated in [docs](docs).
-Focus of [kgcnn](kgcnn) is (batched) graph learning for molecules [kgcnn.mol](kgcnn/mol) and materials [kgcnn.crystal](kgcnn/crystal).
+Focus of [kgcnn](kgcnn) is (batched) graph learning for molecules [kgcnn.molecule](kgcnn/molecule) and materials [kgcnn.crystal](kgcnn/crystal).
 If you want to get in contact, feel free to [discuss](https://github.com/aimat-lab/gcnn_keras/discussions). 
 
 <a name="requirements"></a>
 # Requirements
 
 
 Standard python package requirements are placed in the `setup.py` and are installed automatically ([kgcnn](https://github.com/aimat-lab/gcnn_keras) >=2.2). 
@@ -135,44 +157,50 @@
     def update_nodes(self, inputs, **kwargs):
         nodes, nodes_update = inputs
         return self.add([nodes, nodes_update])
 ```
 
 <a name="literature"></a>
 # Literature
-A version of the following models and variants thereof are implemented in [literature](kgcnn/literature):
-* **[GCN](kgcnn/literature/GCN.py)**: [Semi-Supervised Classification with Graph Convolutional Networks](https://arxiv.org/abs/1609.02907) by Kipf et al. (2016)
-* **[Schnet](kgcnn/literature/Schnet.py)**: [SchNet – A deep learning architecture for molecules and materials ](https://aip.scitation.org/doi/10.1063/1.5019779) by Schütt et al. (2017)
-* **[GAT](kgcnn/literature/GAT.py)**: [Graph Attention Networks](https://arxiv.org/abs/1710.10903) by Veličković et al. (2018)
-* **[GraphSAGE](kgcnn/literature/GraphSAGE.py)**: [Inductive Representation Learning on Large Graphs](http://arxiv.org/abs/1706.02216) by Hamilton et al. (2017)
-* **[DimeNetPP](kgcnn/literature/DimeNetPP.py)**: [Fast and Uncertainty-Aware Directional Message Passing for Non-Equilibrium Molecules](https://arxiv.org/abs/2011.14115) by Klicpera et al. (2020)
-* **[GNNExplainer](kgcnn/literature/GNNExplain.py)**: [GNNExplainer: Generating Explanations for Graph Neural Networks](https://arxiv.org/abs/1903.03894) by Ying et al. (2019)
-* **[AttentiveFP](kgcnn/literature/AttentiveFP.py)**: [Pushing the Boundaries of Molecular Representation for Drug Discovery with the Graph Attention Mechanism](https://pubs.acs.org/doi/10.1021/acs.jmedchem.9b00959) by Xiong et al. (2019)
+The following models, proposed in literature, have a module in [literature](kgcnn/literature). The module usually exposes a `make_model` function
+to create a ``tf.keras.models.Model``, which features ragged tensor in- or output. The models can but must not be build completely from `kgcnn.layers` and can for example include
+original implementations (with proper licencing).
+
+* **[GCN](kgcnn/literature/GCN)**: [Semi-Supervised Classification with Graph Convolutional Networks](https://arxiv.org/abs/1609.02907) by Kipf et al. (2016)
+* **[Schnet](kgcnn/literature/Schnet)**: [SchNet – A deep learning architecture for molecules and materials ](https://aip.scitation.org/doi/10.1063/1.5019779) by Schütt et al. (2017)
+* **[GAT](kgcnn/literature/GAT)**: [Graph Attention Networks](https://arxiv.org/abs/1710.10903) by Veličković et al. (2018)
+* **[GraphSAGE](kgcnn/literature/GraphSAGE)**: [Inductive Representation Learning on Large Graphs](http://arxiv.org/abs/1706.02216) by Hamilton et al. (2017)
+* **[DimeNetPP](kgcnn/literature/DimeNetPP)**: [Fast and Uncertainty-Aware Directional Message Passing for Non-Equilibrium Molecules](https://arxiv.org/abs/2011.14115) by Klicpera et al. (2020)
+* **[GNNExplainer](kgcnn/literature/GNNExplain)**: [GNNExplainer: Generating Explanations for Graph Neural Networks](https://arxiv.org/abs/1903.03894) by Ying et al. (2019)
+* **[AttentiveFP](kgcnn/literature/AttentiveFP)**: [Pushing the Boundaries of Molecular Representation for Drug Discovery with the Graph Attention Mechanism](https://pubs.acs.org/doi/10.1021/acs.jmedchem.9b00959) by Xiong et al. (2019)
 
 <details>
 <summary> ... and many more <b>(click to expand)</b>.</summary>
 
-* **[INorp](kgcnn/literature/INorp.py)**: [Interaction Networks for Learning about Objects,Relations and Physics](https://arxiv.org/abs/1612.00222) by Battaglia et al. (2016)
-* **[Megnet](kgcnn/literature/Megnet.py)**: [Graph Networks as a Universal Machine Learning Framework for Molecules and Crystals](https://doi.org/10.1021/acs.chemmater.9b01294) by Chen et al. (2019)
-* **[NMPN](kgcnn/literature/NMPN.py)**: [Neural Message Passing for Quantum Chemistry](http://arxiv.org/abs/1704.01212) by Gilmer et al. (2017)
-* **[Unet](kgcnn/literature/Unet.py)**: [Graph U-Nets](http://proceedings.mlr.press/v97/gao19a/gao19a.pdf) by H. Gao and S. Ji (2019)
-* **[GATv2](kgcnn/literature/GATv2.py)**: [How Attentive are Graph Attention Networks?](https://arxiv.org/abs/2105.14491) by Brody et al. (2021)
-* **[GIN](kgcnn/literature/GIN.py)**: [How Powerful are Graph Neural Networks?](https://arxiv.org/abs/1810.00826) by Xu et al. (2019)
-* **[PAiNN](kgcnn/literature/PAiNN.py)**: [Equivariant message passing for the prediction of tensorial properties and molecular spectra](https://arxiv.org/pdf/2102.03150.pdf) by Schütt et al. (2020)
-* **[DMPNN](kgcnn/literature/DMPNN.py)**: [Analyzing Learned Molecular Representations for Property Prediction](https://pubs.acs.org/doi/abs/10.1021/acs.jcim.9b00237) by Yang et al. (2019)
-* **[HamNet](kgcnn/literature/HamNet.py)**: [HamNet: Conformation-Guided Molecular Representation with Hamiltonian Neural Networks](https://arxiv.org/abs/2105.03688) by Li et al. (2021)
-* **[CGCNN](kgcnn/literature/CGCNN.py)**: [Crystal Graph Convolutional Neural Networks for an Accurate and Interpretable Prediction of Material Properties](https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.120.145301) by Xie et al. (2018)
-* **[CMPNN](kgcnn/literature/CMPNN.py)**: [Communicative Representation Learning on Attributed Molecular Graphs](https://www.ijcai.org/proceedings/2020/0392.pdf) by Song et al. (2020)
-* **[EGNN](kgcnn/literature/EGNN.py)**: [E(n) Equivariant Graph Neural Networks](https://arxiv.org/abs/2102.09844) by Satorras et al. (2021)
-* **[MAT](kgcnn/literature/MAT.py)**: [Molecule Attention Transformer](https://arxiv.org/abs/2002.08264) by Maziarka et al. (2020)
-* **[MXMNet](kgcnn/literature/MXMNet.py)**: [Molecular Mechanics-Driven Graph Neural Network with Multiplex Graph for Molecular Structures](https://arxiv.org/abs/2011.07457) by Zhang et al. (2020)
-* **[RGCN](kgcnn/literature/RGCN.py)**: [Modeling Relational Data with Graph Convolutional Networks](https://arxiv.org/abs/1703.06103) by Schlichtkrull et al. (2017)
-* **[GNNFilm](kgcnn/literature/GNNFilm.py)**: [GNN-FiLM: Graph Neural Networks with Feature-wise Linear Modulation](https://arxiv.org/abs/1906.12192) by Marc Brockschmidt (2020)
-* **[HDNNP2nd](kgcnn/literature/HDNNP2nd.py)**: [Atom-centered symmetry functions for constructing high-dimensional neural network potentials](https://aip.scitation.org/doi/abs/10.1063/1.3553717) by Jörg Behler (2011)
-* **[HDNNP4th](kgcnn/literature/HDNNP4th.py)**: [A fourth-generation high-dimensional neural network potential with accurate electrostatics including non-local charge transfer](https://www.nature.com/articles/s41467-020-20427-2) by Ko et al. (2021)
+* **[INorp](kgcnn/literature/INorp)**: [Interaction Networks for Learning about Objects,Relations and Physics](https://arxiv.org/abs/1612.00222) by Battaglia et al. (2016)
+* **[Megnet](kgcnn/literature/Megnet)**: [Graph Networks as a Universal Machine Learning Framework for Molecules and Crystals](https://doi.org/10.1021/acs.chemmater.9b01294) by Chen et al. (2019)
+* **[NMPN](kgcnn/literature/NMPN)**: [Neural Message Passing for Quantum Chemistry](http://arxiv.org/abs/1704.01212) by Gilmer et al. (2017)
+* **[Unet](kgcnn/literature/Unet)**: [Graph U-Nets](http://proceedings.mlr.press/v97/gao19a/gao19a.pdf) by H. Gao and S. Ji (2019)
+* **[GATv2](kgcnn/literature/GATv2)**: [How Attentive are Graph Attention Networks?](https://arxiv.org/abs/2105.14491) by Brody et al. (2021)
+* **[GIN](kgcnn/literature/GIN)**: [How Powerful are Graph Neural Networks?](https://arxiv.org/abs/1810.00826) by Xu et al. (2019)
+* **[PAiNN](kgcnn/literature/PAiNN)**: [Equivariant message passing for the prediction of tensorial properties and molecular spectra](https://arxiv.org/pdf/2102.03150.pdf) by Schütt et al. (2020)
+* **[DMPNN](kgcnn/literature/DMPNN)**: [Analyzing Learned Molecular Representations for Property Prediction](https://pubs.acs.org/doi/abs/10.1021/acs.jcim.9b00237) by Yang et al. (2019)
+* **[HamNet](kgcnn/literature/HamNet)**: [HamNet: Conformation-Guided Molecular Representation with Hamiltonian Neural Networks](https://arxiv.org/abs/2105.03688) by Li et al. (2021)
+* **[CGCNN](kgcnn/literature/CGCNN)**: [Crystal Graph Convolutional Neural Networks for an Accurate and Interpretable Prediction of Material Properties](https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.120.145301) by Xie et al. (2018)
+* **[CMPNN](kgcnn/literature/CMPNN)**: [Communicative Representation Learning on Attributed Molecular Graphs](https://www.ijcai.org/proceedings/2020/0392.pdf) by Song et al. (2020)
+* **[EGNN](kgcnn/literature/EGNN)**: [E(n) Equivariant Graph Neural Networks](https://arxiv.org/abs/2102.09844) by Satorras et al. (2021)
+* **[MAT](kgcnn/literature/MAT)**: [Molecule Attention Transformer](https://arxiv.org/abs/2002.08264) by Maziarka et al. (2020)
+* **[MXMNet](kgcnn/literature/MXMNet)**: [Molecular Mechanics-Driven Graph Neural Network with Multiplex Graph for Molecular Structures](https://arxiv.org/abs/2011.07457) by Zhang et al. (2020)
+* **[RGCN](kgcnn/literature/RGCN)**: [Modeling Relational Data with Graph Convolutional Networks](https://arxiv.org/abs/1703.06103) by Schlichtkrull et al. (2017)
+* **[GNNFilm](kgcnn/literature/GNNFilm)**: [GNN-FiLM: Graph Neural Networks with Feature-wise Linear Modulation](https://arxiv.org/abs/1906.12192) by Marc Brockschmidt (2020)
+* **[HDNNP2nd](kgcnn/literature/HDNNP2nd)**: [Atom-centered symmetry functions for constructing high-dimensional neural network potentials](https://aip.scitation.org/doi/abs/10.1063/1.3553717) by Jörg Behler (2011)
+* **[HDNNP4th](kgcnn/literature/HDNNP4th)**: [A fourth-generation high-dimensional neural network potential with accurate electrostatics including non-local charge transfer](https://www.nature.com/articles/s41467-020-20427-2) by Ko et al. (2021)
+* **[DGIN](kgcnn/literature/DGIN)**: [Improved Lipophilicity and Aqueous Solubility Prediction with Composite Graph Neural Networks ](https://pubmed.ncbi.nlm.nih.gov/34684766/) by Wieder et al. (2021)
+* **[MoGAT](kgcnn/literature/MoGAT)**: [Multi-order graph attention network for water solubility prediction and interpretation](https://www.nature.com/articles/s41598-022-25701-5) by Lee et al. (2023)
+* **[rGIN](kgcnn/literature/rGIN)** [Random Features Strengthen Graph Neural Networks](https://arxiv.org/abs/2002.03155) by Sato et al. (2020)
 </details>
 
 
 <a name="data"></a>
 # Data
 
 How to construct ragged tensors is shown [above](#implementation-details-input). 
@@ -300,7 +328,9 @@
 }
 ```
 
 <a name="references"></a>
 # References
 
 - https://www.tensorflow.org/api_docs/python/tf/RaggedTensor
+
+
```

### Comparing `kgcnn-2.2.4/kgcnn/data/base.py` & `kgcnn-3.0.0/kgcnn/data/base.py`

 * *Files identical despite different names*

### Comparing `kgcnn-2.2.4/kgcnn/data/crystal.py` & `kgcnn-3.0.0/kgcnn/data/crystal.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from kgcnn.graph.base import GraphDict
 
 
 class CrystalDataset(MemoryGraphDataset):
     r"""Class for making graph dataset from periodic structures such as crystals.
 
     The dataset class requires a :obj:`data_directory` to store a table '.csv' file containing labels and information
-    of the structures stored in multiple (CIF, POSCAR, ...) files in :obj:`file_directory`.
+    of the structures stored in multiple (CIF, POSCAR, ...) files in :obj:`file_directory` .
     The file names must be included in the '.csv' table. The table file must have one line of header with column names!
 
     .. code-block:: console
 
         ├── data_directory
             ├── file_directory
             │   ├── *.cif
@@ -30,15 +30,15 @@
             │   └── ...
             ├── file_name.csv
             ├── file_name.pymatgen.json
             └── dataset_name.kgcnn.pickle
 
     This class uses :obj:`pymatgen.core.structure.Structure` and therefore requires :obj:`pymatgen` to be installed.
     A '.pymatgen.json' serialized file is generated to store a list of structures from single '.cif' files via
-    :obj:`prepare_data()`.
+    :obj:`prepare_data()` .
     Consequently, a 'file_name.pymatgen.json' can be directly stored in :obj:`data_directory`.
     In this, case :obj:`prepare_data()` does not have to be used. Additionally, a table file 'file_name.csv'
     that lists the single file names and possible labels or classification targets is required.
 
     .. code-block:: python
 
         from kgcnn.data.crystal import CrystalDataset
@@ -254,28 +254,33 @@
         self._map_callbacks(structs=self.get_structures_from_json_file(),
                             data=self.read_in_table_file(file_path=self.file_path).data_frame,
                             callbacks=callbacks)
 
         return self
 
     def set_representation(self, pre_processor: CrystalPreprocessor, reset_graphs: bool = False):
-        # TODO: Add documentation
+        r"""Build a graph representation for this dataset using :obj:`kgcnn.crystal` .
+
+        Args:
+            pre_processor (CrystalPreprocessor): Crystal preprocessor to use.
+            reset_graphs (bool): Whether to reset the graph information. Default is False.
+
+        Returns:
+
+        """
         if reset_graphs:
             self.clear()
         # Read pymatgen JSON file from file.
         structs = self.get_structures_from_json_file()
         if reset_graphs:
             self.empty(len(structs))
 
+        pre_processor.output_graph_as_dict = True
+
         for index, s in enumerate(structs):
             g = pre_processor(s)
-            graph_dict = GraphDict()
-            graph_dict.from_networkx(g, node_attributes=pre_processor.node_attributes,
-                                     edge_attributes=pre_processor.edge_attributes)
-            # TODO: Add graph attributes (label, lattice_matrix, etc.)
-            # TODO: Rename node and edge properties to match kgcnn conventions
-            # TODO: Add GraphDict to dataset
+            self[index].update(g)
 
             if index % self._default_loop_update_info == 0:
                 self.info(" ... preprocess structures {0} from {1}".format(index, len(structs)))
 
         return self
```

### Comparing `kgcnn-2.2.4/kgcnn/data/datasets/ClinToxDataset.py` & `kgcnn-3.0.0/kgcnn/data/datasets/ClinToxDataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-2.2.4/kgcnn/data/datasets/CoraDataset.py` & `kgcnn-3.0.0/kgcnn/data/datasets/CoraDataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 
 import numpy as np
 import scipy.sparse as sp
 
 from kgcnn.data.base import MemoryGraphDataset
 from kgcnn.data.download import DownloadDataset
-from kgcnn.graph.adj import convert_scaled_adjacency_to_list
+from kgcnn.graph.methods import convert_scaled_adjacency_to_list
 
 
 class CoraDataset(DownloadDataset, MemoryGraphDataset):
     r"""Store and process (full) Cora dataset.
 
     Data loaded from `<https://github.com/abojchevski/graph2gauss/raw/master/data>`_ .
```

### Comparing `kgcnn-2.2.4/kgcnn/data/datasets/CoraLuDataset.py` & `kgcnn-3.0.0/kgcnn/data/datasets/CoraLuDataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-2.2.4/kgcnn/data/datasets/ESOLDataset.py` & `kgcnn-3.0.0/kgcnn/data/datasets/ESOLDataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-2.2.4/kgcnn/data/datasets/FreeSolvDataset.py` & `kgcnn-3.0.0/kgcnn/data/datasets/FreeSolvDataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-2.2.4/kgcnn/data/datasets/GraphTUDataset2020.py` & `kgcnn-3.0.0/kgcnn/data/datasets/GraphTUDataset2020.py`

 * *Files identical despite different names*

### Comparing `kgcnn-2.2.4/kgcnn/data/datasets/ISO17Dataset.py` & `kgcnn-3.0.0/kgcnn/data/datasets/ISO17Dataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-2.2.4/kgcnn/data/datasets/LipopDataset.py` & `kgcnn-3.0.0/kgcnn/data/datasets/LipopDataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-2.2.4/kgcnn/data/datasets/MD17Dataset.py` & `kgcnn-3.0.0/kgcnn/data/datasets/MD17Dataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-2.2.4/kgcnn/data/datasets/MD17RevisedDataset.py` & `kgcnn-3.0.0/kgcnn/data/datasets/MD17RevisedDataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-2.2.4/kgcnn/data/datasets/MUTAGDataset.py` & `kgcnn-3.0.0/kgcnn/data/datasets/MUTAGDataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-2.2.4/kgcnn/data/datasets/MatBenchDataset2020.py` & `kgcnn-3.0.0/kgcnn/data/datasets/MatBenchDataset2020.py`

 * *Files identical despite different names*

### Comparing `kgcnn-2.2.4/kgcnn/data/datasets/MatProjectDielectricDataset.py` & `kgcnn-3.0.0/kgcnn/data/datasets/MatProjectDielectricDataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-2.2.4/kgcnn/data/datasets/MatProjectEFormDataset.py` & `kgcnn-3.0.0/kgcnn/data/datasets/MatProjectEFormDataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-2.2.4/kgcnn/data/datasets/MatProjectGapDataset.py` & `kgcnn-3.0.0/kgcnn/data/datasets/MatProjectGapDataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-2.2.4/kgcnn/data/datasets/MatProjectIsMetalDataset.py` & `kgcnn-3.0.0/kgcnn/data/datasets/MatProjectIsMetalDataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-2.2.4/kgcnn/data/datasets/MatProjectJdft2dDataset.py` & `kgcnn-3.0.0/kgcnn/data/datasets/MatProjectJdft2dDataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-2.2.4/kgcnn/data/datasets/MatProjectLogGVRHDataset.py` & `kgcnn-3.0.0/kgcnn/data/datasets/MatProjectLogGVRHDataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-2.2.4/kgcnn/data/datasets/MatProjectLogKVRHDataset.py` & `kgcnn-3.0.0/kgcnn/data/datasets/MatProjectLogKVRHDataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-2.2.4/kgcnn/data/datasets/MatProjectPerovskitesDataset.py` & `kgcnn-3.0.0/kgcnn/data/datasets/MatProjectPerovskitesDataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-2.2.4/kgcnn/data/datasets/MatProjectPhononsDataset.py` & `kgcnn-3.0.0/kgcnn/data/datasets/MatProjectPhononsDataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-2.2.4/kgcnn/data/datasets/MoleculeNetDataset2018.py` & `kgcnn-3.0.0/kgcnn/data/datasets/MoleculeNetDataset2018.py`

 * *Files identical despite different names*

### Comparing `kgcnn-2.2.4/kgcnn/data/datasets/MutagenicityDataset.py` & `kgcnn-3.0.0/kgcnn/data/datasets/MutagenicityDataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-2.2.4/kgcnn/data/datasets/PROTEINSDataset.py` & `kgcnn-3.0.0/kgcnn/data/datasets/PROTEINSDataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import numpy as np
 
 from kgcnn.data.datasets.GraphTUDataset2020 import GraphTUDataset2020
-from kgcnn.mol.encoder import OneHotEncoder
+from kgcnn.molecule.encoder import OneHotEncoder
 
 
 class PROTEINSDataset(GraphTUDataset2020):
     r"""Store and process PROTEINS dataset from `TUDatasets <https://chrsmrrs.github.io/datasets/>`__ .
 
     In `Papers with Code <https://paperswithcode.com/dataset/proteins>`__ :
     PROTEINS is a dataset of proteins that are classified as enzymes or non-enzymes.
```

### Comparing `kgcnn-2.2.4/kgcnn/data/datasets/QM7Dataset.py` & `kgcnn-3.0.0/kgcnn/data/datasets/QM7Dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 import numpy as np
 import scipy.io
 import json
 import pandas as pd
 from typing import Union
 from kgcnn.data.qm import QMDataset
 from kgcnn.data.download import DownloadDataset
-from kgcnn.mol.io import write_list_to_xyz_file
-from kgcnn.graph.geom import coulomb_matrix_to_inverse_distance_proton, coordinates_from_distance_matrix
-from kgcnn.graph.adj import invert_distance
-from kgcnn.mol.methods import inverse_global_proton_dict
+from kgcnn.molecule.io import write_list_to_xyz_file
+from kgcnn.graph.methods import coulomb_matrix_to_inverse_distance_proton, coordinates_from_distance_matrix
+from kgcnn.graph.methods import invert_distance
+from kgcnn.molecule.methods import inverse_global_proton_dict
 
 
 class QM7Dataset(QMDataset, DownloadDataset):
     r"""Store and process QM7 dataset from `Quantum Machine <http://quantum-machine.org/datasets/>`__ . dataset.
 
     From `Quantum Machine <http://quantum-machine.org/datasets/>`__ :
     This dataset is a subset of GDB-13 (a database of nearly 1 billion stable and synthetically accessible
```

### Comparing `kgcnn-2.2.4/kgcnn/data/datasets/QM7bDataset.py` & `kgcnn-3.0.0/kgcnn/data/datasets/QM7bDataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import os
 import numpy as np
 import scipy.io
 import pandas as pd
 
 from kgcnn.data.qm import QMDataset
 from kgcnn.data.download import DownloadDataset
-from kgcnn.mol.io import write_list_to_xyz_file
-from kgcnn.graph.geom import coulomb_matrix_to_inverse_distance_proton, coordinates_from_distance_matrix
-from kgcnn.graph.adj import invert_distance
-from kgcnn.mol.methods import inverse_global_proton_dict
+from kgcnn.molecule.io import write_list_to_xyz_file
+from kgcnn.graph.methods import coulomb_matrix_to_inverse_distance_proton, coordinates_from_distance_matrix
+from kgcnn.graph.methods import invert_distance
+from kgcnn.molecule.methods import inverse_global_proton_dict
 
 
 class QM7bDataset(QMDataset, DownloadDataset):
     r"""Store and process QM7b dataset from `Quantum Machine <http://quantum-machine.org/datasets/>`__ .
 
     From `Quantum Machine <http://quantum-machine.org/datasets/>`__ :
     This dataset is an extension of the QM7 dataset for multitask learning where 13 additional properties
```

### Comparing `kgcnn-2.2.4/kgcnn/data/datasets/QM8Dataset.py` & `kgcnn-3.0.0/kgcnn/data/datasets/QM8Dataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-2.2.4/kgcnn/data/datasets/QM9Dataset.py` & `kgcnn-3.0.0/kgcnn/data/datasets/QM9Dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # import pickle
 import numpy as np
 import json
 import pandas as pd
 # from typing import Union
 from kgcnn.data.qm import QMDataset
 from kgcnn.data.download import DownloadDataset
-from kgcnn.mol.io import write_list_to_xyz_file
+from kgcnn.molecule.io import write_list_to_xyz_file
 
 
 class QM9Dataset(QMDataset, DownloadDataset):
     r"""Store and process QM9 dataset from `Quantum Machine <http://quantum-machine.org/datasets/>`__ . dataset.
 
     Dataset of 134k stable small organic molecules made up of C,H,O,N,F.
```

### Comparing `kgcnn-2.2.4/kgcnn/data/datasets/QM9MolNetDataset.py` & `kgcnn-3.0.0/kgcnn/data/datasets/QM9MolNetDataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-2.2.4/kgcnn/data/datasets/SIDERDataset.py` & `kgcnn-3.0.0/kgcnn/data/datasets/SIDERDataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-2.2.4/kgcnn/data/datasets/Tox21MolNetDataset.py` & `kgcnn-3.0.0/kgcnn/data/datasets/Tox21MolNetDataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-2.2.4/kgcnn/data/download.py` & `kgcnn-3.0.0/kgcnn/data/download.py`

 * *Files identical despite different names*

### Comparing `kgcnn-2.2.4/kgcnn/data/moleculenet.py` & `kgcnn-3.0.0/kgcnn/data/moleculenet.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import os
 import numpy as np
 import pandas as pd
 
 from typing import Dict, Callable, Union, List
 from collections import defaultdict
-from kgcnn.mol.serial import deserialize_encoder
+from kgcnn.molecule.serial import deserialize_encoder
 from kgcnn.data.base import MemoryGraphDataset
-from kgcnn.mol.base import MolGraphInterface
-from kgcnn.mol.encoder import OneHotEncoder
-from kgcnn.mol.io import write_mol_block_list_to_sdf, read_mol_list_from_sdf_file, write_smiles_file
-from kgcnn.mol.convert import MolConverter
+from kgcnn.molecule.base import MolGraphInterface
+from kgcnn.molecule.encoder import OneHotEncoder
+from kgcnn.molecule.io import write_mol_block_list_to_sdf, read_mol_list_from_sdf_file, write_smiles_file
+from kgcnn.molecule.convert import MolConverter
 
 try:
-    from kgcnn.mol.graph_rdkit import MolecularGraphRDKit
+    from kgcnn.molecule.graph_rdkit import MolecularGraphRDKit
 except ModuleNotFoundError:
     MolecularGraphRDKit = None
 
 
 def map_molecule_callbacks(mol_list: List[str],
                            data: Union[pd.Series, pd.DataFrame],
                            callbacks: Dict[str, Callable[[MolGraphInterface, pd.Series], None]],
```

### Comparing `kgcnn-2.2.4/kgcnn/data/qm.py` & `kgcnn-3.0.0/kgcnn/data/qm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import os
 import numpy as np
 import pandas as pd
 from typing import Union, Callable, List, Dict
-from kgcnn.mol.base import MolGraphInterface
-from kgcnn.data.transform.scaler.mol import QMGraphLabelScaler
+from kgcnn.molecule.base import MolGraphInterface
+from kgcnn.data.transform.scaler.molecule import QMGraphLabelScaler
 from sklearn.preprocessing import StandardScaler
-from kgcnn.mol.serial import deserialize_encoder
+from kgcnn.molecule.serial import deserialize_encoder
 from kgcnn.data.base import MemoryGraphDataset
-from kgcnn.mol.io import parse_list_to_xyz_str, read_xyz_file, \
+from kgcnn.molecule.io import parse_list_to_xyz_str, read_xyz_file, \
     write_mol_block_list_to_sdf, read_mol_list_from_sdf_file, write_list_to_xyz_file
-from kgcnn.mol.methods import global_proton_dict, inverse_global_proton_dict
-from kgcnn.mol.convert import MolConverter
+from kgcnn.molecule.methods import global_proton_dict, inverse_global_proton_dict
+from kgcnn.molecule.convert import MolConverter
 from kgcnn.data.moleculenet import map_molecule_callbacks
 
 try:
-    from kgcnn.mol.graph_babel import MolecularGraphOpenBabel
+    from kgcnn.molecule.graph_babel import MolecularGraphOpenBabel
 except ModuleNotFoundError:
     MolecularGraphOpenBabel = None
 
 try:
-    from kgcnn.mol.graph_rdkit import MolecularGraphRDKit
+    from kgcnn.molecule.graph_rdkit import MolecularGraphRDKit
 except ModuleNotFoundError:
     MolecularGraphRDKit = None
 
 
 class QMDataset(MemoryGraphDataset):
     r"""This is a base class for QM (quantum mechanical) datasets.
```

### Comparing `kgcnn-2.2.4/kgcnn/data/serial.py` & `kgcnn-3.0.0/kgcnn/data/serial.py`

 * *Files identical despite different names*

### Comparing `kgcnn-2.2.4/kgcnn/data/transform/scaler/force.py` & `kgcnn-3.0.0/kgcnn/data/transform/scaler/force.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 import logging
 from typing import Union, List, Dict, Tuple
-from kgcnn.data.transform.scaler.mol import ExtensiveMolecularScalerBase
+from kgcnn.data.transform.scaler.molecule import ExtensiveMolecularScalerBase
 
 logging.basicConfig()  # Module logger
 module_logger = logging.getLogger(__name__)
 module_logger.setLevel(logging.INFO)
 
 
 class EnergyForceExtensiveLabelScaler(ExtensiveMolecularScalerBase):
```

### Comparing `kgcnn-2.2.4/kgcnn/data/transform/scaler/mol.py` & `kgcnn-3.0.0/kgcnn/data/transform/scaler/molecule.py`

 * *Files identical despite different names*

### Comparing `kgcnn-2.2.4/kgcnn/data/transform/scaler/scaler.py` & `kgcnn-3.0.0/kgcnn/data/transform/scaler/standard.py`

 * *Files identical despite different names*

### Comparing `kgcnn-2.2.4/kgcnn/data/transform/scaler/serial.py` & `kgcnn-3.0.0/kgcnn/data/transform/scaler/serial.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 import importlib
 from typing import Union
 from kgcnn.utils.serial import deserialize as deserialize_general
 
 module_list = {
-    "StandardScaler": "kgcnn.data.transform.scaler",
-    "StandardLabelScaler": "kgcnn.data.transform.scaler",
-    "ExtensiveMolecularScaler": "kgcnn.data.transform.mol",
-    "ExtensiveMolecularLabelScaler": "kgcnn.data.transform.mol",
+    "StandardScaler": "kgcnn.data.transform.standard",
+    "StandardLabelScaler": "kgcnn.data.transform.standard",
+    "ExtensiveMolecularScaler": "kgcnn.data.transform.molecule",
+    "ExtensiveMolecularLabelScaler": "kgcnn.data.transform.molecule",
     "EnergyForceExtensiveLabelScaler": "kgcnn.data.transform.force",
     "QMGraphLabelScaler": "kgcnn.data.transform.mol"
 }
 
 
 def deserialize(name: Union[str, dict], **kwargs):
     """Deserialize a scaler class.
 
     Args:
-        name (str, dict): Serialization dictionary of class. This can also be a name of former graph functions for
-            backward compatibility that now coincides with the processor's default name.
+        name (str, dict): Serialization dictionary of class. This can also be a name of a scaler.
         kwargs: Kwargs for processor initialization, if :obj:`name` is string.
 
     Returns:
         GraphPreProcessorBase: Instance of graph preprocessor.
     """
 
     if isinstance(name, dict):
```

### Comparing `kgcnn-2.2.4/kgcnn/data/tudataset.py` & `kgcnn-3.0.0/kgcnn/data/tudataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import numpy as np
 import os
+from typing import Callable
 # import logging
 
 from kgcnn.data.base import MemoryGraphDataset
 
 # TUDataset: A collection of benchmark datasets for learning with graphs
 # by Christopher Morris and Nils M. Kriege and Franka Bause and Kristian Kersting and Petra Mutzel and Marion Neumann
 # http://graphlearning.io
@@ -119,15 +120,15 @@
             g_attr = None
 
         # labels
         num_graphs = np.amax(g_n_id)
         if g_labels is not None:
             if len(g_labels) != num_graphs:
                 self.error(
-                    "Wrong number of graphs, not matching graph labels, {0}, {1}".format(len(g_labels), num_graphs))
+                    "Wrong number of graphs, not matching graph labels, {0}, {1}.".format(len(g_labels), num_graphs))
 
         # shift index, should start at 0 for python indexing
         if int(np.amin(g_n_id)) == 1 and int(np.amin(g_a)) == 1:
             self.info("Shift start of graph ID to zero for '%s' to match python indexing." % name_dataset)
             g_a = g_a - 1
             g_n_id = g_n_id - 1
 
@@ -185,15 +186,15 @@
                            "edge_attributes": e_attr, "edge_indices": edge_indices, "edge_labels": e_labels,
                            "graph_attributes": g_attr, "graph_labels": g_labels}.items():
             self.assign_property(key, value)
 
         return self
 
     @staticmethod
-    def read_csv_simple(filepath: str, delimiter: str = ",", dtype=float):
+    def read_csv_simple(filepath: str, delimiter: str = ",", dtype: Callable = float):
         """Very simple python-only function to read in a csv-file from file.
 
         Args:
             filepath (str): Full filepath of csv-file to read in.
             delimiter (str): Delimiter character for separation. Default is ",".
             dtype: Callable type conversion from string. Default is float.
```

### Comparing `kgcnn-2.2.4/kgcnn/data/utils.py` & `kgcnn-3.0.0/kgcnn/data/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,23 +118,23 @@
     elif type_ending == "pickle":
         return load_pickle_file(file_name, **kwargs)
     elif type_ending == "py":
         path = os.path.realpath(file_name)
         hyper = getattr(SourceFileLoader(os.path.basename(path).replace(".py", ""), path).load_module(), "hyper")
         return hyper
     else:
-        module_logger.error("Unsupported file type %s" % type_ending)
+        module_logger.error("Unsupported file type '%s'." % type_ending)
     return {}
 
 
-def ragged_tensor_from_nested_numpy(numpy_list: list, dtype: str = None, row_splits_dtype = "int64"):
+def ragged_tensor_from_nested_numpy(numpy_list: list, dtype: str = None, row_splits_dtype: str = "int64"):
     r"""Make ragged tensor from a list of numpy arrays. Each array can have different length but must match in shape
     except the first dimension.
     This will result in a ragged tensor with ragged dimension only at first axis (ragged_rank=1), like
-    shape `(batch, None, ...)`. This way a tensor can be generated faster than tf.ragged.constant().
+    shape `(batch, None, ...)` . This way a tensor can be generated faster than `tf.ragged.constant()` .
 
     .. warning::
         The data will be copied for this operation.
 
     .. code-block:: python
 
         import tensorflow as tf
@@ -157,15 +157,15 @@
         np.concatenate(numpy_list, axis=0, dtype=dtype), np.array([len(x) for x in numpy_list], dtype=row_splits_dtype))
 
 
 def pad_np_array_list_batch_dim(values: list):
     r"""Pad a list of numpy arrays along first dimension.
 
     Args:
-        values (list): List of :obj:`np.ndarray`.
+        values (list): List of :obj:`np.ndarray` .
 
     Returns:
         tuple: Padded and mask :obj:`np.ndarray` of values.
     """
     max_shape = np.amax([x.shape for x in values], axis=0)
     final_shape = np.concatenate([np.array([len(values)]), max_shape])
     padded = np.zeros(final_shape, dtype=values[0].dtype)
```

### Comparing `kgcnn-2.2.4/kgcnn/graph/adj.py` & `kgcnn-3.0.0/kgcnn/graph/methods/_adj.py`

 * *Files identical despite different names*

### Comparing `kgcnn-2.2.4/kgcnn/graph/base.py` & `kgcnn-3.0.0/kgcnn/graph/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
 import re
 import logging
 import networkx as nx
 from collections.abc import MutableMapping
 from kgcnn.graph.serial import get_preprocessor
-from typing import Any, Union
+from typing import Any, Union, List
 from copy import deepcopy, copy
 
 logging.basicConfig()  # Module logger
 module_logger = logging.getLogger(__name__)
 module_logger.setLevel(logging.INFO)
 
 
@@ -172,29 +172,32 @@
         if key not in self or self.obtain_property(key) is None:
             return False
         return True
 
     def from_networkx(self, graph: nx.Graph,
                       node_number: str = "node_number",
                       edge_indices: str = "edge_indices",
-                      node_attributes: str = None,
-                      edge_attributes: str = None,
+                      node_attributes: Union[str, List[str]] = None,
+                      edge_attributes: Union[str, List[str]] = None,
+                      graph_attributes: Union[str, List[str]] = None,
                       node_labels: str = None):
         r"""Convert a networkx graph instance into a dictionary of graph-tensors. The networkx graph is always converted
         into integer node labels. The former node IDs can be hold in :obj:`node_labels`. Furthermore, node or edge
         data can be cast into attributes via :obj:`node_attributes` and :obj:`edge_attributes`.
 
         Args:
             graph (nx.Graph): A networkx graph instance to convert.
             node_number (str): The name that the node numbers are assigned to. Default is "node_number".
             edge_indices (str): The name that the edge indices are assigned to. Default is "edge_indices".
             node_attributes (str, list): Name of node attributes to add from node data. Can also be a list of names.
                 Default is None.
             edge_attributes (str, list): Name of edge attributes to add from edge data. Can also be a list of names.
                 Default is None.
+            graph_attributes (str, list): Name of graph attributes to add from graph data. Can also be a list of names.
+                Default is None.
             node_labels (str): Name of the labels of nodes to store former node IDs into. Default is None.
 
         Returns:
             self.
         """
         assert node_labels is None or isinstance(node_labels, str), "Please provide name of node labels or `None`"
         graph_int = nx.convert_node_labels_to_integers(graph, label_attribute=node_labels)
@@ -215,34 +218,45 @@
             node_attr += [node_labels]
         node_attr_dict = {x: [None] * graph_size for x in node_attr}
         nodes_id = []
         for i, x in enumerate(graph_int.nodes.data()):
             nodes_id.append(x[0])
             for d in node_attr:
                 if d not in x[1]:
-                    raise KeyError("Node does not have property %s" % d)
+                    raise KeyError("Node does not have property '%s'." % d)
                 node_attr_dict[d][i] = x[1][d]
 
+        # Loop over edges in graph.
         edge_id = []
         edges_attr = _attr_to_list(edge_attributes)
-        edges_attr_dict = {x: [None] * graph.number_of_edges() for x in edges_attr}
+        edges_attr_dict = {x: [None] * graph_int.number_of_edges() for x in edges_attr}
         for i, x in enumerate(graph_int.edges.data()):
             edge_id.append(x[:2])
             for d in edges_attr:
                 if d not in x[2]:
-                    raise KeyError("Edge does not have property %s" % d)
+                    raise KeyError("Edge does not have property '%s'." % d)
                 edges_attr_dict[d][i] = x[2][d]
 
+        graph_attr = _attr_to_list(graph_attributes)
+        graph_attr_dict = {x: None for x in graph_attr}
+        # We use original graph input for this. Does not need node relabeling.
+        for _, x in enumerate(graph_attr):
+            # This is a temporary solution until we find a better way to store graph-level information.
+            if hasattr(graph, x):
+                graph_attr_dict[x] = getattr(graph, x)
+
         # Storing graph tensors in self.
         self.assign_property(node_number, nodes_id)
         self.assign_property(edge_indices, edge_id)
         for key, value in node_attr_dict.items():
             self.assign_property(key, value)
         for key, value in edges_attr_dict.items():
             self.assign_property(key, value)
+        for key, value in graph_attr_dict.items():
+            self.assign_property(key, value)
         return self
 
     def to_networkx(self, edge_indices: str = "edge_indices"):
         """Function draft to make a networkx graph. No attributes or data is supported at the moment.
 
         Args:
             edge_indices (str): Name of edge index tensors to make graph with. Default is "edge_indices".
```

### Comparing `kgcnn-2.2.4/kgcnn/graph/geom.py` & `kgcnn-3.0.0/kgcnn/graph/methods/_geom.py`

 * *Files identical despite different names*

### Comparing `kgcnn-2.2.4/kgcnn/graph/postprocessor.py` & `kgcnn-3.0.0/kgcnn/graph/postprocessor.py`

 * *Files identical despite different names*

### Comparing `kgcnn-2.2.4/kgcnn/graph/preprocessor.py` & `kgcnn-3.0.0/kgcnn/graph/preprocessor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,12 @@
 import numpy as np
 import logging
 from typing import Union
 from kgcnn.graph.base import GraphPreProcessorBase
-from kgcnn.graph.adj import get_angle_indices, coordinates_to_distancematrix, invert_distance, \
-    define_adjacency_from_distance, sort_edge_indices, get_angle, add_edges_reverse_indices, \
-    rescale_edge_weights_degree_sym, add_self_loops_to_edge_indices, compute_reverse_edges_index_map, \
-    distance_to_gauss_basis
-from kgcnn.graph.geom import range_neighbour_lattice, get_principal_moments_of_inertia, \
-    shift_coordinates_to_unit_cell, distance_for_range_indices, distance_for_range_indices_periodic
+from kgcnn.graph.methods import *
 
 logging.basicConfig()  # Module logger
 module_logger = logging.getLogger(__name__)
 module_logger.setLevel(logging.INFO)
 
 
 class MakeUndirectedEdges(GraphPreProcessorBase):
```

### Comparing `kgcnn-2.2.4/kgcnn/graph/serial.py` & `kgcnn-3.0.0/kgcnn/graph/serial.py`

 * *Files identical despite different names*

### Comparing `kgcnn-2.2.4/kgcnn/hyper/hyper.py` & `kgcnn-3.0.0/kgcnn/training/hyper.py`

 * *Files identical despite different names*

### Comparing `kgcnn-2.2.4/kgcnn/io/loader.py` & `kgcnn-3.0.0/kgcnn/io/loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Union, List
 from kgcnn.data.utils import ragged_tensor_from_nested_numpy
 from kgcnn.data.base import MemoryGraphDataset
 ks = tf.keras
 
 
 class GraphBatchLoader(ks.utils.Sequence):
-    r"""Example (minimal) implementation of a graph batch loader based on :obj:`ks.utils.Sequence`."""
+    r"""Example (minimal) implementation of a graph batch loader based on :obj:`ks.utils.Sequence` ."""
 
     def __init__(self,
                  data: Union[List[dict], MemoryGraphDataset],
                  inputs: Union[dict, List[dict]],
                  outputs: Union[dict, List[dict]],
                  batch_size: int = 32,
                  shuffle: bool = False):
```

### Comparing `kgcnn-2.2.4/kgcnn/layers/base.py` & `kgcnn-3.0.0/kgcnn/layers/base.py`

 * *Files identical despite different names*

### Comparing `kgcnn-2.2.4/kgcnn/layers/casting.py` & `kgcnn-3.0.0/kgcnn/layers/casting.py`

 * *Files identical despite different names*

### Comparing `kgcnn-2.2.4/kgcnn/layers/conv/acsf_conv.py` & `kgcnn-3.0.0/kgcnn/literature/HDNNP2nd/_acsf_conv.py`

 * *Files identical despite different names*

### Comparing `kgcnn-2.2.4/kgcnn/layers/conv/attentivefp_conv.py` & `kgcnn-3.0.0/kgcnn/literature/AttentiveFP/_attentivefp_conv.py`

 * *Files identical despite different names*

### Comparing `kgcnn-2.2.4/kgcnn/layers/conv/cgcnn_conv.py` & `kgcnn-3.0.0/kgcnn/literature/CGCNN/_cgcnn_conv.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 from kgcnn.layers.modules import Activation, LazyMultiply, LazyConcatenate, LazyAdd, Dense
 ks = tf.keras
 
 
 @ks.utils.register_keras_serializable(package='kgcnn', name='CGCNNLayer')
 class CGCNNLayer(MessagePassingBase):
     r"""Message Passing Layer used in the Crystal Graph Convolutional Neural Network:
-    `CGCNN <https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.120.145301>`_.
+
+    `CGCNN <https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.120.145301>`__ .
 
     Based on the original code in pytorch (<https://github.com/txie-93/cgcnn>).
 
     Args:
         units (int): Units for Dense layer.
         activation_s (str): Tensorflow activation applied before gating the message.
         activation_out (str): Tensorflow activation applied the very end of the layer (after gating).
```

### Comparing `kgcnn-2.2.4/kgcnn/layers/conv/dimenet_conv.py` & `kgcnn-3.0.0/kgcnn/literature/DimeNetPP/_dimenet_conv.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,85 +1,19 @@
 import tensorflow as tf
 
 from kgcnn.layers.base import GraphBaseLayer
 from kgcnn.layers.modules import Dense, LazyMultiply, LazyAdd
 from kgcnn.layers.pooling import PoolingLocalEdges
 from kgcnn.layers.gather import GatherNodesOutgoing
 from kgcnn.layers.mlp import GraphMLP
+from kgcnn.layers.update import ResidualLayer
 from kgcnn.ops.polynom import spherical_bessel_jn_zeros, spherical_bessel_jn_normalization_prefactor, \
     tf_spherical_bessel_jn, tf_spherical_harmonics_yl
 
 
-@tf.keras.utils.register_keras_serializable(package='kgcnn', name='ResidualLayer')
-class ResidualLayer(GraphBaseLayer):
-    """Residual Layer as defined by `DimNetPP <https://arxiv.org/abs/2011.14115>`_ .
-
-    Args:
-        units: Dimension of the kernel.
-        use_bias (bool, optional): Use bias. Defaults to True.
-        activation (str): Activation function. Default is "kgcnn>swish".
-        kernel_regularizer: Kernel regularization. Default is None.
-        bias_regularizer: Bias regularization. Default is None.
-        activity_regularizer: Activity regularization. Default is None.
-        kernel_constraint: Kernel constrains. Default is None.
-        bias_constraint: Bias constrains. Default is None.
-        kernel_initializer: Initializer for kernels. Default is 'glorot_uniform'.
-        bias_initializer: Initializer for bias. Default is 'zeros'.
-    """
-
-    def __init__(self, units,
-                 use_bias=True,
-                 activation='kgcnn>swish',
-                 kernel_regularizer=None,
-                 bias_regularizer=None,
-                 activity_regularizer=None,
-                 kernel_constraint=None,
-                 bias_constraint=None,
-                 kernel_initializer='glorot_uniform',
-                 bias_initializer='zeros',
-                 **kwargs):
-        """Initialize layer."""
-        super(ResidualLayer, self).__init__(**kwargs)
-        dense_args = {"units": units, "activation": activation, "use_bias": use_bias,
-                      "kernel_regularizer": kernel_regularizer, "activity_regularizer": activity_regularizer,
-                      "bias_regularizer": bias_regularizer, "kernel_constraint": kernel_constraint,
-                      "bias_constraint": bias_constraint, "kernel_initializer": kernel_initializer,
-                      "bias_initializer": bias_initializer}
-
-        self.dense_1 = Dense(**dense_args)
-        self.dense_2 = Dense(**dense_args)
-        self.add_end = LazyAdd()
-
-    def build(self, input_shape):
-        """Build layer."""
-        super(ResidualLayer, self).build(input_shape)
-
-    def call(self, inputs, **kwargs):
-        """Forward pass.
-
-        Args:
-            inputs (tf.RaggedTensor): Node or edge embedding of shape (batch, [N], F)
-
-        Returns:
-            tf.RaggedTensor: Node or edge embedding of shape (batch, [N], F)
-        """
-        x = self.dense_1(inputs, **kwargs)
-        x = self.dense_2(x, **kwargs)
-        x = self.add_end([inputs, x], **kwargs)
-        return x
-
-    def get_config(self):
-        config = super(ResidualLayer, self).get_config()
-        conf_dense = self.dense_1.get_config()
-        for x in ["kernel_regularizer", "activity_regularizer", "bias_regularizer", "kernel_constraint",
-                  "bias_constraint", "kernel_initializer", "bias_initializer", "activation", "use_bias", "units"]:
-            config.update({x: conf_dense[x]})
-        return config
-
-
 @tf.keras.utils.register_keras_serializable(package='kgcnn', name='DimNetInteractionPPBlock')
 class DimNetInteractionPPBlock(GraphBaseLayer):
     """DimNetPP Interaction Block as defined by `DimNetPP <https://arxiv.org/abs/2011.14115>`_ .
 
     Args:
         emb_size: Embedding size used for the messages
         int_emb_size (int): Embedding size used for interaction triplets
@@ -322,16 +256,17 @@
         config.update({"emb_size": self.emb_size, "out_emb_size": self.out_emb_size, "num_dense": self.num_dense,
                        "num_targets": self.num_targets})
         return config
 
 
 @tf.keras.utils.register_keras_serializable(package='kgcnn', name='EmbeddingDimeBlock')
 class EmbeddingDimeBlock(tf.keras.layers.Layer):
-    """Custom Embedding Block of `DimNetPP <https://arxiv.org/abs/2011.14115>`_ . Naming of inputs here should match
-    keras Embedding layer.
+    """Custom Embedding Block of `DimNetPP <https://arxiv.org/abs/2011.14115>`__ .
+
+    Naming of inputs here should match keras Embedding layer.
 
     Args:
         input_dim (int): Integer. Size of the vocabulary, i.e. maximum integer index + 1.
         output_dim (int): Integer. Dimension of the dense embedding.
         embeddings_initializer: Initializer for the embeddings matrix (see keras.initializers).
         embeddings_regularizer: Regularizer function applied to the embeddings matrix (see keras.regularizers).
         embeddings_constraint: Constraint function applied to the embeddings matrix (see keras.constraints).
@@ -375,21 +310,22 @@
                        })
         return config
 
 
 @tf.keras.utils.register_keras_serializable(package='kgcnn', name='SphericalBasisLayer')
 class SphericalBasisLayer(GraphBaseLayer):
     r"""Expand a distance into a Bessel Basis with :math:`l=m=0`, according to
-    `Klicpera et al. 2020 <https://arxiv.org/abs/2011.14115>`_ .
+    `Klicpera et al. 2020 <https://arxiv.org/abs/2011.14115>`__ .
 
     Args:
         num_spherical (int): Number of spherical basis functions
         num_radial (int): Number of radial basis functions
         cutoff (float): Cutoff distance c
         envelope_exponent (int): Degree of the envelope to smoothen at cutoff. Default is 5.
+
     """
 
     def __init__(self, num_spherical,
                  num_radial,
                  cutoff,
                  envelope_exponent=5,
                  **kwargs):
```

### Comparing `kgcnn-2.2.4/kgcnn/layers/conv/dmpnn_conv.py` & `kgcnn-3.0.0/kgcnn/layers/message.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,89 +1,104 @@
 import tensorflow as tf
 
 from kgcnn.layers.base import GraphBaseLayer
-from kgcnn.layers.gather import GatherNodesOutgoing, GatherNodesIngoing
+from kgcnn.layers.gather import GatherEmbeddingSelection
 from kgcnn.layers.pooling import PoolingLocalEdges
-from kgcnn.layers.modules import LazySubtract
 
 
-@tf.keras.utils.register_keras_serializable(package='kgcnn', name='DMPNNGatherEdgesPairs')
-class DMPNNGatherEdgesPairs(GraphBaseLayer):
-    """Gather edge pairs that also works for invalid indices given a certain pair, i.e. if a edge does not have its
-    reverse counterpart in the edge indices list.
-    This class is used in `DMPNN <https://pubs.acs.org/doi/full/10.1021/acs.jcim.9b00237>`_ .
+@tf.keras.utils.register_keras_serializable(package='kgcnn', name='MessagePassingBase')
+class MessagePassingBase(GraphBaseLayer):
+    r"""Base layer for Message passing type networks. This is a general frame to implement custom message and
+    update functions. The idea is to create a subclass of :obj:`MessagePassingBase` and then just implement the methods
+    :obj:`message_function` and :obj:`update_nodes`. The pooling or aggregating is handled by built-in
+    :obj:`PoolingLocalEdges`.
 
+    Alternatively also :obj:`aggregate_message` could be overwritten.
+    The original message passing scheme was proposed by `NMPNN <http://arxiv.org/abs/1704.01212>`_ .
     """
 
-    def __init__(self, **kwargs):
-        """Initialize layer."""
-        super(DMPNNGatherEdgesPairs, self).__init__(**kwargs)
-        self.gather_layer = GatherNodesIngoing()
-
-    def build(self, input_shape):
-        """Build layer."""
-        super(DMPNNGatherEdgesPairs, self).build(input_shape)
+    def __init__(self, pooling_method: str = "sum", **kwargs):
+        r"""Initialize :obj:`MessagePassingBase` layer.
 
-    def call(self, inputs, **kwargs):
-        """Forward pass.
+        Args:
+            pooling_method (str): Aggregation method of edges. Default is "sum".
+        """
+        super(MessagePassingBase, self).__init__(**kwargs)
+        self.pooling_method = pooling_method
+        self.lay_gather = GatherEmbeddingSelection([0, 1])
+        self.lay_pool_default = PoolingLocalEdges(pooling_method=self.pooling_method)
+
+    def message_function(self, inputs, **kwargs):
+        r"""Defines the message function, i.e. a method the generates a message from node and edge embeddings at a
+        certain depth (not considered here).
 
         Args:
-            inputs (list): [edges, pair_index]
+            inputs: [nodes_in, nodes_out, edge_index]
 
-                - edges (tf.RaggedTensor): Node embeddings of shape (batch, [M], F)
-                - pair_index (tf.RaggedTensor): Edge indices referring to edges of shape (batch, [M], 1)
+                - nodes (tf.RaggedTensor): Receiving node embeddings of shape (batch, [N], F)
+                - nodes_out (tf.RaggedTensor): Sending node embeddings of shape (batch, [N], F)
+                - edge_index (tf.RaggedTensor): Edge indices referring to nodes of shape (batch, [M], 2)
 
         Returns:
-            list: Gathered edge embeddings that match the reverse edges of shape (batch, [M], F) for selection_index.
+            tf.RaggedTensor: Messages for each edge of shape (batch, [M], F)
         """
-        self.assert_ragged_input_rank(inputs)
-        edges, pair_index = inputs
-        index_corrected = tf.RaggedTensor.from_row_splits(
-            tf.where(pair_index.values >= 0, pair_index.values, tf.zeros_like(pair_index.values)),
-            pair_index.row_splits, validate=self.ragged_validate)
-        edges_paired = self.gather_layer([edges, index_corrected], **kwargs)
-        edges_corrected = tf.RaggedTensor.from_row_splits(
-            tf.where(pair_index.values >= 0, edges_paired.values, tf.zeros_like(edges_paired.values)),
-            edges_paired.row_splits, validate=self.ragged_validate)
-        return edges_corrected
-
-
-@tf.keras.utils.register_keras_serializable(package='kgcnn', name='DMPNNPPoolingEdgesDirected')
-class DMPNNPPoolingEdgesDirected(GraphBaseLayer):
-    """Pooling of edges for around a target node as defined by
-    `DMPNN <https://pubs.acs.org/doi/full/10.1021/acs.jcim.9b00237>`_ . This slightly different than the normal node
-    aggregation from message passing like networks. Requires edge pairs for this implementation.
+        n_in, n_out, edges = inputs
+        raise NotImplementedError(
+            "A method to generate messages must be implemented in sub-class of `MessagePassingBase`.")
 
-    """
+    def aggregate_message(self, inputs, **kwargs):
+        r"""Pre-defined message aggregation that uses :obj:`PoolingLocalEdges`.
+
+        Args:
+            inputs: [nodes, edges, edge_index]
+
+                - nodes (tf.RaggedTensor): Node embeddings of shape (batch, [N], F)
+                - edges (tf.RaggedTensor): Edge or message embeddings of shape (batch, [M], F)
+                - edge_index (tf.RaggedTensor): Edge indices referring to nodes of shape (batch, [M], 2)
+
+        Returns:
+            tf.RaggedTensor: Aggregated edge embeddings per node of shape (batch, [N], F)
+        """
+        return self.lay_pool_default(inputs, **kwargs)
+
+    def update_nodes(self, inputs, **kwargs):
+        r"""Defines the update function, i.e. a method that updates the node embeddings from aggregated messages.
 
-    def __init__(self, **kwargs):
-        """Initialize layer."""
-        super(DMPNNPPoolingEdgesDirected, self).__init__(**kwargs)
-        self.pool_edge_1 = PoolingLocalEdges(pooling_method="sum")
-        self.gather_edges = GatherNodesOutgoing()
-        self.gather_pairs = DMPNNGatherEdgesPairs()
-        self.subtract_layer = LazySubtract()
-
-    def build(self, input_shape):
-        """Build layer."""
-        super(DMPNNPPoolingEdgesDirected, self).build(input_shape)
+        Args:
+            inputs: [nodes, node_updates]
+
+                - nodes (tf.RaggedTensor): Node embeddings (from previous step) of shape (batch, [N], F)
+                - node_updates (tf.RaggedTensor): Updates for nodes of shape (batch, [N], F)
+
+        Returns:
+            tf.RaggedTensor: Updated node embeddings (for next step) of shape (batch, [N], F)
+        """
+        nodes, nodes_update = inputs
+        raise NotImplementedError(
+            "A method to update nodes must be implemented in sub-class of `MessagePassingBase`.")
 
     def call(self, inputs, **kwargs):
-        """Forward pass.
+        r"""Pre-implemented standard message passing scheme using :obj:`update_nodes`, :obj:`aggregate_message` and
+        :obj:`message_function`.
 
         Args:
-            inputs: [nodes, edges, edge_index, edge_reverse_pair]
+            inputs: [nodes, edges, edge_index]
 
                 - nodes (tf.RaggedTensor): Node embeddings of shape (batch, [N], F)
                 - edges (tf.RaggedTensor): Edge or message embeddings of shape (batch, [M], F)
                 - edge_index (tf.RaggedTensor): Edge indices referring to nodes of shape (batch, [M], 2)
-                - edge_reverse_pair (tf.RaggedTensor): Pair mappings for reverse edges (batch, [M], 1)
 
         Returns:
-            tf.RaggedTensor: Edge embeddings of shape (batch, [M], F)
+            tf.RaggedTensor: Updated node embeddings of shape (batch, [N], F)
         """
-        n, ed, edi, edp = inputs
-        pool_edge_receive = self.pool_edge_1([n, ed, edi], **kwargs)  # Sum pooling of all edges
-        ed_new = self.gather_edges([pool_edge_receive, edi], **kwargs)
-        ed_not = self.gather_pairs([ed, edp],  **kwargs)
-        out = self.subtract_layer([ed_new, ed_not],  **kwargs)
-        return out
+        nodes, edges, edge_index = inputs
+        n_in, n_out = self.lay_gather([nodes, edge_index], **kwargs)
+        msg = self.message_function([n_in, n_out, edges], **kwargs)
+        pool_n = self.aggregate_message([nodes, msg, edge_index], **kwargs)
+        n_new = self.update_nodes([nodes, pool_n], **kwargs)
+        return n_new
+
+    def get_config(self):
+        """Update config."""
+        config = super(MessagePassingBase, self).get_config()
+        config.update({"pooling_method": self.pooling_method})
+        return config
```

### Comparing `kgcnn-2.2.4/kgcnn/layers/conv/gat_conv.py` & `kgcnn-3.0.0/kgcnn/layers/attention.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import tensorflow as tf
 
 from kgcnn.layers.base import GraphBaseLayer
 from kgcnn.layers.gather import GatherNodesIngoing, GatherNodesOutgoing
-from kgcnn.layers.modules import Dense, LazyConcatenate, LazyAverage, Activation
+from kgcnn.layers.modules import Dense, LazyConcatenate, Activation, LazyAverage
 from kgcnn.layers.pooling import PoolingLocalEdgesAttention
 
 
 @tf.keras.utils.register_keras_serializable(package='kgcnn', name='AttentionHeadGAT')
 class AttentionHeadGAT(GraphBaseLayer):
-    r"""Computes the attention head according to `GAT <https://arxiv.org/abs/1710.10903>`_ .
+    r"""Computes the attention head according to `GAT <https://arxiv.org/abs/1710.10903>`__ .
+
     The attention coefficients are computed by :math:`a_{ij} = \sigma(a^T W n_i || W n_j)`,
     optionally by :math:`a_{ij} = \sigma( W n_i || W n_j || e_{ij})` with edges :math:`e_{ij}`.
     The attention is obtained by :math:`\alpha_{ij} = \text{softmax}_j (a_{ij})`.
     And the messages are pooled by :math:`m_i = \sum_j \alpha_{ij} W n_j`.
     If the graph has no self-loops, they must be added beforehand or use external skip connections.
     And optionally passed through an activation :math:`h_i = \sigma(\sum_j \alpha_{ij} W n_j)`.
 
@@ -92,15 +93,15 @@
         w_n = self.lay_linear_trafo(node, **kwargs)
         wn_in = self.lay_gather_in([w_n, edge_index], **kwargs)
         wn_out = self.lay_gather_out([w_n, edge_index], **kwargs)
         if self.use_edge_features:
             e_ij = self.lay_concat([wn_in, wn_out, edge], **kwargs)
         else:
             e_ij = self.lay_concat([wn_in, wn_out], **kwargs)
-        a_ij = self.lay_alpha(e_ij, **kwargs)  # Should be dimension (batch*None,1)
+        a_ij = self.lay_alpha(e_ij, **kwargs)  # Should be dimension (batch, None,1)
         h_i = self.lay_pool_attention([node, wn_out, a_ij, edge_index], **kwargs)
 
         if self.use_final_activation:
             h_i = self.lay_final_activ(h_i, **kwargs)
         return h_i
 
     def get_config(self):
@@ -114,15 +115,16 @@
                   "bias_constraint", "kernel_initializer", "bias_initializer", "activation"]:
             config.update({x: conf_sub[x]})
         return config
 
 
 @tf.keras.utils.register_keras_serializable(package='kgcnn', name='AttentionHeadGATV2')
 class AttentionHeadGATV2(GraphBaseLayer):
-    r"""Computes the modified attention head according to `GATv2 <https://arxiv.org/pdf/2105.14491.pdf>`_ .
+    r"""Computes the modified attention head according to `GATv2 <https://arxiv.org/pdf/2105.14491.pdf>`__ .
+
     The attention coefficients are computed by :math:`a_{ij} = a^T \sigma( W [n_i || n_j] )`,
     optionally by :math:`a_{ij} = a^T \sigma( W [n_i || n_j || e_{ij}] )` with edges :math:`e_{ij}`.
     The attention is obtained by :math:`\alpha_{ij} = \text{softmax}_j (a_{ij})`.
     And the messages are pooled by :math:`m_i =  \sum_j \alpha_{ij} e_{ij}`.
     If the graph has no self-loops, they must be added beforehand or use external skip connections.
     And optionally passed through an activation :math:`h_i = \sigma(\sum_j \alpha_{ij} e_{ij})`.
 
@@ -317,8 +319,8 @@
         """Update layer config."""
         config = super(MultiHeadGATV2Layer, self).get_config()
         config.update({
             'num_heads': self.num_heads,
             'concat_heads': self.concat_heads
         })
 
-        return config
+        return config
```

### Comparing `kgcnn-2.2.4/kgcnn/layers/conv/gin_conv.py` & `kgcnn-3.0.0/kgcnn/literature/GIN/_gin_conv.py`

 * *Files identical despite different names*

### Comparing `kgcnn-2.2.4/kgcnn/layers/conv/hamnet_conv.py` & `kgcnn-3.0.0/kgcnn/literature/HamNet/_hamnet_conv.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import tensorflow as tf
 from kgcnn.layers.base import GraphBaseLayer
-from kgcnn.layers.gather import GatherNodesOutgoing, GatherState, GatherEmbeddingSelection
+from kgcnn.layers.gather import GatherState, GatherEmbeddingSelection
 from kgcnn.layers.pooling import PoolingLocalEdgesAttention, PoolingNodes, PoolingNodesAttention
 from kgcnn.layers.modules import LazySubtract, Dense, Dropout, LazyConcatenate, Activation
-from kgcnn.layers.conv.mpnn_conv import GRUUpdate
+from kgcnn.layers.update import GRUUpdate
+
 # import tensorflow.keras as ks
 # import tensorflow.python.keras as ks
 ks = tf.keras
 
 # Gated recurrent unit update. See kgcnn.layers.conv.mpnn_conv for details.
 HamNetGRUUnion = GRUUpdate
 
@@ -538,59 +539,7 @@
         if self.use_dropout:
             conf_drop = self.dropout_layer.get_config()
             for x in ["rate", "noise_shape", "seed"]:
                 config.update({x: conf_drop[x]})
         conf_last = self.final_activ.get_config()
         config.update({"activation_last": conf_last["activation"]})
         return config
-
-
-# @ks.utils.register_keras_serializable(package='kgcnn', name='HamiltonEngine')
-# class HamiltonEngine(GraphBaseLayer):
-#     def __init__(self,
-#                  units,
-#                  activation="kgcnn>leaky_relu",
-#                  use_bias=True,
-#                  kernel_regularizer=None,
-#                  bias_regularizer=None,
-#                  activity_regularizer=None,
-#                  kernel_constraint=None,
-#                  bias_constraint=None,
-#                  kernel_initializer='glorot_uniform',
-#                  bias_initializer='zeros',
-#                  **kwargs):
-#         """Initialize layer."""
-#         super(HamiltonEngine, self).__init__(**kwargs)
-#         self.units = int(units)
-#         self.use_bias = bool(use_bias)
-#         kernel_args = {"kernel_regularizer": kernel_regularizer,
-#                        "activity_regularizer": activity_regularizer, "bias_regularizer": bias_regularizer,
-#                        "kernel_constraint": kernel_constraint, "bias_constraint": bias_constraint,
-#                        "kernel_initializer": kernel_initializer, "bias_initializer": bias_initializer}
-#         self.dense_atom = Dense(units=units, activation="tanh", use_bias=use_bias, **kernel_args)
-#         self.dense_edge = Dense(units=units, activation="tanh", use_bias=use_bias, **kernel_args)
-#
-#     def build(self, input_shape):
-#         """Build layer."""
-#         super(HamiltonEngine, self).build(input_shape)
-#
-#     def call(self, inputs, **kwargs):
-#         """Forward pass.
-#
-#         Args:
-#             inputs: [nodes, edge, edge_indices]
-#
-#                 - nodes (tf.RaggedTensor): Node features of shape (batch, [N], F)
-#
-#         Returns:
-#             tf.RaggedTensor: Embedding tensor of pooled node attentions of shape (batch, F)
-#         """
-#         atom_ftr, bond_ftr, edge_idx = inputs
-#         hv_ftr = self.dense_atom(atom_ftr, **kwargs)
-#         he_ftr = self.dense_edge(bond_ftr, **kwargs)
-#         return
-#
-#     def get_config(self):
-#         """Update layer config."""
-#         config = super(HamiltonEngine, self).get_config()
-#         config.update({"use_bias": self.use_bias, "units": self.units,})
-#         return config
```

### Comparing `kgcnn-2.2.4/kgcnn/layers/conv/hdnnp_conv.py` & `kgcnn-3.0.0/kgcnn/literature/HDNNP4th/_hdnnp_conv.py`

 * *Files identical despite different names*

### Comparing `kgcnn-2.2.4/kgcnn/layers/conv/megnet_conv.py` & `kgcnn-3.0.0/kgcnn/literature/Megnet/_megnet_conv.py`

 * *Files identical despite different names*

### Comparing `kgcnn-2.2.4/kgcnn/layers/conv/mpnn_conv.py` & `kgcnn-3.0.0/kgcnn/layers/update.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,201 +1,104 @@
 import tensorflow as tf
-import tensorflow.keras as ks
 
 from kgcnn.layers.base import GraphBaseLayer
-from kgcnn.layers.modules import Dense
-
-
-@tf.keras.utils.register_keras_serializable(package='kgcnn', name='TrafoEdgeNetMessages')
-class TrafoEdgeNetMessages(GraphBaseLayer):
-    """Make message from edges for a linear transformation, i.e. matrix multiplication.
-    The actual matrix is not a trainable weight of this layer but generated by a dense layer.
-    This was proposed by `NMPNN <http://arxiv.org/abs/1704.01212>`_ .
-
-    Args:
-        target_shape (int): Target shape for message matrix.
-    """
-
-    def __init__(self, target_shape,
-                 activation="linear",
-                 use_bias=True,
-                 kernel_regularizer=None, bias_regularizer=None, activity_regularizer=None,
-                 kernel_constraint=None, bias_constraint=None,
-                 kernel_initializer='glorot_uniform', bias_initializer='zeros',
-                 **kwargs):
-        """Initialize layer."""
-        super(TrafoEdgeNetMessages, self).__init__(**kwargs)
-        self.target_shape = target_shape
-        self._units_out = int(target_shape[0])
-        self._units_in = int(target_shape[1])
-        self.lay_dense = Dense(units=self._units_out * self._units_in,
-                               activation=activation, use_bias=use_bias,
-                               kernel_regularizer=kernel_regularizer, bias_regularizer=bias_regularizer,
-                               activity_regularizer=activity_regularizer, kernel_constraint=kernel_constraint,
-                               bias_constraint=bias_constraint, kernel_initializer=kernel_initializer,
-                               bias_initializer=bias_initializer)
-
-    def build(self, input_shape):
-        """Build layer."""
-        super(TrafoEdgeNetMessages, self).build(input_shape)
-
-    def call(self, inputs, **kwargs):
-        """Forward pass.
-
-        Args:
-            inputs (tf.RaggedTensor): Messages embeddings or messages (batch, [M], F)
-
-        Returns:
-            tf.RaggedTensor: Messages in matrix for multiplication of shape (batch, [M], F, F)
-        """
-        self.assert_ragged_input_rank(inputs)
-        up_scale = self.lay_dense(inputs, **kwargs)
-        dens_trafo, trafo_part = up_scale.values, up_scale.row_splits
-        dens_m = tf.reshape(dens_trafo, (ks.backend.shape(dens_trafo)[0], self._units_out, self._units_in))
-        out = tf.RaggedTensor.from_row_splits(dens_m, trafo_part, validate=self.ragged_validate)
-        return out
-
-    def get_config(self):
-        """Update layer config."""
-        config = super(TrafoEdgeNetMessages, self).get_config()
-        config.update({"target_shape": self.target_shape})
-        config_dense = self.lay_dense.get_config()
-        for x in ["kernel_regularizer", "activity_regularizer", "bias_regularizer", "kernel_constraint",
-                  "bias_constraint", "kernel_initializer", "bias_initializer", "activation", "use_bias"]:
-            config.update({x: config_dense[x]})
-        return config
-
-
-@tf.keras.utils.register_keras_serializable(package='kgcnn', name='MatMulMessages')
-class MatMulMessages(GraphBaseLayer):
-    """Linear transformation of edges or messages, i.e. matrix multiplication.
-    The message dimension must be suitable for matrix multiplication. The actual matrix is not a trainable weight of
-    this layer but passed as input.
-    This was proposed by `NMPNN <http://arxiv.org/abs/1704.01212>`_ .
-
-    """
-
-    def __init__(self, **kwargs):
-        """Initialize layer."""
-        super(MatMulMessages, self).__init__(**kwargs)
-
-    def build(self, input_shape):
-        """Build layer."""
-        super(MatMulMessages, self).build(input_shape)
-
-    def call(self, inputs, **kwargs):
-        """Forward pass. Operates on values without checking splits of the ragged dimension.
-
-        Args:
-            inputs (list): [trafo_mat, edges]
-
-                - trafo_mat (tf.RaggedTensor): Transformation matrix for each message of shape (batch, [M], F', F).
-                - edges (tf.RaggedTensor): Edge embeddings or messages (batch, [M], F)
-            
-        Returns:
-            tf.RaggedTensor: Transformation of messages by matrix multiplication of shape (batch, [M], F')
-        """
-        self.assert_ragged_input_rank(inputs)
-        dens_trafo, trafo_part = inputs[0].values, inputs[0].row_splits
-        dens_e, epart = inputs[1].values, inputs[1].row_splits
-        out = tf.keras.backend.batch_dot(dens_trafo, dens_e)
-        out = tf.RaggedTensor.from_row_splits(out, epart, validate=self.ragged_validate)
-        return out
-
-    def get_config(self):
-        """Update layer config."""
-        config = super(MatMulMessages, self).get_config()
-        return config
+from kgcnn.layers.modules import Dense, LazyAdd
 
 
 @tf.keras.utils.register_keras_serializable(package='kgcnn', name='GRUUpdate')
 class GRUUpdate(GraphBaseLayer):
-    """Gated recurrent unit for updating embeddings. First proposed by `NMPNN <http://arxiv.org/abs/1704.01212>`_ .
+    r"""Gated recurrent unit for updating node or edge embeddings.
+    As proposed by `NMPNN <http://arxiv.org/abs/1704.01212>`__ .
 
-    Args:
-        units (int): Units for GRU.
-        activation: Activation function to use. Default: hyperbolic tangent
-            (`tanh`). If you pass None, no activation is applied
-            (ie. "linear" activation: `a(x) = x`).
-        recurrent_activation: Activation function to use for the recurrent step.
-            Default: sigmoid (`sigmoid`). If you pass `None`, no activation is
-            applied (ie. "linear" activation: `a(x) = x`).
-        use_bias: Boolean, (default `True`), whether the layer uses a bias vector.
-        kernel_initializer: Initializer for the `kernel` weights matrix,
-            used for the linear transformation of the inputs. Default:
-            `glorot_uniform`.
-        recurrent_initializer: Initializer for the `recurrent_kernel`
-            weights matrix, used for the linear transformation of the recurrent state.
-            Default: `orthogonal`.
-        bias_initializer: Initializer for the bias vector. Default: `zeros`.
-        kernel_regularizer: Regularizer function applied to the `kernel` weights
-            matrix. Default: `None`.
-        recurrent_regularizer: Regularizer function applied to the
-            `recurrent_kernel` weights matrix. Default: `None`.
-        bias_regularizer: Regularizer function applied to the bias vector. Default:
-            `None`.
-        kernel_constraint: Constraint function applied to the `kernel` weights
-            matrix. Default: `None`.
-        recurrent_constraint: Constraint function applied to the `recurrent_kernel`
-            weights matrix. Default: `None`.
-        bias_constraint: Constraint function applied to the bias vector. Default:
-            `None`.
-        dropout: Float between 0 and 1. Fraction of the units to drop for the
-            linear transformation of the inputs. Default: 0.
-        recurrent_dropout: Float between 0 and 1. Fraction of the units to drop for
-            the linear transformation of the recurrent state. Default: 0.
-        reset_after: GRU convention (whether to apply reset gate after or
-            before matrix multiplication). False = "before",
-            True = "after" (default and CuDNN compatible).
     """
 
     def __init__(self, units,
                  activation='tanh', recurrent_activation='sigmoid',
                  use_bias=True, kernel_initializer='glorot_uniform',
                  recurrent_initializer='orthogonal',
                  bias_initializer='zeros', kernel_regularizer=None,
                  recurrent_regularizer=None, bias_regularizer=None, kernel_constraint=None,
                  recurrent_constraint=None, bias_constraint=None, dropout=0.0,
                  recurrent_dropout=0.0, reset_after=True,
                  **kwargs):
-        """Initialize layer."""
+        r"""Initialize layer.
+
+        Args:
+            units (int): Units for GRU.
+            activation: Activation function to use. Default: hyperbolic tangent
+                (`tanh`). If you pass None, no activation is applied
+                (ie. "linear" activation: `a(x) = x`).
+            recurrent_activation: Activation function to use for the recurrent step.
+                Default: sigmoid (`sigmoid`). If you pass `None`, no activation is
+                applied (ie. "linear" activation: `a(x) = x`).
+            use_bias: Boolean, (default `True`), whether the layer uses a bias vector.
+            kernel_initializer: Initializer for the `kernel` weights matrix,
+                used for the linear transformation of the inputs. Default:
+                `glorot_uniform`.
+            recurrent_initializer: Initializer for the `recurrent_kernel`
+                weights matrix, used for the linear transformation of the recurrent state.
+                Default: `orthogonal`.
+            bias_initializer: Initializer for the bias vector. Default: `zeros`.
+            kernel_regularizer: Regularizer function applied to the `kernel` weights
+                matrix. Default: `None`.
+            recurrent_regularizer: Regularizer function applied to the
+                `recurrent_kernel` weights matrix. Default: `None`.
+            bias_regularizer: Regularizer function applied to the bias vector. Default:
+                `None`.
+            kernel_constraint: Constraint function applied to the `kernel` weights
+                matrix. Default: `None`.
+            recurrent_constraint: Constraint function applied to the `recurrent_kernel`
+                weights matrix. Default: `None`.
+            bias_constraint: Constraint function applied to the bias vector. Default:
+                `None`.
+            dropout: Float between 0 and 1. Fraction of the units to drop for the
+                linear transformation of the inputs. Default: 0.
+            recurrent_dropout: Float between 0 and 1. Fraction of the units to drop for
+                the linear transformation of the recurrent state. Default: 0.
+            reset_after: GRU convention (whether to apply reset gate after or
+                before matrix multiplication). False = "before",
+                True = "after" (default and CuDNN compatible).
+        """
         super(GRUUpdate, self).__init__(**kwargs)
         self.units = units
 
-        self.gru_cell = tf.keras.layers.GRUCell(units=units,
-                                                activation=activation, recurrent_activation=recurrent_activation,
-                                                use_bias=use_bias, kernel_initializer=kernel_initializer,
-                                                recurrent_initializer=recurrent_initializer,
-                                                bias_initializer=bias_initializer,
-                                                kernel_regularizer=kernel_regularizer,
-                                                recurrent_regularizer=recurrent_regularizer,
-                                                bias_regularizer=bias_regularizer,
-                                                kernel_constraint=kernel_constraint,
-                                                recurrent_constraint=recurrent_constraint,
-                                                bias_constraint=bias_constraint,
-                                                dropout=dropout,
-                                                recurrent_dropout=recurrent_dropout, reset_after=reset_after)
+        self.gru_cell = tf.keras.layers.GRUCell(
+            units=units,
+            activation=activation, recurrent_activation=recurrent_activation,
+            use_bias=use_bias, kernel_initializer=kernel_initializer,
+            recurrent_initializer=recurrent_initializer,
+            bias_initializer=bias_initializer,
+            kernel_regularizer=kernel_regularizer,
+            recurrent_regularizer=recurrent_regularizer,
+            bias_regularizer=bias_regularizer,
+            kernel_constraint=kernel_constraint,
+            recurrent_constraint=recurrent_constraint,
+            bias_constraint=bias_constraint,
+            dropout=dropout,
+            recurrent_dropout=recurrent_dropout, reset_after=reset_after
+        )
 
     def build(self, input_shape):
         """Build layer."""
         super(GRUUpdate, self).build(input_shape)
 
-    def call(self, inputs, **kwargs):
+    def call(self, inputs, mask=None, **kwargs):
         """Forward pass.
 
         Args:
             inputs (list): [nodes, updates]
 
                 - nodes (tf.RaggedTensor): Node embeddings of shape (batch, [N], F)
                 - updates (tf.RaggedTensor): Matching node updates of shape (batch, [N], F)
+            mask: Mask for inputs. Default is None.
 
         Returns:
            tf.RaggedTensor: Updated nodes of shape (batch, [N], F)
         """
-        self.assert_ragged_input_rank(inputs)
+        inputs = self.assert_ragged_input_rank(inputs, ragged_rank=1, mask=mask)
         n, npart = inputs[0].values, inputs[0].row_splits
         eu, _ = inputs[1].values, inputs[1].row_splits
         out, _ = self.gru_cell(eu, n, **kwargs)
         out = tf.RaggedTensor.from_row_splits(out, npart, validate=self.ragged_validate)
         return out
 
     def get_config(self):
@@ -208,7 +111,78 @@
                       "bias_initializer", "kernel_regularizer",
                       "recurrent_regularizer", "bias_regularizer", "kernel_constraint",
                       "recurrent_constraint", "bias_constraint", "dropout",
                       "recurrent_dropout", "reset_after"]
         for x in param_list:
             config.update({x: conf_cell[x]})
         return config
+
+
+@tf.keras.utils.register_keras_serializable(package='kgcnn', name='ResidualLayer')
+class ResidualLayer(GraphBaseLayer):
+    r"""Residual Layer as defined by `DimNetPP <https://arxiv.org/abs/2011.14115>`__ .
+
+    """
+
+    def __init__(self, units,
+                 use_bias=True,
+                 activation='kgcnn>swish',
+                 kernel_regularizer=None,
+                 bias_regularizer=None,
+                 activity_regularizer=None,
+                 kernel_constraint=None,
+                 bias_constraint=None,
+                 kernel_initializer='glorot_uniform',
+                 bias_initializer='zeros',
+                 **kwargs):
+        """Initialize layer.
+
+        Args:
+            units: Dimension of the kernel.
+            use_bias (bool, optional): Use bias. Defaults to True.
+            activation (str): Activation function. Default is "kgcnn>swish".
+            kernel_regularizer: Kernel regularization. Default is None.
+            bias_regularizer: Bias regularization. Default is None.
+            activity_regularizer: Activity regularization. Default is None.
+            kernel_constraint: Kernel constrains. Default is None.
+            bias_constraint: Bias constrains. Default is None.
+            kernel_initializer: Initializer for kernels. Default is 'glorot_uniform'.
+            bias_initializer: Initializer for bias. Default is 'zeros'.
+        """
+        super(ResidualLayer, self).__init__(**kwargs)
+        dense_args = {
+            "units": units, "activation": activation, "use_bias": use_bias,
+            "kernel_regularizer": kernel_regularizer, "activity_regularizer": activity_regularizer,
+            "bias_regularizer": bias_regularizer, "kernel_constraint": kernel_constraint,
+            "bias_constraint": bias_constraint, "kernel_initializer": kernel_initializer,
+            "bias_initializer": bias_initializer
+        }
+
+        self.dense_1 = Dense(**dense_args)
+        self.dense_2 = Dense(**dense_args)
+        self.add_end = LazyAdd()
+
+    def build(self, input_shape):
+        """Build layer."""
+        super(ResidualLayer, self).build(input_shape)
+
+    def call(self, inputs, **kwargs):
+        """Forward pass.
+
+        Args:
+            inputs (tf.RaggedTensor): Node or edge embedding of shape (batch, [N], F)
+
+        Returns:
+            tf.RaggedTensor: Node or edge embedding of shape (batch, [N], F)
+        """
+        x = self.dense_1(inputs, **kwargs)
+        x = self.dense_2(x, **kwargs)
+        x = self.add_end([inputs, x], **kwargs)
+        return x
+
+    def get_config(self):
+        config = super(ResidualLayer, self).get_config()
+        conf_dense = self.dense_1.get_config()
+        for x in ["kernel_regularizer", "activity_regularizer", "bias_regularizer", "kernel_constraint",
+                  "bias_constraint", "kernel_initializer", "bias_initializer", "activation", "use_bias", "units"]:
+            config.update({x: conf_dense[x]})
+        return config
```

### Comparing `kgcnn-2.2.4/kgcnn/layers/conv/mxmnet_conv.py` & `kgcnn-3.0.0/kgcnn/literature/MXMNet/_mxmnet_conv.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import tensorflow as tf
 from kgcnn.layers.base import GraphBaseLayer
 from kgcnn.layers.mlp import GraphMLP
 from kgcnn.layers.modules import LazyAdd, Dense, LazyConcatenate, LazyMultiply
-from kgcnn.layers.conv.dimenet_conv import ResidualLayer
+from kgcnn.layers.update import ResidualLayer
 from kgcnn.layers.gather import GatherEmbeddingSelection, GatherNodesOutgoing
 from kgcnn.layers.pooling import PoolingLocalMessages
 ks = tf.keras
 
 
 @ks.utils.register_keras_serializable(package='kgcnn', name='MXMGlobalMP')
 class MXMGlobalMP(GraphBaseLayer):
```

### Comparing `kgcnn-2.2.4/kgcnn/layers/conv/painn_conv.py` & `kgcnn-3.0.0/kgcnn/literature/PAiNN/_painn_conv.py`

 * *Files identical despite different names*

### Comparing `kgcnn-2.2.4/kgcnn/layers/conv/sage_conv.py` & `kgcnn-3.0.0/kgcnn/layers/conv.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import tensorflow as tf
 
 from kgcnn.layers.base import GraphBaseLayer
-from kgcnn.layers.modules import LazyConcatenate
+from kgcnn.layers.modules import LazyConcatenate, Dense, Activation
 from kgcnn.layers.norm import GraphLayerNormalization
 from kgcnn.layers.mlp import GraphMLP
 from kgcnn.layers.gather import GatherNodesOutgoing, GatherNodes
-from kgcnn.layers.pooling import PoolingLocalMessages, PoolingLocalEdgesLSTM
+from kgcnn.layers.pooling import PoolingLocalMessages, PoolingLocalEdgesLSTM, PoolingWeightedLocalEdges
 
 
 @tf.keras.utils.register_keras_serializable(package='kgcnn', name='GraphSageNodeLayer')
 class GraphSageNodeLayer(GraphBaseLayer):
-    r"""This is a convolutional layer for `GraphSAGE <http://arxiv.org/abs/1706.02216>`_  model as proposed
+    r"""This is a convolutional layer for `GraphSAGE <http://arxiv.org/abs/1706.02216>`__  model as proposed
     by Hamilton et al. (2018). It is not used in the :obj:``kgcnn.literature.GraphSAGE`` model implementation
     but meant as a simplified module for other networks.
 
     Args:
         units: Dimensionality of embedding for each layer in the MLP.
         use_edge_features: Whether to use edge-features in addition to node features for convolution. Default is False.
         pooling_method: Pooling method to apply to node attributes. Default is "sum".
@@ -111,15 +111,15 @@
                   "bias_constraint", "kernel_initializer", "bias_initializer", "use_bias", "activation"]:
             config.update({x: conf_mlp[x]})
         return config
 
 
 @tf.keras.utils.register_keras_serializable(package='kgcnn', name='GraphSageEdgeUpdateLayer')
 class GraphSageEdgeUpdateLayer(GraphBaseLayer):
-    r"""An extension for `GraphSAGE <http://arxiv.org/abs/1706.02216>`_ model to have edge updates.
+    r"""An extension for `GraphSAGE <http://arxiv.org/abs/1706.02216>`__ model to have edge updates.
 
     It is a direct extension and should fit the GraphSAGE idea of message passing.
 
     Args:
         units: Dimensionality of embedding for each layer in the MLP.
         use_normalization: Whether to use GraphLayerNormalization at the output of the update. Default is True.
         activation: Activation function to use. Default is "relu".
@@ -191,7 +191,108 @@
         config = super(GraphSageEdgeUpdateLayer, self).get_config()
         config.update({"units": self.units, "use_normalization": self.use_normalization})
         conf_mlp = self.update_edge_mlp.get_config()
         for x in ["kernel_regularizer", "activity_regularizer", "bias_regularizer", "kernel_constraint",
                   "bias_constraint", "kernel_initializer", "bias_initializer", "use_bias", "activation"]:
             config.update({x: conf_mlp[x]})
         return config
+
+
+@tf.keras.utils.register_keras_serializable(package='kgcnn', name='GCN')
+class GCN(GraphBaseLayer):
+    r"""Graph convolution according to `Kipf et al <https://arxiv.org/abs/1609.02907>`__ .
+
+    Computes graph convolution as :math:`\sigma(A_s(WX+b))` where :math:`A_s` is the precomputed and scaled adjacency
+    matrix. The scaled adjacency matrix is defined by :math:`A_s = D^{-0.5} (A + I) D^{-0.5}` with the degree
+    matrix :math:`D` . In place of :math:`A_s` , this layers uses edge features (that are the entries of :math:`A_s` )
+    and edge indices.
+    :math:`A_s` is considered pre-scaled, this is not done by this layer!
+    If no scaled edge features are available, you could consider use e.g. "segment_mean",
+    or :obj:`normalize_by_weights` to obtain a similar behaviour that is expected b
+    y a pre-scaled adjacency matrix input.
+
+    Edge features must be possible to broadcast to node features, since they are multiplied with the node features.
+    Ideally they are weights of shape `(..., 1)` for broadcasting, e.g. entries of :math:`A_s` .
+
+    Args:
+        units (int): Output dimension/ units of dense layer.
+        pooling_method (str): Pooling method for summing edges. Default is 'segment_sum'.
+        normalize_by_weights (bool): Normalize the pooled output by the sum of weights. Default is False.
+            In this case the edge features are considered weights of dimension (...,1) and are summed for each node.
+        activation (str): Activation. Default is {"class_name": "kgcnn>leaky_relu", "config": {"alpha": 0.2}}.
+        use_bias (bool): Use bias. Default is True.
+        kernel_regularizer: Kernel regularization. Default is None.
+        bias_regularizer: Bias regularization. Default is None.
+        activity_regularizer: Activity regularization. Default is None.
+        kernel_constraint: Kernel constrains. Default is None.
+        bias_constraint: Bias constrains. Default is None.
+        kernel_initializer: Initializer for kernels. Default is 'glorot_uniform'.
+        bias_initializer: Initializer for bias. Default is 'zeros'.
+    """
+
+    def __init__(self,
+                 units,
+                 pooling_method='sum',
+                 normalize_by_weights=False,
+                 activation='kgcnn>leaky_relu',
+                 use_bias=True,
+                 kernel_regularizer=None,
+                 bias_regularizer=None,
+                 activity_regularizer=None,
+                 kernel_constraint=None,
+                 bias_constraint=None,
+                 kernel_initializer='glorot_uniform',
+                 bias_initializer='zeros',
+                 **kwargs):
+        """Initialize layer."""
+        super(GCN, self).__init__(**kwargs)
+        self.normalize_by_weights = normalize_by_weights
+        self.pooling_method = pooling_method
+        self.units = units
+        kernel_args = {"kernel_regularizer": kernel_regularizer, "activity_regularizer": activity_regularizer,
+                       "bias_regularizer": bias_regularizer, "kernel_constraint": kernel_constraint,
+                       "bias_constraint": bias_constraint, "kernel_initializer": kernel_initializer,
+                       "bias_initializer": bias_initializer, "use_bias": use_bias}
+        pool_args = {"pooling_method": pooling_method, "normalize_by_weights": normalize_by_weights}
+
+        # Layers
+        self.lay_gather = GatherNodesOutgoing()
+        self.lay_dense = Dense(units=self.units, activation='linear', **kernel_args)
+        self.lay_pool = PoolingWeightedLocalEdges(**pool_args)
+        self.lay_act = Activation(activation)
+
+    def build(self, input_shape):
+        """Build layer."""
+        super(GCN, self).build(input_shape)
+
+    def call(self, inputs, **kwargs):
+        """Forward pass.
+
+        Args:
+            inputs: [nodes, edges, edge_index]
+
+                - nodes (tf.RaggedTensor): Node embeddings of shape (batch, [N], F)
+                - edges (tf.RaggedTensor): Edge or message embeddings of shape (batch, [M], F)
+                - edge_index (tf.RaggedTensor): Edge indices referring to nodes of shape (batch, [M], 2)
+
+        Returns:
+            tf.RaggedTensor: Node embeddings of shape (batch, [N], F)
+        """
+        node, edges, edge_index = inputs
+        no = self.lay_dense(node, **kwargs)
+        no = self.lay_gather([no, edge_index], **kwargs)
+        nu = self.lay_pool([node, no, edge_index, edges], **kwargs)  # Summing for each node connection
+        out = self.lay_act(nu, **kwargs)
+        return out
+
+    def get_config(self):
+        """Update config."""
+        config = super(GCN, self).get_config()
+        config.update({"normalize_by_weights": self.normalize_by_weights,
+                       "pooling_method": self.pooling_method, "units": self.units})
+        conf_dense = self.lay_dense.get_config()
+        for x in ["kernel_regularizer", "activity_regularizer", "bias_regularizer", "kernel_constraint",
+                  "bias_constraint", "kernel_initializer", "bias_initializer", "use_bias"]:
+            config.update({x: conf_dense[x]})
+        conf_act = self.lay_act.get_config()
+        config.update({"activation": conf_act["activation"]})
+        return config
```

### Comparing `kgcnn-2.2.4/kgcnn/layers/conv/schnet_conv.py` & `kgcnn-3.0.0/kgcnn/literature/Schnet/_schnet_conv.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from kgcnn.layers.modules import LazyMultiply, Dense, LazyAdd
 from kgcnn.layers.pooling import PoolingLocalEdges
 from kgcnn.layers.gather import GatherNodesOutgoing
 
 
 @tf.keras.utils.register_keras_serializable(package='kgcnn', name='SchNetCFconv')
 class SchNetCFconv(GraphBaseLayer):
-    r"""Continuous filter convolution of `SchNet <https://aip.scitation.org/doi/pdf/10.1063/1.5019779>`_ .
+    r"""Continuous filter convolution of `SchNet <https://aip.scitation.org/doi/pdf/10.1063/1.5019779>`__ .
 
     Edges are processed by 2 :obj:`Dense` layers, multiplied on outgoing node features and pooled for receiving node.
 
     Args:
         units (int): Units for Dense layer.
         cfconv_pool (str): Pooling method. Default is 'segment_sum'.
         use_bias (bool): Use bias. Default is True.
```

### Comparing `kgcnn-2.2.4/kgcnn/layers/conv/wacsf_conv.py` & `kgcnn-3.0.0/kgcnn/literature/HDNNP2nd/_wacsf_conv.py`

 * *Files identical despite different names*

### Comparing `kgcnn-2.2.4/kgcnn/layers/gather.py` & `kgcnn-3.0.0/kgcnn/layers/gather.py`

 * *Files 3% similar despite different names*

```diff
@@ -376,7 +376,49 @@
         out = tf.RaggedTensor.from_row_lengths(out, target_len, validate=self.ragged_validate)
         return out
 
     def get_config(self):
         """Update layer config."""
         config = super(GatherState, self).get_config()
         return config
+
+
+@tf.keras.utils.register_keras_serializable(package='kgcnn', name='GatherEdgesPairs')
+class GatherEdgesPairs(GraphBaseLayer):
+    """Gather edge pairs that also works for invalid indices given a certain pair, i.e. if an edge does not have its
+    reverse counterpart in the edge indices list.
+
+    This class is used in `DMPNN <https://pubs.acs.org/doi/full/10.1021/acs.jcim.9b00237>`__ .
+
+    """
+
+    def __init__(self, **kwargs):
+        """Initialize layer."""
+        super(GatherEdgesPairs, self).__init__(**kwargs)
+        self.gather_layer = GatherNodesIngoing()
+
+    def build(self, input_shape):
+        """Build layer."""
+        super(GatherEdgesPairs, self).build(input_shape)
+
+    def call(self, inputs, **kwargs):
+        """Forward pass.
+
+        Args:
+            inputs (list): [edges, pair_index]
+
+                - edges (tf.RaggedTensor): Node embeddings of shape (batch, [M], F)
+                - pair_index (tf.RaggedTensor): Edge indices referring to edges of shape (batch, [M], 1)
+
+        Returns:
+            list: Gathered edge embeddings that match the reverse edges of shape (batch, [M], F) for selection_index.
+        """
+        self.assert_ragged_input_rank(inputs)
+        edges, pair_index = inputs
+        index_corrected = tf.RaggedTensor.from_row_splits(
+            tf.where(pair_index.values >= 0, pair_index.values, tf.zeros_like(pair_index.values)),
+            pair_index.row_splits, validate=self.ragged_validate)
+        edges_paired = self.gather_layer([edges, index_corrected], **kwargs)
+        edges_corrected = tf.RaggedTensor.from_row_splits(
+            tf.where(pair_index.values >= 0, edges_paired.values, tf.zeros_like(edges_paired.values)),
+            edges_paired.row_splits, validate=self.ragged_validate)
+        return edges_corrected
```

### Comparing `kgcnn-2.2.4/kgcnn/layers/geom.py` & `kgcnn-3.0.0/kgcnn/layers/geom.py`

 * *Files identical despite different names*

### Comparing `kgcnn-2.2.4/kgcnn/layers/mlp.py` & `kgcnn-3.0.0/kgcnn/layers/mlp.py`

 * *Files identical despite different names*

### Comparing `kgcnn-2.2.4/kgcnn/layers/modules.py` & `kgcnn-3.0.0/kgcnn/layers/modules.py`

 * *Files identical despite different names*

### Comparing `kgcnn-2.2.4/kgcnn/layers/norm.py` & `kgcnn-3.0.0/kgcnn/layers/norm.py`

 * *Files identical despite different names*

### Comparing `kgcnn-2.2.4/kgcnn/layers/pool/set2set.py` & `kgcnn-3.0.0/kgcnn/layers/set2set.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,86 +1,27 @@
 import tensorflow as tf
-import tensorflow.keras as ks
-import tensorflow.keras.backend as ksb
-
 from kgcnn.layers.base import GraphBaseLayer
 
+ks = tf.keras
+ksb = tf.keras.backend
+
+
 # Order Matters: Sequence to sequence for sets
 # by Vinyals et al. 2016
 # https://arxiv.org/abs/1511.06391
 
 
-@tf.keras.utils.register_keras_serializable(package='kgcnn', name='PoolingSet2Set')
-class PoolingSet2Set(GraphBaseLayer):
-    """Pooling Node or edge embeddings by the Set2Set encoder part from layer.
-    This was first proposed by `NMPNN <http://arxiv.org/abs/1704.01212>`_ .
+@tf.keras.utils.register_keras_serializable(package='kgcnn', name='PoolingSet2SetEncoder')
+class PoolingSet2SetEncoder(GraphBaseLayer):
+    r"""Pooling Node or edge embeddings by the Set2Set encoder part from layer.
+
+    This was first proposed by `NMPNN <http://arxiv.org/abs/1704.01212>`__ .
     The Reading to Memory has to be handled separately.
     Uses a keras LSTM layer for the updates.
-    
-    Args:
-        channels (int): Number of channels for the LSTM update.
-        T (int): Numer of iterations. Default is T=3.
-        pooling_method : Pooling method for PoolingSet2Set. Default is 'mean'.
-        init_qstar: How to generate the first q_star vector. Default is 'mean'.
-        activation: Activation function to use.
-            Default: hyperbolic tangent (`tanh`). If you pass `None`, no activation
-            is applied (ie. "linear" activation: `a(x) = x`).
-        recurrent_activation: Activation function to use for the recurrent step.
-            Default: sigmoid (`sigmoid`). If you pass `None`, no activation is
-            applied (ie. "linear" activation: `a(x) = x`).
-        use_bias: Boolean (default `True`), whether the layer uses a bias vector.
-        kernel_initializer: Initializer for the `kernel` weights matrix, used for
-            the linear transformation of the inputs. Default: `glorot_uniform`.
-            recurrent_initializer: Initializer for the `recurrent_kernel` weights
-            matrix, used for the linear transformation of the recurrent state.
-            Default: `orthogonal`.
-        bias_initializer: Initializer for the bias vector. Default: `zeros`.
-            unit_forget_bias: Boolean (default `True`). If True, add 1 to the bias of
-            the forget gate at initialization. Setting it to true will also force
-            `bias_initializer="zeros"`. This is recommended in [Jozefowicz et
-            al.](http://www.jmlr.org/proceedings/papers/v37/jozefowicz15.pdf).
-        kernel_regularizer: Regularizer function applied to the `kernel` weights
-            matrix. Default: `None`.
-        recurrent_regularizer: Regularizer function applied to the
-            `recurrent_kernel` weights matrix. Default: `None`.
-            bias_regularizer: Regularizer function applied to the bias vector. Default:
-            `None`.
-        activity_regularizer: Regularizer function applied to the output of the
-            layer (its "activation"). Default: `None`.
-        kernel_constraint: Constraint function applied to the `kernel` weights
-            matrix. Default: `None`.
-        recurrent_constraint: Constraint function applied to the `recurrent_kernel`
-            weights matrix. Default: `None`.
-        bias_constraint: Constraint function applied to the bias vector. Default:
-            `None`.
-        dropout: Float between 0 and 1. Fraction of the units to drop for the linear
-            transformation of the inputs. Default: 0.
-            recurrent_dropout: Float between 0 and 1. Fraction of the units to drop for
-            the linear transformation of the recurrent state. Default: 0.
-        return_sequences: Boolean. Whether to return the last output. in the output
-            sequence, or the full sequence. Default: `False`.
-        return_state: Boolean. Whether to return the last state in addition to the
-            output. Default: `False`.
-        go_backwards: Boolean (default `False`). If True, process the input sequence
-            backwards and return the reversed sequence.
-        stateful: Boolean (default `False`). If True, the last state for each sample
-            at index i in a batch will be used as initial state for the sample of
-            index i in the following batch.
-        time_major: The shape format of the `inputs` and `outputs` tensors.
-            If True, the inputs and outputs will be in shape
-            `[timesteps, batch, feature]`, whereas in the False case, it will be
-            `[batch, timesteps, feature]`. Using `time_major = True` is a bit more
-            efficient because it avoids transposes at the beginning and end of the
-            RNN calculation. However, most TensorFlow data is batch-major, so by
-            default this function accepts input and emits output in batch-major
-            form.
-        unroll: Boolean (default `False`). If True, the network will be unrolled,
-            else a symbolic loop will be used. Unrolling can speed-up a RNN, although
-            it tends to be more memory-intensive. Unrolling is only suitable for short
-            sequences.
+
     """
 
     def __init__(self,
                  # Args
                  channels,
                  T=3,
                  pooling_method='mean',
@@ -106,16 +47,79 @@
                  return_sequences=False,  # Should not be changed here
                  return_state=False,  # Should not be changed here
                  go_backwards=False,  # Should not be changed here
                  stateful=False,
                  time_major=False,
                  unroll=False,
                  **kwargs):
-        """Init layer."""
-        super(PoolingSet2Set, self).__init__(**kwargs)
+        """Init layer.
+
+        Args:
+            channels (int): Number of channels for the LSTM update.
+            T (int): Numer of iterations. Default is T=3.
+            pooling_method : Pooling method for PoolingSet2SetEncoder. Default is 'mean'.
+            init_qstar: How to generate the first q_star vector. Default is 'mean'.
+            activation: Activation function to use.
+                Default: hyperbolic tangent (`tanh`). If you pass `None`, no activation
+                is applied (ie. "linear" activation: `a(x) = x`).
+            recurrent_activation: Activation function to use for the recurrent step.
+                Default: sigmoid (`sigmoid`). If you pass `None`, no activation is
+                applied (ie. "linear" activation: `a(x) = x`).
+            use_bias: Boolean (default `True`), whether the layer uses a bias vector.
+            kernel_initializer: Initializer for the `kernel` weights matrix, used for
+                the linear transformation of the inputs. Default: `glorot_uniform`.
+                recurrent_initializer: Initializer for the `recurrent_kernel` weights
+                matrix, used for the linear transformation of the recurrent state.
+                Default: `orthogonal`.
+            bias_initializer: Initializer for the bias vector. Default: `zeros`.
+                unit_forget_bias: Boolean (default `True`). If True, add 1 to the bias of
+                the forget gate at initialization. Setting it to true will also force
+                `bias_initializer="zeros"`. This is recommended in [Jozefowicz et
+                al.](http://www.jmlr.org/proceedings/papers/v37/jozefowicz15.pdf).
+            kernel_regularizer: Regularizer function applied to the `kernel` weights
+                matrix. Default: `None`.
+            recurrent_regularizer: Regularizer function applied to the
+                `recurrent_kernel` weights matrix. Default: `None`.
+                bias_regularizer: Regularizer function applied to the bias vector. Default:
+                `None`.
+            activity_regularizer: Regularizer function applied to the output of the
+                layer (its "activation"). Default: `None`.
+            kernel_constraint: Constraint function applied to the `kernel` weights
+                matrix. Default: `None`.
+            recurrent_constraint: Constraint function applied to the `recurrent_kernel`
+                weights matrix. Default: `None`.
+            bias_constraint: Constraint function applied to the bias vector. Default:
+                `None`.
+            dropout: Float between 0 and 1. Fraction of the units to drop for the linear
+                transformation of the inputs. Default: 0.
+                recurrent_dropout: Float between 0 and 1. Fraction of the units to drop for
+                the linear transformation of the recurrent state. Default: 0.
+            return_sequences: Boolean. Whether to return the last output. in the output
+                sequence, or the full sequence. Default: `False`.
+            return_state: Boolean. Whether to return the last state in addition to the
+                output. Default: `False`.
+            go_backwards: Boolean (default `False`). If True, process the input sequence
+                backwards and return the reversed sequence.
+            stateful: Boolean (default `False`). If True, the last state for each sample
+                at index i in a batch will be used as initial state for the sample of
+                index i in the following batch.
+            time_major: The shape format of the `inputs` and `outputs` tensors.
+                If True, the inputs and outputs will be in shape
+                `[timesteps, batch, feature]`, whereas in the False case, it will be
+                `[batch, timesteps, feature]`. Using `time_major = True` is a bit more
+                efficient because it avoids transposes at the beginning and end of the
+                RNN calculation. However, most TensorFlow data is batch-major, so by
+                default this function accepts input and emits output in batch-major
+                form.
+            unroll: Boolean (default `False`). If True, the network will be unrolled,
+                else a symbolic loop will be used. Unrolling can speed-up a RNN, although
+                it tends to be more memory-intensive. Unrolling is only suitable for short
+                sequences.
+        """
+        super(PoolingSet2SetEncoder, self).__init__(**kwargs)
         # Number of Channels to use in LSTM
         self.channels = channels
         self.T = T  # Number of Iterations to work on memory
         self.pooling_method = pooling_method
         self.init_qstar = init_qstar
 
         if self.pooling_method == 'mean':
@@ -128,43 +132,44 @@
         if self.init_qstar == 'mean':
             self.qstar0 = self.init_qstar_mean
         else:
             self.qstar0 = self.init_qstar_0
         # ...
 
         # LSTM Layer to run on m
-        self.lay_lstm = ks.layers.LSTM(channels,
-                                       activation=activation,
-                                       recurrent_activation=recurrent_activation,
-                                       use_bias=use_bias,
-                                       kernel_initializer=kernel_initializer,
-                                       recurrent_initializer=recurrent_initializer,
-                                       bias_initializer=bias_initializer,
-                                       unit_forget_bias=unit_forget_bias,
-                                       kernel_regularizer=kernel_regularizer,
-                                       recurrent_regularizer=recurrent_regularizer,
-                                       bias_regularizer=bias_regularizer,
-                                       activity_regularizer=activity_regularizer,
-                                       kernel_constraint=kernel_constraint,
-                                       recurrent_constraint=recurrent_constraint,
-                                       bias_constraint=bias_constraint,
-                                       dropout=dropout,
-                                       recurrent_dropout=recurrent_dropout,
-                                       implementation=implementation,
-                                       return_sequences=return_sequences,
-                                       return_state=return_state,
-                                       go_backwards=go_backwards,
-                                       stateful=stateful,
-                                       time_major=time_major,
-                                       unroll=unroll
-                                       )
+        self.lay_lstm = ks.layers.LSTM(
+            channels,
+            activation=activation,
+            recurrent_activation=recurrent_activation,
+            use_bias=use_bias,
+            kernel_initializer=kernel_initializer,
+            recurrent_initializer=recurrent_initializer,
+            bias_initializer=bias_initializer,
+            unit_forget_bias=unit_forget_bias,
+            kernel_regularizer=kernel_regularizer,
+            recurrent_regularizer=recurrent_regularizer,
+            bias_regularizer=bias_regularizer,
+            activity_regularizer=activity_regularizer,
+            kernel_constraint=kernel_constraint,
+            recurrent_constraint=recurrent_constraint,
+            bias_constraint=bias_constraint,
+            dropout=dropout,
+            recurrent_dropout=recurrent_dropout,
+            implementation=implementation,
+            return_sequences=return_sequences,
+            return_state=return_state,
+            go_backwards=go_backwards,
+            stateful=stateful,
+            time_major=time_major,
+            unroll=unroll
+        )
 
     def build(self, input_shape):
         """Build layer."""
-        super(PoolingSet2Set, self).build(input_shape)
+        super(PoolingSet2SetEncoder, self).build(input_shape)
 
     def call(self, inputs, **kwargs):
         """Forward pass.
 
         Args:
             inputs: nodes
 
@@ -258,15 +263,15 @@
         # [q0,r0]
         qstar = ksb.concatenate([q, rt], axis=1)  # (batch,2*feat)
         qstar = ksb.expand_dims(qstar, axis=1)  # (batch,1,2*feat)
         return qstar
 
     def get_config(self):
         """Make config for layer."""
-        config = super(PoolingSet2Set, self).get_config()
+        config = super(PoolingSet2SetEncoder, self).get_config()
         config.update({"channels": self.channels, "T": self.T, "pooling_method": self.pooling_method,
                        "init_qstar": self.init_qstar})
         lstm_conf = self.lay_lstm.get_config()
         lstm_param = ["activation",
                       "recurrent_activation",
                       "use_bias",
                       "kernel_initializer",
```

### Comparing `kgcnn-2.2.4/kgcnn/layers/pool/topk.py` & `kgcnn-3.0.0/kgcnn/literature/Unet/_topk.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import tensorflow as tf
-import tensorflow.keras as ks
-
 from kgcnn.ops.partition import change_partition_by_name, partition_row_indexing
 from kgcnn.layers.base import GraphBaseLayer
 
+ks = tf.keras
+
 
 @tf.keras.utils.register_keras_serializable(package='kgcnn',name='PoolingTopK')
 class PoolingTopK(GraphBaseLayer):
     """Layer for pooling of nodes. Disjoint representation including length tensor.
     
     This implements a learnable score vector plus gate. Implements gPool of Gao et al.
```

### Comparing `kgcnn-2.2.4/kgcnn/layers/pooling.py` & `kgcnn-3.0.0/kgcnn/layers/pooling.py`

 * *Files 0% similar despite different names*

```diff
@@ -494,15 +494,15 @@
                       "bias_constraint", "dropout", "recurrent_dropout", "implementation", "return_sequences",
                       "return_state", "go_backwards", "stateful", "time_major", "unroll"]
         for x in lstm_param:
             config.update({x: conf_lstm[x]})
         return config
 
 
-PoolingLocalMessagesLSTM = PoolingLocalEdgesLSTM  # For now they are synonyms
+PoolingLocalMessagesLSTM = PoolingLocalEdgesLSTM  # For now, they are synonyms
 
 
 @ks.utils.register_keras_serializable(package='kgcnn', name='PoolingLocalEdgesAttention')
 class PoolingLocalEdgesAttention(GraphBaseLayer):
     r"""Pooling or aggregation of all edges or edge-like features per node,
     corresponding to node assigned by edge indices.
     Uses attention for pooling. i.e. :math:`n_i =  \sum_j \alpha_{ij} e_{ij}`
```

### Comparing `kgcnn-2.2.4/kgcnn/layers/relational.py` & `kgcnn-3.0.0/kgcnn/layers/relational.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,14 +162,15 @@
                 initializer=self.kernel_initializer,
                 regularizer=self.kernel_regularizer,
                 constraint=self.kernel_constraint,
                 dtype=self.dtype, trainable=True,
             )
         else:
             self.lin_bases = None
+
         if self.use_bias:
             self.bias = self.add_weight(
                 "bias",
                 shape=[self.units, ],
                 initializer=self.bias_initializer,
                 regularizer=self.bias_regularizer,
                 constraint=self.bias_constraint,
```

### Comparing `kgcnn-2.2.4/kgcnn/literature/AttentiveFP.py` & `kgcnn-3.0.0/kgcnn/literature/AttentiveFP/_make.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import tensorflow as tf
 from kgcnn.layers.casting import ChangeTensorType
-from kgcnn.layers.conv.attentivefp_conv import AttentiveHeadFP, PoolingNodesAttentive
-from kgcnn.layers.conv.mpnn_conv import GRUUpdate
+from ._attentivefp_conv import AttentiveHeadFP, PoolingNodesAttentive
+from kgcnn.layers.update import GRUUpdate
 from kgcnn.layers.modules import Dense, Dropout, OptionalInputEmbedding
 from kgcnn.layers.mlp import GraphMLP, MLP
 from kgcnn.model.utils import update_model_kwargs
 
-# import tensorflow.keras as ks
-ks = tf.keras
-
 # Keep track of model version from commit date in literature.
 # To be updated if model is changed in a significant way.
 __model_version__ = "2022.11.25"
 
+# import tensorflow.keras as ks
+ks = tf.keras
+
 # Implementation of AttentiveFP in `tf.keras` from paper:
 # Pushing the Boundaries of Molecular Representation for Drug Discovery with the Graph Attention Mechanism
 # Zhaoping Xiong, Dingyan Wang, Xiaohong Liu, Feisheng Zhong, Xiaozhe Wan, Xutong Li, Zhaojun Li,
 # Xiaomin Luo, Kaixian Chen, Hualiang Jiang*, and Mingyue Zheng*
 # Cite this: J. Med. Chem. 2020, 63, 16, 8749–8760
 # Publication Date:August 13, 2019
 # https://doi.org/10.1021/acs.jmedchem.9b00959
```

### Comparing `kgcnn-2.2.4/kgcnn/literature/CGCNN.py` & `kgcnn-3.0.0/kgcnn/literature/CGCNN/_make.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import tensorflow as tf
-from kgcnn.layers.conv.cgcnn_conv import CGCNNLayer
+from ._cgcnn_conv import CGCNNLayer
 from kgcnn.layers.geom import DisplacementVectorsASU, DisplacementVectorsUnitCell, FracToRealCoordinates, \
     EuclideanNorm, GaussBasisLayer, NodePosition
 from kgcnn.layers.pooling import PoolingNodes, PoolingWeightedNodes
 from kgcnn.layers.modules import OptionalInputEmbedding, LazySubtract, Dense
 from kgcnn.layers.mlp import MLP
 from kgcnn.model.utils import update_model_kwargs
```

### Comparing `kgcnn-2.2.4/kgcnn/literature/CMPNN.py` & `kgcnn-3.0.0/kgcnn/literature/CMPNN/_make.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import tensorflow as tf
 from typing import Union
 from kgcnn.layers.casting import ChangeTensorType
-from kgcnn.layers.gather import GatherNodesOutgoing
+from kgcnn.layers.gather import GatherNodesOutgoing, GatherEdgesPairs
 from kgcnn.layers.modules import Dense, LazyConcatenate, Activation, LazyAdd, Dropout, \
     OptionalInputEmbedding, LazySubtract, LazyMultiply
 from kgcnn.layers.mlp import GraphMLP, MLP
 from kgcnn.layers.pooling import PoolingLocalEdges, PoolingNodes
-from kgcnn.layers.conv.dmpnn_conv import DMPNNGatherEdgesPairs
 from kgcnn.model.utils import update_model_kwargs
 
 ks = tf.keras
 
 # Keep track of model version from commit date in literature.
 # To be updated if model is changed in a significant way.
 __model_version__ = "2022.11.25"
@@ -132,15 +131,15 @@
         m_max = PoolingLocalEdges(pooling_method="segment_max")([h, he, edi])
         m = LazyMultiply()([m_pool, m_max])
         # In paper there is a potential COMMUNICATE() here but in reference code just add() operation.
         h = LazyAdd()([h, m])
 
         # Edge message/update
         h_out = GatherNodesOutgoing()([h, edi])
-        e_rev = DMPNNGatherEdgesPairs()([he, ed_pairs])
+        e_rev = GatherEdgesPairs()([he, ed_pairs])
         he = LazySubtract()([h_out, e_rev])
         he = Dense(**edge_dense)(he)
         he = LazyAdd()([he, he0])
         he = Activation(**edge_activation)(he)
         if dropout:
             he = Dropout(**dropout)(he)
```

### Comparing `kgcnn-2.2.4/kgcnn/literature/DMPNN.py` & `kgcnn-3.0.0/kgcnn/literature/DMPNN/_make.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import tensorflow as tf
 from kgcnn.layers.casting import ChangeTensorType
 from kgcnn.layers.gather import GatherNodesOutgoing, GatherState
 from kgcnn.layers.modules import Dense, LazyConcatenate, Activation, LazyAdd, Dropout, \
     OptionalInputEmbedding
 from kgcnn.layers.mlp import GraphMLP, MLP
 from kgcnn.layers.pooling import PoolingLocalEdges, PoolingNodes
-from kgcnn.layers.conv.dmpnn_conv import DMPNNPPoolingEdgesDirected
+from ._dmpnn_conv import DMPNNPPoolingEdgesDirected
 from kgcnn.model.utils import update_model_kwargs
 
 ks = tf.keras
 
 # Keep track of model version from commit date in literature.
 # To be updated if model is changed in a significant way.
 __model_version__ = "2022.11.25"
```

### Comparing `kgcnn-2.2.4/kgcnn/literature/DimeNetPP.py` & `kgcnn-3.0.0/kgcnn/literature/DimeNetPP/_make.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import tensorflow as tf
-from kgcnn.layers.conv.dimenet_conv import DimNetInteractionPPBlock, DimNetOutputBlock, EmbeddingDimeBlock, \
-    SphericalBasisLayer
+from ._dimenet_conv import DimNetInteractionPPBlock, DimNetOutputBlock, EmbeddingDimeBlock, SphericalBasisLayer
 from kgcnn.layers.gather import GatherNodes
 from kgcnn.layers.geom import NodeDistanceEuclidean, EdgeAngle, BesselBasisLayer, NodePosition, ShiftPeriodicLattice
 from kgcnn.layers.modules import Dense, LazyConcatenate, LazyAdd, LazySubtract
 from kgcnn.layers.pooling import PoolingNodes
 from kgcnn.model.utils import update_model_kwargs
 from kgcnn.layers.mlp import MLP
```

### Comparing `kgcnn-2.2.4/kgcnn/literature/EGNN.py` & `kgcnn-3.0.0/kgcnn/literature/EGNN/_make.py`

 * *Files identical despite different names*

### Comparing `kgcnn-2.2.4/kgcnn/literature/GAT.py` & `kgcnn-3.0.0/kgcnn/literature/GAT/_make.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import tensorflow as tf
 from kgcnn.layers.casting import ChangeTensorType
-from kgcnn.layers.conv.gat_conv import AttentionHeadGAT
+from kgcnn.layers.attention import AttentionHeadGAT
 from kgcnn.layers.modules import LazyConcatenate, Dense, LazyAverage, Activation, \
     OptionalInputEmbedding
 from kgcnn.layers.mlp import GraphMLP, MLP
 from kgcnn.layers.pooling import PoolingNodes
 from kgcnn.model.utils import update_model_kwargs
 
 ks = tf.keras
```

### Comparing `kgcnn-2.2.4/kgcnn/literature/GATv2.py` & `kgcnn-3.0.0/kgcnn/literature/GATv2/_make.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import tensorflow as tf
 from kgcnn.layers.casting import ChangeTensorType
-from kgcnn.layers.conv.gat_conv import AttentionHeadGATV2
+from kgcnn.layers.attention import AttentionHeadGATV2
 from kgcnn.layers.modules import LazyConcatenate, Dense, LazyAverage, Activation, \
     OptionalInputEmbedding
 from kgcnn.layers.mlp import GraphMLP, MLP
 from kgcnn.layers.pooling import PoolingNodes
 from kgcnn.model.utils import update_model_kwargs
 
 ks = tf.keras
```

### Comparing `kgcnn-2.2.4/kgcnn/literature/GCN.py` & `kgcnn-3.0.0/kgcnn/literature/GCN/_make.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,208 +1,208 @@
-import tensorflow as tf
-from kgcnn.layers.casting import ChangeTensorType
-from kgcnn.layers.conv.gcn_conv import GCN
-from kgcnn.layers.modules import Dense, OptionalInputEmbedding
-from kgcnn.layers.mlp import GraphMLP, MLP
-from kgcnn.layers.pooling import PoolingNodes, PoolingWeightedNodes
-from kgcnn.model.utils import generate_embedding, update_model_kwargs
-
-ks = tf.keras
-
-# Keep track of model version from commit date in literature.
-# To be updated if model is changed in a significant way.
-__model_version__ = "2022.11.25"
-
-# Implementation of GCN in `tf.keras` from paper:
-# Semi-Supervised Classification with Graph Convolutional Networks
-# by Thomas N. Kipf, Max Welling
-# https://arxiv.org/abs/1609.02907
-# https://github.com/tkipf/gcn
-
-model_default = {
-    "name": "GCN",
-    "inputs": [{"shape": (None,), "name": "node_attributes", "dtype": "float32", "ragged": True},
-               {"shape": (None, 1), "name": "edge_weights", "dtype": "float32", "ragged": True},
-               {"shape": (None, 2), "name": "edge_indices", "dtype": "int64", "ragged": True}],
-    "input_embedding": {"node": {"input_dim": 95, "output_dim": 64},
-                        "edge": {"input_dim": 10, "output_dim": 64}},
-    "gcn_args": {"units": 100, "use_bias": True, "activation": "relu", "pooling_method": "sum"},
-    "depth": 3, "verbose": 10,
-    "output_embedding": "graph", "output_to_tensor": True,
-    "output_mlp": {"use_bias": [True, True, False], "units": [25, 10, 1],
-                   "activation": ["relu", "relu", "sigmoid"]}
-}
-
-
-@update_model_kwargs(model_default)
-def make_model(inputs: list = None,
-               input_embedding: dict = None,
-               depth: int = None,
-               gcn_args: dict = None,
-               name: str = None,
-               verbose: int = None,
-               output_embedding: str = None,
-               output_to_tensor: bool = None,
-               output_mlp: dict = None
-               ):
-    r"""Make `GCN <https://arxiv.org/abs/1609.02907>`_ graph network via functional API.
-    Default parameters can be found in :obj:`kgcnn.literature.GCN.model_default`.
-
-    Inputs:
-        list: `[node_attributes, edge_weights, edge_indices]`
-
-            - node_attributes (tf.RaggedTensor): Node attributes of shape `(batch, None, F)` or `(batch, None)`
-              using an embedding layer.
-            - edge_weights (tf.RaggedTensor): Edge weights of shape `(batch, None, 1)`, that are entries of a scaled
-              adjacency matrix.
-            - edge_indices (tf.RaggedTensor): Index list for edges of shape `(batch, None, 2)`.
-
-    Outputs:
-        tf.Tensor: Graph embeddings of shape `(batch, L)` if :obj:`output_embedding="graph"`.
-
-    Args:
-        inputs (list): List of dictionaries unpacked in :obj:`tf.keras.layers.Input`. Order must match model definition.
-        input_embedding (dict): Dictionary of embedding arguments for nodes etc. unpacked in :obj:`Embedding` layers.
-        depth (int): Number of graph embedding units or depth of the network.
-        gcn_args (dict): Dictionary of layer arguments unpacked in :obj:`GCN` convolutional layer.
-        name (str): Name of the model.
-        verbose (int): Level of print output.
-        output_embedding (str): Main embedding task for graph network. Either "node", "edge" or "graph".
-        output_to_tensor (bool): Whether to cast model output to :obj:`tf.Tensor`.
-        output_mlp (dict): Dictionary of layer arguments unpacked in the final classification :obj:`MLP` layer block.
-            Defines number of model outputs and activation.
-
-    Returns:
-        :obj:`tf.keras.models.Model`
-    """
-    if inputs[1]['shape'][-1] != 1:
-        raise ValueError("No edge features available for GCN, only edge weights of pre-scaled adjacency matrix, \
-                         must be shape (batch, None, 1), but got (without batch-dimension): ", inputs[1]['shape'])
-
-    # Make input
-    node_input = ks.layers.Input(**inputs[0])
-    edge_input = ks.layers.Input(**inputs[1])
-    edge_index_input = ks.layers.Input(**inputs[2])
-
-    # Embedding, if no feature dimension
-    n = OptionalInputEmbedding(**input_embedding['node'],
-                               use_embedding=len(inputs[0]['shape']) < 2)(node_input)
-    ed = OptionalInputEmbedding(**input_embedding['edge'],
-                                use_embedding=len(inputs[1]['shape']) < 2)(edge_input)
-    edi = edge_index_input
-
-    # Model
-    n = Dense(gcn_args["units"], use_bias=True, activation='linear')(n)  # Map to units
-    for i in range(0, depth):
-        n = GCN(**gcn_args)([n, ed, edi])
-
-    # Output embedding choice
-    if output_embedding == "graph":
-        out = PoolingNodes()(n)  # will return tensor
-        out = MLP(**output_mlp)(out)
-    elif output_embedding == "node":
-        out = GraphMLP(**output_mlp)(n)
-        if output_to_tensor:  # For tf version < 2.8 cast to tensor below.
-            out = ChangeTensorType(input_tensor_type='ragged', output_tensor_type="tensor")(out)
-    else:
-        raise ValueError("Unsupported output embedding for `GCN`")
-
-    model = ks.models.Model(inputs=[node_input, edge_input, edge_index_input], outputs=out)
-    model.__kgcnn_model_version__ = __model_version__
-    return model
-
-
-model_default_weighted = {
-    "name": "GCN_weighted",
-    "inputs": [{"shape": (None,), "name": "node_attributes", "dtype": "float32", "ragged": True},
-               {"shape": (None, 1), "name": "edge_weights", "dtype": "float32","ragged": True},
-               {"shape": (None, 2), "name": "edge_indices", "dtype": "int64", "ragged": True},
-               {"shape": (None, 1), "name": "node_weights", "dtype": "float32", "ragged": True}],
-    "input_embedding": {"node": {"input_dim": 95, "output_dim": 64},
-                        "edge": {"input_dim": 10, "output_dim": 64}},
-    "gcn_args": {"units": 100, "use_bias": True, "activation": "relu", "pooling_method": "sum"},
-    "depth": 3, "verbose": 1,
-    "output_embedding": "graph", "output_to_tensor": True,
-    "output_mlp": {"use_bias": [True, True, False], "units": [25, 10, 1],
-                   "activation": ["relu", "relu", "sigmoid"]},
-}
-
-
-@update_model_kwargs(model_default_weighted)
-def make_model_weighted(inputs: list = None,
-                        input_embedding: dict = None,
-                        depth: int = None,
-                        gcn_args: dict = None,
-                        name: str = None,
-                        verbose: int = None,
-                        output_embedding: str = None,
-                        output_to_tensor: bool = None,
-                        output_mlp: dict = None,
-                        ):
-    r"""Make weighted `GCN <https://arxiv.org/abs/1609.02907>`_ graph network via functional API.
-    Default parameters can be found in :obj:`kgcnn.literature.GCN.model_default_weighted`.
-
-    Inputs:
-        list: `[node_attributes, edge_weights, edge_indices, node_weights]`
-
-            - node_attributes (tf.RaggedTensor): Node attributes of shape `(batch, None, F)` or `(batch, None)`
-              using an embedding layer.
-            - edge_weights (tf.RaggedTensor): Edge weights of shape `(batch, None, 1)`, that are entries of a scaled
-              adjacency matrix.
-            - edge_indices (tf.RaggedTensor): Index list for edges of shape `(batch, None, 2)`.
-            - node_weights (tf.RaggedTensor): Node weights of shape `(batch, None, 1)` that can be e.g. a node mask.
-
-    Outputs:
-        tf.Tensor: Graph embeddings of shape `(batch, L)` if :obj:`output_embedding="graph"`.
-
-    Args:
-        inputs (list): List of dictionaries unpacked in :obj:`tf.keras.layers.Input`. Order must match model definition.
-        input_embedding (dict): Dictionary of embedding arguments for nodes etc. unpacked in :obj:`Embedding` layers.
-        depth (int): Number of graph embedding units or depth of the network.
-        gcn_args (dict): Dictionary of layer arguments unpacked in :obj:`GCN` convolutional layer.
-        name (str): Name of the model.
-        verbose (int): Level of print output.
-        output_embedding (str): Main embedding task for graph network. Either "node", "edge" or "graph".
-        output_to_tensor (bool): Whether to cast model output to :obj:`tf.Tensor`.
-        output_mlp (dict): Dictionary of layer arguments unpacked in the final classification :obj:`MLP` layer block.
-            Defines number of model outputs and activation.
-
-    Returns:
-        :obj:`tf.keras.models.Model`
-    """
-    if inputs[1]['shape'][-1] != 1:
-        raise ValueError("No edge features available for GCN, only edge weights of pre-scaled adjacency matrix, \
-                         must be shape (batch, None, 1), but got (without batch-dimension): ", inputs[1]['shape'])
-
-    # Make input
-    node_input = ks.layers.Input(**inputs[0])
-    edge_input = ks.layers.Input(**inputs[1])
-    edge_index_input = ks.layers.Input(**inputs[2])
-    node_weights_input = ks.layers.Input(**inputs[3])
-
-    # Embedding, if no feature dimension
-    n = OptionalInputEmbedding(**input_embedding['node'],
-                               use_embedding=len(inputs[0]['shape']) < 2)(node_input)
-    ed = OptionalInputEmbedding(**input_embedding['edge'],
-                                use_embedding=len(inputs[1]['shape']) < 2)(edge_input)
-    edi = edge_index_input
-    nw = node_weights_input
-
-    # Model
-    n = Dense(gcn_args["units"], use_bias=True, activation='linear')(n)  # Map to units
-    for i in range(0, depth):
-        n = GCN(**gcn_args)([n, ed, edi])
-
-    # Output embedding choice
-    if output_embedding == "graph":
-        out = PoolingWeightedNodes()([n, nw])  # will return tensor
-        out = MLP(**output_mlp)(out)
-    elif output_embedding == "node":
-        out = GraphMLP(**output_mlp)(n)
-        if output_to_tensor:  # For tf version < 2.8 cast to tensor below.
-            out = ChangeTensorType(input_tensor_type='ragged', output_tensor_type="tensor")(out)
-    else:
-        raise ValueError("Unsupported output embedding for `GCN`")
-
-    model = ks.models.Model(inputs=[node_input, edge_input, edge_index_input, node_weights_input], outputs=out)
-    model.__kgcnn_model_version__ = __model_version__
-    return model
+import tensorflow as tf
+from kgcnn.layers.casting import ChangeTensorType
+from kgcnn.layers.conv import GCN
+from kgcnn.layers.modules import Dense, OptionalInputEmbedding
+from kgcnn.layers.mlp import GraphMLP, MLP
+from kgcnn.layers.pooling import PoolingNodes, PoolingWeightedNodes
+from kgcnn.model.utils import update_model_kwargs
+
+ks = tf.keras
+
+# Keep track of model version from commit date in literature.
+# To be updated if model is changed in a significant way.
+__model_version__ = "2022.11.25"
+
+# Implementation of GCN in `tf.keras` from paper:
+# Semi-Supervised Classification with Graph Convolutional Networks
+# by Thomas N. Kipf, Max Welling
+# https://arxiv.org/abs/1609.02907
+# https://github.com/tkipf/gcn
+
+model_default = {
+    "name": "GCN",
+    "inputs": [{"shape": (None,), "name": "node_attributes", "dtype": "float32", "ragged": True},
+               {"shape": (None, 1), "name": "edge_weights", "dtype": "float32", "ragged": True},
+               {"shape": (None, 2), "name": "edge_indices", "dtype": "int64", "ragged": True}],
+    "input_embedding": {"node": {"input_dim": 95, "output_dim": 64},
+                        "edge": {"input_dim": 10, "output_dim": 64}},
+    "gcn_args": {"units": 100, "use_bias": True, "activation": "relu", "pooling_method": "sum"},
+    "depth": 3, "verbose": 10,
+    "output_embedding": "graph", "output_to_tensor": True,
+    "output_mlp": {"use_bias": [True, True, False], "units": [25, 10, 1],
+                   "activation": ["relu", "relu", "sigmoid"]}
+}
+
+
+@update_model_kwargs(model_default)
+def make_model(inputs: list = None,
+               input_embedding: dict = None,
+               depth: int = None,
+               gcn_args: dict = None,
+               name: str = None,
+               verbose: int = None,
+               output_embedding: str = None,
+               output_to_tensor: bool = None,
+               output_mlp: dict = None
+               ):
+    r"""Make `GCN <https://arxiv.org/abs/1609.02907>`_ graph network via functional API.
+    Default parameters can be found in :obj:`kgcnn.literature.GCN.model_default`.
+
+    Inputs:
+        list: `[node_attributes, edge_weights, edge_indices]`
+
+            - node_attributes (tf.RaggedTensor): Node attributes of shape `(batch, None, F)` or `(batch, None)`
+              using an embedding layer.
+            - edge_weights (tf.RaggedTensor): Edge weights of shape `(batch, None, 1)`, that are entries of a scaled
+              adjacency matrix.
+            - edge_indices (tf.RaggedTensor): Index list for edges of shape `(batch, None, 2)`.
+
+    Outputs:
+        tf.Tensor: Graph embeddings of shape `(batch, L)` if :obj:`output_embedding="graph"`.
+
+    Args:
+        inputs (list): List of dictionaries unpacked in :obj:`tf.keras.layers.Input`. Order must match model definition.
+        input_embedding (dict): Dictionary of embedding arguments for nodes etc. unpacked in :obj:`Embedding` layers.
+        depth (int): Number of graph embedding units or depth of the network.
+        gcn_args (dict): Dictionary of layer arguments unpacked in :obj:`GCN` convolutional layer.
+        name (str): Name of the model.
+        verbose (int): Level of print output.
+        output_embedding (str): Main embedding task for graph network. Either "node", "edge" or "graph".
+        output_to_tensor (bool): Whether to cast model output to :obj:`tf.Tensor`.
+        output_mlp (dict): Dictionary of layer arguments unpacked in the final classification :obj:`MLP` layer block.
+            Defines number of model outputs and activation.
+
+    Returns:
+        :obj:`tf.keras.models.Model`
+    """
+    if inputs[1]['shape'][-1] != 1:
+        raise ValueError("No edge features available for GCN, only edge weights of pre-scaled adjacency matrix, \
+                         must be shape (batch, None, 1), but got (without batch-dimension): ", inputs[1]['shape'])
+
+    # Make input
+    node_input = ks.layers.Input(**inputs[0])
+    edge_input = ks.layers.Input(**inputs[1])
+    edge_index_input = ks.layers.Input(**inputs[2])
+
+    # Embedding, if no feature dimension
+    n = OptionalInputEmbedding(**input_embedding['node'],
+                               use_embedding=len(inputs[0]['shape']) < 2)(node_input)
+    ed = OptionalInputEmbedding(**input_embedding['edge'],
+                                use_embedding=len(inputs[1]['shape']) < 2)(edge_input)
+    edi = edge_index_input
+
+    # Model
+    n = Dense(gcn_args["units"], use_bias=True, activation='linear')(n)  # Map to units
+    for i in range(0, depth):
+        n = GCN(**gcn_args)([n, ed, edi])
+
+    # Output embedding choice
+    if output_embedding == "graph":
+        out = PoolingNodes()(n)  # will return tensor
+        out = MLP(**output_mlp)(out)
+    elif output_embedding == "node":
+        out = GraphMLP(**output_mlp)(n)
+        if output_to_tensor:  # For tf version < 2.8 cast to tensor below.
+            out = ChangeTensorType(input_tensor_type='ragged', output_tensor_type="tensor")(out)
+    else:
+        raise ValueError("Unsupported output embedding for `GCN`")
+
+    model = ks.models.Model(inputs=[node_input, edge_input, edge_index_input], outputs=out)
+    model.__kgcnn_model_version__ = __model_version__
+    return model
+
+
+model_default_weighted = {
+    "name": "GCN_weighted",
+    "inputs": [{"shape": (None,), "name": "node_attributes", "dtype": "float32", "ragged": True},
+               {"shape": (None, 1), "name": "edge_weights", "dtype": "float32","ragged": True},
+               {"shape": (None, 2), "name": "edge_indices", "dtype": "int64", "ragged": True},
+               {"shape": (None, 1), "name": "node_weights", "dtype": "float32", "ragged": True}],
+    "input_embedding": {"node": {"input_dim": 95, "output_dim": 64},
+                        "edge": {"input_dim": 10, "output_dim": 64}},
+    "gcn_args": {"units": 100, "use_bias": True, "activation": "relu", "pooling_method": "sum"},
+    "depth": 3, "verbose": 1,
+    "output_embedding": "graph", "output_to_tensor": True,
+    "output_mlp": {"use_bias": [True, True, False], "units": [25, 10, 1],
+                   "activation": ["relu", "relu", "sigmoid"]},
+}
+
+
+@update_model_kwargs(model_default_weighted)
+def make_model_weighted(inputs: list = None,
+                        input_embedding: dict = None,
+                        depth: int = None,
+                        gcn_args: dict = None,
+                        name: str = None,
+                        verbose: int = None,
+                        output_embedding: str = None,
+                        output_to_tensor: bool = None,
+                        output_mlp: dict = None,
+                        ):
+    r"""Make weighted `GCN <https://arxiv.org/abs/1609.02907>`_ graph network via functional API.
+    Default parameters can be found in :obj:`kgcnn.literature.GCN.model_default_weighted`.
+
+    Inputs:
+        list: `[node_attributes, edge_weights, edge_indices, node_weights]`
+
+            - node_attributes (tf.RaggedTensor): Node attributes of shape `(batch, None, F)` or `(batch, None)`
+              using an embedding layer.
+            - edge_weights (tf.RaggedTensor): Edge weights of shape `(batch, None, 1)`, that are entries of a scaled
+              adjacency matrix.
+            - edge_indices (tf.RaggedTensor): Index list for edges of shape `(batch, None, 2)`.
+            - node_weights (tf.RaggedTensor): Node weights of shape `(batch, None, 1)` that can be e.g. a node mask.
+
+    Outputs:
+        tf.Tensor: Graph embeddings of shape `(batch, L)` if :obj:`output_embedding="graph"`.
+
+    Args:
+        inputs (list): List of dictionaries unpacked in :obj:`tf.keras.layers.Input`. Order must match model definition.
+        input_embedding (dict): Dictionary of embedding arguments for nodes etc. unpacked in :obj:`Embedding` layers.
+        depth (int): Number of graph embedding units or depth of the network.
+        gcn_args (dict): Dictionary of layer arguments unpacked in :obj:`GCN` convolutional layer.
+        name (str): Name of the model.
+        verbose (int): Level of print output.
+        output_embedding (str): Main embedding task for graph network. Either "node", "edge" or "graph".
+        output_to_tensor (bool): Whether to cast model output to :obj:`tf.Tensor`.
+        output_mlp (dict): Dictionary of layer arguments unpacked in the final classification :obj:`MLP` layer block.
+            Defines number of model outputs and activation.
+
+    Returns:
+        :obj:`tf.keras.models.Model`
+    """
+    if inputs[1]['shape'][-1] != 1:
+        raise ValueError("No edge features available for GCN, only edge weights of pre-scaled adjacency matrix, \
+                         must be shape (batch, None, 1), but got (without batch-dimension): ", inputs[1]['shape'])
+
+    # Make input
+    node_input = ks.layers.Input(**inputs[0])
+    edge_input = ks.layers.Input(**inputs[1])
+    edge_index_input = ks.layers.Input(**inputs[2])
+    node_weights_input = ks.layers.Input(**inputs[3])
+
+    # Embedding, if no feature dimension
+    n = OptionalInputEmbedding(**input_embedding['node'],
+                               use_embedding=len(inputs[0]['shape']) < 2)(node_input)
+    ed = OptionalInputEmbedding(**input_embedding['edge'],
+                                use_embedding=len(inputs[1]['shape']) < 2)(edge_input)
+    edi = edge_index_input
+    nw = node_weights_input
+
+    # Model
+    n = Dense(gcn_args["units"], use_bias=True, activation='linear')(n)  # Map to units
+    for i in range(0, depth):
+        n = GCN(**gcn_args)([n, ed, edi])
+
+    # Output embedding choice
+    if output_embedding == "graph":
+        out = PoolingWeightedNodes()([n, nw])  # will return tensor
+        out = MLP(**output_mlp)(out)
+    elif output_embedding == "node":
+        out = GraphMLP(**output_mlp)(n)
+        if output_to_tensor:  # For tf version < 2.8 cast to tensor below.
+            out = ChangeTensorType(input_tensor_type='ragged', output_tensor_type="tensor")(out)
+    else:
+        raise ValueError("Unsupported output embedding for `GCN`")
+
+    model = ks.models.Model(inputs=[node_input, edge_input, edge_index_input, node_weights_input], outputs=out)
+    model.__kgcnn_model_version__ = __model_version__
+    return model
```

### Comparing `kgcnn-2.2.4/kgcnn/literature/GIN.py` & `kgcnn-3.0.0/kgcnn/literature/GIN/_make.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import tensorflow as tf
 from kgcnn.layers.casting import ChangeTensorType
-from kgcnn.layers.conv.gin_conv import GIN, GINE
+from ._gin_conv import GIN, GINE
 from kgcnn.layers.modules import Dense, OptionalInputEmbedding
 from kgcnn.layers.mlp import GraphMLP, MLP
 from kgcnn.layers.pooling import PoolingNodes
 from kgcnn.model.utils import update_model_kwargs
 
 ks = tf.keras
```

### Comparing `kgcnn-2.2.4/kgcnn/literature/GNNExplain.py` & `kgcnn-3.0.0/kgcnn/literature/GNNExplain/_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import time
 import typing as t
 
 import numpy as np
 import tensorflow as tf
 ks = tf.keras
 
-from kgcnn.xai.base import ImportanceExplanationMethod
+from ._xai._base import ImportanceExplanationMethod
 
 # Keep track of model version from commit date in literature.
 # To be updated if model is changed in a significant way.
 __model_version__ = "2023.01.30"
 
 
 # == REDUCED, RAGGED TENSOR IMPLEMENTATION ==
```

### Comparing `kgcnn-2.2.4/kgcnn/literature/GNNFilm.py` & `kgcnn-3.0.0/kgcnn/literature/GNNFilm/_make.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import tensorflow as tf
 from kgcnn.layers.casting import ChangeTensorType
 from kgcnn.layers.gather import GatherNodesSelection
-from kgcnn.layers.modules import Dense, OptionalInputEmbedding, LazyMultiply, LazyAdd, Activation
+from kgcnn.layers.modules import OptionalInputEmbedding, LazyMultiply, LazyAdd, Activation
 from kgcnn.layers.pooling import PoolingLocalMessages
 from kgcnn.layers.mlp import GraphMLP, MLP
 from kgcnn.layers.pooling import PoolingNodes
 from kgcnn.layers.relational import RelationalDense
 from kgcnn.model.utils import update_model_kwargs
 
 ks = tf.keras
```

### Comparing `kgcnn-2.2.4/kgcnn/literature/GraphSAGE.py` & `kgcnn-3.0.0/kgcnn/literature/GraphSAGE/_make.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 # Implementation of GraphSAGE in `tf.keras` from paper:
 # Inductive Representation Learning on Large Graphs
 # by William L. Hamilton and Rex Ying and Jure Leskovec
 # http://arxiv.org/abs/1706.02216
 
 
-hyper_model_default = {
+model_default = {
     'name': "GraphSAGE",
     'inputs': [{'shape': (None,), 'name': "node_attributes", 'dtype': 'float32', 'ragged': True},
                {'shape': (None,), 'name': "edge_attributes", 'dtype': 'float32', 'ragged': True},
                {'shape': (None, 2), 'name': "edge_indices", 'dtype': 'int64', 'ragged': True}],
     'input_embedding': {"node": {"input_dim": 95, "output_dim": 64},
                         "edge": {"input_dim": 5, "output_dim": 64}},
     'node_mlp_args': {"units": [100, 50], "use_bias": True, "activation": ['relu', "linear"]},
@@ -34,15 +34,15 @@
     'depth': 3, 'verbose': 10,
     'output_embedding': 'graph', "output_to_tensor": True,
     'output_mlp': {"use_bias": [True, True, False], "units": [25, 10, 1],
                    "activation": ['relu', 'relu', 'sigmoid']}
 }
 
 
-@update_model_kwargs(hyper_model_default)
+@update_model_kwargs(model_default)
 def make_model(inputs: list = None,
                input_embedding: dict = None,
                node_mlp_args: dict = None,
                edge_mlp_args: dict = None,
                pooling_args: dict = None,
                pooling_nodes_args: dict = None,
                gather_args: dict = None,
@@ -52,15 +52,16 @@
                name: str = None,
                verbose: int = None,
                output_embedding: str = None,
                output_to_tensor: bool = None,
                output_mlp: dict = None
                ):
     r"""Make `GraphSAGE <http://arxiv.org/abs/1706.02216>`_ graph network via functional API.
-    Default parameters can be found in :obj:`kgcnn.literature.GraphSAGE.hyper_model_default`.
+
+    Default parameters can be found in :obj:`kgcnn.literature.GraphSAGE.model_default` .
 
     Inputs:
         list: `[node_attributes, edge_attributes, edge_indices]`
 
             - node_attributes (tf.RaggedTensor): Node attributes of shape `(batch, None, F)` or `(batch, None)`
               using an embedding layer.
             - edge_attributes (tf.RaggedTensor): Edge attributes of shape `(batch, None, F)` or `(batch, None)`
```

### Comparing `kgcnn-2.2.4/kgcnn/literature/HDNNP2nd.py` & `kgcnn-3.0.0/kgcnn/literature/HDNNP2nd/_make.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import tensorflow as tf
 from kgcnn.layers.casting import ChangeTensorType
 from kgcnn.layers.modules import LazyConcatenate
-from kgcnn.layers.conv.wacsf_conv import wACSFAng, wACSFRad
-from kgcnn.layers.conv.acsf_conv import ACSFG2, ACSFG4, ACSFConstNormalization
+from ._wacsf_conv import wACSFAng, wACSFRad
+from ._acsf_conv import ACSFG2, ACSFG4, ACSFConstNormalization
 from kgcnn.layers.mlp import GraphMLP, MLP
 from kgcnn.layers.pooling import PoolingNodes
 from kgcnn.model.utils import update_model_kwargs
 from kgcnn.layers.mlp import RelationalMLP
 from kgcnn.layers.norm import GraphBatchNormalization
 
 ks = tf.keras
@@ -242,15 +242,15 @@
     model = ks.models.Model(
         inputs=[node_input, xyz_input, edge_index_input, angle_index_input], outputs=out, name=name)
 
     model.__kgcnn_model_version__ = __model_version__
     return model
 
 
-model_atom_wise_default = {
+model_default_atom_wise = {
     "name": "HDNNP2nd",
     "inputs": [{"shape": (None,), "name": "node_number", "dtype": "int64", "ragged": True},
                {"shape": (None, 3), "name": "node_representation", "dtype": "float32", "ragged": True}],
     "mlp_kwargs": {"units": [64, 64, 64],
                    "num_relations": 96,
                    "activation": ["swish", "swish", "linear"]},
     "node_pooling_args": {"pooling_method": "sum"},
@@ -258,28 +258,28 @@
     "output_embedding": "graph", "output_to_tensor": True,
     "use_output_mlp": False,
     "output_mlp": {"use_bias": [True, True], "units": [64, 1],
                    "activation": ["swish", "linear"]}
 }
 
 
-@update_model_kwargs(model_atom_wise_default)
+@update_model_kwargs(model_default_atom_wise)
 def make_model_atom_wise(inputs: list = None,
                          node_pooling_args: dict = None,
                          name: str = None,
                          verbose: int = None,
                          mlp_kwargs: dict = None,
                          output_embedding: str = None,
                          use_output_mlp: bool = None,
                          output_to_tensor: bool = None,
                          output_mlp: dict = None
                          ):
     r"""Make 2nd generation `HDNNP <https://arxiv.org/abs/1706.08566>`_ network via functional API.
 
-    Default parameters can be found in :obj:`kgcnn.literature.HDNNP2nd.model_atom_wise_default`.
+    Default parameters can be found in :obj:`kgcnn.literature.HDNNP2nd.model_default_atom_wise`.
 
     Inputs:
         list: `[node_number, node_representation]`
 
             - node_number (tf.RaggedTensor): Atomic number of shape `(batch, None)` .
             - node_representation (tf.RaggedTensor): Node (atomic) features of shape `(batch, None, F)`
 
@@ -327,7 +327,8 @@
 
     model.__kgcnn_model_version__ = __model_version__
     return model
 
 
 # For default, the weighted ACSF are used, since they do should in principle work for all elements.
 make_model = make_model_weighted
+model_default = model_default_weighted
```

### Comparing `kgcnn-2.2.4/kgcnn/literature/HDNNP4th.py` & `kgcnn-3.0.0/kgcnn/literature/HDNNP4th/_make.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import tensorflow as tf
 from kgcnn.layers.modules import LazyConcatenate
-from kgcnn.layers.conv.acsf_conv import ACSFG2, ACSFG4, ACSFConstNormalization
-from kgcnn.layers.mlp import GraphMLP, MLP
+from kgcnn.literature.HDNNP2nd._acsf_conv import ACSFG2, ACSFG4, ACSFConstNormalization
+from kgcnn.layers.mlp import MLP
 from kgcnn.layers.pooling import PoolingNodes
 from kgcnn.model.utils import update_model_kwargs
 # from kgcnn.layers.conv.hdnnp_conv import CENTCharge, ElectrostaticEnergyCharge
-from kgcnn.layers.conv.hdnnp_conv import CENTChargePlusElectrostaticEnergy
+from ._hdnnp_conv import CENTChargePlusElectrostaticEnergy
 from kgcnn.layers.mlp import RelationalMLP
 from kgcnn.layers.norm import GraphBatchNormalization
 
 ks = tf.keras
 
 # Keep track of model version from commit date in literature.
 # To be updated if model is changed in a significant way.
```

### Comparing `kgcnn-2.2.4/kgcnn/literature/HamNet.py` & `kgcnn-3.0.0/kgcnn/literature/HamNet/_make.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 from math import inf
 from kgcnn.layers.gather import GatherNodes
 from kgcnn.layers.casting import ChangeTensorType
 from kgcnn.layers.mlp import MLP, GraphMLP
 from kgcnn.model.utils import update_model_kwargs
 from kgcnn.layers.modules import LazyConcatenate, OptionalInputEmbedding, Dense, Activation, ZerosLike
 from kgcnn.layers.pooling import PoolingNodes, PoolingEmbeddingAttention
-from kgcnn.layers.conv.hamnet_conv import HamNaiveDynMessage, HamNetFingerprintGenerator, HamNetGRUUnion, \
-    HamNetNaiveUnion
+from ._hamnet_conv import HamNaiveDynMessage, HamNetFingerprintGenerator, HamNetGRUUnion, HamNetNaiveUnion
 
 # import tensorflow.keras as ks
 # import tensorflow.python.keras as ks
 ks = tf.keras
 
 # Keep track of model version from commit date in literature.
 # To be updated if model is changed in a significant way.
@@ -22,15 +21,15 @@
 # by Ziyao Li, Shuwen Yang, Guojie Song, Lingsheng Cai
 # Link to paper: https://arxiv.org/abs/2105.03688
 # Original implementation: https://github.com/PKUterran/HamNet
 # Later implementation: https://github.com/PKUterran/MoleculeClub
 # Note: the 2. implementation is cleaner than the original code and has been used as template.
 
 
-hyper_model_default = {
+model_default = {
     "name": "HamNet",
     "inputs": [{'shape': (None,), 'name': "node_attributes", 'dtype': 'float32', 'ragged': True},
                {'shape': (None,), 'name': "edge_attributes", 'dtype': 'float32', 'ragged': True},
                {'shape': (None, 2), 'name': "edge_indices", 'dtype': 'int64', 'ragged': True},
                {'shape': (None, 3), 'name': "node_coordinates", 'dtype': 'float32', 'ragged': True}],
     "input_embedding": {"node": {"input_dim": 95, "output_dim": 64},
                         "edge": {"input_dim": 5, "output_dim": 64}},
@@ -43,15 +42,15 @@
     "given_coordinates": True,
     'output_embedding': 'graph', "output_to_tensor": True,
     'output_mlp': {"use_bias": [True, True, False], "units": [25, 10, 1],
                    "activation": ['relu', 'relu', 'linear']}
 }
 
 
-@update_model_kwargs(hyper_model_default, update_recursive=inf)
+@update_model_kwargs(model_default, update_recursive=inf)
 def make_model(name: str = None,
                inputs: list = None,
                input_embedding: dict = None,
                verbose: int = None,
                message_kwargs: dict = None,
                gru_kwargs: dict = None,
                fingerprint_kwargs: dict = None,
@@ -60,15 +59,15 @@
                given_coordinates: bool = None,
                depth: int = None,
                output_embedding: str = None,
                output_to_tensor: bool = None,
                output_mlp: dict = None
                ):
     r"""Make `HamNet <https://arxiv.org/abs/2105.03688>`_ graph model via functional API.
-    Default parameters can be found in :obj:`kgcnn.literature.HamNet.hyper_model_default`.
+    Default parameters can be found in :obj:`kgcnn.literature.HamNet.model_default` .
 
     .. note::
         At the moment only the Fingerprint Generator for graph embeddings is implemented and coordinates must
         be provided as model input.
 
     Inputs:
         list: `[node_attributes, edge_attributes, edge_indices]`,
```

### Comparing `kgcnn-2.2.4/kgcnn/literature/INorp.py` & `kgcnn-3.0.0/kgcnn/literature/INorp/_make.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,153 +1,154 @@
-import tensorflow as tf
-from kgcnn.layers.casting import ChangeTensorType
-from kgcnn.layers.gather import GatherState, GatherNodesIngoing, GatherNodesOutgoing
-from kgcnn.layers.modules import LazyConcatenate, Dense, OptionalInputEmbedding
-from kgcnn.layers.mlp import GraphMLP, MLP
-from kgcnn.layers.pooling import PoolingLocalEdges, PoolingNodes
-from kgcnn.layers.pool.set2set import PoolingSet2Set
-from kgcnn.model.utils import update_model_kwargs
-
-ks = tf.keras
-
-# Keep track of model version from commit date in literature.
-# To be updated if model is changed in a significant way.
-__model_version__ = "2022.11.25"
-
-# Implementation of INorp in `tf.keras` from paper:
-# 'Interaction Networks for Learning about Objects, Relations and Physics'
-# by Peter W. Battaglia, Razvan Pascanu, Matthew Lai, Danilo Rezende, Koray Kavukcuoglu
-# http://papers.nips.cc/paper/6417-interaction-networks-for-learning-about-objects-relations-and-physics
-# https://arxiv.org/abs/1612.00222
-# https://github.com/higgsfield/interaction_network_pytorch
-
-hyper_model_default = {'name': "INorp",
-                       'inputs': [{'shape': (None,), 'name': "node_attributes", 'dtype': 'float32', 'ragged': True},
-                                  {'shape': (None,), 'name': "edge_attributes", 'dtype': 'float32', 'ragged': True},
-                                  {'shape': (None, 2), 'name': "edge_indices", 'dtype': 'int64', 'ragged': True},
-                                  {'shape': [], 'name': "graph_attributes", 'dtype': 'float32', 'ragged': False}],
-                       'input_embedding': {"node": {"input_dim": 95, "output_dim": 64},
-                                           "edge": {"input_dim": 5, "output_dim": 64},
-                                           "graph": {"input_dim": 100, "output_dim": 64}},
-                       'set2set_args': {"channels": 32, "T": 3, "pooling_method": "mean",
-                                        "init_qstar": "mean"},
-                       'node_mlp_args': {"units": [100, 50], "use_bias": True, "activation": ['relu', "linear"]},
-                       'edge_mlp_args': {"units": [100, 100, 100, 100, 50],
-                                         "activation": ['relu', 'relu', 'relu', 'relu', "linear"]},
-                       'pooling_args': {'pooling_method': "segment_mean"},
-                       'depth': 3, 'use_set2set': False, 'verbose': 10,
-                       'gather_args': {},
-                       'output_embedding': 'graph', "output_to_tensor": True,
-                       'output_mlp': {"use_bias": [True, True, False], "units": [25, 10, 1],
-                                      "activation": ['relu', 'relu', 'sigmoid']}
-                       }
-
-
-@update_model_kwargs(hyper_model_default)
-def make_model(inputs: list = None,
-               input_embedding: dict = None,
-               depth: int = None,
-               gather_args: dict = None,
-               edge_mlp_args: dict = None,
-               node_mlp_args: dict = None,
-               set2set_args: dict = None,
-               pooling_args: dict = None,
-               use_set2set: dict = None,
-               name: str = None,
-               verbose: int = None,
-               output_embedding: str = None,
-               output_to_tensor: bool = None,
-               output_mlp: dict = None
-               ):
-    r"""Make `INorp <https://arxiv.org/abs/1612.00222>`_ graph network via functional API.
-    Default parameters can be found in :obj:`kgcnn.literature.INorp.hyper_model_default`.
-
-    Inputs:
-        list: `[node_attributes, edge_attributes, edge_indices, state_attributes]`
-
-            - node_attributes (tf.RaggedTensor): Node attributes of shape `(batch, None, F)` or `(batch, None)`
-              using an embedding layer.
-            - edge_attributes (tf.RaggedTensor): Edge attributes of shape `(batch, None, F)` or `(batch, None)`
-              using an embedding layer.
-            - edge_indices (tf.RaggedTensor): Index list for edges of shape `(batch, None, 2)`.
-            - state_attributes (tf.Tensor): Environment or graph state attributes of shape `(batch, F)` or `(batch,)`
-              using an embedding layer.
-
-    Outputs:
-        tf.Tensor: Graph embeddings of shape `(batch, L)` if :obj:`output_embedding="graph"`.
-
-    Args:
-        inputs (list): List of dictionaries unpacked in :obj:`tf.keras.layers.Input`. Order must match model definition.
-        input_embedding (dict): Dictionary of embedding arguments for nodes etc. unpacked in :obj:`Embedding` layers.
-        depth (int): Number of graph embedding units or depth of the network.
-        gather_args (dict): Dictionary of layer arguments unpacked in :obj:`GatherNodes` layer.
-        edge_mlp_args (dict): Dictionary of layer arguments unpacked in :obj:`MLP` layer for edge updates.
-        node_mlp_args (dict): Dictionary of layer arguments unpacked in :obj:`MLP` layer for node updates.
-        set2set_args (dict): Dictionary of layer arguments unpacked in :obj:`PoolingSet2Set` layer.
-        pooling_args (dict): Dictionary of layer arguments unpacked in :obj:`PoolingLocalEdges`, :obj:`PoolingNodes`
-            layer.
-        use_set2set (bool): Whether to use :obj:`PoolingSet2Set` layer.
-        verbose (int): Level of verbosity.
-        name (str): Name of the model.
-        output_embedding (str): Main embedding task for graph network. Either "node", "edge" or "graph".
-        output_to_tensor (bool): Whether to cast model output to :obj:`tf.Tensor`.
-        output_mlp (dict): Dictionary of layer arguments unpacked in the final classification :obj:`MLP` layer block.
-            Defines number of model outputs and activation.
-
-    Returns:
-        :obj:`tf.keras.models.Model`
-    """
-    # Make input
-    node_input = ks.layers.Input(**inputs[0])
-    edge_input = ks.layers.Input(**inputs[1])
-    edge_index_input = ks.layers.Input(**inputs[2])
-    env_input = ks.Input(**inputs[3])
-
-    # embedding, if no feature dimension
-    n = OptionalInputEmbedding(**input_embedding['node'],
-                               use_embedding=len(inputs[0]['shape']) < 2)(node_input)
-    ed = OptionalInputEmbedding(**input_embedding['edge'],
-                                use_embedding=len(inputs[1]['shape']) < 2)(edge_input)
-    uenv = OptionalInputEmbedding(**input_embedding['graph'],
-                                  use_embedding=len(inputs[3]['shape']) < 1)(env_input)
-    edi = edge_index_input
-
-    # Model
-    ev = GatherState(**gather_args)([uenv, n])
-    # n-Layer Step
-    for i in range(0, depth):
-        # upd = GatherNodes()([n,edi])
-        eu1 = GatherNodesIngoing(**gather_args)([n, edi])
-        eu2 = GatherNodesOutgoing(**gather_args)([n, edi])
-        upd = LazyConcatenate(axis=-1)([eu2, eu1])
-        eu = LazyConcatenate(axis=-1)([upd, ed])
-
-        eu = GraphMLP(**edge_mlp_args)(eu)
-        # Pool message
-        nu = PoolingLocalEdges(**pooling_args)(
-            [n, eu, edi])  # Summing for each node connection
-        # Add environment
-        nu = LazyConcatenate(axis=-1)(
-            [n, nu, ev])  # LazyConcatenate node features with new edge updates
-        n = GraphMLP(**node_mlp_args)(nu)
-
-    # Output embedding choice
-    if output_embedding == 'graph':
-        if use_set2set:
-            # output
-            n = Dense(set2set_args["channels"], activation="linear")(n)
-            out = PoolingSet2Set(**set2set_args)(n)
-        else:
-            out = PoolingNodes(**pooling_args)(n)
-        out = ks.layers.Flatten()(out)
-        out = MLP(**output_mlp)(out)
-    elif output_embedding == 'node':
-        out = GraphMLP(**output_mlp)(n)
-        if output_to_tensor:  # For tf version < 2.8 cast to tensor below.
-            out = ChangeTensorType(input_tensor_type="ragged", output_tensor_type="tensor")(out)
-    else:
-        raise ValueError("Unsupported output embedding for mode `INorp`")
-
-    model = ks.models.Model(inputs=[node_input, edge_input, edge_index_input, env_input], outputs=out)
-
-    model.__kgcnn_model_version__ = __model_version__
-    return model
+import tensorflow as tf
+from kgcnn.layers.casting import ChangeTensorType
+from kgcnn.layers.gather import GatherState, GatherNodesIngoing, GatherNodesOutgoing
+from kgcnn.layers.modules import LazyConcatenate, Dense, OptionalInputEmbedding
+from kgcnn.layers.mlp import GraphMLP, MLP
+from kgcnn.layers.pooling import PoolingLocalEdges, PoolingNodes
+from kgcnn.layers.set2set import PoolingSet2SetEncoder
+from kgcnn.model.utils import update_model_kwargs
+
+ks = tf.keras
+
+# Keep track of model version from commit date in literature.
+# To be updated if model is changed in a significant way.
+__model_version__ = "2022.11.25"
+
+# Implementation of INorp in `tf.keras` from paper:
+# 'Interaction Networks for Learning about Objects, Relations and Physics'
+# by Peter W. Battaglia, Razvan Pascanu, Matthew Lai, Danilo Rezende, Koray Kavukcuoglu
+# http://papers.nips.cc/paper/6417-interaction-networks-for-learning-about-objects-relations-and-physics
+# https://arxiv.org/abs/1612.00222
+# https://github.com/higgsfield/interaction_network_pytorch
+
+model_default = {'name': "INorp",
+                 'inputs': [{'shape': (None,), 'name': "node_attributes", 'dtype': 'float32', 'ragged': True},
+                            {'shape': (None,), 'name': "edge_attributes", 'dtype': 'float32', 'ragged': True},
+                            {'shape': (None, 2), 'name': "edge_indices", 'dtype': 'int64', 'ragged': True},
+                            {'shape': [], 'name': "graph_attributes", 'dtype': 'float32', 'ragged': False}],
+                 'input_embedding': {"node": {"input_dim": 95, "output_dim": 64},
+                                     "edge": {"input_dim": 5, "output_dim": 64},
+                                     "graph": {"input_dim": 100, "output_dim": 64}},
+                 'set2set_args': {"channels": 32, "T": 3, "pooling_method": "mean",
+                                  "init_qstar": "mean"},
+                 'node_mlp_args': {"units": [100, 50], "use_bias": True, "activation": ['relu', "linear"]},
+                 'edge_mlp_args': {"units": [100, 100, 100, 100, 50],
+                                   "activation": ['relu', 'relu', 'relu', 'relu', "linear"]},
+                 'pooling_args': {'pooling_method': "segment_mean"},
+                 'depth': 3, 'use_set2set': False, 'verbose': 10,
+                 'gather_args': {},
+                 'output_embedding': 'graph', "output_to_tensor": True,
+                 'output_mlp': {"use_bias": [True, True, False], "units": [25, 10, 1],
+                                "activation": ['relu', 'relu', 'sigmoid']}
+                 }
+
+
+@update_model_kwargs(model_default)
+def make_model(inputs: list = None,
+               input_embedding: dict = None,
+               depth: int = None,
+               gather_args: dict = None,
+               edge_mlp_args: dict = None,
+               node_mlp_args: dict = None,
+               set2set_args: dict = None,
+               pooling_args: dict = None,
+               use_set2set: dict = None,
+               name: str = None,
+               verbose: int = None,
+               output_embedding: str = None,
+               output_to_tensor: bool = None,
+               output_mlp: dict = None
+               ):
+    r"""Make `INorp <https://arxiv.org/abs/1612.00222>`_ graph network via functional API.
+
+    Default parameters can be found in :obj:`kgcnn.literature.INorp.model_default` .
+
+    Inputs:
+        list: `[node_attributes, edge_attributes, edge_indices, state_attributes]`
+
+            - node_attributes (tf.RaggedTensor): Node attributes of shape `(batch, None, F)` or `(batch, None)`
+              using an embedding layer.
+            - edge_attributes (tf.RaggedTensor): Edge attributes of shape `(batch, None, F)` or `(batch, None)`
+              using an embedding layer.
+            - edge_indices (tf.RaggedTensor): Index list for edges of shape `(batch, None, 2)`.
+            - state_attributes (tf.Tensor): Environment or graph state attributes of shape `(batch, F)` or `(batch,)`
+              using an embedding layer.
+
+    Outputs:
+        tf.Tensor: Graph embeddings of shape `(batch, L)` if :obj:`output_embedding="graph"`.
+
+    Args:
+        inputs (list): List of dictionaries unpacked in :obj:`tf.keras.layers.Input`. Order must match model definition.
+        input_embedding (dict): Dictionary of embedding arguments for nodes etc. unpacked in :obj:`Embedding` layers.
+        depth (int): Number of graph embedding units or depth of the network.
+        gather_args (dict): Dictionary of layer arguments unpacked in :obj:`GatherNodes` layer.
+        edge_mlp_args (dict): Dictionary of layer arguments unpacked in :obj:`MLP` layer for edge updates.
+        node_mlp_args (dict): Dictionary of layer arguments unpacked in :obj:`MLP` layer for node updates.
+        set2set_args (dict): Dictionary of layer arguments unpacked in :obj:`PoolingSet2SetEncoder` layer.
+        pooling_args (dict): Dictionary of layer arguments unpacked in :obj:`PoolingLocalEdges`, :obj:`PoolingNodes`
+            layer.
+        use_set2set (bool): Whether to use :obj:`PoolingSet2SetEncoder` layer.
+        verbose (int): Level of verbosity.
+        name (str): Name of the model.
+        output_embedding (str): Main embedding task for graph network. Either "node", "edge" or "graph".
+        output_to_tensor (bool): Whether to cast model output to :obj:`tf.Tensor`.
+        output_mlp (dict): Dictionary of layer arguments unpacked in the final classification :obj:`MLP` layer block.
+            Defines number of model outputs and activation.
+
+    Returns:
+        :obj:`tf.keras.models.Model`
+    """
+    # Make input
+    node_input = ks.layers.Input(**inputs[0])
+    edge_input = ks.layers.Input(**inputs[1])
+    edge_index_input = ks.layers.Input(**inputs[2])
+    env_input = ks.Input(**inputs[3])
+
+    # embedding, if no feature dimension
+    n = OptionalInputEmbedding(**input_embedding['node'],
+                               use_embedding=len(inputs[0]['shape']) < 2)(node_input)
+    ed = OptionalInputEmbedding(**input_embedding['edge'],
+                                use_embedding=len(inputs[1]['shape']) < 2)(edge_input)
+    uenv = OptionalInputEmbedding(**input_embedding['graph'],
+                                  use_embedding=len(inputs[3]['shape']) < 1)(env_input)
+    edi = edge_index_input
+
+    # Model
+    ev = GatherState(**gather_args)([uenv, n])
+    # n-Layer Step
+    for i in range(0, depth):
+        # upd = GatherNodes()([n,edi])
+        eu1 = GatherNodesIngoing(**gather_args)([n, edi])
+        eu2 = GatherNodesOutgoing(**gather_args)([n, edi])
+        upd = LazyConcatenate(axis=-1)([eu2, eu1])
+        eu = LazyConcatenate(axis=-1)([upd, ed])
+
+        eu = GraphMLP(**edge_mlp_args)(eu)
+        # Pool message
+        nu = PoolingLocalEdges(**pooling_args)(
+            [n, eu, edi])  # Summing for each node connection
+        # Add environment
+        nu = LazyConcatenate(axis=-1)(
+            [n, nu, ev])  # LazyConcatenate node features with new edge updates
+        n = GraphMLP(**node_mlp_args)(nu)
+
+    # Output embedding choice
+    if output_embedding == 'graph':
+        if use_set2set:
+            # output
+            n = Dense(set2set_args["channels"], activation="linear")(n)
+            out = PoolingSet2SetEncoder(**set2set_args)(n)
+        else:
+            out = PoolingNodes(**pooling_args)(n)
+        out = ks.layers.Flatten()(out)
+        out = MLP(**output_mlp)(out)
+    elif output_embedding == 'node':
+        out = GraphMLP(**output_mlp)(n)
+        if output_to_tensor:  # For tf version < 2.8 cast to tensor below.
+            out = ChangeTensorType(input_tensor_type="ragged", output_tensor_type="tensor")(out)
+    else:
+        raise ValueError("Unsupported output embedding for mode `INorp`")
+
+    model = ks.models.Model(inputs=[node_input, edge_input, edge_index_input, env_input], outputs=out)
+
+    model.__kgcnn_model_version__ = __model_version__
+    return model
```

### Comparing `kgcnn-2.2.4/kgcnn/literature/MAT.py` & `kgcnn-3.0.0/kgcnn/literature/MAT/_make.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import tensorflow as tf
 from typing import Union
 from kgcnn.layers.modules import OptionalInputEmbedding
 from kgcnn.layers.casting import ChangeTensorType, CastEdgeIndicesToDenseAdjacency
 from kgcnn.layers.mlp import GraphMLP, MLP
 from kgcnn.model.utils import update_model_kwargs
-from kgcnn.layers.conv.mat_conv import MATAttentionHead, MATDistanceMatrix, MATReduceMask, MATGlobalPool, MATExpandMask
+from ._mat_conv import MATAttentionHead, MATDistanceMatrix, MATReduceMask, MATGlobalPool, MATExpandMask
 
 ks = tf.keras
 
 # Keep track of model version from commit date in literature.
 # To be updated if model is changed in a significant way.
 __model_version__ = "2022.11.25"
```

### Comparing `kgcnn-2.2.4/kgcnn/literature/MEGAN.py` & `kgcnn-3.0.0/kgcnn/literature/MEGAN/_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,30 +4,31 @@
 import tensorflow as tf
 
 from tensorflow.python.keras.engine import compile_utils
 from kgcnn.layers.base import GraphBaseLayer
 from kgcnn.layers.modules import Dense, OptionalInputEmbedding
 from kgcnn.layers.modules import Activation, Dropout
 from kgcnn.layers.modules import LazyConcatenate, LazyAverage
-from kgcnn.layers.conv.gat_conv import MultiHeadGATV2Layer
+from kgcnn.layers.attention import MultiHeadGATV2Layer
 from kgcnn.layers.pooling import PoolingLocalEdges
 from kgcnn.layers.pooling import PoolingWeightedNodes, PoolingNodes
-from kgcnn.xai.base import ImportanceExplanationMixin
+from kgcnn.literature.GNNExplain._xai._base import ImportanceExplanationMixin
 
 ks = tf.keras
 
-# Keep track of model version from commit date in literature.
-# To be updated if model is changed in a significant way.
-__model_version__ = "2022.12.15"
-
 
 def shifted_sigmoid(x, shift=5, multiplier=1):
     return ks.backend.sigmoid((x - shift) / multiplier)
 
 
+# Keep track of model version from commit date in literature.
+# To be updated if model is changed in a significant way.
+__model_version__ = "2022.12.15"
+
+
 class ExplanationSparsityRegularization(GraphBaseLayer):
 
     def __init__(self,
                  factor: float = 1.0,
                  **kwargs):
         super(ExplanationSparsityRegularization, self).__init__(**kwargs)
         self.factor = factor
@@ -463,32 +464,7 @@
 
     def explain_importances(self,
                             x: t.Sequence[tf.Tensor],
                             **kwargs
                             ) -> t.Tuple[tf.RaggedTensor, tf.RaggedTensor]:
         y, node_importances, edge_importances = self(x, return_importances=True)
         return node_importances, edge_importances
-
-
-def make_model(inputs: t.Optional[list] = None,
-               **kwargs
-               ):
-    r"""Functional model definition of MEGAN. Please check documentation of :obj:`kgcnn.literature.MEGAN` .
-
-    Args:
-        inputs (list): List of dictionaries unpacked in :obj:`tf.keras.layers.Input`. Order must match model definition.
-        kwargs: Kwargs for MEGAN model. Please check documentation of :obj:`kgcnn.literature.MEGAN` .
-
-    Returns:
-        :obj:`tf.keras.models.Model`
-    """
-    # Building the actual model
-    megan = MEGAN(**kwargs)
-
-    # Wrapping the actual model inside a keras functional model to be able to account for the input shapes
-    # definitions which are provided.
-    layer_inputs = [ks.layers.Input(**kwargs) for kwargs in inputs]
-    outputs = megan(layer_inputs)
-    model = ks.models.Model(inputs=layer_inputs, outputs=outputs)
-
-    model.__kgcnn_model_version__ = __model_version__
-    return model
```

### Comparing `kgcnn-2.2.4/kgcnn/literature/MXMNet.py` & `kgcnn-3.0.0/kgcnn/literature/MXMNet/_make.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import tensorflow as tf
 from kgcnn.layers.casting import ChangeTensorType
-from kgcnn.layers.geom import NodeDistanceEuclidean, EdgeAngle, BesselBasisLayer, NodePosition, ShiftPeriodicLattice
-from kgcnn.layers.modules import Dense, OptionalInputEmbedding, LazyConcatenate, LazySubtract, LazyAdd
+from kgcnn.layers.geom import NodeDistanceEuclidean, EdgeAngle, BesselBasisLayer, NodePosition
+from kgcnn.layers.modules import OptionalInputEmbedding, LazyConcatenate, LazySubtract, LazyAdd
 from kgcnn.layers.mlp import GraphMLP, MLP
 from kgcnn.layers.pooling import PoolingNodes
 from kgcnn.model.utils import update_model_kwargs
-from kgcnn.layers.conv.dimenet_conv import SphericalBasisLayer, EmbeddingDimeBlock
-from kgcnn.layers.conv.mxmnet_conv import MXMGlobalMP, MXMLocalMP
+from kgcnn.literature.DimeNetPP._dimenet_conv import SphericalBasisLayer, EmbeddingDimeBlock
+from ._mxmnet_conv import MXMGlobalMP, MXMLocalMP
 
 ks = tf.keras
 
 # Keep track of model version from commit date in literature.
 # To be updated if model is changed in a significant way.
 __model_version__ = "2022.11.25"
```

### Comparing `kgcnn-2.2.4/kgcnn/literature/Megnet.py` & `kgcnn-3.0.0/kgcnn/literature/Megnet/_make.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,374 +1,374 @@
-import tensorflow as tf
-from kgcnn.layers.conv.megnet_conv import MEGnetBlock
-from kgcnn.layers.geom import NodeDistanceEuclidean, GaussBasisLayer, NodePosition, ShiftPeriodicLattice
-from kgcnn.layers.modules import Dense, LazyAdd, Dropout, OptionalInputEmbedding
-from kgcnn.layers.mlp import GraphMLP, MLP
-from kgcnn.layers.pooling import PoolingGlobalEdges, PoolingNodes
-from kgcnn.layers.pool.set2set import PoolingSet2Set
-from kgcnn.model.utils import update_model_kwargs
-
-# from kgcnn.layers.casting import ChangeTensorType
-ks = tf.keras
-
-# Keep track of model version from commit date in literature.
-# To be updated if model is changed in a significant way.
-__model_version__ = "2022.11.25"
-
-
-# Implementation of Megnet in `tf.keras` from paper:
-# Graph Networks as a Universal Machine Learning Framework for Molecules and Crystals
-# by Chi Chen, Weike Ye, Yunxing Zuo, Chen Zheng, and Shyue Ping Ong*
-# https://github.com/materialsvirtuallab/megnet
-# https://pubs.acs.org/doi/10.1021/acs.chemmater.9b01294
-
-
-model_default = {
-    "name": "Megnet",
-    "inputs": [{"shape": (None,), "name": "node_attributes", "dtype": "float32", "ragged": True},
-               {"shape": (None, 3), "name": "node_coordinates", "dtype": "float32", "ragged": True},
-               {"shape": (None, 2), "name": "edge_indices", "dtype": "int64", "ragged": True},
-               {"shape": [], "name": "graph_attributes", "dtype": "float32", "ragged": False}],
-    "input_embedding": {"node": {"input_dim": 95, "output_dim": 64},
-                        "graph": {"input_dim": 100, "output_dim": 64}},
-    "make_distance": True, "expand_distance": True,
-    "gauss_args": {"bins": 20, "distance": 4, "offset": 0.0, "sigma": 0.4},
-    "meg_block_args": {"node_embed": [64, 32, 32], "edge_embed": [64, 32, 32],
-                       "env_embed": [64, 32, 32], "activation": "kgcnn>softplus2"},
-    "set2set_args": {"channels": 16, "T": 3, "pooling_method": "sum", "init_qstar": "0"},
-    "node_ff_args": {"units": [64, 32], "activation": "kgcnn>softplus2"},
-    "edge_ff_args": {"units": [64, 32], "activation": "kgcnn>softplus2"},
-    "state_ff_args": {"units": [64, 32], "activation": "kgcnn>softplus2"},
-    "nblocks": 3, "has_ff": True, "dropout": None, "use_set2set": True,
-    "verbose": 10,
-    "output_embedding": "graph",
-    "output_mlp": {"use_bias": [True, True, True], "units": [32, 16, 1],
-                   "activation": ["kgcnn>softplus2", "kgcnn>softplus2", "linear"]}
-}
-
-
-@update_model_kwargs(model_default)
-def make_model(inputs: list = None,
-               input_embedding: dict = None,
-               expand_distance: bool = None,
-               make_distance: bool = None,
-               gauss_args: dict = None,
-               meg_block_args: dict = None,
-               set2set_args: dict = None,
-               node_ff_args: dict = None,
-               edge_ff_args: dict = None,
-               state_ff_args: dict = None,
-               use_set2set: bool = None,
-               nblocks: int = None,
-               has_ff: bool = None,
-               dropout: float = None,
-               name: str = None,
-               verbose: int = None,
-               output_embedding: str = None,
-               output_mlp: dict = None
-               ):
-    r"""Make `MegNet <https://pubs.acs.org/doi/10.1021/acs.chemmater.9b01294>`_ graph network via functional API.
-    Default parameters can be found in :obj:`kgcnn.literature.Megnet.model_default`.
-
-    Inputs:
-        list: `[node_attributes, edge_distance, edge_indices, state_attributes]`
-        or `[node_attributes, node_coordinates, edge_indices, state_attributes]` if :obj:`make_distance=True` and
-        :obj:`expand_distance=True` to compute edge distances from node coordinates within the model.
-
-            - node_attributes (tf.RaggedTensor): Node attributes of shape `(batch, None, F)` or `(batch, None)`
-              using an embedding layer.
-            - edge_distance (tf.RaggedTensor): Edge attributes or distance of shape `(batch, None, D)` expanded
-              in a basis of dimension `D` or `(batch, None, 1)` if using a :obj:`GaussBasisLayer` layer
-              with model argument :obj:`expand_distance=True` and the numeric distance between nodes.
-            - edge_indices (tf.RaggedTensor): Index list for edges of shape `(batch, None, 2)`.
-            - state_attributes (tf.Tensor): Environment or graph state attributes of shape `(batch, F)` or `(batch,)`
-              using an embedding layer.
-            - node_coordinates (tf.RaggedTensor): Node (atomic) coordinates of shape `(batch, None, 3)`.
-
-    Outputs:
-        tf.Tensor: Graph embeddings of shape `(batch, L)` if :obj:`output_embedding="graph"`.
-
-    Args:
-        inputs (list): List of dictionaries unpacked in :obj:`tf.keras.layers.Input`. Order must match model definition.
-        input_embedding (dict): Dictionary of embedding arguments for nodes etc. unpacked in :obj:`Embedding` layers.
-        make_distance (bool): Whether input is distance or coordinates at in place of edges.
-        expand_distance (bool): If the edge input are actual edges or node coordinates instead that are expanded to
-            form edges with a gauss distance basis given edge indices. Expansion uses `gauss_args`.
-        gauss_args (dict): Dictionary of layer arguments unpacked in :obj:`GaussBasisLayer` layer.
-        meg_block_args (dict): Dictionary of layer arguments unpacked in :obj:`MEGnetBlock` layer.
-        set2set_args (dict): Dictionary of layer arguments unpacked in `:obj:PoolingSet2Set` layer.
-        node_ff_args (dict): Dictionary of layer arguments unpacked in :obj:`MLP` feed-forward layer.
-        edge_ff_args (dict): Dictionary of layer arguments unpacked in :obj:`MLP` feed-forward layer.
-        state_ff_args (dict): Dictionary of layer arguments unpacked in :obj:`MLP` feed-forward layer.
-        use_set2set (bool): Whether to use :obj:`PoolingSet2Set` layer.
-        nblocks (int): Number of graph embedding blocks or depth of the network.
-        has_ff (bool): Use feed-forward MLP in each block.
-        dropout (int): Dropout to use. Default is None.
-        name (str): Name of the model.
-        verbose (int): Verbosity level of print.
-        output_embedding (str): Main embedding task for graph network. Either "node", "edge" or "graph".
-        output_mlp (dict): Dictionary of layer arguments unpacked in the final classification :obj:`MLP` layer block.
-            Defines number of model outputs and activation.
-
-    Returns:
-        :obj:`tf.keras.models.Model`
-    """
-    # Make input
-    node_input = ks.layers.Input(**inputs[0])
-    xyz_input = ks.layers.Input(**inputs[1])
-    edge_index_input = ks.layers.Input(**inputs[2])
-    env_input = ks.Input(**inputs[3])
-
-    # embedding, if no feature dimension
-    n = OptionalInputEmbedding(**input_embedding['node'],
-                               use_embedding=len(inputs[0]['shape']) < 2)(node_input)
-    uenv = OptionalInputEmbedding(**input_embedding['graph'],
-                                  use_embedding=len(inputs[3]['shape']) < 1)(env_input)
-    edi = edge_index_input
-
-    # Edge distance as Gauss-Basis
-    if make_distance:
-        x = xyz_input
-        pos1, pos2 = NodePosition()([x, edi])
-        ed = NodeDistanceEuclidean()([pos1, pos2])
-    else:
-        ed = xyz_input
-
-    if expand_distance:
-        ed = GaussBasisLayer(**gauss_args)(ed)
-
-    # Model
-    vp = n
-    ep = ed
-    up = uenv
-    vp = GraphMLP(**node_ff_args)(vp)
-    ep = GraphMLP(**edge_ff_args)(ep)
-    up = MLP(**state_ff_args)(up)
-    vp2 = vp
-    ep2 = ep
-    up2 = up
-    for i in range(0, nblocks):
-        if has_ff and i > 0:
-            vp2 = GraphMLP(**node_ff_args)(vp)
-            ep2 = GraphMLP(**edge_ff_args)(ep)
-            up2 = MLP(**state_ff_args)(up)
-
-        # MEGnetBlock
-        vp2, ep2, up2 = MEGnetBlock(**meg_block_args)(
-            [vp2, ep2, edi, up2])
-
-        # skip connection
-        if dropout is not None:
-            vp2 = Dropout(dropout, name='dropout_atom_%d' % i)(vp2)
-            ep2 = Dropout(dropout, name='dropout_bond_%d' % i)(ep2)
-            up2 = ks.layers.Dropout(dropout, name='dropout_state_%d' % i)(up2)
-
-        vp = LazyAdd()([vp2, vp])
-        ep = LazyAdd()([ep2, ep])
-        up = ks.layers.Add()([up2, up])
-
-    if use_set2set:
-        vp = Dense(set2set_args["channels"], activation='linear')(vp)  # to match units
-        ep = Dense(set2set_args["channels"], activation='linear')(ep)  # to match units
-        vp = PoolingSet2Set(**set2set_args)(vp)
-        ep = PoolingSet2Set(**set2set_args)(ep)
-    else:
-        vp = PoolingNodes()(vp)
-        ep = PoolingGlobalEdges()(ep)
-
-    ep = ks.layers.Flatten()(ep)
-    vp = ks.layers.Flatten()(vp)
-    final_vec = ks.layers.Concatenate(axis=-1)([vp, ep, up])
-
-    if dropout is not None:
-        final_vec = ks.layers.Dropout(dropout, name='dropout_final')(final_vec)
-
-    # Only graph embedding for Megnet
-    if output_embedding != "graph":
-        raise ValueError("Unsupported output embedding for mode `Megnet`.")
-
-    main_output = MLP(**output_mlp)(final_vec)
-    model = ks.models.Model(inputs=[node_input, xyz_input, edge_index_input, env_input], outputs=main_output)
-
-    model.__kgcnn_model_version__ = __model_version__
-    return model
-
-
-model_crystal_default = {
-    'name': "Megnet",
-    'inputs': [{'shape': (None,), 'name': "node_attributes", 'dtype': 'float32', 'ragged': True},
-               {'shape': (None, 3), 'name': "node_coordinates", 'dtype': 'float32', 'ragged': True},
-               {'shape': (None, 2), 'name': "edge_indices", 'dtype': 'int64', 'ragged': True},
-               {'shape': [1], 'name': "charge", 'dtype': 'float32', 'ragged': False},
-               {'shape': (None, 3), 'name': "edge_image", 'dtype': 'int64', 'ragged': True},
-               {'shape': (3, 3), 'name': "graph_lattice", 'dtype': 'float32', 'ragged': False}],
-    'input_embedding': {"node": {"input_dim": 95, "output_dim": 64},
-                        "graph": {"input_dim": 100, "output_dim": 64}},
-    "make_distance": True, "expand_distance": True,
-    'gauss_args': {"bins": 20, "distance": 4, "offset": 0.0, "sigma": 0.4},
-    'meg_block_args': {'node_embed': [64, 32, 32], 'edge_embed': [64, 32, 32],
-                       'env_embed': [64, 32, 32], 'activation': 'kgcnn>softplus2'},
-    'set2set_args': {'channels': 16, 'T': 3, "pooling_method": "sum", "init_qstar": "0"},
-    'node_ff_args': {"units": [64, 32], "activation": "kgcnn>softplus2"},
-    'edge_ff_args': {"units": [64, 32], "activation": "kgcnn>softplus2"},
-    'state_ff_args': {"units": [64, 32], "activation": "kgcnn>softplus2"},
-    'nblocks': 3, 'has_ff': True, 'dropout': None, 'use_set2set': True,
-    'verbose': 10,
-    'output_embedding': 'graph',
-    'output_mlp': {"use_bias": [True, True, True], "units": [32, 16, 1],
-                   "activation": ['kgcnn>softplus2', 'kgcnn>softplus2', 'linear']}
-}
-
-
-@update_model_kwargs(model_crystal_default)
-def make_crystal_model(inputs: list = None,
-                       input_embedding: dict = None,
-                       expand_distance: bool = None,
-                       make_distance: bool = None,
-                       gauss_args: dict = None,
-                       meg_block_args: dict = None,
-                       set2set_args: dict = None,
-                       node_ff_args: dict = None,
-                       edge_ff_args: dict = None,
-                       state_ff_args: dict = None,
-                       use_set2set: bool = None,
-                       nblocks: int = None,
-                       has_ff: bool = None,
-                       dropout: float = None,
-                       name: str = None,
-                       verbose: int = None,
-                       output_embedding: str = None,
-                       output_mlp: dict = None
-                       ):
-    r"""Make `MegNet <https://pubs.acs.org/doi/10.1021/acs.chemmater.9b01294>`_ graph network via functional API.
-    Default parameters can be found in :obj:`kgcnn.literature.Megnet.model_crystal_default`.
-
-    Inputs:
-        list: `[node_attributes, edge_distance, edge_indices, state_attributes, edge_image, lattice]`
-        or `[node_attributes, node_coordinates, edge_indices, state_attributes, edge_image, lattice]`
-        if :obj:`make_distance=True` and :obj:`expand_distance=True` to compute edge distances
-        from node coordinates within the model.
-
-            - node_attributes (tf.RaggedTensor): Node attributes of shape `(batch, None, F)` or `(batch, None)`
-              using an embedding layer.
-            - edge_distance (tf.RaggedTensor): Edge distance of shape `(batch, None, D)` expanded
-              in a basis of dimension `D` or `(batch, None, 1)` if using a :obj:`GaussBasisLayer` layer
-              with model argument :obj:`expand_distance=True` and the numeric distance between nodes.
-            - edge_indices (tf.RaggedTensor): Index list for edges of shape `(batch, None, 2)`.
-            - node_coordinates (tf.RaggedTensor): Node (atomic) coordinates of shape `(batch, None, 3)`.
-            - lattice (tf.Tensor): Lattice matrix of the periodic structure of shape `(batch, 3, 3)`.
-            - edge_image (tf.RaggedTensor): Indices of the periodic image the sending node is located. The indices
-                of and edge are :math:`(i, j)` with :math:`j` being the sending node.
-            - state_attributes (tf.Tensor): Environment or graph state attributes of shape `(batch, F)` or `(batch,)`
-                using an embedding layer.
-
-    Outputs:
-        tf.Tensor: Graph embeddings of shape `(batch, L)` if :obj:`output_embedding="graph"`.
-
-    Args:
-        inputs (list): List of dictionaries unpacked in :obj:`tf.keras.layers.Input`. Order must match model definition.
-        input_embedding (dict): Dictionary of embedding arguments for nodes etc. unpacked in :obj:`Embedding` layers.
-        make_distance (bool): Whether input is distance or coordinates at in place of edges.
-        expand_distance (bool): If the edge input are actual edges or node coordinates instead that are expanded to
-            form edges with a gauss distance basis given edge indices. Expansion uses `gauss_args`.
-        gauss_args (dict): Dictionary of layer arguments unpacked in :obj:`GaussBasisLayer` layer.
-        meg_block_args (dict): Dictionary of layer arguments unpacked in :obj:`MEGnetBlock` layer.
-        set2set_args (dict): Dictionary of layer arguments unpacked in `:obj:PoolingSet2Set` layer.
-        node_ff_args (dict): Dictionary of layer arguments unpacked in :obj:`MLP` feed-forward layer.
-        edge_ff_args (dict): Dictionary of layer arguments unpacked in :obj:`MLP` feed-forward layer.
-        state_ff_args (dict): Dictionary of layer arguments unpacked in :obj:`MLP` feed-forward layer.
-        use_set2set (bool): Whether to use :obj:`PoolingSet2Set` layer.
-        nblocks (int): Number of graph embedding blocks or depth of the network.
-        has_ff (bool): Use feed-forward MLP in each block.
-        dropout (int): Dropout to use. Default is None.
-        name (str): Name of the model.
-        verbose (int): Verbosity level of print.
-        output_embedding (str): Main embedding task for graph network. Either "node", "edge" or "graph".
-        output_mlp (dict): Dictionary of layer arguments unpacked in the final classification :obj:`MLP` layer block.
-            Defines number of model outputs and activation.
-
-    Returns:
-        :obj:`tf.keras.models.Model`
-    """
-    # Make input
-    node_input = ks.layers.Input(**inputs[0])
-    xyz_input = ks.layers.Input(**inputs[1])
-    edge_index_input = ks.layers.Input(**inputs[2])
-    env_input = ks.Input(**inputs[3])
-    edge_image = ks.layers.Input(**inputs[4])
-    lattice = ks.layers.Input(**inputs[5])
-
-    # embedding, if no feature dimension
-    n = OptionalInputEmbedding(**input_embedding['node'],
-                               use_embedding=len(inputs[0]['shape']) < 2)(node_input)
-    uenv = OptionalInputEmbedding(**input_embedding['graph'],
-                                  use_embedding=len(inputs[3]['shape']) < 1)(env_input)
-    edi = edge_index_input
-
-    # Edge distance as Gauss-Basis
-    if make_distance:
-        x = xyz_input
-        pos1, pos2 = NodePosition()([x, edi])
-        pos2 = ShiftPeriodicLattice()([pos2, edge_image, lattice])
-        ed = NodeDistanceEuclidean()([pos1, pos2])
-    else:
-        ed = xyz_input
-
-    if expand_distance:
-        ed = GaussBasisLayer(**gauss_args)(ed)
-
-    # Model
-    vp = n
-    ep = ed
-    up = uenv
-    vp = GraphMLP(**node_ff_args)(vp)
-    ep = GraphMLP(**edge_ff_args)(ep)
-    up = MLP(**state_ff_args)(up)
-    vp2 = vp
-    ep2 = ep
-    up2 = up
-    for i in range(0, nblocks):
-        if has_ff and i > 0:
-            vp2 = GraphMLP(**node_ff_args)(vp)
-            ep2 = GraphMLP(**edge_ff_args)(ep)
-            up2 = MLP(**state_ff_args)(up)
-
-        # MEGnetBlock
-        vp2, ep2, up2 = MEGnetBlock(**meg_block_args)(
-            [vp2, ep2, edi, up2])
-
-        # skip connection
-        if dropout is not None:
-            vp2 = Dropout(dropout, name='dropout_atom_%d' % i)(vp2)
-            ep2 = Dropout(dropout, name='dropout_bond_%d' % i)(ep2)
-            up2 = ks.layers.Dropout(dropout, name='dropout_state_%d' % i)(up2)
-
-        vp = LazyAdd()([vp2, vp])
-        ep = LazyAdd()([ep2, ep])
-        up = ks.layers.Add()([up2, up])
-
-    if use_set2set:
-        vp = Dense(set2set_args["channels"], activation='linear')(vp)  # to match units
-        ep = Dense(set2set_args["channels"], activation='linear')(ep)  # to match units
-        vp = PoolingSet2Set(**set2set_args)(vp)
-        ep = PoolingSet2Set(**set2set_args)(ep)
-    else:
-        vp = PoolingNodes()(vp)
-        ep = PoolingGlobalEdges()(ep)
-
-    ep = ks.layers.Flatten()(ep)
-    vp = ks.layers.Flatten()(vp)
-    final_vec = ks.layers.Concatenate(axis=-1)([vp, ep, up])
-
-    if dropout is not None:
-        final_vec = ks.layers.Dropout(dropout, name='dropout_final')(final_vec)
-
-    # Only graph embedding for Megnet
-    if output_embedding != "graph":
-        raise ValueError("Unsupported output embedding for mode `Megnet`.")
-
-    main_output = MLP(**output_mlp)(final_vec)
-    model = ks.models.Model(inputs=[node_input, xyz_input, edge_index_input, env_input, edge_image, lattice],
-                            outputs=main_output)
-
-    model.__kgcnn_model_version__ = __model_version__
-    return model
+import tensorflow as tf
+from ._megnet_conv import MEGnetBlock
+from kgcnn.layers.geom import NodeDistanceEuclidean, GaussBasisLayer, NodePosition, ShiftPeriodicLattice
+from kgcnn.layers.modules import Dense, LazyAdd, Dropout, OptionalInputEmbedding
+from kgcnn.layers.mlp import GraphMLP, MLP
+from kgcnn.layers.pooling import PoolingGlobalEdges, PoolingNodes
+from kgcnn.layers.set2set import PoolingSet2SetEncoder
+from kgcnn.model.utils import update_model_kwargs
+
+# from kgcnn.layers.casting import ChangeTensorType
+ks = tf.keras
+
+# Keep track of model version from commit date in literature.
+# To be updated if model is changed in a significant way.
+__model_version__ = "2022.11.25"
+
+
+# Implementation of Megnet in `tf.keras` from paper:
+# Graph Networks as a Universal Machine Learning Framework for Molecules and Crystals
+# by Chi Chen, Weike Ye, Yunxing Zuo, Chen Zheng, and Shyue Ping Ong*
+# https://github.com/materialsvirtuallab/megnet
+# https://pubs.acs.org/doi/10.1021/acs.chemmater.9b01294
+
+
+model_default = {
+    "name": "Megnet",
+    "inputs": [{"shape": (None,), "name": "node_attributes", "dtype": "float32", "ragged": True},
+               {"shape": (None, 3), "name": "node_coordinates", "dtype": "float32", "ragged": True},
+               {"shape": (None, 2), "name": "edge_indices", "dtype": "int64", "ragged": True},
+               {"shape": [], "name": "graph_attributes", "dtype": "float32", "ragged": False}],
+    "input_embedding": {"node": {"input_dim": 95, "output_dim": 64},
+                        "graph": {"input_dim": 100, "output_dim": 64}},
+    "make_distance": True, "expand_distance": True,
+    "gauss_args": {"bins": 20, "distance": 4, "offset": 0.0, "sigma": 0.4},
+    "meg_block_args": {"node_embed": [64, 32, 32], "edge_embed": [64, 32, 32],
+                       "env_embed": [64, 32, 32], "activation": "kgcnn>softplus2"},
+    "set2set_args": {"channels": 16, "T": 3, "pooling_method": "sum", "init_qstar": "0"},
+    "node_ff_args": {"units": [64, 32], "activation": "kgcnn>softplus2"},
+    "edge_ff_args": {"units": [64, 32], "activation": "kgcnn>softplus2"},
+    "state_ff_args": {"units": [64, 32], "activation": "kgcnn>softplus2"},
+    "nblocks": 3, "has_ff": True, "dropout": None, "use_set2set": True,
+    "verbose": 10,
+    "output_embedding": "graph",
+    "output_mlp": {"use_bias": [True, True, True], "units": [32, 16, 1],
+                   "activation": ["kgcnn>softplus2", "kgcnn>softplus2", "linear"]}
+}
+
+
+@update_model_kwargs(model_default)
+def make_model(inputs: list = None,
+               input_embedding: dict = None,
+               expand_distance: bool = None,
+               make_distance: bool = None,
+               gauss_args: dict = None,
+               meg_block_args: dict = None,
+               set2set_args: dict = None,
+               node_ff_args: dict = None,
+               edge_ff_args: dict = None,
+               state_ff_args: dict = None,
+               use_set2set: bool = None,
+               nblocks: int = None,
+               has_ff: bool = None,
+               dropout: float = None,
+               name: str = None,
+               verbose: int = None,
+               output_embedding: str = None,
+               output_mlp: dict = None
+               ):
+    r"""Make `MegNet <https://pubs.acs.org/doi/10.1021/acs.chemmater.9b01294>`_ graph network via functional API.
+    Default parameters can be found in :obj:`kgcnn.literature.Megnet.model_default`.
+
+    Inputs:
+        list: `[node_attributes, edge_distance, edge_indices, state_attributes]`
+        or `[node_attributes, node_coordinates, edge_indices, state_attributes]` if :obj:`make_distance=True` and
+        :obj:`expand_distance=True` to compute edge distances from node coordinates within the model.
+
+            - node_attributes (tf.RaggedTensor): Node attributes of shape `(batch, None, F)` or `(batch, None)`
+              using an embedding layer.
+            - edge_distance (tf.RaggedTensor): Edge attributes or distance of shape `(batch, None, D)` expanded
+              in a basis of dimension `D` or `(batch, None, 1)` if using a :obj:`GaussBasisLayer` layer
+              with model argument :obj:`expand_distance=True` and the numeric distance between nodes.
+            - edge_indices (tf.RaggedTensor): Index list for edges of shape `(batch, None, 2)`.
+            - state_attributes (tf.Tensor): Environment or graph state attributes of shape `(batch, F)` or `(batch,)`
+              using an embedding layer.
+            - node_coordinates (tf.RaggedTensor): Node (atomic) coordinates of shape `(batch, None, 3)`.
+
+    Outputs:
+        tf.Tensor: Graph embeddings of shape `(batch, L)` if :obj:`output_embedding="graph"`.
+
+    Args:
+        inputs (list): List of dictionaries unpacked in :obj:`tf.keras.layers.Input`. Order must match model definition.
+        input_embedding (dict): Dictionary of embedding arguments for nodes etc. unpacked in :obj:`Embedding` layers.
+        make_distance (bool): Whether input is distance or coordinates at in place of edges.
+        expand_distance (bool): If the edge input are actual edges or node coordinates instead that are expanded to
+            form edges with a gauss distance basis given edge indices. Expansion uses `gauss_args`.
+        gauss_args (dict): Dictionary of layer arguments unpacked in :obj:`GaussBasisLayer` layer.
+        meg_block_args (dict): Dictionary of layer arguments unpacked in :obj:`MEGnetBlock` layer.
+        set2set_args (dict): Dictionary of layer arguments unpacked in `:obj:PoolingSet2SetEncoder` layer.
+        node_ff_args (dict): Dictionary of layer arguments unpacked in :obj:`MLP` feed-forward layer.
+        edge_ff_args (dict): Dictionary of layer arguments unpacked in :obj:`MLP` feed-forward layer.
+        state_ff_args (dict): Dictionary of layer arguments unpacked in :obj:`MLP` feed-forward layer.
+        use_set2set (bool): Whether to use :obj:`PoolingSet2SetEncoder` layer.
+        nblocks (int): Number of graph embedding blocks or depth of the network.
+        has_ff (bool): Use feed-forward MLP in each block.
+        dropout (int): Dropout to use. Default is None.
+        name (str): Name of the model.
+        verbose (int): Verbosity level of print.
+        output_embedding (str): Main embedding task for graph network. Either "node", "edge" or "graph".
+        output_mlp (dict): Dictionary of layer arguments unpacked in the final classification :obj:`MLP` layer block.
+            Defines number of model outputs and activation.
+
+    Returns:
+        :obj:`tf.keras.models.Model`
+    """
+    # Make input
+    node_input = ks.layers.Input(**inputs[0])
+    xyz_input = ks.layers.Input(**inputs[1])
+    edge_index_input = ks.layers.Input(**inputs[2])
+    env_input = ks.Input(**inputs[3])
+
+    # embedding, if no feature dimension
+    n = OptionalInputEmbedding(**input_embedding['node'],
+                               use_embedding=len(inputs[0]['shape']) < 2)(node_input)
+    uenv = OptionalInputEmbedding(**input_embedding['graph'],
+                                  use_embedding=len(inputs[3]['shape']) < 1)(env_input)
+    edi = edge_index_input
+
+    # Edge distance as Gauss-Basis
+    if make_distance:
+        x = xyz_input
+        pos1, pos2 = NodePosition()([x, edi])
+        ed = NodeDistanceEuclidean()([pos1, pos2])
+    else:
+        ed = xyz_input
+
+    if expand_distance:
+        ed = GaussBasisLayer(**gauss_args)(ed)
+
+    # Model
+    vp = n
+    ep = ed
+    up = uenv
+    vp = GraphMLP(**node_ff_args)(vp)
+    ep = GraphMLP(**edge_ff_args)(ep)
+    up = MLP(**state_ff_args)(up)
+    vp2 = vp
+    ep2 = ep
+    up2 = up
+    for i in range(0, nblocks):
+        if has_ff and i > 0:
+            vp2 = GraphMLP(**node_ff_args)(vp)
+            ep2 = GraphMLP(**edge_ff_args)(ep)
+            up2 = MLP(**state_ff_args)(up)
+
+        # MEGnetBlock
+        vp2, ep2, up2 = MEGnetBlock(**meg_block_args)(
+            [vp2, ep2, edi, up2])
+
+        # skip connection
+        if dropout is not None:
+            vp2 = Dropout(dropout, name='dropout_atom_%d' % i)(vp2)
+            ep2 = Dropout(dropout, name='dropout_bond_%d' % i)(ep2)
+            up2 = ks.layers.Dropout(dropout, name='dropout_state_%d' % i)(up2)
+
+        vp = LazyAdd()([vp2, vp])
+        ep = LazyAdd()([ep2, ep])
+        up = ks.layers.Add()([up2, up])
+
+    if use_set2set:
+        vp = Dense(set2set_args["channels"], activation='linear')(vp)  # to match units
+        ep = Dense(set2set_args["channels"], activation='linear')(ep)  # to match units
+        vp = PoolingSet2SetEncoder(**set2set_args)(vp)
+        ep = PoolingSet2SetEncoder(**set2set_args)(ep)
+    else:
+        vp = PoolingNodes()(vp)
+        ep = PoolingGlobalEdges()(ep)
+
+    ep = ks.layers.Flatten()(ep)
+    vp = ks.layers.Flatten()(vp)
+    final_vec = ks.layers.Concatenate(axis=-1)([vp, ep, up])
+
+    if dropout is not None:
+        final_vec = ks.layers.Dropout(dropout, name='dropout_final')(final_vec)
+
+    # Only graph embedding for Megnet
+    if output_embedding != "graph":
+        raise ValueError("Unsupported output embedding for mode `Megnet`.")
+
+    main_output = MLP(**output_mlp)(final_vec)
+    model = ks.models.Model(inputs=[node_input, xyz_input, edge_index_input, env_input], outputs=main_output)
+
+    model.__kgcnn_model_version__ = __model_version__
+    return model
+
+
+model_crystal_default = {
+    'name': "Megnet",
+    'inputs': [{'shape': (None,), 'name': "node_attributes", 'dtype': 'float32', 'ragged': True},
+               {'shape': (None, 3), 'name': "node_coordinates", 'dtype': 'float32', 'ragged': True},
+               {'shape': (None, 2), 'name': "edge_indices", 'dtype': 'int64', 'ragged': True},
+               {'shape': [1], 'name': "charge", 'dtype': 'float32', 'ragged': False},
+               {'shape': (None, 3), 'name': "edge_image", 'dtype': 'int64', 'ragged': True},
+               {'shape': (3, 3), 'name': "graph_lattice", 'dtype': 'float32', 'ragged': False}],
+    'input_embedding': {"node": {"input_dim": 95, "output_dim": 64},
+                        "graph": {"input_dim": 100, "output_dim": 64}},
+    "make_distance": True, "expand_distance": True,
+    'gauss_args': {"bins": 20, "distance": 4, "offset": 0.0, "sigma": 0.4},
+    'meg_block_args': {'node_embed': [64, 32, 32], 'edge_embed': [64, 32, 32],
+                       'env_embed': [64, 32, 32], 'activation': 'kgcnn>softplus2'},
+    'set2set_args': {'channels': 16, 'T': 3, "pooling_method": "sum", "init_qstar": "0"},
+    'node_ff_args': {"units": [64, 32], "activation": "kgcnn>softplus2"},
+    'edge_ff_args': {"units": [64, 32], "activation": "kgcnn>softplus2"},
+    'state_ff_args': {"units": [64, 32], "activation": "kgcnn>softplus2"},
+    'nblocks': 3, 'has_ff': True, 'dropout': None, 'use_set2set': True,
+    'verbose': 10,
+    'output_embedding': 'graph',
+    'output_mlp': {"use_bias": [True, True, True], "units": [32, 16, 1],
+                   "activation": ['kgcnn>softplus2', 'kgcnn>softplus2', 'linear']}
+}
+
+
+@update_model_kwargs(model_crystal_default)
+def make_crystal_model(inputs: list = None,
+                       input_embedding: dict = None,
+                       expand_distance: bool = None,
+                       make_distance: bool = None,
+                       gauss_args: dict = None,
+                       meg_block_args: dict = None,
+                       set2set_args: dict = None,
+                       node_ff_args: dict = None,
+                       edge_ff_args: dict = None,
+                       state_ff_args: dict = None,
+                       use_set2set: bool = None,
+                       nblocks: int = None,
+                       has_ff: bool = None,
+                       dropout: float = None,
+                       name: str = None,
+                       verbose: int = None,
+                       output_embedding: str = None,
+                       output_mlp: dict = None
+                       ):
+    r"""Make `MegNet <https://pubs.acs.org/doi/10.1021/acs.chemmater.9b01294>`_ graph network via functional API.
+    Default parameters can be found in :obj:`kgcnn.literature.Megnet.model_crystal_default`.
+
+    Inputs:
+        list: `[node_attributes, edge_distance, edge_indices, state_attributes, edge_image, lattice]`
+        or `[node_attributes, node_coordinates, edge_indices, state_attributes, edge_image, lattice]`
+        if :obj:`make_distance=True` and :obj:`expand_distance=True` to compute edge distances
+        from node coordinates within the model.
+
+            - node_attributes (tf.RaggedTensor): Node attributes of shape `(batch, None, F)` or `(batch, None)`
+              using an embedding layer.
+            - edge_distance (tf.RaggedTensor): Edge distance of shape `(batch, None, D)` expanded
+              in a basis of dimension `D` or `(batch, None, 1)` if using a :obj:`GaussBasisLayer` layer
+              with model argument :obj:`expand_distance=True` and the numeric distance between nodes.
+            - edge_indices (tf.RaggedTensor): Index list for edges of shape `(batch, None, 2)`.
+            - node_coordinates (tf.RaggedTensor): Node (atomic) coordinates of shape `(batch, None, 3)`.
+            - lattice (tf.Tensor): Lattice matrix of the periodic structure of shape `(batch, 3, 3)`.
+            - edge_image (tf.RaggedTensor): Indices of the periodic image the sending node is located. The indices
+                of and edge are :math:`(i, j)` with :math:`j` being the sending node.
+            - state_attributes (tf.Tensor): Environment or graph state attributes of shape `(batch, F)` or `(batch,)`
+                using an embedding layer.
+
+    Outputs:
+        tf.Tensor: Graph embeddings of shape `(batch, L)` if :obj:`output_embedding="graph"`.
+
+    Args:
+        inputs (list): List of dictionaries unpacked in :obj:`tf.keras.layers.Input`. Order must match model definition.
+        input_embedding (dict): Dictionary of embedding arguments for nodes etc. unpacked in :obj:`Embedding` layers.
+        make_distance (bool): Whether input is distance or coordinates at in place of edges.
+        expand_distance (bool): If the edge input are actual edges or node coordinates instead that are expanded to
+            form edges with a gauss distance basis given edge indices. Expansion uses `gauss_args`.
+        gauss_args (dict): Dictionary of layer arguments unpacked in :obj:`GaussBasisLayer` layer.
+        meg_block_args (dict): Dictionary of layer arguments unpacked in :obj:`MEGnetBlock` layer.
+        set2set_args (dict): Dictionary of layer arguments unpacked in `:obj:PoolingSet2SetEncoder` layer.
+        node_ff_args (dict): Dictionary of layer arguments unpacked in :obj:`MLP` feed-forward layer.
+        edge_ff_args (dict): Dictionary of layer arguments unpacked in :obj:`MLP` feed-forward layer.
+        state_ff_args (dict): Dictionary of layer arguments unpacked in :obj:`MLP` feed-forward layer.
+        use_set2set (bool): Whether to use :obj:`PoolingSet2SetEncoder` layer.
+        nblocks (int): Number of graph embedding blocks or depth of the network.
+        has_ff (bool): Use feed-forward MLP in each block.
+        dropout (int): Dropout to use. Default is None.
+        name (str): Name of the model.
+        verbose (int): Verbosity level of print.
+        output_embedding (str): Main embedding task for graph network. Either "node", "edge" or "graph".
+        output_mlp (dict): Dictionary of layer arguments unpacked in the final classification :obj:`MLP` layer block.
+            Defines number of model outputs and activation.
+
+    Returns:
+        :obj:`tf.keras.models.Model`
+    """
+    # Make input
+    node_input = ks.layers.Input(**inputs[0])
+    xyz_input = ks.layers.Input(**inputs[1])
+    edge_index_input = ks.layers.Input(**inputs[2])
+    env_input = ks.Input(**inputs[3])
+    edge_image = ks.layers.Input(**inputs[4])
+    lattice = ks.layers.Input(**inputs[5])
+
+    # embedding, if no feature dimension
+    n = OptionalInputEmbedding(**input_embedding['node'],
+                               use_embedding=len(inputs[0]['shape']) < 2)(node_input)
+    uenv = OptionalInputEmbedding(**input_embedding['graph'],
+                                  use_embedding=len(inputs[3]['shape']) < 1)(env_input)
+    edi = edge_index_input
+
+    # Edge distance as Gauss-Basis
+    if make_distance:
+        x = xyz_input
+        pos1, pos2 = NodePosition()([x, edi])
+        pos2 = ShiftPeriodicLattice()([pos2, edge_image, lattice])
+        ed = NodeDistanceEuclidean()([pos1, pos2])
+    else:
+        ed = xyz_input
+
+    if expand_distance:
+        ed = GaussBasisLayer(**gauss_args)(ed)
+
+    # Model
+    vp = n
+    ep = ed
+    up = uenv
+    vp = GraphMLP(**node_ff_args)(vp)
+    ep = GraphMLP(**edge_ff_args)(ep)
+    up = MLP(**state_ff_args)(up)
+    vp2 = vp
+    ep2 = ep
+    up2 = up
+    for i in range(0, nblocks):
+        if has_ff and i > 0:
+            vp2 = GraphMLP(**node_ff_args)(vp)
+            ep2 = GraphMLP(**edge_ff_args)(ep)
+            up2 = MLP(**state_ff_args)(up)
+
+        # MEGnetBlock
+        vp2, ep2, up2 = MEGnetBlock(**meg_block_args)(
+            [vp2, ep2, edi, up2])
+
+        # skip connection
+        if dropout is not None:
+            vp2 = Dropout(dropout, name='dropout_atom_%d' % i)(vp2)
+            ep2 = Dropout(dropout, name='dropout_bond_%d' % i)(ep2)
+            up2 = ks.layers.Dropout(dropout, name='dropout_state_%d' % i)(up2)
+
+        vp = LazyAdd()([vp2, vp])
+        ep = LazyAdd()([ep2, ep])
+        up = ks.layers.Add()([up2, up])
+
+    if use_set2set:
+        vp = Dense(set2set_args["channels"], activation='linear')(vp)  # to match units
+        ep = Dense(set2set_args["channels"], activation='linear')(ep)  # to match units
+        vp = PoolingSet2SetEncoder(**set2set_args)(vp)
+        ep = PoolingSet2SetEncoder(**set2set_args)(ep)
+    else:
+        vp = PoolingNodes()(vp)
+        ep = PoolingGlobalEdges()(ep)
+
+    ep = ks.layers.Flatten()(ep)
+    vp = ks.layers.Flatten()(vp)
+    final_vec = ks.layers.Concatenate(axis=-1)([vp, ep, up])
+
+    if dropout is not None:
+        final_vec = ks.layers.Dropout(dropout, name='dropout_final')(final_vec)
+
+    # Only graph embedding for Megnet
+    if output_embedding != "graph":
+        raise ValueError("Unsupported output embedding for mode `Megnet`.")
+
+    main_output = MLP(**output_mlp)(final_vec)
+    model = ks.models.Model(inputs=[node_input, xyz_input, edge_index_input, env_input, edge_image, lattice],
+                            outputs=main_output)
+
+    model.__kgcnn_model_version__ = __model_version__
+    return model
```

### Comparing `kgcnn-2.2.4/kgcnn/literature/NMPN.py` & `kgcnn-3.0.0/kgcnn/literature/NMPN/_make.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,333 +1,334 @@
-import tensorflow as tf
-from kgcnn.layers.casting import ChangeTensorType
-from kgcnn.layers.conv.mpnn_conv import GRUUpdate, TrafoEdgeNetMessages, MatMulMessages
-from kgcnn.layers.gather import GatherNodesOutgoing, GatherNodesIngoing
-from kgcnn.layers.modules import Dense, LazyConcatenate, OptionalInputEmbedding
-from kgcnn.layers.mlp import GraphMLP, MLP
-from kgcnn.layers.pooling import PoolingLocalEdges, PoolingNodes
-from kgcnn.layers.pool.set2set import PoolingSet2Set
-from kgcnn.model.utils import update_model_kwargs
-from kgcnn.layers.geom import NodePosition, NodeDistanceEuclidean, GaussBasisLayer, ShiftPeriodicLattice
-
-ks = tf.keras
-
-# Keep track of model version from commit date in literature.
-# To be updated if model is changed in a significant way.
-__model_version__ = "2022.11.25"
-
-
-# Implementation of NMPN in `tf.keras` from paper:
-# Neural Message Passing for Quantum Chemistry
-# by Justin Gilmer, Samuel S. Schoenholz, Patrick F. Riley, Oriol Vinyals, George E. Dahl
-# http://arxiv.org/abs/1704.01212    
-
-model_default = {
-    "name": "NMPN",
-    "inputs": [{"shape": (None,), "name": "node_attributes", "dtype": "float32", "ragged": True},
-               {"shape": (None,), "name": "edge_attributes", "dtype": "float32", "ragged": True},
-               {"shape": (None, 2), "name": "edge_indices", "dtype": "int64", "ragged": True}],
-    "input_embedding": {"node": {"input_dim": 95, "output_dim": 64},
-                        "edge": {"input_dim": 5, "output_dim": 64}},
-    "geometric_edge": False, "make_distance": False, "expand_distance": False,
-    "gauss_args": {"bins": 20, "distance": 4, "offset": 0.0, "sigma": 0.4},
-    "set2set_args": {"channels": 32, "T": 3, "pooling_method": "sum",
-                     "init_qstar": "0"},
-    "pooling_args": {"pooling_method": "segment_sum"},
-    "edge_mlp": {"use_bias": True, "activation": "swish", "units": [64, 64, 64]},
-    "use_set2set": True, "depth": 3, "node_dim": 64,
-    "verbose": 10,
-    "output_embedding": 'graph', "output_to_tensor": True,
-    "output_mlp": {"use_bias": [True, True, False], "units": [25, 10, 1],
-                   "activation": ["selu", "selu", "sigmoid"]},
-}
-
-
-@update_model_kwargs(model_default)
-def make_model(inputs: list = None,
-               input_embedding: dict = None,
-               geometric_edge: bool = None,
-               make_distance: bool = None,
-               expand_distance: bool = None,
-               gauss_args: dict = None,
-               set2set_args: dict = None,
-               pooling_args: dict = None,
-               edge_mlp: dict = None,
-               use_set2set: bool = None,
-               node_dim: int = None,
-               depth: int = None,
-               verbose: int = None,
-               name: str = None,
-               output_embedding: str = None,
-               output_to_tensor: bool = None,
-               output_mlp: dict = None
-               ):
-    r"""Make `NMPN <http://arxiv.org/abs/1704.01212>`_ graph network via functional API.
-    Default parameters can be found in :obj:`kgcnn.literature.NMPN.model_default`.
-
-    Inputs:
-        list: `[node_attributes, edge_attributes, edge_indices]`
-        or `[node_attributes, edge_distance, edge_indices]` if :obj:`geometric_edge=True`
-        or `[node_attributes, node_coordinates, edge_indices]` if :obj:`make_distance=True` and
-        :obj:`expand_distance=True` to compute edge distances from node coordinates within the model.
-
-            - node_attributes (tf.RaggedTensor): Node attributes of shape `(batch, None, F)` or `(batch, None)`
-              using an embedding layer.
-            - edge_attributes (tf.RaggedTensor): Edge attributes of shape `(batch, None, F)` or `(batch, None)`
-              using an embedding layer.
-            - edge_distance (tf.RaggedTensor): Edge attributes or distance of shape `(batch, None, D)` expanded
-              in a basis of dimension `D` or `(batch, None, 1)` if using a :obj:`GaussBasisLayer` layer
-              with model argument :obj:`expand_distance=True` and the numeric distance between nodes.
-            - edge_indices (tf.RaggedTensor): Index list for edges of shape `(batch, None, 2)`.
-            - node_coordinates (tf.RaggedTensor): Node (atomic) coordinates of shape `(batch, None, 3)`.
-
-    Outputs:
-        tf.Tensor: Graph embeddings of shape `(batch, L)` if :obj:`output_embedding="graph"`.
-
-    Args:
-        inputs (list): List of dictionaries unpacked in :obj:`tf.keras.layers.Input`. Order must match model definition.
-        input_embedding (dict): Dictionary of embedding arguments for nodes etc. unpacked in :obj:`Embedding` layers.
-        geometric_edge (bool): Whether the edges are geometric, like distance or coordinates.
-        make_distance (bool): Whether input is distance or coordinates at in place of edges.
-        expand_distance (bool): If the edge input are actual edges or node coordinates instead that are expanded to
-            form edges with a gauss distance basis given edge indices. Expansion uses `gauss_args`.
-        gauss_args (dict): Dictionary of layer arguments unpacked in :obj:`GaussBasisLayer` layer.
-        set2set_args (dict): Dictionary of layer arguments unpacked in :obj:`PoolingSet2Set` layer.
-        pooling_args (dict): Dictionary of layer arguments unpacked in :obj:`PoolingNodes`, `PoolingLocalEdges` layers.
-        edge_mlp (dict): Dictionary of layer arguments unpacked in :obj:`MLP` layer for edge matrix.
-        use_set2set (bool): Whether to use :obj:`PoolingSet2Set` layer.
-        node_dim (int): Dimension of hidden node embedding.
-        depth (int): Number of graph embedding units or depth of the network.
-        verbose (int): Level of verbosity.
-        name (str): Name of the model.
-        output_embedding (str): Main embedding task for graph network. Either "node", "edge" or "graph".
-        output_to_tensor (bool): Whether to cast model output to :obj:`tf.Tensor`.
-        output_mlp (dict): Dictionary of layer arguments unpacked in the final classification :obj:`MLP` layer block.
-            Defines number of model outputs and activation.
-
-    Returns:
-        :obj:`tf.keras.models.Model`
-    """
-    # Make input
-    node_input = ks.layers.Input(**inputs[0])
-    edge_input = ks.layers.Input(**inputs[1])  # Or coordinates
-    edge_index_input = ks.layers.Input(**inputs[2])
-    edi = edge_index_input
-
-    # embedding, if no feature dimension
-    n0 = OptionalInputEmbedding(**input_embedding['node'], use_embedding=len(inputs[0]['shape']) < 2)(node_input)
-    if not geometric_edge:
-        ed = OptionalInputEmbedding(**input_embedding['edge'], use_embedding=len(inputs[1]['shape']) < 2)(edge_input)
-    else:
-        ed = edge_input
-
-    # If coordinates are in place of edges
-    if make_distance:
-        pos1, pos2 = NodePosition()([ed, edi])
-        ed = NodeDistanceEuclidean()([pos1, pos2])
-
-    if expand_distance:
-        ed = GaussBasisLayer(**gauss_args)(ed)
-
-    # Make hidden dimension
-    n = Dense(node_dim, activation="linear")(n0)
-
-    # Make edge networks.
-    edge_net_in = GraphMLP(**edge_mlp)(ed)
-    edge_net_in = TrafoEdgeNetMessages(target_shape=(node_dim, node_dim))(edge_net_in)
-    edge_net_out = GraphMLP(**edge_mlp)(ed)
-    edge_net_out = TrafoEdgeNetMessages(target_shape=(node_dim, node_dim))(edge_net_out)
-
-    # Gru for node updates
-    gru = GRUUpdate(node_dim)
-
-    for i in range(0, depth):
-        n_in = GatherNodesOutgoing()([n, edi])
-        n_out = GatherNodesIngoing()([n, edi])
-        m_in = MatMulMessages()([edge_net_in, n_in])
-        m_out = MatMulMessages()([edge_net_out, n_out])
-        eu = LazyConcatenate(axis=-1)([m_in, m_out])
-        eu = PoolingLocalEdges(**pooling_args)([n, eu, edi])  # Summing for each node connections
-        n = gru([n, eu])
-
-    n = LazyConcatenate(axis=-1)([n0, n])
-
-    # Output embedding choice
-    if output_embedding == 'graph':
-        if use_set2set:
-            # output
-            out = Dense(set2set_args['channels'], activation="linear")(n)
-            out = PoolingSet2Set(**set2set_args)(out)
-        else:
-            out = PoolingNodes(**pooling_args)(n)
-        out = ks.layers.Flatten()(out)  # Flatten() required for to Set2Set output.
-        out = MLP(**output_mlp)(out)
-    elif output_embedding == 'node':
-        out = GraphMLP(**output_mlp)(n)
-        if output_to_tensor:  # For tf version < 2.8 cast to tensor below.
-            out = ChangeTensorType(input_tensor_type='ragged', output_tensor_type="tensor")(out)
-    else:
-        raise ValueError("Unsupported output embedding for mode `NMPN`")
-
-    model = ks.models.Model(inputs=[node_input, edge_input, edge_index_input], outputs=out)
-    return model
-
-
-model_crystal_default = {
-    "name": "NMPN",
-    "inputs": [{"shape": (None,), "name": "node_attributes", "dtype": "float32", "ragged": True},
-               {"shape": (None,), "name": "edge_attributes", "dtype": "float32", "ragged": True},
-               {"shape": (None, 2), "name": "edge_indices", "dtype": "int64", "ragged": True}],
-    "input_embedding": {"node": {"input_dim": 95, "output_dim": 64},
-                        "edge": {"input_dim": 5, "output_dim": 64}},
-    "geometric_edge": False, "make_distance": False, "expand_distance": False,
-    "gauss_args": {"bins": 20, "distance": 4, "offset": 0.0, "sigma": 0.4},
-    "set2set_args": {"channels": 32, "T": 3, "pooling_method": "sum",
-                     "init_qstar": "0"},
-    "pooling_args": {"pooling_method": "segment_sum"},
-    "edge_mlp": {"use_bias": True, "activation": "swish", "units": [64, 64, 64]},
-    "use_set2set": True, "depth": 3, "node_dim": 64,
-    "verbose": 10,
-    "output_embedding": 'graph', "output_to_tensor": True,
-    "output_mlp": {"use_bias": [True, True, False], "units": [25, 10, 1],
-                   "activation": ["selu", "selu", "sigmoid"]},
-}
-
-
-@update_model_kwargs(model_crystal_default)
-def make_crystal_model(inputs: list = None,
-                       input_embedding: dict = None,
-                       geometric_edge: bool = None,
-                       make_distance: bool = None,
-                       expand_distance: bool = None,
-                       gauss_args: dict = None,
-                       set2set_args: dict = None,
-                       pooling_args: dict = None,
-                       edge_mlp: dict = None,
-                       use_set2set: bool = None,
-                       node_dim: int = None,
-                       depth: int = None,
-                       verbose: int = None,
-                       name: str = None,
-                       output_embedding: str = None,
-                       output_to_tensor: bool = None,
-                       output_mlp: dict = None
-                       ):
-    r"""Make `NMPN <http://arxiv.org/abs/1704.01212>`_ graph network via functional API.
-    Default parameters can be found in :obj:`kgcnn.literature.NMPN.model_crystal_default`.
-
-    Inputs:
-        list: `[node_attributes, edge_attributes, edge_indices, edge_image, lattice]`
-        or `[node_attributes, edge_distance, edge_indices, edge_image, lattice]` if :obj:`geometric_edge=True`
-        or `[node_attributes, node_coordinates, edge_indices, edge_image, lattice]` if :obj:`make_distance=True` and
-        :obj:`expand_distance=True` to compute edge distances from node coordinates within the model.
-
-            - node_attributes (tf.RaggedTensor): Node attributes of shape `(batch, None, F)` or `(batch, None)`
-              using an embedding layer.
-            - edge_attributes (tf.RaggedTensor): Edge attributes of shape `(batch, None, F)` or `(batch, None)`
-              using an embedding layer.
-            - edge_distance (tf.RaggedTensor): Edge attributes or distance of shape `(batch, None, D)` expanded
-              in a basis of dimension `D` or `(batch, None, 1)` if using a :obj:`GaussBasisLayer` layer
-              with model argument :obj:`expand_distance=True` and the numeric distance between nodes.
-            - edge_indices (tf.RaggedTensor): Index list for edges of shape `(batch, None, 2)`.
-            - node_coordinates (tf.RaggedTensor): Node (atomic) coordinates of shape `(batch, None, 3)`.
-            - lattice (tf.Tensor): Lattice matrix of the periodic structure of shape `(batch, 3, 3)`.
-            - edge_image (tf.RaggedTensor): Indices of the periodic image the sending node is located. The indices
-                of and edge are :math:`(i, j)` with :math:`j` being the sending node.
-
-    Outputs:
-        tf.Tensor: Graph embeddings of shape `(batch, L)` if :obj:`output_embedding="graph"`.
-
-    Args:
-        inputs (list): List of dictionaries unpacked in :obj:`tf.keras.layers.Input`. Order must match model definition.
-        input_embedding (dict): Dictionary of embedding arguments for nodes etc. unpacked in :obj:`Embedding` layers.
-        geometric_edge (bool): Whether the edges are geometric, like distance or coordinates.
-        make_distance (bool): Whether input is distance or coordinates at in place of edges.
-        expand_distance (bool): If the edge input are actual edges or node coordinates instead that are expanded to
-            form edges with a gauss distance basis given edge indices. Expansion uses `gauss_args`.
-        gauss_args (dict): Dictionary of layer arguments unpacked in :obj:`GaussBasisLayer` layer.
-        set2set_args (dict): Dictionary of layer arguments unpacked in :obj:`PoolingSet2Set` layer.
-        pooling_args (dict): Dictionary of layer arguments unpacked in :obj:`PoolingNodes`, `PoolingLocalEdges` layers.
-        edge_mlp (dict): Dictionary of layer arguments unpacked in :obj:`MLP` layer for edge matrix.
-        use_set2set (bool): Whether to use :obj:`PoolingSet2Set` layer.
-        node_dim (int): Dimension of hidden node embedding.
-        depth (int): Number of graph embedding units or depth of the network.
-        verbose (int): Level of verbosity.
-        name (str): Name of the model.
-        output_embedding (str): Main embedding task for graph network. Either "node", "edge" or "graph".
-        output_to_tensor (bool): Whether to cast model output to :obj:`tf.Tensor`.
-        output_mlp (dict): Dictionary of layer arguments unpacked in the final classification :obj:`MLP` layer block.
-            Defines number of model outputs and activation.
-
-    Returns:
-        :obj:`tf.keras.models.Model`
-    """
-    # Make input
-    node_input = ks.layers.Input(**inputs[0])
-    edge_input = ks.layers.Input(**inputs[1])  # Or coordinates
-    edge_index_input = ks.layers.Input(**inputs[2])
-    edge_image = ks.layers.Input(**inputs[3])
-    lattice = ks.layers.Input(**inputs[4])
-
-    edi = edge_index_input
-
-    # embedding, if no feature dimension
-    n0 = OptionalInputEmbedding(**input_embedding['node'], use_embedding=len(inputs[0]['shape']) < 2)(node_input)
-    if not geometric_edge:
-        ed = OptionalInputEmbedding(**input_embedding['edge'], use_embedding=len(inputs[1]['shape']) < 2)(edge_input)
-    else:
-        ed = edge_input
-
-    # If coordinates are in place of edges
-    if make_distance:
-        x = ed
-        pos1, pos2 = NodePosition()([x, edi])
-        pos2 = ShiftPeriodicLattice()([pos2, edge_image, lattice])
-        ed = NodeDistanceEuclidean()([pos1, pos2])
-
-    if expand_distance:
-        ed = GaussBasisLayer(**gauss_args)(ed)
-
-    # Make hidden dimension
-    n = Dense(node_dim, activation="linear")(n0)
-
-    # Make edge networks.
-    edge_net_in = GraphMLP(**edge_mlp)(ed)
-    edge_net_in = TrafoEdgeNetMessages(target_shape=(node_dim, node_dim))(edge_net_in)
-    edge_net_out = GraphMLP(**edge_mlp)(ed)
-    edge_net_out = TrafoEdgeNetMessages(target_shape=(node_dim, node_dim))(edge_net_out)
-
-    # Gru for node updates
-    gru = GRUUpdate(node_dim)
-
-    for i in range(0, depth):
-        n_in = GatherNodesOutgoing()([n, edi])
-        n_out = GatherNodesIngoing()([n, edi])
-        m_in = MatMulMessages()([edge_net_in, n_in])
-        m_out = MatMulMessages()([edge_net_out, n_out])
-        eu = LazyConcatenate(axis=-1)([m_in, m_out])
-        eu = PoolingLocalEdges(**pooling_args)([n, eu, edi])  # Summing for each node connections
-        n = gru([n, eu])
-
-    n = LazyConcatenate(axis=-1)([n0, n])
-
-    # Output embedding choice
-    if output_embedding == 'graph':
-        if use_set2set:
-            # output
-            out = Dense(set2set_args['channels'], activation="linear")(n)
-            out = PoolingSet2Set(**set2set_args)(out)
-        else:
-            out = PoolingNodes(**pooling_args)(n)
-        out = ks.layers.Flatten()(out)  # Flatten() required for to Set2Set output.
-        out = MLP(**output_mlp)(out)
-    elif output_embedding == 'node':
-        out = GraphMLP(**output_mlp)(n)
-        if output_to_tensor:  # For tf version < 2.8 cast to tensor below.
-            out = ChangeTensorType(input_tensor_type='ragged', output_tensor_type="tensor")(out)
-    else:
-        raise ValueError("Unsupported output embedding for mode `NMPN`")
-
-    model = ks.models.Model(inputs=[node_input, edge_input, edge_index_input, edge_image, lattice], outputs=out)
-
-    model.__kgcnn_model_version__ = __model_version__
-    return model
+import tensorflow as tf
+from kgcnn.layers.casting import ChangeTensorType
+from ._mpnn_conv import TrafoEdgeNetMessages, MatMulMessages
+from kgcnn.layers.update import GRUUpdate
+from kgcnn.layers.gather import GatherNodesOutgoing, GatherNodesIngoing
+from kgcnn.layers.modules import Dense, LazyConcatenate, OptionalInputEmbedding
+from kgcnn.layers.mlp import GraphMLP, MLP
+from kgcnn.layers.pooling import PoolingLocalEdges, PoolingNodes
+from kgcnn.layers.set2set import PoolingSet2SetEncoder
+from kgcnn.model.utils import update_model_kwargs
+from kgcnn.layers.geom import NodePosition, NodeDistanceEuclidean, GaussBasisLayer, ShiftPeriodicLattice
+
+ks = tf.keras
+
+# Keep track of model version from commit date in literature.
+# To be updated if model is changed in a significant way.
+__model_version__ = "2022.11.25"
+
+
+# Implementation of NMPN in `tf.keras` from paper:
+# Neural Message Passing for Quantum Chemistry
+# by Justin Gilmer, Samuel S. Schoenholz, Patrick F. Riley, Oriol Vinyals, George E. Dahl
+# http://arxiv.org/abs/1704.01212    
+
+model_default = {
+    "name": "NMPN",
+    "inputs": [{"shape": (None,), "name": "node_attributes", "dtype": "float32", "ragged": True},
+               {"shape": (None,), "name": "edge_attributes", "dtype": "float32", "ragged": True},
+               {"shape": (None, 2), "name": "edge_indices", "dtype": "int64", "ragged": True}],
+    "input_embedding": {"node": {"input_dim": 95, "output_dim": 64},
+                        "edge": {"input_dim": 5, "output_dim": 64}},
+    "geometric_edge": False, "make_distance": False, "expand_distance": False,
+    "gauss_args": {"bins": 20, "distance": 4, "offset": 0.0, "sigma": 0.4},
+    "set2set_args": {"channels": 32, "T": 3, "pooling_method": "sum",
+                     "init_qstar": "0"},
+    "pooling_args": {"pooling_method": "segment_sum"},
+    "edge_mlp": {"use_bias": True, "activation": "swish", "units": [64, 64, 64]},
+    "use_set2set": True, "depth": 3, "node_dim": 64,
+    "verbose": 10,
+    "output_embedding": 'graph', "output_to_tensor": True,
+    "output_mlp": {"use_bias": [True, True, False], "units": [25, 10, 1],
+                   "activation": ["selu", "selu", "sigmoid"]},
+}
+
+
+@update_model_kwargs(model_default)
+def make_model(inputs: list = None,
+               input_embedding: dict = None,
+               geometric_edge: bool = None,
+               make_distance: bool = None,
+               expand_distance: bool = None,
+               gauss_args: dict = None,
+               set2set_args: dict = None,
+               pooling_args: dict = None,
+               edge_mlp: dict = None,
+               use_set2set: bool = None,
+               node_dim: int = None,
+               depth: int = None,
+               verbose: int = None,
+               name: str = None,
+               output_embedding: str = None,
+               output_to_tensor: bool = None,
+               output_mlp: dict = None
+               ):
+    r"""Make `NMPN <http://arxiv.org/abs/1704.01212>`_ graph network via functional API.
+    Default parameters can be found in :obj:`kgcnn.literature.NMPN.model_default`.
+
+    Inputs:
+        list: `[node_attributes, edge_attributes, edge_indices]`
+        or `[node_attributes, edge_distance, edge_indices]` if :obj:`geometric_edge=True`
+        or `[node_attributes, node_coordinates, edge_indices]` if :obj:`make_distance=True` and
+        :obj:`expand_distance=True` to compute edge distances from node coordinates within the model.
+
+            - node_attributes (tf.RaggedTensor): Node attributes of shape `(batch, None, F)` or `(batch, None)`
+              using an embedding layer.
+            - edge_attributes (tf.RaggedTensor): Edge attributes of shape `(batch, None, F)` or `(batch, None)`
+              using an embedding layer.
+            - edge_distance (tf.RaggedTensor): Edge attributes or distance of shape `(batch, None, D)` expanded
+              in a basis of dimension `D` or `(batch, None, 1)` if using a :obj:`GaussBasisLayer` layer
+              with model argument :obj:`expand_distance=True` and the numeric distance between nodes.
+            - edge_indices (tf.RaggedTensor): Index list for edges of shape `(batch, None, 2)`.
+            - node_coordinates (tf.RaggedTensor): Node (atomic) coordinates of shape `(batch, None, 3)`.
+
+    Outputs:
+        tf.Tensor: Graph embeddings of shape `(batch, L)` if :obj:`output_embedding="graph"`.
+
+    Args:
+        inputs (list): List of dictionaries unpacked in :obj:`tf.keras.layers.Input`. Order must match model definition.
+        input_embedding (dict): Dictionary of embedding arguments for nodes etc. unpacked in :obj:`Embedding` layers.
+        geometric_edge (bool): Whether the edges are geometric, like distance or coordinates.
+        make_distance (bool): Whether input is distance or coordinates at in place of edges.
+        expand_distance (bool): If the edge input are actual edges or node coordinates instead that are expanded to
+            form edges with a gauss distance basis given edge indices. Expansion uses `gauss_args`.
+        gauss_args (dict): Dictionary of layer arguments unpacked in :obj:`GaussBasisLayer` layer.
+        set2set_args (dict): Dictionary of layer arguments unpacked in :obj:`PoolingSet2SetEncoder` layer.
+        pooling_args (dict): Dictionary of layer arguments unpacked in :obj:`PoolingNodes`, `PoolingLocalEdges` layers.
+        edge_mlp (dict): Dictionary of layer arguments unpacked in :obj:`MLP` layer for edge matrix.
+        use_set2set (bool): Whether to use :obj:`PoolingSet2SetEncoder` layer.
+        node_dim (int): Dimension of hidden node embedding.
+        depth (int): Number of graph embedding units or depth of the network.
+        verbose (int): Level of verbosity.
+        name (str): Name of the model.
+        output_embedding (str): Main embedding task for graph network. Either "node", "edge" or "graph".
+        output_to_tensor (bool): Whether to cast model output to :obj:`tf.Tensor`.
+        output_mlp (dict): Dictionary of layer arguments unpacked in the final classification :obj:`MLP` layer block.
+            Defines number of model outputs and activation.
+
+    Returns:
+        :obj:`tf.keras.models.Model`
+    """
+    # Make input
+    node_input = ks.layers.Input(**inputs[0])
+    edge_input = ks.layers.Input(**inputs[1])  # Or coordinates
+    edge_index_input = ks.layers.Input(**inputs[2])
+    edi = edge_index_input
+
+    # embedding, if no feature dimension
+    n0 = OptionalInputEmbedding(**input_embedding['node'], use_embedding=len(inputs[0]['shape']) < 2)(node_input)
+    if not geometric_edge:
+        ed = OptionalInputEmbedding(**input_embedding['edge'], use_embedding=len(inputs[1]['shape']) < 2)(edge_input)
+    else:
+        ed = edge_input
+
+    # If coordinates are in place of edges
+    if make_distance:
+        pos1, pos2 = NodePosition()([ed, edi])
+        ed = NodeDistanceEuclidean()([pos1, pos2])
+
+    if expand_distance:
+        ed = GaussBasisLayer(**gauss_args)(ed)
+
+    # Make hidden dimension
+    n = Dense(node_dim, activation="linear")(n0)
+
+    # Make edge networks.
+    edge_net_in = GraphMLP(**edge_mlp)(ed)
+    edge_net_in = TrafoEdgeNetMessages(target_shape=(node_dim, node_dim))(edge_net_in)
+    edge_net_out = GraphMLP(**edge_mlp)(ed)
+    edge_net_out = TrafoEdgeNetMessages(target_shape=(node_dim, node_dim))(edge_net_out)
+
+    # Gru for node updates
+    gru = GRUUpdate(node_dim)
+
+    for i in range(0, depth):
+        n_in = GatherNodesOutgoing()([n, edi])
+        n_out = GatherNodesIngoing()([n, edi])
+        m_in = MatMulMessages()([edge_net_in, n_in])
+        m_out = MatMulMessages()([edge_net_out, n_out])
+        eu = LazyConcatenate(axis=-1)([m_in, m_out])
+        eu = PoolingLocalEdges(**pooling_args)([n, eu, edi])  # Summing for each node connections
+        n = gru([n, eu])
+
+    n = LazyConcatenate(axis=-1)([n0, n])
+
+    # Output embedding choice
+    if output_embedding == 'graph':
+        if use_set2set:
+            # output
+            out = Dense(set2set_args['channels'], activation="linear")(n)
+            out = PoolingSet2SetEncoder(**set2set_args)(out)
+        else:
+            out = PoolingNodes(**pooling_args)(n)
+        out = ks.layers.Flatten()(out)  # Flatten() required for to Set2Set output.
+        out = MLP(**output_mlp)(out)
+    elif output_embedding == 'node':
+        out = GraphMLP(**output_mlp)(n)
+        if output_to_tensor:  # For tf version < 2.8 cast to tensor below.
+            out = ChangeTensorType(input_tensor_type='ragged', output_tensor_type="tensor")(out)
+    else:
+        raise ValueError("Unsupported output embedding for mode `NMPN`")
+
+    model = ks.models.Model(inputs=[node_input, edge_input, edge_index_input], outputs=out)
+    return model
+
+
+model_crystal_default = {
+    "name": "NMPN",
+    "inputs": [{"shape": (None,), "name": "node_attributes", "dtype": "float32", "ragged": True},
+               {"shape": (None,), "name": "edge_attributes", "dtype": "float32", "ragged": True},
+               {"shape": (None, 2), "name": "edge_indices", "dtype": "int64", "ragged": True}],
+    "input_embedding": {"node": {"input_dim": 95, "output_dim": 64},
+                        "edge": {"input_dim": 5, "output_dim": 64}},
+    "geometric_edge": False, "make_distance": False, "expand_distance": False,
+    "gauss_args": {"bins": 20, "distance": 4, "offset": 0.0, "sigma": 0.4},
+    "set2set_args": {"channels": 32, "T": 3, "pooling_method": "sum",
+                     "init_qstar": "0"},
+    "pooling_args": {"pooling_method": "segment_sum"},
+    "edge_mlp": {"use_bias": True, "activation": "swish", "units": [64, 64, 64]},
+    "use_set2set": True, "depth": 3, "node_dim": 64,
+    "verbose": 10,
+    "output_embedding": 'graph', "output_to_tensor": True,
+    "output_mlp": {"use_bias": [True, True, False], "units": [25, 10, 1],
+                   "activation": ["selu", "selu", "sigmoid"]},
+}
+
+
+@update_model_kwargs(model_crystal_default)
+def make_crystal_model(inputs: list = None,
+                       input_embedding: dict = None,
+                       geometric_edge: bool = None,
+                       make_distance: bool = None,
+                       expand_distance: bool = None,
+                       gauss_args: dict = None,
+                       set2set_args: dict = None,
+                       pooling_args: dict = None,
+                       edge_mlp: dict = None,
+                       use_set2set: bool = None,
+                       node_dim: int = None,
+                       depth: int = None,
+                       verbose: int = None,
+                       name: str = None,
+                       output_embedding: str = None,
+                       output_to_tensor: bool = None,
+                       output_mlp: dict = None
+                       ):
+    r"""Make `NMPN <http://arxiv.org/abs/1704.01212>`_ graph network via functional API.
+    Default parameters can be found in :obj:`kgcnn.literature.NMPN.model_crystal_default`.
+
+    Inputs:
+        list: `[node_attributes, edge_attributes, edge_indices, edge_image, lattice]`
+        or `[node_attributes, edge_distance, edge_indices, edge_image, lattice]` if :obj:`geometric_edge=True`
+        or `[node_attributes, node_coordinates, edge_indices, edge_image, lattice]` if :obj:`make_distance=True` and
+        :obj:`expand_distance=True` to compute edge distances from node coordinates within the model.
+
+            - node_attributes (tf.RaggedTensor): Node attributes of shape `(batch, None, F)` or `(batch, None)`
+              using an embedding layer.
+            - edge_attributes (tf.RaggedTensor): Edge attributes of shape `(batch, None, F)` or `(batch, None)`
+              using an embedding layer.
+            - edge_distance (tf.RaggedTensor): Edge attributes or distance of shape `(batch, None, D)` expanded
+              in a basis of dimension `D` or `(batch, None, 1)` if using a :obj:`GaussBasisLayer` layer
+              with model argument :obj:`expand_distance=True` and the numeric distance between nodes.
+            - edge_indices (tf.RaggedTensor): Index list for edges of shape `(batch, None, 2)`.
+            - node_coordinates (tf.RaggedTensor): Node (atomic) coordinates of shape `(batch, None, 3)`.
+            - lattice (tf.Tensor): Lattice matrix of the periodic structure of shape `(batch, 3, 3)`.
+            - edge_image (tf.RaggedTensor): Indices of the periodic image the sending node is located. The indices
+                of and edge are :math:`(i, j)` with :math:`j` being the sending node.
+
+    Outputs:
+        tf.Tensor: Graph embeddings of shape `(batch, L)` if :obj:`output_embedding="graph"`.
+
+    Args:
+        inputs (list): List of dictionaries unpacked in :obj:`tf.keras.layers.Input`. Order must match model definition.
+        input_embedding (dict): Dictionary of embedding arguments for nodes etc. unpacked in :obj:`Embedding` layers.
+        geometric_edge (bool): Whether the edges are geometric, like distance or coordinates.
+        make_distance (bool): Whether input is distance or coordinates at in place of edges.
+        expand_distance (bool): If the edge input are actual edges or node coordinates instead that are expanded to
+            form edges with a gauss distance basis given edge indices. Expansion uses `gauss_args`.
+        gauss_args (dict): Dictionary of layer arguments unpacked in :obj:`GaussBasisLayer` layer.
+        set2set_args (dict): Dictionary of layer arguments unpacked in :obj:`PoolingSet2SetEncoder` layer.
+        pooling_args (dict): Dictionary of layer arguments unpacked in :obj:`PoolingNodes`, `PoolingLocalEdges` layers.
+        edge_mlp (dict): Dictionary of layer arguments unpacked in :obj:`MLP` layer for edge matrix.
+        use_set2set (bool): Whether to use :obj:`PoolingSet2SetEncoder` layer.
+        node_dim (int): Dimension of hidden node embedding.
+        depth (int): Number of graph embedding units or depth of the network.
+        verbose (int): Level of verbosity.
+        name (str): Name of the model.
+        output_embedding (str): Main embedding task for graph network. Either "node", "edge" or "graph".
+        output_to_tensor (bool): Whether to cast model output to :obj:`tf.Tensor`.
+        output_mlp (dict): Dictionary of layer arguments unpacked in the final classification :obj:`MLP` layer block.
+            Defines number of model outputs and activation.
+
+    Returns:
+        :obj:`tf.keras.models.Model`
+    """
+    # Make input
+    node_input = ks.layers.Input(**inputs[0])
+    edge_input = ks.layers.Input(**inputs[1])  # Or coordinates
+    edge_index_input = ks.layers.Input(**inputs[2])
+    edge_image = ks.layers.Input(**inputs[3])
+    lattice = ks.layers.Input(**inputs[4])
+
+    edi = edge_index_input
+
+    # embedding, if no feature dimension
+    n0 = OptionalInputEmbedding(**input_embedding['node'], use_embedding=len(inputs[0]['shape']) < 2)(node_input)
+    if not geometric_edge:
+        ed = OptionalInputEmbedding(**input_embedding['edge'], use_embedding=len(inputs[1]['shape']) < 2)(edge_input)
+    else:
+        ed = edge_input
+
+    # If coordinates are in place of edges
+    if make_distance:
+        x = ed
+        pos1, pos2 = NodePosition()([x, edi])
+        pos2 = ShiftPeriodicLattice()([pos2, edge_image, lattice])
+        ed = NodeDistanceEuclidean()([pos1, pos2])
+
+    if expand_distance:
+        ed = GaussBasisLayer(**gauss_args)(ed)
+
+    # Make hidden dimension
+    n = Dense(node_dim, activation="linear")(n0)
+
+    # Make edge networks.
+    edge_net_in = GraphMLP(**edge_mlp)(ed)
+    edge_net_in = TrafoEdgeNetMessages(target_shape=(node_dim, node_dim))(edge_net_in)
+    edge_net_out = GraphMLP(**edge_mlp)(ed)
+    edge_net_out = TrafoEdgeNetMessages(target_shape=(node_dim, node_dim))(edge_net_out)
+
+    # Gru for node updates
+    gru = GRUUpdate(node_dim)
+
+    for i in range(0, depth):
+        n_in = GatherNodesOutgoing()([n, edi])
+        n_out = GatherNodesIngoing()([n, edi])
+        m_in = MatMulMessages()([edge_net_in, n_in])
+        m_out = MatMulMessages()([edge_net_out, n_out])
+        eu = LazyConcatenate(axis=-1)([m_in, m_out])
+        eu = PoolingLocalEdges(**pooling_args)([n, eu, edi])  # Summing for each node connections
+        n = gru([n, eu])
+
+    n = LazyConcatenate(axis=-1)([n0, n])
+
+    # Output embedding choice
+    if output_embedding == 'graph':
+        if use_set2set:
+            # output
+            out = Dense(set2set_args['channels'], activation="linear")(n)
+            out = PoolingSet2SetEncoder(**set2set_args)(out)
+        else:
+            out = PoolingNodes(**pooling_args)(n)
+        out = ks.layers.Flatten()(out)  # Flatten() required for to Set2Set output.
+        out = MLP(**output_mlp)(out)
+    elif output_embedding == 'node':
+        out = GraphMLP(**output_mlp)(n)
+        if output_to_tensor:  # For tf version < 2.8 cast to tensor below.
+            out = ChangeTensorType(input_tensor_type='ragged', output_tensor_type="tensor")(out)
+    else:
+        raise ValueError("Unsupported output embedding for mode `NMPN`")
+
+    model = ks.models.Model(inputs=[node_input, edge_input, edge_index_input, edge_image, lattice], outputs=out)
+
+    model.__kgcnn_model_version__ = __model_version__
+    return model
```

### Comparing `kgcnn-2.2.4/kgcnn/literature/PAiNN.py` & `kgcnn-3.0.0/kgcnn/literature/PAiNN/_make.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import tensorflow as tf
 from kgcnn.layers.casting import ChangeTensorType
-from kgcnn.layers.conv.painn_conv import PAiNNUpdate, EquivariantInitialize
-from kgcnn.layers.conv.painn_conv import PAiNNconv
+from ._painn_conv import PAiNNUpdate, EquivariantInitialize
+from ._painn_conv import PAiNNconv
 from kgcnn.layers.geom import NodeDistanceEuclidean, BesselBasisLayer, EdgeDirectionNormalized, CosCutOffEnvelope, \
     NodePosition, ShiftPeriodicLattice
 from kgcnn.layers.modules import LazyAdd, OptionalInputEmbedding
 from kgcnn.layers.mlp import GraphMLP, MLP
 from kgcnn.layers.pooling import PoolingNodes
 from kgcnn.layers.norm import GraphLayerNormalization, GraphBatchNormalization
 from kgcnn.model.utils import update_model_kwargs
```

### Comparing `kgcnn-2.2.4/kgcnn/literature/RGCN.py` & `kgcnn-3.0.0/kgcnn/literature/RGCN/_make.py`

 * *Files identical despite different names*

### Comparing `kgcnn-2.2.4/kgcnn/literature/Schnet.py` & `kgcnn-3.0.0/kgcnn/literature/Schnet/_make.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,282 +1,282 @@
-import tensorflow as tf
-from kgcnn.layers.casting import ChangeTensorType
-from kgcnn.layers.conv.schnet_conv import SchNetInteraction
-from kgcnn.layers.geom import NodeDistanceEuclidean, GaussBasisLayer, NodePosition, ShiftPeriodicLattice
-from kgcnn.layers.modules import Dense, OptionalInputEmbedding
-from kgcnn.layers.mlp import GraphMLP, MLP
-from kgcnn.layers.pooling import PoolingNodes
-from kgcnn.model.utils import update_model_kwargs
-
-ks = tf.keras
-
-# Keep track of model version from commit date in literature.
-# To be updated if model is changed in a significant way.
-__model_version__ = "2022.11.25"
-
-# Implementation of Schnet in `tf.keras` from paper:
-# by Kristof T. Schütt, Pieter-Jan Kindermans, Huziel E. Sauceda, Stefan Chmiela,
-# Alexandre Tkatchenko, Klaus-Robert Müller (2018)
-# https://doi.org/10.1063/1.5019779
-# https://arxiv.org/abs/1706.08566  
-# https://aip.scitation.org/doi/pdf/10.1063/1.5019779
-
-
-model_default = {
-    "name": "Schnet",
-    "inputs": [{"shape": (None,), "name": "node_attributes", "dtype": "float32", "ragged": True},
-               {"shape": (None, 3), "name": "node_coordinates", "dtype": "float32", "ragged": True},
-               {"shape": (None, 2), "name": "edge_indices", "dtype": "int64", "ragged": True}],
-    "input_embedding": {"node": {"input_dim": 95, "output_dim": 64}},
-    "make_distance": True, "expand_distance": True,
-    "interaction_args": {"units": 128, "use_bias": True,
-                         "activation": "kgcnn>shifted_softplus", "cfconv_pool": "sum"},
-    "node_pooling_args": {"pooling_method": "sum"},
-    "depth": 4,
-    "gauss_args": {"bins": 20, "distance": 4, "offset": 0.0, "sigma": 0.4},
-    "verbose": 10,
-    "last_mlp": {"use_bias": [True, True], "units": [128, 64],
-                 "activation": ["kgcnn>shifted_softplus", "kgcnn>shifted_softplus"]},
-    "output_embedding": "graph", "output_to_tensor": True,
-    "use_output_mlp": True,
-    "output_mlp": {"use_bias": [True, True], "units": [64, 1],
-                   "activation": ["kgcnn>shifted_softplus", "linear"]}
-}
-
-
-@update_model_kwargs(model_default)
-def make_model(inputs: list = None,
-               input_embedding: dict = None,
-               make_distance: bool = None,
-               expand_distance: bool = None,
-               gauss_args: dict = None,
-               interaction_args: dict = None,
-               node_pooling_args: dict = None,
-               depth: int = None,
-               name: str = None,
-               verbose: int = None,
-               last_mlp: dict = None,
-               output_embedding: str = None,
-               use_output_mlp: bool = None,
-               output_to_tensor: bool = None,
-               output_mlp: dict = None
-               ):
-    r"""Make `SchNet <https://arxiv.org/abs/1706.08566>`_ graph network via functional API.
-    Default parameters can be found in :obj:`kgcnn.literature.Schnet.model_default`.
-
-    Inputs:
-        list: `[node_attributes, edge_distance, edge_indices]`
-        or `[node_attributes, node_coordinates, edge_indices]` if :obj:`make_distance=True` and
-        :obj:`expand_distance=True` to compute edge distances from node coordinates within the model.
-
-            - node_attributes (tf.RaggedTensor): Node attributes of shape `(batch, None, F)` or `(batch, None)`
-              using an embedding layer.
-            - edge_distance (tf.RaggedTensor): Edge distance of shape `(batch, None, D)` expanded
-              in a basis of dimension `D` or `(batch, None, 1)` if using a :obj:`GaussBasisLayer` layer
-              with model argument :obj:`expand_distance=True` and the numeric distance between nodes.
-            - edge_indices (tf.RaggedTensor): Index list for edges of shape `(batch, None, 2)`.
-            - node_coordinates (tf.RaggedTensor): Node (atomic) coordinates of shape `(batch, None, 3)`.
-
-    Outputs:
-        tf.Tensor: Graph embeddings of shape `(batch, L)` if :obj:`output_embedding="graph"`.
-
-    Args:
-        inputs (list): List of dictionaries unpacked in :obj:`tf.keras.layers.Input`. Order must match model definition.
-        input_embedding (dict): Dictionary of embedding arguments for nodes etc. unpacked in :obj:`Embedding` layers.
-        make_distance (bool): Whether input is distance or coordinates at in place of edges.
-        expand_distance (bool): If the edge input are actual edges or node coordinates instead that are expanded to
-            form edges with a gauss distance basis given edge indices. Expansion uses `gauss_args`.
-        gauss_args (dict): Dictionary of layer arguments unpacked in :obj:`GaussBasisLayer` layer.
-        depth (int): Number of graph embedding units or depth of the network.
-        interaction_args (dict): Dictionary of layer arguments unpacked in final :obj:`SchNetInteraction` layers.
-        node_pooling_args (dict): Dictionary of layer arguments unpacked in :obj:`PoolingNodes` layers.
-        verbose (int): Level of verbosity.
-        name (str): Name of the model.
-        last_mlp (dict): Dictionary of layer arguments unpacked in last :obj:`MLP` layer before output or pooling.
-        output_embedding (str): Main embedding task for graph network. Either "node", "edge" or "graph".
-        use_output_mlp (bool): Whether to use the final output MLP. Possibility to skip final MLP.
-        output_to_tensor (bool): Whether to cast model output to :obj:`tf.Tensor`.
-        output_mlp (dict): Dictionary of layer arguments unpacked in the final classification :obj:`MLP` layer block.
-            Defines number of model outputs and activation.
-
-    Returns:
-        :obj:`tf.keras.models.Model`
-    """
-    # Make input
-    node_input = ks.layers.Input(**inputs[0])
-    xyz_input = ks.layers.Input(**inputs[1])
-    edge_index_input = ks.layers.Input(**inputs[2])
-
-    # embedding, if no feature dimension
-    n = OptionalInputEmbedding(**input_embedding['node'],
-                               use_embedding=len(inputs[0]['shape']) < 2)(node_input)
-    edi = edge_index_input
-
-    if make_distance:
-        x = xyz_input
-        pos1, pos2 = NodePosition()([x, edi])
-        ed = NodeDistanceEuclidean()([pos1, pos2])
-    else:
-        ed = xyz_input
-
-    if expand_distance:
-        ed = GaussBasisLayer(**gauss_args)(ed)
-
-    # Model
-    n = Dense(interaction_args["units"], activation='linear')(n)
-    for i in range(0, depth):
-        n = SchNetInteraction(**interaction_args)([n, ed, edi])
-
-    n = GraphMLP(**last_mlp)(n)
-
-    # Output embedding choice
-    if output_embedding == 'graph':
-        out = PoolingNodes(**node_pooling_args)(n)
-        if use_output_mlp:
-            out = MLP(**output_mlp)(out)
-    elif output_embedding == 'node':
-        out = n
-        if use_output_mlp:
-            out = GraphMLP(**output_mlp)(out)
-        if output_to_tensor:  # For tf version < 2.8 cast to tensor below.
-            out = ChangeTensorType(input_tensor_type="ragged", output_tensor_type="tensor")(out)
-    else:
-        raise ValueError("Unsupported output embedding for mode `SchNet`")
-
-    model = ks.models.Model(inputs=[node_input, xyz_input, edge_index_input], outputs=out)
-
-    model.__kgcnn_model_version__ = __model_version__
-    return model
-
-
-model_crystal_default = {
-    "name": "Schnet",
-    "inputs": [{"shape": (None,), "name": "node_number", "dtype": "float32", "ragged": True},
-               {"shape": (None, 3), "name": "node_coordinates", "dtype": "float32", "ragged": True},
-               {"shape": (None, 2), "name": "edge_indices", "dtype": "int64", "ragged": True},
-               {"shape": (None, 3), "name": "edge_image", "dtype": "int64", "ragged": True},
-               {"shape": (3, 3), "name": "graph_lattice", "dtype": "float32", "ragged": False}],
-    "input_embedding": {"node": {"input_dim": 95, "output_dim": 64}},
-    "make_distance": True, "expand_distance": True,
-    "interaction_args": {"units": 128, "use_bias": True, "activation": "kgcnn>shifted_softplus", "cfconv_pool": "sum"},
-    "node_pooling_args": {"pooling_method": "sum"},
-    "depth": 4,
-    "gauss_args": {"bins": 20, "distance": 4, "offset": 0.0, "sigma": 0.4},
-    "verbose": 10,
-    "last_mlp": {"use_bias": [True, True], "units": [128, 64],
-                 "activation": ["kgcnn>shifted_softplus", "kgcnn>shifted_softplus"]},
-    "output_embedding": "graph", "output_to_tensor": True,
-    "use_output_mlp": True,
-    "output_mlp": {"use_bias": [True, True], "units": [64, 1],
-                   "activation": ["kgcnn>shifted_softplus", "linear"]}
-}
-
-
-@update_model_kwargs(model_default)
-def make_crystal_model(inputs: list = None,
-                       input_embedding: dict = None,
-                       make_distance: bool = None,
-                       expand_distance: bool = None,
-                       gauss_args: dict = None,
-                       interaction_args: dict = None,
-                       node_pooling_args: dict = None,
-                       depth: int = None,
-                       name: str = None,
-                       verbose: int = None,
-                       last_mlp: dict = None,
-                       output_embedding: str = None,
-                       use_output_mlp: bool = None,
-                       output_to_tensor: bool = None,
-                       output_mlp: dict = None
-                       ):
-    r"""Make `SchNet <https://arxiv.org/abs/1706.08566>`_ graph network via functional API.
-    Default parameters can be found in :obj:`kgcnn.literature.Schnet.model_crystal_default`.
-
-    Inputs:
-        list: `[node_attributes, edge_distance, edge_indices, edge_image, lattice]`
-        or `[node_attributes, node_coordinates, edge_indices, edge_image, lattice]` if :obj:`make_distance=True` and
-        :obj:`expand_distance=True` to compute edge distances from node coordinates within the model.
-
-            - node_attributes (tf.RaggedTensor): Node attributes of shape `(batch, None, F)` or `(batch, None)`
-              using an embedding layer.
-            - edge_distance (tf.RaggedTensor): Edge distance of shape `(batch, None, D)` expanded
-              in a basis of dimension `D` or `(batch, None, 1)` if using a :obj:`GaussBasisLayer` layer
-              with model argument :obj:`expand_distance=True` and the numeric distance between nodes.
-            - edge_indices (tf.RaggedTensor): Index list for edges of shape `(batch, None, 2)`.
-            - node_coordinates (tf.RaggedTensor): Node (atomic) coordinates of shape `(batch, None, 3)`.
-            - lattice (tf.Tensor): Lattice matrix of the periodic structure of shape `(batch, 3, 3)`.
-            - edge_image (tf.RaggedTensor): Indices of the periodic image the sending node is located. The indices
-                of and edge are :math:`(i, j)` with :math:`j` being the sending node.
-
-    Outputs:
-        tf.Tensor: Graph embeddings of shape `(batch, L)` if :obj:`output_embedding="graph"`.
-
-    Args:
-        inputs (list): List of dictionaries unpacked in :obj:`tf.keras.layers.Input`. Order must match model definition.
-        input_embedding (dict): Dictionary of embedding arguments for nodes etc. unpacked in :obj:`Embedding` layers.
-        make_distance (bool): Whether input is distance or coordinates at in place of edges.
-        expand_distance (bool): If the edge input are actual edges or node coordinates instead that are expanded to
-            form edges with a gauss distance basis given edge indices. Expansion uses `gauss_args`.
-        gauss_args (dict): Dictionary of layer arguments unpacked in :obj:`GaussBasisLayer` layer.
-        depth (int): Number of graph embedding units or depth of the network.
-        interaction_args (dict): Dictionary of layer arguments unpacked in final :obj:`SchNetInteraction` layers.
-        node_pooling_args (dict): Dictionary of layer arguments unpacked in :obj:`PoolingNodes` layers.
-        verbose (int): Level of verbosity.
-        name (str): Name of the model.
-        last_mlp (dict): Dictionary of layer arguments unpacked in last :obj:`MLP` layer before output or pooling.
-        output_embedding (str): Main embedding task for graph network. Either "node", "edge" or "graph".
-        use_output_mlp (bool): Whether to use the final output MLP. Possibility to skip final MLP.
-        output_to_tensor (bool): Whether to cast model output to :obj:`tf.Tensor`.
-        output_mlp (dict): Dictionary of layer arguments unpacked in the final classification :obj:`MLP` layer block.
-            Defines number of model outputs and activation.
-
-    Returns:
-        :obj:`tf.keras.models.Model`
-    """
-    # Make input
-    node_input = ks.layers.Input(**inputs[0])
-    xyz_input = ks.layers.Input(**inputs[1])
-    edge_index_input = ks.layers.Input(**inputs[2])
-    edge_image = ks.layers.Input(**inputs[3])
-    lattice = ks.layers.Input(**inputs[4])
-
-    # embedding, if no feature dimension
-    n = OptionalInputEmbedding(**input_embedding['node'],
-                               use_embedding=len(inputs[0]['shape']) < 2)(node_input)
-    edi = edge_index_input
-
-    if make_distance:
-        x = xyz_input
-        pos1, pos2 = NodePosition()([x, edi])
-        pos2 = ShiftPeriodicLattice()([pos2, edge_image, lattice])
-        ed = NodeDistanceEuclidean()([pos1, pos2])
-    else:
-        ed = xyz_input
-
-    if expand_distance:
-        ed = GaussBasisLayer(**gauss_args)(ed)
-
-    # Model
-    n = Dense(interaction_args["units"], activation='linear')(n)
-    for i in range(0, depth):
-        n = SchNetInteraction(**interaction_args)([n, ed, edi])
-
-    n = GraphMLP(**last_mlp)(n)
-
-    # Output embedding choice
-    if output_embedding == 'graph':
-        out = PoolingNodes(**node_pooling_args)(n)
-        if use_output_mlp:
-            out = MLP(**output_mlp)(out)
-    elif output_embedding == 'node':
-        out = n
-        if use_output_mlp:
-            out = GraphMLP(**output_mlp)(out)
-        if output_to_tensor:  # For tf version < 2.8 cast to tensor below.
-            out = ChangeTensorType(input_tensor_type="ragged", output_tensor_type="tensor")(out)
-    else:
-        raise ValueError("Unsupported output embedding for mode `SchNet`")
-
-    model = ks.models.Model(inputs=[node_input, xyz_input, edge_index_input, edge_image, lattice], outputs=out)
-
-    model.__kgcnn_model_version__ = __model_version__
-    return model
+import tensorflow as tf
+from kgcnn.layers.casting import ChangeTensorType
+from ._schnet_conv import SchNetInteraction
+from kgcnn.layers.geom import NodeDistanceEuclidean, GaussBasisLayer, NodePosition, ShiftPeriodicLattice
+from kgcnn.layers.modules import Dense, OptionalInputEmbedding
+from kgcnn.layers.mlp import GraphMLP, MLP
+from kgcnn.layers.pooling import PoolingNodes
+from kgcnn.model.utils import update_model_kwargs
+
+ks = tf.keras
+
+# Keep track of model version from commit date in literature.
+# To be updated if model is changed in a significant way.
+__model_version__ = "2022.11.25"
+
+# Implementation of Schnet in `tf.keras` from paper:
+# by Kristof T. Schütt, Pieter-Jan Kindermans, Huziel E. Sauceda, Stefan Chmiela,
+# Alexandre Tkatchenko, Klaus-Robert Müller (2018)
+# https://doi.org/10.1063/1.5019779
+# https://arxiv.org/abs/1706.08566  
+# https://aip.scitation.org/doi/pdf/10.1063/1.5019779
+
+
+model_default = {
+    "name": "Schnet",
+    "inputs": [{"shape": (None,), "name": "node_attributes", "dtype": "float32", "ragged": True},
+               {"shape": (None, 3), "name": "node_coordinates", "dtype": "float32", "ragged": True},
+               {"shape": (None, 2), "name": "edge_indices", "dtype": "int64", "ragged": True}],
+    "input_embedding": {"node": {"input_dim": 95, "output_dim": 64}},
+    "make_distance": True, "expand_distance": True,
+    "interaction_args": {"units": 128, "use_bias": True,
+                         "activation": "kgcnn>shifted_softplus", "cfconv_pool": "sum"},
+    "node_pooling_args": {"pooling_method": "sum"},
+    "depth": 4,
+    "gauss_args": {"bins": 20, "distance": 4, "offset": 0.0, "sigma": 0.4},
+    "verbose": 10,
+    "last_mlp": {"use_bias": [True, True], "units": [128, 64],
+                 "activation": ["kgcnn>shifted_softplus", "kgcnn>shifted_softplus"]},
+    "output_embedding": "graph", "output_to_tensor": True,
+    "use_output_mlp": True,
+    "output_mlp": {"use_bias": [True, True], "units": [64, 1],
+                   "activation": ["kgcnn>shifted_softplus", "linear"]}
+}
+
+
+@update_model_kwargs(model_default)
+def make_model(inputs: list = None,
+               input_embedding: dict = None,
+               make_distance: bool = None,
+               expand_distance: bool = None,
+               gauss_args: dict = None,
+               interaction_args: dict = None,
+               node_pooling_args: dict = None,
+               depth: int = None,
+               name: str = None,
+               verbose: int = None,
+               last_mlp: dict = None,
+               output_embedding: str = None,
+               use_output_mlp: bool = None,
+               output_to_tensor: bool = None,
+               output_mlp: dict = None
+               ):
+    r"""Make `SchNet <https://arxiv.org/abs/1706.08566>`_ graph network via functional API.
+    Default parameters can be found in :obj:`kgcnn.literature.Schnet.model_default`.
+
+    Inputs:
+        list: `[node_attributes, edge_distance, edge_indices]`
+        or `[node_attributes, node_coordinates, edge_indices]` if :obj:`make_distance=True` and
+        :obj:`expand_distance=True` to compute edge distances from node coordinates within the model.
+
+            - node_attributes (tf.RaggedTensor): Node attributes of shape `(batch, None, F)` or `(batch, None)`
+              using an embedding layer.
+            - edge_distance (tf.RaggedTensor): Edge distance of shape `(batch, None, D)` expanded
+              in a basis of dimension `D` or `(batch, None, 1)` if using a :obj:`GaussBasisLayer` layer
+              with model argument :obj:`expand_distance=True` and the numeric distance between nodes.
+            - edge_indices (tf.RaggedTensor): Index list for edges of shape `(batch, None, 2)`.
+            - node_coordinates (tf.RaggedTensor): Node (atomic) coordinates of shape `(batch, None, 3)`.
+
+    Outputs:
+        tf.Tensor: Graph embeddings of shape `(batch, L)` if :obj:`output_embedding="graph"`.
+
+    Args:
+        inputs (list): List of dictionaries unpacked in :obj:`tf.keras.layers.Input`. Order must match model definition.
+        input_embedding (dict): Dictionary of embedding arguments for nodes etc. unpacked in :obj:`Embedding` layers.
+        make_distance (bool): Whether input is distance or coordinates at in place of edges.
+        expand_distance (bool): If the edge input are actual edges or node coordinates instead that are expanded to
+            form edges with a gauss distance basis given edge indices. Expansion uses `gauss_args`.
+        gauss_args (dict): Dictionary of layer arguments unpacked in :obj:`GaussBasisLayer` layer.
+        depth (int): Number of graph embedding units or depth of the network.
+        interaction_args (dict): Dictionary of layer arguments unpacked in final :obj:`SchNetInteraction` layers.
+        node_pooling_args (dict): Dictionary of layer arguments unpacked in :obj:`PoolingNodes` layers.
+        verbose (int): Level of verbosity.
+        name (str): Name of the model.
+        last_mlp (dict): Dictionary of layer arguments unpacked in last :obj:`MLP` layer before output or pooling.
+        output_embedding (str): Main embedding task for graph network. Either "node", "edge" or "graph".
+        use_output_mlp (bool): Whether to use the final output MLP. Possibility to skip final MLP.
+        output_to_tensor (bool): Whether to cast model output to :obj:`tf.Tensor`.
+        output_mlp (dict): Dictionary of layer arguments unpacked in the final classification :obj:`MLP` layer block.
+            Defines number of model outputs and activation.
+
+    Returns:
+        :obj:`tf.keras.models.Model`
+    """
+    # Make input
+    node_input = ks.layers.Input(**inputs[0])
+    xyz_input = ks.layers.Input(**inputs[1])
+    edge_index_input = ks.layers.Input(**inputs[2])
+
+    # embedding, if no feature dimension
+    n = OptionalInputEmbedding(**input_embedding['node'],
+                               use_embedding=len(inputs[0]['shape']) < 2)(node_input)
+    edi = edge_index_input
+
+    if make_distance:
+        x = xyz_input
+        pos1, pos2 = NodePosition()([x, edi])
+        ed = NodeDistanceEuclidean()([pos1, pos2])
+    else:
+        ed = xyz_input
+
+    if expand_distance:
+        ed = GaussBasisLayer(**gauss_args)(ed)
+
+    # Model
+    n = Dense(interaction_args["units"], activation='linear')(n)
+    for i in range(0, depth):
+        n = SchNetInteraction(**interaction_args)([n, ed, edi])
+
+    n = GraphMLP(**last_mlp)(n)
+
+    # Output embedding choice
+    if output_embedding == 'graph':
+        out = PoolingNodes(**node_pooling_args)(n)
+        if use_output_mlp:
+            out = MLP(**output_mlp)(out)
+    elif output_embedding == 'node':
+        out = n
+        if use_output_mlp:
+            out = GraphMLP(**output_mlp)(out)
+        if output_to_tensor:  # For tf version < 2.8 cast to tensor below.
+            out = ChangeTensorType(input_tensor_type="ragged", output_tensor_type="tensor")(out)
+    else:
+        raise ValueError("Unsupported output embedding for mode `SchNet`")
+
+    model = ks.models.Model(inputs=[node_input, xyz_input, edge_index_input], outputs=out)
+
+    model.__kgcnn_model_version__ = __model_version__
+    return model
+
+
+model_crystal_default = {
+    "name": "Schnet",
+    "inputs": [{"shape": (None,), "name": "node_number", "dtype": "float32", "ragged": True},
+               {"shape": (None, 3), "name": "node_coordinates", "dtype": "float32", "ragged": True},
+               {"shape": (None, 2), "name": "edge_indices", "dtype": "int64", "ragged": True},
+               {"shape": (None, 3), "name": "edge_image", "dtype": "int64", "ragged": True},
+               {"shape": (3, 3), "name": "graph_lattice", "dtype": "float32", "ragged": False}],
+    "input_embedding": {"node": {"input_dim": 95, "output_dim": 64}},
+    "make_distance": True, "expand_distance": True,
+    "interaction_args": {"units": 128, "use_bias": True, "activation": "kgcnn>shifted_softplus", "cfconv_pool": "sum"},
+    "node_pooling_args": {"pooling_method": "sum"},
+    "depth": 4,
+    "gauss_args": {"bins": 20, "distance": 4, "offset": 0.0, "sigma": 0.4},
+    "verbose": 10,
+    "last_mlp": {"use_bias": [True, True], "units": [128, 64],
+                 "activation": ["kgcnn>shifted_softplus", "kgcnn>shifted_softplus"]},
+    "output_embedding": "graph", "output_to_tensor": True,
+    "use_output_mlp": True,
+    "output_mlp": {"use_bias": [True, True], "units": [64, 1],
+                   "activation": ["kgcnn>shifted_softplus", "linear"]}
+}
+
+
+@update_model_kwargs(model_default)
+def make_crystal_model(inputs: list = None,
+                       input_embedding: dict = None,
+                       make_distance: bool = None,
+                       expand_distance: bool = None,
+                       gauss_args: dict = None,
+                       interaction_args: dict = None,
+                       node_pooling_args: dict = None,
+                       depth: int = None,
+                       name: str = None,
+                       verbose: int = None,
+                       last_mlp: dict = None,
+                       output_embedding: str = None,
+                       use_output_mlp: bool = None,
+                       output_to_tensor: bool = None,
+                       output_mlp: dict = None
+                       ):
+    r"""Make `SchNet <https://arxiv.org/abs/1706.08566>`_ graph network via functional API.
+    Default parameters can be found in :obj:`kgcnn.literature.Schnet.model_crystal_default`.
+
+    Inputs:
+        list: `[node_attributes, edge_distance, edge_indices, edge_image, lattice]`
+        or `[node_attributes, node_coordinates, edge_indices, edge_image, lattice]` if :obj:`make_distance=True` and
+        :obj:`expand_distance=True` to compute edge distances from node coordinates within the model.
+
+            - node_attributes (tf.RaggedTensor): Node attributes of shape `(batch, None, F)` or `(batch, None)`
+              using an embedding layer.
+            - edge_distance (tf.RaggedTensor): Edge distance of shape `(batch, None, D)` expanded
+              in a basis of dimension `D` or `(batch, None, 1)` if using a :obj:`GaussBasisLayer` layer
+              with model argument :obj:`expand_distance=True` and the numeric distance between nodes.
+            - edge_indices (tf.RaggedTensor): Index list for edges of shape `(batch, None, 2)`.
+            - node_coordinates (tf.RaggedTensor): Node (atomic) coordinates of shape `(batch, None, 3)`.
+            - lattice (tf.Tensor): Lattice matrix of the periodic structure of shape `(batch, 3, 3)`.
+            - edge_image (tf.RaggedTensor): Indices of the periodic image the sending node is located. The indices
+                of and edge are :math:`(i, j)` with :math:`j` being the sending node.
+
+    Outputs:
+        tf.Tensor: Graph embeddings of shape `(batch, L)` if :obj:`output_embedding="graph"`.
+
+    Args:
+        inputs (list): List of dictionaries unpacked in :obj:`tf.keras.layers.Input`. Order must match model definition.
+        input_embedding (dict): Dictionary of embedding arguments for nodes etc. unpacked in :obj:`Embedding` layers.
+        make_distance (bool): Whether input is distance or coordinates at in place of edges.
+        expand_distance (bool): If the edge input are actual edges or node coordinates instead that are expanded to
+            form edges with a gauss distance basis given edge indices. Expansion uses `gauss_args`.
+        gauss_args (dict): Dictionary of layer arguments unpacked in :obj:`GaussBasisLayer` layer.
+        depth (int): Number of graph embedding units or depth of the network.
+        interaction_args (dict): Dictionary of layer arguments unpacked in final :obj:`SchNetInteraction` layers.
+        node_pooling_args (dict): Dictionary of layer arguments unpacked in :obj:`PoolingNodes` layers.
+        verbose (int): Level of verbosity.
+        name (str): Name of the model.
+        last_mlp (dict): Dictionary of layer arguments unpacked in last :obj:`MLP` layer before output or pooling.
+        output_embedding (str): Main embedding task for graph network. Either "node", "edge" or "graph".
+        use_output_mlp (bool): Whether to use the final output MLP. Possibility to skip final MLP.
+        output_to_tensor (bool): Whether to cast model output to :obj:`tf.Tensor`.
+        output_mlp (dict): Dictionary of layer arguments unpacked in the final classification :obj:`MLP` layer block.
+            Defines number of model outputs and activation.
+
+    Returns:
+        :obj:`tf.keras.models.Model`
+    """
+    # Make input
+    node_input = ks.layers.Input(**inputs[0])
+    xyz_input = ks.layers.Input(**inputs[1])
+    edge_index_input = ks.layers.Input(**inputs[2])
+    edge_image = ks.layers.Input(**inputs[3])
+    lattice = ks.layers.Input(**inputs[4])
+
+    # embedding, if no feature dimension
+    n = OptionalInputEmbedding(**input_embedding['node'],
+                               use_embedding=len(inputs[0]['shape']) < 2)(node_input)
+    edi = edge_index_input
+
+    if make_distance:
+        x = xyz_input
+        pos1, pos2 = NodePosition()([x, edi])
+        pos2 = ShiftPeriodicLattice()([pos2, edge_image, lattice])
+        ed = NodeDistanceEuclidean()([pos1, pos2])
+    else:
+        ed = xyz_input
+
+    if expand_distance:
+        ed = GaussBasisLayer(**gauss_args)(ed)
+
+    # Model
+    n = Dense(interaction_args["units"], activation='linear')(n)
+    for i in range(0, depth):
+        n = SchNetInteraction(**interaction_args)([n, ed, edi])
+
+    n = GraphMLP(**last_mlp)(n)
+
+    # Output embedding choice
+    if output_embedding == 'graph':
+        out = PoolingNodes(**node_pooling_args)(n)
+        if use_output_mlp:
+            out = MLP(**output_mlp)(out)
+    elif output_embedding == 'node':
+        out = n
+        if use_output_mlp:
+            out = GraphMLP(**output_mlp)(out)
+        if output_to_tensor:  # For tf version < 2.8 cast to tensor below.
+            out = ChangeTensorType(input_tensor_type="ragged", output_tensor_type="tensor")(out)
+    else:
+        raise ValueError("Unsupported output embedding for mode `SchNet`")
+
+    model = ks.models.Model(inputs=[node_input, xyz_input, edge_index_input, edge_image, lattice], outputs=out)
+
+    model.__kgcnn_model_version__ = __model_version__
+    return model
```

### Comparing `kgcnn-2.2.4/kgcnn/literature/Unet.py` & `kgcnn-3.0.0/kgcnn/literature/Unet/_make.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,164 +1,168 @@
-import tensorflow as tf
-from kgcnn.layers.casting import ChangeTensorType
-from kgcnn.layers.gather import GatherNodesOutgoing
-from kgcnn.layers.modules import Dense, Activation, LazyAdd, OptionalInputEmbedding
-from kgcnn.layers.mlp import GraphMLP, MLP
-from kgcnn.layers.pooling import PoolingNodes, PoolingLocalEdges
-from kgcnn.layers.pool.topk import PoolingTopK, UnPoolingTopK, AdjacencyPower
-from kgcnn.model.utils import update_model_kwargs
-
-ks = tf.keras
-
-# Keep track of model version from commit date in literature.
-# To be updated if model is changed in a significant way.
-__model_version__ = "2022.11.25"
-
-
-# Implementation of Unet in `tf.keras` from paper:
-# Graph U-Nets
-# by Hongyang Gao, Shuiwang Ji
-# https://arxiv.org/pdf/1905.05178.pdf
-
-model_default = {'name': "Unet",
-                 'inputs': [{'shape': (None,), 'name': "node_attributes", 'dtype': 'float32', 'ragged': True},
-                            {'shape': (None,), 'name': "edge_attributes", 'dtype': 'float32', 'ragged': True},
-                            {'shape': (None, 2), 'name': "edge_indices", 'dtype': 'int64', 'ragged': True}],
-                 'input_embedding': {"node": {"input_dim": 95, "output_dim": 64},
-                                     "edge": {"input_dim": 5, "output_dim": 64}},
-                 'hidden_dim': {'units': 32, 'use_bias': True, 'activation': 'linear'},
-                 'top_k_args': {'k': 0.3, 'kernel_initializer': 'ones'},
-                 'activation': 'relu',
-                 'use_reconnect': True,
-                 'depth': 4,
-                 'pooling_args': {"pooling_method": 'segment_mean'},
-                 'gather_args': {},
-                 'verbose': 10,
-                 'output_embedding': 'graph', "output_to_tensor": True,
-                 'output_mlp': {"use_bias": [True, False], "units": [25, 1], "activation": ['relu', 'sigmoid']}
-                 }
-
-
-@update_model_kwargs(model_default)
-def make_model(inputs: list = None,
-               input_embedding: dict = None,
-               pooling_args: dict = None,
-               gather_args: dict = None,
-               top_k_args: dict = None,
-               depth: int = None,
-               use_reconnect: bool = None,
-               hidden_dim: dict = None,
-               activation: str = None,
-               name: str = None,
-               verbose: int = None,
-               output_embedding: str = None,
-               output_to_tensor: bool = None,
-               output_mlp: dict = None
-               ):
-    r"""Make `U-Net <https://arxiv.org/pdf/1905.05178.pdf>`_ graph network via functional API.
-    Default parameters can be found in :obj:`kgcnn.literature.Unet.model_default`.
-
-    Inputs:
-        list: `[node_attributes, edge_attributes, edge_indices]`
-
-            - node_attributes (tf.RaggedTensor): Node attributes of shape `(batch, None, F)` or `(batch, None)`
-              using an embedding layer.
-            - edge_attributes (tf.RaggedTensor): Edge attributes of shape `(batch, None, F)` or `(batch, None)`
-              using an embedding layer.
-            - edge_indices (tf.RaggedTensor): Index list for edges of shape `(batch, None, 2)`.
-
-    Outputs:
-        tf.Tensor: Graph embeddings of shape `(batch, L)` if :obj:`output_embedding="graph"`.
-
-    Args:
-        inputs (list): List of dictionaries unpacked in :obj:`tf.keras.layers.Input`. Order must match model definition.
-        input_embedding (dict): Dictionary of embedding arguments for nodes etc. unpacked in :obj:`Embedding` layers.
-        depth (int): Number of graph embedding units or depth of the network.
-        pooling_args (dict): Dictionary of layer arguments unpacked in :obj:`PoolingLocalEdges` layers.
-        gather_args (dict): Dictionary of layer arguments unpacked in :obj:`GatherNodesOutgoing` layers.
-        top_k_args (dict): Dictionary of layer arguments unpacked in :obj:`PoolingTopK` layers.
-        use_reconnect (bool): Whether to use :math:`A^2` between pooling.
-        hidden_dim (dict): Dictionary of layer arguments unpacked in hidden `Dense` layer.
-        activation (dict, str): Activation to use.
-        verbose (int): Level of verbosity.
-        name (str): Name of the model.
-        output_embedding (str): Main embedding task for graph network. Either "node", "edge" or "graph".
-        output_to_tensor (bool): Whether to cast model output to :obj:`tf.Tensor`.
-        output_mlp (dict): Dictionary of layer arguments unpacked in the final classification :obj:`MLP` layer block.
-            Defines number of model outputs and activation.
-
-    Returns:
-        :obj:`tf.keras.models.Model`
-    """
-    # Make input
-    node_input = ks.layers.Input(**inputs[0])
-    edge_input = ks.layers.Input(**inputs[1])
-    edge_index_input = ks.layers.Input(**inputs[2])
-
-    # embedding, if no feature dimension
-    n = OptionalInputEmbedding(**input_embedding['node'],
-                               use_embedding=len(inputs[0]['shape']) < 2)(node_input)
-    ed = OptionalInputEmbedding(**input_embedding['edge'],
-                                use_embedding=len(inputs[1]['shape']) < 2)(edge_input)
-    edi = edge_index_input
-
-    # Model
-    n = Dense(**hidden_dim)(n)
-    in_graph = [n, ed, edi]
-    graph_list = [in_graph]
-    map_list = []
-
-    # U Down
-    i_graph = in_graph
-    for i in range(0, depth):
-
-        n, ed, edi = i_graph
-        # GCN layer
-        eu = GatherNodesOutgoing(**gather_args)([n, edi])
-        eu = Dense(**hidden_dim)(eu)
-        nu = PoolingLocalEdges(**pooling_args)([n, eu, edi])  # Summing for each node connection
-        n = Activation(activation=activation)(nu)
-
-        if use_reconnect:
-            ed, edi = AdjacencyPower(n=2)([n, ed, edi])
-
-        # Pooling
-        i_graph, i_map = PoolingTopK(**top_k_args)([n, ed, edi])
-
-        graph_list.append(i_graph)
-        map_list.append(i_map)
-
-    # U Up
-    ui_graph = i_graph
-    for i in range(depth, 0, -1):
-        o_graph = graph_list[i - 1]
-        i_map = map_list[i - 1]
-        ui_graph = UnPoolingTopK()(o_graph + i_map + ui_graph)
-
-        n, ed, edi = ui_graph
-        # skip connection
-        n = LazyAdd()([n, o_graph[0]])
-        # GCN
-        eu = GatherNodesOutgoing(**gather_args)([n, edi])
-        eu = Dense(**hidden_dim)(eu)
-        nu = PoolingLocalEdges(**pooling_args)([n, eu, edi])  # Summing for each node connection
-        n = Activation(activation=activation)(nu)
-
-        ui_graph = [n, ed, edi]
-
-    # Output embedding choice
-    n = ui_graph[0]
-    if output_embedding == 'graph':
-        out = PoolingNodes(**pooling_args)(n)
-        out = ks.layers.Flatten()(out)  # will be tensor
-        out = MLP(**output_mlp)(out)
-    elif output_embedding == 'node':
-        out = GraphMLP(**output_mlp)(n)
-        if output_to_tensor:  # For tf version < 2.8 cast to tensor below.
-            out = ChangeTensorType(input_tensor_type='ragged', output_tensor_type="tensor")(out)
-    else:
-        raise ValueError("Unsupported graph embedding for mode `Unet`")
-
-    model = ks.models.Model(inputs=[node_input, edge_input, edge_index_input], outputs=out)
-
-    model.__kgcnn_model_version__ = __model_version__
-    return model
+import tensorflow as tf
+from kgcnn.layers.casting import ChangeTensorType
+from kgcnn.layers.gather import GatherNodesOutgoing
+from kgcnn.layers.modules import Dense, Activation, LazyAdd, OptionalInputEmbedding
+from kgcnn.layers.mlp import GraphMLP, MLP
+from kgcnn.layers.pooling import PoolingNodes, PoolingLocalEdges
+from ._topk import PoolingTopK, UnPoolingTopK, AdjacencyPower
+from kgcnn.model.utils import update_model_kwargs
+
+ks = tf.keras
+
+# Keep track of model version from commit date in literature.
+# To be updated if model is changed in a significant way.
+__model_version__ = "2022.11.25"
+
+
+# Implementation of Unet in `tf.keras` from paper:
+# Graph U-Nets
+# by Hongyang Gao, Shuiwang Ji
+# https://arxiv.org/pdf/1905.05178.pdf
+
+model_default = {'name': "Unet",
+                 'inputs': [{'shape': (None,), 'name': "node_attributes", 'dtype': 'float32', 'ragged': True},
+                            {'shape': (None,), 'name': "edge_attributes", 'dtype': 'float32', 'ragged': True},
+                            {'shape': (None, 2), 'name': "edge_indices", 'dtype': 'int64', 'ragged': True}],
+                 'input_embedding': {"node": {"input_dim": 95, "output_dim": 64},
+                                     "edge": {"input_dim": 5, "output_dim": 64}},
+                 'hidden_dim': {'units': 32, 'use_bias': True, 'activation': 'linear'},
+                 'top_k_args': {'k': 0.3, 'kernel_initializer': 'ones'},
+                 'activation': 'relu',
+                 'use_reconnect': True,
+                 'depth': 4,
+                 'pooling_args': {"pooling_method": 'segment_mean'},
+                 'gather_args': {},
+                 'verbose': 10,
+                 'output_embedding': 'graph', "output_to_tensor": True,
+                 'output_mlp': {"use_bias": [True, False], "units": [25, 1], "activation": ['relu', 'sigmoid']}
+                 }
+
+
+@update_model_kwargs(model_default)
+def make_model(inputs: list = None,
+               input_embedding: dict = None,
+               pooling_args: dict = None,
+               gather_args: dict = None,
+               top_k_args: dict = None,
+               depth: int = None,
+               use_reconnect: bool = None,
+               hidden_dim: dict = None,
+               activation: str = None,
+               name: str = None,
+               verbose: int = None,
+               output_embedding: str = None,
+               output_to_tensor: bool = None,
+               output_mlp: dict = None
+               ):
+    r"""Make `U-Net <https://arxiv.org/pdf/1905.05178.pdf>`_ graph network via functional API.
+    Default parameters can be found in :obj:`kgcnn.literature.Unet.model_default` .
+
+    Inputs:
+        list: `[node_attributes, edge_attributes, edge_indices]`
+
+            - node_attributes (tf.RaggedTensor): Node attributes of shape `(batch, None, F)` or `(batch, None)`
+              using an embedding layer.
+            - edge_attributes (tf.RaggedTensor): Edge attributes of shape `(batch, None, F)` or `(batch, None)`
+              using an embedding layer.
+            - edge_indices (tf.RaggedTensor): Index list for edges of shape `(batch, None, 2)`.
+
+    Outputs:
+        tf.Tensor: Graph embeddings of shape `(batch, L)` if :obj:`output_embedding="graph"` .
+
+    Args:
+        inputs (list): List of dictionaries unpacked in :obj:`tf.keras.layers.Input`. Order must match model definition.
+        input_embedding (dict): Dictionary of embedding arguments for nodes etc. unpacked in :obj:`Embedding` layers.
+        depth (int): Number of graph embedding units or depth of the network.
+        pooling_args (dict): Dictionary of layer arguments unpacked in :obj:`PoolingLocalEdges` layers.
+        gather_args (dict): Dictionary of layer arguments unpacked in :obj:`GatherNodesOutgoing` layers.
+        top_k_args (dict): Dictionary of layer arguments unpacked in :obj:`PoolingTopK` layers.
+        use_reconnect (bool): Whether to use :math:`A^2` between pooling.
+        hidden_dim (dict): Dictionary of layer arguments unpacked in hidden `Dense` layer.
+        activation (dict, str): Activation to use.
+        verbose (int): Level of verbosity.
+        name (str): Name of the model.
+        output_embedding (str): Main embedding task for graph network. Either "node", "edge" or "graph".
+        output_to_tensor (bool): Whether to cast model output to :obj:`tf.Tensor` .
+        output_mlp (dict): Dictionary of layer arguments unpacked in the final classification :obj:`MLP` layer block.
+            Defines number of model outputs and activation.
+
+    Returns:
+        :obj:`tf.keras.models.Model`
+    """
+    # Make input
+    node_input = ks.layers.Input(**inputs[0])
+    edge_input = ks.layers.Input(**inputs[1])
+    edge_index_input = ks.layers.Input(**inputs[2])
+
+    # embedding, if no feature dimension
+    n = OptionalInputEmbedding(**input_embedding['node'],
+                               use_embedding=len(inputs[0]['shape']) < 2)(node_input)
+    ed = OptionalInputEmbedding(**input_embedding['edge'],
+                                use_embedding=len(inputs[1]['shape']) < 2)(edge_input)
+    edi = edge_index_input
+
+    # Model
+    n = Dense(**hidden_dim)(n)
+    in_graph = [n, ed, edi]
+    graph_list = [in_graph]
+    map_list = []
+
+    # U Down
+    i_graph = in_graph
+    for i in range(0, depth):
+
+        n, ed, edi = i_graph
+        # GCN layer
+        eu = GatherNodesOutgoing(**gather_args)([n, edi])
+        eu = Dense(**hidden_dim)(eu)
+        nu = PoolingLocalEdges(**pooling_args)([n, eu, edi])  # Summing for each node connection
+        n = Activation(activation=activation)(nu)
+
+        if use_reconnect:
+            ed, edi = AdjacencyPower(n=2)([n, ed, edi])
+
+        # Pooling
+        i_graph, i_map = PoolingTopK(**top_k_args)([n, ed, edi])
+
+        graph_list.append(i_graph)
+        map_list.append(i_map)
+
+    # U Up
+    ui_graph = i_graph
+    for i in range(depth, 0, -1):
+        o_graph = graph_list[i - 1]
+        i_map = map_list[i - 1]
+        ui_graph = UnPoolingTopK()(o_graph + i_map + ui_graph)
+
+        n, ed, edi = ui_graph
+        # skip connection
+        n = LazyAdd()([n, o_graph[0]])
+        # GCN
+        eu = GatherNodesOutgoing(**gather_args)([n, edi])
+        eu = Dense(**hidden_dim)(eu)
+        nu = PoolingLocalEdges(**pooling_args)([n, eu, edi])  # Summing for each node connection
+        n = Activation(activation=activation)(nu)
+
+        ui_graph = [n, ed, edi]
+
+    # Output embedding choice
+    n = ui_graph[0]
+    if output_embedding == 'graph':
+        out = PoolingNodes(**pooling_args)(n)
+        out = ks.layers.Flatten()(out)  # will be tensor
+        out = MLP(**output_mlp)(out)
+    elif output_embedding == 'node':
+        out = GraphMLP(**output_mlp)(n)
+        if output_to_tensor:  # For tf version < 2.8 cast to tensor below.
+            out = ChangeTensorType(input_tensor_type='ragged', output_tensor_type="tensor")(out)
+    else:
+        raise ValueError("Unsupported graph embedding for mode `Unet`")
+
+    model = ks.models.Model(
+        inputs=[node_input, edge_input, edge_index_input],
+        outputs=out,
+        name=name
+    )
+
+    model.__kgcnn_model_version__ = __model_version__
+    return model
```

### Comparing `kgcnn-2.2.4/kgcnn/metrics/loss.py` & `kgcnn-3.0.0/kgcnn/metrics/loss.py`

 * *Files identical despite different names*

### Comparing `kgcnn-2.2.4/kgcnn/metrics/metrics.py` & `kgcnn-3.0.0/kgcnn/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `kgcnn-2.2.4/kgcnn/model/force.py` & `kgcnn-3.0.0/kgcnn/model/force.py`

 * *Files identical despite different names*

### Comparing `kgcnn-2.2.4/kgcnn/model/utils.py` & `kgcnn-3.0.0/kgcnn/model/utils.py`

 * *Files identical despite different names*

### Comparing `kgcnn-2.2.4/kgcnn/mol/base.py` & `kgcnn-3.0.0/kgcnn/molecule/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Module logger
 logging.basicConfig()
 module_logger = logging.getLogger(__name__)
 module_logger.setLevel(logging.INFO)
 
 
 class MolGraphInterface:
-    r"""The `MolGraphInterface` defines the base class interface to handle a molecular graph.
+    r"""The `MolGraphInterface` defines the base class interface to extract a molecular graph.
 
     The method implementation to generate a molecule-instance from smiles etc. can be obtained from different backends
     like `RDkit` . The mol-instance of a chemical informatics package like `RDkit` is treated via composition.
     The interface is designed to extract a graph from a mol instance, not to make a mol object from a graph.
 
     """
```

### Comparing `kgcnn-2.2.4/kgcnn/mol/convert.py` & `kgcnn-3.0.0/kgcnn/molecule/convert.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import logging
 from typing import Callable
-from kgcnn.mol.io import read_mol_list_from_sdf_file, read_xyz_file, read_smiles_file, write_mol_block_list_to_sdf, \
+from kgcnn.molecule.io import read_mol_list_from_sdf_file, read_xyz_file, read_smiles_file, write_mol_block_list_to_sdf, \
     parse_list_to_xyz_str
 from concurrent.futures import ThreadPoolExecutor  # , ProcessPoolExecutor
-from kgcnn.mol.external.ballloon import BalloonInterface
+from kgcnn.molecule.external.ballloon import BalloonInterface
 
 logging.basicConfig()  # Module logger
 module_logger = logging.getLogger(__name__)
 module_logger.setLevel(logging.INFO)
 
 # RDkit
 try:
```

### Comparing `kgcnn-2.2.4/kgcnn/mol/encoder.py` & `kgcnn-3.0.0/kgcnn/molecule/encoder.py`

 * *Files identical despite different names*

### Comparing `kgcnn-2.2.4/kgcnn/mol/external/ballloon.py` & `kgcnn-3.0.0/kgcnn/molecule/external/ballloon.py`

 * *Files identical despite different names*

### Comparing `kgcnn-2.2.4/kgcnn/mol/graph_babel.py` & `kgcnn-3.0.0/kgcnn/molecule/graph_babel.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 import os
 import logging
-from kgcnn.mol.base import MolGraphInterface
+from kgcnn.molecule.base import MolGraphInterface
 from openbabel import openbabel
 
 # Module logger.
 logging.basicConfig()
 module_logger = logging.getLogger(__name__)
 module_logger.setLevel(logging.INFO)
```

### Comparing `kgcnn-2.2.4/kgcnn/mol/graph_rdkit.py` & `kgcnn-3.0.0/kgcnn/molecule/graph_rdkit.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import logging
 
 # For this module please install rdkit. See: https://www.rdkit.org/docs/Install.html
 # or check https://pypi.org/project/rdkit-pypi/ via `pip install rdkit-pypi`
 # or try `conda install -c rdkit rdkit` or `conda install -c conda-forge rdkit`
 # Note: RDkit version >= 2022.9.2 can be installed with `pip install rdkit` only, successor of `rdkit-pypi`.
 # Has been added as requirements to kgcnn.
-from kgcnn.mol.base import MolGraphInterface
+from kgcnn.molecule.base import MolGraphInterface
 
 # Module logger
 logging.basicConfig()
 module_logger = logging.getLogger(__name__)
 module_logger.setLevel(logging.INFO)
 
 # Adjust RDLogger
@@ -61,14 +61,15 @@
         "NumExplicitHs": lambda atom: atom.GetNumExplicitHs(),
         "NumImplicitHs": lambda atom: atom.GetNumImplicitHs(),
         "TotalNumHs": lambda atom: atom.GetTotalNumHs(),
         "IsAromatic": lambda atom: atom.GetIsAromatic(),
         "Isotope": lambda atom: atom.GetIsotope(),
         "TotalValence": lambda atom: atom.GetTotalValence(),
         "Mass": lambda atom: atom.GetMass(),
+        "MassScaled": lambda atom: float((atom.GetMass() - 10.812)/116.092),
         "IsInRing": lambda atom: atom.IsInRing(),
         "Hybridization": lambda atom: atom.GetHybridization(),
         "NoImplicit": lambda atom: atom.GetNoImplicit(),
         "ChiralTag": lambda atom: atom.GetChiralTag(),
         "FormalCharge": lambda atom: atom.GetFormalCharge(),
         "ExplicitValence": lambda atom: atom.GetExplicitValence(),
         "ImplicitValence": lambda atom: atom.GetImplicitValence(),
@@ -84,14 +85,19 @@
         "MolFileRLabel": lambda atom: atom.GetProp('_MolFileRLabel') if atom.HasProp('_MolFileRLabel') else None,
         "GasteigerCharge": lambda atom: atom.GetProp('_GasteigerCharge') if atom.HasProp(
             '_GasteigerCharge') else None,
         "GasteigerHCharge": lambda atom: atom.GetProp('_GasteigerHCharge') if atom.HasProp(
             '_GasteigerHCharge') else None,
         "AtomFeatures": lambda atom: rdkit.Chem.rdMolDescriptors.GetAtomFeatures(atom.GetOwningMol(), atom.GetIdx()),
         "DescribeQuery": lambda atom: atom.DescribeQuery(),
+        "Rvdw": lambda atom: float(rdkit.Chem.GetPeriodicTable().GetRvdw(atom.GetAtomicNum())),
+        "RvdwScaled": lambda atom: float((rdkit.Chem.GetPeriodicTable().GetRvdw(atom.GetAtomicNum()) - 1.5) / 0.6),
+        "Rcovalent": lambda atom: float(rdkit.Chem.GetPeriodicTable().GetRcovalent(atom.GetAtomicNum())),
+        "RcovalentScaled": lambda atom: float(
+            (rdkit.Chem.GetPeriodicTable().GetRcovalent(atom.GetAtomicNum()) - 0.64) / 0.76),
     }
 
     # Dictionary of predefined bond or edge properties
     bond_fun_dict = {
         "BondType": lambda bond: bond.GetBondType(),
         "IsAromatic": lambda bond: bond.GetIsAromatic(),
         "IsConjugated": lambda bond: bond.GetIsConjugated(),
```

### Comparing `kgcnn-2.2.4/kgcnn/mol/io.py` & `kgcnn-3.0.0/kgcnn/molecule/io.py`

 * *Files 0% similar despite different names*

```diff
@@ -179,15 +179,15 @@
                                     "  0  0  0  0  0  0  0  0  0  0 V2000\n",
                                     "M  END\n"]))
                 if i < len(mol_block_list) - 1:
                     file.write("$$$$\n")
 
 
 def read_mol_list_from_sdf_file(filepath, line_by_line=False):
-    """Simple loader to load a SDF file by only splitting.
+    """Simple loader to load an SDF file by only splitting.
 
     Args:
         filepath (str): File path for SDF file.
         line_by_line (bool): Whether to read SDF file line by line.
 
     Returns:
         list: List of mol blocks as string.
```

### Comparing `kgcnn-2.2.4/kgcnn/mol/methods.py` & `kgcnn-3.0.0/kgcnn/molecule/methods.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 
-from kgcnn.data.transform.scaler.mol import ExtensiveMolecularScaler
+from kgcnn.data.transform.scaler.molecule import ExtensiveMolecularScaler
 
 
 global_proton_dict = {'H': 1, 'He': 2, 'Li': 3, 'Be': 4, 'B': 5, 'C': 6, 'N': 7, 'O': 8, 'F': 9, 'Ne': 10, 'Na': 11,
                       'Mg': 12, 'Al': 13, 'Si': 14, 'P': 15, 'S': 16, 'Cl': 17, 'Ar': 18, 'K': 19, 'Ca': 20,
                       'Sc': 21, 'Ti': 22, 'V': 23, 'Cr': 24, 'Mn': 25, 'Fe': 26, 'Co': 27, 'Ni': 28, 'Cu': 29,
                       'Zn': 30, 'Ga': 31, 'Ge': 32, 'As': 33, 'Se': 34, 'Br': 35, 'Kr': 36, 'Rb': 37, 'Sr': 38,
                       'Y': 39, 'Zr': 40, 'Nb': 41, 'Mo': 42, 'Tc': 43, 'Ru': 44, 'Rh': 45, 'Pd': 46, 'Ag': 47,
```

### Comparing `kgcnn-2.2.4/kgcnn/mol/serial.py` & `kgcnn-3.0.0/kgcnn/molecule/serial.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from kgcnn.mol.encoder import OneHotEncoder
+from kgcnn.molecule.encoder import OneHotEncoder
 
 
 def deserialize_encoder(encoder_identifier):
     """Deserialization of encoder class.
 
     Args:
         encoder_identifier: Identifier, class or function of an encoder.
```

### Comparing `kgcnn-2.2.4/kgcnn/moldyn/ase_calc.py` & `kgcnn-3.0.0/kgcnn/molecule/dynamics/ase_calc.py`

 * *Files identical despite different names*

### Comparing `kgcnn-2.2.4/kgcnn/moldyn/base.py` & `kgcnn-3.0.0/kgcnn/molecule/dynamics/base.py`

 * *Files identical despite different names*

### Comparing `kgcnn-2.2.4/kgcnn/ops/activ.py` & `kgcnn-3.0.0/kgcnn/ops/activ.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import tensorflow as tf
 ks = tf.keras
 
 
 @tf.keras.utils.register_keras_serializable(package='kgcnn', name='shifted_softplus')
 def shifted_softplus(x):
-    r"""Shifted softplus activation function.
+    r"""Shifted soft-plus activation function.
     
     Args:
         x (tf.Tensor): Single values to apply activation with tf.keras functions.
     
     Returns:
         tf.Tensor: Output tensor computed as :math:`\log(e^{x}+1) - \log(2)`.
     """
     return ks.activations.softplus(x) - ks.backend.log(2.0)
 
 
 @tf.keras.utils.register_keras_serializable(package='kgcnn', name='softplus2')
 def softplus2(x):
-    r"""Softplus function that is :math:`0` at :math:`x=0`, the implementation aims at avoiding overflow
+    r"""Soft-plus function that is :math:`0` at :math:`x=0`, the implementation aims at avoiding overflow
     :math:`\log(e^{x}+1) - \log(2)`.
     
     Args:
         x (tf.Tensor): Single values to apply activation with tf.keras functions.
     
     Returns:
          tf.Tensor: Output tensor computed as :math:`\log(e^{x}+1) - \log(2)`.
```

### Comparing `kgcnn-2.2.4/kgcnn/ops/axis.py` & `kgcnn-3.0.0/kgcnn/ops/axis.py`

 * *Files identical despite different names*

### Comparing `kgcnn-2.2.4/kgcnn/ops/partition.py` & `kgcnn-3.0.0/kgcnn/ops/partition.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,19 +144,19 @@
 
     # Just gather the splits i.e. index offset for each graph id
     shift_index = tf.gather(nod_splits, edge_ids)
 
     # Expand dimension to broadcast to indices for suitable axis
     # The shift_index is always 1D tensor. Add further (N, 1, 1, ...)
     for i in range(1, tensor_index.shape.rank):
-        shift_index = tf.expand_dims(shift_index,axis=-1)
+        shift_index = tf.expand_dims(shift_index, axis=-1)
 
     # Add or remove batch offset from index tensor
     if to_indexing == 'batch' and from_indexing == 'sample':
         indexlist = tensor_index + tf.cast(shift_index, dtype=tensor_index.dtype)
     elif to_indexing == 'sample' and from_indexing == 'batch':
         indexlist = tensor_index - tf.cast(shift_index, dtype=tensor_index.dtype)
     else:
         raise TypeError("ERROR:kgcnn: Unknown index change, use: 'sample', 'batch', ...")
 
     out = indexlist
-    return out
+    return out
```

### Comparing `kgcnn-2.2.4/kgcnn/ops/polynom.py` & `kgcnn-3.0.0/kgcnn/ops/polynom.py`

 * *Files identical despite different names*

### Comparing `kgcnn-2.2.4/kgcnn/ops/ragged.py` & `kgcnn-3.0.0/kgcnn/ops/ragged.py`

 * *Files identical despite different names*

### Comparing `kgcnn-2.2.4/kgcnn/ops/scatter.py` & `kgcnn-3.0.0/kgcnn/ops/scatter.py`

 * *Files identical despite different names*

### Comparing `kgcnn-2.2.4/kgcnn/ops/segment.py` & `kgcnn-3.0.0/kgcnn/ops/segment.py`

 * *Files identical despite different names*

### Comparing `kgcnn-2.2.4/kgcnn/training/callbacks.py` & `kgcnn-3.0.0/kgcnn/training/callbacks.py`

 * *Files identical despite different names*

### Comparing `kgcnn-2.2.4/kgcnn/training/history.py` & `kgcnn-3.0.0/kgcnn/training/history.py`

 * *Files identical despite different names*

### Comparing `kgcnn-2.2.4/kgcnn/training/optimizer.py` & `kgcnn-3.0.0/kgcnn/training/optimizer.py`

 * *Files identical despite different names*

### Comparing `kgcnn-2.2.4/kgcnn/training/schedule.py` & `kgcnn-3.0.0/kgcnn/training/schedule.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,49 +3,63 @@
 
 
 @tf.keras.utils.register_keras_serializable(package='kgcnn', name='LinearWarmupExponentialDecay')
 class LinearWarmupExponentialDecay(tf.optimizers.schedules.LearningRateSchedule):
     r"""This schedule combines a linear warmup with an exponential decay.
     Combines :obj:` tf.optimizers.schedules.PolynomialDecay` with an actual increase during warmup
     and :obj:`tf.optimizers.schedules.ExponentialDecay` after.
-    Used by `DimeNetPP <https://arxiv.org/abs/2011.14115>`_.
+
+    Introduced by `DimeNetPP <https://arxiv.org/abs/2011.14115>`__ .
+
     The closed-from learning rate schedule for learning rate :math:`\eta` for :math:`s_0` warmup and decay
-    :math:`S_\tau` is given as a function of steps :math:`s` below.
+    :math:`S_\tau` is given as a function of steps :math:`s` below (deduced from documentation of keras modules).
 
     .. math::
 
         \eta (s) = \eta_0 \;  \gamma ^ {s / S_\tau}  \; [1 - \frac{s_0-1}{s_0} \frac{s_0 - \text{min}(s_0, S)}{s_0}]
+
+    This class has been updated to be compatible with `GemNet <https://arxiv.org/abs/2106.08903>`__ training.
+
     """
 
-    def __init__(self, learning_rate, warmup_steps, decay_steps, decay_rate):
+    def __init__(self, learning_rate, warmup_steps, decay_steps, decay_rate, staircase: bool = False):
         """Initialize class.
 
         Args:
             learning_rate: Learning rate to use.
             warmup_steps: Number of warmup steps.
             decay_steps: Number of which to decay the learning rate.
             decay_rate: Factor to reduce the learning rate.
+            staircase (bool): If True use staircase decay and not (continuous) exponential decay.
         """
         super().__init__()
         self._input_config_settings = {"learning_rate": learning_rate, "warmup_steps": warmup_steps,
-                                       "decay_steps": decay_steps, "decay_rate": decay_rate}
+                                       "decay_steps": decay_steps, "decay_rate": decay_rate, "staircase": staircase}
         self.warmup = tf.optimizers.schedules.PolynomialDecay(
             1 / warmup_steps, warmup_steps, end_learning_rate=1)
         self.decay = tf.optimizers.schedules.ExponentialDecay(
-            learning_rate, decay_steps, decay_rate)
+            learning_rate, decay_steps, decay_rate, staircase=staircase)
 
     def __call__(self, step):
         """Decay learning rate as a functions of steps.
 
         Args:
             step: Current step of training.
 
         Returns:
             float: New learning rate.
         """
         return self.warmup(step) * self.decay(step)
 
+    @property
+    def initial_learning_rate(self):
+        return self.decay.initial_learning_rate
+
+    @initial_learning_rate.setter
+    def initial_learning_rate(self, value):
+        self.decay.initial_learning_rate = value
+
     def get_config(self):
         """Get config for this class."""
         config = {}
         config.update(self._input_config_settings)
         return config
```

### Comparing `kgcnn-2.2.4/kgcnn/training/scheduler.py` & `kgcnn-3.0.0/kgcnn/training/scheduler.py`

 * *Files identical despite different names*

### Comparing `kgcnn-2.2.4/kgcnn/utils/devices.py` & `kgcnn-3.0.0/kgcnn/utils/devices.py`

 * *Files identical despite different names*

### Comparing `kgcnn-2.2.4/kgcnn/utils/plots.py` & `kgcnn-3.0.0/kgcnn/utils/plots.py`

 * *Files identical despite different names*

### Comparing `kgcnn-2.2.4/kgcnn/utils/serial.py` & `kgcnn-3.0.0/kgcnn/utils/serial.py`

 * *Files identical despite different names*

### Comparing `kgcnn-2.2.4/kgcnn/xai/base.py` & `kgcnn-3.0.0/kgcnn/literature/GNNExplain/_xai/_base.py`

 * *Files identical despite different names*

### Comparing `kgcnn-2.2.4/kgcnn/xai/testing.py` & `kgcnn-3.0.0/kgcnn/literature/GNNExplain/_xai/_testing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import random
 import typing as t
 
 import numpy as np
 import tensorflow as tf
-import tensorflow.keras as ks
-
-from kgcnn.layers.conv.gat_conv import AttentionHeadGATV2
+from kgcnn.layers.attention import AttentionHeadGATV2
 from kgcnn.layers.modules import DenseEmbedding
 from kgcnn.layers.pooling import PoolingGlobalEdges
 from kgcnn.data.utils import ragged_tensor_from_nested_numpy
 
+ks = tf.keras
 
 # This is a very simple mock implementation, because to test the explanation methods we need some sort
 # of a model as basis and this model will act as such.
 class Model(ks.models.Model):
 
     def __init__(self,
                  num_targets: int = 1):
```

### Comparing `kgcnn-2.2.4/kgcnn/xai/utils.py` & `kgcnn-3.0.0/kgcnn/literature/GNNExplain/_xai/_utils.py`

 * *Files identical despite different names*

### Comparing `kgcnn-2.2.4/kgcnn.egg-info/PKG-INFO` & `kgcnn-3.0.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: kgcnn
-Version: 2.2.4
-Summary: General Base Layers for Graph Convolutions with tensorflow.keras
-Home-page: https://github.com/aimat-lab/gcnn_keras
-Author: Patrick Reiser
-Author-email: patrick.reiser@kit.edu
-License: UNKNOWN
-Keywords: materials,science,machine,learning,deep,graph,networks,neural
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Classifier: Topic :: Scientific/Engineering :: Physics
-Classifier: Topic :: Scientific/Engineering :: Chemistry
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Description-Content-Type: text/markdown
-Provides-Extra: openbabel
-License-File: LICENSE
-License-File: AUTHORS
-
 ![GitHub release (latest by date)](https://img.shields.io/github/v/release/aimat-lab/gcnn_keras)
 [![Documentation Status](https://readthedocs.org/projects/kgcnn/badge/?version=latest)](https://kgcnn.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/kgcnn.svg)](https://badge.fury.io/py/kgcnn)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/kgcnn)
 [![kgcnn_unit_tests](https://github.com/aimat-lab/gcnn_keras/actions/workflows/unittests.yml/badge.svg)](https://github.com/aimat-lab/gcnn_keras/actions/workflows/unittests.yml)
 [![DOI](https://img.shields.io/badge/DOI-10.1016%2Fj.simpa.2021.100095%20-blue)](https://doi.org/10.1016/j.simpa.2021.100095)
 ![GitHub](https://img.shields.io/github/license/aimat-lab/gcnn_keras)
@@ -43,15 +21,15 @@
 
 <a name="general"></a>
 # General
 
 The package in [kgcnn](kgcnn) contains several layer classes to build up graph convolution models. 
 Some models are given as an example.
 A [documentation](https://kgcnn.readthedocs.io/en/latest/index.html) is generated in [docs](docs).
-Focus of [kgcnn](kgcnn) is (batched) graph learning for molecules [kgcnn.mol](kgcnn/mol) and materials [kgcnn.crystal](kgcnn/crystal).
+Focus of [kgcnn](kgcnn) is (batched) graph learning for molecules [kgcnn.molecule](kgcnn/molecule) and materials [kgcnn.crystal](kgcnn/crystal).
 If you want to get in contact, feel free to [discuss](https://github.com/aimat-lab/gcnn_keras/discussions). 
 
 <a name="requirements"></a>
 # Requirements
 
 
 Standard python package requirements are placed in the `setup.py` and are installed automatically ([kgcnn](https://github.com/aimat-lab/gcnn_keras) >=2.2). 
@@ -157,44 +135,50 @@
     def update_nodes(self, inputs, **kwargs):
         nodes, nodes_update = inputs
         return self.add([nodes, nodes_update])
 ```
 
 <a name="literature"></a>
 # Literature
-A version of the following models and variants thereof are implemented in [literature](kgcnn/literature):
-* **[GCN](kgcnn/literature/GCN.py)**: [Semi-Supervised Classification with Graph Convolutional Networks](https://arxiv.org/abs/1609.02907) by Kipf et al. (2016)
-* **[Schnet](kgcnn/literature/Schnet.py)**: [SchNet – A deep learning architecture for molecules and materials ](https://aip.scitation.org/doi/10.1063/1.5019779) by Schütt et al. (2017)
-* **[GAT](kgcnn/literature/GAT.py)**: [Graph Attention Networks](https://arxiv.org/abs/1710.10903) by Veličković et al. (2018)
-* **[GraphSAGE](kgcnn/literature/GraphSAGE.py)**: [Inductive Representation Learning on Large Graphs](http://arxiv.org/abs/1706.02216) by Hamilton et al. (2017)
-* **[DimeNetPP](kgcnn/literature/DimeNetPP.py)**: [Fast and Uncertainty-Aware Directional Message Passing for Non-Equilibrium Molecules](https://arxiv.org/abs/2011.14115) by Klicpera et al. (2020)
-* **[GNNExplainer](kgcnn/literature/GNNExplain.py)**: [GNNExplainer: Generating Explanations for Graph Neural Networks](https://arxiv.org/abs/1903.03894) by Ying et al. (2019)
-* **[AttentiveFP](kgcnn/literature/AttentiveFP.py)**: [Pushing the Boundaries of Molecular Representation for Drug Discovery with the Graph Attention Mechanism](https://pubs.acs.org/doi/10.1021/acs.jmedchem.9b00959) by Xiong et al. (2019)
+The following models, proposed in literature, have a module in [literature](kgcnn/literature). The module usually exposes a `make_model` function
+to create a ``tf.keras.models.Model``, which features ragged tensor in- or output. The models can but must not be build completely from `kgcnn.layers` and can for example include
+original implementations (with proper licencing).
+
+* **[GCN](kgcnn/literature/GCN)**: [Semi-Supervised Classification with Graph Convolutional Networks](https://arxiv.org/abs/1609.02907) by Kipf et al. (2016)
+* **[Schnet](kgcnn/literature/Schnet)**: [SchNet – A deep learning architecture for molecules and materials ](https://aip.scitation.org/doi/10.1063/1.5019779) by Schütt et al. (2017)
+* **[GAT](kgcnn/literature/GAT)**: [Graph Attention Networks](https://arxiv.org/abs/1710.10903) by Veličković et al. (2018)
+* **[GraphSAGE](kgcnn/literature/GraphSAGE)**: [Inductive Representation Learning on Large Graphs](http://arxiv.org/abs/1706.02216) by Hamilton et al. (2017)
+* **[DimeNetPP](kgcnn/literature/DimeNetPP)**: [Fast and Uncertainty-Aware Directional Message Passing for Non-Equilibrium Molecules](https://arxiv.org/abs/2011.14115) by Klicpera et al. (2020)
+* **[GNNExplainer](kgcnn/literature/GNNExplain)**: [GNNExplainer: Generating Explanations for Graph Neural Networks](https://arxiv.org/abs/1903.03894) by Ying et al. (2019)
+* **[AttentiveFP](kgcnn/literature/AttentiveFP)**: [Pushing the Boundaries of Molecular Representation for Drug Discovery with the Graph Attention Mechanism](https://pubs.acs.org/doi/10.1021/acs.jmedchem.9b00959) by Xiong et al. (2019)
 
 <details>
 <summary> ... and many more <b>(click to expand)</b>.</summary>
 
-* **[INorp](kgcnn/literature/INorp.py)**: [Interaction Networks for Learning about Objects,Relations and Physics](https://arxiv.org/abs/1612.00222) by Battaglia et al. (2016)
-* **[Megnet](kgcnn/literature/Megnet.py)**: [Graph Networks as a Universal Machine Learning Framework for Molecules and Crystals](https://doi.org/10.1021/acs.chemmater.9b01294) by Chen et al. (2019)
-* **[NMPN](kgcnn/literature/NMPN.py)**: [Neural Message Passing for Quantum Chemistry](http://arxiv.org/abs/1704.01212) by Gilmer et al. (2017)
-* **[Unet](kgcnn/literature/Unet.py)**: [Graph U-Nets](http://proceedings.mlr.press/v97/gao19a/gao19a.pdf) by H. Gao and S. Ji (2019)
-* **[GATv2](kgcnn/literature/GATv2.py)**: [How Attentive are Graph Attention Networks?](https://arxiv.org/abs/2105.14491) by Brody et al. (2021)
-* **[GIN](kgcnn/literature/GIN.py)**: [How Powerful are Graph Neural Networks?](https://arxiv.org/abs/1810.00826) by Xu et al. (2019)
-* **[PAiNN](kgcnn/literature/PAiNN.py)**: [Equivariant message passing for the prediction of tensorial properties and molecular spectra](https://arxiv.org/pdf/2102.03150.pdf) by Schütt et al. (2020)
-* **[DMPNN](kgcnn/literature/DMPNN.py)**: [Analyzing Learned Molecular Representations for Property Prediction](https://pubs.acs.org/doi/abs/10.1021/acs.jcim.9b00237) by Yang et al. (2019)
-* **[HamNet](kgcnn/literature/HamNet.py)**: [HamNet: Conformation-Guided Molecular Representation with Hamiltonian Neural Networks](https://arxiv.org/abs/2105.03688) by Li et al. (2021)
-* **[CGCNN](kgcnn/literature/CGCNN.py)**: [Crystal Graph Convolutional Neural Networks for an Accurate and Interpretable Prediction of Material Properties](https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.120.145301) by Xie et al. (2018)
-* **[CMPNN](kgcnn/literature/CMPNN.py)**: [Communicative Representation Learning on Attributed Molecular Graphs](https://www.ijcai.org/proceedings/2020/0392.pdf) by Song et al. (2020)
-* **[EGNN](kgcnn/literature/EGNN.py)**: [E(n) Equivariant Graph Neural Networks](https://arxiv.org/abs/2102.09844) by Satorras et al. (2021)
-* **[MAT](kgcnn/literature/MAT.py)**: [Molecule Attention Transformer](https://arxiv.org/abs/2002.08264) by Maziarka et al. (2020)
-* **[MXMNet](kgcnn/literature/MXMNet.py)**: [Molecular Mechanics-Driven Graph Neural Network with Multiplex Graph for Molecular Structures](https://arxiv.org/abs/2011.07457) by Zhang et al. (2020)
-* **[RGCN](kgcnn/literature/RGCN.py)**: [Modeling Relational Data with Graph Convolutional Networks](https://arxiv.org/abs/1703.06103) by Schlichtkrull et al. (2017)
-* **[GNNFilm](kgcnn/literature/GNNFilm.py)**: [GNN-FiLM: Graph Neural Networks with Feature-wise Linear Modulation](https://arxiv.org/abs/1906.12192) by Marc Brockschmidt (2020)
-* **[HDNNP2nd](kgcnn/literature/HDNNP2nd.py)**: [Atom-centered symmetry functions for constructing high-dimensional neural network potentials](https://aip.scitation.org/doi/abs/10.1063/1.3553717) by Jörg Behler (2011)
-* **[HDNNP4th](kgcnn/literature/HDNNP4th.py)**: [A fourth-generation high-dimensional neural network potential with accurate electrostatics including non-local charge transfer](https://www.nature.com/articles/s41467-020-20427-2) by Ko et al. (2021)
+* **[INorp](kgcnn/literature/INorp)**: [Interaction Networks for Learning about Objects,Relations and Physics](https://arxiv.org/abs/1612.00222) by Battaglia et al. (2016)
+* **[Megnet](kgcnn/literature/Megnet)**: [Graph Networks as a Universal Machine Learning Framework for Molecules and Crystals](https://doi.org/10.1021/acs.chemmater.9b01294) by Chen et al. (2019)
+* **[NMPN](kgcnn/literature/NMPN)**: [Neural Message Passing for Quantum Chemistry](http://arxiv.org/abs/1704.01212) by Gilmer et al. (2017)
+* **[Unet](kgcnn/literature/Unet)**: [Graph U-Nets](http://proceedings.mlr.press/v97/gao19a/gao19a.pdf) by H. Gao and S. Ji (2019)
+* **[GATv2](kgcnn/literature/GATv2)**: [How Attentive are Graph Attention Networks?](https://arxiv.org/abs/2105.14491) by Brody et al. (2021)
+* **[GIN](kgcnn/literature/GIN)**: [How Powerful are Graph Neural Networks?](https://arxiv.org/abs/1810.00826) by Xu et al. (2019)
+* **[PAiNN](kgcnn/literature/PAiNN)**: [Equivariant message passing for the prediction of tensorial properties and molecular spectra](https://arxiv.org/pdf/2102.03150.pdf) by Schütt et al. (2020)
+* **[DMPNN](kgcnn/literature/DMPNN)**: [Analyzing Learned Molecular Representations for Property Prediction](https://pubs.acs.org/doi/abs/10.1021/acs.jcim.9b00237) by Yang et al. (2019)
+* **[HamNet](kgcnn/literature/HamNet)**: [HamNet: Conformation-Guided Molecular Representation with Hamiltonian Neural Networks](https://arxiv.org/abs/2105.03688) by Li et al. (2021)
+* **[CGCNN](kgcnn/literature/CGCNN)**: [Crystal Graph Convolutional Neural Networks for an Accurate and Interpretable Prediction of Material Properties](https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.120.145301) by Xie et al. (2018)
+* **[CMPNN](kgcnn/literature/CMPNN)**: [Communicative Representation Learning on Attributed Molecular Graphs](https://www.ijcai.org/proceedings/2020/0392.pdf) by Song et al. (2020)
+* **[EGNN](kgcnn/literature/EGNN)**: [E(n) Equivariant Graph Neural Networks](https://arxiv.org/abs/2102.09844) by Satorras et al. (2021)
+* **[MAT](kgcnn/literature/MAT)**: [Molecule Attention Transformer](https://arxiv.org/abs/2002.08264) by Maziarka et al. (2020)
+* **[MXMNet](kgcnn/literature/MXMNet)**: [Molecular Mechanics-Driven Graph Neural Network with Multiplex Graph for Molecular Structures](https://arxiv.org/abs/2011.07457) by Zhang et al. (2020)
+* **[RGCN](kgcnn/literature/RGCN)**: [Modeling Relational Data with Graph Convolutional Networks](https://arxiv.org/abs/1703.06103) by Schlichtkrull et al. (2017)
+* **[GNNFilm](kgcnn/literature/GNNFilm)**: [GNN-FiLM: Graph Neural Networks with Feature-wise Linear Modulation](https://arxiv.org/abs/1906.12192) by Marc Brockschmidt (2020)
+* **[HDNNP2nd](kgcnn/literature/HDNNP2nd)**: [Atom-centered symmetry functions for constructing high-dimensional neural network potentials](https://aip.scitation.org/doi/abs/10.1063/1.3553717) by Jörg Behler (2011)
+* **[HDNNP4th](kgcnn/literature/HDNNP4th)**: [A fourth-generation high-dimensional neural network potential with accurate electrostatics including non-local charge transfer](https://www.nature.com/articles/s41467-020-20427-2) by Ko et al. (2021)
+* **[DGIN](kgcnn/literature/DGIN)**: [Improved Lipophilicity and Aqueous Solubility Prediction with Composite Graph Neural Networks ](https://pubmed.ncbi.nlm.nih.gov/34684766/) by Wieder et al. (2021)
+* **[MoGAT](kgcnn/literature/MoGAT)**: [Multi-order graph attention network for water solubility prediction and interpretation](https://www.nature.com/articles/s41598-022-25701-5) by Lee et al. (2023)
+* **[rGIN](kgcnn/literature/rGIN)** [Random Features Strengthen Graph Neural Networks](https://arxiv.org/abs/2002.03155) by Sato et al. (2020)
 </details>
 
 
 <a name="data"></a>
 # Data
 
 How to construct ragged tensors is shown [above](#implementation-details-input). 
@@ -322,9 +306,7 @@
 }
 ```
 
 <a name="references"></a>
 # References
 
 - https://www.tensorflow.org/api_docs/python/tf/RaggedTensor
-
-
```

### Comparing `kgcnn-2.2.4/setup.py` & `kgcnn-3.0.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf8") as fh:
     long_description = fh.read()
 
 setup(
     name="kgcnn",
-    version="2.2.4",  # If version is updated, change version in `kgcnn.__init__` too. (and update changelog)
+    version="3.0.0",  # If version is updated, change version in `kgcnn.__init__` too. (and update changelog)
     author="Patrick Reiser",
     author_email="patrick.reiser@kit.edu",
     description="General Base Layers for Graph Convolutions with tensorflow.keras",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/aimat-lab/gcnn_keras",
     install_requires=[
@@ -18,32 +18,31 @@
         "scikit-learn>=1.1.3",
         "pandas>=1.5.2",
         "scipy>=1.9.3",
         "matplotlib>=3.6.0",
         "rdkit>=2022.9.2",
         "pymatgen>=2022.11.7",
         "tensorflow>=2.9.0",
-        # "tensorflow-gpu>=2.10.0",  # No longer used in tensorflow.
         "tensorflow-addons>=0.18.0",
         "keras-tuner>=1.1.3",
         "requests>=2.28.1",
         "networkx>=2.8.8",
         "sympy>=1.11.1",
         "pyyaml>=6.0",
         "ase>=3.22.1",
         "click>=7.1.2",
-        "visual_graph_datasets>=0.7.1",
-        "brotli>=1.0.9"
+        "brotli>=1.0.9",
+        "pyxtal>=0.5.5"
     ],
     extras_require={
         "openbabel": ["openbabel"],
     },
     packages=find_packages(),
     include_package_data=True,
-    package_data={"kgcnn": ["*.json", "*.yaml"]},
+    package_data={"kgcnn": ["*.json", "*.yaml", "*.csv"]},
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
         "Intended Audience :: Science/Research",
         "Topic :: Scientific/Engineering :: Information Analysis",
         "Topic :: Scientific/Engineering :: Physics",
         "Topic :: Scientific/Engineering :: Chemistry",
```

### Comparing `kgcnn-2.2.4/test/test_adj.py` & `kgcnn-3.0.0/test/test_graph_methods.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 import unittest
 
-from kgcnn.graph.adj import add_edges_reverse_indices, add_self_loops_to_edge_indices
-from kgcnn.graph.adj import get_angle_indices, get_angle, get_angle_between_edges
+from kgcnn.graph.methods import add_edges_reverse_indices, add_self_loops_to_edge_indices
+from kgcnn.graph.methods import get_angle_indices, get_angle, get_angle_between_edges
 
 
 class ReverseEdges(unittest.TestCase):
 
     def test_add_indices_only_no_order(self):
         indices = np.array([[0, 0], [1, 2], [2, 3], [0, 1]])
         result = add_edges_reverse_indices(indices)
```

### Comparing `kgcnn-2.2.4/test/test_connect.py` & `kgcnn-3.0.0/kgcnn/literature/Unet/_test_connect.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 import tensorflow as tf
 import unittest
 
-from kgcnn.layers.pool.topk import AdjacencyPower
+from kgcnn.literature.Unet._topk import AdjacencyPower
 
 nods = tf.ragged.constant([[[5.0],[5.0],[5.0]],[[5.0],[5.0],[5.0]]],ragged_rank=1)
 inds = tf.ragged.constant([[[0,1],[0,2],[1,0],[2,0]],[[0,0],[1,1],[2,2]]],ragged_rank=1)
 edges = tf.ragged.constant([[[1.0],[1.0],[1.0],[1.0]],[[1.0],[1.0],[1.0]]],ragged_rank=1)
 
 edge_index = inds.values
 edge = edges.values
@@ -22,14 +22,14 @@
     edges = tf.ragged.constant([[[1.0], [1.0], [1.0], [1.0]], [[1.0], [1.0], [1.0]]], ragged_rank=1)
 
     def test_attention_pooling(self):
 
         result = AdjacencyPower()([self.nods,self.edges,self.inds])
         print(result)
 
-        self.assertTrue(np.max(np.abs(result[1][0].numpy() -  np.array([[0, 0], [1, 1], [1, 2], [2, 1], [2, 2]]))) < 1e-4)
+        self.assertTrue(np.max(np.abs(result[1][0].numpy() - np.array([[0, 0], [1, 1], [1, 2], [2, 1], [2, 2]]))) < 1e-4)
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kgcnn-2.2.4/test/test_conv_attention.py` & `kgcnn-3.0.0/test/test_layers_attention.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,20 +3,19 @@
 
 import numpy as np
 import tensorflow as tf
 
 
 from kgcnn.layers.casting import ChangeTensorType
 from kgcnn.layers.base import GraphBaseLayer
-from kgcnn.layers.conv.gat_conv import PoolingLocalEdgesAttention
-from kgcnn.layers.conv.gat_conv import AttentionHeadGAT
-from kgcnn.layers.conv.gat_conv import MultiHeadGATV2Layer
+from kgcnn.layers.attention import PoolingLocalEdgesAttention
+from kgcnn.layers.attention import AttentionHeadGAT, MultiHeadGATV2Layer
 
 
-class TestAttentionDisjoint(unittest.TestCase):
+class TestPoolingLocalEdgesAttention(unittest.TestCase):
 
     n1 = [[[1.0], [6.0], [1.0], [6.0], [1.0], [1.0], [6.0], [6.0]],
           [[6.0], [1.0], [1.0], [1.0], [7.0], [1.0], [6.0], [8.0], [6.0], [1.0], [6.0], [7.0], [1.0], [1.0], [1.0]]]
     ei1 = [[[0, 1], [1, 0], [1, 6], [2, 3], [3, 2], [3, 5], [3, 7], [4, 7], [5, 3], [6, 1], [6, 7], [7, 3], [7, 4],
             [7, 6]],
            [[0, 6], [0, 8], [0, 9], [1, 11], [2, 4], [3, 4], [4, 2], [4, 3], [4, 6], [5, 10], [6, 0], [6, 4], [6, 14],
             [7, 8], [8, 0], [8, 7], [8, 11], [9, 0], [10, 5], [10, 11], [10, 12], [10, 13], [11, 1], [11, 8], [11, 10],
```

### Comparing `kgcnn-2.2.4/test/test_data_base.py` & `kgcnn-3.0.0/test/test_data_base.py`

 * *Files identical despite different names*

### Comparing `kgcnn-2.2.4/test/test_data_moleculenet.py` & `kgcnn-3.0.0/test/test_data_moleculenet.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 from pprint import pprint
 
 import numpy as np
 import pandas as pd
 from rdkit import RDLogger
 RDLogger.DisableLog('rdApp.*')
 
-from kgcnn.mol.graph_rdkit import MolecularGraphRDKit
+from kgcnn.molecule.graph_rdkit import MolecularGraphRDKit
 from kgcnn.data.moleculenet import MoleculeNetDataset, map_molecule_callbacks
-from kgcnn.mol.encoder import OneHotEncoder
+from kgcnn.molecule.encoder import OneHotEncoder
 
 from .utils import ASSETS_PATH
 
 
 class TestMoleculeNetDataset(unittest.TestCase):
 
     # -- UNITTESTS --
```

### Comparing `kgcnn-2.2.4/test/test_gather.py` & `kgcnn-3.0.0/test/test_layers_pooling.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import unittest
 
 import numpy as np
 import tensorflow as tf
 
+from kgcnn.layers.pooling import PoolingLocalEdgesLSTM
 from kgcnn.layers.gather import GatherNodes
+from kgcnn.layers.modules import LazyConcatenate
 
 
-class TestGather(unittest.TestCase):
+class TestPoolingLocalEdgesLSTM(unittest.TestCase):
 
     n1 = [[[1.0], [6.0], [1.0], [6.0], [1.0], [1.0], [6.0], [6.0]],
           [[6.0], [1.0], [1.0], [1.0], [7.0], [1.0], [6.0], [8.0], [6.0], [1.0], [6.0], [7.0], [1.0], [1.0], [1.0]]]
     ei1 = [[[0, 1], [1, 0], [1, 6], [2, 3], [3, 2], [3, 5], [3, 7], [4, 7], [5, 3], [6, 1], [6, 7], [7, 3], [7, 4],
             [7, 6]],
            [[0, 6], [0, 8], [0, 9], [1, 11], [2, 4], [3, 4], [4, 2], [4, 3], [4, 6], [5, 10], [6, 0], [6, 4], [6, 14],
             [7, 8], [8, 0], [8, 7], [8, 11], [9, 0], [10, 5], [10, 11], [10, 12], [10, 13], [11, 1], [11, 8], [11, 10],
@@ -21,35 +23,23 @@
           [[0.25], [0.25], [0.35355339059327373], [0.35355339059327373], [0.35355339059327373], [0.35355339059327373],
            [0.35355339059327373], [0.35355339059327373], [0.25], [0.3162277660168379], [0.25], [0.25],
            [0.35355339059327373], [0.35355339059327373], [0.25], [0.35355339059327373], [0.25], [0.35355339059327373],
            [0.3162277660168379], [0.22360679774997896], [0.3162277660168379], [0.3162277660168379],
            [0.35355339059327373], [0.25], [0.22360679774997896], [0.3162277660168379], [0.3162277660168379],
            [0.35355339059327373]]]
 
-    def test_gather_nodes_concat(self):
-        node = tf.ragged.constant(self.n1, ragged_rank=1, inner_shape=(1,))
-        edgeind = tf.ragged.constant(self.ei1, ragged_rank=1, inner_shape=(2,))
-
-        gathered_nodes_concat = GatherNodes()([node,edgeind])
-        np_gather = np.reshape(np.array(self.n1[1])[np.array(self.ei1[1])],(28,2*1))
-        test = np.sum(np.abs(np.array(gathered_nodes_concat[1]) - np_gather)) < 1e-6
-        self.assertTrue(test)
-
-    def test_gather_nodes(self):
-        node = tf.ragged.constant(self.n1, ragged_rank=1, inner_shape=(1,))
-        edgeind = tf.ragged.constant(self.ei1, ragged_rank=1, inner_shape=(2,))
-
-        gathered_nodes = GatherNodes(concat_axis=None)([node, edgeind])
-        np_gather = np.array(self.n1[1])[np.array(self.ei1[1])]
-        test = np.sum(np.abs(np.array(gathered_nodes[1]) - np_gather)) < 1e-6
-        self.assertTrue(test)
-
-    # def test_gather_empty(self):
-    #     node = tf.ragged.constant(self.n1, ragged_rank=1, inner_shape=(1,))
-    #
-    #     ei2 = tf.RaggedTensor.from_row_lengths(tf.constant([],dtype=tf.int64),tf.constant([0,0],dtype=tf.int64))
-    #     gather_empty = GatherNodes(concat_axis=False)([node,ei2])
-    #     gather_empty_concat = GatherNodes(concat_axis=True)([node, ei2])
+    def test_pooling_LSTM(self):
+        n = tf.ragged.constant(self.n1, ragged_rank=1, inner_shape=(1,))
+        edi = tf.ragged.constant(self.ei1, ragged_rank=1, inner_shape=(2,))
+        ed = tf.ragged.constant(self.e1, ragged_rank=1, inner_shape=(1,))
+
+        ns = GatherNodes()([n, edi])
+        messages = LazyConcatenate(axis=-1)([ed, ns])
+        out = PoolingLocalEdgesLSTM(units=3)([n, messages, edi])
+        print(out[0].shape)
+        self.assertTrue(np.all(np.array(out[0].shape) == np.array([8,3])))
 
 
 if __name__ == '__main__':
-    unittest.main()
+    unittest.main()
+
+
```

### Comparing `kgcnn-2.2.4/test/test_geom.py` & `kgcnn-3.0.0/test/test_layers_geom.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,67 +1,66 @@
 import unittest
 import numpy as np
 import os
 from .utils import ASSETS_PATH
 import tensorflow as tf
-from kgcnn.graph.adj import get_angle_indices
+from kgcnn.graph.methods import get_angle_indices
 from kgcnn.layers.geom import NodeDistanceEuclidean, EdgeAngle, NodePosition
-from kgcnn.layers.conv.dimenet_conv import SphericalBasisLayer
+from kgcnn.literature.DimeNetPP._dimenet_conv import SphericalBasisLayer
 from kgcnn.layers.geom import BesselBasisLayer
 from kgcnn.layers.modules import LazySubtract
 
 
 class TestSphericalBasisLayer(unittest.TestCase):
 
     def test_result_original(self):
-
         ei = np.array([[0, 1], [0, 2], [0, 3], [0, 4], [1, 0], [1, 2], [1, 3], [1, 4], [2, 0], [2, 1], [2, 3], [2, 4],
-                               [3, 0], [3, 1], [3, 2], [3, 4], [4, 0], [4, 1], [4, 2], [4, 3]])
+                       [3, 0], [3, 1], [3, 2], [3, 4], [4, 0], [4, 1], [4, 2], [4, 3]])
         ei1 = np.array([[0, 1], [0, 2], [0, 3], [0, 4], [0, 5], [0, 6], [0, 7],
                         [0, 8], [0, 9], [0, 10], [1, 0], [1, 2], [1, 3], [1, 4], [1, 5],
                         [1, 6], [1, 7], [1, 8], [1, 9], [1, 10], [2, 0], [2, 1], [2, 3],
                         [2, 4], [2, 5], [2, 6], [2, 7], [2, 8], [2, 9], [2, 10], [3, 0],
                         [3, 1], [3, 2], [3, 4], [3, 5], [3, 6], [3, 7], [3, 8], [3, 9],
                         [3, 10], [4, 0], [4, 1], [4, 2], [4, 3], [4, 5], [4, 6], [4, 7], [4, 8],
                         [4, 9], [4, 10], [5, 0], [5, 1], [5, 2], [5, 3], [5, 4], [5, 6], [5, 7],
                         [5, 8], [5, 10], [6, 0], [6, 1], [6, 2], [6, 3], [6, 4], [6, 5], [6, 7],
                         [6, 8], [6, 9], [6, 10], [7, 0], [7, 1], [7, 2], [7, 3], [7, 4], [7, 5],
                         [7, 6], [7, 8], [7, 9], [7, 10], [8, 0], [8, 1], [8, 2], [8, 3], [8, 4],
                         [8, 5], [8, 6], [8, 7], [8, 9], [8, 10], [9, 0], [9, 1], [9, 2],
                         [9, 3], [9, 4], [9, 6], [9, 7], [9, 8], [9, 10], [10, 0], [10, 1], [10, 2],
                         [10, 3], [10, 4], [10, 5], [10, 6], [10, 7], [10, 8], [10, 9]])
-        x1 = np.array([[-0.03113825,  1.54081582,  0.03192126],
-               [ 0.01215347,  0.01092235, -0.01603259],
-               [ 0.72169129, -0.52583353, -1.2623057 ],
-               [ 0.97955987,  1.96459116,  0.03098367],
-               [-0.55840223,  1.94831192, -0.83816075],
-               [-0.54252252,  1.90153531,  0.93005671],
-               [ 0.51522791, -0.36840234,  0.88231134],
-               [-1.01070641, -0.38456999,  0.02051783],
-               [ 1.7585121 , -0.17376585, -1.30871516],
-               [ 0.74087192, -1.62024959, -1.27516511],
-               [ 0.22023351, -0.19051179, -2.1772902 ]])
-        x = np.array([[-1.26981359e-02,  1.08580416e+00,  8.00099580e-03],
-               [ 2.15041600e-03, -6.03131760e-03,  1.97612040e-03],
-               [ 1.01173084e+00,  1.46375116e+00,  2.76574800e-04],
-               [-5.40815069e-01,  1.44752661e+00, -8.76643715e-01],
-               [-5.23813634e-01,  1.43793264e+00,  9.06397294e-01]])
+        x1 = np.array([[-0.03113825, 1.54081582, 0.03192126],
+                       [0.01215347, 0.01092235, -0.01603259],
+                       [0.72169129, -0.52583353, -1.2623057],
+                       [0.97955987, 1.96459116, 0.03098367],
+                       [-0.55840223, 1.94831192, -0.83816075],
+                       [-0.54252252, 1.90153531, 0.93005671],
+                       [0.51522791, -0.36840234, 0.88231134],
+                       [-1.01070641, -0.38456999, 0.02051783],
+                       [1.7585121, -0.17376585, -1.30871516],
+                       [0.74087192, -1.62024959, -1.27516511],
+                       [0.22023351, -0.19051179, -2.1772902]])
+        x = np.array([[-1.26981359e-02, 1.08580416e+00, 8.00099580e-03],
+                      [2.15041600e-03, -6.03131760e-03, 1.97612040e-03],
+                      [1.01173084e+00, 1.46375116e+00, 2.76574800e-04],
+                      [-5.40815069e-01, 1.44752661e+00, -8.76643715e-01],
+                      [-5.23813634e-01, 1.43793264e+00, 9.06397294e-01]])
 
         ei, _, a = get_angle_indices(ei)
         ei1, _, a1 = get_angle_indices(ei1)
 
-        rag_x = tf.RaggedTensor.from_row_lengths(np.concatenate([x,x1]), np.array([len(x),len(x1)]))
-        rag_ei = tf.RaggedTensor.from_row_lengths(np.concatenate([ei,ei1]), np.array([len(ei),len(ei1)]))
-        rag_a = tf.RaggedTensor.from_row_lengths(np.concatenate([a,a1]), np.array([len(a),len(a1)]))
+        rag_x = tf.RaggedTensor.from_row_lengths(np.concatenate([x, x1]), np.array([len(x), len(x1)]))
+        rag_ei = tf.RaggedTensor.from_row_lengths(np.concatenate([ei, ei1]), np.array([len(ei), len(ei1)]))
+        rag_a = tf.RaggedTensor.from_row_lengths(np.concatenate([a, a1]), np.array([len(a), len(a1)]))
 
         a, b = NodePosition()([rag_x, rag_ei])
         dist = NodeDistanceEuclidean()([a, b])
         vec = LazySubtract()([a, b])
         angs = EdgeAngle()([vec, rag_a])
-        bessel = SphericalBasisLayer(10,10,5.0)([dist, angs, rag_a])
+        bessel = SphericalBasisLayer(10, 10, 5.0)([dist, angs, rag_a])
 
         loaded_reference = np.load(os.path.join(ASSETS_PATH, "bessel_basis_reference.npz"), allow_pickle=True)
         test = np.array(loaded_reference["spherical_basis_0"])
         test1 = np.array(loaded_reference["spherical_basis_1"])
         pred = np.array(bessel[0])
         pred1 = np.array(bessel[1])
 
@@ -75,15 +74,14 @@
         self.assertTrue(np.max(valid) < 0.05)
         self.assertTrue(np.max(valid1) < 0.05)
 
 
 class TestBesselBasisLayer(unittest.TestCase):
 
     def test_result_original(self):
-
         ei = np.array([[0, 1], [0, 2], [0, 3], [0, 4], [1, 0], [1, 2], [1, 3], [1, 4], [2, 0], [2, 1], [2, 3], [2, 4],
                        [3, 0], [3, 1], [3, 2], [3, 4], [4, 0], [4, 1], [4, 2], [4, 3]])
         ei1 = np.array([[0, 1], [0, 2], [0, 3], [0, 4], [0, 5], [0, 6], [0, 7],
                         [0, 8], [0, 9], [0, 10], [1, 0], [1, 2], [1, 3], [1, 4], [1, 5],
                         [1, 6], [1, 7], [1, 8], [1, 9], [1, 10], [2, 0], [2, 1], [2, 3],
                         [2, 4], [2, 5], [2, 6], [2, 7], [2, 8], [2, 9], [2, 10], [3, 0],
                         [3, 1], [3, 2], [3, 4], [3, 5], [3, 6], [3, 7], [3, 8], [3, 9],
@@ -91,36 +89,36 @@
                         [4, 9], [4, 10], [5, 0], [5, 1], [5, 2], [5, 3], [5, 4], [5, 6], [5, 7],
                         [5, 8], [5, 10], [6, 0], [6, 1], [6, 2], [6, 3], [6, 4], [6, 5], [6, 7],
                         [6, 8], [6, 9], [6, 10], [7, 0], [7, 1], [7, 2], [7, 3], [7, 4], [7, 5],
                         [7, 6], [7, 8], [7, 9], [7, 10], [8, 0], [8, 1], [8, 2], [8, 3], [8, 4],
                         [8, 5], [8, 6], [8, 7], [8, 9], [8, 10], [9, 0], [9, 1], [9, 2],
                         [9, 3], [9, 4], [9, 6], [9, 7], [9, 8], [9, 10], [10, 0], [10, 1], [10, 2],
                         [10, 3], [10, 4], [10, 5], [10, 6], [10, 7], [10, 8], [10, 9]])
-        x1 = np.array([[-0.03113825,  1.54081582,  0.03192126],
-               [ 0.01215347,  0.01092235, -0.01603259],
-               [ 0.72169129, -0.52583353, -1.2623057 ],
-               [ 0.97955987,  1.96459116,  0.03098367],
-               [-0.55840223,  1.94831192, -0.83816075],
-               [-0.54252252,  1.90153531,  0.93005671],
-               [ 0.51522791, -0.36840234,  0.88231134],
-               [-1.01070641, -0.38456999,  0.02051783],
-               [ 1.7585121 , -0.17376585, -1.30871516],
-               [ 0.74087192, -1.62024959, -1.27516511],
-               [ 0.22023351, -0.19051179, -2.1772902 ]])
-        x= np.array([[-1.26981359e-02,  1.08580416e+00,  8.00099580e-03],
-               [ 2.15041600e-03, -6.03131760e-03,  1.97612040e-03],
-               [ 1.01173084e+00,  1.46375116e+00,  2.76574800e-04],
-               [-5.40815069e-01,  1.44752661e+00, -8.76643715e-01],
-               [-5.23813634e-01,  1.43793264e+00,  9.06397294e-01]])
+        x1 = np.array([[-0.03113825, 1.54081582, 0.03192126],
+                       [0.01215347, 0.01092235, -0.01603259],
+                       [0.72169129, -0.52583353, -1.2623057],
+                       [0.97955987, 1.96459116, 0.03098367],
+                       [-0.55840223, 1.94831192, -0.83816075],
+                       [-0.54252252, 1.90153531, 0.93005671],
+                       [0.51522791, -0.36840234, 0.88231134],
+                       [-1.01070641, -0.38456999, 0.02051783],
+                       [1.7585121, -0.17376585, -1.30871516],
+                       [0.74087192, -1.62024959, -1.27516511],
+                       [0.22023351, -0.19051179, -2.1772902]])
+        x = np.array([[-1.26981359e-02, 1.08580416e+00, 8.00099580e-03],
+                      [2.15041600e-03, -6.03131760e-03, 1.97612040e-03],
+                      [1.01173084e+00, 1.46375116e+00, 2.76574800e-04],
+                      [-5.40815069e-01, 1.44752661e+00, -8.76643715e-01],
+                      [-5.23813634e-01, 1.43793264e+00, 9.06397294e-01]])
 
-        rag_x = tf.RaggedTensor.from_row_lengths(np.concatenate([x,x1]), np.array([len(x),len(x1)]))
-        rag_ei = tf.RaggedTensor.from_row_lengths(np.concatenate([ei,ei1]), np.array([len(ei),len(ei1)]))
+        rag_x = tf.RaggedTensor.from_row_lengths(np.concatenate([x, x1]), np.array([len(x), len(x1)]))
+        rag_ei = tf.RaggedTensor.from_row_lengths(np.concatenate([ei, ei1]), np.array([len(ei), len(ei1)]))
         a, b = NodePosition()([rag_x, rag_ei])
         dist = NodeDistanceEuclidean()([a, b])
-        bessel = BesselBasisLayer(10,5.0)(dist)
+        bessel = BesselBasisLayer(10, 5.0)(dist)
 
         loaded_reference = np.load(os.path.join(ASSETS_PATH, "bessel_basis_reference.npz"), allow_pickle=True)
         test0 = np.array(loaded_reference["bessel_basis_0"])
         test1 = np.array(loaded_reference["bessel_basis_1"])
 
         # print(np.max(np.abs(test0 - bessel[0])))
         # print(np.max(np.abs(test1 - bessel[1])))
```

### Comparing `kgcnn-2.2.4/test/test_graph_base.py` & `kgcnn-3.0.0/test/test_graph_base.py`

 * *Files identical despite different names*

### Comparing `kgcnn-2.2.4/test/test_hdnnp.py` & `kgcnn-3.0.0/kgcnn/literature/HDNNP4th/_test_hdnnp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import unittest
 import tensorflow as tf
-from kgcnn.layers.conv.acsf_conv import ACSFG2, ACSFG4
+from kgcnn.literature.HDNNP2nd._acsf_conv import ACSFG2, ACSFG4
 from kgcnn.graph.adj import get_angle_indices
 import numpy as np
 
 
 class ACSFTest(unittest.TestCase):
     positions = [
         [
```

### Comparing `kgcnn-2.2.4/test/test_literature_gnnexplain.py` & `kgcnn-3.0.0/kgcnn/literature/GNNExplain/_test_literature_gnnexplain.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import unittest
 
 import tensorflow as tf
 
-from kgcnn.xai.testing import MockContext
+from ._xai._testing import MockContext
 from kgcnn.literature.GNNExplain import GnnExplainer
 
 
 class TestGnnExplainer(unittest.TestCase):
 
     def test_basically_works(self):
         num_targets = 1
```

### Comparing `kgcnn-2.2.4/test/test_literature_megan.py` & `kgcnn-3.0.0/kgcnn/literature/MEGAN/_test_literature_megan.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,18 @@
 import tensorflow as tf
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 
 from kgcnn.literature.MEGAN import MEGAN
 from kgcnn.literature.MEGAN import shifted_sigmoid
 
-from .utils import ASSETS_PATH
+try:
+    from .utils import ASSETS_PATH
+except:
+    ASSETS_PATH = ""
 
 ks = tf.keras
 # mpl.use('TkAgg')
 mpl.use('Agg')
 
 
 class TestMegan(unittest.TestCase):
```

### Comparing `kgcnn-2.2.4/test/test_range_periodic.py` & `kgcnn-3.0.0/test/test_range_periodic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import unittest
 import numpy as np
 
-from kgcnn.graph.geom import range_neighbour_lattice
+from kgcnn.graph.methods import range_neighbour_lattice
 # from kgcnn.data.datasets.MatProjectEFormDataset import MatProjectEFormDataset
 
 
 class TestRangePeriodic(unittest.TestCase):
     # Handmade test case.
     artificial_lattice = np.array([[1.0, 0.0, 0.0], [1.0, 1.0, 0.0], [0.0, 0.0, 1.0]])
     artificial_atoms = np.array([[0.1, 0.0, 0.0], [0.5, 0.5, 0.5]])
```

### Comparing `kgcnn-2.2.4/test/test_topk.py` & `kgcnn-3.0.0/kgcnn/literature/Unet/_test_topk.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import unittest
 
 import numpy as np
 import tensorflow as tf
 
-from kgcnn.layers.pool.topk import PoolingTopK, UnPoolingTopK
+from kgcnn.literature.Unet._topk import PoolingTopK, UnPoolingTopK
 
 
 class TestTopKLayerRagged(unittest.TestCase):
     n1 = [[[1.0], [6.0], [1.0], [6.0], [1.0], [1.0], [6.0], [6.0]],
           [[6.0], [1.0], [1.0], [1.0], [7.0], [1.0], [6.0], [8.0], [6.0], [1.0], [6.0], [7.0], [1.0], [1.0], [1.0]]]
     ei1 = [[[0, 1], [1, 0], [1, 6], [2, 3], [3, 2], [3, 5], [3, 7], [4, 7], [5, 3], [6, 1], [6, 7], [7, 3], [7, 4],
             [7, 6]],
@@ -21,20 +21,19 @@
            [0.35355339059327373], [0.35355339059327373], [0.25], [0.3162277660168379], [0.25], [0.25],
            [0.35355339059327373], [0.35355339059327373], [0.25], [0.35355339059327373], [0.25], [0.35355339059327373],
            [0.3162277660168379], [0.22360679774997896], [0.3162277660168379], [0.3162277660168379],
            [0.35355339059327373], [0.25], [0.22360679774997896], [0.3162277660168379], [0.3162277660168379],
            [0.35355339059327373]]]
 
     def test_pool_multiple_times(self):
-
         node = tf.ragged.constant(self.n1, ragged_rank=1, inner_shape=(1,))
-        edgeind = tf.ragged.constant(self.ei1, ragged_rank=1, inner_shape=(2,),dtype=tf.int64)
+        edgeind = tf.ragged.constant(self.ei1, ragged_rank=1, inner_shape=(2,), dtype=tf.int64)
         edgefeat = tf.ragged.constant(self.e1, ragged_rank=1, inner_shape=(1,))
 
-        out1, map1 = PoolingTopK(k=0.3, kernel_initializer="ones", ragged_validate=True)([node, edgefeat,edgeind])
+        out1, map1 = PoolingTopK(k=0.3, kernel_initializer="ones", ragged_validate=True)([node, edgefeat, edgeind])
         out2, map2 = PoolingTopK(k=0.3, kernel_initializer="ones", ragged_validate=True)(out1)
         out3, map3 = PoolingTopK(k=0.3, kernel_initializer="ones", ragged_validate=True)(out2)
         out4, map4 = PoolingTopK(k=0.3, kernel_initializer="ones", ragged_validate=True)(out3)
         out5, map5 = PoolingTopK(k=0.3, kernel_initializer="ones", ragged_validate=True)(out4)
         out6, map6 = PoolingTopK(k=0.3, kernel_initializer="ones", ragged_validate=True)(out5)
         out7, map7 = PoolingTopK(k=0.3, kernel_initializer="ones", ragged_validate=True)(out6)
         out8, map8 = PoolingTopK(k=0.3, kernel_initializer="ones", ragged_validate=True)(out7)
@@ -50,18 +49,20 @@
         uout3 = UnPoolingTopK(ragged_validate=True)(out3 + map4 + uout4)
         uout2 = UnPoolingTopK(ragged_validate=True)(out2 + map3 + uout3)
         uout1 = UnPoolingTopK(ragged_validate=True)(out1 + map2 + uout2)
         uout = UnPoolingTopK(ragged_validate=True)([node, edgefeat, edgeind] + map1 + uout1)
 
         # Expected output
         unpool_nodes = [[[0.], [0.], [0.], [0.], [0.], [0.], [0.], [5.8759007]],
-                        [[0.], [0.], [0.], [0.], [0.], [0.], [0.], [7.9783587], [0.], [0.], [0.], [0.], [0.], [0.], [0.]]]
+                        [[0.], [0.], [0.], [0.], [0.], [0.], [0.], [7.9783587], [0.], [0.], [0.], [0.], [0.], [0.],
+                         [0.]]]
 
         print(uout)
         # Check unpooled
-        self.assertTrue(np.sum(np.abs(uout[0][0].numpy()-np.array(unpool_nodes[0]))) < 1e-5 and np.sum(np.abs(uout[0][1].numpy()-np.array(unpool_nodes[1]))) < 1e-5)
+        self.assertTrue(np.sum(np.abs(uout[0][0].numpy() - np.array(unpool_nodes[0]))) < 1e-5 and np.sum(
+            np.abs(uout[0][1].numpy() - np.array(unpool_nodes[1]))) < 1e-5)
         self.assertTrue(np.all(uout[2][1].numpy() == np.array(self.ei1[1])))
         # print(out1[0])
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kgcnn-2.2.4/test/test_xai_base.py` & `kgcnn-3.0.0/kgcnn/literature/GNNExplain/_test_xai_base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import unittest
 
 import numpy as np
 import tensorflow as tf
 import tensorflow.keras as ks
 
-from kgcnn.xai.testing import MockContext
-from kgcnn.xai.base import MockImportanceExplanationMethod
+from ._xai._testing import MockContext
+from ._xai._base import MockImportanceExplanationMethod
 
 
 # == UNIT TESTS ==
 
 class TestMockImportanceExplanationMethod(unittest.TestCase):
 
     @classmethod
```

### Comparing `kgcnn-2.2.4/test/test_xai_testing.py` & `kgcnn-3.0.0/kgcnn/literature/GNNExplain/_test_xai_testing.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import unittest
 
 import numpy as np
 import tensorflow as tf
 import tensorflow.keras as ks
 
-from kgcnn.xai.testing import MockContext
+from ._xai._testing import MockContext
 
 
 class TestMockContext(unittest.TestCase):
 
     def test_basically_works(self):
         num_elements = 10
         num_targets = 2
```

### Comparing `kgcnn-2.2.4/test/test_xai_utils.py` & `kgcnn-3.0.0/kgcnn/literature/GNNExplain/_test_xai_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import unittest
 
 import numpy as np
 
-from kgcnn.xai.utils import flatten_importances_list
+from ._xai._utils import flatten_importances_list
 
 
 class TestFunctions(unittest.TestCase):
 
     def test_flatten_importances_list_basically_works(self):
         importances_list = [
             np.array([
```

