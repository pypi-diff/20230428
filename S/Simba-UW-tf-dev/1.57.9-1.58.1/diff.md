# Comparing `tmp/Simba-UW-tf-dev-1.57.9.tar.gz` & `tmp/Simba-UW-tf-dev-1.58.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Simba-UW-tf-dev-1.57.9.tar", last modified: Fri Apr 28 00:34:08 2023, max compression
+gzip compressed data, was "dist/Simba-UW-tf-dev-1.58.1.tar", last modified: Fri Apr 28 15:16:29 2023, max compression
```

## Comparing `Simba-UW-tf-dev-1.57.9.tar` & `Simba-UW-tf-dev-1.58.1.tar`

### file list

```diff
@@ -1,398 +1,400 @@
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/
--rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/PKG-INFO
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/simba/
--rw-r--r--   0 simon      (501) staff       (20)    41423 2023-04-27 12:44:27.000000 Simba-UW-tf-dev-1.57.9/simba/video_processing.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/simba/blob_storage/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-21 20:39:46.000000 Simba-UW-tf-dev-1.57.9/simba/blob_storage/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    11569 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/interpolate_smooth.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/simba/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)    11932 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/unsupervised/dbcv_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     3385 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/unsupervised/enums.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-23 19:55:32.000000 Simba-UW-tf-dev-1.57.9/simba/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7442 2023-04-28 00:11:10.000000 Simba-UW-tf-dev-1.57.9/simba/unsupervised/dataset_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     4805 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/unsupervised/grid_search_visualizers.py
--rw-r--r--   0 simon      (501) staff       (20)     6679 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/unsupervised/data_extractor.py
--rw-r--r--   0 simon      (501) staff       (20)     9937 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/unsupervised/ui.py
--rw-r--r--   0 simon      (501) staff       (20)     8367 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/unsupervised/umap_embedder.py
--rw-r--r--   0 simon      (501) staff       (20)    41506 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/unsupervised/pop_up_classes.py
--rw-r--r--   0 simon      (501) staff       (20)     2348 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/unsupervised/bout_aggregator.py
--rw-r--r--   0 simon      (501) staff       (20)    18474 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/unsupervised/cluster_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     2188 2023-04-18 23:25:29.000000 Simba-UW-tf-dev-1.57.9/simba/unsupervised/data_map.yaml
--rw-r--r--   0 simon      (501) staff       (20)     8331 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/unsupervised/hdbscan_clusterer.py
--rw-r--r--   0 simon      (501) staff       (20)     3931 2023-04-19 18:21:47.000000 Simba-UW-tf-dev-1.57.9/simba/unsupervised/tsne.py
--rw-r--r--   0 simon      (501) staff       (20)     5901 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/unsupervised/cluster_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    19750 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/enums.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/simba/bounding_box_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/bounding_box_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     6790 2023-04-28 00:15:19.000000 Simba-UW-tf-dev-1.57.9/simba/bounding_box_tools/agg_boundary_stats.py
--rw-r--r--   0 simon      (501) staff       (20)    23569 2023-04-28 00:19:41.000000 Simba-UW-tf-dev-1.57.9/simba/bounding_box_tools/boundary_menus.py
--rw-r--r--   0 simon      (501) staff       (20)     8515 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/bounding_box_tools/boundary_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     6067 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/bounding_box_tools/find_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    11228 2023-04-28 00:28:29.000000 Simba-UW-tf-dev-1.57.9/simba/bounding_box_tools/visualize_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    32772 2023-04-26 18:25:34.000000 Simba-UW-tf-dev-1.57.9/simba/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/
--rw-r--r--   0 simon      (501) staff       (20)    42279 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/feature_extractor_14bp.py
--rw-r--r--   0 simon      (501) staff       (20)    21408 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/feature_extractor_7bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/
--rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/doctests.py
--rw-r--r--   0 simon      (501) staff       (20)    23850 2023-04-17 18:48:40.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
--rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/read_in_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     2460 2023-04-22 18:02:29.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/peaks.py
--rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/fish_feature_extractor_2022.py
--rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
--rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/convex_hull_scratch_1.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    21398 2023-04-16 17:03:37.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
--rw-r--r--   0 simon      (501) staff       (20)     7127 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/egocentrical_aligner.py
--rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/count_values_in_range.py
--rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/graph_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/termite_rois.csv
--rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/mutual_exclusive.py
--rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/video_color.py
--rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/graph_3d_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/video_rotator.py
--rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/add_probability_cnt_features.py
--rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/make_splash.py
--rw-r--r--   0 simon      (501) staff       (20)     1658 2023-04-22 19:16:28.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/time_stamp_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-15 19:24:18.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/video_rotator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    30677 2023-04-27 01:57:28.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
--rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/convex_hull_scratch_2.py
--rw-r--r--   0 simon      (501) staff       (20)    27739 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/feature_extractor_8bps_2_animals.py
--rw-r--r--   0 simon      (501) staff       (20)    10244 2023-04-25 21:03:39.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     2338 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/perimeter_jit.py
--rw-r--r--   0 simon      (501) staff       (20)    10793 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/feature_subsets.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/__pycache__/
--rw-r--r--   0 simon      (501) staff       (20)      905 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)   238196 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    69038 2023-04-04 11:32:25.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)   238298 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    69338 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc
--rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     2179 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     8282 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/feature_extractor_user_defined.py
--rw-r--r--   0 simon      (501) staff       (20)    46225 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/feature_extractor_16bp.py
--rw-r--r--   0 simon      (501) staff       (20)    27389 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/feature_extractor_9bp.py
--rw-r--r--   0 simon      (501) staff       (20)    23905 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/feature_extractor_8bp.py
--rw-r--r--   0 simon      (501) staff       (20)    16825 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/feature_extractor_4bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/.idea/features_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/.idea/.gitignore
--rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/.idea/.name
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)    15351 2023-04-06 14:48:36.000000 Simba-UW-tf-dev-1.57.9/simba/requirements.txt
--rw-r--r--   0 simon      (501) staff       (20)     4814 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.57.9/simba/severity_processor.py
--rw-r--r--   0 simon      (501) staff       (20)     5942 2023-04-25 15:16:24.000000 Simba-UW-tf-dev-1.57.9/simba/user_pose_config_creator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/simba/mixins/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:26:03.000000 Simba-UW-tf-dev-1.57.9/simba/mixins/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    40274 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/mixins/pop_up_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    28905 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/mixins/config_reader.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/simba/mixins/__pycache__/
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-25 20:46:51.000000 Simba-UW-tf-dev-1.57.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-24 19:51:34.000000 Simba-UW-tf-dev-1.57.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-24 19:51:34.000000 Simba-UW-tf-dev-1.57.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-25 20:46:51.000000 Simba-UW-tf-dev-1.57.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-24 19:06:57.000000 Simba-UW-tf-dev-1.57.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-24 19:06:57.000000 Simba-UW-tf-dev-1.57.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    22108 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/mixins/feature_extraction_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    54715 2023-04-28 00:26:29.000000 Simba-UW-tf-dev-1.57.9/simba/mixins/plotting_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     6093 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/mixins/unsupervised_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    55244 2023-04-27 01:40:24.000000 Simba-UW-tf-dev-1.57.9/simba/mixins/train_model_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    33917 2023-04-27 16:59:00.000000 Simba-UW-tf-dev-1.57.9/simba/machine_model_settings_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5223 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/remove_keypoints_in_pose.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/simba/third_party_label_appenders/
--rw-r--r--   0 simon      (501) staff       (20)     6228 2023-04-26 18:27:58.000000 Simba-UW-tf-dev-1.57.9/simba/third_party_label_appenders/deepethogram_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     9945 2023-04-25 01:50:43.000000 Simba-UW-tf-dev-1.57.9/simba/third_party_label_appenders/BORIS_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     9063 2023-04-25 01:50:43.000000 Simba-UW-tf-dev-1.57.9/simba/third_party_label_appenders/observer_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    16888 2023-04-25 14:58:07.000000 Simba-UW-tf-dev-1.57.9/simba/third_party_label_appenders/tools.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.57.9/simba/third_party_label_appenders/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18242 2023-04-25 01:50:43.000000 Simba-UW-tf-dev-1.57.9/simba/third_party_label_appenders/third_party_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     8173 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.57.9/simba/third_party_label_appenders/ethovision_import.py
--rw-r--r--   0 simon      (501) staff       (20)     6859 2023-04-25 01:50:43.000000 Simba-UW-tf-dev-1.57.9/simba/third_party_label_appenders/BENTO_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     5331 2023-04-25 01:50:43.000000 Simba-UW-tf-dev-1.57.9/simba/third_party_label_appenders/solomon_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     7168 2023-04-25 11:55:36.000000 Simba-UW-tf-dev-1.57.9/simba/multi_cropper.py
--rw-r--r--   0 simon      (501) staff       (20)    12659 2023-04-28 00:12:04.000000 Simba-UW-tf-dev-1.57.9/simba/FSTTC_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    12570 2023-04-25 15:08:48.000000 Simba-UW-tf-dev-1.57.9/simba/create_project_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    13056 2023-04-26 18:37:46.000000 Simba-UW-tf-dev-1.57.9/simba/video_info_table.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/simba/cue_light_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:25:58.000000 Simba-UW-tf-dev-1.57.9/simba/cue_light_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7588 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/cue_light_tools/cue_light_clf_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)    12048 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/cue_light_tools/cue_light_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    17725 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/cue_light_tools/cue_light_menues.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/cue_light_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     1690 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/cue_light_tools/cue_light_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    15283 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/cue_light_tools/cue_light_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    11952 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/cue_light_tools/cue_light_movement_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     2833 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/extract_frames_fast.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/simba/utils/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 20:15:03.000000 Simba-UW-tf-dev-1.57.9/simba/utils/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7365 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/utils/warnings.py
--rw-r--r--   0 simon      (501) staff       (20)     5592 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/utils/checks.py
--rw-r--r--   0 simon      (501) staff       (20)    33757 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/utils/read_write.py
--rw-r--r--   0 simon      (501) staff       (20)     7028 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/utils/lookups.py
--rw-r--r--   0 simon      (501) staff       (20)    14660 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/utils/errors.py
--rw-r--r--   0 simon      (501) staff       (20)    14092 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/utils/data.py
--rw-r--r--   0 simon      (501) staff       (20)     1567 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/utils/printing.py
--rw-r--r--   0 simon      (501) staff       (20)    20580 2023-04-25 15:08:48.000000 Simba-UW-tf-dev-1.57.9/simba/labelling_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     9371 2023-04-26 20:31:09.000000 Simba-UW-tf-dev-1.57.9/simba/timebins_movement_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/SimBA_dash_app.py
--rw-r--r--   0 simon      (501) staff       (20)     7421 2023-04-27 02:02:22.000000 Simba-UW-tf-dev-1.57.9/simba/timebins_clf_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     8215 2023-04-25 11:06:37.000000 Simba-UW-tf-dev-1.57.9/simba/calculate_px_dist.py
--rw-r--r--   0 simon      (501) staff       (20)     6411 2023-04-25 18:52:57.000000 Simba-UW-tf-dev-1.57.9/simba/movement_processor.py
--rw-r--r--   0 simon      (501) staff       (20)     2904 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/pybursts.py
--rw-r--r--   0 simon      (501) staff       (20)     5617 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.57.9/simba/reverse_2_animal_tracking.py
--rw-r--r--   0 simon      (501) staff       (20)     9654 2023-04-25 11:22:07.000000 Simba-UW-tf-dev-1.57.9/simba/Directing_animals_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     3170 2023-04-25 13:13:10.000000 Simba-UW-tf-dev-1.57.9/simba/Validate_model_one_video_run_clf.py
--rw-r--r--   0 simon      (501) staff       (20)    10861 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.57.9/simba/tkinter_functions.py
--rw-r--r--   0 simon      (501) staff       (20)    13112 2023-04-26 21:09:13.000000 Simba-UW-tf-dev-1.57.9/simba/setting_menu.py
--rw-r--r--   0 simon      (501) staff       (20)     6317 2023-04-25 18:03:32.000000 Simba-UW-tf-dev-1.57.9/simba/interpolate_pose.py
--rw-r--r--   0 simon      (501) staff       (20)     3530 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.57.9/simba/run_inference.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/simba/plotting/
--rw-r--r--   0 simon      (501) staff       (20)     9137 2023-04-26 02:10:59.000000 Simba-UW-tf-dev-1.57.9/simba/plotting/gantt_creator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/simba/plotting/tools/
--rw-r--r--   0 simon      (501) staff       (20)     5388 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/plotting/tools/tkinter_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    13231 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.57.9/simba/plotting/ROI_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-25 23:35:57.000000 Simba-UW-tf-dev-1.57.9/simba/plotting/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    14630 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/plotting/shap_agg_stats_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    10167 2023-04-26 15:08:19.000000 Simba-UW-tf-dev-1.57.9/simba/plotting/gantt_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15975 2023-04-26 13:44:02.000000 Simba-UW-tf-dev-1.57.9/simba/plotting/heat_mapper_clf_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     8557 2023-04-26 12:36:28.000000 Simba-UW-tf-dev-1.57.9/simba/plotting/probability_plot_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    12301 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/plotting/plot_clf_results.py
--rw-r--r--   0 simon      (501) staff       (20)    16586 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/plotting/plot_clf_results_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15885 2023-04-26 12:47:24.000000 Simba-UW-tf-dev-1.57.9/simba/plotting/ROI_feature_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12733 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.57.9/simba/plotting/heat_mapper_location.py
--rw-r--r--   0 simon      (501) staff       (20)    12507 2023-04-26 12:41:15.000000 Simba-UW-tf-dev-1.57.9/simba/plotting/probability_plot_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     5226 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.57.9/simba/plotting/interactive_probability_grapher.py
--rw-r--r--   0 simon      (501) staff       (20)     5748 2023-04-26 11:37:28.000000 Simba-UW-tf-dev-1.57.9/simba/plotting/plot_pose_in_dir.py
--rw-r--r--   0 simon      (501) staff       (20)    12771 2023-04-26 14:16:42.000000 Simba-UW-tf-dev-1.57.9/simba/plotting/single_run_model_validation_video.py
--rw-r--r--   0 simon      (501) staff       (20)    12236 2023-04-27 12:57:18.000000 Simba-UW-tf-dev-1.57.9/simba/plotting/frame_mergerer_ffmpeg.py
--rw-r--r--   0 simon      (501) staff       (20)     7887 2023-04-26 13:22:21.000000 Simba-UW-tf-dev-1.57.9/simba/plotting/Directing_animals_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    11204 2023-04-27 12:38:21.000000 Simba-UW-tf-dev-1.57.9/simba/plotting/clf_validator.py
--rw-r--r--   0 simon      (501) staff       (20)    16708 2023-04-26 15:09:39.000000 Simba-UW-tf-dev-1.57.9/simba/plotting/path_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    11324 2023-04-26 13:09:33.000000 Simba-UW-tf-dev-1.57.9/simba/plotting/ROI_feature_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     9876 2023-04-25 23:33:34.000000 Simba-UW-tf-dev-1.57.9/simba/plotting/data_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    12920 2023-04-26 10:57:46.000000 Simba-UW-tf-dev-1.57.9/simba/plotting/path_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     8493 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.57.9/simba/plotting/ez_lineplot.py
--rw-r--r--   0 simon      (501) staff       (20)    11482 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.57.9/simba/plotting/distance_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15604 2023-04-26 13:46:25.000000 Simba-UW-tf-dev-1.57.9/simba/plotting/ROI_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13127 2023-04-25 13:50:19.000000 Simba-UW-tf-dev-1.57.9/simba/plotting/heat_mapper_clf.py
--rw-r--r--   0 simon      (501) staff       (20)     8973 2023-04-26 00:37:26.000000 Simba-UW-tf-dev-1.57.9/simba/plotting/distance_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13560 2023-04-27 18:03:45.000000 Simba-UW-tf-dev-1.57.9/simba/plotting/single_run_model_validation_video_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     9731 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.57.9/simba/plotting/Directing_animals_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    16315 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.57.9/simba/plotting/heat_mapper_location_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/run_dash_tkinter.py
--rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/dash_app.py
--rw-r--r--   0 simon      (501) staff       (20)     2907 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/extract_annotation_frames.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/simba/roi_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6501 2023-04-25 18:50:18.000000 Simba-UW-tf-dev-1.57.9/simba/roi_tools/ROI_time_bin_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     1753 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.57.9/simba/roi_tools/ROI_movement_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-20 12:47:56.000000 Simba-UW-tf-dev-1.57.9/simba/roi_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    43128 2023-04-26 19:19:44.000000 Simba-UW-tf-dev-1.57.9/simba/roi_tools/ROI_define.py
--rw-r--r--   0 simon      (501) staff       (20)     3402 2023-04-26 19:25:50.000000 Simba-UW-tf-dev-1.57.9/simba/roi_tools/ROI_reset.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/roi_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    19690 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.57.9/simba/roi_tools/ROI_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    11332 2023-04-26 21:13:20.000000 Simba-UW-tf-dev-1.57.9/simba/roi_tools/ROI_feature_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     3651 2023-04-26 19:22:41.000000 Simba-UW-tf-dev-1.57.9/simba/roi_tools/ROI_multiply.py
--rw-r--r--   0 simon      (501) staff       (20)      961 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/roi_tools/ROI_size_calculations.py
--rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/roi_tools/ROI_zoom.py
--rw-r--r--   0 simon      (501) staff       (20)    11384 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.57.9/simba/roi_tools/ROI_directing_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/roi_tools/ROI_move_shape.py
--rw-r--r--   0 simon      (501) staff       (20)     5073 2023-04-25 14:55:41.000000 Simba-UW-tf-dev-1.57.9/simba/roi_tools/ROI_menus.py
--rw-r--r--   0 simon      (501) staff       (20)    13793 2023-04-26 14:59:42.000000 Simba-UW-tf-dev-1.57.9/simba/roi_tools/ROI_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    22685 2023-04-25 14:55:41.000000 Simba-UW-tf-dev-1.57.9/simba/roi_tools/ROI_image.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/simba/pose_importers/
--rw-r--r--   0 simon      (501) staff       (20)     2464 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.57.9/simba/pose_importers/read_DANNCE_mat.py
--rw-r--r--   0 simon      (501) staff       (20)    21991 2023-04-27 15:50:07.000000 Simba-UW-tf-dev-1.57.9/simba/pose_importers/sleap_importer_slp.py
--rw-r--r--   0 simon      (501) staff       (20)    23507 2023-04-27 15:45:27.000000 Simba-UW-tf-dev-1.57.9/simba/pose_importers/sleap_importer_h5.py
--rw-r--r--   0 simon      (501) staff       (20)    23579 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.57.9/simba/pose_importers/dlc_multi_animal_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-25 16:49:14.000000 Simba-UW-tf-dev-1.57.9/simba/pose_importers/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    21003 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/pose_importers/sleap_importer_csv.py
--rw-r--r--   0 simon      (501) staff       (20)     7761 2023-04-25 18:26:26.000000 Simba-UW-tf-dev-1.57.9/simba/pose_importers/import_mars.py
--rw-r--r--   0 simon      (501) staff       (20)     6922 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.57.9/simba/pose_importers/dlc_importer_csv.py
--rw-r--r--   0 simon      (501) staff       (20)     8100 2023-04-27 21:09:15.000000 Simba-UW-tf-dev-1.57.9/simba/pose_importers/trk_importer.py
--rw-r--r--   0 simon      (501) staff       (20)   238321 2023-04-28 00:09:50.000000 Simba-UW-tf-dev-1.57.9/simba/pop_up_classes.py
--rw-r--r--   0 simon      (501) staff       (20)     4695 2023-04-26 18:17:53.000000 Simba-UW-tf-dev-1.57.9/simba/extract_seqframes.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/simba/pose_configurations/
--rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.57.9/simba/pose_configurations/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/simba/pose_configurations/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.57.9/simba/pose_configurations/bp_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-10 12:22:28.000000 Simba-UW-tf-dev-1.57.9/simba/pose_configurations/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/simba/pose_configurations/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       24 2023-03-20 15:55:45.000000 Simba-UW-tf-dev-1.57.9/simba/pose_configurations/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.57.9/simba/pose_configurations/no_animals/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/simba/pose_configurations/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.57.9/simba/pose_configurations/configuration_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)      267 2023-03-20 15:55:45.000000 Simba-UW-tf-dev-1.57.9/simba/pose_configurations/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/simba/pose_configurations/schematics/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.57.9/simba/pose_configurations/schematics/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/pose_configurations/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.57.9/simba/pose_configurations/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/pose_configurations/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.57.9/simba/pose_configurations/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.57.9/simba/pose_configurations/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/pose_configurations/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/pose_configurations/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/pose_configurations/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/pose_configurations/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/pose_configurations/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/pose_configurations/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/pose_configurations/schematics/1.png
--rw-r--r--   0 simon      (501) staff       (20)     7171 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.57.9/simba/get_coordinates_tools_v2.py
--rw-r--r--   0 simon      (501) staff       (20)    15761 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/pup_retrieval_protocol.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/simba/outlier_tools/
--rw-r--r--   0 simon      (501) staff       (20)     7427 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/outlier_tools/outlier_corrector_movement.py
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-15 17:05:05.000000 Simba-UW-tf-dev-1.57.9/simba/outlier_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/outlier_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8191 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/outlier_tools/outlier_corrector_location.py
--rw-r--r--   0 simon      (501) staff       (20)     2706 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/outlier_tools/skip_outlier_correction.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/simba/outlier_tools/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/outlier_tools/.idea/outlier_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/outlier_tools/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/simba/outlier_tools/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/simba/outlier_tools/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/outlier_tools/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/outlier_tools/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/outlier_tools/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/outlier_tools/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)     2613 2023-04-25 15:16:24.000000 Simba-UW-tf-dev-1.57.9/simba/pose_reset.py
--rw-r--r--   0 simon      (501) staff       (20)    18234 2023-04-27 17:03:57.000000 Simba-UW-tf-dev-1.57.9/simba/train_mutiple_models.py
--rw-r--r--   0 simon      (501) staff       (20)    63957 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.57.9/simba/SimBA.py
--rw-r--r--   0 simon      (501) staff       (20)    26559 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.57.9/simba/labelling_advanced_interface.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/simba/assets/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/simba/assets/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/assets/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/assets/unsupervised/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/assets/unsupervised/features.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/simba/assets/shap/
--rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/assets/shap/down_arrow.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/assets/shap/intruder_shape.jpg
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/simba/assets/shap/feature_categories/
--rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
--rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/assets/shap/feature_categories/shap_feature_categories.csv
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-04-10 20:37:13.000000 Simba-UW-tf-dev-1.57.9/simba/assets/shap/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/assets/shap/resident_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/assets/shap/resident_intruder_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/assets/shap/animal_distances.jpg
--rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/assets/shap/baseline_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/assets/shap/ubuntu.regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/assets/shap/side_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/assets/shap/UbuntuMono-Regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/assets/shap/side_scale_5.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/assets/shap/intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/assets/shap/resident_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/assets/shap/color_bar.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/assets/shap/resident_intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)    16388 2023-04-25 19:14:34.000000 Simba-UW-tf-dev-1.57.9/simba/assets/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/simba/assets/lookups/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/assets/lookups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/assets/lookups/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)     2987 2023-04-25 20:39:03.000000 Simba-UW-tf-dev-1.57.9/simba/assets/lookups/feature_extraction_headers.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/assets/lookups/features.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/assets/lookups/unsupervised_example_x.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/simba/assets/stl/
--rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/assets/stl/operant_tray.stl
--rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/assets/stl/operant_lever.stl
--rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/assets/stl/operant_walls.stl
--rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/assets/stl/grid_floor.stl
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/simba/assets/img/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.57.9/simba/assets/img/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/assets/img/about_me.png
--rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.57.9/simba/assets/img/splash.mp4
--rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.57.9/simba/assets/img/bg_2.png
--rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/assets/img/splash.pptx
--rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.57.9/simba/assets/img/bg.png
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/assets/UbuntuMono-Regular.ttf
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/
--rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/factory.png
--rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/cluster.png
--rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/load.png
--rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/gif.png
--rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/pose.png
--rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/features.png
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/.DS_Store
--rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/settings.png
--rw-r--r--   0 simon      (501) staff       (20)     2090 2023-04-22 15:14:17.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/stopwatch.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/link.png
--rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/dash_simba.css
--rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/documentation.png
--rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/fps.png
--rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/dimensionality_reduction.png
--rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/roi.png
--rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/superimpose.png
--rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/label.png
--rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/change.png
--rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/crop.png
--rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/rotate.png
--rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/path.png
--rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/clip.png
--rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/restart.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/calipher.png
--rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/add_on.png
--rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/create.png
--rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/SimBA_logo.ico
--rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/print.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/clf.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/concat_icons/
--rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/concat_icons/mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/concat_icons/vertical.png
--rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/concat_icons/horizontal.png
--rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/concat_icons/mixed_mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/merge.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/clean.png
--rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/clf_2.png
--rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/visualize.png
--rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/concat.png
--rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/boris.png
--rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/frames.png
--rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/video.png
--rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/sample.png
--rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/metrics.png
--rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/grey.png
--rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/exit.png
--rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/outlier.png
--rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/clahe.png
--rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/trash.png
--rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/about.png
--rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/convert.png
--rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/SimBA_logo.icns
--rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/reorganize.png
--rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/browse.png
--rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/SimBA_logo.png
--rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/ethovision.png
--rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/close.png
--rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/assets/dash_simba_base.css
--rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/assets/TheGoldenLab.PNG
--rw-r--r--   0 simon      (501) staff       (20)     9478 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.57.9/simba/read_config_unit_tests.py
--rw-r--r--   0 simon      (501) staff       (20)    11645 2023-04-25 15:16:24.000000 Simba-UW-tf-dev-1.57.9/simba/project_config_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    19000 2023-04-26 18:08:54.000000 Simba-UW-tf-dev-1.57.9/simba/train_single_model.py
--rw-r--r--   0 simon      (501) staff       (20)     6308 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.57.9/simba/create_clf_log.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/simba/batch_process_videos/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-17 14:43:38.000000 Simba-UW-tf-dev-1.57.9/simba/batch_process_videos/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    24639 2023-04-25 13:26:59.000000 Simba-UW-tf-dev-1.57.9/simba/batch_process_videos/batch_process_menus.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/batch_process_videos/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    11106 2023-04-25 13:26:59.000000 Simba-UW-tf-dev-1.57.9/simba/batch_process_videos/batch_process_create_ffmpeg_commands.py
--rw-r--r--   0 simon      (501) staff       (20)     9520 2023-04-25 19:02:08.000000 Simba-UW-tf-dev-1.57.9/simba/Kleinberg_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8341 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/reorganize_keypoint_in_pose.py
--rw-r--r--   0 simon      (501) staff       (20)      165 2023-03-25 11:18:21.000000 Simba-UW-tf-dev-1.57.9/simba/~$features.pptx
--rw-r--r--   0 simon      (501) staff       (20)     6543 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.57.9/simba/play_annotation_video.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/Simba_UW_tf_dev.egg-info/
--rw-rw-r--   0 simon      (501) staff       (20)      579 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/Simba_UW_tf_dev.egg-info/PKG-INFO
--rw-rw-r--   0 simon      (501) staff       (20)    13977 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/Simba_UW_tf_dev.egg-info/SOURCES.txt
--rw-rw-r--   0 simon      (501) staff       (20)       44 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/Simba_UW_tf_dev.egg-info/entry_points.txt
--rw-rw-r--   0 simon      (501) staff       (20)      639 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/Simba_UW_tf_dev.egg-info/requires.txt
--rw-rw-r--   0 simon      (501) staff       (20)        6 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/Simba_UW_tf_dev.egg-info/top_level.txt
--rw-rw-r--   0 simon      (501) staff       (20)        1 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/Simba_UW_tf_dev.egg-info/dependency_links.txt
--rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.57.9/LICENSE.md
--rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.57.9/MANIFEST.in
--rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.57.9/README.md
--rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-04-28 00:33:54.000000 Simba-UW-tf-dev-1.57.9/setup.py
--rw-r--r--   0 simon      (501) staff       (20)       38 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/setup.cfg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 15:16:29.000000 Simba-UW-tf-dev-1.58.1/
+-rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-28 15:16:29.000000 Simba-UW-tf-dev-1.58.1/PKG-INFO
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 15:16:29.000000 Simba-UW-tf-dev-1.58.1/simba/
+-rw-r--r--   0 simon      (501) staff       (20)    41423 2023-04-27 12:44:27.000000 Simba-UW-tf-dev-1.58.1/simba/video_processing.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 15:16:29.000000 Simba-UW-tf-dev-1.58.1/simba/blob_storage/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-21 20:39:46.000000 Simba-UW-tf-dev-1.58.1/simba/blob_storage/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    11569 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.1/simba/interpolate_smooth.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 15:16:29.000000 Simba-UW-tf-dev-1.58.1/simba/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)    11932 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.1/simba/unsupervised/dbcv_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3385 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.1/simba/unsupervised/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-23 19:55:32.000000 Simba-UW-tf-dev-1.58.1/simba/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     8187 2023-04-28 13:09:30.000000 Simba-UW-tf-dev-1.58.1/simba/unsupervised/dataset_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5693 2023-04-28 13:09:30.000000 Simba-UW-tf-dev-1.58.1/simba/unsupervised/grid_search_visualizers.py
+-rw-r--r--   0 simon      (501) staff       (20)     7268 2023-04-28 12:30:12.000000 Simba-UW-tf-dev-1.58.1/simba/unsupervised/data_extractor.py
+-rw-r--r--   0 simon      (501) staff       (20)     9937 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.1/simba/unsupervised/ui.py
+-rw-r--r--   0 simon      (501) staff       (20)     9915 2023-04-28 13:09:30.000000 Simba-UW-tf-dev-1.58.1/simba/unsupervised/umap_embedder.py
+-rw-r--r--   0 simon      (501) staff       (20)    41557 2023-04-28 13:09:30.000000 Simba-UW-tf-dev-1.58.1/simba/unsupervised/pop_up_classes.py
+-rw-r--r--   0 simon      (501) staff       (20)     2347 2023-04-28 12:22:34.000000 Simba-UW-tf-dev-1.58.1/simba/unsupervised/bout_aggregator.py
+-rw-r--r--   0 simon      (501) staff       (20)    20880 2023-04-28 12:22:34.000000 Simba-UW-tf-dev-1.58.1/simba/unsupervised/cluster_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     2188 2023-04-18 23:25:29.000000 Simba-UW-tf-dev-1.58.1/simba/unsupervised/data_map.yaml
+-rw-r--r--   0 simon      (501) staff       (20)    10289 2023-04-28 13:09:30.000000 Simba-UW-tf-dev-1.58.1/simba/unsupervised/hdbscan_clusterer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3931 2023-04-19 18:21:47.000000 Simba-UW-tf-dev-1.58.1/simba/unsupervised/tsne.py
+-rw-r--r--   0 simon      (501) staff       (20)     6692 2023-04-28 12:30:12.000000 Simba-UW-tf-dev-1.58.1/simba/unsupervised/cluster_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    19750 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.1/simba/enums.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 15:16:29.000000 Simba-UW-tf-dev-1.58.1/simba/bounding_box_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/bounding_box_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     6790 2023-04-28 00:15:19.000000 Simba-UW-tf-dev-1.58.1/simba/bounding_box_tools/agg_boundary_stats.py
+-rw-r--r--   0 simon      (501) staff       (20)    23569 2023-04-28 00:19:41.000000 Simba-UW-tf-dev-1.58.1/simba/bounding_box_tools/boundary_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)     8515 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.1/simba/bounding_box_tools/boundary_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     6067 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.1/simba/bounding_box_tools/find_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    11228 2023-04-28 00:28:29.000000 Simba-UW-tf-dev-1.58.1/simba/bounding_box_tools/visualize_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    32772 2023-04-26 18:25:34.000000 Simba-UW-tf-dev-1.58.1/simba/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 15:16:29.000000 Simba-UW-tf-dev-1.58.1/simba/feature_extractors/
+-rw-r--r--   0 simon      (501) staff       (20)    42317 2023-04-28 15:16:26.000000 Simba-UW-tf-dev-1.58.1/simba/feature_extractors/feature_extractor_14bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    21427 2023-04-28 15:16:26.000000 Simba-UW-tf-dev-1.58.1/simba/feature_extractors/feature_extractor_7bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 15:16:29.000000 Simba-UW-tf-dev-1.58.1/simba/feature_extractors/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.58.1/simba/feature_extractors/misc/doctests.py
+-rw-r--r--   0 simon      (501) staff       (20)    23850 2023-04-17 18:48:40.000000 Simba-UW-tf-dev-1.58.1/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.58.1/simba/feature_extractors/misc/read_in_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     2460 2023-04-22 18:02:29.000000 Simba-UW-tf-dev-1.58.1/simba/feature_extractors/misc/peaks.py
+-rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.58.1/simba/feature_extractors/misc/fish_feature_extractor_2022.py
+-rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.58.1/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.58.1/simba/feature_extractors/misc/convex_hull_scratch_1.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.58.1/simba/feature_extractors/misc/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    21398 2023-04-16 17:03:37.000000 Simba-UW-tf-dev-1.58.1/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     7127 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/feature_extractors/misc/egocentrical_aligner.py
+-rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.58.1/simba/feature_extractors/misc/count_values_in_range.py
+-rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/feature_extractors/misc/graph_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/feature_extractors/misc/termite_rois.csv
+-rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.58.1/simba/feature_extractors/misc/mutual_exclusive.py
+-rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.58.1/simba/feature_extractors/misc/video_color.py
+-rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/feature_extractors/misc/graph_3d_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.58.1/simba/feature_extractors/misc/video_rotator.py
+-rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/feature_extractors/misc/add_probability_cnt_features.py
+-rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.58.1/simba/feature_extractors/misc/make_splash.py
+-rw-r--r--   0 simon      (501) staff       (20)     1658 2023-04-22 19:16:28.000000 Simba-UW-tf-dev-1.58.1/simba/feature_extractors/misc/time_stamp_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-15 19:24:18.000000 Simba-UW-tf-dev-1.58.1/simba/feature_extractors/misc/video_rotator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    30677 2023-04-27 01:57:28.000000 Simba-UW-tf-dev-1.58.1/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
+-rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.58.1/simba/feature_extractors/misc/convex_hull_scratch_2.py
+-rw-r--r--   0 simon      (501) staff       (20)    27777 2023-04-28 15:16:26.000000 Simba-UW-tf-dev-1.58.1/simba/feature_extractors/feature_extractor_8bps_2_animals.py
+-rw-r--r--   0 simon      (501) staff       (20)    10244 2023-04-25 21:03:39.000000 Simba-UW-tf-dev-1.58.1/simba/feature_extractors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     2337 2023-04-28 15:11:24.000000 Simba-UW-tf-dev-1.58.1/simba/feature_extractors/perimeter_jit.py
+-rw-r--r--   0 simon      (501) staff       (20)    10869 2023-04-28 15:16:26.000000 Simba-UW-tf-dev-1.58.1/simba/feature_extractors/feature_subsets.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/feature_extractors/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 15:16:29.000000 Simba-UW-tf-dev-1.58.1/simba/feature_extractors/__pycache__/
+-rw-r--r--   0 simon      (501) staff       (20)      905 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.58.1/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)   238196 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.58.1/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    69038 2023-04-04 11:32:25.000000 Simba-UW-tf-dev-1.58.1/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)   238298 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.58.1/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    69338 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.58.1/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc
+-rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.58.1/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     2179 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.58.1/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     8282 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.1/simba/feature_extractors/feature_extractor_user_defined.py
+-rw-r--r--   0 simon      (501) staff       (20)    46263 2023-04-28 15:16:26.000000 Simba-UW-tf-dev-1.58.1/simba/feature_extractors/feature_extractor_16bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    27409 2023-04-28 15:16:26.000000 Simba-UW-tf-dev-1.58.1/simba/feature_extractors/feature_extractor_9bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    23924 2023-04-28 15:16:26.000000 Simba-UW-tf-dev-1.58.1/simba/feature_extractors/feature_extractor_8bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16825 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.1/simba/feature_extractors/feature_extractor_4bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 15:16:29.000000 Simba-UW-tf-dev-1.58.1/simba/feature_extractors/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/feature_extractors/.idea/features_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/feature_extractors/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 15:16:29.000000 Simba-UW-tf-dev-1.58.1/simba/feature_extractors/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 15:16:29.000000 Simba-UW-tf-dev-1.58.1/simba/feature_extractors/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/feature_extractors/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/feature_extractors/.idea/.gitignore
+-rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/feature_extractors/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/feature_extractors/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/feature_extractors/.idea/.name
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/feature_extractors/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)    15351 2023-04-06 14:48:36.000000 Simba-UW-tf-dev-1.58.1/simba/requirements.txt
+-rw-r--r--   0 simon      (501) staff       (20)     4814 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.1/simba/severity_processor.py
+-rw-r--r--   0 simon      (501) staff       (20)     5942 2023-04-25 15:16:24.000000 Simba-UW-tf-dev-1.58.1/simba/user_pose_config_creator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 15:16:29.000000 Simba-UW-tf-dev-1.58.1/simba/mixins/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:26:03.000000 Simba-UW-tf-dev-1.58.1/simba/mixins/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    40530 2023-04-28 01:01:52.000000 Simba-UW-tf-dev-1.58.1/simba/mixins/pop_up_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    29191 2023-04-28 01:01:52.000000 Simba-UW-tf-dev-1.58.1/simba/mixins/config_reader.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 15:16:29.000000 Simba-UW-tf-dev-1.58.1/simba/mixins/__pycache__/
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-25 20:46:51.000000 Simba-UW-tf-dev-1.58.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-24 19:51:34.000000 Simba-UW-tf-dev-1.58.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-28 15:11:42.000000 Simba-UW-tf-dev-1.58.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    49963 2023-04-28 15:11:42.000000 Simba-UW-tf-dev-1.58.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-24 19:51:34.000000 Simba-UW-tf-dev-1.58.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-25 20:46:51.000000 Simba-UW-tf-dev-1.58.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-24 19:06:57.000000 Simba-UW-tf-dev-1.58.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-24 19:06:57.000000 Simba-UW-tf-dev-1.58.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    22274 2023-04-28 01:01:52.000000 Simba-UW-tf-dev-1.58.1/simba/mixins/feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    54770 2023-04-28 01:01:52.000000 Simba-UW-tf-dev-1.58.1/simba/mixins/plotting_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     6155 2023-04-28 01:01:52.000000 Simba-UW-tf-dev-1.58.1/simba/mixins/unsupervised_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    55313 2023-04-28 01:01:52.000000 Simba-UW-tf-dev-1.58.1/simba/mixins/train_model_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    33917 2023-04-27 16:59:00.000000 Simba-UW-tf-dev-1.58.1/simba/machine_model_settings_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5223 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.1/simba/remove_keypoints_in_pose.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 15:16:29.000000 Simba-UW-tf-dev-1.58.1/simba/third_party_label_appenders/
+-rw-r--r--   0 simon      (501) staff       (20)     6228 2023-04-26 18:27:58.000000 Simba-UW-tf-dev-1.58.1/simba/third_party_label_appenders/deepethogram_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     9945 2023-04-25 01:50:43.000000 Simba-UW-tf-dev-1.58.1/simba/third_party_label_appenders/BORIS_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     9063 2023-04-25 01:50:43.000000 Simba-UW-tf-dev-1.58.1/simba/third_party_label_appenders/observer_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16888 2023-04-25 14:58:07.000000 Simba-UW-tf-dev-1.58.1/simba/third_party_label_appenders/tools.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.58.1/simba/third_party_label_appenders/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18242 2023-04-25 01:50:43.000000 Simba-UW-tf-dev-1.58.1/simba/third_party_label_appenders/third_party_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     8173 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.1/simba/third_party_label_appenders/ethovision_import.py
+-rw-r--r--   0 simon      (501) staff       (20)     6859 2023-04-25 01:50:43.000000 Simba-UW-tf-dev-1.58.1/simba/third_party_label_appenders/BENTO_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     5331 2023-04-25 01:50:43.000000 Simba-UW-tf-dev-1.58.1/simba/third_party_label_appenders/solomon_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     7168 2023-04-25 11:55:36.000000 Simba-UW-tf-dev-1.58.1/simba/multi_cropper.py
+-rw-r--r--   0 simon      (501) staff       (20)    12659 2023-04-28 00:12:04.000000 Simba-UW-tf-dev-1.58.1/simba/FSTTC_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12570 2023-04-25 15:08:48.000000 Simba-UW-tf-dev-1.58.1/simba/create_project_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    13056 2023-04-26 18:37:46.000000 Simba-UW-tf-dev-1.58.1/simba/video_info_table.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 15:16:29.000000 Simba-UW-tf-dev-1.58.1/simba/cue_light_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:25:58.000000 Simba-UW-tf-dev-1.58.1/simba/cue_light_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7588 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.1/simba/cue_light_tools/cue_light_clf_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)    12048 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.1/simba/cue_light_tools/cue_light_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    17725 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.1/simba/cue_light_tools/cue_light_menues.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/cue_light_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     1690 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.1/simba/cue_light_tools/cue_light_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    15283 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.1/simba/cue_light_tools/cue_light_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    11952 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.1/simba/cue_light_tools/cue_light_movement_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     2833 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.1/simba/extract_frames_fast.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 15:16:29.000000 Simba-UW-tf-dev-1.58.1/simba/utils/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 20:15:03.000000 Simba-UW-tf-dev-1.58.1/simba/utils/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7365 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.1/simba/utils/warnings.py
+-rw-r--r--   0 simon      (501) staff       (20)     5592 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.1/simba/utils/checks.py
+-rw-r--r--   0 simon      (501) staff       (20)    33757 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.1/simba/utils/read_write.py
+-rw-r--r--   0 simon      (501) staff       (20)     7028 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.1/simba/utils/lookups.py
+-rw-r--r--   0 simon      (501) staff       (20)    14660 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.1/simba/utils/errors.py
+-rw-r--r--   0 simon      (501) staff       (20)    14092 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.1/simba/utils/data.py
+-rw-r--r--   0 simon      (501) staff       (20)     1567 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.1/simba/utils/printing.py
+-rw-r--r--   0 simon      (501) staff       (20)    20580 2023-04-25 15:08:48.000000 Simba-UW-tf-dev-1.58.1/simba/labelling_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     9371 2023-04-26 20:31:09.000000 Simba-UW-tf-dev-1.58.1/simba/timebins_movement_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/SimBA_dash_app.py
+-rw-r--r--   0 simon      (501) staff       (20)     7421 2023-04-27 02:02:22.000000 Simba-UW-tf-dev-1.58.1/simba/timebins_clf_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     8215 2023-04-25 11:06:37.000000 Simba-UW-tf-dev-1.58.1/simba/calculate_px_dist.py
+-rw-r--r--   0 simon      (501) staff       (20)     6411 2023-04-25 18:52:57.000000 Simba-UW-tf-dev-1.58.1/simba/movement_processor.py
+-rw-r--r--   0 simon      (501) staff       (20)     2904 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/pybursts.py
+-rw-r--r--   0 simon      (501) staff       (20)     5617 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.1/simba/reverse_2_animal_tracking.py
+-rw-r--r--   0 simon      (501) staff       (20)     9654 2023-04-25 11:22:07.000000 Simba-UW-tf-dev-1.58.1/simba/Directing_animals_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3170 2023-04-25 13:13:10.000000 Simba-UW-tf-dev-1.58.1/simba/Validate_model_one_video_run_clf.py
+-rw-r--r--   0 simon      (501) staff       (20)    10861 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.1/simba/tkinter_functions.py
+-rw-r--r--   0 simon      (501) staff       (20)    13112 2023-04-26 21:09:13.000000 Simba-UW-tf-dev-1.58.1/simba/setting_menu.py
+-rw-r--r--   0 simon      (501) staff       (20)     6317 2023-04-25 18:03:32.000000 Simba-UW-tf-dev-1.58.1/simba/interpolate_pose.py
+-rw-r--r--   0 simon      (501) staff       (20)     3530 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.1/simba/run_inference.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 15:16:29.000000 Simba-UW-tf-dev-1.58.1/simba/plotting/
+-rw-r--r--   0 simon      (501) staff       (20)     9137 2023-04-26 02:10:59.000000 Simba-UW-tf-dev-1.58.1/simba/plotting/gantt_creator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 15:16:29.000000 Simba-UW-tf-dev-1.58.1/simba/plotting/tools/
+-rw-r--r--   0 simon      (501) staff       (20)     5388 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.1/simba/plotting/tools/tkinter_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    13231 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.1/simba/plotting/ROI_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-25 23:35:57.000000 Simba-UW-tf-dev-1.58.1/simba/plotting/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    14630 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.1/simba/plotting/shap_agg_stats_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10167 2023-04-26 15:08:19.000000 Simba-UW-tf-dev-1.58.1/simba/plotting/gantt_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15975 2023-04-26 13:44:02.000000 Simba-UW-tf-dev-1.58.1/simba/plotting/heat_mapper_clf_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     8557 2023-04-26 12:36:28.000000 Simba-UW-tf-dev-1.58.1/simba/plotting/probability_plot_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12301 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.1/simba/plotting/plot_clf_results.py
+-rw-r--r--   0 simon      (501) staff       (20)    16586 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.1/simba/plotting/plot_clf_results_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15885 2023-04-26 12:47:24.000000 Simba-UW-tf-dev-1.58.1/simba/plotting/ROI_feature_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12733 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.1/simba/plotting/heat_mapper_location.py
+-rw-r--r--   0 simon      (501) staff       (20)    12507 2023-04-26 12:41:15.000000 Simba-UW-tf-dev-1.58.1/simba/plotting/probability_plot_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     5226 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.1/simba/plotting/interactive_probability_grapher.py
+-rw-r--r--   0 simon      (501) staff       (20)     5748 2023-04-26 11:37:28.000000 Simba-UW-tf-dev-1.58.1/simba/plotting/plot_pose_in_dir.py
+-rw-r--r--   0 simon      (501) staff       (20)    12771 2023-04-26 14:16:42.000000 Simba-UW-tf-dev-1.58.1/simba/plotting/single_run_model_validation_video.py
+-rw-r--r--   0 simon      (501) staff       (20)    12236 2023-04-27 12:57:18.000000 Simba-UW-tf-dev-1.58.1/simba/plotting/frame_mergerer_ffmpeg.py
+-rw-r--r--   0 simon      (501) staff       (20)     7887 2023-04-26 13:22:21.000000 Simba-UW-tf-dev-1.58.1/simba/plotting/Directing_animals_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    11204 2023-04-27 12:38:21.000000 Simba-UW-tf-dev-1.58.1/simba/plotting/clf_validator.py
+-rw-r--r--   0 simon      (501) staff       (20)    16708 2023-04-26 15:09:39.000000 Simba-UW-tf-dev-1.58.1/simba/plotting/path_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    11324 2023-04-26 13:09:33.000000 Simba-UW-tf-dev-1.58.1/simba/plotting/ROI_feature_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     9876 2023-04-25 23:33:34.000000 Simba-UW-tf-dev-1.58.1/simba/plotting/data_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    12920 2023-04-26 10:57:46.000000 Simba-UW-tf-dev-1.58.1/simba/plotting/path_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     8493 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.1/simba/plotting/ez_lineplot.py
+-rw-r--r--   0 simon      (501) staff       (20)    11482 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.1/simba/plotting/distance_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15604 2023-04-26 13:46:25.000000 Simba-UW-tf-dev-1.58.1/simba/plotting/ROI_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13127 2023-04-25 13:50:19.000000 Simba-UW-tf-dev-1.58.1/simba/plotting/heat_mapper_clf.py
+-rw-r--r--   0 simon      (501) staff       (20)     8973 2023-04-26 00:37:26.000000 Simba-UW-tf-dev-1.58.1/simba/plotting/distance_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13560 2023-04-27 18:03:45.000000 Simba-UW-tf-dev-1.58.1/simba/plotting/single_run_model_validation_video_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     9731 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.1/simba/plotting/Directing_animals_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16315 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.1/simba/plotting/heat_mapper_location_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/run_dash_tkinter.py
+-rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/dash_app.py
+-rw-r--r--   0 simon      (501) staff       (20)     2907 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.1/simba/extract_annotation_frames.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 15:16:29.000000 Simba-UW-tf-dev-1.58.1/simba/roi_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6501 2023-04-25 18:50:18.000000 Simba-UW-tf-dev-1.58.1/simba/roi_tools/ROI_time_bin_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     1753 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.1/simba/roi_tools/ROI_movement_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-20 12:47:56.000000 Simba-UW-tf-dev-1.58.1/simba/roi_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    43128 2023-04-26 19:19:44.000000 Simba-UW-tf-dev-1.58.1/simba/roi_tools/ROI_define.py
+-rw-r--r--   0 simon      (501) staff       (20)     3402 2023-04-26 19:25:50.000000 Simba-UW-tf-dev-1.58.1/simba/roi_tools/ROI_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/roi_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    19690 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.1/simba/roi_tools/ROI_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    11332 2023-04-26 21:13:20.000000 Simba-UW-tf-dev-1.58.1/simba/roi_tools/ROI_feature_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3651 2023-04-26 19:22:41.000000 Simba-UW-tf-dev-1.58.1/simba/roi_tools/ROI_multiply.py
+-rw-r--r--   0 simon      (501) staff       (20)      961 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/roi_tools/ROI_size_calculations.py
+-rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/roi_tools/ROI_zoom.py
+-rw-r--r--   0 simon      (501) staff       (20)    11384 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.1/simba/roi_tools/ROI_directing_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/roi_tools/ROI_move_shape.py
+-rw-r--r--   0 simon      (501) staff       (20)     5073 2023-04-25 14:55:41.000000 Simba-UW-tf-dev-1.58.1/simba/roi_tools/ROI_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)    13793 2023-04-26 14:59:42.000000 Simba-UW-tf-dev-1.58.1/simba/roi_tools/ROI_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    22685 2023-04-25 14:55:41.000000 Simba-UW-tf-dev-1.58.1/simba/roi_tools/ROI_image.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 15:16:29.000000 Simba-UW-tf-dev-1.58.1/simba/pose_importers/
+-rw-r--r--   0 simon      (501) staff       (20)     2464 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.1/simba/pose_importers/read_DANNCE_mat.py
+-rw-r--r--   0 simon      (501) staff       (20)    21991 2023-04-27 15:50:07.000000 Simba-UW-tf-dev-1.58.1/simba/pose_importers/sleap_importer_slp.py
+-rw-r--r--   0 simon      (501) staff       (20)    23507 2023-04-27 15:45:27.000000 Simba-UW-tf-dev-1.58.1/simba/pose_importers/sleap_importer_h5.py
+-rw-r--r--   0 simon      (501) staff       (20)    23579 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.1/simba/pose_importers/dlc_multi_animal_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-25 16:49:14.000000 Simba-UW-tf-dev-1.58.1/simba/pose_importers/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    21003 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.1/simba/pose_importers/sleap_importer_csv.py
+-rw-r--r--   0 simon      (501) staff       (20)     7761 2023-04-25 18:26:26.000000 Simba-UW-tf-dev-1.58.1/simba/pose_importers/import_mars.py
+-rw-r--r--   0 simon      (501) staff       (20)     6922 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.1/simba/pose_importers/dlc_importer_csv.py
+-rw-r--r--   0 simon      (501) staff       (20)     8100 2023-04-27 21:09:15.000000 Simba-UW-tf-dev-1.58.1/simba/pose_importers/trk_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)   238321 2023-04-28 00:09:50.000000 Simba-UW-tf-dev-1.58.1/simba/pop_up_classes.py
+-rw-r--r--   0 simon      (501) staff       (20)     4695 2023-04-26 18:17:53.000000 Simba-UW-tf-dev-1.58.1/simba/extract_seqframes.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 15:16:29.000000 Simba-UW-tf-dev-1.58.1/simba/pose_configurations/
+-rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.58.1/simba/pose_configurations/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 15:16:29.000000 Simba-UW-tf-dev-1.58.1/simba/pose_configurations/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.58.1/simba/pose_configurations/bp_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-10 12:22:28.000000 Simba-UW-tf-dev-1.58.1/simba/pose_configurations/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 15:16:29.000000 Simba-UW-tf-dev-1.58.1/simba/pose_configurations/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       24 2023-03-20 15:55:45.000000 Simba-UW-tf-dev-1.58.1/simba/pose_configurations/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.58.1/simba/pose_configurations/no_animals/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 15:16:29.000000 Simba-UW-tf-dev-1.58.1/simba/pose_configurations/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.58.1/simba/pose_configurations/configuration_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)      267 2023-03-20 15:55:45.000000 Simba-UW-tf-dev-1.58.1/simba/pose_configurations/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 15:16:29.000000 Simba-UW-tf-dev-1.58.1/simba/pose_configurations/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.58.1/simba/pose_configurations/schematics/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/pose_configurations/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.58.1/simba/pose_configurations/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/pose_configurations/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.58.1/simba/pose_configurations/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.58.1/simba/pose_configurations/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/pose_configurations/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/pose_configurations/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/pose_configurations/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/pose_configurations/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/pose_configurations/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/pose_configurations/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/pose_configurations/schematics/1.png
+-rw-r--r--   0 simon      (501) staff       (20)     7171 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.1/simba/get_coordinates_tools_v2.py
+-rw-r--r--   0 simon      (501) staff       (20)    15761 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.1/simba/pup_retrieval_protocol.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 15:16:29.000000 Simba-UW-tf-dev-1.58.1/simba/outlier_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     7427 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.1/simba/outlier_tools/outlier_corrector_movement.py
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-15 17:05:05.000000 Simba-UW-tf-dev-1.58.1/simba/outlier_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/outlier_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8191 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.1/simba/outlier_tools/outlier_corrector_location.py
+-rw-r--r--   0 simon      (501) staff       (20)     2706 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.1/simba/outlier_tools/skip_outlier_correction.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 15:16:29.000000 Simba-UW-tf-dev-1.58.1/simba/outlier_tools/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/outlier_tools/.idea/outlier_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/outlier_tools/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 15:16:29.000000 Simba-UW-tf-dev-1.58.1/simba/outlier_tools/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 15:16:29.000000 Simba-UW-tf-dev-1.58.1/simba/outlier_tools/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/outlier_tools/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/outlier_tools/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/outlier_tools/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/outlier_tools/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)     2613 2023-04-25 15:16:24.000000 Simba-UW-tf-dev-1.58.1/simba/pose_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)    18234 2023-04-27 17:03:57.000000 Simba-UW-tf-dev-1.58.1/simba/train_mutiple_models.py
+-rw-r--r--   0 simon      (501) staff       (20)    63955 2023-04-28 14:49:21.000000 Simba-UW-tf-dev-1.58.1/simba/SimBA.py
+-rw-r--r--   0 simon      (501) staff       (20)    26559 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.1/simba/labelling_advanced_interface.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 15:16:29.000000 Simba-UW-tf-dev-1.58.1/simba/assets/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 15:16:29.000000 Simba-UW-tf-dev-1.58.1/simba/assets/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/assets/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/assets/unsupervised/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/assets/unsupervised/features.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 15:16:29.000000 Simba-UW-tf-dev-1.58.1/simba/assets/shap/
+-rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/assets/shap/down_arrow.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/assets/shap/intruder_shape.jpg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 15:16:29.000000 Simba-UW-tf-dev-1.58.1/simba/assets/shap/feature_categories/
+-rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
+-rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/assets/shap/feature_categories/shap_feature_categories.csv
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-04-10 20:37:13.000000 Simba-UW-tf-dev-1.58.1/simba/assets/shap/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/assets/shap/resident_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/assets/shap/resident_intruder_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/assets/shap/animal_distances.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/assets/shap/baseline_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/assets/shap/ubuntu.regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/assets/shap/side_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/assets/shap/UbuntuMono-Regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/assets/shap/side_scale_5.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/assets/shap/intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/assets/shap/resident_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/assets/shap/color_bar.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/assets/shap/resident_intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)    16388 2023-04-25 19:14:34.000000 Simba-UW-tf-dev-1.58.1/simba/assets/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 15:16:29.000000 Simba-UW-tf-dev-1.58.1/simba/assets/lookups/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/assets/lookups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/assets/lookups/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)     2987 2023-04-25 20:39:03.000000 Simba-UW-tf-dev-1.58.1/simba/assets/lookups/feature_extraction_headers.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/assets/lookups/features.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/assets/lookups/unsupervised_example_x.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 15:16:29.000000 Simba-UW-tf-dev-1.58.1/simba/assets/stl/
+-rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/assets/stl/operant_tray.stl
+-rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/assets/stl/operant_lever.stl
+-rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/assets/stl/operant_walls.stl
+-rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/assets/stl/grid_floor.stl
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 15:16:29.000000 Simba-UW-tf-dev-1.58.1/simba/assets/img/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.58.1/simba/assets/img/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/assets/img/about_me.png
+-rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.58.1/simba/assets/img/splash.mp4
+-rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.58.1/simba/assets/img/bg_2.png
+-rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/assets/img/splash.pptx
+-rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.58.1/simba/assets/img/bg.png
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/assets/UbuntuMono-Regular.ttf
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 15:16:29.000000 Simba-UW-tf-dev-1.58.1/simba/assets/icons/
+-rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.58.1/simba/assets/icons/factory.png
+-rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.58.1/simba/assets/icons/cluster.png
+-rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.58.1/simba/assets/icons/load.png
+-rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.58.1/simba/assets/icons/gif.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.58.1/simba/assets/icons/pose.png
+-rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.58.1/simba/assets/icons/features.png
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.58.1/simba/assets/icons/.DS_Store
+-rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.58.1/simba/assets/icons/settings.png
+-rw-r--r--   0 simon      (501) staff       (20)     2090 2023-04-22 15:14:17.000000 Simba-UW-tf-dev-1.58.1/simba/assets/icons/stopwatch.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.58.1/simba/assets/icons/link.png
+-rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/assets/icons/dash_simba.css
+-rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.58.1/simba/assets/icons/documentation.png
+-rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.58.1/simba/assets/icons/fps.png
+-rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.58.1/simba/assets/icons/dimensionality_reduction.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.58.1/simba/assets/icons/roi.png
+-rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.58.1/simba/assets/icons/superimpose.png
+-rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.58.1/simba/assets/icons/label.png
+-rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.58.1/simba/assets/icons/change.png
+-rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.58.1/simba/assets/icons/crop.png
+-rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.58.1/simba/assets/icons/rotate.png
+-rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.58.1/simba/assets/icons/path.png
+-rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.58.1/simba/assets/icons/clip.png
+-rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.58.1/simba/assets/icons/restart.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.58.1/simba/assets/icons/calipher.png
+-rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.58.1/simba/assets/icons/add_on.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.58.1/simba/assets/icons/create.png
+-rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.58.1/simba/assets/icons/SimBA_logo.ico
+-rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.58.1/simba/assets/icons/print.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.58.1/simba/assets/icons/clf.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 15:16:29.000000 Simba-UW-tf-dev-1.58.1/simba/assets/icons/concat_icons/
+-rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/assets/icons/concat_icons/mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/assets/icons/concat_icons/vertical.png
+-rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/assets/icons/concat_icons/horizontal.png
+-rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/assets/icons/concat_icons/mixed_mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.58.1/simba/assets/icons/merge.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.58.1/simba/assets/icons/clean.png
+-rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.58.1/simba/assets/icons/clf_2.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.58.1/simba/assets/icons/visualize.png
+-rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.58.1/simba/assets/icons/concat.png
+-rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.58.1/simba/assets/icons/boris.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.58.1/simba/assets/icons/frames.png
+-rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.58.1/simba/assets/icons/video.png
+-rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.58.1/simba/assets/icons/sample.png
+-rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.58.1/simba/assets/icons/metrics.png
+-rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.58.1/simba/assets/icons/grey.png
+-rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.58.1/simba/assets/icons/exit.png
+-rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.58.1/simba/assets/icons/outlier.png
+-rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.58.1/simba/assets/icons/clahe.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.58.1/simba/assets/icons/trash.png
+-rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.58.1/simba/assets/icons/about.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.58.1/simba/assets/icons/convert.png
+-rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.58.1/simba/assets/icons/SimBA_logo.icns
+-rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.58.1/simba/assets/icons/reorganize.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.58.1/simba/assets/icons/browse.png
+-rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.58.1/simba/assets/icons/SimBA_logo.png
+-rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.58.1/simba/assets/icons/ethovision.png
+-rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.58.1/simba/assets/icons/close.png
+-rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/assets/dash_simba_base.css
+-rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/assets/TheGoldenLab.PNG
+-rw-r--r--   0 simon      (501) staff       (20)     9478 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.1/simba/read_config_unit_tests.py
+-rw-r--r--   0 simon      (501) staff       (20)    11645 2023-04-25 15:16:24.000000 Simba-UW-tf-dev-1.58.1/simba/project_config_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    19000 2023-04-26 18:08:54.000000 Simba-UW-tf-dev-1.58.1/simba/train_single_model.py
+-rw-r--r--   0 simon      (501) staff       (20)     6308 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.1/simba/create_clf_log.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 15:16:29.000000 Simba-UW-tf-dev-1.58.1/simba/batch_process_videos/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-17 14:43:38.000000 Simba-UW-tf-dev-1.58.1/simba/batch_process_videos/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    24639 2023-04-25 13:26:59.000000 Simba-UW-tf-dev-1.58.1/simba/batch_process_videos/batch_process_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.1/simba/batch_process_videos/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    11106 2023-04-25 13:26:59.000000 Simba-UW-tf-dev-1.58.1/simba/batch_process_videos/batch_process_create_ffmpeg_commands.py
+-rw-r--r--   0 simon      (501) staff       (20)     9520 2023-04-25 19:02:08.000000 Simba-UW-tf-dev-1.58.1/simba/Kleinberg_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8341 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.1/simba/reorganize_keypoint_in_pose.py
+-rw-r--r--   0 simon      (501) staff       (20)      165 2023-03-25 11:18:21.000000 Simba-UW-tf-dev-1.58.1/simba/~$features.pptx
+-rw-r--r--   0 simon      (501) staff       (20)     6543 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.1/simba/play_annotation_video.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 15:16:29.000000 Simba-UW-tf-dev-1.58.1/Simba_UW_tf_dev.egg-info/
+-rw-rw-r--   0 simon      (501) staff       (20)      579 2023-04-28 15:16:29.000000 Simba-UW-tf-dev-1.58.1/Simba_UW_tf_dev.egg-info/PKG-INFO
+-rw-rw-r--   0 simon      (501) staff       (20)    14165 2023-04-28 15:16:29.000000 Simba-UW-tf-dev-1.58.1/Simba_UW_tf_dev.egg-info/SOURCES.txt
+-rw-rw-r--   0 simon      (501) staff       (20)       44 2023-04-28 15:16:29.000000 Simba-UW-tf-dev-1.58.1/Simba_UW_tf_dev.egg-info/entry_points.txt
+-rw-rw-r--   0 simon      (501) staff       (20)      639 2023-04-28 15:16:29.000000 Simba-UW-tf-dev-1.58.1/Simba_UW_tf_dev.egg-info/requires.txt
+-rw-rw-r--   0 simon      (501) staff       (20)        6 2023-04-28 15:16:29.000000 Simba-UW-tf-dev-1.58.1/Simba_UW_tf_dev.egg-info/top_level.txt
+-rw-rw-r--   0 simon      (501) staff       (20)        1 2023-04-28 15:16:29.000000 Simba-UW-tf-dev-1.58.1/Simba_UW_tf_dev.egg-info/dependency_links.txt
+-rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.58.1/LICENSE.md
+-rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.58.1/MANIFEST.in
+-rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.58.1/README.md
+-rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-04-28 15:16:26.000000 Simba-UW-tf-dev-1.58.1/setup.py
+-rw-r--r--   0 simon      (501) staff       (20)       38 2023-04-28 15:16:29.000000 Simba-UW-tf-dev-1.58.1/setup.cfg
```

### Comparing `Simba-UW-tf-dev-1.57.9/PKG-INFO` & `Simba-UW-tf-dev-1.58.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.57.9
+Version: 1.58.1
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.57.9/simba/video_processing.py` & `Simba-UW-tf-dev-1.58.1/simba/video_processing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/blob_storage/.DS_Store` & `Simba-UW-tf-dev-1.58.1/simba/blob_storage/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/interpolate_smooth.py` & `Simba-UW-tf-dev-1.58.1/simba/interpolate_smooth.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/unsupervised/dbcv_calculator.py` & `Simba-UW-tf-dev-1.58.1/simba/unsupervised/dbcv_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/unsupervised/enums.py` & `Simba-UW-tf-dev-1.58.1/simba/unsupervised/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.58.1/simba/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/unsupervised/dataset_creator.py` & `Simba-UW-tf-dev-1.58.1/simba/unsupervised/dataset_creator.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,14 +13,26 @@
 from simba.utils.printing import stdout_success
 
 class DatasetCreator(ConfigReader, UnsupervisedMixin):
     def __init__(self,
                  config_path: str,
                  settings: dict):
 
