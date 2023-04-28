# Comparing `tmp/Simba-UW-tf-dev-1.57.8.tar.gz` & `tmp/Simba-UW-tf-dev-1.57.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Simba-UW-tf-dev-1.57.8.tar", last modified: Thu Apr 27 19:37:20 2023, max compression
+gzip compressed data, was "dist/Simba-UW-tf-dev-1.57.9.tar", last modified: Fri Apr 28 00:34:08 2023, max compression
```

## Comparing `Simba-UW-tf-dev-1.57.8.tar` & `Simba-UW-tf-dev-1.57.9.tar`

### file list

```diff
@@ -1,398 +1,398 @@
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-27 19:37:20.000000 Simba-UW-tf-dev-1.57.8/
--rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-27 19:37:20.000000 Simba-UW-tf-dev-1.57.8/PKG-INFO
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-27 19:37:20.000000 Simba-UW-tf-dev-1.57.8/simba/
--rw-r--r--   0 simon      (501) staff       (20)    41423 2023-04-27 12:44:27.000000 Simba-UW-tf-dev-1.57.8/simba/video_processing.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-27 19:37:20.000000 Simba-UW-tf-dev-1.57.8/simba/blob_storage/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-21 20:39:46.000000 Simba-UW-tf-dev-1.57.8/simba/blob_storage/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    11539 2023-04-27 15:22:30.000000 Simba-UW-tf-dev-1.57.8/simba/interpolate_smooth.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-27 19:37:20.000000 Simba-UW-tf-dev-1.57.8/simba/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)    11902 2023-04-25 01:50:43.000000 Simba-UW-tf-dev-1.57.8/simba/unsupervised/dbcv_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     3354 2023-04-20 14:05:40.000000 Simba-UW-tf-dev-1.57.8/simba/unsupervised/enums.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-23 19:55:32.000000 Simba-UW-tf-dev-1.57.8/simba/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7412 2023-04-25 14:58:07.000000 Simba-UW-tf-dev-1.57.8/simba/unsupervised/dataset_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     4775 2023-04-25 14:58:07.000000 Simba-UW-tf-dev-1.57.8/simba/unsupervised/grid_search_visualizers.py
--rw-r--r--   0 simon      (501) staff       (20)     6649 2023-04-25 14:58:07.000000 Simba-UW-tf-dev-1.57.8/simba/unsupervised/data_extractor.py
--rw-r--r--   0 simon      (501) staff       (20)     9907 2023-04-20 12:55:14.000000 Simba-UW-tf-dev-1.57.8/simba/unsupervised/ui.py
--rw-r--r--   0 simon      (501) staff       (20)     8337 2023-04-25 11:06:37.000000 Simba-UW-tf-dev-1.57.8/simba/unsupervised/umap_embedder.py
--rw-r--r--   0 simon      (501) staff       (20)    41476 2023-04-25 14:58:07.000000 Simba-UW-tf-dev-1.57.8/simba/unsupervised/pop_up_classes.py
--rw-r--r--   0 simon      (501) staff       (20)     2317 2023-04-25 14:58:07.000000 Simba-UW-tf-dev-1.57.8/simba/unsupervised/bout_aggregator.py
--rw-r--r--   0 simon      (501) staff       (20)    18443 2023-04-25 14:58:07.000000 Simba-UW-tf-dev-1.57.8/simba/unsupervised/cluster_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     2188 2023-04-18 23:25:29.000000 Simba-UW-tf-dev-1.57.8/simba/unsupervised/data_map.yaml
--rw-r--r--   0 simon      (501) staff       (20)     8301 2023-04-25 11:05:05.000000 Simba-UW-tf-dev-1.57.8/simba/unsupervised/hdbscan_clusterer.py
--rw-r--r--   0 simon      (501) staff       (20)     3931 2023-04-19 18:21:47.000000 Simba-UW-tf-dev-1.57.8/simba/unsupervised/tsne.py
--rw-r--r--   0 simon      (501) staff       (20)     5871 2023-04-25 01:50:43.000000 Simba-UW-tf-dev-1.57.8/simba/unsupervised/cluster_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    19720 2023-04-27 15:13:49.000000 Simba-UW-tf-dev-1.57.8/simba/enums.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-27 19:37:20.000000 Simba-UW-tf-dev-1.57.8/simba/bounding_box_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/bounding_box_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     6794 2023-04-25 13:26:59.000000 Simba-UW-tf-dev-1.57.8/simba/bounding_box_tools/agg_boundary_stats.py
--rw-r--r--   0 simon      (501) staff       (20)    23483 2023-04-25 19:00:39.000000 Simba-UW-tf-dev-1.57.8/simba/bounding_box_tools/boundary_menus.py
--rw-r--r--   0 simon      (501) staff       (20)     8485 2023-04-25 13:26:59.000000 Simba-UW-tf-dev-1.57.8/simba/bounding_box_tools/boundary_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     6037 2023-04-25 15:53:12.000000 Simba-UW-tf-dev-1.57.8/simba/bounding_box_tools/find_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    10470 2023-04-25 13:27:00.000000 Simba-UW-tf-dev-1.57.8/simba/bounding_box_tools/visualize_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    32772 2023-04-26 18:25:34.000000 Simba-UW-tf-dev-1.57.8/simba/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-27 19:37:20.000000 Simba-UW-tf-dev-1.57.8/simba/feature_extractors/
--rw-r--r--   0 simon      (501) staff       (20)    42247 2023-04-26 01:31:26.000000 Simba-UW-tf-dev-1.57.8/simba/feature_extractors/feature_extractor_14bp.py
--rw-r--r--   0 simon      (501) staff       (20)    21376 2023-04-26 01:31:26.000000 Simba-UW-tf-dev-1.57.8/simba/feature_extractors/feature_extractor_7bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-27 19:37:20.000000 Simba-UW-tf-dev-1.57.8/simba/feature_extractors/misc/
--rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.57.8/simba/feature_extractors/misc/doctests.py
--rw-r--r--   0 simon      (501) staff       (20)    23850 2023-04-17 18:48:40.000000 Simba-UW-tf-dev-1.57.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
--rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.57.8/simba/feature_extractors/misc/read_in_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     2460 2023-04-22 18:02:29.000000 Simba-UW-tf-dev-1.57.8/simba/feature_extractors/misc/peaks.py
--rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.57.8/simba/feature_extractors/misc/fish_feature_extractor_2022.py
--rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.57.8/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
--rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.57.8/simba/feature_extractors/misc/convex_hull_scratch_1.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.57.8/simba/feature_extractors/misc/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    21398 2023-04-16 17:03:37.000000 Simba-UW-tf-dev-1.57.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
--rw-r--r--   0 simon      (501) staff       (20)     7127 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/feature_extractors/misc/egocentrical_aligner.py
--rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.57.8/simba/feature_extractors/misc/count_values_in_range.py
--rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/feature_extractors/misc/graph_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/feature_extractors/misc/termite_rois.csv
--rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.57.8/simba/feature_extractors/misc/mutual_exclusive.py
--rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.57.8/simba/feature_extractors/misc/video_color.py
--rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/feature_extractors/misc/graph_3d_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.57.8/simba/feature_extractors/misc/video_rotator.py
--rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/feature_extractors/misc/add_probability_cnt_features.py
--rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.57.8/simba/feature_extractors/misc/make_splash.py
--rw-r--r--   0 simon      (501) staff       (20)     1658 2023-04-22 19:16:28.000000 Simba-UW-tf-dev-1.57.8/simba/feature_extractors/misc/time_stamp_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-15 19:24:18.000000 Simba-UW-tf-dev-1.57.8/simba/feature_extractors/misc/video_rotator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    30677 2023-04-27 01:57:28.000000 Simba-UW-tf-dev-1.57.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
--rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.57.8/simba/feature_extractors/misc/convex_hull_scratch_2.py
--rw-r--r--   0 simon      (501) staff       (20)    27709 2023-04-26 01:31:26.000000 Simba-UW-tf-dev-1.57.8/simba/feature_extractors/feature_extractor_8bps_2_animals.py
--rw-r--r--   0 simon      (501) staff       (20)    10244 2023-04-25 21:03:39.000000 Simba-UW-tf-dev-1.57.8/simba/feature_extractors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     2293 2023-04-24 20:15:27.000000 Simba-UW-tf-dev-1.57.8/simba/feature_extractors/perimeter_jit.py
--rw-r--r--   0 simon      (501) staff       (20)    10762 2023-04-25 21:03:09.000000 Simba-UW-tf-dev-1.57.8/simba/feature_extractors/feature_subsets.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/feature_extractors/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-27 19:37:20.000000 Simba-UW-tf-dev-1.57.8/simba/feature_extractors/__pycache__/
--rw-r--r--   0 simon      (501) staff       (20)      905 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.57.8/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)   238196 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.57.8/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    69038 2023-04-04 11:32:25.000000 Simba-UW-tf-dev-1.57.8/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)   238298 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.57.8/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    69338 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.57.8/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc
--rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.57.8/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     2179 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.57.8/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     8248 2023-04-26 01:31:25.000000 Simba-UW-tf-dev-1.57.8/simba/feature_extractors/feature_extractor_user_defined.py
--rw-r--r--   0 simon      (501) staff       (20)    46191 2023-04-26 01:31:25.000000 Simba-UW-tf-dev-1.57.8/simba/feature_extractors/feature_extractor_16bp.py
--rw-r--r--   0 simon      (501) staff       (20)    27391 2023-04-25 20:57:10.000000 Simba-UW-tf-dev-1.57.8/simba/feature_extractors/feature_extractor_9bp.py
--rw-r--r--   0 simon      (501) staff       (20)    23873 2023-04-26 01:31:26.000000 Simba-UW-tf-dev-1.57.8/simba/feature_extractors/feature_extractor_8bp.py
--rw-r--r--   0 simon      (501) staff       (20)    16793 2023-04-26 01:31:26.000000 Simba-UW-tf-dev-1.57.8/simba/feature_extractors/feature_extractor_4bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-27 19:37:20.000000 Simba-UW-tf-dev-1.57.8/simba/feature_extractors/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/feature_extractors/.idea/features_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/feature_extractors/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-27 19:37:20.000000 Simba-UW-tf-dev-1.57.8/simba/feature_extractors/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-27 19:37:20.000000 Simba-UW-tf-dev-1.57.8/simba/feature_extractors/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/feature_extractors/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/feature_extractors/.idea/.gitignore
--rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/feature_extractors/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/feature_extractors/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/feature_extractors/.idea/.name
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/feature_extractors/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)    15351 2023-04-06 14:48:36.000000 Simba-UW-tf-dev-1.57.8/simba/requirements.txt
--rw-r--r--   0 simon      (501) staff       (20)     4827 2023-04-27 02:10:00.000000 Simba-UW-tf-dev-1.57.8/simba/severity_processor.py
--rw-r--r--   0 simon      (501) staff       (20)     5942 2023-04-25 15:16:24.000000 Simba-UW-tf-dev-1.57.8/simba/user_pose_config_creator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-27 19:37:20.000000 Simba-UW-tf-dev-1.57.8/simba/mixins/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:26:03.000000 Simba-UW-tf-dev-1.57.8/simba/mixins/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    40244 2023-04-26 00:44:45.000000 Simba-UW-tf-dev-1.57.8/simba/mixins/pop_up_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    28874 2023-04-26 19:15:07.000000 Simba-UW-tf-dev-1.57.8/simba/mixins/config_reader.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-27 19:37:20.000000 Simba-UW-tf-dev-1.57.8/simba/mixins/__pycache__/
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-25 20:46:51.000000 Simba-UW-tf-dev-1.57.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-24 19:51:34.000000 Simba-UW-tf-dev-1.57.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-24 19:51:34.000000 Simba-UW-tf-dev-1.57.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-25 20:46:51.000000 Simba-UW-tf-dev-1.57.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-24 19:06:57.000000 Simba-UW-tf-dev-1.57.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-24 19:06:57.000000 Simba-UW-tf-dev-1.57.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    22078 2023-04-27 01:56:00.000000 Simba-UW-tf-dev-1.57.8/simba/mixins/feature_extraction_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    52214 2023-04-27 17:55:13.000000 Simba-UW-tf-dev-1.57.8/simba/mixins/plotting_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     6063 2023-04-24 20:15:27.000000 Simba-UW-tf-dev-1.57.8/simba/mixins/unsupervised_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    55244 2023-04-27 01:40:24.000000 Simba-UW-tf-dev-1.57.8/simba/mixins/train_model_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    33917 2023-04-27 16:59:00.000000 Simba-UW-tf-dev-1.57.8/simba/machine_model_settings_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5193 2023-04-25 12:41:52.000000 Simba-UW-tf-dev-1.57.8/simba/remove_keypoints_in_pose.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-27 19:37:20.000000 Simba-UW-tf-dev-1.57.8/simba/third_party_label_appenders/
--rw-r--r--   0 simon      (501) staff       (20)     6228 2023-04-26 18:27:58.000000 Simba-UW-tf-dev-1.57.8/simba/third_party_label_appenders/deepethogram_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     9945 2023-04-25 01:50:43.000000 Simba-UW-tf-dev-1.57.8/simba/third_party_label_appenders/BORIS_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     9063 2023-04-25 01:50:43.000000 Simba-UW-tf-dev-1.57.8/simba/third_party_label_appenders/observer_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    16888 2023-04-25 14:58:07.000000 Simba-UW-tf-dev-1.57.8/simba/third_party_label_appenders/tools.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.57.8/simba/third_party_label_appenders/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18242 2023-04-25 01:50:43.000000 Simba-UW-tf-dev-1.57.8/simba/third_party_label_appenders/third_party_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     8186 2023-04-25 01:50:43.000000 Simba-UW-tf-dev-1.57.8/simba/third_party_label_appenders/ethovision_import.py
--rw-r--r--   0 simon      (501) staff       (20)     6859 2023-04-25 01:50:43.000000 Simba-UW-tf-dev-1.57.8/simba/third_party_label_appenders/BENTO_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     5331 2023-04-25 01:50:43.000000 Simba-UW-tf-dev-1.57.8/simba/third_party_label_appenders/solomon_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     7168 2023-04-25 11:55:36.000000 Simba-UW-tf-dev-1.57.8/simba/multi_cropper.py
--rw-r--r--   0 simon      (501) staff       (20)    12720 2023-04-25 15:08:49.000000 Simba-UW-tf-dev-1.57.8/simba/FSTTC_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    12570 2023-04-25 15:08:48.000000 Simba-UW-tf-dev-1.57.8/simba/create_project_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    13056 2023-04-26 18:37:46.000000 Simba-UW-tf-dev-1.57.8/simba/video_info_table.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-27 19:37:20.000000 Simba-UW-tf-dev-1.57.8/simba/cue_light_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:25:58.000000 Simba-UW-tf-dev-1.57.8/simba/cue_light_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7558 2023-04-25 13:26:59.000000 Simba-UW-tf-dev-1.57.8/simba/cue_light_tools/cue_light_clf_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)    12017 2023-04-25 13:26:59.000000 Simba-UW-tf-dev-1.57.8/simba/cue_light_tools/cue_light_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    17695 2023-04-25 13:27:00.000000 Simba-UW-tf-dev-1.57.8/simba/cue_light_tools/cue_light_menues.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/cue_light_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     1660 2023-04-25 15:53:12.000000 Simba-UW-tf-dev-1.57.8/simba/cue_light_tools/cue_light_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    15253 2023-04-25 15:26:48.000000 Simba-UW-tf-dev-1.57.8/simba/cue_light_tools/cue_light_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    11922 2023-04-25 18:38:05.000000 Simba-UW-tf-dev-1.57.8/simba/cue_light_tools/cue_light_movement_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     2799 2023-04-25 11:23:20.000000 Simba-UW-tf-dev-1.57.8/simba/extract_frames_fast.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-27 19:37:20.000000 Simba-UW-tf-dev-1.57.8/simba/utils/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 20:15:03.000000 Simba-UW-tf-dev-1.57.8/simba/utils/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7335 2023-04-10 18:32:39.000000 Simba-UW-tf-dev-1.57.8/simba/utils/warnings.py
--rw-r--r--   0 simon      (501) staff       (20)     5562 2023-04-25 21:03:09.000000 Simba-UW-tf-dev-1.57.8/simba/utils/checks.py
--rw-r--r--   0 simon      (501) staff       (20)    33727 2023-04-27 15:02:22.000000 Simba-UW-tf-dev-1.57.8/simba/utils/read_write.py
--rw-r--r--   0 simon      (501) staff       (20)     6998 2023-04-25 20:57:10.000000 Simba-UW-tf-dev-1.57.8/simba/utils/lookups.py
--rw-r--r--   0 simon      (501) staff       (20)    14630 2023-04-26 12:39:28.000000 Simba-UW-tf-dev-1.57.8/simba/utils/errors.py
--rw-r--r--   0 simon      (501) staff       (20)    14062 2023-04-27 18:46:49.000000 Simba-UW-tf-dev-1.57.8/simba/utils/data.py
--rw-r--r--   0 simon      (501) staff       (20)     1537 2023-04-24 18:39:34.000000 Simba-UW-tf-dev-1.57.8/simba/utils/printing.py
--rw-r--r--   0 simon      (501) staff       (20)    20580 2023-04-25 15:08:48.000000 Simba-UW-tf-dev-1.57.8/simba/labelling_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     9371 2023-04-26 20:31:09.000000 Simba-UW-tf-dev-1.57.8/simba/timebins_movement_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/SimBA_dash_app.py
--rw-r--r--   0 simon      (501) staff       (20)     7421 2023-04-27 02:02:22.000000 Simba-UW-tf-dev-1.57.8/simba/timebins_clf_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     8215 2023-04-25 11:06:37.000000 Simba-UW-tf-dev-1.57.8/simba/calculate_px_dist.py
--rw-r--r--   0 simon      (501) staff       (20)     6411 2023-04-25 18:52:57.000000 Simba-UW-tf-dev-1.57.8/simba/movement_processor.py
--rw-r--r--   0 simon      (501) staff       (20)     2904 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/pybursts.py
--rw-r--r--   0 simon      (501) staff       (20)     5630 2023-04-25 15:16:24.000000 Simba-UW-tf-dev-1.57.8/simba/reverse_2_animal_tracking.py
--rw-r--r--   0 simon      (501) staff       (20)     9654 2023-04-25 11:22:07.000000 Simba-UW-tf-dev-1.57.8/simba/Directing_animals_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     3170 2023-04-25 13:13:10.000000 Simba-UW-tf-dev-1.57.8/simba/Validate_model_one_video_run_clf.py
--rw-r--r--   0 simon      (501) staff       (20)    10874 2023-04-25 13:05:45.000000 Simba-UW-tf-dev-1.57.8/simba/tkinter_functions.py
--rw-r--r--   0 simon      (501) staff       (20)    13112 2023-04-26 21:09:13.000000 Simba-UW-tf-dev-1.57.8/simba/setting_menu.py
--rw-r--r--   0 simon      (501) staff       (20)     6317 2023-04-25 18:03:32.000000 Simba-UW-tf-dev-1.57.8/simba/interpolate_pose.py
--rw-r--r--   0 simon      (501) staff       (20)     3543 2023-04-27 18:41:05.000000 Simba-UW-tf-dev-1.57.8/simba/run_inference.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-27 19:37:20.000000 Simba-UW-tf-dev-1.57.8/simba/plotting/
--rw-r--r--   0 simon      (501) staff       (20)     9137 2023-04-26 02:10:59.000000 Simba-UW-tf-dev-1.57.8/simba/plotting/gantt_creator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-27 19:37:20.000000 Simba-UW-tf-dev-1.57.8/simba/plotting/tools/
--rw-r--r--   0 simon      (501) staff       (20)     5358 2023-04-24 20:41:26.000000 Simba-UW-tf-dev-1.57.8/simba/plotting/tools/tkinter_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    13244 2023-04-26 19:34:04.000000 Simba-UW-tf-dev-1.57.8/simba/plotting/ROI_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-25 23:35:57.000000 Simba-UW-tf-dev-1.57.8/simba/plotting/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    14600 2023-04-26 14:02:58.000000 Simba-UW-tf-dev-1.57.8/simba/plotting/shap_agg_stats_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    10167 2023-04-26 15:08:19.000000 Simba-UW-tf-dev-1.57.8/simba/plotting/gantt_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15975 2023-04-26 13:44:02.000000 Simba-UW-tf-dev-1.57.8/simba/plotting/heat_mapper_clf_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     8557 2023-04-26 12:36:28.000000 Simba-UW-tf-dev-1.57.8/simba/plotting/probability_plot_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    12267 2023-04-26 11:18:28.000000 Simba-UW-tf-dev-1.57.8/simba/plotting/plot_clf_results.py
--rw-r--r--   0 simon      (501) staff       (20)    16556 2023-04-26 11:24:45.000000 Simba-UW-tf-dev-1.57.8/simba/plotting/plot_clf_results_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15885 2023-04-26 12:47:24.000000 Simba-UW-tf-dev-1.57.8/simba/plotting/ROI_feature_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12746 2023-04-26 20:06:54.000000 Simba-UW-tf-dev-1.57.8/simba/plotting/heat_mapper_location.py
--rw-r--r--   0 simon      (501) staff       (20)    12507 2023-04-26 12:41:15.000000 Simba-UW-tf-dev-1.57.8/simba/plotting/probability_plot_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     5239 2023-04-26 02:56:05.000000 Simba-UW-tf-dev-1.57.8/simba/plotting/interactive_probability_grapher.py
--rw-r--r--   0 simon      (501) staff       (20)     5748 2023-04-26 11:37:28.000000 Simba-UW-tf-dev-1.57.8/simba/plotting/plot_pose_in_dir.py
--rw-r--r--   0 simon      (501) staff       (20)    12771 2023-04-26 14:16:42.000000 Simba-UW-tf-dev-1.57.8/simba/plotting/single_run_model_validation_video.py
--rw-r--r--   0 simon      (501) staff       (20)    12236 2023-04-27 12:57:18.000000 Simba-UW-tf-dev-1.57.8/simba/plotting/frame_mergerer_ffmpeg.py
--rw-r--r--   0 simon      (501) staff       (20)     7887 2023-04-26 13:22:21.000000 Simba-UW-tf-dev-1.57.8/simba/plotting/Directing_animals_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    11204 2023-04-27 12:38:21.000000 Simba-UW-tf-dev-1.57.8/simba/plotting/clf_validator.py
--rw-r--r--   0 simon      (501) staff       (20)    16708 2023-04-26 15:09:39.000000 Simba-UW-tf-dev-1.57.8/simba/plotting/path_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    11324 2023-04-26 13:09:33.000000 Simba-UW-tf-dev-1.57.8/simba/plotting/ROI_feature_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     9876 2023-04-25 23:33:34.000000 Simba-UW-tf-dev-1.57.8/simba/plotting/data_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    12920 2023-04-26 10:57:46.000000 Simba-UW-tf-dev-1.57.8/simba/plotting/path_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     8506 2023-04-25 13:35:52.000000 Simba-UW-tf-dev-1.57.8/simba/plotting/ez_lineplot.py
--rw-r--r--   0 simon      (501) staff       (20)    11494 2023-04-26 13:25:36.000000 Simba-UW-tf-dev-1.57.8/simba/plotting/distance_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15604 2023-04-26 13:46:25.000000 Simba-UW-tf-dev-1.57.8/simba/plotting/ROI_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13127 2023-04-25 13:50:19.000000 Simba-UW-tf-dev-1.57.8/simba/plotting/heat_mapper_clf.py
--rw-r--r--   0 simon      (501) staff       (20)     8973 2023-04-26 00:37:26.000000 Simba-UW-tf-dev-1.57.8/simba/plotting/distance_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13560 2023-04-27 18:03:45.000000 Simba-UW-tf-dev-1.57.8/simba/plotting/single_run_model_validation_video_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     9744 2023-04-25 18:55:04.000000 Simba-UW-tf-dev-1.57.8/simba/plotting/Directing_animals_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    16328 2023-04-26 20:12:38.000000 Simba-UW-tf-dev-1.57.8/simba/plotting/heat_mapper_location_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/run_dash_tkinter.py
--rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/dash_app.py
--rw-r--r--   0 simon      (501) staff       (20)     2877 2023-04-25 15:08:48.000000 Simba-UW-tf-dev-1.57.8/simba/extract_annotation_frames.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-27 19:37:20.000000 Simba-UW-tf-dev-1.57.8/simba/roi_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6501 2023-04-25 18:50:18.000000 Simba-UW-tf-dev-1.57.8/simba/roi_tools/ROI_time_bin_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     1766 2023-04-25 18:48:44.000000 Simba-UW-tf-dev-1.57.8/simba/roi_tools/ROI_movement_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-20 12:47:56.000000 Simba-UW-tf-dev-1.57.8/simba/roi_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    43128 2023-04-26 19:19:44.000000 Simba-UW-tf-dev-1.57.8/simba/roi_tools/ROI_define.py
--rw-r--r--   0 simon      (501) staff       (20)     3402 2023-04-26 19:25:50.000000 Simba-UW-tf-dev-1.57.8/simba/roi_tools/ROI_reset.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/roi_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    19703 2023-04-26 14:59:42.000000 Simba-UW-tf-dev-1.57.8/simba/roi_tools/ROI_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    11332 2023-04-26 21:13:20.000000 Simba-UW-tf-dev-1.57.8/simba/roi_tools/ROI_feature_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     3651 2023-04-26 19:22:41.000000 Simba-UW-tf-dev-1.57.8/simba/roi_tools/ROI_multiply.py
--rw-r--r--   0 simon      (501) staff       (20)      961 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/roi_tools/ROI_size_calculations.py
--rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/roi_tools/ROI_zoom.py
--rw-r--r--   0 simon      (501) staff       (20)    11397 2023-04-26 15:12:12.000000 Simba-UW-tf-dev-1.57.8/simba/roi_tools/ROI_directing_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/roi_tools/ROI_move_shape.py
--rw-r--r--   0 simon      (501) staff       (20)     5073 2023-04-25 14:55:41.000000 Simba-UW-tf-dev-1.57.8/simba/roi_tools/ROI_menus.py
--rw-r--r--   0 simon      (501) staff       (20)    13793 2023-04-26 14:59:42.000000 Simba-UW-tf-dev-1.57.8/simba/roi_tools/ROI_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    22685 2023-04-25 14:55:41.000000 Simba-UW-tf-dev-1.57.8/simba/roi_tools/ROI_image.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-27 19:37:20.000000 Simba-UW-tf-dev-1.57.8/simba/pose_importers/
--rw-r--r--   0 simon      (501) staff       (20)     2477 2023-04-26 18:25:13.000000 Simba-UW-tf-dev-1.57.8/simba/pose_importers/read_DANNCE_mat.py
--rw-r--r--   0 simon      (501) staff       (20)    21991 2023-04-27 15:50:07.000000 Simba-UW-tf-dev-1.57.8/simba/pose_importers/sleap_importer_slp.py
--rw-r--r--   0 simon      (501) staff       (20)    23507 2023-04-27 15:45:27.000000 Simba-UW-tf-dev-1.57.8/simba/pose_importers/sleap_importer_h5.py
--rw-r--r--   0 simon      (501) staff       (20)    23592 2023-04-27 15:41:32.000000 Simba-UW-tf-dev-1.57.8/simba/pose_importers/dlc_multi_animal_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-25 16:49:14.000000 Simba-UW-tf-dev-1.57.8/simba/pose_importers/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    20973 2023-04-27 15:41:32.000000 Simba-UW-tf-dev-1.57.8/simba/pose_importers/sleap_importer_csv.py
--rw-r--r--   0 simon      (501) staff       (20)     7761 2023-04-25 18:26:26.000000 Simba-UW-tf-dev-1.57.8/simba/pose_importers/import_mars.py
--rw-r--r--   0 simon      (501) staff       (20)     6935 2023-04-27 14:57:59.000000 Simba-UW-tf-dev-1.57.8/simba/pose_importers/dlc_importer_csv.py
--rw-r--r--   0 simon      (501) staff       (20)     6705 2023-04-25 18:51:56.000000 Simba-UW-tf-dev-1.57.8/simba/pose_importers/trk_importer.py
--rw-r--r--   0 simon      (501) staff       (20)   238447 2023-04-27 19:37:01.000000 Simba-UW-tf-dev-1.57.8/simba/pop_up_classes.py
--rw-r--r--   0 simon      (501) staff       (20)     4695 2023-04-26 18:17:53.000000 Simba-UW-tf-dev-1.57.8/simba/extract_seqframes.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-27 19:37:20.000000 Simba-UW-tf-dev-1.57.8/simba/pose_configurations/
--rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.57.8/simba/pose_configurations/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-27 19:37:20.000000 Simba-UW-tf-dev-1.57.8/simba/pose_configurations/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.57.8/simba/pose_configurations/bp_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-10 12:22:28.000000 Simba-UW-tf-dev-1.57.8/simba/pose_configurations/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-27 19:37:20.000000 Simba-UW-tf-dev-1.57.8/simba/pose_configurations/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       24 2023-03-20 15:55:45.000000 Simba-UW-tf-dev-1.57.8/simba/pose_configurations/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.57.8/simba/pose_configurations/no_animals/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-27 19:37:20.000000 Simba-UW-tf-dev-1.57.8/simba/pose_configurations/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.57.8/simba/pose_configurations/configuration_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)      267 2023-03-20 15:55:45.000000 Simba-UW-tf-dev-1.57.8/simba/pose_configurations/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-27 19:37:20.000000 Simba-UW-tf-dev-1.57.8/simba/pose_configurations/schematics/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.57.8/simba/pose_configurations/schematics/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/pose_configurations/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.57.8/simba/pose_configurations/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/pose_configurations/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.57.8/simba/pose_configurations/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.57.8/simba/pose_configurations/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/pose_configurations/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/pose_configurations/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/pose_configurations/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/pose_configurations/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/pose_configurations/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/pose_configurations/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/pose_configurations/schematics/1.png
--rw-r--r--   0 simon      (501) staff       (20)     7184 2023-04-25 11:24:28.000000 Simba-UW-tf-dev-1.57.8/simba/get_coordinates_tools_v2.py
--rw-r--r--   0 simon      (501) staff       (20)    15731 2023-04-25 15:16:24.000000 Simba-UW-tf-dev-1.57.8/simba/pup_retrieval_protocol.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-27 19:37:20.000000 Simba-UW-tf-dev-1.57.8/simba/outlier_tools/
--rw-r--r--   0 simon      (501) staff       (20)     7397 2023-04-26 19:04:38.000000 Simba-UW-tf-dev-1.57.8/simba/outlier_tools/outlier_corrector_movement.py
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-15 17:05:05.000000 Simba-UW-tf-dev-1.57.8/simba/outlier_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/outlier_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8161 2023-04-26 19:05:15.000000 Simba-UW-tf-dev-1.57.8/simba/outlier_tools/outlier_corrector_location.py
--rw-r--r--   0 simon      (501) staff       (20)     2674 2023-04-26 19:01:06.000000 Simba-UW-tf-dev-1.57.8/simba/outlier_tools/skip_outlier_correction.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-27 19:37:20.000000 Simba-UW-tf-dev-1.57.8/simba/outlier_tools/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/outlier_tools/.idea/outlier_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/outlier_tools/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-27 19:37:20.000000 Simba-UW-tf-dev-1.57.8/simba/outlier_tools/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-27 19:37:20.000000 Simba-UW-tf-dev-1.57.8/simba/outlier_tools/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/outlier_tools/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/outlier_tools/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/outlier_tools/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/outlier_tools/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)     2613 2023-04-25 15:16:24.000000 Simba-UW-tf-dev-1.57.8/simba/pose_reset.py
--rw-r--r--   0 simon      (501) staff       (20)    18234 2023-04-27 17:03:57.000000 Simba-UW-tf-dev-1.57.8/simba/train_mutiple_models.py
--rw-r--r--   0 simon      (501) staff       (20)    63970 2023-04-27 18:41:05.000000 Simba-UW-tf-dev-1.57.8/simba/SimBA.py
--rw-r--r--   0 simon      (501) staff       (20)    26572 2023-04-25 11:49:41.000000 Simba-UW-tf-dev-1.57.8/simba/labelling_advanced_interface.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-27 19:37:20.000000 Simba-UW-tf-dev-1.57.8/simba/assets/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-27 19:37:20.000000 Simba-UW-tf-dev-1.57.8/simba/assets/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/assets/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/assets/unsupervised/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/assets/unsupervised/features.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-27 19:37:20.000000 Simba-UW-tf-dev-1.57.8/simba/assets/shap/
--rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/assets/shap/down_arrow.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/assets/shap/intruder_shape.jpg
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-27 19:37:20.000000 Simba-UW-tf-dev-1.57.8/simba/assets/shap/feature_categories/
--rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
--rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/assets/shap/feature_categories/shap_feature_categories.csv
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-04-10 20:37:13.000000 Simba-UW-tf-dev-1.57.8/simba/assets/shap/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/assets/shap/resident_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/assets/shap/resident_intruder_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/assets/shap/animal_distances.jpg
--rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/assets/shap/baseline_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/assets/shap/ubuntu.regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/assets/shap/side_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/assets/shap/UbuntuMono-Regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/assets/shap/side_scale_5.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/assets/shap/intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/assets/shap/resident_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/assets/shap/color_bar.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/assets/shap/resident_intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)    16388 2023-04-25 19:14:34.000000 Simba-UW-tf-dev-1.57.8/simba/assets/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-27 19:37:20.000000 Simba-UW-tf-dev-1.57.8/simba/assets/lookups/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/assets/lookups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/assets/lookups/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)     2987 2023-04-25 20:39:03.000000 Simba-UW-tf-dev-1.57.8/simba/assets/lookups/feature_extraction_headers.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/assets/lookups/features.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/assets/lookups/unsupervised_example_x.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-27 19:37:20.000000 Simba-UW-tf-dev-1.57.8/simba/assets/stl/
--rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/assets/stl/operant_tray.stl
--rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/assets/stl/operant_lever.stl
--rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/assets/stl/operant_walls.stl
--rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/assets/stl/grid_floor.stl
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-27 19:37:20.000000 Simba-UW-tf-dev-1.57.8/simba/assets/img/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.57.8/simba/assets/img/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/assets/img/about_me.png
--rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.57.8/simba/assets/img/splash.mp4
--rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.57.8/simba/assets/img/bg_2.png
--rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/assets/img/splash.pptx
--rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.57.8/simba/assets/img/bg.png
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/assets/UbuntuMono-Regular.ttf
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-27 19:37:20.000000 Simba-UW-tf-dev-1.57.8/simba/assets/icons/
--rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.57.8/simba/assets/icons/factory.png
--rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.57.8/simba/assets/icons/cluster.png
--rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.57.8/simba/assets/icons/load.png
--rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.57.8/simba/assets/icons/gif.png
--rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.57.8/simba/assets/icons/pose.png
--rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.57.8/simba/assets/icons/features.png
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.57.8/simba/assets/icons/.DS_Store
--rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.57.8/simba/assets/icons/settings.png
--rw-r--r--   0 simon      (501) staff       (20)     2090 2023-04-22 15:14:17.000000 Simba-UW-tf-dev-1.57.8/simba/assets/icons/stopwatch.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.57.8/simba/assets/icons/link.png
--rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/assets/icons/dash_simba.css
--rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.57.8/simba/assets/icons/documentation.png
--rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.57.8/simba/assets/icons/fps.png
--rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.57.8/simba/assets/icons/dimensionality_reduction.png
--rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.57.8/simba/assets/icons/roi.png
--rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.57.8/simba/assets/icons/superimpose.png
--rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.57.8/simba/assets/icons/label.png
--rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.57.8/simba/assets/icons/change.png
--rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.57.8/simba/assets/icons/crop.png
--rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.57.8/simba/assets/icons/rotate.png
--rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.57.8/simba/assets/icons/path.png
--rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.57.8/simba/assets/icons/clip.png
--rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.57.8/simba/assets/icons/restart.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.57.8/simba/assets/icons/calipher.png
--rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.57.8/simba/assets/icons/add_on.png
--rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.57.8/simba/assets/icons/create.png
--rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.57.8/simba/assets/icons/SimBA_logo.ico
--rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.57.8/simba/assets/icons/print.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.57.8/simba/assets/icons/clf.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-27 19:37:20.000000 Simba-UW-tf-dev-1.57.8/simba/assets/icons/concat_icons/
--rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/assets/icons/concat_icons/mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/assets/icons/concat_icons/vertical.png
--rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/assets/icons/concat_icons/horizontal.png
--rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/assets/icons/concat_icons/mixed_mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.57.8/simba/assets/icons/merge.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.57.8/simba/assets/icons/clean.png
--rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.57.8/simba/assets/icons/clf_2.png
--rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.57.8/simba/assets/icons/visualize.png
--rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.57.8/simba/assets/icons/concat.png
--rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.57.8/simba/assets/icons/boris.png
--rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.57.8/simba/assets/icons/frames.png
--rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.57.8/simba/assets/icons/video.png
--rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.57.8/simba/assets/icons/sample.png
--rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.57.8/simba/assets/icons/metrics.png
--rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.57.8/simba/assets/icons/grey.png
--rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.57.8/simba/assets/icons/exit.png
--rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.57.8/simba/assets/icons/outlier.png
--rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.57.8/simba/assets/icons/clahe.png
--rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.57.8/simba/assets/icons/trash.png
--rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.57.8/simba/assets/icons/about.png
--rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.57.8/simba/assets/icons/convert.png
--rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.57.8/simba/assets/icons/SimBA_logo.icns
--rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.57.8/simba/assets/icons/reorganize.png
--rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.57.8/simba/assets/icons/browse.png
--rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.57.8/simba/assets/icons/SimBA_logo.png
--rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.57.8/simba/assets/icons/ethovision.png
--rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.57.8/simba/assets/icons/close.png
--rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/assets/dash_simba_base.css
--rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/assets/TheGoldenLab.PNG
--rw-r--r--   0 simon      (501) staff       (20)     9491 2023-04-25 16:28:55.000000 Simba-UW-tf-dev-1.57.8/simba/read_config_unit_tests.py
--rw-r--r--   0 simon      (501) staff       (20)    11645 2023-04-25 15:16:24.000000 Simba-UW-tf-dev-1.57.8/simba/project_config_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    19000 2023-04-26 18:08:54.000000 Simba-UW-tf-dev-1.57.8/simba/train_single_model.py
--rw-r--r--   0 simon      (501) staff       (20)     6321 2023-04-25 15:08:48.000000 Simba-UW-tf-dev-1.57.8/simba/create_clf_log.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-27 19:37:20.000000 Simba-UW-tf-dev-1.57.8/simba/batch_process_videos/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-17 14:43:38.000000 Simba-UW-tf-dev-1.57.8/simba/batch_process_videos/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    24639 2023-04-25 13:26:59.000000 Simba-UW-tf-dev-1.57.8/simba/batch_process_videos/batch_process_menus.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.8/simba/batch_process_videos/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    11106 2023-04-25 13:26:59.000000 Simba-UW-tf-dev-1.57.8/simba/batch_process_videos/batch_process_create_ffmpeg_commands.py
--rw-r--r--   0 simon      (501) staff       (20)     9520 2023-04-25 19:02:08.000000 Simba-UW-tf-dev-1.57.8/simba/Kleinberg_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8311 2023-04-25 15:16:24.000000 Simba-UW-tf-dev-1.57.8/simba/reorganize_keypoint_in_pose.py
--rw-r--r--   0 simon      (501) staff       (20)      165 2023-03-25 11:18:21.000000 Simba-UW-tf-dev-1.57.8/simba/~$features.pptx
--rw-r--r--   0 simon      (501) staff       (20)     6556 2023-04-25 12:27:22.000000 Simba-UW-tf-dev-1.57.8/simba/play_annotation_video.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-27 19:37:20.000000 Simba-UW-tf-dev-1.57.8/Simba_UW_tf_dev.egg-info/
--rw-rw-r--   0 simon      (501) staff       (20)      579 2023-04-27 19:37:19.000000 Simba-UW-tf-dev-1.57.8/Simba_UW_tf_dev.egg-info/PKG-INFO
--rw-rw-r--   0 simon      (501) staff       (20)    13977 2023-04-27 19:37:19.000000 Simba-UW-tf-dev-1.57.8/Simba_UW_tf_dev.egg-info/SOURCES.txt
--rw-rw-r--   0 simon      (501) staff       (20)       44 2023-04-27 19:37:19.000000 Simba-UW-tf-dev-1.57.8/Simba_UW_tf_dev.egg-info/entry_points.txt
--rw-rw-r--   0 simon      (501) staff       (20)      639 2023-04-27 19:37:19.000000 Simba-UW-tf-dev-1.57.8/Simba_UW_tf_dev.egg-info/requires.txt
--rw-rw-r--   0 simon      (501) staff       (20)        6 2023-04-27 19:37:19.000000 Simba-UW-tf-dev-1.57.8/Simba_UW_tf_dev.egg-info/top_level.txt
--rw-rw-r--   0 simon      (501) staff       (20)        1 2023-04-27 19:37:19.000000 Simba-UW-tf-dev-1.57.8/Simba_UW_tf_dev.egg-info/dependency_links.txt
--rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.57.8/LICENSE.md
--rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.57.8/MANIFEST.in
--rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.57.8/README.md
--rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-04-27 19:37:01.000000 Simba-UW-tf-dev-1.57.8/setup.py
--rw-r--r--   0 simon      (501) staff       (20)       38 2023-04-27 19:37:20.000000 Simba-UW-tf-dev-1.57.8/setup.cfg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/
+-rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/PKG-INFO
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/simba/
+-rw-r--r--   0 simon      (501) staff       (20)    41423 2023-04-27 12:44:27.000000 Simba-UW-tf-dev-1.57.9/simba/video_processing.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/simba/blob_storage/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-21 20:39:46.000000 Simba-UW-tf-dev-1.57.9/simba/blob_storage/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    11569 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/interpolate_smooth.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/simba/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)    11932 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/unsupervised/dbcv_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3385 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/unsupervised/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-23 19:55:32.000000 Simba-UW-tf-dev-1.57.9/simba/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7442 2023-04-28 00:11:10.000000 Simba-UW-tf-dev-1.57.9/simba/unsupervised/dataset_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     4805 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/unsupervised/grid_search_visualizers.py
+-rw-r--r--   0 simon      (501) staff       (20)     6679 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/unsupervised/data_extractor.py
+-rw-r--r--   0 simon      (501) staff       (20)     9937 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/unsupervised/ui.py
+-rw-r--r--   0 simon      (501) staff       (20)     8367 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/unsupervised/umap_embedder.py
+-rw-r--r--   0 simon      (501) staff       (20)    41506 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/unsupervised/pop_up_classes.py
+-rw-r--r--   0 simon      (501) staff       (20)     2348 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/unsupervised/bout_aggregator.py
+-rw-r--r--   0 simon      (501) staff       (20)    18474 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/unsupervised/cluster_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     2188 2023-04-18 23:25:29.000000 Simba-UW-tf-dev-1.57.9/simba/unsupervised/data_map.yaml
+-rw-r--r--   0 simon      (501) staff       (20)     8331 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/unsupervised/hdbscan_clusterer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3931 2023-04-19 18:21:47.000000 Simba-UW-tf-dev-1.57.9/simba/unsupervised/tsne.py
+-rw-r--r--   0 simon      (501) staff       (20)     5901 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/unsupervised/cluster_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    19750 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/enums.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/simba/bounding_box_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/bounding_box_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     6790 2023-04-28 00:15:19.000000 Simba-UW-tf-dev-1.57.9/simba/bounding_box_tools/agg_boundary_stats.py
+-rw-r--r--   0 simon      (501) staff       (20)    23569 2023-04-28 00:19:41.000000 Simba-UW-tf-dev-1.57.9/simba/bounding_box_tools/boundary_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)     8515 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/bounding_box_tools/boundary_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     6067 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/bounding_box_tools/find_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    11228 2023-04-28 00:28:29.000000 Simba-UW-tf-dev-1.57.9/simba/bounding_box_tools/visualize_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    32772 2023-04-26 18:25:34.000000 Simba-UW-tf-dev-1.57.9/simba/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/
+-rw-r--r--   0 simon      (501) staff       (20)    42279 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/feature_extractor_14bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    21408 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/feature_extractor_7bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/doctests.py
+-rw-r--r--   0 simon      (501) staff       (20)    23850 2023-04-17 18:48:40.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/read_in_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     2460 2023-04-22 18:02:29.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/peaks.py
+-rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/fish_feature_extractor_2022.py
+-rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/convex_hull_scratch_1.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    21398 2023-04-16 17:03:37.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     7127 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/egocentrical_aligner.py
+-rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/count_values_in_range.py
+-rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/graph_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/termite_rois.csv
+-rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/mutual_exclusive.py
+-rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/video_color.py
+-rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/graph_3d_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/video_rotator.py
+-rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/add_probability_cnt_features.py
+-rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/make_splash.py
+-rw-r--r--   0 simon      (501) staff       (20)     1658 2023-04-22 19:16:28.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/time_stamp_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-15 19:24:18.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/video_rotator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    30677 2023-04-27 01:57:28.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
+-rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/convex_hull_scratch_2.py
+-rw-r--r--   0 simon      (501) staff       (20)    27739 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/feature_extractor_8bps_2_animals.py
+-rw-r--r--   0 simon      (501) staff       (20)    10244 2023-04-25 21:03:39.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     2338 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/perimeter_jit.py
+-rw-r--r--   0 simon      (501) staff       (20)    10793 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/feature_subsets.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/__pycache__/
+-rw-r--r--   0 simon      (501) staff       (20)      905 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)   238196 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    69038 2023-04-04 11:32:25.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)   238298 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    69338 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc
+-rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     2179 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     8282 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/feature_extractor_user_defined.py
+-rw-r--r--   0 simon      (501) staff       (20)    46225 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/feature_extractor_16bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    27389 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/feature_extractor_9bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    23905 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/feature_extractor_8bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16825 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/feature_extractor_4bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/.idea/features_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/.idea/.gitignore
+-rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/.idea/.name
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/feature_extractors/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)    15351 2023-04-06 14:48:36.000000 Simba-UW-tf-dev-1.57.9/simba/requirements.txt
+-rw-r--r--   0 simon      (501) staff       (20)     4814 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.57.9/simba/severity_processor.py
+-rw-r--r--   0 simon      (501) staff       (20)     5942 2023-04-25 15:16:24.000000 Simba-UW-tf-dev-1.57.9/simba/user_pose_config_creator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/simba/mixins/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:26:03.000000 Simba-UW-tf-dev-1.57.9/simba/mixins/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    40274 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/mixins/pop_up_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    28905 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/mixins/config_reader.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/simba/mixins/__pycache__/
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-25 20:46:51.000000 Simba-UW-tf-dev-1.57.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-24 19:51:34.000000 Simba-UW-tf-dev-1.57.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-24 19:51:34.000000 Simba-UW-tf-dev-1.57.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-25 20:46:51.000000 Simba-UW-tf-dev-1.57.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-24 19:06:57.000000 Simba-UW-tf-dev-1.57.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-24 19:06:57.000000 Simba-UW-tf-dev-1.57.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    22108 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/mixins/feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    54715 2023-04-28 00:26:29.000000 Simba-UW-tf-dev-1.57.9/simba/mixins/plotting_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     6093 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/mixins/unsupervised_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    55244 2023-04-27 01:40:24.000000 Simba-UW-tf-dev-1.57.9/simba/mixins/train_model_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    33917 2023-04-27 16:59:00.000000 Simba-UW-tf-dev-1.57.9/simba/machine_model_settings_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5223 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/remove_keypoints_in_pose.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/simba/third_party_label_appenders/
+-rw-r--r--   0 simon      (501) staff       (20)     6228 2023-04-26 18:27:58.000000 Simba-UW-tf-dev-1.57.9/simba/third_party_label_appenders/deepethogram_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     9945 2023-04-25 01:50:43.000000 Simba-UW-tf-dev-1.57.9/simba/third_party_label_appenders/BORIS_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     9063 2023-04-25 01:50:43.000000 Simba-UW-tf-dev-1.57.9/simba/third_party_label_appenders/observer_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16888 2023-04-25 14:58:07.000000 Simba-UW-tf-dev-1.57.9/simba/third_party_label_appenders/tools.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.57.9/simba/third_party_label_appenders/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18242 2023-04-25 01:50:43.000000 Simba-UW-tf-dev-1.57.9/simba/third_party_label_appenders/third_party_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     8173 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.57.9/simba/third_party_label_appenders/ethovision_import.py
+-rw-r--r--   0 simon      (501) staff       (20)     6859 2023-04-25 01:50:43.000000 Simba-UW-tf-dev-1.57.9/simba/third_party_label_appenders/BENTO_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     5331 2023-04-25 01:50:43.000000 Simba-UW-tf-dev-1.57.9/simba/third_party_label_appenders/solomon_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     7168 2023-04-25 11:55:36.000000 Simba-UW-tf-dev-1.57.9/simba/multi_cropper.py
+-rw-r--r--   0 simon      (501) staff       (20)    12659 2023-04-28 00:12:04.000000 Simba-UW-tf-dev-1.57.9/simba/FSTTC_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12570 2023-04-25 15:08:48.000000 Simba-UW-tf-dev-1.57.9/simba/create_project_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    13056 2023-04-26 18:37:46.000000 Simba-UW-tf-dev-1.57.9/simba/video_info_table.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/simba/cue_light_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:25:58.000000 Simba-UW-tf-dev-1.57.9/simba/cue_light_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7588 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/cue_light_tools/cue_light_clf_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)    12048 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/cue_light_tools/cue_light_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    17725 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/cue_light_tools/cue_light_menues.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/cue_light_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     1690 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/cue_light_tools/cue_light_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    15283 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/cue_light_tools/cue_light_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    11952 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/cue_light_tools/cue_light_movement_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     2833 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/extract_frames_fast.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/simba/utils/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 20:15:03.000000 Simba-UW-tf-dev-1.57.9/simba/utils/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7365 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/utils/warnings.py
+-rw-r--r--   0 simon      (501) staff       (20)     5592 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/utils/checks.py
+-rw-r--r--   0 simon      (501) staff       (20)    33757 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/utils/read_write.py
+-rw-r--r--   0 simon      (501) staff       (20)     7028 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/utils/lookups.py
+-rw-r--r--   0 simon      (501) staff       (20)    14660 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/utils/errors.py
+-rw-r--r--   0 simon      (501) staff       (20)    14092 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/utils/data.py
+-rw-r--r--   0 simon      (501) staff       (20)     1567 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/utils/printing.py
+-rw-r--r--   0 simon      (501) staff       (20)    20580 2023-04-25 15:08:48.000000 Simba-UW-tf-dev-1.57.9/simba/labelling_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     9371 2023-04-26 20:31:09.000000 Simba-UW-tf-dev-1.57.9/simba/timebins_movement_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/SimBA_dash_app.py
+-rw-r--r--   0 simon      (501) staff       (20)     7421 2023-04-27 02:02:22.000000 Simba-UW-tf-dev-1.57.9/simba/timebins_clf_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     8215 2023-04-25 11:06:37.000000 Simba-UW-tf-dev-1.57.9/simba/calculate_px_dist.py
+-rw-r--r--   0 simon      (501) staff       (20)     6411 2023-04-25 18:52:57.000000 Simba-UW-tf-dev-1.57.9/simba/movement_processor.py
+-rw-r--r--   0 simon      (501) staff       (20)     2904 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/pybursts.py
+-rw-r--r--   0 simon      (501) staff       (20)     5617 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.57.9/simba/reverse_2_animal_tracking.py
+-rw-r--r--   0 simon      (501) staff       (20)     9654 2023-04-25 11:22:07.000000 Simba-UW-tf-dev-1.57.9/simba/Directing_animals_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3170 2023-04-25 13:13:10.000000 Simba-UW-tf-dev-1.57.9/simba/Validate_model_one_video_run_clf.py
+-rw-r--r--   0 simon      (501) staff       (20)    10861 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.57.9/simba/tkinter_functions.py
+-rw-r--r--   0 simon      (501) staff       (20)    13112 2023-04-26 21:09:13.000000 Simba-UW-tf-dev-1.57.9/simba/setting_menu.py
+-rw-r--r--   0 simon      (501) staff       (20)     6317 2023-04-25 18:03:32.000000 Simba-UW-tf-dev-1.57.9/simba/interpolate_pose.py
+-rw-r--r--   0 simon      (501) staff       (20)     3530 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.57.9/simba/run_inference.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/simba/plotting/
+-rw-r--r--   0 simon      (501) staff       (20)     9137 2023-04-26 02:10:59.000000 Simba-UW-tf-dev-1.57.9/simba/plotting/gantt_creator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/simba/plotting/tools/
+-rw-r--r--   0 simon      (501) staff       (20)     5388 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/plotting/tools/tkinter_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    13231 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.57.9/simba/plotting/ROI_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-25 23:35:57.000000 Simba-UW-tf-dev-1.57.9/simba/plotting/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    14630 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/plotting/shap_agg_stats_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10167 2023-04-26 15:08:19.000000 Simba-UW-tf-dev-1.57.9/simba/plotting/gantt_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15975 2023-04-26 13:44:02.000000 Simba-UW-tf-dev-1.57.9/simba/plotting/heat_mapper_clf_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     8557 2023-04-26 12:36:28.000000 Simba-UW-tf-dev-1.57.9/simba/plotting/probability_plot_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12301 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/plotting/plot_clf_results.py
+-rw-r--r--   0 simon      (501) staff       (20)    16586 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/plotting/plot_clf_results_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15885 2023-04-26 12:47:24.000000 Simba-UW-tf-dev-1.57.9/simba/plotting/ROI_feature_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12733 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.57.9/simba/plotting/heat_mapper_location.py
+-rw-r--r--   0 simon      (501) staff       (20)    12507 2023-04-26 12:41:15.000000 Simba-UW-tf-dev-1.57.9/simba/plotting/probability_plot_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     5226 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.57.9/simba/plotting/interactive_probability_grapher.py
+-rw-r--r--   0 simon      (501) staff       (20)     5748 2023-04-26 11:37:28.000000 Simba-UW-tf-dev-1.57.9/simba/plotting/plot_pose_in_dir.py
+-rw-r--r--   0 simon      (501) staff       (20)    12771 2023-04-26 14:16:42.000000 Simba-UW-tf-dev-1.57.9/simba/plotting/single_run_model_validation_video.py
+-rw-r--r--   0 simon      (501) staff       (20)    12236 2023-04-27 12:57:18.000000 Simba-UW-tf-dev-1.57.9/simba/plotting/frame_mergerer_ffmpeg.py
+-rw-r--r--   0 simon      (501) staff       (20)     7887 2023-04-26 13:22:21.000000 Simba-UW-tf-dev-1.57.9/simba/plotting/Directing_animals_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    11204 2023-04-27 12:38:21.000000 Simba-UW-tf-dev-1.57.9/simba/plotting/clf_validator.py
+-rw-r--r--   0 simon      (501) staff       (20)    16708 2023-04-26 15:09:39.000000 Simba-UW-tf-dev-1.57.9/simba/plotting/path_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    11324 2023-04-26 13:09:33.000000 Simba-UW-tf-dev-1.57.9/simba/plotting/ROI_feature_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     9876 2023-04-25 23:33:34.000000 Simba-UW-tf-dev-1.57.9/simba/plotting/data_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    12920 2023-04-26 10:57:46.000000 Simba-UW-tf-dev-1.57.9/simba/plotting/path_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     8493 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.57.9/simba/plotting/ez_lineplot.py
+-rw-r--r--   0 simon      (501) staff       (20)    11482 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.57.9/simba/plotting/distance_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15604 2023-04-26 13:46:25.000000 Simba-UW-tf-dev-1.57.9/simba/plotting/ROI_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13127 2023-04-25 13:50:19.000000 Simba-UW-tf-dev-1.57.9/simba/plotting/heat_mapper_clf.py
+-rw-r--r--   0 simon      (501) staff       (20)     8973 2023-04-26 00:37:26.000000 Simba-UW-tf-dev-1.57.9/simba/plotting/distance_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13560 2023-04-27 18:03:45.000000 Simba-UW-tf-dev-1.57.9/simba/plotting/single_run_model_validation_video_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     9731 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.57.9/simba/plotting/Directing_animals_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16315 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.57.9/simba/plotting/heat_mapper_location_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/run_dash_tkinter.py
+-rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/dash_app.py
+-rw-r--r--   0 simon      (501) staff       (20)     2907 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/extract_annotation_frames.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/simba/roi_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6501 2023-04-25 18:50:18.000000 Simba-UW-tf-dev-1.57.9/simba/roi_tools/ROI_time_bin_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     1753 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.57.9/simba/roi_tools/ROI_movement_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-20 12:47:56.000000 Simba-UW-tf-dev-1.57.9/simba/roi_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    43128 2023-04-26 19:19:44.000000 Simba-UW-tf-dev-1.57.9/simba/roi_tools/ROI_define.py
+-rw-r--r--   0 simon      (501) staff       (20)     3402 2023-04-26 19:25:50.000000 Simba-UW-tf-dev-1.57.9/simba/roi_tools/ROI_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/roi_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    19690 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.57.9/simba/roi_tools/ROI_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    11332 2023-04-26 21:13:20.000000 Simba-UW-tf-dev-1.57.9/simba/roi_tools/ROI_feature_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3651 2023-04-26 19:22:41.000000 Simba-UW-tf-dev-1.57.9/simba/roi_tools/ROI_multiply.py
+-rw-r--r--   0 simon      (501) staff       (20)      961 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/roi_tools/ROI_size_calculations.py
+-rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/roi_tools/ROI_zoom.py
+-rw-r--r--   0 simon      (501) staff       (20)    11384 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.57.9/simba/roi_tools/ROI_directing_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/roi_tools/ROI_move_shape.py
+-rw-r--r--   0 simon      (501) staff       (20)     5073 2023-04-25 14:55:41.000000 Simba-UW-tf-dev-1.57.9/simba/roi_tools/ROI_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)    13793 2023-04-26 14:59:42.000000 Simba-UW-tf-dev-1.57.9/simba/roi_tools/ROI_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    22685 2023-04-25 14:55:41.000000 Simba-UW-tf-dev-1.57.9/simba/roi_tools/ROI_image.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/simba/pose_importers/
+-rw-r--r--   0 simon      (501) staff       (20)     2464 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.57.9/simba/pose_importers/read_DANNCE_mat.py
+-rw-r--r--   0 simon      (501) staff       (20)    21991 2023-04-27 15:50:07.000000 Simba-UW-tf-dev-1.57.9/simba/pose_importers/sleap_importer_slp.py
+-rw-r--r--   0 simon      (501) staff       (20)    23507 2023-04-27 15:45:27.000000 Simba-UW-tf-dev-1.57.9/simba/pose_importers/sleap_importer_h5.py
+-rw-r--r--   0 simon      (501) staff       (20)    23579 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.57.9/simba/pose_importers/dlc_multi_animal_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-25 16:49:14.000000 Simba-UW-tf-dev-1.57.9/simba/pose_importers/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    21003 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/pose_importers/sleap_importer_csv.py
+-rw-r--r--   0 simon      (501) staff       (20)     7761 2023-04-25 18:26:26.000000 Simba-UW-tf-dev-1.57.9/simba/pose_importers/import_mars.py
+-rw-r--r--   0 simon      (501) staff       (20)     6922 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.57.9/simba/pose_importers/dlc_importer_csv.py
+-rw-r--r--   0 simon      (501) staff       (20)     8100 2023-04-27 21:09:15.000000 Simba-UW-tf-dev-1.57.9/simba/pose_importers/trk_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)   238321 2023-04-28 00:09:50.000000 Simba-UW-tf-dev-1.57.9/simba/pop_up_classes.py
+-rw-r--r--   0 simon      (501) staff       (20)     4695 2023-04-26 18:17:53.000000 Simba-UW-tf-dev-1.57.9/simba/extract_seqframes.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/simba/pose_configurations/
+-rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.57.9/simba/pose_configurations/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/simba/pose_configurations/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.57.9/simba/pose_configurations/bp_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-10 12:22:28.000000 Simba-UW-tf-dev-1.57.9/simba/pose_configurations/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/simba/pose_configurations/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       24 2023-03-20 15:55:45.000000 Simba-UW-tf-dev-1.57.9/simba/pose_configurations/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.57.9/simba/pose_configurations/no_animals/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/simba/pose_configurations/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.57.9/simba/pose_configurations/configuration_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)      267 2023-03-20 15:55:45.000000 Simba-UW-tf-dev-1.57.9/simba/pose_configurations/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/simba/pose_configurations/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.57.9/simba/pose_configurations/schematics/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/pose_configurations/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.57.9/simba/pose_configurations/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/pose_configurations/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.57.9/simba/pose_configurations/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.57.9/simba/pose_configurations/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/pose_configurations/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/pose_configurations/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/pose_configurations/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/pose_configurations/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/pose_configurations/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/pose_configurations/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/pose_configurations/schematics/1.png
+-rw-r--r--   0 simon      (501) staff       (20)     7171 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.57.9/simba/get_coordinates_tools_v2.py
+-rw-r--r--   0 simon      (501) staff       (20)    15761 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/pup_retrieval_protocol.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/simba/outlier_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     7427 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/outlier_tools/outlier_corrector_movement.py
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-15 17:05:05.000000 Simba-UW-tf-dev-1.57.9/simba/outlier_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/outlier_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8191 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/outlier_tools/outlier_corrector_location.py
+-rw-r--r--   0 simon      (501) staff       (20)     2706 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/outlier_tools/skip_outlier_correction.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/simba/outlier_tools/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/outlier_tools/.idea/outlier_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/outlier_tools/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/simba/outlier_tools/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/simba/outlier_tools/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/outlier_tools/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/outlier_tools/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/outlier_tools/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/outlier_tools/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)     2613 2023-04-25 15:16:24.000000 Simba-UW-tf-dev-1.57.9/simba/pose_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)    18234 2023-04-27 17:03:57.000000 Simba-UW-tf-dev-1.57.9/simba/train_mutiple_models.py
+-rw-r--r--   0 simon      (501) staff       (20)    63957 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.57.9/simba/SimBA.py
+-rw-r--r--   0 simon      (501) staff       (20)    26559 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.57.9/simba/labelling_advanced_interface.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/simba/assets/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/simba/assets/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/assets/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/assets/unsupervised/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/assets/unsupervised/features.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/simba/assets/shap/
+-rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/assets/shap/down_arrow.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/assets/shap/intruder_shape.jpg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/simba/assets/shap/feature_categories/
+-rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
+-rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/assets/shap/feature_categories/shap_feature_categories.csv
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-04-10 20:37:13.000000 Simba-UW-tf-dev-1.57.9/simba/assets/shap/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/assets/shap/resident_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/assets/shap/resident_intruder_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/assets/shap/animal_distances.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/assets/shap/baseline_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/assets/shap/ubuntu.regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/assets/shap/side_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/assets/shap/UbuntuMono-Regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/assets/shap/side_scale_5.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/assets/shap/intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/assets/shap/resident_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/assets/shap/color_bar.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/assets/shap/resident_intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)    16388 2023-04-25 19:14:34.000000 Simba-UW-tf-dev-1.57.9/simba/assets/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/simba/assets/lookups/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/assets/lookups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/assets/lookups/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)     2987 2023-04-25 20:39:03.000000 Simba-UW-tf-dev-1.57.9/simba/assets/lookups/feature_extraction_headers.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/assets/lookups/features.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/assets/lookups/unsupervised_example_x.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/simba/assets/stl/
+-rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/assets/stl/operant_tray.stl
+-rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/assets/stl/operant_lever.stl
+-rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/assets/stl/operant_walls.stl
+-rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/assets/stl/grid_floor.stl
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/simba/assets/img/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.57.9/simba/assets/img/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/assets/img/about_me.png
+-rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.57.9/simba/assets/img/splash.mp4
+-rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.57.9/simba/assets/img/bg_2.png
+-rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/assets/img/splash.pptx
+-rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.57.9/simba/assets/img/bg.png
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/assets/UbuntuMono-Regular.ttf
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/
+-rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/factory.png
+-rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/cluster.png
+-rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/load.png
+-rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/gif.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/pose.png
+-rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/features.png
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/.DS_Store
+-rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/settings.png
+-rw-r--r--   0 simon      (501) staff       (20)     2090 2023-04-22 15:14:17.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/stopwatch.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/link.png
+-rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/dash_simba.css
+-rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/documentation.png
+-rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/fps.png
+-rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/dimensionality_reduction.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/roi.png
+-rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/superimpose.png
+-rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/label.png
+-rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/change.png
+-rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/crop.png
+-rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/rotate.png
+-rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/path.png
+-rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/clip.png
+-rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/restart.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/calipher.png
+-rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/add_on.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/create.png
+-rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/SimBA_logo.ico
+-rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/print.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/clf.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/concat_icons/
+-rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/concat_icons/mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/concat_icons/vertical.png
+-rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/concat_icons/horizontal.png
+-rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/concat_icons/mixed_mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/merge.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/clean.png
+-rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/clf_2.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/visualize.png
+-rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/concat.png
+-rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/boris.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/frames.png
+-rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/video.png
+-rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/sample.png
+-rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/metrics.png
+-rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/grey.png
+-rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/exit.png
+-rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/outlier.png
+-rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/clahe.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/trash.png
+-rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/about.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/convert.png
+-rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/SimBA_logo.icns
+-rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/reorganize.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/browse.png
+-rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/SimBA_logo.png
+-rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/ethovision.png
+-rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.57.9/simba/assets/icons/close.png
+-rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/assets/dash_simba_base.css
+-rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/assets/TheGoldenLab.PNG
+-rw-r--r--   0 simon      (501) staff       (20)     9478 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.57.9/simba/read_config_unit_tests.py
+-rw-r--r--   0 simon      (501) staff       (20)    11645 2023-04-25 15:16:24.000000 Simba-UW-tf-dev-1.57.9/simba/project_config_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    19000 2023-04-26 18:08:54.000000 Simba-UW-tf-dev-1.57.9/simba/train_single_model.py
+-rw-r--r--   0 simon      (501) staff       (20)     6308 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.57.9/simba/create_clf_log.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/simba/batch_process_videos/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-17 14:43:38.000000 Simba-UW-tf-dev-1.57.9/simba/batch_process_videos/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    24639 2023-04-25 13:26:59.000000 Simba-UW-tf-dev-1.57.9/simba/batch_process_videos/batch_process_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.9/simba/batch_process_videos/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    11106 2023-04-25 13:26:59.000000 Simba-UW-tf-dev-1.57.9/simba/batch_process_videos/batch_process_create_ffmpeg_commands.py
+-rw-r--r--   0 simon      (501) staff       (20)     9520 2023-04-25 19:02:08.000000 Simba-UW-tf-dev-1.57.9/simba/Kleinberg_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8341 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.57.9/simba/reorganize_keypoint_in_pose.py
+-rw-r--r--   0 simon      (501) staff       (20)      165 2023-03-25 11:18:21.000000 Simba-UW-tf-dev-1.57.9/simba/~$features.pptx
+-rw-r--r--   0 simon      (501) staff       (20)     6543 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.57.9/simba/play_annotation_video.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/Simba_UW_tf_dev.egg-info/
+-rw-rw-r--   0 simon      (501) staff       (20)      579 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/Simba_UW_tf_dev.egg-info/PKG-INFO
+-rw-rw-r--   0 simon      (501) staff       (20)    13977 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/Simba_UW_tf_dev.egg-info/SOURCES.txt
+-rw-rw-r--   0 simon      (501) staff       (20)       44 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/Simba_UW_tf_dev.egg-info/entry_points.txt
+-rw-rw-r--   0 simon      (501) staff       (20)      639 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/Simba_UW_tf_dev.egg-info/requires.txt
+-rw-rw-r--   0 simon      (501) staff       (20)        6 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/Simba_UW_tf_dev.egg-info/top_level.txt
+-rw-rw-r--   0 simon      (501) staff       (20)        1 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/Simba_UW_tf_dev.egg-info/dependency_links.txt
+-rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.57.9/LICENSE.md
+-rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.57.9/MANIFEST.in
+-rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.57.9/README.md
+-rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-04-28 00:33:54.000000 Simba-UW-tf-dev-1.57.9/setup.py
+-rw-r--r--   0 simon      (501) staff       (20)       38 2023-04-28 00:34:08.000000 Simba-UW-tf-dev-1.57.9/setup.cfg
```

### Comparing `Simba-UW-tf-dev-1.57.8/PKG-INFO` & `Simba-UW-tf-dev-1.57.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.57.8
+Version: 1.57.9
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/video_processing.py` & `Simba-UW-tf-dev-1.57.9/simba/video_processing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/blob_storage/.DS_Store` & `Simba-UW-tf-dev-1.57.9/simba/blob_storage/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/interpolate_smooth.py` & `Simba-UW-tf-dev-1.57.9/simba/interpolate_smooth.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+__author__ = "Simon Nilsson"
+
 from scipy.signal import savgol_filter
 import glob, os
 import numpy as np
 import pandas as pd
 import shutil
 from simba.mixins.config_reader import ConfigReader
 from simba.utils.printing import stdout_success, SimbaTimer
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/unsupervised/dbcv_calculator.py` & `Simba-UW-tf-dev-1.57.9/simba/unsupervised/dbcv_calculator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+__author__ = "Simon Nilsson"
+
 import os.path
 import pandas as pd
 import numpy as np
 from numba import jit, prange
 from numba.typed import List
 from scipy.sparse.csgraph import minimum_spanning_tree
 from scipy.sparse import csgraph
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/unsupervised/enums.py` & `Simba-UW-tf-dev-1.57.9/simba/unsupervised/enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+__author__ = "Simon Nilsson"
+
+
 from enum import Enum
 import numpy as np
 
 class Unsupervised(Enum):
     ALL_FEATURES_EX_POSE = 'ALL FEATURES (EXCLUDING POSE)'
     DATA_SLICE_SELECTION = 'data_slice'
     CLF_SLICE_SELECTION = 'clf_slice'
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.57.9/simba/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/unsupervised/dataset_creator.py` & `Simba-UW-tf-dev-1.57.9/simba/unsupervised/dataset_creator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+__author__ = "Simon Nilsson"
+
 import os
 import pandas as pd
 import numpy as np
 from simba.unsupervised.bout_aggregator import bout_aggregator
 from simba.unsupervised.enums import Unsupervised
 from simba.mixins.config_reader import ConfigReader
 from simba.mixins.unsupervised_mixin import UnsupervisedMixin