+        """
+        Class for transforming raw frame-wise supervised classification data into aggregated
+        data for unsupervised analyses.
+
+        :param config_path: path to SimBA configparser.ConfigParser project_config.ini
+        :param settings: user attributes for how the data should be aggregated.
+
+        :example:
+        >>> settings = {'data_slice': 'ALL FEATURES (EXCLUDING POSE)', 'clf_slice': 'Attack', 'bout_aggregation_type': 'MEDIAN', 'min_bout_length': 66, 'feature_path': '/Users/simon/Desktop/envs/simba_dev/simba/assets/unsupervised/features.csv'}
+        >>> _ = DatasetCreator(config_path='/Users/simon/Desktop/envs/troubleshooting/unsupervised/project_folder/project_config.ini', settings=settings)
+        """
+
         print('Creating unsupervised learning dataset...')
         ConfigReader.__init__(self, config_path=config_path)
         UnsupervisedMixin.__init__(self)
         check_if_filepath_list_is_empty(filepaths=self.machine_results_paths, error_msg='NO MACHINE LEARNING DATA FOUND')
         self.settings = settings
         self.clf_type, self.feature_lst = None, None
         self.save_path = os.path.join(self.logs_path, 'unsupervised_data_{}.pickle'.format(self.datetime))
```

### Comparing `Simba-UW-tf-dev-1.57.9/simba/unsupervised/grid_search_visualizers.py` & `Simba-UW-tf-dev-1.58.1/simba/unsupervised/grid_search_visualizers.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,14 +12,28 @@
 
 
 class GridSearchVisualizer(UnsupervisedMixin):
     def __init__(self,
                  model_dir: str,
                  save_dir: str,
                  settings: dict):
+        """
+        Class for visualizing grid-searched hyper-parameters in .png format.
+
+        :param model_dir: path to pickle holding unsupervised results in ``data_map.yaml`` format.
+        :param save_dir: directory holding one or more unsupervised results in pickle ``data_map.yaml`` format.
+        :param settings: User-defined image attributes (e.g., continous and catehorical palettes)
+
+        :example:
+        >>> settings = {'CATEGORICAL_PALETTE': 'Pastel1', 'SCATTER_SIZE': 10}
+        >>> visualizer = GridSearchVisualizer(model_dir='/Users/simon/Desktop/envs/troubleshooting/unsupervised/cluster_models_042023', save_dir='/Users/simon/Desktop/envs/troubleshooting/unsupervised/images', settings=settings)
+        >>> visualizer.continuous_visualizer(continuous_vars=['START_FRAME'])
+        >>> visualizer.categorical_visualizer(categoricals=['CLUSTER'])
+        """
+
 
         super().__init__()
         check_if_dir_exists(in_dir=save_dir)
         check_if_dir_exists(in_dir=model_dir)
         self.save_dir, self.settings, self.model_dir = save_dir, settings, model_dir
         self.data_path = glob.glob(model_dir + '/*.pickle')
         check_if_filepath_list_is_empty(filepaths=self.data_path, error_msg=f'SIMBA ERROR: No pickle files in {model_dir}')