@@ -94,18 +96,18 @@
         if len(self.bouts_x_df) == 0:
             raise NoDataError(msg='The data contains zero frames after the chosen slice setting')
         results = {}
         results['DATETIME'] = self.datetime
         results['AGGREGATION_METHOD'] = self.settings[Unsupervised.BOUT_AGGREGATION_TYPE.value]
         results['MIN_BOUT'] = self.settings[Unsupervised.MIN_BOUT_LENGTH.value]
         results['FEATURE_NAMES'] = self.feature_names
-        results['FRAME_FEATURES'] = self.raw_x_df.set_index([Unsupervised.VIDEO.value, Unsupervised.FRAME.value]).astype(np.float16)
-        results['FRAME_POSE'] = self.raw_bp_df.set_index([Unsupervised.VIDEO.value, Unsupervised.FRAME.value]).astype(np.float16)
-        results['FRAME_TARGETS'] = self.raw_y_df.set_index([Unsupervised.VIDEO.value, Unsupervised.FRAME.value]).astype(np.float16)
-        results['BOUTS_FEATURES'] = self.bouts_x_df.set_index([Unsupervised.VIDEO.value, Unsupervised.START_FRAME.value, Unsupervised.END_FRAME.value]).astype(np.float16)
+        results['FRAME_FEATURES'] = self.raw_x_df.set_index([Unsupervised.VIDEO.value, Unsupervised.FRAME.value]).astype(np.float32)
+        results['FRAME_POSE'] = self.raw_bp_df.set_index([Unsupervised.VIDEO.value, Unsupervised.FRAME.value]).astype(np.float32)
+        results['FRAME_TARGETS'] = self.raw_y_df.set_index([Unsupervised.VIDEO.value, Unsupervised.FRAME.value]).astype(np.float32)
+        results['BOUTS_FEATURES'] = self.bouts_x_df.set_index([Unsupervised.VIDEO.value, Unsupervised.START_FRAME.value, Unsupervised.END_FRAME.value]).astype(np.float32)
         results['BOUTS_TARGETS'] = self.bouts_y_df
 
         self.write_pickle(data=results, save_path=self.save_path)
         self.timer.stop_timer()
         self.__aggregate_dataset_stats()
         stdout_success(msg=f'Dataset for unsupervised learning saved at {self.save_path}', elapsed_time=self.timer.elapsed_time_str)
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/unsupervised/grid_search_visualizers.py` & `Simba-UW-tf-dev-1.57.9/simba/unsupervised/grid_search_visualizers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+__author__ = "Simon Nilsson"
+
 import numpy as np
 import glob, os
 import pandas as pd
 import seaborn as sns
 import matplotlib.pyplot as plt
 from simba.unsupervised.enums import Clustering, Unsupervised
 from simba.mixins.unsupervised_mixin import UnsupervisedMixin
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/unsupervised/data_extractor.py` & `Simba-UW-tf-dev-1.57.9/simba/unsupervised/data_extractor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+__author__ = "Simon Nilsson"
+
 import os
 import json
 import pandas as pd
 from simba.mixins.unsupervised_mixin import UnsupervisedMixin
 from simba.mixins.config_reader import ConfigReader
 from simba.unsupervised.enums import Unsupervised, Clustering
 from simba.utils.checks import check_if_dir_exists, check_file_exist_and_readable
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/unsupervised/ui.py` & `Simba-UW-tf-dev-1.57.9/simba/unsupervised/ui.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+__author__ = "Simon Nilsson"
+
 from tkinter import *
 from simba.tkinter_functions import (hxtScrollbar,
                                      Entry_Box,
                                      DropDownMenu,
                                      FileSelect)
 import tkinter.ttk as ttk
 from simba.enums import Formats
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/unsupervised/umap_embedder.py` & `Simba-UW-tf-dev-1.57.9/simba/unsupervised/umap_embedder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+__author__ = "Simon Nilsson"
+
 import os
 import random
 from copy import deepcopy
 from simba.mixins.unsupervised_mixin import UnsupervisedMixin
 from simba.unsupervised.enums import Unsupervised
 from simba.utils.printing import stdout_success, SimbaTimer
 from simba.utils.checks import check_file_exist_and_readable
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/unsupervised/pop_up_classes.py` & `Simba-UW-tf-dev-1.57.9/simba/unsupervised/pop_up_classes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+__author__ = "Simon Nilsson"
+
 import glob
 from tkinter import *
 import numpy as np
 
 from simba.tkinter_functions import (FolderSelect,
                                      DropDownMenu,
                                      FileSelect,
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/unsupervised/bout_aggregator.py` & `Simba-UW-tf-dev-1.57.9/simba/unsupervised/bout_aggregator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+__author__ = "Simon Nilsson"
+
+
 import pandas as pd
 from joblib.externals.loky import get_reusable_executor
 from joblib import Parallel, delayed
 from simba.utils.read_write import read_video_info
 from simba.utils.data import detect_bouts
 
 def bout_aggregator(data: pd.DataFrame,
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/unsupervised/cluster_statistics.py` & `Simba-UW-tf-dev-1.57.9/simba/unsupervised/cluster_statistics.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+__author__ = "Simon Nilsson"
+
+
 import os
 import numpy as np
 import pandas as pd
 from copy import deepcopy
 from scipy.stats import f_oneway
 import shap
 from statsmodels.stats.multicomp import pairwise_tukeyhsd
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/unsupervised/data_map.yaml` & `Simba-UW-tf-dev-1.57.9/simba/unsupervised/data_map.yaml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/unsupervised/hdbscan_clusterer.py` & `Simba-UW-tf-dev-1.57.9/simba/unsupervised/hdbscan_clusterer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+__author__ = "Simon Nilsson"
+
 try:
     from cuml.cluster.hdbscan import HDBSCAN
     from cuml.cluster import hdbscan
     gpu_flag = True
 except ModuleNotFoundError:
     from hdbscan import HDBSCAN
     import hdbscan
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/unsupervised/tsne.py` & `Simba-UW-tf-dev-1.57.9/simba/unsupervised/tsne.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/unsupervised/cluster_visualizer.py` & `Simba-UW-tf-dev-1.57.9/simba/unsupervised/cluster_visualizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+__author__ = "Simon Nilsson"
+
 import pandas as pd
 import numpy as np
 import os
 import cv2
 
 from simba.utils.checks import check_file_exist_and_readable
 from simba.utils.read_write import find_all_videos_in_directory, get_video_meta_data
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/enums.py` & `Simba-UW-tf-dev-1.57.9/simba/enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+__author__ = "Simon Nilsson"
+
 from enum import Enum
 import pkg_resources
 from pathlib import Path
 import cv2
 import numpy as np
 
 class ReadConfig(Enum):
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/bounding_box_tools/.DS_Store` & `Simba-UW-tf-dev-1.57.9/simba/bounding_box_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/bounding_box_tools/agg_boundary_stats.py` & `Simba-UW-tf-dev-1.57.9/simba/bounding_box_tools/agg_boundary_stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+__author__ = "Simon Nilsson"
+
 import pandas as pd
 import os, glob
 from simba.utils.read_write import read_df, get_fn_ext
 from simba.utils.printing import stdout_success
 from simba.utils.errors import NotDirectoryError
 from simba.utils.data import detect_bouts, plug_holes_shortest_bout
 from simba.mixins.config_reader import ConfigReader
@@ -50,15 +52,14 @@
         for file_cnt, file_path in enumerate(self.files_found):
             _, self.file_name, ext = get_fn_ext(file_path)
             print(f'Creating aggregate statistics for video {self.file_name}...')
             _, _, fps = self.read_video_info(video_name=self.file_name)
             data_df = read_df(file_path=file_path, file_type=ext[1:])
             if (self.shortest_allowed_interaction_ms / fps) > 0:
                 for column in data_df.columns:
-                    print(column)
                     data_df = plug_holes_shortest_bout(data_df=data_df, clf_name=column, fps=int(fps),shortest_bout=self.shortest_allowed_interaction_ms)
             bouts_df = detect_bouts(data_df=data_df, target_lst=list(data_df.columns), fps=int(fps))
             self.video_results, self.detailed_interactions_results = {}, {}
             if 'INTERACTION TIME (s)' in self.measures:
                 self.video_results['INTERACTION TIME (s)'] = bouts_df.groupby(by='Event')['Bout_time'].sum().to_dict()
             if ('INTERACTION BOUT COUNT' in self.measures):
                 self.video_results['INTERACTION BOUT COUNT'] = bouts_df.groupby(by='Event')['Bout_time'].count().to_dict()
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/bounding_box_tools/boundary_menus.py` & `Simba-UW-tf-dev-1.57.9/simba/bounding_box_tools/boundary_menus.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,24 @@
+__author__ = "Simon Nilsson"
+
 import os, glob
 import pickle
 from tkinter import *
 from simba.bounding_box_tools.find_boundaries import AnimalBoundaryFinder
 from simba.bounding_box_tools.visualize_boundaries import BoundaryVisualizer
 from simba.bounding_box_tools.boundary_statistics import BoundaryStatisticsCalculator
 from simba.bounding_box_tools.agg_boundary_stats import AggBoundaryStatisticsCalculator
 from simba.utils.errors import NoFilesFoundError, NoChoosenMeasurementError
 from simba.enums import Keys, Links
 from simba.mixins.config_reader import ConfigReader
 from simba.mixins.pop_up_mixin import PopUpMixin
 from simba.tkinter_functions import (DropDownMenu,
                                      Entry_Box,
                                      CreateLabelFrameWithIcon)
-from simba.utils.read_write import get_fn_ext
+from simba.utils.read_write import get_fn_ext, find_all_videos_in_project
 from simba.utils.checks import check_int
 from simba.enums import Formats
 from simba.utils.lookups import get_named_colors
 
 class BoundaryMenus(ConfigReader, PopUpMixin):
     """
     Class creating GUI interface for extrapolating bounding boxes from pose-estimation data, and calculating
@@ -117,15 +119,15 @@
         boundary_finder.find_boundaries()
 
     def __launch_visualize_boundaries(self):
         self.anchored_roi_path = os.path.join(self.project_path, 'logs', 'anchored_rois.pickle')
         if not os.path.isfile(self.anchored_roi_path):
             raise NoFilesFoundError(msg='No anchored ROI found in {}.'.format(self.anchored_roi_path))
         with open(self.anchored_roi_path, 'rb') as fp: self.roi_data = pickle.load(fp)
-        videos_in_project = glob.glob(self.video_dir + '/*')
+        videos_in_project = find_all_videos_in_project(videos_dir=self.video_dir)
         videos_with_data = list(self.roi_data.keys())
         if len(videos_in_project) == 0:
             raise NoFilesFoundError(msg='Zero video files found in SimBA project')
         video_names = []
         for file_path in videos_in_project:
             _, name, _ = get_fn_ext(filepath=file_path)
             video_names.append(name)
@@ -309,10 +311,10 @@
 
         agg_stats_calculator = AggBoundaryStatisticsCalculator(config_path=self.config_path,
                                                                measures=measures,
                                                                shortest_allowed_interaction=int(min_bout))
         agg_stats_calculator.run()
         agg_stats_calculator.save()
 
-# test = BoundaryMenus(config_path='/Users/simon/Desktop/envs/troubleshooting/sleap_5_animals/project_folder/project_config.ini')
+# test = BoundaryMenus(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini')
 # test.main_frm.mainloop()
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/bounding_box_tools/boundary_statistics.py` & `Simba-UW-tf-dev-1.57.9/simba/bounding_box_tools/boundary_statistics.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+__author__ = "Simon Nilsson"
+
 import pandas as pd
 import os
 from joblib import Parallel, delayed
 from shapely.geometry import Point
 from copy import deepcopy
 from collections import defaultdict
 from simba.utils.errors import NoFilesFoundError
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/bounding_box_tools/find_boundaries.py` & `Simba-UW-tf-dev-1.57.9/simba/bounding_box_tools/find_boundaries.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+__author__ = "Simon Nilsson"
+
 import os
 import itertools
 import numpy as np
 from shapely.geometry import (Polygon,
                               Point,
                               LineString)
 import shapely.wkt
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/bounding_box_tools/visualize_boundaries.py` & `Simba-UW-tf-dev-1.57.9/simba/bounding_box_tools/visualize_boundaries.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,63 +1,68 @@
+__author__ = "Simon Nilsson"
+
 import pandas as pd
 import numpy as np
 import pickle
 import functools
 import cv2
 import multiprocessing
 from multiprocessing import pool
 import platform
 import os
+
 from simba.utils.errors import NoFilesFoundError
 from simba.mixins.config_reader import ConfigReader
+from simba.mixins.plotting_mixin import PlottingMixin
 from simba.utils.read_write import (read_df,
                                     get_fn_ext,
                                     get_video_meta_data,
                                     concatenate_videos_in_folder)
 from simba.utils.checks import check_file_exist_and_readable
 from simba.utils.printing import stdout_success
+#
+# def _image_creator(frm_range: list,
+#                    polygon_data: dict,
+#                    animal_bp_dict: dict,
+#                    data_df: pd.DataFrame or None,
+#                    intersection_data_df: pd.DataFrame or None,
+#                    roi_attributes: dict,
+#                    video_path: str,
+#                    key_points: bool,
+#                    greyscale: bool):
+#
+#     cap, current_frame = cv2.VideoCapture(video_path), frm_range[0]
+#     cap.set(1, frm_range[0])
+#     img_lst = []
+#     while current_frame < frm_range[-1]:
+#         ret, frame = cap.read()
+#         if ret:
+#             if key_points:
+#                 frm_data = data_df.iloc[current_frame]
+#             if greyscale:
+#                 frame = cv2.cvtColor(frame, cv2.COLOR_BGR2GRAY)
+#                 frame = cv2.cvtColor(frame, cv2.COLOR_GRAY2BGR)
+#             for animal_cnt, (animal, animal_data) in enumerate(animal_bp_dict.items()):
+#                 if key_points:
+#                     for bp_cnt, (x_col, y_col) in enumerate(zip(animal_data['X_bps'], animal_data['Y_bps'])):
+#                         cv2.circle(frame, (frm_data[x_col], frm_data[y_col]), 0, roi_attributes[animal]['bbox_clr'], roi_attributes[animal]['keypoint_size'])
+#                 animal_polygon = np.array(list(polygon_data[animal][current_frame].convex_hull.exterior.coords)).astype(int)
+#                 if intersection_data_df is not None:
+#                     intersect = intersection_data_df.loc[current_frame, intersection_data_df.columns.str.startswith(animal)].sum()
+#                     if intersect > 0:
+#                         cv2.polylines(frame, [animal_polygon], 1, roi_attributes[animal]['highlight_clr'], roi_attributes[animal]['highlight_clr_thickness'])
+#                 cv2.polylines(frame, [animal_polygon], 1, roi_attributes[animal]['bbox_clr'], roi_attributes[animal]['bbox_thickness'])
+#             img_lst.append(frame)
+#             current_frame += 1
+#         else:
+#             print('SIMBA WARNING: SimBA tried to grab frame number {} from video {}, but could not find it. The video has {} frames.'.format(str(current_frame), video_path, str(cap.get(cv2.CAP_PROP_FRAME_COUNT))))
+#     return img_lst
 
-def _image_creator(frm_range: list,
-                   polygon_data: dict,
-                   animal_bp_dict: dict,
-                   data_df: pd.DataFrame or None,
-                   intersection_data_df: pd.DataFrame or None,
-                   roi_attributes: dict,
-                   video_path: str,
-                   key_points: bool,
-                   greyscale: bool):
-
-    cap, current_frame = cv2.VideoCapture(video_path), frm_range[0]
-    cap.set(1, frm_range[0])
-    img_lst = []
-    while current_frame < frm_range[-1]:
-        ret, frame = cap.read()
-        if ret:
-            if key_points:
-                frm_data = data_df.iloc[current_frame]
-            if greyscale:
-                frame = cv2.cvtColor(frame, cv2.COLOR_BGR2GRAY)
-                frame = cv2.cvtColor(frame, cv2.COLOR_GRAY2BGR)
-            for animal_cnt, (animal, animal_data) in enumerate(animal_bp_dict.items()):
-                if key_points:
-                    for bp_cnt, (x_col, y_col) in enumerate(zip(animal_data['X_bps'], animal_data['Y_bps'])):
-                        cv2.circle(frame, (frm_data[x_col], frm_data[y_col]), 0, roi_attributes[animal]['bbox_clr'], roi_attributes[animal]['keypoint_size'])
-                animal_polygon = np.array(list(polygon_data[animal][current_frame].convex_hull.exterior.coords)).astype(int)
-                if intersection_data_df is not None:
-                    intersect = intersection_data_df.loc[current_frame, intersection_data_df.columns.str.startswith(animal)].sum()
-                    if intersect > 0:
-                        cv2.polylines(frame, [animal_polygon], 1, roi_attributes[animal]['highlight_clr'], roi_attributes[animal]['highlight_clr_thickness'])
-                cv2.polylines(frame, [animal_polygon], 1, roi_attributes[animal]['bbox_clr'], roi_attributes[animal]['bbox_thickness'])
-            img_lst.append(frame)
-            current_frame += 1
-        else:
-            print('SIMBA WARNING: SimBA tried to grab frame number {} from video {}, but could not find it. The video has {} frames.'.format(str(current_frame), video_path, str(cap.get(cv2.CAP_PROP_FRAME_COUNT))))
-    return img_lst
-
-class BoundaryVisualizer(ConfigReader):
+class BoundaryVisualizer(ConfigReader,
+                         PlottingMixin):
     """
     Class visualizing user-specified animal-anchored ROI boundaries. Results are stored in the
     `project_folder/frames/output/anchored_rois` directory of teh SimBA project
 
     Parameters
     ----------
     config_path: str
@@ -86,14 +91,16 @@
                  video_name: str,
                  include_key_points: bool,
                  greyscale: bool,
                  show_intersections: bool or None,
                  roi_attributes: dict or None):
 
         ConfigReader.__init__(self, config_path=config_path)
+        PlottingMixin.__init__(self)
+
         if platform.system() == "Darwin":
             multiprocessing.set_start_method('spawn', force=True)
         self.polygon_path = os.path.join(self.project_path, 'logs', 'anchored_rois.pickle')
         check_file_exist_and_readable(file_path=self.polygon_path)
         self.video_name, self.include_key_points, self.greyscale, self.roi_attributes = video_name, include_key_points, greyscale, roi_attributes
         self.show_intersections, self.intersection_data_folder = show_intersections, os.path.join(self.project_path, 'csv', 'anchored_roi_data')
         self.intersections_df = None
@@ -141,17 +148,17 @@
                 self.roi_attributes[animal_name]['highlight_clr_thickness'] = 10
 
         self.video_save_path = os.path.join(self.save_parent_dir, self.video_name + '.mp4')
         self.temp_folder = os.path.join(self.save_parent_dir, self.video_name)
         if not os.path.exists(self.temp_folder): os.makedirs(self.temp_folder)
         frame_chunks = [[i, i + chunk_size] for i in range(0, video_meta_data['frame_count'], chunk_size)]
         frame_chunks[-1][-1] = min(frame_chunks[-1][-1], video_meta_data['frame_count'])
-        functools.partial(_image_creator, b=self.data_df)
+        functools.partial(self.bbox_mp, b=self.data_df)
         with pool.Pool(self.cpu_to_use, maxtasksperchild=self.maxtasksperchild) as p:
-            constants = functools.partial(_image_creator,
+            constants = functools.partial(self.bbox_mp,
                                           data_df=self.data_df,
                                           polygon_data=self.polygons[self.video_name],
                                           animal_bp_dict=self.animal_bp_dict,
                                           roi_attributes=self.roi_attributes,
                                           video_path=video_path,
                                           key_points=self.include_key_points,
                                           greyscale=self.greyscale,
@@ -173,7 +180,15 @@
 # boundary_visualizer = BoundaryVisualizer(config_path='/Users/simon/Desktop/envs/troubleshooting/sleap_5_animals/project_folder/project_config.ini',
 #                                          video_name='Testing_Video_3',
 #                                          include_key_points=True,
 #                                          greyscale=True,
 #                                          show_intersections=True,
 #                                          roi_attributes=None)
 # boundary_visualizer.run_visualization()
+
+# boundary_visualizer = BoundaryVisualizer(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini',
+#                                          video_name='Together_3',
+#                                          include_key_points=True,
+#                                          greyscale=True,
+#                                          show_intersections=True,
+#                                          roi_attributes=None)
+# boundary_visualizer.run_visualization()
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/.DS_Store` & `Simba-UW-tf-dev-1.57.9/simba/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/feature_extractors/feature_extractor_14bp.py` & `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/feature_extractor_14bp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+__author__ = "Simon Nilsson"
+
 import os
 import pandas as pd
 from copy import deepcopy
 import numpy as np
 from collections import defaultdict
 import math
 from simba.enums import Formats
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/feature_extractors/feature_extractor_7bp.py` & `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/feature_extractor_7bp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+__author__ = "Simon Nilsson"
+
 import os
 import pandas as pd
 import numpy as np
 from copy import deepcopy
 import math
 from scipy.spatial import ConvexHull
 from collections import defaultdict
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/feature_extractors/misc/doctests.py` & `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/doctests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py` & `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/feature_extractors/misc/read_in_mp.py` & `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/read_in_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/feature_extractors/misc/peaks.py` & `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/peaks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/feature_extractors/misc/fish_feature_extractor_2022.py` & `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/fish_feature_extractor_2022.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/feature_extractors/misc/convex_hull_3_scratch_3.py` & `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/convex_hull_3_scratch_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/feature_extractors/misc/convex_hull_scratch_1.py` & `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/convex_hull_scratch_1.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/feature_extractors/misc/.DS_Store` & `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py` & `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/feature_extractors/misc/egocentrical_aligner.py` & `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/egocentrical_aligner.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/feature_extractors/misc/count_values_in_range.py` & `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/count_values_in_range.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/feature_extractors/misc/graph_creator.py` & `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/graph_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/feature_extractors/misc/termite_rois.csv` & `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/termite_rois.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/feature_extractors/misc/mutual_exclusive.py` & `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/mutual_exclusive.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/feature_extractors/misc/video_color.py` & `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/video_color.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/feature_extractors/misc/graph_3d_plotter.py` & `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/graph_3d_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/feature_extractors/misc/video_rotator.py` & `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/video_rotator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/feature_extractors/misc/add_probability_cnt_features.py` & `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/add_probability_cnt_features.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/feature_extractors/misc/make_splash.py` & `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/make_splash.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/feature_extractors/misc/time_stamp_calculator.py` & `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/time_stamp_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/feature_extractors/misc/video_rotator_mp.py` & `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/video_rotator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py` & `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/feature_extractors/misc/convex_hull_scratch_2.py` & `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/misc/convex_hull_scratch_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/feature_extractors/feature_extractor_8bps_2_animals.py` & `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/feature_extractor_8bps_2_animals.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+__author__ = "Simon Nilsson"
+
 import pandas as pd
 import numpy as np
 from copy import deepcopy
 from collections import defaultdict
 import os
 from simba.mixins.feature_extraction_mixin import FeatureExtractionMixin
 from simba.mixins.config_reader import ConfigReader
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/feature_extractors/.DS_Store` & `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/feature_extractors/perimeter_jit.py` & `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/perimeter_jit.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-### https://stackoverflow.com/questions/74812556/computing-quick-convex-hull-using-numba/74817179#74817179
+__author__ = "Simon Nilsson"
+
+
+### modified from https://stackoverflow.com/questions/74812556/computing-quick-convex-hull-using-numba/74817179#74817179
 
 import numpy as np
 from numba import njit, prange
 from numba.np.extensions import cross2d
 
 @njit('(float64[:,:], int64[:], int64, int64)')
 def process(S, P, a, b):
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/feature_extractors/feature_subsets.py` & `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/feature_subsets.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+__author__ = "Simon Nilsson"
+
+
 import pandas as pd
 import os
 import numpy as np
 from itertools import combinations
 from simba.feature_extractors.perimeter_jit import jitted_hull
 from simba.enums import Formats
 from simba.mixins.config_reader import ConfigReader
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi` & `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc` & `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc` & `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc` & `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc` & `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi` & `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi` & `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/feature_extractors/feature_extractor_user_defined.py` & `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/feature_extractor_user_defined.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+__author__ = "Simon Nilsson"
+
+
 import os
 import pandas as pd
 import numpy as np
 from itertools import product
 from simba.mixins.feature_extraction_mixin import FeatureExtractionMixin
 from simba.mixins.config_reader import ConfigReader
 from simba.utils.printing import stdout_success, SimbaTimer
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/feature_extractors/feature_extractor_16bp.py` & `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/feature_extractor_16bp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+__author__ = "Simon Nilsson"
+
+
 import os
 import pandas as pd
 import numpy as np
 from copy import deepcopy
 import math
 from collections import defaultdict
 from simba.enums import Formats
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/feature_extractors/feature_extractor_9bp.py` & `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/feature_extractor_9bp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from __future__ import division
+__author__ = "Simon Nilsson"
+
 import os, glob
 import pandas as pd
 import math
 import numpy as np
 from copy import deepcopy
 from collections import defaultdict
 from simba.utils.read_write import get_fn_ext, read_df, write_df
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/feature_extractors/feature_extractor_8bp.py` & `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/feature_extractor_8bp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+__author__ = "Simon Nilsson"
+
 import os
 import numpy as np
 import pandas as pd
 from copy import deepcopy
 import math
 from collections import defaultdict
 from simba.enums import Formats
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/feature_extractors/feature_extractor_4bp.py` & `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/feature_extractor_4bp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+__author__ = "Simon Nilsson"
+
 import os
 import pandas as pd
 import numpy as np
 from copy import deepcopy
 import math
 from collections import defaultdict
 import scipy
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/feature_extractors/.idea/features_scripts.iml` & `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/.idea/features_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/feature_extractors/.idea/workspace.xml` & `Simba-UW-tf-dev-1.57.9/simba/feature_extractors/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/requirements.txt` & `Simba-UW-tf-dev-1.57.9/simba/requirements.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/severity_processor.py` & `Simba-UW-tf-dev-1.57.9/simba/severity_processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__author__ = "Simon Nilsson", "JJ Choong"
+__author__ = "Simon Nilsson"
 
 import numpy as np
 import glob, os
 import pandas as pd
 from datetime import datetime
 from numba import jit
 from simba.utils.read_write import read_video_info_csv, get_fn_ext, read_df
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/user_pose_config_creator.py` & `Simba-UW-tf-dev-1.57.9/simba/user_pose_config_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/mixins/.DS_Store` & `Simba-UW-tf-dev-1.57.9/simba/mixins/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/mixins/pop_up_mixin.py` & `Simba-UW-tf-dev-1.57.9/simba/mixins/pop_up_mixin.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+__author__ = "Simon Nilsson"
+
 from tkinter import *
 from PIL import ImageTk
 import PIL.Image
 from tkinter import messagebox
 import os
 from simba.pose_importers import trk_importer
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/mixins/config_reader.py` & `Simba-UW-tf-dev-1.57.9/simba/mixins/config_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+__author__ = "Simon Nilsson"
+
+
 from datetime import datetime
 import shutil
 import logging
 from configparser import ConfigParser
 import os, glob
 import pandas as pd
 import itertools
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.nbi` & `Simba-UW-tf-dev-1.57.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.1.nbc` & `Simba-UW-tf-dev-1.57.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.nbi` & `Simba-UW-tf-dev-1.57.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.1.nbc` & `Simba-UW-tf-dev-1.57.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.1.nbc` & `Simba-UW-tf-dev-1.57.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.nbi` & `Simba-UW-tf-dev-1.57.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/mixins/feature_extraction_mixin.py` & `Simba-UW-tf-dev-1.57.9/simba/mixins/feature_extraction_mixin.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+__author__ = "Simon Nilsson"
+
 import warnings
 warnings.filterwarnings("ignore")
 import numpy as np
 from numba import jit, prange
 from scipy.spatial import ConvexHull
 from scipy.spatial.qhull import QhullError
 import math
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/mixins/plotting_mixin.py` & `Simba-UW-tf-dev-1.57.9/simba/mixins/plotting_mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+__author__ = "Simon Nilsson"
+
 import cv2
 import matplotlib.pyplot as plt
 import pandas as pd
 import PIL
 import io
 import os
 import numpy as np
@@ -1067,8 +1069,53 @@
             writer.write(np.uint8(img))
             current_frm += 1
             print('Multi-processing video frame {} on core {}...'.format(str(current_frm), str(group)))
 
         cap.release()
         writer.release()
 
-        return group
+        return group
+
+    @staticmethod
+    def bbox_mp(frm_range: list,
+                polygon_data: dict,
+                animal_bp_dict: dict,
+                data_df: pd.DataFrame or None,
+                intersection_data_df: pd.DataFrame or None,
+                roi_attributes: dict,
+                video_path: str,
+                key_points: bool,
+                greyscale: bool):
+
+        cap, current_frame = cv2.VideoCapture(video_path), frm_range[0]
+        cap.set(1, frm_range[0])
+        img_lst = []
+        while current_frame < frm_range[-1]:
+            ret, frame = cap.read()
+            if ret:
+                if key_points:
+                    frm_data = data_df.iloc[current_frame]
+                if greyscale:
+                    frame = cv2.cvtColor(frame, cv2.COLOR_BGR2GRAY)
+                    frame = cv2.cvtColor(frame, cv2.COLOR_GRAY2BGR)
+                for animal_cnt, (animal, animal_data) in enumerate(animal_bp_dict.items()):
+                    if key_points:
+                        for bp_cnt, (x_col, y_col) in enumerate(zip(animal_data['X_bps'], animal_data['Y_bps'])):
+                            cv2.circle(frame, (frm_data[x_col], frm_data[y_col]), 0, roi_attributes[animal]['bbox_clr'],
+                                       roi_attributes[animal]['keypoint_size'])
+                    animal_polygon = np.array(
+                        list(polygon_data[animal][current_frame].convex_hull.exterior.coords)).astype(int)
+                    if intersection_data_df is not None:
+                        intersect = intersection_data_df.loc[
+                            current_frame, intersection_data_df.columns.str.startswith(animal)].sum()
+                        if intersect > 0:
+                            cv2.polylines(frame, [animal_polygon], 1, roi_attributes[animal]['highlight_clr'],
+                                          roi_attributes[animal]['highlight_clr_thickness'])
+                    cv2.polylines(frame, [animal_polygon], 1, roi_attributes[animal]['bbox_clr'],
+                                  roi_attributes[animal]['bbox_thickness'])
+                img_lst.append(frame)
+                current_frame += 1
+            else:
+                print(
+                    'SIMBA WARNING: SimBA tried to grab frame number {} from video {}, but could not find it. The video has {} frames.'.format(
+                        str(current_frame), video_path, str(cap.get(cv2.CAP_PROP_FRAME_COUNT))))
+        return img_lst
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/mixins/unsupervised_mixin.py` & `Simba-UW-tf-dev-1.57.9/simba/mixins/unsupervised_mixin.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+__author__ = "Simon Nilsson"
+
 import os, glob
 import pickle
 import simba
 from simba.enums import Paths
 from sklearn.feature_selection import VarianceThreshold
 from simba.unsupervised.enums import Unsupervised
 import pandas as pd
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/mixins/train_model_mixin.py` & `Simba-UW-tf-dev-1.57.9/simba/mixins/train_model_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/machine_model_settings_pop_up.py` & `Simba-UW-tf-dev-1.57.9/simba/machine_model_settings_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/remove_keypoints_in_pose.py` & `Simba-UW-tf-dev-1.57.9/simba/remove_keypoints_in_pose.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+__author__ = "Simon Nilsson"
+
 import glob, os
 import pandas as pd
 from datetime import datetime
 import warnings
 from tables import NaturalNameWarning
 from simba.utils.printing import stdout_success, SimbaTimer
 from simba.utils.checks import check_if_filepath_list_is_empty
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/third_party_label_appenders/deepethogram_importer.py` & `Simba-UW-tf-dev-1.57.9/simba/third_party_label_appenders/deepethogram_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/third_party_label_appenders/BORIS_appender.py` & `Simba-UW-tf-dev-1.57.9/simba/third_party_label_appenders/BORIS_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/third_party_label_appenders/observer_importer.py` & `Simba-UW-tf-dev-1.57.9/simba/third_party_label_appenders/observer_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/third_party_label_appenders/tools.py` & `Simba-UW-tf-dev-1.57.9/simba/third_party_label_appenders/tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/third_party_label_appenders/third_party_appender.py` & `Simba-UW-tf-dev-1.57.9/simba/third_party_label_appenders/third_party_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/third_party_label_appenders/ethovision_import.py` & `Simba-UW-tf-dev-1.57.9/simba/third_party_label_appenders/ethovision_import.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__author__ = "Simon Nilsson", "JJ Choong"
+__author__ = "Simon Nilsson"
 
 import os, glob
 import numpy as np
 import pandas as pd
 from simba.utils.read_write import get_fn_ext, read_df, write_df, read_config_file
 from simba.utils.checks import check_if_filepath_list_is_empty, check_that_column_exist
 from simba.utils.printing import stdout_success
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/third_party_label_appenders/BENTO_appender.py` & `Simba-UW-tf-dev-1.57.9/simba/third_party_label_appenders/BENTO_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/third_party_label_appenders/solomon_importer.py` & `Simba-UW-tf-dev-1.57.9/simba/third_party_label_appenders/solomon_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/multi_cropper.py` & `Simba-UW-tf-dev-1.57.9/simba/multi_cropper.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/FSTTC_calculator.py` & `Simba-UW-tf-dev-1.57.9/simba/FSTTC_calculator.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import pandas as pd
 import itertools
 import seaborn as sns
 from simba.utils.data import detect_bouts
 from simba.utils.printing import stdout_success
 from simba.utils.read_write import get_fn_ext, read_df
 from simba.utils.checks import check_if_filepath_list_is_empty
+from simba.utils.errors import CountError
 from simba.mixins.config_reader import ConfigReader
 
 class FSTTCPerformer(ConfigReader):
     """
     Class for calculating forward spike-time tiling coefficients between pairs of
     classified behaviors.
 
@@ -54,17 +55,19 @@
                  behavior_lst: list,
                  create_graphs: bool):
 
         super().__init__(config_path=config_path)
 
         self.time_delta = int(time_window)
         self.behavior_lst = behavior_lst
+        if len(self.behavior_lst) < 2:
+            raise CountError(msg='FSTCC requires at least two behaviors')
         self.graph_status = create_graphs
         check_if_filepath_list_is_empty(filepaths=self.machine_results_paths,
-                                        error_msg=f'SIMBA ERROR: Cannot calculate FSTTC, no data found in {self.machine_results_paths} directory')
+                                        error_msg=f'Cannot calculate FSTTC, no data found in {self.machine_results_paths} directory')
         self.clf_permutations = list(itertools.permutations(self.behavior_lst, 2))
         print(f'Processing FSTTC for {str(len(self.machine_results_paths))} file(s)...')
 
     def find_sequences(self):
         """
         Method to create list of dataframes holding information on the sequences of behaviors including
         inter-temporal distances.
@@ -74,29 +77,29 @@
         Attribute: list
             vide_df_sequence_lst
         """
 
         self.video_sequence_dict = {}
         out_columns =['Video',
                       'First behaviour',
-                        'First behaviour start frame',
-                         'First behavior end frame',
-                         'Second behaviour',
-                         'Second behaviour start frame',
-                         'Difference: first behavior start to second behavior start',
-                         'Time 2nd behaviour start to time window end']
+                      'First behaviour start frame',
+                      'First behavior end frame',
+                      'Second behaviour',
+                      'Second behaviour start frame',
+                      'Difference: first behavior start to second behavior start',
+                      'Time 2nd behaviour start to time window end']
 
         for file_cnt, file_path in enumerate(self.machine_results_paths):
             _, self.video_name, _ = get_fn_ext(file_path)
             self.video_sequence_dict[self.video_name] = {}
             print('Analyzing behavioral sequences: {}. Video {}/{}'.format(self.video_name, str(file_cnt + 1), str(len(self.machine_results_paths))))
             _, _, self.fps = self.read_video_info(video_name=self.video_name)
             self.video_sequence_dict[self.video_name]['fps'] = self.fps
             self.frames_in_window = int((self.fps / 1000) * self.time_delta)
-            self.data_df = read_df(file_path, self.file_type)[self.behavior_lst]
+            self.data_df = read_df(file_path, self.file_type)#[self.behavior_lst]
             self.video_sequence_dict[self.video_name]['session_length_frames'] = len(self.data_df)
             bouts_df = detect_bouts(data_df=self.data_df, target_lst=self.behavior_lst, fps=self.fps)
             bouts_df['Start_frame'] = (bouts_df['Start_time'] * self.fps).astype(int) - 1
             bouts_df = bouts_df[['Event', 'Start_frame', 'End_frame']]
             for first_clf, second_clf in self.clf_permutations:
                 self.vide_df_sequence_lst = []
                 sequence_name = 'FSTTC {} {}'.format(first_clf, second_clf)
@@ -115,65 +118,89 @@
                         second_clf_df_crtrn['Frames_between_second_behavior_start_to_time_window_end'] = (row['End_frame'] + self.frames_in_window) - second_clf_df_crtrn['Start_frame'].values[0]
                         self.vide_df_sequence_lst.append(pd.DataFrame([[self.video_name, first_clf, row['Start_frame'],
                                                  row['End_frame'], second_clf, second_clf_df_crtrn['Start_frame'].values[0],
                                                  second_clf_df_crtrn['Frames_between_behaviors'].values[0],
                                                  second_clf_df_crtrn['Frames_between_second_behavior_start_to_time_window_end'].values[0]]], columns=out_columns))
                     else:
 
-                        self.vide_df_sequence_lst.append(pd.DataFrame([[self.video_name, first_clf,
-                                                               int(row['Start_frame']),
-                                                               int(row['End_frame']),
-                                                               'None',
-                                                               'None',
-                                                               'None',
-                                                               'None']],
+                        self.vide_df_sequence_lst.append(pd.DataFrame([[self.video_name,
+                                                                        first_clf,
+                                                                        int(row['Start_frame']),
+                                                                        int(row['End_frame']),
+                                                                        'None',
+                                                                        'None',
+                                                                        'None',
+                                                                        'None']],
                                                              columns=out_columns))
 
                 if len(self.vide_df_sequence_lst) > 0:
                     video_sequences = pd.concat(self.vide_df_sequence_lst, axis=0).drop_duplicates(subset=['Video', 'First behaviour', 'First behaviour start frame', 'First behavior end frame', 'Second behaviour'], keep='first').reset_index(drop=True)
                     video_sequences['Total_window_frames'] = ((video_sequences['First behavior end frame'] - video_sequences['First behaviour start frame']) + self.frames_in_window)
                     self.video_sequence_dict[self.video_name][sequence_name] = video_sequences
                 else:
                     self.video_sequence_dict[self.video_name][sequence_name] = None
 
 
-    def calculate_FSTTC(self):
+    def run(self):
         """
         Method to calculate forward spike-time tiling coefficients (FSTTC) using the data computed in :meth:
         :meth:`~simba.FSTTCPerformer.find_sequences`.
 
         Returns
         -------
         Attribute: dict
             results_dict
         """
 
-
+        self.find_sequences()
         self.results_dict = {}
         for video_name, video_data in self.video_sequence_dict.items():
             self.results_dict[video_name] = {}
             fps, session_frames = video_data['fps'], video_data['session_length_frames']
             for first_clf, second_clf in self.clf_permutations:
-                sequence_name = 'FSTTC {} {}'.format(first_clf, second_clf)
+                sequence_name = f'FSTTC {first_clf} {second_clf}'
                 sequence_data = video_data[sequence_name]
                 if sequence_data is None:
                     self.results_dict[video_name][sequence_name] = 'No events'
                 else:
                     len_clf_1 = len(sequence_data[sequence_data['First behaviour'] == first_clf])
                     len_clf_1_2 = len(sequence_data[(sequence_data['First behaviour'] == first_clf) & (sequence_data['Second behaviour'] == second_clf)])
                     if (len_clf_1 > 0) & (len_clf_1_2 == 0):
                         self.results_dict[video_name][sequence_name] = 0.0
                     else:
                         clf_1_2_df = sequence_data[(sequence_data['First behaviour'] == first_clf) & (sequence_data['Second behaviour'] == second_clf)]
                         P = len_clf_1_2 / len_clf_1
                         Ta = sum(clf_1_2_df['Total_window_frames']) / session_frames
                         Tb = sum(clf_1_2_df['Time 2nd behaviour start to time window end']) / session_frames
                         self.results_dict[video_name][sequence_name] = 0.5 * ((P - Tb) / (1 - (P * Tb)) + ((P - Ta) / (1 - (P * Ta))))
+        self.save()
+        if self.graph_status:
+            self.plot_FSTTC()
+
+    def plot_FSTTC(self):
+        """
+        Method to visualize forward spike-time tiling coefficients (FSTTC) as png violin plots. Results are stored on
+        disk within the `project_folder/logs` directory.
+
+        Returns
+        -------
+        None
+        """
+
+        data_df = self.out_df[self.out_df['Value'] != 'No events'].reset_index(drop=True)
+        data_df['Value'] = pd.to_numeric(data_df['Value'], errors='coerce')
+        figure_FSCTT = sns.violinplot(x="FSTTC", y="Value", data=data_df, cut=0)
+        figure_FSCTT.set_xticklabels(figure_FSCTT.get_xticklabels(), rotation=45, size=7)
+        figure_FSCTT.figure.set_size_inches(13.7, 8.27)
+        save_plot_path = os.path.join(self.logs_path, f'FSTTC_{self.datetime}.png')
+        figure_FSCTT.figure.savefig(save_plot_path, bbox_inches="tight")
+        stdout_success(msg=f'FSTTC figure saved at {save_plot_path}')
 
-    def save_FSTTC(self):
+
+    def save(self):
         """
         Method to save forward spike-time tiling coefficients (FSTTC) to disk within the `project_folder/logs` directory.
 
         Returns
         -------
         None
         """
@@ -184,50 +211,20 @@
             video_df.insert(loc=0, column='Video', value=video)
             self.out_df = pd.concat([self.out_df,video_df], axis=0)
         file_save_path = os.path.join(self.logs_path, 'FSTTC_{}.csv'.format(str(self.datetime)))
         self.out_df.to_csv(file_save_path)
         self.timer.stop_timer()
         stdout_success(msg=f'FSTTC data saved at {file_save_path}', elapsed_time=self.timer.elapsed_time_str)
 
-    def plot_FSTTC(self):
-        """
-        Method to visualize forward spike-time tiling coefficients (FSTTC) as png violin plots. Results are stored on
-        disk within the `project_folder/logs` directory.
-
-        Returns
-        -------
-        None
-        """
-
-        if self.graph_status:
-            data_df = self.out_df[self.out_df['Value'] != 'No events'].reset_index(drop=True)
-            data_df['Value'] = pd.to_numeric(data_df['Value'], errors='coerce')
-            figure_FSCTT = sns.violinplot(x="FSTTC", y="Value", data=data_df, cut=0)
-            figure_FSCTT.set_xticklabels(figure_FSCTT.get_xticklabels(), rotation=45, size=7)
-            figure_FSCTT.figure.set_size_inches(13.7, 8.27)
-            save_plot_path = os.path.join(self.logs_path, 'FSTTC_{}.png'.format(str(self.datetime)))
-            figure_FSCTT.figure.savefig(save_plot_path, bbox_inches="tight")
-            stdout_success(msg=f'FSTTC figure saved at {save_plot_path}')
-
-
-# test = FSTTCPerformer(config_path='/Users/simon/Desktop/train_model_project/project_folder/project_config.ini',
-#                      time_window=2,
+# test = FSTTCPerformer(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini',
+#                      time_window=5,
 #                      behavior_lst=['Attack', 'Sniffing'],
 #                     create_graphs=True)
-# test.find_sequences()
-# test.calculate_FSTTC()
-# test.save_FSTTC()
-# test.plot_FSTTC()
-
-
-
-# test = FSTTCPerformer(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals/project_folder/project_config.ini',
-#                      time_window=2,
-#                      behavior_lst=['Attack', 'Sniffing'],
-#                     create_graphs=False)
+# test.run()
+#test.save()
 # test.find_sequences()
 # test.calculate_FSTTC()
 # test.save_FSTTC()
 # test.plot_FSTTC()
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/create_project_pop_up.py` & `Simba-UW-tf-dev-1.57.9/simba/create_project_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/video_info_table.py` & `Simba-UW-tf-dev-1.57.9/simba/video_info_table.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/cue_light_tools/.DS_Store` & `Simba-UW-tf-dev-1.57.9/simba/cue_light_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/cue_light_tools/cue_light_clf_statistics.py` & `Simba-UW-tf-dev-1.57.9/simba/cue_light_tools/cue_light_clf_statistics.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+__author__ = "Simon Nilsson"
+
 import pandas as pd
 import os, glob
 from simba.utils.read_write import read_df, get_fn_ext, read_config_entry
 from simba.utils.printing import stdout_success
 from simba.utils.checks import check_that_column_exist
 from simba.cue_light_tools.cue_light_tools import find_frames_when_cue_light_on
 from simba.utils.errors import NoFilesFoundError
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/cue_light_tools/cue_light_analyzer.py` & `Simba-UW-tf-dev-1.57.9/simba/cue_light_tools/cue_light_analyzer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+__author__ = "Simon Nilsson"
+
+
 from sklearn.cluster import KMeans
 import os, glob
 import itertools
 import pandas as pd
 import cv2
 import numpy as np
 import multiprocessing
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/cue_light_tools/cue_light_menues.py` & `Simba-UW-tf-dev-1.57.9/simba/cue_light_tools/cue_light_menues.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+__author__ = "Simon Nilsson"
+
 from tkinter import *
 import glob, os
 import itertools
 import pandas as pd
 
 from simba.utils.checks import check_float, check_int
 from simba.utils.read_write import get_fn_ext, find_video_of_file, get_all_clf_names, read_config_entry
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/cue_light_tools/cue_light_tools.py` & `Simba-UW-tf-dev-1.57.9/simba/cue_light_tools/cue_light_tools.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+__author__ = "Simon Nilsson"
+
 import pandas as pd
 from simba.utils.data import detect_bouts
 
 def find_frames_when_cue_light_on(data_df: pd.DataFrame,
                                   cue_light_names: list,
                                   fps: int,
                                   prior_window_frames_cnt: int,
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/cue_light_tools/cue_light_visualizer.py` & `Simba-UW-tf-dev-1.57.9/simba/cue_light_tools/cue_light_visualizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+__author__ = "Simon Nilsson"
+
 import itertools, os
 import pandas as pd
 import cv2
 from simba.utils.errors import NoSpecifiedOutputError, NoROIDataError
 from simba.mixins.config_reader import ConfigReader
 from simba.utils.read_write import read_df, get_fn_ext, get_video_meta_data
 from simba.utils.printing import stdout_success
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/cue_light_tools/cue_light_movement_statistics.py` & `Simba-UW-tf-dev-1.57.9/simba/cue_light_tools/cue_light_movement_statistics.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+__author__ = "Simon Nilsson"
+
 import os, glob
 from collections import defaultdict
 import pandas as pd
 import numpy as np
 from statistics import mean
 from simba.roi_tools.ROI_analyzer import ROIAnalyzer
 from simba.cue_light_tools.cue_light_tools import find_frames_when_cue_light_on
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/extract_frames_fast.py` & `Simba-UW-tf-dev-1.57.9/simba/extract_frames_fast.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+__author__ = "Simon Nilsson"
+
+
 # MODIFIED FROM https://gist.github.com/HaydenFaulkner/54318fd3e9b9bdb66c5440c44e4e08b8
 # Medium article https://medium.com/@haydenfaulkner/extracting-frames-fast-from-a-video-using-opencv-and-python-73b9b7dc9661
 # All cred to Hayden Faulkner, ta!
 
 from concurrent.futures import ProcessPoolExecutor
 import cv2
 import multiprocessing
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/utils/.DS_Store` & `Simba-UW-tf-dev-1.57.9/simba/utils/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/utils/warnings.py` & `Simba-UW-tf-dev-1.57.9/simba/utils/warnings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+__author__ = "Simon Nilsson"
+
 import logging
 from simba.utils.printing import stdout_warning
 
 def ThirdPartyAnnotationsOutsidePoseEstimationDataWarning(video_name: str,
                                                           frm_cnt: int,
                                                           log_status: bool = False,
                                                           clf_name: str or None = None,
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/utils/checks.py` & `Simba-UW-tf-dev-1.57.9/simba/utils/checks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+__author__ = "Simon Nilsson"
+
 import os
 import trafaret as t
 import pandas as pd
 from simba.utils.errors import (NoFilesFoundError,
                                 CorruptedFileError,
                                 IntegerError,
                                 FloatError,
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/utils/read_write.py` & `Simba-UW-tf-dev-1.57.9/simba/utils/read_write.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+__author__ = "Simon Nilsson"
+
 import pandas as pd
 import platform
 from datetime import datetime
 import shutil
 import glob, re
 import configparser
 from configparser import ConfigParser
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/utils/lookups.py` & `Simba-UW-tf-dev-1.57.9/simba/utils/lookups.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+__author__ = "Simon Nilsson"
+
 import os, glob
 import pandas as pd
 import re
 import struct
 import simba
 from simba.enums import Paths, Methods
 from simba.utils.checks import check_file_exist_and_readable, check_if_dir_exists
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/utils/errors.py` & `Simba-UW-tf-dev-1.57.9/simba/utils/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+__author__ = "Simon Nilsson"
+
 from tkinter import messagebox as mb
 from simba.enums import TagNames, Defaults
 
 WINDOW_TITLE = 'SIMBA ERROR'
 
 class SimbaError(Exception):
     def __init__(self, msg: str, show_window: bool):
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/utils/data.py` & `Simba-UW-tf-dev-1.57.9/simba/utils/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+__author__ = "Simon Nilsson"
+
 import pandas as pd
 from copy import deepcopy
 import configparser
 from pathlib import Path
 import ast, os
 from scipy.signal import savgol_filter
 from simba.enums import Dtypes
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/utils/printing.py` & `Simba-UW-tf-dev-1.57.9/simba/utils/printing.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+__author__ = "Simon Nilsson"
+
 from simba.enums import TagNames, Defaults
 import time
 
 def stdout_success(msg: str, elapsed_time: str or None=None) -> None:
     if elapsed_time:
         print(f'SIMBA COMPLETE: {msg} (elapsed time: {elapsed_time}s) {Defaults.STR_SPLIT_DELIMITER.value}{TagNames.COMPLETE.value}')
     else:
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/labelling_interface.py` & `Simba-UW-tf-dev-1.57.9/simba/labelling_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/timebins_movement_analyzer.py` & `Simba-UW-tf-dev-1.57.9/simba/timebins_movement_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/SimBA_dash_app.py` & `Simba-UW-tf-dev-1.57.9/simba/SimBA_dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/timebins_clf_analyzer.py` & `Simba-UW-tf-dev-1.57.9/simba/timebins_clf_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/calculate_px_dist.py` & `Simba-UW-tf-dev-1.57.9/simba/calculate_px_dist.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/movement_processor.py` & `Simba-UW-tf-dev-1.57.9/simba/movement_processor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/pybursts.py` & `Simba-UW-tf-dev-1.57.9/simba/pybursts.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/reverse_2_animal_tracking.py` & `Simba-UW-tf-dev-1.57.9/simba/reverse_2_animal_tracking.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__author__ = "Simon Nilsson", "JJ Choong"
+__author__ = "Simon Nilsson"
 
 import pandas as pd
 import shutil
 import os, glob
 from datetime import datetime
 
 from simba.feature_extractors.feature_extractor_16bp import ExtractFeaturesFrom16bps
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/Directing_animals_analyzer.py` & `Simba-UW-tf-dev-1.57.9/simba/Directing_animals_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/Validate_model_one_video_run_clf.py` & `Simba-UW-tf-dev-1.57.9/simba/Validate_model_one_video_run_clf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/tkinter_functions.py` & `Simba-UW-tf-dev-1.57.9/simba/tkinter_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__author__ = "Simon Nilsson", "JJ Choong"
+__author__ = "Simon Nilsson"
 
 from tkinter import *
 import platform
 from PIL import ImageTk
 import PIL.Image
 import webbrowser
 from tkinter.filedialog import askopenfilename, askdirectory
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/setting_menu.py` & `Simba-UW-tf-dev-1.57.9/simba/setting_menu.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/interpolate_pose.py` & `Simba-UW-tf-dev-1.57.9/simba/interpolate_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/run_inference.py` & `Simba-UW-tf-dev-1.57.9/simba/run_inference.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__author__ = "Simon Nilsson", "JJ Choong"
+__author__ = "Simon Nilsson"
 
 import os
 from copy import deepcopy
 import numpy as np
 from simba.mixins.train_model_mixin import TrainModelMixin
 from simba.mixins.config_reader import ConfigReader
 from simba.utils.data import plug_holes_shortest_bout
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/plotting/gantt_creator.py` & `Simba-UW-tf-dev-1.57.9/simba/plotting/gantt_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/plotting/tools/tkinter_tools.py` & `Simba-UW-tf-dev-1.57.9/simba/plotting/tools/tkinter_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+__author__ = "Simon Nilsson"
+
 from tkinter import *
 import cv2
 import numpy as np
 from PIL import Image as Img
 from PIL import ImageTk
 from simba.utils.errors import FrameRangeError
 from simba.utils.read_write import get_video_meta_data
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/plotting/ROI_plotter_mp.py` & `Simba-UW-tf-dev-1.57.9/simba/plotting/ROI_plotter_mp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__author__ = "Simon Nilsson", "JJ Choong"
+__author__ = "Simon Nilsson"
 
 
 import pandas as pd
 import os
 import itertools
 import cv2
 import platform
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/plotting/.DS_Store` & `Simba-UW-tf-dev-1.57.9/simba/plotting/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/plotting/shap_agg_stats_visualizer.py` & `Simba-UW-tf-dev-1.57.9/simba/plotting/shap_agg_stats_visualizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+__author__ = "Simon Nilsson"
+
 import pandas as pd
 import numpy as np
 import itertools
 import os
 import cv2
 import simba
 from simba.enums import Paths
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/plotting/gantt_creator_mp.py` & `Simba-UW-tf-dev-1.57.9/simba/plotting/gantt_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/plotting/heat_mapper_clf_mp.py` & `Simba-UW-tf-dev-1.57.9/simba/plotting/heat_mapper_clf_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/plotting/probability_plot_creator.py` & `Simba-UW-tf-dev-1.57.9/simba/plotting/probability_plot_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/plotting/plot_clf_results.py` & `Simba-UW-tf-dev-1.57.9/simba/plotting/plot_clf_results.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+__author__ = "Simon Nilsson"
+
+
 import os, glob
 from copy import deepcopy
 import cv2
 import numpy as np
 from PIL import Image
 from simba.mixins.config_reader import ConfigReader
 from simba.mixins.train_model_mixin import TrainModelMixin
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/plotting/plot_clf_results_mp.py` & `Simba-UW-tf-dev-1.57.9/simba/plotting/plot_clf_results_mp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+__author__ = "Simon Nilsson"
+
 import os
 from copy import deepcopy
 import multiprocessing
 import cv2
 import numpy as np
 import functools
 import platform
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/plotting/ROI_feature_visualizer.py` & `Simba-UW-tf-dev-1.57.9/simba/plotting/ROI_feature_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/plotting/heat_mapper_location.py` & `Simba-UW-tf-dev-1.57.9/simba/plotting/heat_mapper_location.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__author__ = "Simon Nilsson", "JJ Choong"
+__author__ = "Simon Nilsson"
 
 import os
 import cv2
 import numpy as np
 from numba import jit, prange
 import pandas as pd
 from simba.enums import Formats
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/plotting/probability_plot_creator_mp.py` & `Simba-UW-tf-dev-1.57.9/simba/plotting/probability_plot_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/plotting/interactive_probability_grapher.py` & `Simba-UW-tf-dev-1.57.9/simba/plotting/interactive_probability_grapher.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__author__ = "Simon Nilsson", "JJ Choong"
+__author__ = "Simon Nilsson"
 
 import matplotlib.pyplot as plt
 import os
 import threading
 from simba.enums import Paths
 from copy import copy
 from simba.mixins.config_reader import ConfigReader
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/plotting/plot_pose_in_dir.py` & `Simba-UW-tf-dev-1.57.9/simba/plotting/plot_pose_in_dir.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/plotting/single_run_model_validation_video.py` & `Simba-UW-tf-dev-1.57.9/simba/plotting/single_run_model_validation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/plotting/frame_mergerer_ffmpeg.py` & `Simba-UW-tf-dev-1.57.9/simba/plotting/frame_mergerer_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/plotting/Directing_animals_visualizer_mp.py` & `Simba-UW-tf-dev-1.57.9/simba/plotting/Directing_animals_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/plotting/clf_validator.py` & `Simba-UW-tf-dev-1.57.9/simba/plotting/clf_validator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/plotting/path_plotter_mp.py` & `Simba-UW-tf-dev-1.57.9/simba/plotting/path_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/plotting/ROI_feature_visualizer_mp.py` & `Simba-UW-tf-dev-1.57.9/simba/plotting/ROI_feature_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/plotting/data_plotter.py` & `Simba-UW-tf-dev-1.57.9/simba/plotting/data_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/plotting/path_plotter.py` & `Simba-UW-tf-dev-1.57.9/simba/plotting/path_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/plotting/ez_lineplot.py` & `Simba-UW-tf-dev-1.57.9/simba/plotting/ez_lineplot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__author__ = "Simon Nilsson", "JJ Choong"
+__author__ = "Simon Nilsson"
 
 import os
 import cv2
 import numpy as np
 import pandas as pd
 from simba.utils.printing import stdout_success, SimbaTimer
 from simba.utils.errors import DuplicationError, InvalidFileTypeError, DataHeaderError
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/plotting/distance_plotter_mp.py` & `Simba-UW-tf-dev-1.57.9/simba/plotting/distance_plotter_mp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-__author__ = "Simon Nilsson", "JJ Choong"
+__author__ = "Simon Nilsson"
+
 import numpy as np
 import multiprocessing
 import functools
 from numba import jit
 import os
 import platform
 from simba.utils.errors import NoSpecifiedOutputError
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/plotting/ROI_plotter.py` & `Simba-UW-tf-dev-1.57.9/simba/plotting/ROI_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/plotting/heat_mapper_clf.py` & `Simba-UW-tf-dev-1.57.9/simba/plotting/heat_mapper_clf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/plotting/distance_plotter.py` & `Simba-UW-tf-dev-1.57.9/simba/plotting/distance_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/plotting/single_run_model_validation_video_mp.py` & `Simba-UW-tf-dev-1.57.9/simba/plotting/single_run_model_validation_video_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/plotting/Directing_animals_visualizer.py` & `Simba-UW-tf-dev-1.57.9/simba/plotting/Directing_animals_visualizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__author__ = "Simon Nilsson", "JJ Choong"
+__author__ = "Simon Nilsson"
 
 import pandas as pd
 import os
 import cv2
 import numpy as np
 import random
 from simba.Directing_animals_analyzer import DirectingOtherAnimalsAnalyzer
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/plotting/heat_mapper_location_mp.py` & `Simba-UW-tf-dev-1.57.9/simba/plotting/heat_mapper_location_mp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__author__ = "Simon Nilsson", "JJ Choong"
+__author__ = "Simon Nilsson"
 
 import pandas as pd
 import numpy as np
 import os
 import cv2
 from numba import jit, prange
 import platform
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/run_dash_tkinter.py` & `Simba-UW-tf-dev-1.57.9/simba/run_dash_tkinter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/dash_app.py` & `Simba-UW-tf-dev-1.57.9/simba/dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/extract_annotation_frames.py` & `Simba-UW-tf-dev-1.57.9/simba/extract_annotation_frames.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+__author__ = "Simon Nilsson"
+
 import os.path
 import cv2
 from simba.mixins.config_reader import ConfigReader
 from simba.utils.read_write import read_df, find_video_of_file, get_fn_ext, get_video_meta_data
 from simba.utils.printing import stdout_success
 from simba.enums import Dtypes
 from simba.utils.errors import FrameRangeError
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/roi_tools/ROI_time_bin_calculator.py` & `Simba-UW-tf-dev-1.57.9/simba/roi_tools/ROI_time_bin_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/roi_tools/ROI_movement_analyzer.py` & `Simba-UW-tf-dev-1.57.9/simba/roi_tools/ROI_movement_analyzer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__author__ = "Simon Nilsson", "JJ Choong"
+__author__ = "Simon Nilsson"
 
 import os
 from simba.utils.printing import stdout_success
 from simba.mixins.config_reader import ConfigReader
 from simba.roi_tools.ROI_analyzer import ROIAnalyzer
 
 class ROIMovementAnalyzer(ConfigReader):
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/roi_tools/.DS_Store` & `Simba-UW-tf-dev-1.57.9/simba/roi_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/roi_tools/ROI_define.py` & `Simba-UW-tf-dev-1.57.9/simba/roi_tools/ROI_define.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/roi_tools/ROI_reset.py` & `Simba-UW-tf-dev-1.57.9/simba/roi_tools/ROI_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/roi_tools/ROI_analyzer.py` & `Simba-UW-tf-dev-1.57.9/simba/roi_tools/ROI_analyzer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__author__ = "Simon Nilsson", "JJ Choong"
+__author__ = "Simon Nilsson"
 
 import os, glob, itertools
 import numpy as np
 from shapely.geometry import Point, Polygon
 import pandas as pd
 from simba.utils.printing import stdout_success
 from simba.enums import ReadConfig, Dtypes
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/roi_tools/ROI_feature_analyzer.py` & `Simba-UW-tf-dev-1.57.9/simba/roi_tools/ROI_feature_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/roi_tools/ROI_multiply.py` & `Simba-UW-tf-dev-1.57.9/simba/roi_tools/ROI_multiply.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/roi_tools/ROI_size_calculations.py` & `Simba-UW-tf-dev-1.57.9/simba/roi_tools/ROI_size_calculations.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/roi_tools/ROI_zoom.py` & `Simba-UW-tf-dev-1.57.9/simba/roi_tools/ROI_zoom.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/roi_tools/ROI_directing_analyzer.py` & `Simba-UW-tf-dev-1.57.9/simba/roi_tools/ROI_directing_analyzer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__author__ = "Simon Nilsson", "JJ Choong"
+__author__ = "Simon Nilsson"
 
 from simba.roi_tools.ROI_analyzer import ROIAnalyzer
 import pandas as pd
 from numba import jit, prange
 from copy import deepcopy
 import numpy as np
 from simba.mixins.config_reader import ConfigReader
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/roi_tools/ROI_move_shape.py` & `Simba-UW-tf-dev-1.57.9/simba/roi_tools/ROI_move_shape.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/roi_tools/ROI_menus.py` & `Simba-UW-tf-dev-1.57.9/simba/roi_tools/ROI_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/roi_tools/ROI_clf_calculator.py` & `Simba-UW-tf-dev-1.57.9/simba/roi_tools/ROI_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/roi_tools/ROI_image.py` & `Simba-UW-tf-dev-1.57.9/simba/roi_tools/ROI_image.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/pose_importers/read_DANNCE_mat.py` & `Simba-UW-tf-dev-1.57.9/simba/pose_importers/read_DANNCE_mat.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__author__ = "Simon Nilsson", "JJ Choong"
+__author__ = "Simon Nilsson"
 
 import scipy.io
 import pandas as pd
 import ast
 import os, glob
 from configparser import ConfigParser, NoSectionError, NoOptionError
 from simba.utils.read_write import get_fn_ext, write_df
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/pose_importers/sleap_importer_slp.py` & `Simba-UW-tf-dev-1.57.9/simba/pose_importers/sleap_importer_slp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/pose_importers/sleap_importer_h5.py` & `Simba-UW-tf-dev-1.57.9/simba/pose_importers/sleap_importer_h5.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/pose_importers/dlc_multi_animal_importer.py` & `Simba-UW-tf-dev-1.57.9/simba/pose_importers/dlc_multi_animal_importer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__author__ = "Simon Nilsson", "JJ Choong"
+__author__ = "Simon Nilsson"
 
 import os, glob
 from datetime import datetime
 import itertools
 import pandas as pd
 import numpy as np
 import cv2
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/pose_importers/.DS_Store` & `Simba-UW-tf-dev-1.57.9/simba/pose_importers/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/pose_importers/sleap_importer_csv.py` & `Simba-UW-tf-dev-1.57.9/simba/pose_importers/sleap_importer_csv.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+__author__ = "Simon Nilsson"
+
 import pandas as pd
 import os, glob
 from numba import jit, prange
 import numpy as np
 from copy import deepcopy
 from datetime import datetime
 import itertools
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/pose_importers/import_mars.py` & `Simba-UW-tf-dev-1.57.9/simba/pose_importers/import_mars.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/pose_importers/dlc_importer_csv.py` & `Simba-UW-tf-dev-1.57.9/simba/pose_importers/dlc_importer_csv.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__author__ = "Simon Nilsson", "JJ Choong"
+__author__ = "Simon Nilsson"
 
 import shutil
 import os, glob
 import pandas as pd
 
 from simba.interpolate_smooth import Interpolate, Smooth
 from simba.utils.printing import stdout_success, SimbaTimer
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/pose_importers/trk_importer.py` & `Simba-UW-tf-dev-1.57.9/simba/pose_importers/trk_importer.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 from simba.read_config_unit_tests import read_config_file, read_config_entry
 import glob, os
 import scipy.io as sio
 import numpy as np
 import h5py
 import pandas as pd
+
 from simba.utils.read_write import get_fn_ext, find_video_of_file, get_video_meta_data
 from simba.utils.errors import NoFilesFoundError, CountError
 from simba.utils.warnings import InvalidValueWarning
+from simba.utils.checks import check_if_filepath_list_is_empty, check_if_dir_exists
 from simba.mixins.config_reader import ConfigReader
 import cv2
 
 class TRKImporter(ConfigReader):
     def __init__(self,
                  config_path: str,
-                 trk_folder: str,
+                 data_path: str,
                  animal_id_lst: list,
                  interpolation_method: str,
-                 smooth_settings: dict):
+                 smoothing_settings: dict):
 
         ConfigReader.__init__(self, config_path=config_path)
-        self.trk_folder, self.id_lst = trk_folder, animal_id_lst
-        self.interpolation_method, self.smooth_settings = interpolation_method, smooth_settings
+        check_if_dir_exists(in_dir=data_path)
+        self.data_path, self.id_lst = data_path, animal_id_lst
+        self.interpolation_method, self.smooth_settings = interpolation_method, smoothing_settings
         if self.animal_cnt == 1:
             self.animal_ids = ['Animal_1']
         else:
             self.animal_ids = read_config_entry(self.config, 'Multi animal IDs', 'id_list', 'str')
             self.animal_ids = self.animal_ids.split(",")
-        self.files_found = glob.glob(self.trk_folder + '/*.trk')
-        if len(self.files_found) == 0:
-            raise NoFilesFoundError(msg=f'No TRK files (with .trk file-ending) found in {self.trk_folder}')
-        self.video_folder = os.path.join(self.project_path, 'videos')
-        self.save_folder = os.path.join(self.project_path, 'csv', 'input_csv')
+        self.data_paths = glob.glob(self.data_path + '/*.trk')
+        check_if_filepath_list_is_empty(filepaths=self.data_paths, error_msg=f'No TRK files (with .trk file-ending) found in {self.data_path}')
         self.space_scaler, self.radius_scaler, self.resolution_scaler, self.font_scaler = 40, 10, 1500, 1.2
         self.frm_number = 0
 
     def trk_read(self, file_path: str):
         print('Reading data using scipy.io...')
         try:
             trk_dict = sio.loadmat(file_path)
@@ -58,68 +58,98 @@
 
         print('Number of animals detected in TRK {}: {}'.format(str(file_path), str(track_cnt)))
         if track_cnt != self.animal_cnt:
             raise CountError(msg=f'There are {str(track_cnt)} tracks in the .trk file {file_path}. But your SimBA project expects {str(self.animal_cnt)} tracks.')
         return animals_tracked_list
 
     def import_trk(self):
-        for file_cnt, file_path in enumerate(self.files_found):
+        for file_cnt, file_path in enumerate(self.data_paths):
             _, file_name, file_ext = get_fn_ext(file_path)
-            video_path = find_video_of_file(self.video_folder, file_name)
-            video_meta_data = get_video_meta_data(video_path=video_path)
-            animal_tracks = self.trk_read(file_path=file_path)
-
-            if self.animal_cnt != 1:
-                animal_df_lst = []
-                for animal in animal_tracks:
-                    m, n, r = animal.shape
-                    out_arr = np.column_stack((np.repeat(np.arange(m), n), animal.reshape(m * n, -1)))
-                    animal_df_lst.append(pd.DataFrame(out_arr).T.iloc[1:].reset_index(drop=True))
-                self.animal_df = pd.concat(animal_df_lst, axis=1).fillna(0)
-            else:
-                m, n, r = animal_tracks.shape
-                out_arr = np.column_stack((np.repeat(np.arange(m), n), animal_tracks.reshape(m * n, -1)))
-                self.animal_df = pd.DataFrame(out_arr).T.iloc[1:].reset_index(drop=True)
-            p_cols = pd.DataFrame(1, index=self.animal_df.index, columns=self.animal_df.columns[1::2] + .5)
-            self.animal_df = pd.concat([self.animal_df, p_cols], axis=1).sort_index(axis=1)
-            if len(self.bp_headers) != len(self.animal_df.columns):
-                raise CountError(msg=f'SimBA detected {str(len(self.animal_df.columns))} body-parts in the .TRK file {file_path}. Your SimBA project however expects {len(self.bp_headers)} body-parts')
-            self.animal_df.columns = self.bp_headers
-
-            max_dim = max(video_meta_data['width'], video_meta_data['height'])
-            self.circle_scale = int(self.radius_scaler / (self.resolution_scaler / max_dim))
-            self.font_scale = float(self.font_scaler / (self.resolution_scaler / max_dim))
-            self.spacingScale = int(self.space_scaler / (self.resolution_scaler / max_dim))
-            cv2.namedWindow('Define animal IDs', cv2.WINDOW_NORMAL)
-            self.cap = cv2.VideoCapture(video_path)
-            self.create_first_interface()
-
-    def __insert_all_animal_bps(self, frame=None):
-        for animal, bp_data in self.img_bp_cords_dict.items():
-            for bp_cnt, bp_tuple in enumerate(bp_data):
-                try:
-                    cv2.circle(frame, bp_tuple, self.circle_scale, self.animal_bp_dict[animal]['colors'][bp_cnt], -1, lineType=cv2.LINE_AA)
-                except Exception as err:
-                    if type(err) == OverflowError:
-                        InvalidValueWarning(f'SimBA encountered a pose-estimated body-part located at pixel position {str(bp_tuple)}. This value is too large to be converted to an integer. Please check your pose-estimation data to make sure that it is accurate.')
-                    print(err.args)
-
-    def create_first_interface(self):
-        while True:
-            self.cap.set(1, self.frm_number)
-            _, self.frame = self.cap.read()
-            self.overlay = self.frame.copy()
-            self.img_bp_cords_dict = {}
-            for animal_cnt, (animal_name, animal_bps) in enumerate(self.animal_bp_dict.items()):
-                self.img_bp_cords_dict[animal_name] = []
-                for bp_cnt in range(len(animal_bps['X_bps'])):
-                    x_cord = int(self.animal_df.loc[self.frm_number, animal_name + '_' + animal_bps['X_bps'][bp_cnt]])
-                    y_cord = int(self.animal_df.loc[self.frm_number, animal_name + '_' + animal_bps['Y_bps'][bp_cnt]])
-                    self.img_bp_cords_dict[animal_name].append((x_cord, y_cord))
-            self.__insert_all_animal_bps(frame=self.overlay)
+            if self.animal_cnt > 0:
+                pass
+            video_path = find_video_of_file(self.video_dir, file_name)
+            if not video_path:
+                raise NoFilesFoundError(msg='Could not find a video jj')
+    #         video_meta_data = get_video_meta_data(video_path=video_path)
+    #         animal_tracks = self.trk_read(file_path=file_path)
+    #
+    #         if self.animal_cnt != 1:
+    #             animal_df_lst = []
+    #             for animal in animal_tracks:
+    #                 m, n, r = animal.shape
+    #                 out_arr = np.column_stack((np.repeat(np.arange(m), n), animal.reshape(m * n, -1)))
+    #                 animal_df_lst.append(pd.DataFrame(out_arr).T.iloc[1:].reset_index(drop=True))
+    #             self.animal_df = pd.concat(animal_df_lst, axis=1).fillna(0)
+    #         else:
+    #             m, n, r = animal_tracks.shape
+    #             out_arr = np.column_stack((np.repeat(np.arange(m), n), animal_tracks.reshape(m * n, -1)))
+    #             self.animal_df = pd.DataFrame(out_arr).T.iloc[1:].reset_index(drop=True)
+    #         p_cols = pd.DataFrame(1, index=self.animal_df.index, columns=self.animal_df.columns[1::2] + .5)
+    #         self.animal_df = pd.concat([self.animal_df, p_cols], axis=1).sort_index(axis=1)
+    #         if len(self.bp_headers) != len(self.animal_df.columns):
+    #             raise CountError(msg=f'SimBA detected {str(len(self.animal_df.columns))} body-parts in the .TRK file {file_path}. Your SimBA project however expects {len(self.bp_headers)} body-parts')
+    #         self.animal_df.columns = self.bp_headers
+    #
+    #         max_dim = max(video_meta_data['width'], video_meta_data['height'])
+    #         self.circle_scale = int(self.radius_scaler / (self.resolution_scaler / max_dim))
+    #         self.font_scale = float(self.font_scaler / (self.resolution_scaler / max_dim))
+    #         self.spacingScale = int(self.space_scaler / (self.resolution_scaler / max_dim))
+    #         cv2.namedWindow('Define animal IDs', cv2.WINDOW_NORMAL)
+    #         self.cap = cv2.VideoCapture(video_path)
+    #         self.create_first_interface()
+    #
+    # def __insert_all_animal_bps(self, frame=None):
+    #     for animal, bp_data in self.img_bp_cords_dict.items():
+    #         for bp_cnt, bp_tuple in enumerate(bp_data):
+    #             try:
+    #                 cv2.circle(frame, bp_tuple, self.circle_scale, self.animal_bp_dict[animal]['colors'][bp_cnt], -1, lineType=cv2.LINE_AA)
+    #             except Exception as err:
+    #                 if type(err) == OverflowError:
+    #                     InvalidValueWarning(f'SimBA encountered a pose-estimated body-part located at pixel position {str(bp_tuple)}. This value is too large to be converted to an integer. Please check your pose-estimation data to make sure that it is accurate.')
+    #                 print(err.args)
+    #
+    # def create_first_interface(self):
+    #     while True:
+    #         self.cap.set(1, self.frm_number)
+    #         _, self.frame = self.cap.read()
+    #         self.overlay = self.frame.copy()
+    #         self.img_bp_cords_dict = {}
+    #         for animal_cnt, (animal_name, animal_bps) in enumerate(self.animal_bp_dict.items()):
+    #             self.img_bp_cords_dict[animal_name] = []
+    #             for bp_cnt in range(len(animal_bps['X_bps'])):
+    #                 x_cord = int(self.animal_df.loc[self.frm_number, animal_name + '_' + animal_bps['X_bps'][bp_cnt]])
+    #                 y_cord = int(self.animal_df.loc[self.frm_number, animal_name + '_' + animal_bps['Y_bps'][bp_cnt]])
+    #                 self.img_bp_cords_dict[animal_name].append((x_cord, y_cord))
+    #         self.__insert_all_animal_bps(frame=self.overlay)
+
+
+# test = TRKImporter(config_path='/Users/simon/Desktop/envs/troubleshooting/DLC_2_Black_animals/project_folder/project_config.ini',
+#                    data_path='/Users/simon/Desktop/envs/simba_dev/tests/test_data/import_tests/trk_data',
+#                    animal_id_lst=['Animal_1', 'Animal_2'],
+#                    interpolation_method="Body-parts: Nearest",
+#                    smoothing_settings = {'Method': 'Savitzky Golay', 'Parameters': {'Time_window': '200'}})
+#
+
+
+# test = SLEAPImporterCSV(config_path=r'/Users/simon/Desktop/envs/troubleshooting/Hornet/project_folder/project_config.ini',
+#                  data_folder=r'/Users/simon/Desktop/envs/troubleshooting/Hornet_single_slp/import',
+#                  actor_IDs=['Hornet'],
+#                  interpolation_settings="Body-parts: Nearest",
+#                  smoothing_settings = {'Method': 'Savitzky Golay', 'Parameters': {'Time_window': '200'}})
+# test.run()
+
+
+
+# def __init__(self,
+#              config_path: str,
+#              data_folder: str,
+#              animal_id_lst: list,
+#              interpolation_method: str,
+#              smooth_settings: dict):
+
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/pop_up_classes.py` & `Simba-UW-tf-dev-1.57.9/simba/pop_up_classes.py`

 * *Files 1% similar despite different names*

```diff
@@ -404,22 +404,20 @@
         for behaviour, behavior_val in behaviours_dict.items():
             if behavior_val.get():
                 targets.append(behaviour)
 
         if len(targets) < 2:
             raise CountError(msg='SIMBA ERROR: FORWARD SPIKE TIME TILING COEFFICIENTS REQUIRE 2 OR MORE BEHAVIORS.')
 
-        FSTCC_performer = FSTTCPerformer(config_path=self.config_path,
+        fsttc_performer = FSTTCPerformer(config_path=self.config_path,
                                          time_window=time_delta,
                                          behavior_lst=targets,
                                          create_graphs=graph_var)
-        FSTCC_performer.find_sequences()
-        FSTCC_performer.calculate_FSTTC()
-        FSTCC_performer.save_FSTTC()
-        FSTCC_performer.plot_FSTTC()
+        fsttc_performer.run()
+
 
 #_ = FSTTCPopUp(config_path='/Users/simon/Desktop/envs/troubleshooting/Two_animals_16bps/project_folder/project_config.ini')
 
 class KleinbergPopUp(PopUpMixin, ConfigReader):
     def __init__(self,
                  config_path: str):
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/extract_seqframes.py` & `Simba-UW-tf-dev-1.57.9/simba/extract_seqframes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/pose_configurations/.DS_Store` & `Simba-UW-tf-dev-1.57.9/simba/pose_configurations/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/pose_configurations/bp_names/.DS_Store` & `Simba-UW-tf-dev-1.57.9/simba/pose_configurations/bp_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/pose_configurations/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.57.9/simba/pose_configurations/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/pose_configurations/no_animals/.DS_Store` & `Simba-UW-tf-dev-1.57.9/simba/pose_configurations/no_animals/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/pose_configurations/configuration_names/.DS_Store` & `Simba-UW-tf-dev-1.57.9/simba/pose_configurations/configuration_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/pose_configurations/schematics/.DS_Store` & `Simba-UW-tf-dev-1.57.9/simba/pose_configurations/schematics/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/pose_configurations/schematics/8.png` & `Simba-UW-tf-dev-1.57.9/simba/pose_configurations/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/pose_configurations/schematics/9.png` & `Simba-UW-tf-dev-1.57.9/simba/pose_configurations/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/pose_configurations/schematics/12.png` & `Simba-UW-tf-dev-1.57.9/simba/pose_configurations/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/pose_configurations/schematics/11.png` & `Simba-UW-tf-dev-1.57.9/simba/pose_configurations/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/pose_configurations/schematics/10.png` & `Simba-UW-tf-dev-1.57.9/simba/pose_configurations/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/pose_configurations/schematics/4.png` & `Simba-UW-tf-dev-1.57.9/simba/pose_configurations/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/pose_configurations/schematics/5.png` & `Simba-UW-tf-dev-1.57.9/simba/pose_configurations/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/pose_configurations/schematics/7.png` & `Simba-UW-tf-dev-1.57.9/simba/pose_configurations/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/pose_configurations/schematics/6.png` & `Simba-UW-tf-dev-1.57.9/simba/pose_configurations/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/pose_configurations/schematics/2.png` & `Simba-UW-tf-dev-1.57.9/simba/pose_configurations/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/pose_configurations/schematics/3.png` & `Simba-UW-tf-dev-1.57.9/simba/pose_configurations/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/pose_configurations/schematics/1.png` & `Simba-UW-tf-dev-1.57.9/simba/pose_configurations/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/get_coordinates_tools_v2.py` & `Simba-UW-tf-dev-1.57.9/simba/get_coordinates_tools_v2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__author__ = "Simon Nilsson", "JJ Choong"
+__author__ = "Simon Nilsson"
 
 
 import os
 import cv2
 import numpy as np
 
 def get_coordinates_nilsson(filenames,knownmm):
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/pup_retrieval_protocol.py` & `Simba-UW-tf-dev-1.57.9/simba/pup_retrieval_protocol.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+__author__ = "Simon Nilsson"
+
 import pandas as pd
 
 
 import os, glob
 from datetime import datetime
 import seaborn as sns
 from simba.mixins.config_reader import ConfigReader
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/outlier_tools/outlier_corrector_movement.py` & `Simba-UW-tf-dev-1.57.9/simba/outlier_tools/outlier_corrector_movement.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+__author__ = "Simon Nilsson"
+
 import os, glob
 import pandas as pd
 import numpy as np
 from simba.mixins.config_reader import ConfigReader
 from simba.utils.read_write import read_df, write_df, get_fn_ext, read_config_entry
 from simba.utils.printing import stdout_success, SimbaTimer
 from simba.utils.warnings import DataHeaderWarning
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/outlier_tools/.DS_Store` & `Simba-UW-tf-dev-1.57.9/simba/outlier_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/outlier_tools/outlier_corrector_location.py` & `Simba-UW-tf-dev-1.57.9/simba/outlier_tools/outlier_corrector_location.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+__author__ = "Simon Nilsson"
+
 import os, glob
 import numpy as np
 import pandas as pd
 from simba.enums import ReadConfig, Dtypes
 from simba.mixins.config_reader import ConfigReader
 from simba.utils.printing import stdout_success, SimbaTimer
 from simba.utils.read_write import read_df, write_df, get_fn_ext, read_config_entry
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/outlier_tools/skip_outlier_correction.py` & `Simba-UW-tf-dev-1.57.9/simba/outlier_tools/skip_outlier_correction.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+__author__ = "Simon Nilsson"
+
 import os
 from simba.utils.printing import stdout_success, SimbaTimer
 from simba.utils.read_write import get_fn_ext, read_df, write_df
 from simba.utils.checks import check_if_filepath_list_is_empty
 from simba.mixins.config_reader import ConfigReader
 
 class OutlierCorrectionSkipper(ConfigReader):
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/outlier_tools/.idea/outlier_scripts.iml` & `Simba-UW-tf-dev-1.57.9/simba/outlier_tools/.idea/outlier_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.57.9/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/outlier_tools/.idea/workspace.xml` & `Simba-UW-tf-dev-1.57.9/simba/outlier_tools/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/pose_reset.py` & `Simba-UW-tf-dev-1.57.9/simba/pose_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/train_mutiple_models.py` & `Simba-UW-tf-dev-1.57.9/simba/train_mutiple_models.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/SimBA.py` & `Simba-UW-tf-dev-1.57.9/simba/SimBA.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__author__ = "Simon Nilsson", "JJ Choong"
+__author__ = "Simon Nilsson"
 
 import os.path
 import warnings
 warnings.filterwarnings('ignore',category=FutureWarning)
 warnings.filterwarnings('ignore',category=DeprecationWarning)
 from tkinter.filedialog import askopenfilename,askdirectory
 from PIL import ImageTk
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/labelling_advanced_interface.py` & `Simba-UW-tf-dev-1.57.9/simba/labelling_advanced_interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__author__ = "Simon Nilsson", "JJ Choong"
+__author__ = "Simon Nilsson"
 
 import simba
 from tkinter import *
 from tkinter import filedialog
 from PIL import Image, ImageTk
 from subprocess import Popen, PIPE
 import os
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.57.9/simba/assets/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/unsupervised/model_names.parquet` & `Simba-UW-tf-dev-1.57.9/simba/assets/unsupervised/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/unsupervised/features.csv` & `Simba-UW-tf-dev-1.57.9/simba/assets/unsupervised/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/shap/down_arrow.jpg` & `Simba-UW-tf-dev-1.57.9/simba/assets/shap/down_arrow.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/shap/intruder_shape.jpg` & `Simba-UW-tf-dev-1.57.9/simba/assets/shap/intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/shap/feature_categories/shap_feature_categories.csv` & `Simba-UW-tf-dev-1.57.9/simba/assets/shap/feature_categories/shap_feature_categories.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/shap/.DS_Store` & `Simba-UW-tf-dev-1.57.9/simba/assets/shap/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/shap/resident_shape.jpg` & `Simba-UW-tf-dev-1.57.9/simba/assets/shap/resident_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/shap/resident_intruder_shape.jpg` & `Simba-UW-tf-dev-1.57.9/simba/assets/shap/resident_intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/shap/animal_distances.jpg` & `Simba-UW-tf-dev-1.57.9/simba/assets/shap/animal_distances.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/shap/baseline_scale.jpg` & `Simba-UW-tf-dev-1.57.9/simba/assets/shap/baseline_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/shap/ubuntu.regular.ttf` & `Simba-UW-tf-dev-1.57.9/simba/assets/shap/ubuntu.regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/shap/side_scale.jpg` & `Simba-UW-tf-dev-1.57.9/simba/assets/shap/side_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/shap/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.57.9/simba/assets/shap/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/shap/side_scale_5.jpg` & `Simba-UW-tf-dev-1.57.9/simba/assets/shap/side_scale_5.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/shap/intruder_movement.jpg` & `Simba-UW-tf-dev-1.57.9/simba/assets/shap/intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/shap/resident_movement.jpg` & `Simba-UW-tf-dev-1.57.9/simba/assets/shap/resident_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/shap/color_bar.jpg` & `Simba-UW-tf-dev-1.57.9/simba/assets/shap/color_bar.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/shap/resident_intruder_movement.jpg` & `Simba-UW-tf-dev-1.57.9/simba/assets/shap/resident_intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/.DS_Store` & `Simba-UW-tf-dev-1.57.9/simba/assets/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/lookups/.DS_Store` & `Simba-UW-tf-dev-1.57.9/simba/assets/lookups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/lookups/model_names.parquet` & `Simba-UW-tf-dev-1.57.9/simba/assets/lookups/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/lookups/feature_extraction_headers.csv` & `Simba-UW-tf-dev-1.57.9/simba/assets/lookups/feature_extraction_headers.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/lookups/features.csv` & `Simba-UW-tf-dev-1.57.9/simba/assets/lookups/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/lookups/unsupervised_example_x.csv` & `Simba-UW-tf-dev-1.57.9/simba/assets/lookups/unsupervised_example_x.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/stl/operant_tray.stl` & `Simba-UW-tf-dev-1.57.9/simba/assets/stl/operant_tray.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/stl/operant_lever.stl` & `Simba-UW-tf-dev-1.57.9/simba/assets/stl/operant_lever.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/stl/operant_walls.stl` & `Simba-UW-tf-dev-1.57.9/simba/assets/stl/operant_walls.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/stl/grid_floor.stl` & `Simba-UW-tf-dev-1.57.9/simba/assets/stl/grid_floor.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/img/.DS_Store` & `Simba-UW-tf-dev-1.57.9/simba/assets/img/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/img/about_me.png` & `Simba-UW-tf-dev-1.57.9/simba/assets/img/about_me.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/img/splash.mp4` & `Simba-UW-tf-dev-1.57.9/simba/assets/img/splash.mp4`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/img/bg_2.png` & `Simba-UW-tf-dev-1.57.9/simba/assets/img/bg_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/img/splash.pptx` & `Simba-UW-tf-dev-1.57.9/simba/assets/img/splash.pptx`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/img/bg.png` & `Simba-UW-tf-dev-1.57.9/simba/assets/img/bg.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.57.9/simba/assets/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/icons/factory.png` & `Simba-UW-tf-dev-1.57.9/simba/assets/icons/factory.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/icons/cluster.png` & `Simba-UW-tf-dev-1.57.9/simba/assets/icons/cluster.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/icons/load.png` & `Simba-UW-tf-dev-1.57.9/simba/assets/icons/load.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/icons/gif.png` & `Simba-UW-tf-dev-1.57.9/simba/assets/icons/gif.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/icons/pose.png` & `Simba-UW-tf-dev-1.57.9/simba/assets/icons/pose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/icons/features.png` & `Simba-UW-tf-dev-1.57.9/simba/assets/icons/features.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/icons/.DS_Store` & `Simba-UW-tf-dev-1.57.9/simba/assets/icons/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/icons/settings.png` & `Simba-UW-tf-dev-1.57.9/simba/assets/icons/settings.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/icons/stopwatch.png` & `Simba-UW-tf-dev-1.57.9/simba/assets/icons/stopwatch.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/icons/link.png` & `Simba-UW-tf-dev-1.57.9/simba/assets/icons/link.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/icons/dash_simba.css` & `Simba-UW-tf-dev-1.57.9/simba/assets/icons/dash_simba.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/icons/documentation.png` & `Simba-UW-tf-dev-1.57.9/simba/assets/icons/documentation.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/icons/fps.png` & `Simba-UW-tf-dev-1.57.9/simba/assets/icons/fps.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/icons/dimensionality_reduction.png` & `Simba-UW-tf-dev-1.57.9/simba/assets/icons/dimensionality_reduction.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/icons/roi.png` & `Simba-UW-tf-dev-1.57.9/simba/assets/icons/roi.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/icons/superimpose.png` & `Simba-UW-tf-dev-1.57.9/simba/assets/icons/superimpose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/icons/label.png` & `Simba-UW-tf-dev-1.57.9/simba/assets/icons/label.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/icons/change.png` & `Simba-UW-tf-dev-1.57.9/simba/assets/icons/change.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/icons/crop.png` & `Simba-UW-tf-dev-1.57.9/simba/assets/icons/crop.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/icons/rotate.png` & `Simba-UW-tf-dev-1.57.9/simba/assets/icons/rotate.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/icons/path.png` & `Simba-UW-tf-dev-1.57.9/simba/assets/icons/path.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/icons/clip.png` & `Simba-UW-tf-dev-1.57.9/simba/assets/icons/clip.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/icons/restart.png` & `Simba-UW-tf-dev-1.57.9/simba/assets/icons/restart.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/icons/calipher.png` & `Simba-UW-tf-dev-1.57.9/simba/assets/icons/calipher.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/icons/add_on.png` & `Simba-UW-tf-dev-1.57.9/simba/assets/icons/add_on.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/icons/create.png` & `Simba-UW-tf-dev-1.57.9/simba/assets/icons/create.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/icons/SimBA_logo.ico` & `Simba-UW-tf-dev-1.57.9/simba/assets/icons/SimBA_logo.ico`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/icons/print.png` & `Simba-UW-tf-dev-1.57.9/simba/assets/icons/print.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/icons/clf.png` & `Simba-UW-tf-dev-1.57.9/simba/assets/icons/clf.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/icons/concat_icons/mosaic.png` & `Simba-UW-tf-dev-1.57.9/simba/assets/icons/concat_icons/mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/icons/concat_icons/vertical.png` & `Simba-UW-tf-dev-1.57.9/simba/assets/icons/concat_icons/vertical.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/icons/concat_icons/horizontal.png` & `Simba-UW-tf-dev-1.57.9/simba/assets/icons/concat_icons/horizontal.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/icons/concat_icons/mixed_mosaic.png` & `Simba-UW-tf-dev-1.57.9/simba/assets/icons/concat_icons/mixed_mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/icons/merge.png` & `Simba-UW-tf-dev-1.57.9/simba/assets/icons/merge.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/icons/clean.png` & `Simba-UW-tf-dev-1.57.9/simba/assets/icons/clean.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/icons/clf_2.png` & `Simba-UW-tf-dev-1.57.9/simba/assets/icons/clf_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/icons/visualize.png` & `Simba-UW-tf-dev-1.57.9/simba/assets/icons/visualize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/icons/concat.png` & `Simba-UW-tf-dev-1.57.9/simba/assets/icons/concat.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/icons/boris.png` & `Simba-UW-tf-dev-1.57.9/simba/assets/icons/boris.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/icons/frames.png` & `Simba-UW-tf-dev-1.57.9/simba/assets/icons/frames.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/icons/video.png` & `Simba-UW-tf-dev-1.57.9/simba/assets/icons/video.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/icons/sample.png` & `Simba-UW-tf-dev-1.57.9/simba/assets/icons/sample.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/icons/metrics.png` & `Simba-UW-tf-dev-1.57.9/simba/assets/icons/metrics.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/icons/grey.png` & `Simba-UW-tf-dev-1.57.9/simba/assets/icons/grey.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/icons/exit.png` & `Simba-UW-tf-dev-1.57.9/simba/assets/icons/exit.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/icons/outlier.png` & `Simba-UW-tf-dev-1.57.9/simba/assets/icons/outlier.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/icons/clahe.png` & `Simba-UW-tf-dev-1.57.9/simba/assets/icons/clahe.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/icons/trash.png` & `Simba-UW-tf-dev-1.57.9/simba/assets/icons/trash.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/icons/about.png` & `Simba-UW-tf-dev-1.57.9/simba/assets/icons/about.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/icons/convert.png` & `Simba-UW-tf-dev-1.57.9/simba/assets/icons/convert.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/icons/SimBA_logo.icns` & `Simba-UW-tf-dev-1.57.9/simba/assets/icons/SimBA_logo.icns`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/icons/reorganize.png` & `Simba-UW-tf-dev-1.57.9/simba/assets/icons/reorganize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/icons/browse.png` & `Simba-UW-tf-dev-1.57.9/simba/assets/icons/browse.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/icons/SimBA_logo.png` & `Simba-UW-tf-dev-1.57.9/simba/assets/icons/SimBA_logo.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/icons/ethovision.png` & `Simba-UW-tf-dev-1.57.9/simba/assets/icons/ethovision.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/icons/close.png` & `Simba-UW-tf-dev-1.57.9/simba/assets/icons/close.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/dash_simba_base.css` & `Simba-UW-tf-dev-1.57.9/simba/assets/dash_simba_base.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/assets/TheGoldenLab.PNG` & `Simba-UW-tf-dev-1.57.9/simba/assets/TheGoldenLab.PNG`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/read_config_unit_tests.py` & `Simba-UW-tf-dev-1.57.9/simba/read_config_unit_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__author__ = "Simon Nilsson", "JJ Choong"
+__author__ = "Simon Nilsson"
 
 import configparser
 import trafaret as t
 import os
 import pandas as pd
 from simba.enums import ReadConfig, Dtypes, Formats
 from configparser import ConfigParser
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/project_config_creator.py` & `Simba-UW-tf-dev-1.57.9/simba/project_config_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/train_single_model.py` & `Simba-UW-tf-dev-1.57.9/simba/train_single_model.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/create_clf_log.py` & `Simba-UW-tf-dev-1.57.9/simba/create_clf_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__author__ = "Simon Nilsson", "JJ Choong"
+__author__ = "Simon Nilsson"
 
 import pandas as pd
 import os
 from simba.utils.checks import check_file_exist_and_readable, check_if_filepath_list_is_empty
 from simba.mixins.config_reader import ConfigReader
 from simba.utils.data import detect_bouts
 from simba.utils.printing import stdout_success
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/batch_process_videos/.DS_Store` & `Simba-UW-tf-dev-1.57.9/simba/batch_process_videos/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/batch_process_videos/batch_process_menus.py` & `Simba-UW-tf-dev-1.57.9/simba/batch_process_videos/batch_process_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/batch_process_videos/batch_process_create_ffmpeg_commands.py` & `Simba-UW-tf-dev-1.57.9/simba/batch_process_videos/batch_process_create_ffmpeg_commands.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/Kleinberg_calculator.py` & `Simba-UW-tf-dev-1.57.9/simba/Kleinberg_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/simba/reorganize_keypoint_in_pose.py` & `Simba-UW-tf-dev-1.57.9/simba/reorganize_keypoint_in_pose.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+__author__ = "Simon Nilsson"
+
 import glob, os
 import pandas as pd
 from collections import OrderedDict
 from datetime import datetime
 from simba.utils.checks import check_if_filepath_list_is_empty, check_if_dir_exists
 from simba.utils.printing import stdout_success
 from simba.enums import Formats
```

### Comparing `Simba-UW-tf-dev-1.57.8/simba/play_annotation_video.py` & `Simba-UW-tf-dev-1.57.9/simba/play_annotation_video.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__author__ = "Simon Nilsson", "JJ Choong"
+__author__ = "Simon Nilsson"
 
 import cv2
 import sys
 import os
 import signal
 from simba.utils.read_write import get_video_meta_data
 from simba.utils.lookups import get_color_dict
```

### Comparing `Simba-UW-tf-dev-1.57.8/Simba_UW_tf_dev.egg-info/PKG-INFO` & `Simba-UW-tf-dev-1.57.9/Simba_UW_tf_dev.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.57.8
+Version: 1.57.9
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.57.8/Simba_UW_tf_dev.egg-info/SOURCES.txt` & `Simba-UW-tf-dev-1.57.9/Simba_UW_tf_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/Simba_UW_tf_dev.egg-info/requires.txt` & `Simba-UW-tf-dev-1.57.9/Simba_UW_tf_dev.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/LICENSE.md` & `Simba-UW-tf-dev-1.57.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/README.md` & `Simba-UW-tf-dev-1.57.9/README.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.8/setup.py` & `Simba-UW-tf-dev-1.57.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Licensed under GNU Lesser General Public License v3.0
 """
 
 import setuptools
 
 setuptools.setup(
     name="Simba-UW-tf-dev",
-    version="1.57.8",
+    version="1.57.9",
     author="Simon Nilsson, Jia Jie Choong, Sophia Hwang",
     author_email="sronilsson@gmail.com",
     description="Toolkit for computer classification of complex social behaviors in experimental animals",
     url="https://github.com/sgoldenlab/simba",
     install_requires=['Pillow == 5.4.1', 'pyyaml == 5.3.1','shapely == 1.7','wxpython == 4.0.4',
               'dtreeviz == 0.8.1','eli5 == 0.10.1','graphviz == 0.11',
               'imblearn == 0.0','imgaug == 0.4.0','imutils == 0.5.2','matplotlib == 3.0.3', 'numpy == 1.18.1',
```