```

### Comparing `Simba-UW-tf-dev-1.57.9/simba/unsupervised/data_extractor.py` & `Simba-UW-tf-dev-1.58.1/simba/unsupervised/data_extractor.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,26 @@
 class DataExtractor(UnsupervisedMixin, ConfigReader):
     def __init__(self,
                  config_path: str,
                  data_path: str,
                  data_type: str,
                  settings: dict or None=None):
 
+        """
+
+        :param config_path: path to SimBA configparser.ConfigParser project_config.ini
+        :param data_path: path to pickle holding unsupervised results in ``data_map.yaml`` format.
+        :param data_type: The type of data to extract.
+        :param settings: User-defined parameters for data extraction.
+
+        :example:
+        >>> extractor = DataExtractor(data_path='unsupervised/cluster_models/awesome_curran.pickle', data_type='BOUTS_TARGETS', settings=None, config_path='unsupervised/project_folder/project_config.ini')
+        >>> extractor.run()
+        """
+
         ConfigReader.__init__(self, config_path=config_path)
         UnsupervisedMixin.__init__(self)
         if os.path.isdir(data_path):
             check_if_dir_exists(in_dir=data_path)
             self.data = self.read_pickle(data_path=data_path)
         else:
             check_file_exist_and_readable(file_path=data_path)
```

### Comparing `Simba-UW-tf-dev-1.57.9/simba/unsupervised/ui.py` & `Simba-UW-tf-dev-1.58.1/simba/unsupervised/ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/unsupervised/umap_embedder.py` & `Simba-UW-tf-dev-1.58.1/simba/unsupervised/umap_embedder.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,18 +19,37 @@
     from umap import UMAP
 
 class UmapEmbedder(UnsupervisedMixin):
 
     def __init__(self):
         super().__init__()
 
+    """
+    Methods for grid-search UMAP model fit and transform.
+    Defaults to GPU and cuml.UMAP if GPU available. If GPU unavailable, then umap.UMAP.
+    """
+
     def fit(self,
             data_path: str,
             save_dir: str,
             hyper_parameters: dict):
+        """
+
+        :param data_path: Path holding pickled data-set created by `simba.unsupervised.dataset_creator.DatasetCreator.
+        :param save_dir: Empty directory where to save the UMAP results.
+        :param hyper_parameters: dict holding UMAP hyperparameters in list format.
+
+        :Example I: Fit.
+        >>> hyper_parameters = {'n_neighbors': [10, 2], 'min_distance': [1.0], 'spread': [1.0], 'scaler': 'MIN-MAX', 'variance': 0.25}
+        >>> data_path = 'unsupervised/project_folder/logs/unsupervised_data_20230416145821.pickle'
+        >>> save_dir = 'unsupervised/dr_models'
+        >>> config_path = 'unsupervised/project_folder/project_config.ini'
+        >>> embedder = UmapEmbedder(data_path=data_path, save_dir=save_dir)
+        >>> embedder.fit(hyper_parameters=hyper_parameters)
+        """
 
         self.data_path = data_path
         check_file_exist_and_readable(file_path=self.data_path)
         self.data = self.read_pickle(data_path=data_path)
         self.umap_df = deepcopy(self.data[Unsupervised.BOUTS_FEATURES.value]).set_index([Unsupervised.VIDEO.value, Unsupervised.START_FRAME.value, Unsupervised.END_FRAME.value])
         self.save_dir = save_dir
         self.check_that_directory_is_empty(directory=self.save_dir)
@@ -90,14 +109,31 @@
 
     def transform(self,
                   data_path: str,
                   model: str or dict,
                   settings: dict,
                   save_dir: str or None=None):
 
+        """
+
+        :param data_path:
+        :param model:
+        :param settings:
+        :param save_dir:
+        :return:
+
+        :Example I: Transform.
+        >>> data_path = 'unsupervised/project_folder/logs/unsupervised_data_20230416145821.pickle'
+        >>> save_dir = 'unsupervised/transformed_umap'
+        >>> settings = {'DATA': 'RAW', 'format': 'csv'}
+        >>> embedder = UmapEmbedder(data_path=data_path, save_dir=save_dir)
+        >>> embedder.transform(model='unsupervised/dr_models/boring_lederberg.pickle', settings=settings)
+
+        """
+
         timer = SimbaTimer(start=True)
         if isinstance(model, str):
             check_file_exist_and_readable(file_path=model)
             model = self.read_pickle(data_path=model)
 
         check_file_exist_and_readable(file_path=data_path)
         data = self.read_pickle(data_path=data_path)
```

### Comparing `Simba-UW-tf-dev-1.57.9/simba/unsupervised/pop_up_classes.py` & `Simba-UW-tf-dev-1.58.1/simba/unsupervised/pop_up_classes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 __author__ = "Simon Nilsson"
 
+""" Tkinter pop-up classes for unsupervised ML"""
+
 import glob
 from tkinter import *
 import numpy as np
 
 from simba.tkinter_functions import (FolderSelect,
                                      DropDownMenu,
                                      FileSelect,
```

### Comparing `Simba-UW-tf-dev-1.57.9/simba/unsupervised/bout_aggregator.py` & `Simba-UW-tf-dev-1.58.1/simba/unsupervised/bout_aggregator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 __author__ = "Simon Nilsson"
 
-
 import pandas as pd
 from joblib.externals.loky import get_reusable_executor
 from joblib import Parallel, delayed
 from simba.utils.read_write import read_video_info
 from simba.utils.data import detect_bouts
 
 def bout_aggregator(data: pd.DataFrame,
```

### Comparing `Simba-UW-tf-dev-1.57.9/simba/unsupervised/cluster_statistics.py` & `Simba-UW-tf-dev-1.58.1/simba/unsupervised/cluster_statistics.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,28 +48,40 @@
 
 
 class ClusterFrequentistCalculator(UnsupervisedMixin, ConfigReader):
     def __init__(self,
                  config_path: str,
                  data_path: str,
                  settings: dict):
+        """
+        Class for computing frequentist statitics based on cluster assignment labels (for explainability purposes).
+
+        :param str config_path: path to SimBA configparser.ConfigParser project_config.ini
+        :param str data_path: path to pickle holding unsupervised results in ``data_map.yaml`` format.
+        :param dict settings: dict holding which statistical tests to use
+
+        :Example:
+        >>> settings = {'scaled': True, 'ANOVA': True, 'tukey_posthoc': True, 'descriptive_statistics': True}
+        >>> calculator = ClusterFrequentistCalculator(config_path='unsupervised/project_folder/project_config.ini', data_path='unsupervised/cluster_models/quizzical_rhodes.pickle', settings=settings)
+        >>> calculator.run()
+        """
 
         ConfigReader.__init__(self, config_path=config_path)
         UnsupervisedMixin.__init__(self)
         self.settings = settings
         check_file_exist_and_readable(file_path=data_path)
         self.data = self.read_pickle(data_path=data_path)
         self.save_path = os.path.join(self.logs_path, f'cluster_descriptive_statistics_{self.data[Clustering.CLUSTER_MODEL.value][Unsupervised.HASHED_NAME.value]}_{self.datetime}.xlsx')
         self.check_key_exist_in_object(object=self.data, key=Clustering.CLUSTER_MODEL.value)
 
 
     def run(self):
         self.x_data = self.data[Unsupervised.METHODS.value][Unsupervised.SCALED_DATA.value]
         self.cluster_data = self.data[Clustering.CLUSTER_MODEL.value][Unsupervised.MODEL.value].labels_
-        if not settings[Unsupervised.SCALED.value]:
+        if not self.settings[Unsupervised.SCALED.value]:
             self.feature_data = self.scaler_inverse_transform(scaler=self.data[Unsupervised.METHODS.value][Unsupervised.SCALER.value], data=self.x_data)
         self.x_y_df = pd.concat([self.x_data, pd.DataFrame(self.cluster_data, columns=[CLUSTER], index=self.x_data.index)], axis=1)
         self.cluster_cnt = self.get_cluster_cnt(data=self.cluster_data, clusterer_name=self.data[Clustering.CLUSTER_MODEL.value][Unsupervised.HASHED_NAME.value], minimum_clusters=2)
         with pd.ExcelWriter(self.save_path, mode='w') as writer:
             pd.DataFrame().to_excel(writer, sheet_name=' ', index=True)
         if self.settings[Methods.ANOVA.value]:
             self.__one_way_anovas()
@@ -132,14 +144,27 @@
 
 class EmbeddingCorrelationCalculator(UnsupervisedMixin, ConfigReader):
     def __init__(self,
                  data_path: str,
                  config_path: str,
                  settings: dict):
 
+        """
+        Class for correlating dimensionality reduction features with original features (for explainability purposes)
+
+        :param str config_path: path to SimBA configparser.ConfigParser project_config.ini
+        :param str data_path: path to pickle holding unsupervised results in ``data_map.yaml`` format.
+        :param dict settings: dict holding which statistical tests to use and how to create plots.
+
+        :Example:
+        >>> settings = {'correlation_methods': ['pearson', 'kendall', 'spearman'], 'plots': {'create': True, 'correlations': 'pearson', 'palette': 'jet'}}
+        >>> calculator = EmbeddingCorrelationCalculator(config_path='unsupervised/project_folder/project_config.ini', data_path='unsupervised/cluster_models/quizzical_rhodes.pickle', settings=settings)
+        >>> calculator.run()
+        """
+
         ConfigReader.__init__(self, config_path=config_path)
         UnsupervisedMixin.__init__(self)
         check_file_exist_and_readable(file_path=data_path)
         self.settings, self.data_path = settings, data_path
         self.data = self.read_pickle(data_path=self.data_path)
         self.save_path = os.path.join(self.logs_path, f'embedding_correlations_{self.data[Unsupervised.DR_MODEL.value][Unsupervised.HASHED_NAME.value]}_{self.datetime}.csv')
 
@@ -178,14 +203,27 @@
 
 class ClusterXAICalculator(UnsupervisedMixin, ConfigReader):
     def __init__(self,
                  data_path: str,
                  config_path: str,
                  settings: dict):
 
+        """
+        Class for building RF models on top of cluster assignments, and calculating explainability metrics on RF models
+
+        :param str config_path: path to SimBA configparser.ConfigParser project_config.ini
+        :param str data_path: path to pickle holding unsupervised results in ``data_map.yaml`` format.
+        :param dict settings: dict holding which tests to use.
+
+        :Example:
+        >>> settings = {'gini_importance': True, 'permutation_importance': True, 'shap': {'method': 'cluster_paired', 'create': True, 'sample': 100}}
+        >>> calculator = ClusterXAICalculator(config_path='unsupervised/project_folder/project_config.ini', data_path='unsupervised/cluster_models/quizzical_rhodes.pickle', settings=settings)
+        >>> calculator.run()
+        """
+
         ConfigReader.__init__(self, config_path=config_path)
         UnsupervisedMixin.__init__(self)
         self.settings, self.data_path = settings, data_path
         check_file_exist_and_readable(file_path=data_path)
         self.data = self.read_pickle(data_path=self.data_path)
         self.save_path = os.path.join(self.logs_path, f'cluster_xai_statistics_{self.data[Unsupervised.DR_MODEL.value][Unsupervised.HASHED_NAME.value]}_{self.datetime}.xlsx')
```

### Comparing `Simba-UW-tf-dev-1.57.9/simba/unsupervised/data_map.yaml` & `Simba-UW-tf-dev-1.58.1/simba/unsupervised/data_map.yaml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/unsupervised/hdbscan_clusterer.py` & `Simba-UW-tf-dev-1.58.1/simba/unsupervised/hdbscan_clusterer.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 try:
     from cuml.cluster.hdbscan import HDBSCAN
     from cuml.cluster import hdbscan
     gpu_flag = True
 except ModuleNotFoundError:
     from hdbscan import HDBSCAN
     import hdbscan
+
 import itertools
 import os, glob
 import random
 import pandas as pd
 from simba.utils.checks import check_if_dir_exists, check_file_exist_and_readable, check_if_filepath_list_is_empty
 from simba.unsupervised.enums import Clustering, Unsupervised
 from simba.utils.printing import stdout_success, SimbaTimer
@@ -18,20 +19,42 @@
 from simba.unsupervised.umap_embedder import UmapEmbedder
 
 
 
 class HDBSCANClusterer(UnsupervisedMixin):
     def __init__(self):
         super().__init__()
+    """
+    Methods for grid-search HDBSCAN model fit and transform.
+    Defaults to GPU and cuml.cluster.HDBSCAN. If GPU unavailable, then hdbscan.HDBSCAN.
+    """
+
 
     def fit(self,
             data_path: str,
             save_dir: str,
             hyper_parameters: dict):
 
+        """
+        :param data_path: Path holding pickled unsupervised dimensionality reduction results in ``data_map.yaml`` format
+        :param save_dir: Empty directory where to save the HDBSCAN results.
+        :param hyper_parameters: dict holding hyperparameters in list format
+        :return:
+
+        :Example I: Grid-search fit:
+        >>> hyper_parameters = {'alpha': [1.0], 'min_cluster_size': [10], 'min_samples': [1], 'cluster_selection_epsilon': [20]}
+        >>> embedding_dir = '/Users/simon/Desktop/envs/troubleshooting/unsupervised/dr_models'
+        >>> save_dir = '/Users/simon/Desktop/envs/troubleshooting/unsupervised/cluster_models'
+        >>> config_path = '/Users/simon/Desktop/envs/troubleshooting/unsupervised/project_folder/project_config.ini'
+        >>> clusterer = HDBSCANClusterer(data_path=embedding_dir, save_dir=save_dir)
+        >>> clusterer.fit(hyper_parameters=hyper_parameters)
+        """
+
+
+
         self.save_dir, self.data_path = save_dir, data_path
         self.check_that_directory_is_empty(directory=self.save_dir)
         if os.path.isdir(data_path):
             check_if_dir_exists(in_dir=data_path)
             check_if_filepath_list_is_empty(filepaths=glob.glob(data_path + '/*.pickle'), error_msg=f'SIMBA ERROR: No pickle files in {data_path}')
         else:
             check_file_exist_and_readable(file_path=data_path)
@@ -81,21 +104,33 @@
                 self.__save(data=results)
 
     def __save(self, data: dict) -> None:
         self.write_pickle(data=data, save_path=os.path.join(self.save_dir, f'{self.model[Unsupervised.HASHED_NAME.value]}.pickle'))
         self.model_timer.stop_timer()
         stdout_success(msg=f'Model {self.model_counter}/{len(self.search_space) * len(list(self.embeddings.keys()))} ({self.model[Unsupervised.HASHED_NAME.value]}) saved...', elapsed_time=self.model_timer.elapsed_time)
 
-
     def transform(self,
                   data_path: str,
                   model: str or dict,
                   save_dir: str or None=None,
                   settings: dict or None=None):
 
+        """
+        :param data_path: Path to directory holding pickled unsupervised dimensionality reduction results in ``data_map.yaml`` format
+        :param model: Path to pickle holding hdbscan model in ``data_map.yaml`` format.
+        :param save_dir: Empty directory where to save the HDBSCAN results. If none, then keep results in memory under self.results.
+        :param settings: User-defined params.
+
+        :Example I: Transform:
+        >>> data_path = 'project_folder/logs/unsupervised_data_20230416145821.pickle'
+        >>> save_path = 'unsupervised/dr_models'
+        >>> clusterer = HDBSCANClusterer(data_path=data_path, save_dir=save_path)
+        >>> clusterer.transform(model='/Users/simon/Desktop/envs/troubleshooting/unsupervised/cluster_models/awesome_curran.pickle', settings={'DATA': None}, data_path=data_path)
+        """
+
         timer = SimbaTimer()
         timer.start_timer()
         if isinstance(model, str):
             check_file_exist_and_readable(file_path=model)
             model = self.read_pickle(data_path=model)
 
         check_file_exist_and_readable(file_path=data_path)
```

### Comparing `Simba-UW-tf-dev-1.57.9/simba/unsupervised/tsne.py` & `Simba-UW-tf-dev-1.58.1/simba/unsupervised/tsne.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/unsupervised/cluster_visualizer.py` & `Simba-UW-tf-dev-1.58.1/simba/unsupervised/cluster_visualizer.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,14 +27,28 @@
 class ClusterVisualizer(ConfigReader, UnsupervisedMixin):
     def __init__(self,
                  config_path: str,
                  video_dir: str,
                  data_path: str,
                  settings: dict):
 
+        """
+        Class for creating video examples of cluster assignments.
+
+        :param str config_path: path to SimBA configparser.ConfigParser project_config.ini
+        :param str data_path: path to pickle holding unsupervised results in ``data_map.yaml`` format.
+        :param str video_dir: path to directory holding videos.
+        :param dict settings: dict holding attributes of the videos
+
+        :Example:
+        >>> settings = {'video_speed': 0.5, 'pose': {'create': True, 'circle_size': 5}}
+        >>> visualizer = ClusterVisualizer(video_dir='unsupervised/project_folder/videos', data_path='unsupervised/cluster_models/quizzical_rhodes.pickle', settings=settings, config_path='unsupervised/project_folder/project_config.ini')
+        >>> visualizer.run()
+        """
+
         ConfigReader.__init__(self, config_path=config_path)
         UnsupervisedMixin.__init__(self)
         self.settings, self.video_dir, self.data_path = settings, video_dir, data_path
         self.save_parent_dir = os.path.join(self.project_path, Paths.CLUSTER_EXAMPLES.value)
         if not os.path.exists(self.save_parent_dir): os.makedirs(self.save_parent_dir)
         check_file_exist_and_readable(file_path=data_path)
         self.fourcc = cv2.VideoWriter_fourcc(*Formats.MP4_CODEC.value)
```

### Comparing `Simba-UW-tf-dev-1.57.9/simba/enums.py` & `Simba-UW-tf-dev-1.58.1/simba/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/bounding_box_tools/.DS_Store` & `Simba-UW-tf-dev-1.58.1/simba/bounding_box_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/bounding_box_tools/agg_boundary_stats.py` & `Simba-UW-tf-dev-1.58.1/simba/bounding_box_tools/agg_boundary_stats.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/bounding_box_tools/boundary_menus.py` & `Simba-UW-tf-dev-1.58.1/simba/bounding_box_tools/boundary_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/bounding_box_tools/boundary_statistics.py` & `Simba-UW-tf-dev-1.58.1/simba/bounding_box_tools/boundary_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/bounding_box_tools/find_boundaries.py` & `Simba-UW-tf-dev-1.58.1/simba/bounding_box_tools/find_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/bounding_box_tools/visualize_boundaries.py` & `Simba-UW-tf-dev-1.58.1/simba/bounding_box_tools/visualize_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/.DS_Store` & `Simba-UW-tf-dev-1.58.1/simba/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/feature_extractor_14bp.py` & `Simba-UW-tf-dev-1.58.1/simba/feature_extractors/feature_extractor_14bp.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,17 +66,17 @@
             video_settings, self.px_per_mm, fps = self.read_video_info(video_name=self.video_name)
             for window in self.roll_windows_values:
                 roll_windows.append(int(fps / window))
             self.in_data = read_df(file_path, self.file_type).fillna(0).apply(pd.to_numeric).reset_index(drop=True)
             print('Processing {} ({} frames)...'.format(self.video_name, str(len(self.in_data))))
             self.in_data = self.insert_default_headers_for_feature_extraction(df=self.in_data, headers=self.in_headers, pose_config='14 body-parts', filename=file_path)
             self.out_data = deepcopy(self.in_data)
-            mouse_1_ar = np.reshape(self.out_data[self.mouse_1_headers].values, (len(self.out_data / 2), -1, 2))
+            mouse_1_ar = np.reshape(self.out_data[self.mouse_1_headers].values, (len(self.out_data / 2), -1, 2)).astype(np.float32)
             self.out_data['Mouse_1_poly_area'] = jitted_hull(points=mouse_1_ar, target=Formats.PERIMETER.value) / self.px_per_mm
-            mouse_2_ar = np.reshape(self.out_data[self.mouse_2_headers].values, (len(self.out_data / 2), -1, 2))
+            mouse_2_ar = np.reshape(self.out_data[self.mouse_2_headers].values, (len(self.out_data / 2), -1, 2)).astype(np.float32)
             self.out_data['Mouse_2_poly_area'] = jitted_hull(points=mouse_2_ar, target=Formats.PERIMETER.value) / self.px_per_mm
             self.in_data_shifted = self.out_data.shift(periods=1).add_suffix('_shifted').fillna(0)
             self.in_data = pd.concat([self.in_data, self.in_data_shifted], axis=1, join='inner').fillna(0).reset_index(drop=True)
             self.out_data['Mouse_1_nose_to_tail'] = self.euclidean_distance(self.out_data['Nose_1_x'].values, self.out_data['Tail_base_1_x'].values, self.out_data['Nose_1_y'].values, self.out_data['Tail_base_1_y'].values, self.px_per_mm)
             self.out_data['Mouse_2_nose_to_tail'] = self.euclidean_distance(self.out_data['Nose_2_x'].values, self.out_data['Tail_base_2_x'].values, self.out_data['Nose_2_y'].values, self.out_data['Tail_base_2_y'].values, self.px_per_mm)
             self.out_data['Mouse_1_width'] = self.euclidean_distance(self.out_data['Lat_left_1_x'].values, self.out_data['Lat_right_1_x'].values, self.out_data['Lat_left_1_y'].values, self.out_data['Lat_right_1_y'].values, self.px_per_mm)
             self.out_data['Mouse_2_width'] = self.euclidean_distance(self.out_data['Lat_left_2_x'].values, self.out_data['Lat_right_2_x'].values, self.out_data['Lat_left_2_y'].values, self.out_data['Lat_right_2_y'].values, self.px_per_mm)
```

### Comparing `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/feature_extractor_7bp.py` & `Simba-UW-tf-dev-1.58.1/simba/feature_extractors/feature_extractor_7bp.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
             roll_windows = []
             for window in self.roll_windows_values:
                 roll_windows.append(int(fps / window))
             self.in_data = read_df(file_path, self.file_type).fillna(0).apply(pd.to_numeric).reset_index(drop=True)
             print('Processing {} ({} frames)...'.format(self.video_name, str(len(self.in_data))))
             self.in_data = self.insert_default_headers_for_feature_extraction(df=self.in_data, headers=self.in_headers, pose_config='7 body-parts', filename=file_path)
             self.out_data = deepcopy(self.in_data)
-            mouse_array = np.reshape(self.out_data[self.mouse_headers].values, (len(self.out_data / 2), -1, 2))
+            mouse_array = np.reshape(self.out_data[self.mouse_headers].values, (len(self.out_data / 2), -1, 2)).astype(np.float32)
             self.out_data['Mouse_poly_area'] = jitted_hull(points=mouse_array, target='perimeter') / self.px_per_mm
             self.in_data_shifted = self.out_data.shift(periods=1).add_suffix('_shifted').fillna(0)
             self.in_data = pd.concat([self.out_data, self.in_data_shifted], axis=1, join='inner').fillna(0).reset_index(drop=True)
             self.out_data['Mouse_nose_to_tail'] = self.euclidean_distance(self.in_data['Nose_x'].values, self.in_data['Tail_base_x'].values, self.in_data['Nose_y'].values, self.in_data['Tail_base_y'].values, self.px_per_mm)
             self.out_data['Mouse_width'] = self.euclidean_distance(self.in_data['Lat_left_x'].values, self.in_data['Lat_right_x'].values, self.in_data['Lat_left_y'].values, self.in_data['Lat_right_y'].values, self.px_per_mm)
             self.out_data['Mouse_Ear_distance'] = self.euclidean_distance(self.in_data['Ear_left_x'].values, self.in_data['Ear_right_x'].values, self.in_data['Ear_left_y'].values, self.in_data['Ear_right_y'].values, self.px_per_mm)
             self.out_data['Mouse_Nose_to_centroid'] = self.euclidean_distance(self.in_data['Nose_x'].values, self.in_data['Center_x'].values, self.in_data['Nose_y'].values, self.in_data['Center_y'].values, self.px_per_mm)
```

### Comparing `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/doctests.py` & `Simba-UW-tf-dev-1.58.1/simba/feature_extractors/misc/doctests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py` & `Simba-UW-tf-dev-1.58.1/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/read_in_mp.py` & `Simba-UW-tf-dev-1.58.1/simba/feature_extractors/misc/read_in_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/peaks.py` & `Simba-UW-tf-dev-1.58.1/simba/feature_extractors/misc/peaks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/fish_feature_extractor_2022.py` & `Simba-UW-tf-dev-1.58.1/simba/feature_extractors/misc/fish_feature_extractor_2022.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/convex_hull_3_scratch_3.py` & `Simba-UW-tf-dev-1.58.1/simba/feature_extractors/misc/convex_hull_3_scratch_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/convex_hull_scratch_1.py` & `Simba-UW-tf-dev-1.58.1/simba/feature_extractors/misc/convex_hull_scratch_1.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/.DS_Store` & `Simba-UW-tf-dev-1.58.1/simba/feature_extractors/misc/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py` & `Simba-UW-tf-dev-1.58.1/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/egocentrical_aligner.py` & `Simba-UW-tf-dev-1.58.1/simba/feature_extractors/misc/egocentrical_aligner.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/count_values_in_range.py` & `Simba-UW-tf-dev-1.58.1/simba/feature_extractors/misc/count_values_in_range.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/graph_creator.py` & `Simba-UW-tf-dev-1.58.1/simba/feature_extractors/misc/graph_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/termite_rois.csv` & `Simba-UW-tf-dev-1.58.1/simba/feature_extractors/misc/termite_rois.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/mutual_exclusive.py` & `Simba-UW-tf-dev-1.58.1/simba/feature_extractors/misc/mutual_exclusive.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/video_color.py` & `Simba-UW-tf-dev-1.58.1/simba/feature_extractors/misc/video_color.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/graph_3d_plotter.py` & `Simba-UW-tf-dev-1.58.1/simba/feature_extractors/misc/graph_3d_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/video_rotator.py` & `Simba-UW-tf-dev-1.58.1/simba/feature_extractors/misc/video_rotator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/add_probability_cnt_features.py` & `Simba-UW-tf-dev-1.58.1/simba/feature_extractors/misc/add_probability_cnt_features.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/make_splash.py` & `Simba-UW-tf-dev-1.58.1/simba/feature_extractors/misc/make_splash.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/time_stamp_calculator.py` & `Simba-UW-tf-dev-1.58.1/simba/feature_extractors/misc/time_stamp_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/video_rotator_mp.py` & `Simba-UW-tf-dev-1.58.1/simba/feature_extractors/misc/video_rotator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py` & `Simba-UW-tf-dev-1.58.1/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/convex_hull_scratch_2.py` & `Simba-UW-tf-dev-1.58.1/simba/feature_extractors/misc/convex_hull_scratch_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/feature_extractor_8bps_2_animals.py` & `Simba-UW-tf-dev-1.58.1/simba/feature_extractors/feature_extractor_8bps_2_animals.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,17 +63,17 @@
             video_settings, self.px_per_mm, fps = self.read_video_info(video_name=self.video_name)
             for window in self.roll_windows_values:
                 roll_windows.append(int(fps / window))
             self.in_data = read_df(file_path, self.file_type).fillna(0).apply(pd.to_numeric).reset_index(drop=True)
             print('Processing {} ({} frames)...'.format(self.video_name, str(len(self.in_data))))
             self.in_data = self.insert_default_headers_for_feature_extraction(df=self.in_data, headers=self.in_headers, pose_config='8 body-parts from 2 animals', filename=file_path)
             self.out_data = deepcopy(self.in_data)
-            mouse_1_ar = np.reshape(self.out_data[self.mouse_1_headers].values, (len(self.out_data / 2), -1, 2))
+            mouse_1_ar = np.reshape(self.out_data[self.mouse_1_headers].values, (len(self.out_data / 2), -1, 2)).astype(np.float32)
             self.out_data['Mouse_1_poly_area'] = jitted_hull(points=mouse_1_ar, target=Formats.PERIMETER.value) / self.px_per_mm
-            mouse_2_ar = np.reshape(self.out_data[self.mouse_2_headers].values, (len(self.out_data / 2), -1, 2))
+            mouse_2_ar = np.reshape(self.out_data[self.mouse_2_headers].values, (len(self.out_data / 2), -1, 2)).astype(np.float32)
             self.out_data['Mouse_2_poly_area'] = jitted_hull(points=mouse_2_ar, target=Formats.PERIMETER.value) / self.px_per_mm
             self.in_data_shifted = self.out_data.shift(periods=1).add_suffix('_shifted').fillna(0)
             self.in_data = pd.concat([self.in_data, self.in_data_shifted], axis=1, join='inner').fillna(0).reset_index(drop=True)
             self.out_data['Mouse_1_nose_to_tail'] = self.euclidean_distance(self.out_data['Nose_1_x'].values, self.out_data['Tail_base_1_x'].values, self.out_data['Nose_1_y'].values, self.out_data['Tail_base_1_y'].values, self.px_per_mm)
             self.out_data['Mouse_2_nose_to_tail'] = self.euclidean_distance(self.out_data['Nose_2_x'].values, self.out_data['Tail_base_2_x'].values, self.out_data['Nose_2_y'].values, self.out_data['Tail_base_2_y'].values, self.px_per_mm)
             self.out_data['Mouse_1_Ear_distance'] = self.euclidean_distance(self.out_data['Ear_left_1_x'].values, self.out_data['Ear_right_1_x'].values, self.out_data['Ear_left_1_y'].values, self.out_data['Ear_right_1_y'].values, self.px_per_mm)
             self.out_data['Mouse_2_Ear_distance'] = self.euclidean_distance(self.out_data['Ear_left_2_x'].values, self.out_data['Ear_right_2_x'].values, self.out_data['Ear_left_2_y'].values, self.out_data['Ear_right_2_y'].values, self.px_per_mm)
```

### Comparing `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/.DS_Store` & `Simba-UW-tf-dev-1.58.1/simba/feature_extractors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/perimeter_jit.py` & `Simba-UW-tf-dev-1.58.1/simba/feature_extractors/perimeter_jit.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 
 ### modified from https://stackoverflow.com/questions/74812556/computing-quick-convex-hull-using-numba/74817179#74817179
 
 import numpy as np
 from numba import njit, prange
 from numba.np.extensions import cross2d
 
-@njit('(float64[:,:], int64[:], int64, int64)')
+@njit('(float32[:,:], int64[:], int64, int64)')
 def process(S, P, a, b):
     signed_dist = cross2d(S[P] - S[a], S[b] - S[a])
     K = np.array([i for s, i in zip(signed_dist, P) if s > 0 and i != a and i != b], dtype=np.int64)
     if len(K) == 0:
         return [a, b]
     c = P[np.argmax(signed_dist)]
     return process(S, K, a, c)[:-1] + process(S, K, c, b)
 
-@njit('(float64[:, :,:], types.unicode_type)', fastmath=True)
-def jitted_hull(points: np.ndarray, target: str='perimeter') -> np.ndarray:
+@njit('(float32[:, :,:], types.unicode_type)', fastmath=True)
+def jitted_hull(points: np.ndarray, target: str = 'perimeter') -> np.ndarray:
 
     """
     :param array points: 3d array FRAMESxBODY-PARTxCOORDINATE
     :param str target: Options [perimeter, area]
     :return: 1d np.array
 
     :EXAMPLE:
@@ -57,10 +57,8 @@
         x_sorted, y_sorted = x[mask], y[mask]
         if target == 'perimeter':
             xy = np.vstack((x_sorted, y_sorted)).T
             results[i] = perimeter(xy)
         if target == 'area':
             results[i] = area(x_sorted, y_sorted)
 
-    return results
-
-
+    return results
```

### Comparing `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/feature_subsets.py` & `Simba-UW-tf-dev-1.58.1/simba/feature_extractors/feature_subsets.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,28 +85,28 @@
                 col_names = list(sum([(x + '_x', y + '_y') for (x, y) in zip(point, point)], ()))
                 self.results[f'Angle (degrees) {point[0]}-{point[1]}-{point[2]}'] = self.angle3pt_serialized(data=self.df[col_names].values)
 
     def calc_three_point_hulls(self):
         for animal, points in self.within_animal_three_point_combs.items():
             for point in points:
                 col_names = list(sum([(x + '_x', y + '_y') for (x, y) in zip(point, point)], ()))
-                three_point_arr = np.reshape(self.df[col_names].values, (len(self.df / 2), -1, 2))
+                three_point_arr = np.reshape(self.df[col_names].values, (len(self.df / 2), -1, 2)).astype(np.float32)
                 self.results[f'{animal} three-point convex hull perimeter (mm) {point[0]}-{point[1]}-{point[2]}'] = jitted_hull(points=three_point_arr, target=Formats.PERIMETER.value) / self.pixel_per_mm
 
     def calc_four_point_hulls(self):
         for animal, points in self.within_animal_four_point_combs.items():
             for point in points:
                 col_names = list(sum([(x + '_x', y + '_y') for (x, y) in zip(point, point)], ()))
-                four_point_arr = np.reshape(self.df[col_names].values, (len(self.df / 2), -1, 2))
+                four_point_arr = np.reshape(self.df[col_names].values, (len(self.df / 2), -1, 2)).astype(np.float32)
                 self.results[f'{animal} four-point convex perimeter (mm) {point[0]}-{point[1]}-{point[2]}-{point[3]}'] = jitted_hull(points=four_point_arr, target=Formats.PERIMETER.value) / self.pixel_per_mm
 
     def animal_convex_hulls(self):
         for animal, point in self.animal_bps.items():
             col_names = list(sum([(x + '_x', y + '_y') for (x, y) in zip(point, point)], ()))
-            animal_point_arr = np.reshape(self.df[col_names].values, (len(self.df / 2), -1, 2))
+            animal_point_arr = np.reshape(self.df[col_names].values, (len(self.df / 2), -1, 2)).astype(np.float32)
             self.results[f'{animal} convex hull perimeter (mm)'] = jitted_hull(points=animal_point_arr, target=Formats.PERIMETER.value) / self.pixel_per_mm
 
     def calc_movements(self):
         for animal, animal_bps in self.animal_bps.items():
             for bp in animal_bps:
                 bp_df = self.df[[f'{bp}_x', f'{bp}_y']]
                 shift = bp_df.shift(periods=1).add_suffix('_shift')
@@ -118,15 +118,15 @@
                                                                                        bp_df[f'{bp}_y_shift'].values,
                                                                                        bp_df[f'{bp}_y'].values,
                                                                                        self.pixel_per_mm)
 
     def calc_animal_convex_hulls_area(self):
         for animal, point in self.animal_bps.items():
             col_names = list(sum([(x + '_x', y + '_y') for (x, y) in zip(point, point)], ()))
-            animal_point_arr = np.reshape(self.df[col_names].values, (len(self.df / 2), -1, 2))
+            animal_point_arr = np.reshape(self.df[col_names].values, (len(self.df / 2), -1, 2)).astype(np.float32)
             self.results[f'{animal} convex hull area (mm2)'] = jitted_hull(points=animal_point_arr, target=Formats.AREA.value) / self.pixel_per_mm
 
     def calc_roi_center_distances(self):
         self.read_roi_data()
         for animal, animal_bps in self.animal_bps.items():
             for bp in animal_bps:
                 bp_arr = self.df[[f'{bp}_x', f'{bp}_y']].values.astype(float)
```

### Comparing `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi` & `Simba-UW-tf-dev-1.58.1/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc` & `Simba-UW-tf-dev-1.58.1/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc` & `Simba-UW-tf-dev-1.58.1/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc` & `Simba-UW-tf-dev-1.58.1/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc` & `Simba-UW-tf-dev-1.58.1/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi` & `Simba-UW-tf-dev-1.58.1/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi` & `Simba-UW-tf-dev-1.58.1/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/feature_extractor_user_defined.py` & `Simba-UW-tf-dev-1.58.1/simba/feature_extractors/feature_extractor_user_defined.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/feature_extractor_16bp.py` & `Simba-UW-tf-dev-1.58.1/simba/feature_extractors/feature_extractor_16bp.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,17 +63,17 @@
             video_settings, self.px_per_mm, fps = self.read_video_info(video_name=self.video_name)
             for window in self.roll_windows_values:
                 roll_windows.append(int(fps / window))
             self.in_data = read_df(file_path, self.file_type).fillna(0).apply(pd.to_numeric).reset_index(drop=True)
             print('Processing {} ({} frames)...'.format(self.video_name, str(len(self.in_data))))
             self.in_data = self.insert_default_headers_for_feature_extraction(df=self.in_data, headers=self.in_headers, pose_config='16 body-parts', filename=file_path)
             self.out_data = deepcopy(self.in_data)
-            mouse_1_ar = np.reshape(self.out_data[self.mouse_1_headers].values, (len(self.out_data / 2), -1, 2))
+            mouse_1_ar = np.reshape(self.out_data[self.mouse_1_headers].values, (len(self.out_data / 2), -1, 2)).astype(np.float32)
             self.out_data['Mouse_1_poly_area'] = jitted_hull(points=mouse_1_ar, target=Formats.PERIMETER.value) / self.px_per_mm
-            mouse_2_ar = np.reshape(self.out_data[self.mouse_2_headers].values, (len(self.out_data / 2), -1, 2))
+            mouse_2_ar = np.reshape(self.out_data[self.mouse_2_headers].values, (len(self.out_data / 2), -1, 2)).astype(np.float32)
             self.out_data['Mouse_2_poly_area'] = jitted_hull(points=mouse_2_ar, target=Formats.PERIMETER.value) / self.px_per_mm
             self.in_data_shifted = self.out_data.shift(periods=1).add_suffix('_shifted').fillna(0)
             self.in_data = pd.concat([self.in_data, self.in_data_shifted], axis=1, join='inner').fillna(0).reset_index(drop=True)
             self.out_data['Mouse_1_nose_to_tail'] = self.euclidean_distance(self.out_data['Nose_1_x'].values, self.out_data['Tail_base_1_x'].values, self.out_data['Nose_1_y'].values, self.out_data['Tail_base_1_y'].values, self.px_per_mm)
             self.out_data['Mouse_2_nose_to_tail'] = self.euclidean_distance(self.out_data['Nose_2_x'].values, self.out_data['Tail_base_2_x'].values, self.out_data['Nose_2_y'].values, self.out_data['Tail_base_2_y'].values, self.px_per_mm)
             self.out_data['Mouse_1_width'] = self.euclidean_distance(self.out_data['Lat_left_1_x'].values, self.out_data['Lat_right_1_x'].values, self.out_data['Lat_left_1_y'].values, self.out_data['Lat_right_1_y'].values, self.px_per_mm)
             self.out_data['Mouse_2_width'] = self.euclidean_distance(self.out_data['Lat_left_2_x'].values, self.out_data['Lat_right_2_x'].values, self.out_data['Lat_left_2_y'].values, self.out_data['Lat_right_2_y'].values, self.px_per_mm)
```

### Comparing `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/feature_extractor_9bp.py` & `Simba-UW-tf-dev-1.58.1/simba/feature_extractors/feature_extractor_9bp.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
                 roll_windows.append(int(fps / window))
             self.roll_windows_values = [int(x) for x in self.roll_windows_values]
             self.in_data = read_df(file_path, self.file_type).fillna(0).apply(pd.to_numeric).reset_index(drop=True)
             self.in_data = self.insert_default_headers_for_feature_extraction(df=self.in_data, headers=self.in_headers, pose_config='1 animal 9 body-parts', filename=file_path)
             self.out_data = deepcopy(self.in_data)
             self.in_data_shifted = self.out_data.shift(periods=1).add_suffix('_shifted').fillna(0)
             self.in_data = pd.concat([self.in_data, self.in_data_shifted], axis=1, join='inner').fillna(0).reset_index(drop=True)
-            mouse_arr = np.reshape(self.out_data[self.mouse_headers].values, (len(self.out_data / 2), -1, 2))
+            mouse_arr = np.reshape(self.out_data[self.mouse_headers].values, (len(self.out_data / 2), -1, 2)).astype(np.float32)
             print('Calculating hull features...')
             self.out_data['Mouse_poly_area'] = jitted_hull(points=mouse_arr, target='perimeter') / self.px_per_mm
 
             print('Calculating Euclidean distances... ')
             self.out_data['Nose_to_tail'] = self.euclidean_distance(self.in_data['Mouse1_nose_x'].values, self.in_data['Mouse1_tail_x'].values, self.in_data['Mouse1_nose_y'].values, self.in_data['Mouse1_tail_y'].values, self.px_per_mm)
             self.out_data['Distance_feet'] = self.euclidean_distance(self.in_data['Mouse1_left_foot_x'].values, self.in_data['Mouse1_right_foot_x'].values, self.in_data['Mouse1_left_foot_y'].values, self.in_data['Mouse1_right_foot_y'].values, self.px_per_mm)
             self.out_data['Distance_hands'] = self.euclidean_distance(self.in_data['Mouse1_left_hand_x'].values, self.in_data['Mouse1_right_hand_x'].values, self.in_data['Mouse1_left_hand_y'].values, self.in_data['Mouse1_right_hand_y'].values, self.px_per_mm)
@@ -275,10 +275,10 @@
 
             video_timer.stop_timer()
 
             print(f'Feature extraction complete for {self.video_name} ({(file_cnt + 1)}/{len(self.files_found)} (elapsed time: {video_timer.elapsed_time_str}s)...')
 
         self.timer.stop_timer()
         stdout_success(msg='All features extracted. Results stored in project_folder/csv/features_extracted directory', elapsed_time=self.timer.elapsed_time_str)
-
+#
 # test = ExtractFeaturesFrom9bps(config_path='/Users/simon/Desktop/envs/troubleshooting/Emergence/project_folder/project_config.ini')
 # test.run()
```

### Comparing `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/feature_extractor_8bp.py` & `Simba-UW-tf-dev-1.58.1/simba/feature_extractors/feature_extractor_8bp.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
             roll_windows = []
             for window in self.roll_windows_values:
                 roll_windows.append(int(fps / window))
             self.in_data = read_df(file_path, self.file_type).fillna(0).apply(pd.to_numeric).reset_index(drop=True)
             print('Processing {} ({} frames)...'.format(self.video_name, str(len(self.in_data))))
             self.in_data = self.insert_default_headers_for_feature_extraction(df=self.in_data, headers=self.in_headers, pose_config='8 body-parts', filename=file_path)
             self.out_data = deepcopy(self.in_data)
-            mouse_1_ar = np.reshape(self.out_data[self.mouse_headers].values, (len(self.out_data / 2), -1, 2))
+            mouse_1_ar = np.reshape(self.out_data[self.mouse_headers].values, (len(self.out_data / 2), -1, 2)).astype(np.float32)
             self.out_data['Mouse_poly_area'] = jitted_hull(points=mouse_1_ar, target=Formats.PERIMETER.value) / self.px_per_mm
             self.in_data_shifted = self.out_data.shift(periods=1).add_suffix('_shifted').fillna(0)
             self.in_data = pd.concat([self.in_data, self.in_data_shifted], axis=1, join='inner').fillna(0).reset_index(drop=True)
             self.out_data['Mouse_nose_to_tail'] = self.euclidean_distance(self.in_data['Nose_x'].values, self.in_data['Tail_base_x'].values, self.in_data['Nose_y'].values, self.in_data['Tail_base_y'].values, self.px_per_mm)
             self.out_data['Mouse_width'] = self.euclidean_distance(self.in_data['Lat_left_x'].values, self.in_data['Lat_right_x'].values, self.in_data['Lat_left_y'].values, self.in_data['Lat_right_y'].values, self.px_per_mm)
             self.out_data['Mouse_Ear_distance'] = self.euclidean_distance(self.in_data['Ear_left_x'].values, self.in_data['Ear_right_x'].values, self.in_data['Ear_left_y'].values, self.in_data['Ear_right_y'].values, self.px_per_mm)
             self.out_data['Mouse_Nose_to_centroid'] = self.euclidean_distance(self.in_data['Nose_x'].values, self.in_data['Center_x'].values, self.in_data['Nose_y'].values, self.in_data['Center_y'].values, self.px_per_mm)
```

### Comparing `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/feature_extractor_4bp.py` & `Simba-UW-tf-dev-1.58.1/simba/feature_extractors/feature_extractor_4bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/.idea/features_scripts.iml` & `Simba-UW-tf-dev-1.58.1/simba/feature_extractors/.idea/features_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.58.1/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/.idea/workspace.xml` & `Simba-UW-tf-dev-1.58.1/simba/feature_extractors/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/requirements.txt` & `Simba-UW-tf-dev-1.58.1/simba/requirements.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/severity_processor.py` & `Simba-UW-tf-dev-1.58.1/simba/severity_processor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/user_pose_config_creator.py` & `Simba-UW-tf-dev-1.58.1/simba/user_pose_config_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/mixins/.DS_Store` & `Simba-UW-tf-dev-1.58.1/simba/mixins/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/mixins/pop_up_mixin.py` & `Simba-UW-tf-dev-1.58.1/simba/mixins/pop_up_mixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,14 +39,22 @@
 
 class PopUpMixin(object):
     def __init__(self,
                  title: str,
                  config_path: str or None=None,
                  size: tuple=(400,400)):
 
+        """
+        Methods for pop-up windows in SimBa.
+
+        :param str title: Pop-up window title
+        :param configparser.Configparser config_path: path to SimBA project_config.ini
+        :param tuple size: HxW of the po-up window.
+        """
+
         self.main_frm = Toplevel()
         self.main_frm.minsize(size[0], size[1])
         self.main_frm.wm_title(title)
         self.main_frm.lift()
         self.main_frm = Canvas(hxtScrollbar(self.main_frm))
         self.main_frm.pack(fill="both", expand=True)
```

### Comparing `Simba-UW-tf-dev-1.57.9/simba/mixins/config_reader.py` & `Simba-UW-tf-dev-1.58.1/simba/mixins/config_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,21 @@
 
 
 class ConfigReader(object):
     def __init__(self,
                  config_path: str,
                  read_video_info: bool=True):
 
+        """
+        Methods for reading SimBA configparser.Configparser project config..
+
+        :param configparser.Configparser config_path: path to SimBA project_config.ini
+        :param bool read_video_info: if true, read the project_folder/logs/video_info.csv file.
+        """
+
         self.timer = SimbaTimer(start=True)
         self.config_path = config_path
         self.config = read_config_file(config_path=config_path)
         self.datetime = datetime.now().strftime('%Y%m%d%H%M%S')
         self.project_path, self.file_type = read_project_path_and_file_type(config=self.config)
         self.input_csv_dir = os.path.join(self.project_path, Paths.INPUT_CSV.value)
         self.features_dir = os.path.join(self.project_path, Paths.FEATURES_EXTRACTED_DIR.value)
```

### Comparing `Simba-UW-tf-dev-1.57.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.nbi` & `Simba-UW-tf-dev-1.58.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.1.nbc` & `Simba-UW-tf-dev-1.58.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.nbi` & `Simba-UW-tf-dev-1.58.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.1.nbc` & `Simba-UW-tf-dev-1.58.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.1.nbc` & `Simba-UW-tf-dev-1.58.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.nbi` & `Simba-UW-tf-dev-1.58.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/mixins/feature_extraction_mixin.py` & `Simba-UW-tf-dev-1.58.1/simba/mixins/feature_extraction_mixin.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,19 @@
 import simba
 
 class FeatureExtractionMixin(object):
 
     def __init__(self,
                  config_path: str or None=None):
 
+        """
+        Methods for featurizing pose-estimation data
+        :param configparser.Configparser config_path: path to SimBA project_config.ini
+        """
+
         if config_path:
             self.config_path = config_path
             self.config = read_config_file(config_path=config_path)
             self.project_path, self.file_type = read_project_path_and_file_type(config=self.config)
             self.video_info_path = os.path.join(self.project_path, Paths.VIDEO_INFO.value)
             self.video_info_df = read_video_info_csv(file_path=self.video_info_path)
             self.data_in_dir = os.path.join(self.project_path, Paths.OUTLIER_CORRECTED.value)
@@ -146,15 +151,15 @@
         return results
 
     def windowed_frequentist_distribution_tests(self,
                                                 data: np.array,
                                                 feature_name: str,
                                                 fps: int):
         """
-        Helper to compare feature value distributions in 1s sequential time-bins: Kolmogorov-Smirnov and T-tests
+        Helper to compare feature value distributions in 1-s sequential time-bins: Kolmogorov-Smirnov and T-tests
         Compares the feature values against a normal distribution: Shapiro.
         Find the number of peaks in *rolling* 1s long feature window.
         """
 
         ks_results, = np.full((data.shape[0]), -1.0),
         t_test_results = np.full((data.shape[0]), -1.0)
         shapiro_results = np.full((data.shape[0]), -1.0)
```

### Comparing `Simba-UW-tf-dev-1.57.9/simba/mixins/plotting_mixin.py` & `Simba-UW-tf-dev-1.58.1/simba/mixins/plotting_mixin.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,14 +19,19 @@
 from simba.utils.lookups import get_color_dict, get_named_colors
 from simba.utils.read_write import get_fn_ext
 from simba.utils.printing import stdout_success, SimbaTimer
 from simba.enums import Formats
 
 class PlottingMixin(object):
     def __init__(self):
+
+        """
+        Methods for plotting
+        """
+
         pass
 
     def create_gantt_img(self,
                          bouts_df: pd.DataFrame,
                          clf_name: str,
                          image_index: int,
                          fps: int,
```

### Comparing `Simba-UW-tf-dev-1.57.9/simba/mixins/unsupervised_mixin.py` & `Simba-UW-tf-dev-1.58.1/simba/mixins/unsupervised_mixin.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,18 @@
 from simba.utils.checks import check_float
 from simba.utils.printing import SimbaTimer
 
 
 class UnsupervisedMixin(object):
     def __init__(self):
 
+        """
+        Methods for unsupervised ML.
+        """
+
         self.datetime = datetime.now().strftime('%Y%m%d%H%M%S')
         self.timer = SimbaTimer(start=True)
         model_names_dir = os.path.join(os.path.dirname(simba.__file__), Paths.UNSUPERVISED_MODEL_NAMES.value)
         self.model_names = list(pd.read_parquet(model_names_dir)[Unsupervised.NAMES.value])
 
     def read_pickle(self,
                     data_path: str) -> dict:
```

### Comparing `Simba-UW-tf-dev-1.57.9/simba/mixins/train_model_mixin.py` & `Simba-UW-tf-dev-1.58.1/simba/mixins/train_model_mixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,17 @@
 
 
 plt.switch_backend('agg')
 
 class TrainModelMixin(object):
     def __init__(self):
         pass
+    """
+    Methods for training and evaluating classifiers.
+    """
 
     def read_all_files_in_folder(self,
                                  file_paths: list,
                                  file_type: str,
                                  classifier_names=None):
         """
         Helper function to read in all data files in a folder to a single pd.DataFrame for downstream ML algorithm.
```

### Comparing `Simba-UW-tf-dev-1.57.9/simba/machine_model_settings_pop_up.py` & `Simba-UW-tf-dev-1.58.1/simba/machine_model_settings_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/remove_keypoints_in_pose.py` & `Simba-UW-tf-dev-1.58.1/simba/remove_keypoints_in_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/third_party_label_appenders/deepethogram_importer.py` & `Simba-UW-tf-dev-1.58.1/simba/third_party_label_appenders/deepethogram_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/third_party_label_appenders/BORIS_appender.py` & `Simba-UW-tf-dev-1.58.1/simba/third_party_label_appenders/BORIS_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/third_party_label_appenders/observer_importer.py` & `Simba-UW-tf-dev-1.58.1/simba/third_party_label_appenders/observer_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/third_party_label_appenders/tools.py` & `Simba-UW-tf-dev-1.58.1/simba/third_party_label_appenders/tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/third_party_label_appenders/third_party_appender.py` & `Simba-UW-tf-dev-1.58.1/simba/third_party_label_appenders/third_party_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/third_party_label_appenders/ethovision_import.py` & `Simba-UW-tf-dev-1.58.1/simba/third_party_label_appenders/ethovision_import.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/third_party_label_appenders/BENTO_appender.py` & `Simba-UW-tf-dev-1.58.1/simba/third_party_label_appenders/BENTO_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/third_party_label_appenders/solomon_importer.py` & `Simba-UW-tf-dev-1.58.1/simba/third_party_label_appenders/solomon_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/multi_cropper.py` & `Simba-UW-tf-dev-1.58.1/simba/multi_cropper.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/FSTTC_calculator.py` & `Simba-UW-tf-dev-1.58.1/simba/FSTTC_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/create_project_pop_up.py` & `Simba-UW-tf-dev-1.58.1/simba/create_project_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/video_info_table.py` & `Simba-UW-tf-dev-1.58.1/simba/video_info_table.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/cue_light_tools/.DS_Store` & `Simba-UW-tf-dev-1.58.1/simba/cue_light_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/cue_light_tools/cue_light_clf_statistics.py` & `Simba-UW-tf-dev-1.58.1/simba/cue_light_tools/cue_light_clf_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/cue_light_tools/cue_light_analyzer.py` & `Simba-UW-tf-dev-1.58.1/simba/cue_light_tools/cue_light_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/cue_light_tools/cue_light_menues.py` & `Simba-UW-tf-dev-1.58.1/simba/cue_light_tools/cue_light_menues.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/cue_light_tools/cue_light_tools.py` & `Simba-UW-tf-dev-1.58.1/simba/cue_light_tools/cue_light_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/cue_light_tools/cue_light_visualizer.py` & `Simba-UW-tf-dev-1.58.1/simba/cue_light_tools/cue_light_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/cue_light_tools/cue_light_movement_statistics.py` & `Simba-UW-tf-dev-1.58.1/simba/cue_light_tools/cue_light_movement_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/extract_frames_fast.py` & `Simba-UW-tf-dev-1.58.1/simba/extract_frames_fast.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/utils/.DS_Store` & `Simba-UW-tf-dev-1.58.1/simba/utils/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/utils/warnings.py` & `Simba-UW-tf-dev-1.58.1/simba/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/utils/checks.py` & `Simba-UW-tf-dev-1.58.1/simba/utils/checks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/utils/read_write.py` & `Simba-UW-tf-dev-1.58.1/simba/utils/read_write.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/utils/lookups.py` & `Simba-UW-tf-dev-1.58.1/simba/utils/lookups.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/utils/errors.py` & `Simba-UW-tf-dev-1.58.1/simba/utils/errors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/utils/data.py` & `Simba-UW-tf-dev-1.58.1/simba/utils/data.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/utils/printing.py` & `Simba-UW-tf-dev-1.58.1/simba/utils/printing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/labelling_interface.py` & `Simba-UW-tf-dev-1.58.1/simba/labelling_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/timebins_movement_analyzer.py` & `Simba-UW-tf-dev-1.58.1/simba/timebins_movement_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/SimBA_dash_app.py` & `Simba-UW-tf-dev-1.58.1/simba/SimBA_dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/timebins_clf_analyzer.py` & `Simba-UW-tf-dev-1.58.1/simba/timebins_clf_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/calculate_px_dist.py` & `Simba-UW-tf-dev-1.58.1/simba/calculate_px_dist.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/movement_processor.py` & `Simba-UW-tf-dev-1.58.1/simba/movement_processor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/pybursts.py` & `Simba-UW-tf-dev-1.58.1/simba/pybursts.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/reverse_2_animal_tracking.py` & `Simba-UW-tf-dev-1.58.1/simba/reverse_2_animal_tracking.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/Directing_animals_analyzer.py` & `Simba-UW-tf-dev-1.58.1/simba/Directing_animals_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/Validate_model_one_video_run_clf.py` & `Simba-UW-tf-dev-1.58.1/simba/Validate_model_one_video_run_clf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/tkinter_functions.py` & `Simba-UW-tf-dev-1.58.1/simba/tkinter_functions.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/setting_menu.py` & `Simba-UW-tf-dev-1.58.1/simba/setting_menu.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/interpolate_pose.py` & `Simba-UW-tf-dev-1.58.1/simba/interpolate_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/run_inference.py` & `Simba-UW-tf-dev-1.58.1/simba/run_inference.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/plotting/gantt_creator.py` & `Simba-UW-tf-dev-1.58.1/simba/plotting/gantt_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/plotting/tools/tkinter_tools.py` & `Simba-UW-tf-dev-1.58.1/simba/plotting/tools/tkinter_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/plotting/ROI_plotter_mp.py` & `Simba-UW-tf-dev-1.58.1/simba/plotting/ROI_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/plotting/.DS_Store` & `Simba-UW-tf-dev-1.58.1/simba/plotting/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/plotting/shap_agg_stats_visualizer.py` & `Simba-UW-tf-dev-1.58.1/simba/plotting/shap_agg_stats_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/plotting/gantt_creator_mp.py` & `Simba-UW-tf-dev-1.58.1/simba/plotting/gantt_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/plotting/heat_mapper_clf_mp.py` & `Simba-UW-tf-dev-1.58.1/simba/plotting/heat_mapper_clf_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/plotting/probability_plot_creator.py` & `Simba-UW-tf-dev-1.58.1/simba/plotting/probability_plot_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/plotting/plot_clf_results.py` & `Simba-UW-tf-dev-1.58.1/simba/plotting/plot_clf_results.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/plotting/plot_clf_results_mp.py` & `Simba-UW-tf-dev-1.58.1/simba/plotting/plot_clf_results_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/plotting/ROI_feature_visualizer.py` & `Simba-UW-tf-dev-1.58.1/simba/plotting/ROI_feature_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/plotting/heat_mapper_location.py` & `Simba-UW-tf-dev-1.58.1/simba/plotting/heat_mapper_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/plotting/probability_plot_creator_mp.py` & `Simba-UW-tf-dev-1.58.1/simba/plotting/probability_plot_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/plotting/interactive_probability_grapher.py` & `Simba-UW-tf-dev-1.58.1/simba/plotting/interactive_probability_grapher.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/plotting/plot_pose_in_dir.py` & `Simba-UW-tf-dev-1.58.1/simba/plotting/plot_pose_in_dir.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/plotting/single_run_model_validation_video.py` & `Simba-UW-tf-dev-1.58.1/simba/plotting/single_run_model_validation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/plotting/frame_mergerer_ffmpeg.py` & `Simba-UW-tf-dev-1.58.1/simba/plotting/frame_mergerer_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/plotting/Directing_animals_visualizer_mp.py` & `Simba-UW-tf-dev-1.58.1/simba/plotting/Directing_animals_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/plotting/clf_validator.py` & `Simba-UW-tf-dev-1.58.1/simba/plotting/clf_validator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/plotting/path_plotter_mp.py` & `Simba-UW-tf-dev-1.58.1/simba/plotting/path_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/plotting/ROI_feature_visualizer_mp.py` & `Simba-UW-tf-dev-1.58.1/simba/plotting/ROI_feature_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/plotting/data_plotter.py` & `Simba-UW-tf-dev-1.58.1/simba/plotting/data_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/plotting/path_plotter.py` & `Simba-UW-tf-dev-1.58.1/simba/plotting/path_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/plotting/ez_lineplot.py` & `Simba-UW-tf-dev-1.58.1/simba/plotting/ez_lineplot.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/plotting/distance_plotter_mp.py` & `Simba-UW-tf-dev-1.58.1/simba/plotting/distance_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/plotting/ROI_plotter.py` & `Simba-UW-tf-dev-1.58.1/simba/plotting/ROI_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/plotting/heat_mapper_clf.py` & `Simba-UW-tf-dev-1.58.1/simba/plotting/heat_mapper_clf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/plotting/distance_plotter.py` & `Simba-UW-tf-dev-1.58.1/simba/plotting/distance_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/plotting/single_run_model_validation_video_mp.py` & `Simba-UW-tf-dev-1.58.1/simba/plotting/single_run_model_validation_video_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/plotting/Directing_animals_visualizer.py` & `Simba-UW-tf-dev-1.58.1/simba/plotting/Directing_animals_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/plotting/heat_mapper_location_mp.py` & `Simba-UW-tf-dev-1.58.1/simba/plotting/heat_mapper_location_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/run_dash_tkinter.py` & `Simba-UW-tf-dev-1.58.1/simba/run_dash_tkinter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/dash_app.py` & `Simba-UW-tf-dev-1.58.1/simba/dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/extract_annotation_frames.py` & `Simba-UW-tf-dev-1.58.1/simba/extract_annotation_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/roi_tools/ROI_time_bin_calculator.py` & `Simba-UW-tf-dev-1.58.1/simba/roi_tools/ROI_time_bin_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/roi_tools/ROI_movement_analyzer.py` & `Simba-UW-tf-dev-1.58.1/simba/roi_tools/ROI_movement_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/roi_tools/.DS_Store` & `Simba-UW-tf-dev-1.58.1/simba/roi_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/roi_tools/ROI_define.py` & `Simba-UW-tf-dev-1.58.1/simba/roi_tools/ROI_define.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/roi_tools/ROI_reset.py` & `Simba-UW-tf-dev-1.58.1/simba/roi_tools/ROI_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/roi_tools/ROI_analyzer.py` & `Simba-UW-tf-dev-1.58.1/simba/roi_tools/ROI_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/roi_tools/ROI_feature_analyzer.py` & `Simba-UW-tf-dev-1.58.1/simba/roi_tools/ROI_feature_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/roi_tools/ROI_multiply.py` & `Simba-UW-tf-dev-1.58.1/simba/roi_tools/ROI_multiply.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/roi_tools/ROI_size_calculations.py` & `Simba-UW-tf-dev-1.58.1/simba/roi_tools/ROI_size_calculations.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/roi_tools/ROI_zoom.py` & `Simba-UW-tf-dev-1.58.1/simba/roi_tools/ROI_zoom.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/roi_tools/ROI_directing_analyzer.py` & `Simba-UW-tf-dev-1.58.1/simba/roi_tools/ROI_directing_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/roi_tools/ROI_move_shape.py` & `Simba-UW-tf-dev-1.58.1/simba/roi_tools/ROI_move_shape.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/roi_tools/ROI_menus.py` & `Simba-UW-tf-dev-1.58.1/simba/roi_tools/ROI_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/roi_tools/ROI_clf_calculator.py` & `Simba-UW-tf-dev-1.58.1/simba/roi_tools/ROI_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/roi_tools/ROI_image.py` & `Simba-UW-tf-dev-1.58.1/simba/roi_tools/ROI_image.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/pose_importers/read_DANNCE_mat.py` & `Simba-UW-tf-dev-1.58.1/simba/pose_importers/read_DANNCE_mat.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/pose_importers/sleap_importer_slp.py` & `Simba-UW-tf-dev-1.58.1/simba/pose_importers/sleap_importer_slp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/pose_importers/sleap_importer_h5.py` & `Simba-UW-tf-dev-1.58.1/simba/pose_importers/sleap_importer_h5.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/pose_importers/dlc_multi_animal_importer.py` & `Simba-UW-tf-dev-1.58.1/simba/pose_importers/dlc_multi_animal_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/pose_importers/.DS_Store` & `Simba-UW-tf-dev-1.58.1/simba/pose_importers/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/pose_importers/sleap_importer_csv.py` & `Simba-UW-tf-dev-1.58.1/simba/pose_importers/sleap_importer_csv.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/pose_importers/import_mars.py` & `Simba-UW-tf-dev-1.58.1/simba/pose_importers/import_mars.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/pose_importers/dlc_importer_csv.py` & `Simba-UW-tf-dev-1.58.1/simba/pose_importers/dlc_importer_csv.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/pose_importers/trk_importer.py` & `Simba-UW-tf-dev-1.58.1/simba/pose_importers/trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/pop_up_classes.py` & `Simba-UW-tf-dev-1.58.1/simba/pop_up_classes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/extract_seqframes.py` & `Simba-UW-tf-dev-1.58.1/simba/extract_seqframes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/pose_configurations/.DS_Store` & `Simba-UW-tf-dev-1.58.1/simba/pose_configurations/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/pose_configurations/bp_names/.DS_Store` & `Simba-UW-tf-dev-1.58.1/simba/pose_configurations/bp_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/pose_configurations/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.58.1/simba/pose_configurations/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/pose_configurations/no_animals/.DS_Store` & `Simba-UW-tf-dev-1.58.1/simba/pose_configurations/no_animals/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/pose_configurations/configuration_names/.DS_Store` & `Simba-UW-tf-dev-1.58.1/simba/pose_configurations/configuration_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/pose_configurations/schematics/.DS_Store` & `Simba-UW-tf-dev-1.58.1/simba/pose_configurations/schematics/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/pose_configurations/schematics/8.png` & `Simba-UW-tf-dev-1.58.1/simba/pose_configurations/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/pose_configurations/schematics/9.png` & `Simba-UW-tf-dev-1.58.1/simba/pose_configurations/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/pose_configurations/schematics/12.png` & `Simba-UW-tf-dev-1.58.1/simba/pose_configurations/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/pose_configurations/schematics/11.png` & `Simba-UW-tf-dev-1.58.1/simba/pose_configurations/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/pose_configurations/schematics/10.png` & `Simba-UW-tf-dev-1.58.1/simba/pose_configurations/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/pose_configurations/schematics/4.png` & `Simba-UW-tf-dev-1.58.1/simba/pose_configurations/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/pose_configurations/schematics/5.png` & `Simba-UW-tf-dev-1.58.1/simba/pose_configurations/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/pose_configurations/schematics/7.png` & `Simba-UW-tf-dev-1.58.1/simba/pose_configurations/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/pose_configurations/schematics/6.png` & `Simba-UW-tf-dev-1.58.1/simba/pose_configurations/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/pose_configurations/schematics/2.png` & `Simba-UW-tf-dev-1.58.1/simba/pose_configurations/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/pose_configurations/schematics/3.png` & `Simba-UW-tf-dev-1.58.1/simba/pose_configurations/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/pose_configurations/schematics/1.png` & `Simba-UW-tf-dev-1.58.1/simba/pose_configurations/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/get_coordinates_tools_v2.py` & `Simba-UW-tf-dev-1.58.1/simba/get_coordinates_tools_v2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/pup_retrieval_protocol.py` & `Simba-UW-tf-dev-1.58.1/simba/pup_retrieval_protocol.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/outlier_tools/outlier_corrector_movement.py` & `Simba-UW-tf-dev-1.58.1/simba/outlier_tools/outlier_corrector_movement.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/outlier_tools/.DS_Store` & `Simba-UW-tf-dev-1.58.1/simba/outlier_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/outlier_tools/outlier_corrector_location.py` & `Simba-UW-tf-dev-1.58.1/simba/outlier_tools/outlier_corrector_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/outlier_tools/skip_outlier_correction.py` & `Simba-UW-tf-dev-1.58.1/simba/outlier_tools/skip_outlier_correction.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/outlier_tools/.idea/outlier_scripts.iml` & `Simba-UW-tf-dev-1.58.1/simba/outlier_tools/.idea/outlier_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.58.1/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/outlier_tools/.idea/workspace.xml` & `Simba-UW-tf-dev-1.58.1/simba/outlier_tools/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/pose_reset.py` & `Simba-UW-tf-dev-1.58.1/simba/pose_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/train_mutiple_models.py` & `Simba-UW-tf-dev-1.58.1/simba/train_mutiple_models.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/SimBA.py` & `Simba-UW-tf-dev-1.58.1/simba/SimBA.py`

 * *Files 0% similar despite different names*

```diff
@@ -683,15 +683,15 @@
     def run_feature_extraction(self):
         print(f'Pose-estimation body part setting for feature extraction: {str(self.animal_cnt)} animals {str(self.pose_setting)} body-parts')
         feature_extractor_classes = get_bp_config_code_class_pairs()
         if self.user_defined_var.get():
             _ = run_user_defined_feature_extraction_class(file_path=self.scriptfile.file_path,
                                                           config_path=self.config_path)
         else:
-            if (self.pose_setting == '8'):
+            if self.pose_setting == '8':
                 feature_extractor = feature_extractor_classes[self.pose_setting][self.animal_cnt](config_path=self.config_path)
             else:
                 feature_extractor = feature_extractor_classes[self.pose_setting](config_path=self.config_path)
             feature_extractor.run()
 
     def set_distance_mm(self):
         check_int(name='DISTANCE IN MILLIMETER', value=self.distance_in_mm_eb.entry_get, min_value=1)
```

### Comparing `Simba-UW-tf-dev-1.57.9/simba/labelling_advanced_interface.py` & `Simba-UW-tf-dev-1.58.1/simba/labelling_advanced_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.58.1/simba/assets/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/unsupervised/model_names.parquet` & `Simba-UW-tf-dev-1.58.1/simba/assets/unsupervised/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/unsupervised/features.csv` & `Simba-UW-tf-dev-1.58.1/simba/assets/unsupervised/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/shap/down_arrow.jpg` & `Simba-UW-tf-dev-1.58.1/simba/assets/shap/down_arrow.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/shap/intruder_shape.jpg` & `Simba-UW-tf-dev-1.58.1/simba/assets/shap/intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/shap/feature_categories/shap_feature_categories.csv` & `Simba-UW-tf-dev-1.58.1/simba/assets/shap/feature_categories/shap_feature_categories.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/shap/.DS_Store` & `Simba-UW-tf-dev-1.58.1/simba/assets/shap/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/shap/resident_shape.jpg` & `Simba-UW-tf-dev-1.58.1/simba/assets/shap/resident_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/shap/resident_intruder_shape.jpg` & `Simba-UW-tf-dev-1.58.1/simba/assets/shap/resident_intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/shap/animal_distances.jpg` & `Simba-UW-tf-dev-1.58.1/simba/assets/shap/animal_distances.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/shap/baseline_scale.jpg` & `Simba-UW-tf-dev-1.58.1/simba/assets/shap/baseline_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/shap/ubuntu.regular.ttf` & `Simba-UW-tf-dev-1.58.1/simba/assets/shap/ubuntu.regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/shap/side_scale.jpg` & `Simba-UW-tf-dev-1.58.1/simba/assets/shap/side_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/shap/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.58.1/simba/assets/shap/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/shap/side_scale_5.jpg` & `Simba-UW-tf-dev-1.58.1/simba/assets/shap/side_scale_5.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/shap/intruder_movement.jpg` & `Simba-UW-tf-dev-1.58.1/simba/assets/shap/intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/shap/resident_movement.jpg` & `Simba-UW-tf-dev-1.58.1/simba/assets/shap/resident_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/shap/color_bar.jpg` & `Simba-UW-tf-dev-1.58.1/simba/assets/shap/color_bar.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/shap/resident_intruder_movement.jpg` & `Simba-UW-tf-dev-1.58.1/simba/assets/shap/resident_intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/.DS_Store` & `Simba-UW-tf-dev-1.58.1/simba/assets/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/lookups/.DS_Store` & `Simba-UW-tf-dev-1.58.1/simba/assets/lookups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/lookups/model_names.parquet` & `Simba-UW-tf-dev-1.58.1/simba/assets/lookups/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/lookups/feature_extraction_headers.csv` & `Simba-UW-tf-dev-1.58.1/simba/assets/lookups/feature_extraction_headers.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/lookups/features.csv` & `Simba-UW-tf-dev-1.58.1/simba/assets/lookups/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/lookups/unsupervised_example_x.csv` & `Simba-UW-tf-dev-1.58.1/simba/assets/lookups/unsupervised_example_x.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/stl/operant_tray.stl` & `Simba-UW-tf-dev-1.58.1/simba/assets/stl/operant_tray.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/stl/operant_lever.stl` & `Simba-UW-tf-dev-1.58.1/simba/assets/stl/operant_lever.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/stl/operant_walls.stl` & `Simba-UW-tf-dev-1.58.1/simba/assets/stl/operant_walls.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/stl/grid_floor.stl` & `Simba-UW-tf-dev-1.58.1/simba/assets/stl/grid_floor.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/img/.DS_Store` & `Simba-UW-tf-dev-1.58.1/simba/assets/img/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/img/about_me.png` & `Simba-UW-tf-dev-1.58.1/simba/assets/img/about_me.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/img/splash.mp4` & `Simba-UW-tf-dev-1.58.1/simba/assets/img/splash.mp4`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/img/bg_2.png` & `Simba-UW-tf-dev-1.58.1/simba/assets/img/bg_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/img/splash.pptx` & `Simba-UW-tf-dev-1.58.1/simba/assets/img/splash.pptx`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/img/bg.png` & `Simba-UW-tf-dev-1.58.1/simba/assets/img/bg.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.58.1/simba/assets/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/icons/factory.png` & `Simba-UW-tf-dev-1.58.1/simba/assets/icons/factory.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/icons/cluster.png` & `Simba-UW-tf-dev-1.58.1/simba/assets/icons/cluster.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/icons/load.png` & `Simba-UW-tf-dev-1.58.1/simba/assets/icons/load.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/icons/gif.png` & `Simba-UW-tf-dev-1.58.1/simba/assets/icons/gif.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/icons/pose.png` & `Simba-UW-tf-dev-1.58.1/simba/assets/icons/pose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/icons/features.png` & `Simba-UW-tf-dev-1.58.1/simba/assets/icons/features.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/icons/.DS_Store` & `Simba-UW-tf-dev-1.58.1/simba/assets/icons/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/icons/settings.png` & `Simba-UW-tf-dev-1.58.1/simba/assets/icons/settings.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/icons/stopwatch.png` & `Simba-UW-tf-dev-1.58.1/simba/assets/icons/stopwatch.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/icons/link.png` & `Simba-UW-tf-dev-1.58.1/simba/assets/icons/link.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/icons/dash_simba.css` & `Simba-UW-tf-dev-1.58.1/simba/assets/icons/dash_simba.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/icons/documentation.png` & `Simba-UW-tf-dev-1.58.1/simba/assets/icons/documentation.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/icons/fps.png` & `Simba-UW-tf-dev-1.58.1/simba/assets/icons/fps.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/icons/dimensionality_reduction.png` & `Simba-UW-tf-dev-1.58.1/simba/assets/icons/dimensionality_reduction.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/icons/roi.png` & `Simba-UW-tf-dev-1.58.1/simba/assets/icons/roi.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/icons/superimpose.png` & `Simba-UW-tf-dev-1.58.1/simba/assets/icons/superimpose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/icons/label.png` & `Simba-UW-tf-dev-1.58.1/simba/assets/icons/label.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/icons/change.png` & `Simba-UW-tf-dev-1.58.1/simba/assets/icons/change.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/icons/crop.png` & `Simba-UW-tf-dev-1.58.1/simba/assets/icons/crop.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/icons/rotate.png` & `Simba-UW-tf-dev-1.58.1/simba/assets/icons/rotate.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/icons/path.png` & `Simba-UW-tf-dev-1.58.1/simba/assets/icons/path.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/icons/clip.png` & `Simba-UW-tf-dev-1.58.1/simba/assets/icons/clip.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/icons/restart.png` & `Simba-UW-tf-dev-1.58.1/simba/assets/icons/restart.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/icons/calipher.png` & `Simba-UW-tf-dev-1.58.1/simba/assets/icons/calipher.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/icons/add_on.png` & `Simba-UW-tf-dev-1.58.1/simba/assets/icons/add_on.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/icons/create.png` & `Simba-UW-tf-dev-1.58.1/simba/assets/icons/create.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/icons/SimBA_logo.ico` & `Simba-UW-tf-dev-1.58.1/simba/assets/icons/SimBA_logo.ico`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/icons/print.png` & `Simba-UW-tf-dev-1.58.1/simba/assets/icons/print.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/icons/clf.png` & `Simba-UW-tf-dev-1.58.1/simba/assets/icons/clf.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/icons/concat_icons/mosaic.png` & `Simba-UW-tf-dev-1.58.1/simba/assets/icons/concat_icons/mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/icons/concat_icons/vertical.png` & `Simba-UW-tf-dev-1.58.1/simba/assets/icons/concat_icons/vertical.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/icons/concat_icons/horizontal.png` & `Simba-UW-tf-dev-1.58.1/simba/assets/icons/concat_icons/horizontal.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/icons/concat_icons/mixed_mosaic.png` & `Simba-UW-tf-dev-1.58.1/simba/assets/icons/concat_icons/mixed_mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/icons/merge.png` & `Simba-UW-tf-dev-1.58.1/simba/assets/icons/merge.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/icons/clean.png` & `Simba-UW-tf-dev-1.58.1/simba/assets/icons/clean.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/icons/clf_2.png` & `Simba-UW-tf-dev-1.58.1/simba/assets/icons/clf_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/icons/visualize.png` & `Simba-UW-tf-dev-1.58.1/simba/assets/icons/visualize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/icons/concat.png` & `Simba-UW-tf-dev-1.58.1/simba/assets/icons/concat.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/icons/boris.png` & `Simba-UW-tf-dev-1.58.1/simba/assets/icons/boris.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/icons/frames.png` & `Simba-UW-tf-dev-1.58.1/simba/assets/icons/frames.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/icons/video.png` & `Simba-UW-tf-dev-1.58.1/simba/assets/icons/video.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/icons/sample.png` & `Simba-UW-tf-dev-1.58.1/simba/assets/icons/sample.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/icons/metrics.png` & `Simba-UW-tf-dev-1.58.1/simba/assets/icons/metrics.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/icons/grey.png` & `Simba-UW-tf-dev-1.58.1/simba/assets/icons/grey.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/icons/exit.png` & `Simba-UW-tf-dev-1.58.1/simba/assets/icons/exit.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/icons/outlier.png` & `Simba-UW-tf-dev-1.58.1/simba/assets/icons/outlier.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/icons/clahe.png` & `Simba-UW-tf-dev-1.58.1/simba/assets/icons/clahe.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/icons/trash.png` & `Simba-UW-tf-dev-1.58.1/simba/assets/icons/trash.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/icons/about.png` & `Simba-UW-tf-dev-1.58.1/simba/assets/icons/about.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/icons/convert.png` & `Simba-UW-tf-dev-1.58.1/simba/assets/icons/convert.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/icons/SimBA_logo.icns` & `Simba-UW-tf-dev-1.58.1/simba/assets/icons/SimBA_logo.icns`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/icons/reorganize.png` & `Simba-UW-tf-dev-1.58.1/simba/assets/icons/reorganize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/icons/browse.png` & `Simba-UW-tf-dev-1.58.1/simba/assets/icons/browse.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/icons/SimBA_logo.png` & `Simba-UW-tf-dev-1.58.1/simba/assets/icons/SimBA_logo.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/icons/ethovision.png` & `Simba-UW-tf-dev-1.58.1/simba/assets/icons/ethovision.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/icons/close.png` & `Simba-UW-tf-dev-1.58.1/simba/assets/icons/close.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/dash_simba_base.css` & `Simba-UW-tf-dev-1.58.1/simba/assets/dash_simba_base.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/assets/TheGoldenLab.PNG` & `Simba-UW-tf-dev-1.58.1/simba/assets/TheGoldenLab.PNG`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/read_config_unit_tests.py` & `Simba-UW-tf-dev-1.58.1/simba/read_config_unit_tests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/project_config_creator.py` & `Simba-UW-tf-dev-1.58.1/simba/project_config_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/train_single_model.py` & `Simba-UW-tf-dev-1.58.1/simba/train_single_model.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/create_clf_log.py` & `Simba-UW-tf-dev-1.58.1/simba/create_clf_log.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/batch_process_videos/.DS_Store` & `Simba-UW-tf-dev-1.58.1/simba/batch_process_videos/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/batch_process_videos/batch_process_menus.py` & `Simba-UW-tf-dev-1.58.1/simba/batch_process_videos/batch_process_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/batch_process_videos/batch_process_create_ffmpeg_commands.py` & `Simba-UW-tf-dev-1.58.1/simba/batch_process_videos/batch_process_create_ffmpeg_commands.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/Kleinberg_calculator.py` & `Simba-UW-tf-dev-1.58.1/simba/Kleinberg_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/reorganize_keypoint_in_pose.py` & `Simba-UW-tf-dev-1.58.1/simba/reorganize_keypoint_in_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/simba/play_annotation_video.py` & `Simba-UW-tf-dev-1.58.1/simba/play_annotation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/Simba_UW_tf_dev.egg-info/PKG-INFO` & `Simba-UW-tf-dev-1.58.1/Simba_UW_tf_dev.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.57.9
+Version: 1.58.1
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.57.9/Simba_UW_tf_dev.egg-info/SOURCES.txt` & `Simba-UW-tf-dev-1.58.1/Simba_UW_tf_dev.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -230,14 +230,16 @@
 simba/mixins/unsupervised_mixin.py
 simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.1.nbc
 simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.nbi
 simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.1.nbc
 simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.nbi
 simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.1.nbc
 simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.nbi
+simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.1.nbc
+simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.nbi
 simba/outlier_tools/.DS_Store
 simba/outlier_tools/__init__.py
 simba/outlier_tools/outlier_corrector_location.py
 simba/outlier_tools/outlier_corrector_movement.py
 simba/outlier_tools/skip_outlier_correction.py
 simba/outlier_tools/.idea/encodings.xml
 simba/outlier_tools/.idea/misc.xml
```

### Comparing `Simba-UW-tf-dev-1.57.9/Simba_UW_tf_dev.egg-info/requires.txt` & `Simba-UW-tf-dev-1.58.1/Simba_UW_tf_dev.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/LICENSE.md` & `Simba-UW-tf-dev-1.58.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/README.md` & `Simba-UW-tf-dev-1.58.1/README.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.9/setup.py` & `Simba-UW-tf-dev-1.58.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Licensed under GNU Lesser General Public License v3.0
 """
 
 import setuptools
 
 setuptools.setup(
     name="Simba-UW-tf-dev",
-    version="1.57.9",
+    version="1.58.1",
     author="Simon Nilsson, Jia Jie Choong, Sophia Hwang",
     author_email="sronilsson@gmail.com",
     description="Toolkit for computer classification of complex social behaviors in experimental animals",
     url="https://github.com/sgoldenlab/simba",
     install_requires=['Pillow == 5.4.1', 'pyyaml == 5.3.1','shapely == 1.7','wxpython == 4.0.4',
               'dtreeviz == 0.8.1','eli5 == 0.10.1','graphviz == 0.11',
               'imblearn == 0.0','imgaug == 0.4.0','imutils == 0.5.2','matplotlib == 3.0.3', 'numpy == 1.18.1',
```

