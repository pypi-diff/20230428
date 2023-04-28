# Comparing `tmp/linora-1.6.0.tar.gz` & `tmp/linora-2.0.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/linora-1.6.0.tar", last modified: Thu Feb 23 02:44:04 2023, max compression
+gzip compressed data, was "dist/linora-2.0.0rc0.tar", last modified: Fri Apr 28 01:24:56 2023, max compression
```

## Comparing `linora-1.6.0.tar` & `linora-2.0.0rc0.tar`

### file list

```diff
@@ -1,198 +1,217 @@
-drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-02-23 02:44:04.000000 linora-1.6.0/
--rw-r--r--   0 liyanpeng   (501) staff       (20)     3733 2023-02-23 02:44:04.000000 linora-1.6.0/PKG-INFO
--rw-r--r--   0 liyanpeng   (501) staff       (20)     2148 2022-05-06 08:30:54.000000 linora-1.6.0/README.md
-drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-02-23 02:44:04.000000 linora-1.6.0/linora/
--rw-r--r--   0 liyanpeng   (501) staff       (20)      927 2022-11-17 02:23:45.000000 linora-1.6.0/linora/__init__.py
-drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-02-23 02:44:04.000000 linora-1.6.0/linora/audio/
--rw-r--r--   0 liyanpeng   (501) staff       (20)       75 2022-11-17 07:55:45.000000 linora-1.6.0/linora/audio/__init__.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     3764 2023-02-07 06:49:28.000000 linora-1.6.0/linora/audio/_audio_io.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)      492 2022-11-17 07:55:32.000000 linora-1.6.0/linora/audio/_audio_util.py
-drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-02-23 02:44:04.000000 linora-1.6.0/linora/chart/
--rw-r--r--   0 liyanpeng   (501) staff       (20)      403 2022-07-14 05:53:05.000000 linora-1.6.0/linora/chart/__init__.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     2453 2022-08-09 08:32:05.000000 linora-1.6.0/linora/chart/_arrow.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     5625 2022-08-09 08:07:44.000000 linora-1.6.0/linora/chart/_bar.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)    37257 2022-08-22 09:14:42.000000 linora-1.6.0/linora/chart/_base.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     5507 2022-08-03 06:11:10.000000 linora-1.6.0/linora/chart/_boxplot.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     1916 2022-08-09 08:11:23.000000 linora-1.6.0/linora/chart/_circle.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     4479 2022-08-09 07:00:01.000000 linora-1.6.0/linora/chart/_coherence.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     3883 2022-08-19 07:12:54.000000 linora-1.6.0/linora/chart/_config.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     4940 2022-08-09 07:03:51.000000 linora-1.6.0/linora/chart/_csd.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     2160 2022-08-09 08:12:42.000000 linora-1.6.0/linora/chart/_ellipse.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     7443 2022-08-03 06:11:42.000000 linora-1.6.0/linora/chart/_errorbar.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     1466 2022-04-24 14:02:43.000000 linora-1.6.0/linora/chart/_feature.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     3870 2022-08-09 02:21:38.000000 linora-1.6.0/linora/chart/_fillline.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     7720 2022-08-10 08:01:23.000000 linora-1.6.0/linora/chart/_grid.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     6951 2022-08-09 02:21:56.000000 linora-1.6.0/linora/chart/_hist.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     1004 2022-08-09 02:22:05.000000 linora-1.6.0/linora/chart/_hist2d.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     1353 2022-08-09 02:22:40.000000 linora-1.6.0/linora/chart/_hlines.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     4557 2022-08-09 02:22:54.000000 linora-1.6.0/linora/chart/_line.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     4806 2022-08-09 02:23:07.000000 linora-1.6.0/linora/chart/_line3D.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)    11321 2022-04-24 14:02:43.000000 linora-1.6.0/linora/chart/_metrics.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     3835 2022-08-03 06:13:51.000000 linora-1.6.0/linora/chart/_pie.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     8171 2022-08-09 08:34:12.000000 linora-1.6.0/linora/chart/_plot.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     1983 2022-08-09 08:12:27.000000 linora-1.6.0/linora/chart/_polygon.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     5312 2022-08-09 02:23:32.000000 linora-1.6.0/linora/chart/_radar.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     2511 2022-08-09 08:11:53.000000 linora-1.6.0/linora/chart/_rectangle.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     2242 2022-08-09 08:11:43.000000 linora-1.6.0/linora/chart/_regularpolygon.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     5718 2022-08-09 02:23:50.000000 linora-1.6.0/linora/chart/_scatter.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     6367 2022-08-09 02:24:07.000000 linora-1.6.0/linora/chart/_scatter3D.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     1350 2022-08-09 02:24:44.000000 linora-1.6.0/linora/chart/_vlines.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     2137 2022-08-09 08:08:19.000000 linora-1.6.0/linora/chart/_wedge.py
-drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-02-23 02:44:04.000000 linora-1.6.0/linora/data/
-drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-02-23 02:44:04.000000 linora-1.6.0/linora/data/Dataset/
--rw-r--r--   0 liyanpeng   (501) staff       (20)       42 2022-06-08 08:59:03.000000 linora-1.6.0/linora/data/Dataset/__init__.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)    27211 2022-08-29 09:18:04.000000 linora-1.6.0/linora/data/Dataset/_data.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)    13157 2022-06-08 08:22:31.000000 linora-1.6.0/linora/data/Dataset/_dataset.py
-drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-02-23 02:44:04.000000 linora-1.6.0/linora/data/TextLineDataset/
--rw-r--r--   0 liyanpeng   (501) staff       (20)       50 2022-05-27 04:17:36.000000 linora-1.6.0/linora/data/TextLineDataset/__init__.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)    15392 2022-05-27 08:07:05.000000 linora-1.6.0/linora/data/TextLineDataset/_dataset.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)      215 2022-12-07 05:59:38.000000 linora-1.6.0/linora/data/__init__.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     4007 2022-11-18 07:47:39.000000 linora-1.6.0/linora/data/_compress.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)    11876 2022-12-07 06:31:44.000000 linora-1.6.0/linora/data/_sql_io_dataset.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     1941 2022-06-01 08:26:01.000000 linora-1.6.0/linora/data/_utils.py
-drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-02-23 02:44:04.000000 linora-1.6.0/linora/data/datasets/
--rw-r--r--   0 liyanpeng   (501) staff       (20)       85 2022-08-19 09:00:53.000000 linora-1.6.0/linora/data/datasets/__init__.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     2071 2022-12-01 09:47:11.000000 linora-1.6.0/linora/data/datasets/_config_path.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)    19314 2022-06-08 08:37:02.000000 linora-1.6.0/linora/data/datasets/_mnist.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     1293 2022-12-02 05:08:27.000000 linora-1.6.0/linora/data/datasets/_utils.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)   264001 2022-08-22 01:29:59.000000 linora-1.6.0/linora/data/datasets/_weather.py
-drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-02-23 02:44:04.000000 linora-1.6.0/linora/feature_column/
--rw-r--r--   0 liyanpeng   (501) staff       (20)      231 2022-11-11 06:00:37.000000 linora-1.6.0/linora/feature_column/__init__.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)    14044 2022-11-16 03:10:08.000000 linora-1.6.0/linora/feature_column/_categorical.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     2485 2022-11-16 02:31:23.000000 linora-1.6.0/linora/feature_column/_feature.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     8702 2022-11-16 03:22:18.000000 linora-1.6.0/linora/feature_column/_normalize.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     7030 2022-11-16 03:31:02.000000 linora-1.6.0/linora/feature_column/_numerical.py
-drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-02-23 02:44:04.000000 linora-1.6.0/linora/feature_column/boundary/
--rw-r--r--   0 liyanpeng   (501) staff       (20)       55 2022-04-24 14:02:43.000000 linora-1.6.0/linora/feature_column/boundary/__init__.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     3495 2022-04-24 14:02:43.000000 linora-1.6.0/linora/feature_column/boundary/_boundary.py
-drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-02-23 02:44:04.000000 linora-1.6.0/linora/feature_selection/
--rw-r--r--   0 liyanpeng   (501) staff       (20)       94 2022-04-24 14:02:43.000000 linora-1.6.0/linora/feature_selection/__init__.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     1780 2022-04-24 14:02:43.000000 linora-1.6.0/linora/feature_selection/_credit.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     2622 2022-05-12 01:17:51.000000 linora-1.6.0/linora/feature_selection/_select.py
-drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-02-23 02:44:04.000000 linora-1.6.0/linora/gfile/
--rw-r--r--   0 liyanpeng   (501) staff       (20)       33 2022-04-24 14:02:43.000000 linora-1.6.0/linora/gfile/__init__.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     5895 2022-11-23 09:16:08.000000 linora-1.6.0/linora/gfile/_gfile.py
-drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-02-23 02:44:04.000000 linora-1.6.0/linora/image/
--rw-r--r--   0 liyanpeng   (501) staff       (20)      636 2022-05-16 10:12:12.000000 linora-1.6.0/linora/image/__init__.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     1442 2022-05-26 02:08:30.000000 linora-1.6.0/linora/image/_image_aug.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     3596 2022-05-18 00:54:35.000000 linora-1.6.0/linora/image/_image_box.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)    29992 2022-11-30 09:53:59.000000 linora-1.6.0/linora/image/_image_color.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)    12038 2022-05-26 02:07:59.000000 linora-1.6.0/linora/image/_image_color_aug.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     8666 2022-05-16 09:32:03.000000 linora-1.6.0/linora/image/_image_crop.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     2963 2022-05-26 02:08:58.000000 linora-1.6.0/linora/image/_image_crop_aug.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)    11337 2022-05-27 06:56:17.000000 linora-1.6.0/linora/image/_image_draw.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     2305 2022-05-27 07:05:28.000000 linora-1.6.0/linora/image/_image_draw_aug.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)    16607 2022-11-18 03:22:32.000000 linora-1.6.0/linora/image/_image_feature.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     8805 2022-05-13 01:24:35.000000 linora-1.6.0/linora/image/_image_filter.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     5629 2022-05-26 02:09:23.000000 linora-1.6.0/linora/image/_image_filter_aug.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     7215 2022-08-01 08:30:47.000000 linora-1.6.0/linora/image/_image_grid.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     2262 2022-08-29 03:23:22.000000 linora-1.6.0/linora/image/_image_io.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     2345 2022-05-22 03:19:04.000000 linora-1.6.0/linora/image/_image_io_aug.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)    13075 2022-05-17 03:28:28.000000 linora-1.6.0/linora/image/_image_noise.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     7787 2022-05-26 02:09:49.000000 linora-1.6.0/linora/image/_image_noise_aug.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     8431 2022-04-25 13:29:23.000000 linora-1.6.0/linora/image/_image_pairs.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)    21630 2022-05-25 09:46:33.000000 linora-1.6.0/linora/image/_image_position.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)    12989 2022-05-26 02:40:18.000000 linora-1.6.0/linora/image/_image_position_aug.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     7012 2022-05-16 02:51:05.000000 linora-1.6.0/linora/image/_image_rescale.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     4257 2022-05-26 02:10:15.000000 linora-1.6.0/linora/image/_image_rescale_aug.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     2527 2022-05-25 02:36:08.000000 linora-1.6.0/linora/image/_image_resize.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)      519 2022-05-09 09:56:14.000000 linora-1.6.0/linora/image/_image_resize_aug.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)    41696 2022-05-27 06:48:41.000000 linora-1.6.0/linora/image/_image_rgb.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     5698 2022-04-24 14:02:43.000000 linora-1.6.0/linora/image/_image_util.py
-drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-02-23 02:44:04.000000 linora-1.6.0/linora/metrics/
--rw-r--r--   0 liyanpeng   (501) staff       (20)      231 2022-04-24 14:02:43.000000 linora-1.6.0/linora/metrics/__init__.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)    27844 2022-06-22 02:45:29.000000 linora-1.6.0/linora/metrics/_classification.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     4966 2022-05-26 08:02:56.000000 linora-1.6.0/linora/metrics/_image.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     2335 2022-05-26 07:22:49.000000 linora-1.6.0/linora/metrics/_metrics.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     2568 2022-06-21 10:20:14.000000 linora-1.6.0/linora/metrics/_rank.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)    18341 2022-11-21 07:42:50.000000 linora-1.6.0/linora/metrics/_regression.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)      370 2022-06-21 10:10:45.000000 linora-1.6.0/linora/metrics/_utils.py
-drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-02-23 02:44:04.000000 linora-1.6.0/linora/metrics/distance/
--rw-r--r--   0 liyanpeng   (501) staff       (20)       97 2022-04-24 14:02:43.000000 linora-1.6.0/linora/metrics/distance/__init__.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)    10758 2022-06-22 01:50:38.000000 linora-1.6.0/linora/metrics/distance/_distance.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     5635 2022-04-24 14:02:43.000000 linora-1.6.0/linora/metrics/distance/_divergence.py
-drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-02-23 02:44:04.000000 linora-1.6.0/linora/parallel/
--rw-r--r--   0 liyanpeng   (501) staff       (20)       77 2022-04-24 14:02:43.000000 linora-1.6.0/linora/parallel/__init__.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     5619 2022-04-24 14:02:43.000000 linora-1.6.0/linora/parallel/_process.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     5408 2022-04-24 14:02:43.000000 linora-1.6.0/linora/parallel/_thread.py
-drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-02-23 02:44:04.000000 linora-1.6.0/linora/param_search/
-drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-02-23 02:44:04.000000 linora-1.6.0/linora/param_search/GEClassifier/
--rw-r--r--   0 liyanpeng   (501) staff       (20)     2941 2022-04-24 14:02:43.000000 linora-1.6.0/linora/param_search/GEClassifier/_GridSearch.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     3182 2022-04-24 14:02:43.000000 linora-1.6.0/linora/param_search/GEClassifier/_RandomSearch.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)      142 2022-04-24 14:02:43.000000 linora-1.6.0/linora/param_search/GEClassifier/__init__.py
-drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-02-23 02:44:04.000000 linora-1.6.0/linora/param_search/GERegressor/
--rw-r--r--   0 liyanpeng   (501) staff       (20)     3219 2022-04-24 14:02:43.000000 linora-1.6.0/linora/param_search/GERegressor/_RandomSearch.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)       71 2022-04-24 14:02:43.000000 linora-1.6.0/linora/param_search/GERegressor/__init__.py
-drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-02-23 02:44:04.000000 linora-1.6.0/linora/param_search/LGBMClassifier/
--rw-r--r--   0 liyanpeng   (501) staff       (20)     7659 2022-05-20 03:53:11.000000 linora-1.6.0/linora/param_search/LGBMClassifier/_GridSearch.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     7646 2022-05-20 03:52:49.000000 linora-1.6.0/linora/param_search/LGBMClassifier/_RandomSearch.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)      144 2022-05-05 06:13:26.000000 linora-1.6.0/linora/param_search/LGBMClassifier/__init__.py
-drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-02-23 02:44:04.000000 linora-1.6.0/linora/param_search/LGBMRegressor/
--rw-r--r--   0 liyanpeng   (501) staff       (20)     7656 2022-05-20 03:53:26.000000 linora-1.6.0/linora/param_search/LGBMRegressor/_GridSearch.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     7644 2022-05-20 03:52:33.000000 linora-1.6.0/linora/param_search/LGBMRegressor/_RandomSearch.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)      141 2022-05-05 06:14:26.000000 linora-1.6.0/linora/param_search/LGBMRegressor/__init__.py
-drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-02-23 02:44:04.000000 linora-1.6.0/linora/param_search/XGBClassifier/
--rw-r--r--   0 liyanpeng   (501) staff       (20)     8752 2022-05-20 03:51:53.000000 linora-1.6.0/linora/param_search/XGBClassifier/_GridSearch.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     8724 2022-05-20 03:52:15.000000 linora-1.6.0/linora/param_search/XGBClassifier/_RandomSearch.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)      142 2022-04-24 14:02:43.000000 linora-1.6.0/linora/param_search/XGBClassifier/__init__.py
-drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-02-23 02:44:04.000000 linora-1.6.0/linora/param_search/XGBRanker/
--rw-r--r--   0 liyanpeng   (501) staff       (20)     5599 2022-04-24 14:02:43.000000 linora-1.6.0/linora/param_search/XGBRanker/_GridSearch.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     5904 2022-04-24 14:02:43.000000 linora-1.6.0/linora/param_search/XGBRanker/_RandomSearch.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)      138 2022-04-24 14:02:43.000000 linora-1.6.0/linora/param_search/XGBRanker/__init__.py
-drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-02-23 02:44:04.000000 linora-1.6.0/linora/param_search/XGBRegressor/
--rw-r--r--   0 liyanpeng   (501) staff       (20)     8912 2022-05-20 03:51:33.000000 linora-1.6.0/linora/param_search/XGBRegressor/_GridSearch.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     8943 2022-05-20 03:51:09.000000 linora-1.6.0/linora/param_search/XGBRegressor/_RandomSearch.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)      140 2022-04-24 14:02:43.000000 linora-1.6.0/linora/param_search/XGBRegressor/__init__.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)    13838 2022-06-15 06:08:40.000000 linora-1.6.0/linora/param_search/_HyperParameters.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     9330 2022-06-02 07:48:01.000000 linora-1.6.0/linora/param_search/_Search.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)      177 2022-06-08 09:41:40.000000 linora-1.6.0/linora/param_search/__init__.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     9231 2022-05-22 02:43:27.000000 linora-1.6.0/linora/param_search/_config.py
-drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-02-23 02:44:04.000000 linora-1.6.0/linora/sample/
--rw-r--r--   0 liyanpeng   (501) staff       (20)      162 2022-05-10 08:08:14.000000 linora-1.6.0/linora/sample/__init__.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     4847 2022-11-04 06:31:17.000000 linora-1.6.0/linora/sample/_fold.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     3542 2022-04-24 14:02:43.000000 linora-1.6.0/linora/sample/_random_walker.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     7072 2022-11-24 03:05:14.000000 linora-1.6.0/linora/sample/_sampling.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     4051 2022-04-27 01:42:13.000000 linora-1.6.0/linora/sample/_timeseries_kfold.py
-drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-02-23 02:44:04.000000 linora-1.6.0/linora/text/
--rw-r--r--   0 liyanpeng   (501) staff       (20)      149 2022-04-24 14:02:43.000000 linora-1.6.0/linora/text/__init__.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     6243 2022-04-24 14:02:43.000000 linora-1.6.0/linora/text/_sequence.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     4002 2022-04-24 14:02:43.000000 linora-1.6.0/linora/text/_util.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     2267 2022-04-24 14:02:43.000000 linora-1.6.0/linora/text/_vectorizer.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     2633 2022-04-24 14:02:43.000000 linora-1.6.0/linora/text/_word_processing.py
-drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-02-23 02:44:04.000000 linora-1.6.0/linora/train/
--rw-r--r--   0 liyanpeng   (501) staff       (20)      308 2022-08-24 08:42:12.000000 linora-1.6.0/linora/train/__init__.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     2922 2022-09-01 01:52:14.000000 linora-1.6.0/linora/train/_callback.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     1781 2022-08-24 02:28:50.000000 linora-1.6.0/linora/train/_csvlogger.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     2371 2022-08-25 05:33:20.000000 linora-1.6.0/linora/train/_earlystopping.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     1768 2022-08-24 02:54:41.000000 linora-1.6.0/linora/train/_modelcheckpoint.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     2193 2022-08-24 01:53:17.000000 linora-1.6.0/linora/train/_remotemonitor.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     2180 2022-09-01 01:55:31.000000 linora-1.6.0/linora/train/_terminateonnan.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     7364 2022-08-27 02:43:20.000000 linora-1.6.0/linora/train/_visual.py
-drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-02-23 02:44:04.000000 linora-1.6.0/linora/train/lr/
--rw-r--r--   0 liyanpeng   (501) staff       (20)       75 2022-08-25 02:12:32.000000 linora-1.6.0/linora/train/lr/__init__.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)    12872 2022-08-26 07:47:29.000000 linora-1.6.0/linora/train/lr/_lr.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     1991 2022-08-25 03:30:35.000000 linora-1.6.0/linora/train/lr/_schedulers.py
-drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-02-23 02:44:04.000000 linora-1.6.0/linora/utils/
--rw-r--r--   0 liyanpeng   (501) staff       (20)      241 2022-11-10 02:19:13.000000 linora-1.6.0/linora/utils/__init__.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     1444 2022-04-24 14:02:43.000000 linora-1.6.0/linora/utils/_config.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)    19066 2022-11-23 01:41:44.000000 linora-1.6.0/linora/utils/_email.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)    17119 2022-11-23 01:25:02.000000 linora-1.6.0/linora/utils/_email_utils.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     9213 2022-05-11 03:45:54.000000 linora-1.6.0/linora/utils/_logger.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     4106 2022-05-31 11:52:27.000000 linora-1.6.0/linora/utils/_progbar.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)    13495 2022-05-11 03:09:28.000000 linora-1.6.0/linora/utils/_schedulers.py
-drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-02-23 02:44:04.000000 linora-1.6.0/linora/utils/message/
--rw-r--r--   0 liyanpeng   (501) staff       (20)    11784 2022-06-14 08:26:34.000000 linora-1.6.0/linora/utils/message/_BotDingTalk.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)      520 2022-04-24 14:02:43.000000 linora-1.6.0/linora/utils/message/_BotFeiShu.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)       93 2022-06-10 09:49:02.000000 linora-1.6.0/linora/utils/message/__init__.py
-drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-02-23 02:44:04.000000 linora-1.6.0/linora/utils/pip/
--rw-r--r--   0 liyanpeng   (501) staff       (20)       35 2022-08-04 02:59:58.000000 linora-1.6.0/linora/utils/pip/__init__.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)    14751 2022-08-05 04:59:06.000000 linora-1.6.0/linora/utils/pip/_pip.py
-drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-02-23 02:44:04.000000 linora-1.6.0/linora.egg-info/
--rw-r--r--   0 liyanpeng   (501) staff       (20)     3733 2023-02-23 02:44:04.000000 linora-1.6.0/linora.egg-info/PKG-INFO
--rw-r--r--   0 liyanpeng   (501) staff       (20)     5071 2023-02-23 02:44:04.000000 linora-1.6.0/linora.egg-info/SOURCES.txt
--rw-r--r--   0 liyanpeng   (501) staff       (20)        1 2023-02-23 02:44:04.000000 linora-1.6.0/linora.egg-info/dependency_links.txt
--rw-r--r--   0 liyanpeng   (501) staff       (20)        1 2023-02-23 02:44:04.000000 linora-1.6.0/linora.egg-info/not-zip-safe
--rw-r--r--   0 liyanpeng   (501) staff       (20)       67 2023-02-23 02:44:04.000000 linora-1.6.0/linora.egg-info/requires.txt
--rw-r--r--   0 liyanpeng   (501) staff       (20)        7 2023-02-23 02:44:04.000000 linora-1.6.0/linora.egg-info/top_level.txt
--rw-r--r--   0 liyanpeng   (501) staff       (20)       79 2023-02-23 02:44:04.000000 linora-1.6.0/setup.cfg
--rw-r--r--   0 liyanpeng   (501) staff       (20)     1628 2023-02-23 02:32:53.000000 linora-1.6.0/setup.py
+drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-04-28 01:24:56.000000 linora-2.0.0rc0/
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     3736 2023-04-28 01:24:56.000000 linora-2.0.0rc0/PKG-INFO
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     2148 2022-05-06 08:30:54.000000 linora-2.0.0rc0/README.md
+drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora/
+-rw-r--r--   0 liyanpeng   (501) staff       (20)      981 2023-03-28 07:21:23.000000 linora-2.0.0rc0/linora/__init__.py
+drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora/audio/
+-rw-r--r--   0 liyanpeng   (501) staff       (20)       75 2022-11-17 07:55:45.000000 linora-2.0.0rc0/linora/audio/__init__.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)    14608 2023-04-27 06:54:53.000000 linora-2.0.0rc0/linora/audio/_audio_io.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)      492 2022-11-17 07:55:32.000000 linora-2.0.0rc0/linora/audio/_audio_util.py
+drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora/chart/
+-rw-r--r--   0 liyanpeng   (501) staff       (20)      403 2022-07-14 05:53:05.000000 linora-2.0.0rc0/linora/chart/__init__.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     2453 2022-08-09 08:32:05.000000 linora-2.0.0rc0/linora/chart/_arrow.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     5625 2022-08-09 08:07:44.000000 linora-2.0.0rc0/linora/chart/_bar.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)    37257 2022-08-22 09:14:42.000000 linora-2.0.0rc0/linora/chart/_base.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     5507 2022-08-03 06:11:10.000000 linora-2.0.0rc0/linora/chart/_boxplot.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     1916 2022-08-09 08:11:23.000000 linora-2.0.0rc0/linora/chart/_circle.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     4479 2022-08-09 07:00:01.000000 linora-2.0.0rc0/linora/chart/_coherence.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     3883 2022-08-19 07:12:54.000000 linora-2.0.0rc0/linora/chart/_config.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     4940 2022-08-09 07:03:51.000000 linora-2.0.0rc0/linora/chart/_csd.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     2160 2022-08-09 08:12:42.000000 linora-2.0.0rc0/linora/chart/_ellipse.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     7443 2022-08-03 06:11:42.000000 linora-2.0.0rc0/linora/chart/_errorbar.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     1466 2022-04-24 14:02:43.000000 linora-2.0.0rc0/linora/chart/_feature.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     3870 2022-08-09 02:21:38.000000 linora-2.0.0rc0/linora/chart/_fillline.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     7720 2022-08-10 08:01:23.000000 linora-2.0.0rc0/linora/chart/_grid.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     6951 2022-08-09 02:21:56.000000 linora-2.0.0rc0/linora/chart/_hist.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     1004 2022-08-09 02:22:05.000000 linora-2.0.0rc0/linora/chart/_hist2d.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     1353 2022-08-09 02:22:40.000000 linora-2.0.0rc0/linora/chart/_hlines.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     4557 2022-08-09 02:22:54.000000 linora-2.0.0rc0/linora/chart/_line.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     4806 2022-08-09 02:23:07.000000 linora-2.0.0rc0/linora/chart/_line3D.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)    11321 2022-04-24 14:02:43.000000 linora-2.0.0rc0/linora/chart/_metrics.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     3835 2022-08-03 06:13:51.000000 linora-2.0.0rc0/linora/chart/_pie.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     8171 2022-08-09 08:34:12.000000 linora-2.0.0rc0/linora/chart/_plot.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     1983 2022-08-09 08:12:27.000000 linora-2.0.0rc0/linora/chart/_polygon.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     5312 2022-08-09 02:23:32.000000 linora-2.0.0rc0/linora/chart/_radar.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     2511 2022-08-09 08:11:53.000000 linora-2.0.0rc0/linora/chart/_rectangle.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     2242 2022-08-09 08:11:43.000000 linora-2.0.0rc0/linora/chart/_regularpolygon.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     5718 2022-08-09 02:23:50.000000 linora-2.0.0rc0/linora/chart/_scatter.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     6367 2022-08-09 02:24:07.000000 linora-2.0.0rc0/linora/chart/_scatter3D.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     1350 2022-08-09 02:24:44.000000 linora-2.0.0rc0/linora/chart/_vlines.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     2137 2022-08-09 08:08:19.000000 linora-2.0.0rc0/linora/chart/_wedge.py
+drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora/data/
+drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora/data/Dataset/
+-rw-r--r--   0 liyanpeng   (501) staff       (20)       42 2022-06-08 08:59:03.000000 linora-2.0.0rc0/linora/data/Dataset/__init__.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)    27211 2022-08-29 09:18:04.000000 linora-2.0.0rc0/linora/data/Dataset/_data.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)    13157 2022-06-08 08:22:31.000000 linora-2.0.0rc0/linora/data/Dataset/_dataset.py
+drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora/data/TextLineDataset/
+-rw-r--r--   0 liyanpeng   (501) staff       (20)       50 2022-05-27 04:17:36.000000 linora-2.0.0rc0/linora/data/TextLineDataset/__init__.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)    15392 2022-05-27 08:07:05.000000 linora-2.0.0rc0/linora/data/TextLineDataset/_dataset.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)      215 2022-12-07 05:59:38.000000 linora-2.0.0rc0/linora/data/__init__.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     4007 2022-11-18 07:47:39.000000 linora-2.0.0rc0/linora/data/_compress.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)    11876 2022-12-07 06:31:44.000000 linora-2.0.0rc0/linora/data/_sql_io_dataset.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     1941 2022-06-01 08:26:01.000000 linora-2.0.0rc0/linora/data/_utils.py
+drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora/data/datasets/
+-rw-r--r--   0 liyanpeng   (501) staff       (20)       85 2022-08-19 09:00:53.000000 linora-2.0.0rc0/linora/data/datasets/__init__.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     2071 2022-12-01 09:47:11.000000 linora-2.0.0rc0/linora/data/datasets/_config_path.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)    19314 2022-06-08 08:37:02.000000 linora-2.0.0rc0/linora/data/datasets/_mnist.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     1293 2022-12-02 05:08:27.000000 linora-2.0.0rc0/linora/data/datasets/_utils.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)   264001 2022-08-22 01:29:59.000000 linora-2.0.0rc0/linora/data/datasets/_weather.py
+drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora/feature_column/
+-rw-r--r--   0 liyanpeng   (501) staff       (20)      277 2023-03-22 09:25:19.000000 linora-2.0.0rc0/linora/feature_column/__init__.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)    20098 2023-03-21 09:04:16.000000 linora-2.0.0rc0/linora/feature_column/_categorical.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     7622 2023-03-23 09:40:18.000000 linora-2.0.0rc0/linora/feature_column/_datetime.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     6523 2023-03-24 06:31:58.000000 linora-2.0.0rc0/linora/feature_column/_feature.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)    10691 2023-03-21 02:03:11.000000 linora-2.0.0rc0/linora/feature_column/_feature_categorical.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     3687 2023-03-23 09:10:38.000000 linora-2.0.0rc0/linora/feature_column/_feature_datetime.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     5298 2023-03-21 02:03:40.000000 linora-2.0.0rc0/linora/feature_column/_feature_normalize.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)    11083 2023-03-24 01:40:41.000000 linora-2.0.0rc0/linora/feature_column/_feature_numerical.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     8774 2023-03-21 09:03:05.000000 linora-2.0.0rc0/linora/feature_column/_normalize.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)    21492 2023-03-24 01:26:31.000000 linora-2.0.0rc0/linora/feature_column/_numerical.py
+drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora/feature_column/boundary/
+-rw-r--r--   0 liyanpeng   (501) staff       (20)       55 2022-04-24 14:02:43.000000 linora-2.0.0rc0/linora/feature_column/boundary/__init__.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     3495 2022-04-24 14:02:43.000000 linora-2.0.0rc0/linora/feature_column/boundary/_boundary.py
+drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora/feature_selection/
+-rw-r--r--   0 liyanpeng   (501) staff       (20)       94 2022-04-24 14:02:43.000000 linora-2.0.0rc0/linora/feature_selection/__init__.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     1780 2022-04-24 14:02:43.000000 linora-2.0.0rc0/linora/feature_selection/_credit.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     2622 2022-05-12 01:17:51.000000 linora-2.0.0rc0/linora/feature_selection/_select.py
+drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora/gfile/
+-rw-r--r--   0 liyanpeng   (501) staff       (20)       33 2022-04-24 14:02:43.000000 linora-2.0.0rc0/linora/gfile/__init__.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     5895 2022-11-23 09:16:08.000000 linora-2.0.0rc0/linora/gfile/_gfile.py
+drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora/image/
+-rw-r--r--   0 liyanpeng   (501) staff       (20)      636 2022-05-16 10:12:12.000000 linora-2.0.0rc0/linora/image/__init__.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     1442 2022-05-26 02:08:30.000000 linora-2.0.0rc0/linora/image/_image_aug.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     3596 2022-05-18 00:54:35.000000 linora-2.0.0rc0/linora/image/_image_box.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)    29992 2022-11-30 09:53:59.000000 linora-2.0.0rc0/linora/image/_image_color.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)    12038 2022-05-26 02:07:59.000000 linora-2.0.0rc0/linora/image/_image_color_aug.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     8666 2022-05-16 09:32:03.000000 linora-2.0.0rc0/linora/image/_image_crop.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     2963 2022-05-26 02:08:58.000000 linora-2.0.0rc0/linora/image/_image_crop_aug.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)    11337 2022-05-27 06:56:17.000000 linora-2.0.0rc0/linora/image/_image_draw.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     2305 2022-05-27 07:05:28.000000 linora-2.0.0rc0/linora/image/_image_draw_aug.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)    16607 2022-11-18 03:22:32.000000 linora-2.0.0rc0/linora/image/_image_feature.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     8805 2022-05-13 01:24:35.000000 linora-2.0.0rc0/linora/image/_image_filter.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     5629 2022-05-26 02:09:23.000000 linora-2.0.0rc0/linora/image/_image_filter_aug.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     7215 2022-08-01 08:30:47.000000 linora-2.0.0rc0/linora/image/_image_grid.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     2693 2023-03-22 09:47:31.000000 linora-2.0.0rc0/linora/image/_image_io.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     2345 2022-05-22 03:19:04.000000 linora-2.0.0rc0/linora/image/_image_io_aug.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)    13075 2022-05-17 03:28:28.000000 linora-2.0.0rc0/linora/image/_image_noise.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     7787 2022-05-26 02:09:49.000000 linora-2.0.0rc0/linora/image/_image_noise_aug.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     8431 2022-04-25 13:29:23.000000 linora-2.0.0rc0/linora/image/_image_pairs.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)    21630 2022-05-25 09:46:33.000000 linora-2.0.0rc0/linora/image/_image_position.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)    12989 2022-05-26 02:40:18.000000 linora-2.0.0rc0/linora/image/_image_position_aug.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     7012 2022-05-16 02:51:05.000000 linora-2.0.0rc0/linora/image/_image_rescale.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     4257 2022-05-26 02:10:15.000000 linora-2.0.0rc0/linora/image/_image_rescale_aug.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     2527 2022-05-25 02:36:08.000000 linora-2.0.0rc0/linora/image/_image_resize.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)      519 2022-05-09 09:56:14.000000 linora-2.0.0rc0/linora/image/_image_resize_aug.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)    41696 2022-05-27 06:48:41.000000 linora-2.0.0rc0/linora/image/_image_rgb.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     5315 2023-04-14 07:37:25.000000 linora-2.0.0rc0/linora/image/_image_util.py
+drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora/metrics/
+-rw-r--r--   0 liyanpeng   (501) staff       (20)      231 2022-04-24 14:02:43.000000 linora-2.0.0rc0/linora/metrics/__init__.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)    27844 2022-06-22 02:45:29.000000 linora-2.0.0rc0/linora/metrics/_classification.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     4966 2022-05-26 08:02:56.000000 linora-2.0.0rc0/linora/metrics/_image.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     2335 2022-05-26 07:22:49.000000 linora-2.0.0rc0/linora/metrics/_metrics.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     2568 2022-06-21 10:20:14.000000 linora-2.0.0rc0/linora/metrics/_rank.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)    18341 2022-11-21 07:42:50.000000 linora-2.0.0rc0/linora/metrics/_regression.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     2518 2023-02-24 06:52:37.000000 linora-2.0.0rc0/linora/metrics/_text.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)      370 2022-06-21 10:10:45.000000 linora-2.0.0rc0/linora/metrics/_utils.py
+drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora/metrics/distance/
+-rw-r--r--   0 liyanpeng   (501) staff       (20)       97 2022-04-24 14:02:43.000000 linora-2.0.0rc0/linora/metrics/distance/__init__.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)    10758 2022-06-22 01:50:38.000000 linora-2.0.0rc0/linora/metrics/distance/_distance.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     5635 2022-04-24 14:02:43.000000 linora-2.0.0rc0/linora/metrics/distance/_divergence.py
+drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora/parallel/
+-rw-r--r--   0 liyanpeng   (501) staff       (20)       77 2022-04-24 14:02:43.000000 linora-2.0.0rc0/linora/parallel/__init__.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     5619 2022-04-24 14:02:43.000000 linora-2.0.0rc0/linora/parallel/_process.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     5408 2022-04-24 14:02:43.000000 linora-2.0.0rc0/linora/parallel/_thread.py
+drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora/param_search/
+drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora/param_search/GEClassifier/
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     2941 2022-04-24 14:02:43.000000 linora-2.0.0rc0/linora/param_search/GEClassifier/_GridSearch.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     3182 2022-04-24 14:02:43.000000 linora-2.0.0rc0/linora/param_search/GEClassifier/_RandomSearch.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)      142 2022-04-24 14:02:43.000000 linora-2.0.0rc0/linora/param_search/GEClassifier/__init__.py
+drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora/param_search/GERegressor/
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     3219 2022-04-24 14:02:43.000000 linora-2.0.0rc0/linora/param_search/GERegressor/_RandomSearch.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)       71 2022-04-24 14:02:43.000000 linora-2.0.0rc0/linora/param_search/GERegressor/__init__.py
+drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora/param_search/LGBMClassifier/
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     7659 2022-05-20 03:53:11.000000 linora-2.0.0rc0/linora/param_search/LGBMClassifier/_GridSearch.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     7646 2022-05-20 03:52:49.000000 linora-2.0.0rc0/linora/param_search/LGBMClassifier/_RandomSearch.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)      144 2022-05-05 06:13:26.000000 linora-2.0.0rc0/linora/param_search/LGBMClassifier/__init__.py
+drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora/param_search/LGBMRegressor/
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     7656 2022-05-20 03:53:26.000000 linora-2.0.0rc0/linora/param_search/LGBMRegressor/_GridSearch.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     7644 2022-05-20 03:52:33.000000 linora-2.0.0rc0/linora/param_search/LGBMRegressor/_RandomSearch.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)      141 2022-05-05 06:14:26.000000 linora-2.0.0rc0/linora/param_search/LGBMRegressor/__init__.py
+drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora/param_search/XGBClassifier/
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     8752 2022-05-20 03:51:53.000000 linora-2.0.0rc0/linora/param_search/XGBClassifier/_GridSearch.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     8724 2022-05-20 03:52:15.000000 linora-2.0.0rc0/linora/param_search/XGBClassifier/_RandomSearch.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)      142 2022-04-24 14:02:43.000000 linora-2.0.0rc0/linora/param_search/XGBClassifier/__init__.py
+drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora/param_search/XGBRanker/
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     5599 2022-04-24 14:02:43.000000 linora-2.0.0rc0/linora/param_search/XGBRanker/_GridSearch.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     5904 2022-04-24 14:02:43.000000 linora-2.0.0rc0/linora/param_search/XGBRanker/_RandomSearch.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)      138 2022-04-24 14:02:43.000000 linora-2.0.0rc0/linora/param_search/XGBRanker/__init__.py
+drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora/param_search/XGBRegressor/
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     8912 2022-05-20 03:51:33.000000 linora-2.0.0rc0/linora/param_search/XGBRegressor/_GridSearch.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     8943 2022-05-20 03:51:09.000000 linora-2.0.0rc0/linora/param_search/XGBRegressor/_RandomSearch.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)      140 2022-04-24 14:02:43.000000 linora-2.0.0rc0/linora/param_search/XGBRegressor/__init__.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)    13838 2022-06-15 06:08:40.000000 linora-2.0.0rc0/linora/param_search/_HyperParameters.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     9259 2023-03-27 01:31:53.000000 linora-2.0.0rc0/linora/param_search/_Search.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)      177 2022-06-08 09:41:40.000000 linora-2.0.0rc0/linora/param_search/__init__.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     9231 2022-05-22 02:43:27.000000 linora-2.0.0rc0/linora/param_search/_config.py
+drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora/sample/
+-rw-r--r--   0 liyanpeng   (501) staff       (20)      162 2022-05-10 08:08:14.000000 linora-2.0.0rc0/linora/sample/__init__.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     4847 2022-11-04 06:31:17.000000 linora-2.0.0rc0/linora/sample/_fold.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     3542 2022-04-24 14:02:43.000000 linora-2.0.0rc0/linora/sample/_random_walker.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     7072 2022-11-24 03:05:14.000000 linora-2.0.0rc0/linora/sample/_sampling.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     4051 2022-04-27 01:42:13.000000 linora-2.0.0rc0/linora/sample/_timeseries_kfold.py
+drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora/server/
+-rw-r--r--   0 liyanpeng   (501) staff       (20)      109 2023-03-28 05:08:20.000000 linora-2.0.0rc0/linora/server/__init__.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)    19067 2023-03-27 01:12:25.000000 linora-2.0.0rc0/linora/server/_email.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)    17119 2023-03-27 01:12:06.000000 linora-2.0.0rc0/linora/server/_email_utils.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)    13495 2023-03-27 00:57:47.000000 linora-2.0.0rc0/linora/server/_schedulers.py
+drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora/server/message/
+-rw-r--r--   0 liyanpeng   (501) staff       (20)    11784 2022-06-14 08:26:34.000000 linora-2.0.0rc0/linora/server/message/_BotDingTalk.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)      520 2022-04-24 14:02:43.000000 linora-2.0.0rc0/linora/server/message/_BotFeiShu.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)       95 2023-03-28 05:07:33.000000 linora-2.0.0rc0/linora/server/message/__init__.py
+drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora/text/
+-rw-r--r--   0 liyanpeng   (501) staff       (20)      149 2022-04-24 14:02:43.000000 linora-2.0.0rc0/linora/text/__init__.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     6243 2022-04-24 14:02:43.000000 linora-2.0.0rc0/linora/text/_sequence.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     4002 2022-04-24 14:02:43.000000 linora-2.0.0rc0/linora/text/_util.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     2267 2022-04-24 14:02:43.000000 linora-2.0.0rc0/linora/text/_vectorizer.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     3037 2023-02-24 05:40:38.000000 linora-2.0.0rc0/linora/text/_word_processing.py
+drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora/train/
+-rw-r--r--   0 liyanpeng   (501) staff       (20)      308 2022-08-24 08:42:12.000000 linora-2.0.0rc0/linora/train/__init__.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     2922 2022-09-01 01:52:14.000000 linora-2.0.0rc0/linora/train/_callback.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     1781 2022-08-24 02:28:50.000000 linora-2.0.0rc0/linora/train/_csvlogger.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     2371 2022-08-25 05:33:20.000000 linora-2.0.0rc0/linora/train/_earlystopping.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     1768 2022-08-24 02:54:41.000000 linora-2.0.0rc0/linora/train/_modelcheckpoint.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     2193 2022-08-24 01:53:17.000000 linora-2.0.0rc0/linora/train/_remotemonitor.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     2180 2022-09-01 01:55:31.000000 linora-2.0.0rc0/linora/train/_terminateonnan.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     7364 2022-08-27 02:43:20.000000 linora-2.0.0rc0/linora/train/_visual.py
+drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora/train/lr/
+-rw-r--r--   0 liyanpeng   (501) staff       (20)       75 2022-08-25 02:12:32.000000 linora-2.0.0rc0/linora/train/lr/__init__.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)    12872 2022-08-26 07:47:29.000000 linora-2.0.0rc0/linora/train/lr/_lr.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     1991 2022-08-25 03:30:35.000000 linora-2.0.0rc0/linora/train/lr/_schedulers.py
+drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora/utils/
+-rw-r--r--   0 liyanpeng   (501) staff       (20)      241 2022-11-10 02:19:13.000000 linora-2.0.0rc0/linora/utils/__init__.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     1444 2022-04-24 14:02:43.000000 linora-2.0.0rc0/linora/utils/_config.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)    19259 2023-03-27 01:06:27.000000 linora-2.0.0rc0/linora/utils/_email.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)    17119 2022-11-23 01:25:02.000000 linora-2.0.0rc0/linora/utils/_email_utils.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     9213 2022-05-11 03:45:54.000000 linora-2.0.0rc0/linora/utils/_logger.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     4106 2022-05-31 11:52:27.000000 linora-2.0.0rc0/linora/utils/_progbar.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)    13658 2023-03-27 01:10:43.000000 linora-2.0.0rc0/linora/utils/_schedulers.py
+drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora/utils/message/
+-rw-r--r--   0 liyanpeng   (501) staff       (20)    11965 2023-03-28 05:06:17.000000 linora-2.0.0rc0/linora/utils/message/_BotDingTalk.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)      739 2023-03-28 05:05:36.000000 linora-2.0.0rc0/linora/utils/message/_BotFeiShu.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)       93 2023-03-28 05:03:07.000000 linora-2.0.0rc0/linora/utils/message/__init__.py
+drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora/utils/pip/
+-rw-r--r--   0 liyanpeng   (501) staff       (20)       35 2022-08-04 02:59:58.000000 linora-2.0.0rc0/linora/utils/pip/__init__.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)    14751 2022-08-05 04:59:06.000000 linora-2.0.0rc0/linora/utils/pip/_pip.py
+drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora/vedio/
+-rw-r--r--   0 liyanpeng   (501) staff       (20)       75 2023-04-14 07:02:50.000000 linora-2.0.0rc0/linora/vedio/__init__.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)    17841 2023-04-27 07:03:50.000000 linora-2.0.0rc0/linora/vedio/_vedio_io.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     3801 2023-04-23 08:50:15.000000 linora-2.0.0rc0/linora/vedio/_vedio_util.py
+drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora.egg-info/
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     3736 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora.egg-info/PKG-INFO
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     5603 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora.egg-info/SOURCES.txt
+-rw-r--r--   0 liyanpeng   (501) staff       (20)        1 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora.egg-info/dependency_links.txt
+-rw-r--r--   0 liyanpeng   (501) staff       (20)        1 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora.egg-info/not-zip-safe
+-rw-r--r--   0 liyanpeng   (501) staff       (20)       67 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora.egg-info/requires.txt
+-rw-r--r--   0 liyanpeng   (501) staff       (20)        7 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora.egg-info/top_level.txt
+-rw-r--r--   0 liyanpeng   (501) staff       (20)       79 2023-04-28 01:24:56.000000 linora-2.0.0rc0/setup.cfg
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     1631 2023-03-21 02:28:13.000000 linora-2.0.0rc0/setup.py
```

### Comparing `linora-1.6.0/PKG-INFO` & `linora-2.0.0rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linora
-Version: 1.6.0
+Version: 2.0.0rc0
 Summary: Simple and efficient tools for data mining and data analysis.
 Home-page: https://github.com/Hourout/linora
 Author: JinQing Lee
 Author-email: hourout@163.com
 License: Apache License Version 2.0
 Description: ![](https://github.com/Hourout/linora/blob/master/image/linora.png)
```

### Comparing `linora-1.6.0/README.md` & `linora-2.0.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/chart/_arrow.py` & `linora-2.0.0rc0/linora/chart/_arrow.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/chart/_bar.py` & `linora-2.0.0rc0/linora/chart/_bar.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/chart/_base.py` & `linora-2.0.0rc0/linora/chart/_base.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/chart/_boxplot.py` & `linora-2.0.0rc0/linora/chart/_boxplot.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/chart/_circle.py` & `linora-2.0.0rc0/linora/chart/_circle.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/chart/_coherence.py` & `linora-2.0.0rc0/linora/chart/_coherence.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/chart/_config.py` & `linora-2.0.0rc0/linora/chart/_config.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/chart/_csd.py` & `linora-2.0.0rc0/linora/chart/_csd.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/chart/_ellipse.py` & `linora-2.0.0rc0/linora/chart/_ellipse.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/chart/_errorbar.py` & `linora-2.0.0rc0/linora/chart/_errorbar.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/chart/_feature.py` & `linora-2.0.0rc0/linora/chart/_feature.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/chart/_fillline.py` & `linora-2.0.0rc0/linora/chart/_fillline.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/chart/_grid.py` & `linora-2.0.0rc0/linora/chart/_grid.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/chart/_hist.py` & `linora-2.0.0rc0/linora/chart/_hist.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/chart/_hist2d.py` & `linora-2.0.0rc0/linora/chart/_hist2d.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/chart/_hlines.py` & `linora-2.0.0rc0/linora/chart/_hlines.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/chart/_line.py` & `linora-2.0.0rc0/linora/chart/_line.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/chart/_line3D.py` & `linora-2.0.0rc0/linora/chart/_line3D.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/chart/_metrics.py` & `linora-2.0.0rc0/linora/chart/_metrics.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/chart/_pie.py` & `linora-2.0.0rc0/linora/chart/_pie.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/chart/_plot.py` & `linora-2.0.0rc0/linora/chart/_plot.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/chart/_polygon.py` & `linora-2.0.0rc0/linora/chart/_polygon.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/chart/_radar.py` & `linora-2.0.0rc0/linora/chart/_radar.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/chart/_rectangle.py` & `linora-2.0.0rc0/linora/chart/_rectangle.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/chart/_regularpolygon.py` & `linora-2.0.0rc0/linora/chart/_regularpolygon.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/chart/_scatter.py` & `linora-2.0.0rc0/linora/chart/_scatter.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/chart/_scatter3D.py` & `linora-2.0.0rc0/linora/chart/_scatter3D.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/chart/_vlines.py` & `linora-2.0.0rc0/linora/chart/_vlines.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/chart/_wedge.py` & `linora-2.0.0rc0/linora/chart/_wedge.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/data/Dataset/_data.py` & `linora-2.0.0rc0/linora/data/Dataset/_data.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/data/Dataset/_dataset.py` & `linora-2.0.0rc0/linora/data/Dataset/_dataset.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/data/TextLineDataset/_dataset.py` & `linora-2.0.0rc0/linora/data/TextLineDataset/_dataset.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/data/_compress.py` & `linora-2.0.0rc0/linora/data/_compress.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/data/_sql_io_dataset.py` & `linora-2.0.0rc0/linora/data/_sql_io_dataset.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/data/_utils.py` & `linora-2.0.0rc0/linora/data/_utils.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/data/datasets/_config_path.py` & `linora-2.0.0rc0/linora/data/datasets/_config_path.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/data/datasets/_mnist.py` & `linora-2.0.0rc0/linora/data/datasets/_mnist.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/data/datasets/_utils.py` & `linora-2.0.0rc0/linora/data/datasets/_utils.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/data/datasets/_weather.py` & `linora-2.0.0rc0/linora/data/datasets/_weather.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/feature_column/_categorical.py` & `linora-2.0.0rc0/linora/feature_column/_categorical.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import pandas as pd
 import numpy as np
 
 __all__ = ['categorical_count', 'categorical_crossed','categorical_encoder', 
            'categorical_hash', 'categorical_hist',
            'categorical_onehot_binarizer', 'categorical_onehot_multiple',
-           'categorical_regress', 
+           'categorical_rare', 'categorical_regress', 'categorical_woe'
           ]
 
 
 def categorical_count(feature, mode=0, normalize=True, abnormal_value=0, miss_value=0, name=None, config=None):
     """Count or frequency of conversion category variables.
     
     Args:
@@ -21,49 +21,50 @@
         normalize: bool, If True then the object returned will contain the relative frequencies of the unique values.
         abnormal_value: int or float, if feature values not in feature_scale dict, return `abnormal_value`.
         miss_value: int or float, if feature values are missing, return `miss_value`.
         name: str, output feature name, if None, name is feature.name .
         config: dict, label parameters dict for this estimator. 
             if config is not None, only parameter `feature` and `mode` is invalid.
     Returns:
-        return count labels and label parameters dict.
+        Refer to params `mode` explanation.
     """
     if config is None:
-        config = {'feature_scale':feature.value_counts(normalize).to_dict(),
-                  'abnormal_value':abnormal_value, 'miss_value':miss_value, 
-                  'type':'categorical_count', 'name_input':feature.name, 
-                  'name_output':feature.name if name is None else name}
+        config = {'param':{'feature_scale':feature.value_counts(normalize).to_dict(),
+                           'normalize':normalize, 'abnormal_value':abnormal_value, 
+                           'miss_value':miss_value, 'name':feature.name if name is None else name},
+                  'type':'categorical_count', 'variable':feature.name}
     if mode==2:
         return config
     else:
-        scale = {**config['feature_scale'], **{i:config['abnormal_value'] for i in feature.unique().tolist() if i not in config['feature_scale']}}
-        t = feature.replace(scale).fillna(config['miss_value']).rename(config['name_output'])
+        scale = {**config['param']['feature_scale'], **{i:config['param']['abnormal_value'] for i in feature.unique().tolist() if i not in config['param']['feature_scale']}}
+        t = feature.replace(scale).fillna(config['param']['miss_value']).rename(config['param']['name'])
         return t if mode else (t, config)
 
 
 def categorical_crossed(feature_list, mode=0, hash_bucket_size=3, name=None, config=None):
     """Crossed categories and hash labels with value between 0 and hash_bucket_size-1.
     
     Args:
         feature_list: pd.Series list, sample feature list.
         mode: if 0, output (transform feature, config); if 1, output transform feature; if 2, output config.
         hash_bucket_size: int, number of categories that need hash.
-        name: str, output feature name, if None, name is feature.name .
+        name: str, output feature name.
         config: dict, label parameters dict for this estimator. 
             if config is not None, only parameter `feature_list` and `mode` is invalid.
     Returns:
-        return hash labels.
+        Refer to params `mode` explanation.
     """
     if config is None:
-        config = {'hash_bucket_size':hash_bucket_size, 'type':'categorical_crossed', 
-                  'name_input':[i.name for i in feature_list], 'name_output':name}
+        config = {'param':{'hash_bucket_size':hash_bucket_size, 
+                           'name':'_'.join(name)+'_crossed' if name is None else name}, 
+                  'type':'categorical_crossed', 'variable':[i.name for i in feature_list]}
     if mode==2:
         return config
     else:
-        t = reduce(lambda x,y:x+y, [i.fillna('').astype(str) for i in feature_list]).map(lambda x:hash(x)).rename(config['name_output'])%config['hash_bucket_size']
+        t = reduce(lambda x,y:x+y, [i.fillna('').astype(str) for i in feature_list]).map(lambda x:hash(x)).rename(config['param']['name'])%config['param']['hash_bucket_size']
         return t if mode else (t, config)
 
 
 def categorical_encoder(feature, mode=0, abnormal_value=-1, miss_value=-1, name=None, config=None):
     """Encode labels with value between 0 and n_classes-1.
     
     Args:
@@ -71,49 +72,50 @@
         mode: if 0, output (transform feature, config); if 1, output transform feature; if 2, output config.
         abnormal_value: int, if feature values not in feature_scale dict, return `abnormal_value`.
         miss_value: int or float, if feature values are missing, return `miss_value`.
         name: str, output feature name, if None, name is feature.name .
         config: dict, label parameters dict for this estimator. 
             if config is not None, only parameter `feature` and `mode` is invalid.
     Returns:
-        return encoded labels and label parameters dict.
+        Refer to params `mode` explanation.
     """
     if config is None:
-        config = {'feature_scale':{j:i for i,j in feature.drop_duplicates().reset_index(drop=True).to_dict().items()},
-                  'abnormal_value':abnormal_value, 'miss_value':miss_value, 
-                  'type':'categorical_encoder', 'name_input':feature.name, 
-                  'name_output':feature.name if name is None else name}
+        config = {'param':{'feature_scale':{j:i for i,j in feature.drop_duplicates().reset_index(drop=True).to_dict().items()},
+                           'abnormal_value':abnormal_value, 'miss_value':miss_value, 
+                           'name':feature.name if name is None else name},
+                  'type':'categorical_encoder', 'variable':feature.name}
     if mode==2:
         return config
     else:
-        scale = {**config['feature_scale'], **{i:config['abnormal_value'] for i in feature.unique().tolist() if i not in config['feature_scale']}}
-        t = feature.replace(scale).fillna(config['miss_value']).rename(config['name_output'])
+        scale = {**config['param']['feature_scale'], **{i:config['param']['abnormal_value'] for i in feature.unique().tolist() if i not in config['param']['feature_scale']}}
+        t = feature.replace(scale).fillna(config['param']['miss_value']).rename(config['param']['name'])
         return t if mode else (t, config)
 
 
 def categorical_hash(feature, mode=0, hash_bucket_size=3, name=None, config=None):
     """Hash labels with value between 0 and hash_bucket_size-1.
     
     Args:
         feature: pd.Series, sample feature.
         mode: if 0, output (transform feature, config); if 1, output transform feature; if 2, output config.
         hash_bucket_size: int, number of categories that need hash.
         name: str, output feature name, if None, name is feature.name .
         config: dict, label parameters dict for this estimator. 
             if config is not None, only parameter `feature` and `mode` is invalid.
     Returns:
-        return hash labels.
+        Refer to params `mode` explanation.
     """
     if config is None:
-        config = {'hash_bucket_size':hash_bucket_size, 'type':'categorical_hash', 
-                  'name_input':feature.name, 'name_output':feature.name if name is None else name}
+        config = {'param':{'hash_bucket_size':hash_bucket_size, 
+                           'name':feature.name if name is None else name},
+                  'type':'categorical_hash', 'variable':feature.name}
     if mode==2:
         return config
     else:
-        t = feature.fillna('').astype(str).map(lambda x:hash(x)).rename(config['name_output'])%config['hash_bucket_size']
+        t = feature.fillna('').astype(str).map(lambda x:hash(x)).rename(config['param']['name'])%config['param']['hash_bucket_size']
         return t if mode else (t, config)
 
 
 def categorical_hist(feature, label, mode=0, abnormal_value=0, miss_value=0, name=None, config=None):
     """Hist labels with value counts prob.
            
     Args:
@@ -122,30 +124,32 @@
         mode: if 0, output (transform feature, config); if 1, output transform feature; if 2, output config.
         abnormal_value: int, if feature values not in feature_scale dict, return `abnormal_value`.
         miss_value: int or float, if feature values are missing, return `miss_value`.
         name: str, output feature name, if None, name is feature.name .
         config: dict, label parameters dict for this estimator. 
             if config is not None, only parameter `feature` and `mode` is invalid, but `label` must be passed in.
     Returns:
-        return hist labels and label parameters DataFrame.
+        Refer to params `mode` explanation.
     """
     if config is None:
-        config = {'feature_scale':None,
-                  'abnormal_value':abnormal_value, 'miss_value':miss_value, 
-                  'type':'categorical_hist', 'name_input':[feature.name, label.name], 
-                  'name_output':feature.name if name is None else name}
+        config = {'param':{'feature_scale':None,
+                           'abnormal_value':abnormal_value, 'miss_value':miss_value, 
+                           'name':feature.name if name is None else name},
+                  'type':'categorical_hist', 'variable':feature.name, 'label':label.name}
         t = pd.concat([feature, label], axis=1).groupby([feature.name])[label.name].value_counts(normalize=True).unstack()
-        t.columns = [config['name_output']+'_'+str(i) for i in t.columns]
-        config['feature_scale'] = t.reset_index().to_dict()
+        t.columns = [config['param']['name']+'_'+str(i) for i in t.columns]
+        config['param']['feature_scale'] = t.reset_index().to_dict()
         
     if mode==2:
         return config
     else:
-        t = (feature.to_frame().merge(pd.DataFrame(config['feature_scale']).fillna(config['miss_value']), on=feature.name, how='left')
-             .drop([feature.name], axis=1).fillna(config['abnormal_value']).rename(config['name_output']))
+        t = (feature.to_frame()
+             .merge(pd.DataFrame(config['param']['feature_scale'])
+                    .fillna(config['param']['miss_value']), on=feature.name, how='left')
+             .drop([feature.name], axis=1).fillna(config['param']['abnormal_value']).rename(config['param']['name']))
         return t if mode else (t, config)
 
 
 def categorical_onehot_binarizer(feature, mode=0, abnormal_value=0, miss_value=0, name=None, config=None):
     """Transform between iterable of iterables and a multilabel format, sample is simple categories.
     
     Args:
@@ -153,40 +157,43 @@
         mode: if 0, output (transform feature, config); if 1, output transform feature; if 2, output config.
         abnormal_value: int, if feature values not in feature_scale dict, return `abnormal_value`.
         miss_value: int or float, if feature values are missing, return `miss_value`.
         name: str, output feature name, if None, name is feature.name .
         config: dict, label parameters dict for this estimator. 
             if config is not None, only parameter `feature` and `mode` is invalid.
     Returns:
-        Dataframe for onehot binarizer and feature parameters list.
+        Refer to params `mode` explanation.
     """
     if config is None:
-        config = {'feature_scale':feature.dropna().drop_duplicates().tolist(),
-                  'abnormal_value':abnormal_value, 'miss_value':miss_value, 
-                  'type':'categorical_onehot_binarizer', 'name_input':feature.name, 
-                  'name_output':feature.name if name is None else name}
+        config = {'param':{'feature_scale':feature.dropna().drop_duplicates().tolist(),
+                           'abnormal_value':abnormal_value, 'miss_value':miss_value, 
+                           'name':feature.name if name is None else name},
+                  'type':'categorical_onehot_binarizer', 'variable':feature.name}
     if mode==2:
         return config
     else:
         scale = feature.dropna().drop_duplicates().tolist()
-        scale_dict = {i:'temp_str' for i in set.difference(set(scale), set(config['feature_scale']))}
-        t = pd.get_dummies(feature.replace(scale_dict), prefix=config['name_output'], dtype='int8', dummy_na=True)
+        scale_dict = {i:'temp_str' for i in set.difference(set(scale), set(config['param']['feature_scale']))}
+        if feature.dtype.char=='O':
+            t = pd.get_dummies(feature.replace(scale_dict), prefix=config['param']['name'], dtype='int8', dummy_na=True)
+        else:
+            t = pd.get_dummies(feature.replace(scale_dict).astype(str), prefix=config['param']['name'], dtype='int8', dummy_na=True)
         
-        for i in set.difference(set(config['feature_scale']), set(scale)):
-            if config['name_output']+'_'+str(i) not in t.columns:
-                t[config['name_output']+'_'+str(i)] = 0
+        for i in set.difference(set(config['param']['feature_scale']), set(scale)):
+            if config['param']['name']+'_'+str(i) not in t.columns:
+                t[config['param']['name']+'_'+str(i)] = 0
                 
-        if f"{config['name_output']}_temp_str" in t.columns:
-            t.loc[t[f"{config['name_output']}_temp_str"]==1, :] = config['abnormal_value']
-            t = t.drop([f"{config['name_output']}_temp_str"], axis=1)
+        if f"{config['param']['name']}_temp_str" in t.columns:
+            t.loc[t[f"{config['param']['name']}_temp_str"]==1, :] = config['param']['abnormal_value']
+            t = t.drop([f"{config['param']['name']}_temp_str"], axis=1)
             
-        if f"{config['name_output']}_nan" in t.columns:
-            t.loc[t[f"{config['name_output']}_nan"]==1, :] = config['miss_value']
-            t = t.drop([f"{config['name_output']}_nan"], axis=1)
-        t = t[[config['name_output']+'_'+str(i) for i in config['feature_scale']]]
+        if f"{config['param']['name']}_nan" in t.columns:
+            t.loc[t[f"{config['param']['name']}_nan"]==1, :] = config['param']['miss_value']
+            t = t.drop([f"{config['param']['name']}_nan"], axis=1)
+        t = t[[config['param']['name']+'_'+str(i) for i in config['param']['feature_scale']]]
         return t if mode else (t, config)
 
 
 def categorical_onehot_multiple(feature, mode=0, abnormal_value=0, miss_value=0, name=None, config=None):
     """Transform between iterable of iterables and a multilabel format, sample is multiple categories.
     
     Args:
@@ -194,43 +201,95 @@
         mode: if 0, output (transform feature, config); if 1, output transform feature; if 2, output config.
         abnormal_value: int, if feature values not in feature_scale dict, return `abnormal_value`.
         miss_value: int or float, if feature values are missing, return `miss_value`.
         name: str, output feature name, if None, name is feature.name .
         config: dict, label parameters dict for this estimator. 
             if config is not None, only parameter `feature` and `mode` is invalid.
     Returns:
-        Dataframe for onehot binarizer and feature parameters list.
+        Refer to params `mode` explanation.
     """
     if config is None:
-        config = {'feature_scale':list(set(itertools.chain.from_iterable(feature.dropna()))),
-                  'abnormal_value':abnormal_value, 'miss_value':miss_value, 
-                  'type':'categorical_onehot_multiple', 'name_input':feature.name, 
-                  'name_output':feature.name if name is None else name}
+        config = {'param':{'feature_scale':list(set(itertools.chain.from_iterable(feature.dropna()))),
+                           'abnormal_value':abnormal_value, 'miss_value':miss_value, 
+                           'name':feature.name if name is None else name},
+                  'type':'categorical_onehot_multiple', 'variable':feature.name}
     if mode==2:
         return config
     else:
         scale = list(set(itertools.chain.from_iterable(feature.fillna('_'))))        
         class_mapping = defaultdict(int)
         class_mapping.default_factory = class_mapping.__len__
         [class_mapping[i] for i in scale]
         col = [class_mapping[i] for i in itertools.chain.from_iterable(feature.fillna('_'))]
         row = [i for i in itertools.chain.from_iterable(map(lambda x,y:[x]*len(y), range(len(feature)), feature.fillna('_')))]
         t = np.zeros([max(row)+1, len(class_mapping)], dtype='int8')
         t[row, col] = 1
-        t = pd.DataFrame(t, columns=[config['name_output']+'_'+str(i) for i in scale], index=feature.index)
+        t = pd.DataFrame(t, columns=[config['param']['name']+'_'+str(i) for i in scale], index=feature.index)
     
-        for i in set.difference(set(config['feature_scale']), set(scale)):
-            if config['name_output']+'_'+str(i) not in t.columns:
-                t[config['name_output']+'_'+str(i)] = 0
-
-        if f"{config['name_output']}__" in t.columns:
-            t.loc[t[f"{config['name_output']}__"]==1, :] = config['miss_value']
-            t = t.drop([f"{config['name_output']}__"], axis=1)
+        for i in set.difference(set(config['param']['feature_scale']), set(scale)):
+            if config['param']['name']+'_'+str(i) not in t.columns:
+                t[config['param']['name']+'_'+str(i)] = 0
+
+        if f"{config['param']['name']}__" in t.columns:
+            t.loc[t[f"{config['param']['name']}__"]==1, :] = config['param']['miss_value']
+            t = t.drop([f"{config['param']['name']}__"], axis=1)
         
-        t = t[[config['name_output']+'_'+str(i) for i in config['feature_scale']]]
+        t = t[[config['param']['name']+'_'+str(i) for i in config['param']['feature_scale']]]
+        return t if mode else (t, config)
+
+
+def categorical_rare(feature, mode=0, p=0.05, min_num=None, max_num=None, abnormal_value=-1, miss_value=-1, name=None, config=None):
+    """Groups rare or infrequent categories in a new category called “Rare”, or any other name entered by the user.
+    
+    Args:
+        feature: pd.Series, sample feature.
+        mode: if 0, output (transform feature, config); if 1, output transform feature; if 2, output config.
+        p: The minimum frequency a label should have to be considered frequent. Categories with frequencies lower than tol will be grouped.
+        min_num: The minimum number of categories a variable should have for the encoder to find frequent labels. 
+            If the variable contains less categories, all of them will be considered frequent.
+        max_num: The maximum number of categories that should be considered frequent. 
+            If None, all categories with frequency above the tolerance (tol) will be considered frequent. 
+            If you enter 5, only the 4 most frequent categories will be retained and the rest grouped.
+        abnormal_value: int or float, if feature values not in feature_scale dict, return `abnormal_value`.
+        miss_value: int or float, if feature values are missing, return `miss_value`.
+        name: str, output feature name, if None, name is feature.name .
+        config: dict, label parameters dict for this estimator. 
+            if config is not None, only parameter `feature` and `mode` is invalid.
+    Returns:
+        Refer to params `mode` explanation.
+    """
+    if config is None:
+        t = feature.value_counts(True)
+        if min_num is None:
+            min_num = len(t[t>p])
+        if max_num is None:
+            max_num = max(min_num, len(t[t>p])+1)
+        k = 1 if len(t[t<=p])>0 else 0
+        if len(t)<min_num:
+            feature_scale = {i:r for r, i in enumerate(t.index)}
+        elif len(t[t>p])+k<min_num:
+            feature_scale = {**{i:r for r, i in enumerate(t.iloc[:min_num-1].index)},
+                             **{i:min_num-1 for i in t.iloc[min_num-1:].index}}
+        elif len(t[t>p])+k>max_num:
+            feature_scale = {**{i:r for r, i in enumerate(t.iloc[:max_num-1].index)},
+                             **{i:max_num-1 for i in t.iloc[max_num-1:].index}}
+        else:
+            feature_scale = {**{i:r for r, i in enumerate(t[t>p].index)},
+                             **{i:len(t[t>p]) for i in t[t<=p].index}}
+            
+        config = {'param':{'feature_scale':feature_scale,
+                           'p':p, 'min_num':min_num, 'max_num':max_num,
+                           'abnormal_value':abnormal_value, 'miss_value':miss_value, 
+                           'name':feature.name if name is None else name},
+                  'type':'categorical_rare', 'variable':feature.name}
+    if mode==2:
+        return config
+    else:
+        scale = {**config['param']['feature_scale'], **{i:config['param']['abnormal_value'] for i in feature.unique().tolist() if i not in config['param']['feature_scale']}}
+        t = feature.replace(scale).fillna(config['param']['miss_value']).rename(config['param']['name'])
         return t if mode else (t, config)
 
 
 def categorical_regress(feature, label, mode=0, method='mean', abnormal_value='mean', miss_value='mean', name=None, config=None):
     """Regress labels with value counts prob.
     
     Args:
@@ -240,21 +299,60 @@
         method: 'mean' or 'median'
         abnormal_value: int, if feature values not in feature_scale dict, return `abnormal_value`.
         miss_value: int or float, if feature values are missing, return `miss_value`.
         name: str, output feature name, if None, name is feature.name .
         config: dict, label parameters dict for this estimator. 
             if config is not None, only parameter `feature` and `mode` is invalid, but `label` must be passed in.
     Returns:
-        return Regress labels and label parameters dict.
+        Refer to params `mode` explanation.
     """
     if config is None:
-        config = {'feature_scale':pd.concat([feature, label], axis=1).groupby([feature.name])[label.name].agg(method).to_dict(),
-                  'abnormal_value':label.mean() if abnormal_value=='mean' else label.median(), 
-                  'miss_value':label.mean() if miss_value=='mean' else label.median(), 
-                  'type':'categorical_regress', 'name_input':[feature.name, label.name], 
-                  'name_output':feature.name if name is None else name}
+        config = {'param':{'method':method,
+                           'feature_scale':pd.concat([feature, label], axis=1).groupby([feature.name])[label.name].agg(method).to_dict(),
+                           'abnormal_value':label.mean() if abnormal_value=='mean' else label.median(), 
+                           'miss_value':label.mean() if miss_value=='mean' else label.median(), 
+                           'name':feature.name if name is None else name},
+                  'type':'categorical_regress', 'variable':feature.name, 'label':label.name}
     if mode==2:
         return config
     else:
-        scale = {**config['feature_scale'], **{i:config['abnormal_value'] for i in feature.unique().tolist() if i not in config['feature_scale']}}
-        t = feature.replace(scale).fillna(config['miss_value']).rename(config['name_output'])
+        scale = {**config['param']['feature_scale'], **{i:config['param']['abnormal_value'] for i in feature.unique().tolist() if i not in config['param']['feature_scale']}}
+        t = feature.replace(scale).fillna(config['param']['miss_value']).rename(config['param']['name'])
         return t if mode else (t, config)
+
+    
+def categorical_woe(feature, label, mode=0, pos_label=1, abnormal_value=-1, miss_value=-1, name=None, config=None):
+    """Calculate series woe value
+    
+    Args:
+        feature: pd.Series, shape (n_samples,) x variable, model feature.
+        label: pd.Series, sample categorical label.
+        mode: if 0, output (transform feature, config); if 1, output transform feature; if 2, output config.
+        pos_label: int, default=1, positive label value.
+        abnormal_value: int, if feature values not in feature_scale dict, return `abnormal_value`.
+        miss_value: int or float, if feature values are missing, return `miss_value`.
+        name: str, output feature name, if None, name is feature.name .
+        config: dict, label parameters dict for this estimator. 
+            if config is not None, only parameter `feature` and `mode` is invalid, but `label` must be passed in.
+    Return:
+        Refer to params `mode` explanation.
+    """
+    if config is None:
+        t = pd.DataFrame({'label':label, 'feature':feature})
+        assert t.label.nunique()==2, "`y_true` should be binary classification."
+        label_dict = {i:1 if i==pos_label else 0 for i in t.label.unique()}
+        t['label'] = t.label.replace(label_dict)
+        corr = t.label.sum()/(t.label.count()-t.label.sum())
+        t = t.groupby(['feature']).label.apply(lambda x:np.log(x.sum()/(x.count()-x.sum())/corr))
+        
+        config = {'param':{'pos_label':pos_label, 'feature_scale':t.to_dict(),
+                           'abnormal_value':abnormal_value, 'miss_value':miss_value, 
+                           'name':feature.name if name is None else name},
+                  'type':'categorical_woe', 'variable':feature.name, 'label':label.name}
+    if mode==2:
+        return config
+    else:
+        scale = {**config['param']['feature_scale'], **{i:config['param']['abnormal_value'] for i in feature.unique().tolist() if i not in config['param']['feature_scale']}}
+        t = feature.replace(scale).fillna(config['param']['miss_value']).rename(config['param']['name'])
+        return t if mode else (t, config)
+    
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `linora-1.6.0/linora/feature_column/_normalize.py` & `linora-2.0.0rc0/linora/feature_column/_normalize.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,172 +10,168 @@
     Args:
         feature: pd.Series, sample feature value.
         mode: if 0, output (transform feature, config); if 1, output transform feature; if 2, output config.
         name: str, output feature name, if None, name is feature.name .
         config: dict, label parameters dict for this estimator. 
             if config is not None, only parameter `feature` and `mode` is invalid.
     Returns:
-        normalize feature and feature_scale.
+        Refer to params `mode` explanation.
     """
     if config is None:
-        config = {'feature_scale':feature.max(),
-                  'type':'normalize_max', 'name_input':feature.name, 
-                  'name_output':feature.name if name is None else name}
+        config = {'param':{'feature_scale':feature.max(), 'name':feature.name if name is None else name},
+                  'type':'normalize_max', 'variable':feature.name}
     if mode==2:
         return config
     else:
-        scale = config['feature_scale']
-        t = (feature/scale).rename(config['name_output'])
+        scale = config['param']['feature_scale']
+        t = (feature/scale).rename(config['param']['name'])
         return t if mode else (t, config)
     
 
 def normalize_maxabs(feature, mode=0, name=None, config=None):
     """normalize feature with maxabs method.
     
     Args:
         feature: pd.Series, sample feature value.
         mode: if 0, output (transform feature, config); if 1, output transform feature; if 2, output config.
         name: str, output feature name, if None, name is feature.name .
         config: dict, label parameters dict for this estimator. 
             if config is not None, only parameter `feature` and `mode` is invalid.
     Returns:
-        normalize feature and feature_scale.
+        Refer to params `mode` explanation.
     """
     if config is None:
-        config = {'feature_scale':feature.abs().max(),
-                  'type':'normalize_maxabs', 'name_input':feature.name, 
-                  'name_output':feature.name if name is None else name}
+        config = {'param':{'feature_scale':feature.abs().max(), 'name':feature.name if name is None else name},
+                  'type':'normalize_maxabs', 'variable':feature.name}
     if mode==2:
         return config
     else:
-        scale = config['feature_scale']
-        t = (feature/scale).rename(config['name_output'])
+        scale = config['param']['feature_scale']
+        t = (feature/scale).rename(config['param']['name'])
         return t if mode else (t, config)
 
 
 def normalize_l1(feature, mode=0, name=None, config=None):
     """normalize feature with l1 method.
     
     Args:
         feature: pd.Series, sample feature value.
         mode: if 0, output (transform feature, config); if 1, output transform feature; if 2, output config.
         name: str, output feature name, if None, name is feature.name .
         config: dict, label parameters dict for this estimator. 
             if config is not None, only parameter `feature` and `mode` is invalid.
     Returns:
-        normalize feature and feature_scale.
+        Refer to params `mode` explanation.
     """
     if config is None:
-        config = {'feature_scale':feature.abs().sum(),
-                  'type':'normalize_l1', 'name_input':feature.name, 
-                  'name_output':feature.name if name is None else name}
+        config = {'param':{'feature_scale':feature.abs().sum(), 'name':feature.name if name is None else name},
+                  'type':'normalize_l1', 'variable':feature.name}
     if mode==2:
         return config
     else:
-        scale = config['feature_scale']
-        t = (feature/scale).rename(config['name_output'])
+        scale = config['param']['feature_scale']
+        t = (feature/scale).rename(config['param']['name'])
         return t if mode else (t, config)
 
 
 def normalize_l2(feature, mode=0, name=None, config=None):
     """normalize feature with l2 method.
     
     Args:
         feature: pd.Series, sample feature value.
         mode: if 0, output (transform feature, config); if 1, output transform feature; if 2, output config.
         name: str, output feature name, if None, name is feature.name .
         config: dict, label parameters dict for this estimator. 
             if config is not None, only parameter `feature` and `mode` is invalid.
     Returns:
-        normalize feature and feature_scale.
+        Refer to params `mode` explanation.
     """
     if config is None:
-        config = {'feature_scale':np.sqrt(np.sum(np.square(feature))),
-                  'type':'normalize_l2', 'name_input':feature.name, 
-                  'name_output':feature.name if name is None else name}
+        config = {'param':{'feature_scale':np.sqrt(np.sum(np.square(feature))), 
+                           'name':feature.name if name is None else name},
+                  'type':'normalize_l2', 'variable':feature.name}
     if mode==2:
         return config
     else:
-        scale = config['feature_scale']
-        t = (feature/scale).rename(config['name_output'])
+        scale = config['param']['feature_scale']
+        t = (feature/scale).rename(config['param']['name_output'])
         return t if mode else (t, config)
 
 
 def normalize_meanminmax(feature, mode=0, name=None, config=None):
     """normalize feature with meanminmax method.
     
     Args:
         feature: pd.Series, sample feature value.
         mode: if 0, output (transform feature, config); if 1, output transform feature; if 2, output config.
         name: str, output feature name, if None, name is feature.name .
         config: dict, label parameters dict for this estimator. 
             if config is not None, only parameter `feature` and `mode` is invalid.
     Returns:
-        normalize feature and feature_scale.
+        Refer to params `mode` explanation.
     """
     if config is None:
-        config = {'feature_scale':[feature.mean(), feature.min(), feature.max()],
-                  'type':'normalize_meanminmax', 'name_input':feature.name, 
-                  'name_output':feature.name if name is None else name}
+        config = {'param':{'feature_scale':[feature.mean(), feature.min(), feature.max()],
+                           'name':feature.name if name is None else name},
+                  'type':'normalize_meanminmax', 'variable':feature.name}
     if mode==2:
         return config
     else:
-        scale = config['feature_scale']
-        t = ((feature-scale[0])/(scale[2]-scale[1])).rename(config['name_output'])
+        scale = config['param']['feature_scale']
+        t = ((feature-scale[0])/(scale[2]-scale[1])).rename(config['param']['name'])
         return t if mode else (t, config)
 
 
 def normalize_minmax(feature, mode=0, feature_range=(0, 1), name=None, config=None):
     """normalize feature with minmax method.
     
     Args:
         feature: pd.Series, sample feature value.
         mode: if 0, output (transform feature, config); if 1, output transform feature; if 2, output config.
         feature_range: list or tuple, range of values after feature transformation.
         name: str, output feature name, if None, name is feature.name .
         config: dict, label parameters dict for this estimator. 
             if config is not None, only parameter `feature` and `mode` is invalid.
     Returns:
-        normalize feature and feature_scale.
+        Refer to params `mode` explanation.
     """
     if config is None:
-        config = {'feature_scale':[feature.min(), feature.max()],
-                  'feature_range':feature_range,
-                  'type':'normalize_minmax', 'name_input':feature.name, 
-                  'name_output':feature.name if name is None else name}
+        config = {'param':{'feature_scale':[feature.min(), feature.max()], 
+                           'feature_range':feature_range, 'name':feature.name if name is None else name},
+                  'type':'normalize_minmax', 'variable':feature.name}
     if mode==2:
         return config
     else:
-        scale = config['feature_scale']
-        ran = config['feature_range']
-        t = ((feature-scale[0])/(scale[1]-scale[0])*(ran[1]-ran[0])+ran[0]).rename(config['name_output'])
+        scale = config['param']['feature_scale']
+        ran = config['param']['feature_range']
+        t = ((feature-scale[0])/(scale[1]-scale[0])*(ran[1]-ran[0])+ran[0]).rename(config['param']['name'])
         return t if mode else (t, config)
 
 
 def normalize_norm(feature, mode=0, name=None, config=None):
     """normalize feature with norm method.
     
     Args:
         feature: pd.Series, sample feature value.
         mode: if 0, output (transform feature, config); if 1, output transform feature; if 2, output config.
         name: str, output feature name, if None, name is feature.name .
         config: dict, label parameters dict for this estimator. 
             if config is not None, only parameter `feature` and `mode` is invalid.
     Returns:
-        normalize feature and feature_scale.
+        Refer to params `mode` explanation.
     """
     if config is None:
-        config = {'feature_scale':[feature.mean(), feature.std()],
-                  'type':'normalize_norm', 'name_input':feature.name, 
-                  'name_output':feature.name if name is None else name}
+        config = {'param':{'feature_scale':[feature.mean(), feature.std()],
+                           'name':feature.name if name is None else name},
+                  'type':'normalize_norm', 'variable':feature.name}
     if mode==2:
         return config
     else:
-        scale = config['feature_scale']
-        t = ((feature-scale[0])/scale[1]).rename(config['name_output'])
+        scale = config['param']['feature_scale']
+        t = ((feature-scale[0])/scale[1]).rename(config['param']['name'])
         return t if mode else (t, config)
 
 
 def normalize_robust(feature, mode=0, feature_scale=(0.5, 0.5), name=None, config=None):
     """normalize feature with robust method.
     
     Args:
@@ -183,19 +179,19 @@
         mode: if 0, output (transform feature, config); if 1, output transform feature; if 2, output config.
         feature_scale: list or tuple, each element is in the [0,1] interval.
                        (feature_scale[0], feature.quantile(0.5+feature_scale[1]/2)-feature.quantile(0.5-feature_scale[1]/2)).
         name: str, output feature name, if None, name is feature.name .
         config: dict, label parameters dict for this estimator. 
             if config is not None, only parameter `feature` and `mode` is invalid.
     Returns:
-        normalize feature and feature_scale.
+        Refer to params `mode` explanation.
     """
     if config is None:
-        config = {'feature_scale':[feature.quantile(feature_scale[0]), feature.quantile(0.5+feature_scale[1]/2)-feature.quantile(0.5-feature_scale[1]/2)],
-                  'type':'normalize_robust', 'name_input':feature.name, 
-                  'name_output':feature.name if name is None else name}
+        config = {'param':{'feature_scale':[feature.quantile(feature_scale[0]), feature.quantile(0.5+feature_scale[1]/2)-feature.quantile(0.5-feature_scale[1]/2)], 
+                           'name':feature.name if name is None else name},
+                  'type':'normalize_robust', 'variable':feature.name}
     if mode==2:
         return config
     else:
-        scale = config['feature_scale']
-        t = ((feature-scale[0])/scale[1]).rename(config['name_output'])
+        scale = config['param']['feature_scale']
+        t = ((feature-scale[0])/scale[1]).rename(config['param']['name'])
         return t if mode else (t, config)
```

### Comparing `linora-1.6.0/linora/feature_column/boundary/_boundary.py` & `linora-2.0.0rc0/linora/feature_column/boundary/_boundary.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/feature_selection/_credit.py` & `linora-2.0.0rc0/linora/feature_selection/_credit.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/feature_selection/_select.py` & `linora-2.0.0rc0/linora/feature_selection/_select.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/gfile/_gfile.py` & `linora-2.0.0rc0/linora/gfile/_gfile.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/image/__init__.py` & `linora-2.0.0rc0/linora/image/__init__.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/image/_image_aug.py` & `linora-2.0.0rc0/linora/image/_image_aug.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/image/_image_box.py` & `linora-2.0.0rc0/linora/image/_image_box.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/image/_image_color.py` & `linora-2.0.0rc0/linora/image/_image_color.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/image/_image_color_aug.py` & `linora-2.0.0rc0/linora/image/_image_color_aug.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/image/_image_crop.py` & `linora-2.0.0rc0/linora/image/_image_crop.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/image/_image_crop_aug.py` & `linora-2.0.0rc0/linora/image/_image_crop_aug.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/image/_image_draw.py` & `linora-2.0.0rc0/linora/image/_image_draw.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/image/_image_draw_aug.py` & `linora-2.0.0rc0/linora/image/_image_draw_aug.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/image/_image_feature.py` & `linora-2.0.0rc0/linora/image/_image_feature.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/image/_image_filter.py` & `linora-2.0.0rc0/linora/image/_image_filter.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/image/_image_filter_aug.py` & `linora-2.0.0rc0/linora/image/_image_filter_aug.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/image/_image_grid.py` & `linora-2.0.0rc0/linora/image/_image_grid.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/image/_image_io.py` & `linora-2.0.0rc0/linora/image/_image_io.py`

 * *Files 21% similar despite different names*

```diff
@@ -39,22 +39,29 @@
         filename: Path or file object.
         image: A PIL instance.
         file_format: Optional file format override. If omitted, the
             format to use is determined from the filename extension.
             If a file object was used instead of a filename, this
             parameter should always be used.
         **kwargs: Additional keyword arguments passed to `PIL.Image.save()`.
+        if save gif, param `duration` and `loop` is optional.
     """
     if file_format is None:
         file_format = filename.split('.')[-1]
     if image.mode == 'RGBA' and file_format in ['jpg', 'jpeg']:
         image = image.convert('RGB')
-    image.save(filename, format=file_format, **kwargs)
+    if filename.lower().endswith('.gif'):
+        assert isinstance(image, list), '`image` must be image of list.'
+        duration = kwargs['duration'] if 'duration' in kwargs else 100
+        loop = kwargs['loop'] if 'loop' in kwargs else 0
+        image[0].save(filename, format='GIF', append_images=image[1:], save_all=True, duration=duration, loop=loop)
+    else:
+        image.save(filename, format=file_format, **kwargs)
+
 
-    
 def encode_base64(filename):
     """encode image to string.
     
     Args
         filename: image file path.
     Returns:
         a bites string.
```

### Comparing `linora-1.6.0/linora/image/_image_io_aug.py` & `linora-2.0.0rc0/linora/image/_image_io_aug.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/image/_image_noise.py` & `linora-2.0.0rc0/linora/image/_image_noise.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/image/_image_noise_aug.py` & `linora-2.0.0rc0/linora/image/_image_noise_aug.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/image/_image_pairs.py` & `linora-2.0.0rc0/linora/image/_image_pairs.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/image/_image_position.py` & `linora-2.0.0rc0/linora/image/_image_position.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/image/_image_position_aug.py` & `linora-2.0.0rc0/linora/image/_image_position_aug.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/image/_image_rescale.py` & `linora-2.0.0rc0/linora/image/_image_rescale.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/image/_image_rescale_aug.py` & `linora-2.0.0rc0/linora/image/_image_rescale_aug.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/image/_image_resize.py` & `linora-2.0.0rc0/linora/image/_image_resize.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/image/_image_resize_aug.py` & `linora-2.0.0rc0/linora/image/_image_resize_aug.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/image/_image_rgb.py` & `linora-2.0.0rc0/linora/image/_image_rgb.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/image/_image_util.py` & `linora-2.0.0rc0/linora/image/_image_util.py`

 * *Files 6% similar despite different names*

```diff
@@ -68,62 +68,55 @@
         elif image.mode != color_mode['mode']:
             image = image.convert(color_mode['mode'])
     else:
         raise ValueError('color_mode error.')
     return image
 
 
-def image_to_array(image, data_format='channels_last', dtype='float32'):
+def image_to_array(image, data_format='HWC', dtype='float32'):
     """Converts a PIL Image instance to a Numpy array.
     
     Args:
         image: PIL instance.
-        data_format: Image data format, either "channels_first" or "channels_last".
+        data_format: array data format, eg.'HWC'.
         dtype: Dtype to use for the returned array.
     Returns:
         A Numpy array.
     Raises:
         ValueError: if invalid `img` or `data_format` is passed.
     """
-    if data_format not in {'channels_first', 'channels_last'}:
-        raise ValueError('Unknown data_format: %s' % data_format)
+    transpose = {'H':0, 'W':1, 'C':2}
     x = np.asarray(image, dtype=dtype)
+    if len(x.shape) == 2:
+        x = np.expand_dims(x, axis=-1)
     if len(x.shape) == 3:
-        if data_format == 'channels_first':
-            x = x.transpose(2, 0, 1)
-    elif len(x.shape) == 2:
-        if data_format == 'channels_first':
-            x = x.reshape((1, x.shape[0], x.shape[1]))
-        else:
-            x = x.reshape((x.shape[0], x.shape[1], 1))
+        x = x.transpose(tuple(transpose[i] for i in data_format))
     else:
         raise ValueError('Unsupported image shape: %s' % (x.shape,))
     return x
 
 
-def array_to_image(x, data_format='channels_last'):
+def array_to_image(x, data_format='HWC'):
     """Converts a 3D Numpy array to a PIL Image instance.
     
     Args:
         x: Input Numpy array.
-        data_format: Image data format, either "channels_first" or "channels_last".
+        data_format: array data format, eg.'HWC'.
     Returns:
         A PIL instance.
     Raises:
         ValueError: if invalid `x` or `data_format` is passed.
     """
     if x.ndim != 3:
         raise ValueError('Expected image array to have rank 3 (single image). '
                          'Got array with shape: %s' % (x.shape,))
 
-    if data_format not in {'channels_first', 'channels_last'}:
-        raise ValueError('Invalid data_format: %s' % data_format)
-
-    if data_format == 'channels_first':
-        x = x.transpose(1, 2, 0)
+    transpose = {i:r for r,i in enumerate(data_format)}
+    if data_format != 'HWC':
+        x = x.transpose(tuple(transpose[i] for i in 'HWC'))
 
     if x.shape[2] == 4:
         return Image.fromarray(x.astype('uint8'), 'RGBA')
     elif x.shape[2] == 3:
         return Image.fromarray(x.astype('uint8'), 'RGB')
     elif x.shape[2] == 1:
         if np.max(x) > 255:
```

### Comparing `linora-1.6.0/linora/metrics/_classification.py` & `linora-2.0.0rc0/linora/metrics/_classification.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/metrics/_image.py` & `linora-2.0.0rc0/linora/metrics/_image.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/metrics/_metrics.py` & `linora-2.0.0rc0/linora/metrics/_metrics.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/metrics/_rank.py` & `linora-2.0.0rc0/linora/metrics/_rank.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/metrics/_regression.py` & `linora-2.0.0rc0/linora/metrics/_regression.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/metrics/distance/_distance.py` & `linora-2.0.0rc0/linora/metrics/distance/_distance.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/metrics/distance/_divergence.py` & `linora-2.0.0rc0/linora/metrics/distance/_divergence.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/parallel/_process.py` & `linora-2.0.0rc0/linora/parallel/_process.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/parallel/_thread.py` & `linora-2.0.0rc0/linora/parallel/_thread.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/param_search/GEClassifier/_GridSearch.py` & `linora-2.0.0rc0/linora/param_search/GEClassifier/_GridSearch.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/param_search/GEClassifier/_RandomSearch.py` & `linora-2.0.0rc0/linora/param_search/GEClassifier/_RandomSearch.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/param_search/GERegressor/_RandomSearch.py` & `linora-2.0.0rc0/linora/param_search/GERegressor/_RandomSearch.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/param_search/LGBMClassifier/_GridSearch.py` & `linora-2.0.0rc0/linora/param_search/LGBMClassifier/_GridSearch.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/param_search/LGBMClassifier/_RandomSearch.py` & `linora-2.0.0rc0/linora/param_search/LGBMClassifier/_RandomSearch.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/param_search/LGBMRegressor/_GridSearch.py` & `linora-2.0.0rc0/linora/param_search/LGBMRegressor/_GridSearch.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/param_search/LGBMRegressor/_RandomSearch.py` & `linora-2.0.0rc0/linora/param_search/LGBMRegressor/_RandomSearch.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/param_search/XGBClassifier/_GridSearch.py` & `linora-2.0.0rc0/linora/param_search/XGBClassifier/_GridSearch.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/param_search/XGBClassifier/_RandomSearch.py` & `linora-2.0.0rc0/linora/param_search/XGBClassifier/_RandomSearch.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/param_search/XGBRanker/_GridSearch.py` & `linora-2.0.0rc0/linora/param_search/XGBRanker/_GridSearch.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/param_search/XGBRanker/_RandomSearch.py` & `linora-2.0.0rc0/linora/param_search/XGBRanker/_RandomSearch.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/param_search/XGBRegressor/_GridSearch.py` & `linora-2.0.0rc0/linora/param_search/XGBRegressor/_GridSearch.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/param_search/XGBRegressor/_RandomSearch.py` & `linora-2.0.0rc0/linora/param_search/XGBRegressor/_RandomSearch.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/param_search/_HyperParameters.py` & `linora-2.0.0rc0/linora/param_search/_HyperParameters.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/param_search/_Search.py` & `linora-2.0.0rc0/linora/param_search/_Search.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import numpy as np
 import pandas as pd
 
 from linora.utils._config import Config
 from linora.utils._logger import Logger
 from linora.sample._fold import kfold, train_test_split
 from linora.param_search._config import model_hp
-from linora.param_search._HyperParameters import HyperParametersRandom
 from linora.param_search._config import __xgboost_version__, __lightgbm_version__
 
 
 __all__ = ['RandomSearch', 'GridSearch']
 
 
 class BaseSearch():
```

### Comparing `linora-1.6.0/linora/param_search/_config.py` & `linora-2.0.0rc0/linora/param_search/_config.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/sample/_fold.py` & `linora-2.0.0rc0/linora/sample/_fold.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/sample/_random_walker.py` & `linora-2.0.0rc0/linora/sample/_random_walker.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/sample/_sampling.py` & `linora-2.0.0rc0/linora/sample/_sampling.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/sample/_timeseries_kfold.py` & `linora-2.0.0rc0/linora/sample/_timeseries_kfold.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/text/_sequence.py` & `linora-2.0.0rc0/linora/text/_sequence.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/text/_util.py` & `linora-2.0.0rc0/linora/text/_util.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/text/_vectorizer.py` & `linora-2.0.0rc0/linora/text/_vectorizer.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/text/_word_processing.py` & `linora-2.0.0rc0/linora/text/_word_processing.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from itertools import chain
 from collections import Counter
 
 __all__ = ['sequence_preprocess', 'word_count', 'word_low_freq', 'word_high_freq', 'filter_word',
-           'filter_punctuation']
+           'filter_punctuation', 'ngrams_iterator']
 
 
 def sequence_preprocess(sequence):
     """Sequence preprocess, keep only Chinese.
     
     Args:
         sequence: pd.Series or np.array or list, sample feature value.
@@ -77,7 +77,21 @@
         a list of Lists.
     """
     punc = '!"#$%&\'()*+,-./:;<=>?@[\\]^_`{|}~（），。’‘”“！？》《·、】【；：' if punctuation is None else punctuation
     table = str.maketrans('', '', punc)
     if isinstance(sequence, str):
         return sequence.translate(table)
     return [s.translate(table) for s in sequence]
+
+
+def ngrams_iterator(token_list, ngrams, join=' '):
+    """Return an iterator that yields the given tokens and their ngrams.
+
+    Args:
+        token_list: A list of tokens
+        ngrams: the number of ngrams.
+    """
+    for x in token_list:
+        yield x
+    for n in range(2, ngrams + 1):
+        for x in zip(*[token_list[i:] for i in range(n)]):
+            yield join.join(x)
```

### Comparing `linora-1.6.0/linora/train/_callback.py` & `linora-2.0.0rc0/linora/train/_callback.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/train/_csvlogger.py` & `linora-2.0.0rc0/linora/train/_csvlogger.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/train/_earlystopping.py` & `linora-2.0.0rc0/linora/train/_earlystopping.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/train/_modelcheckpoint.py` & `linora-2.0.0rc0/linora/train/_modelcheckpoint.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/train/_remotemonitor.py` & `linora-2.0.0rc0/linora/train/_remotemonitor.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/train/_terminateonnan.py` & `linora-2.0.0rc0/linora/train/_terminateonnan.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/train/_visual.py` & `linora-2.0.0rc0/linora/train/_visual.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/train/lr/_lr.py` & `linora-2.0.0rc0/linora/train/lr/_lr.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/train/lr/_schedulers.py` & `linora-2.0.0rc0/linora/train/lr/_schedulers.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/utils/_config.py` & `linora-2.0.0rc0/linora/utils/_config.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/utils/_email.py` & `linora-2.0.0rc0/linora/server/_email.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from email.mime.base import MIMEBase
 from email.mime.multipart import MIMEMultipart
 from email.mime.text import MIMEText
 
 import pandas as pd
 
 from linora.utils._config import Config
-from linora.utils._email_utils import parse_mail, parse_headers
+from linora.server._email_utils import parse_mail, parse_headers
 
 __all__ = ['EMail']
 
 
 poplib._MAXLINE = 4096
 mail_personal = {
     '163.com': {
```

### Comparing `linora-1.6.0/linora/utils/_email_utils.py` & `linora-2.0.0rc0/linora/server/_email_utils.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/utils/_logger.py` & `linora-2.0.0rc0/linora/utils/_logger.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/utils/_progbar.py` & `linora-2.0.0rc0/linora/utils/_progbar.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/utils/_schedulers.py` & `linora-2.0.0rc0/linora/server/_schedulers.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/utils/message/_BotDingTalk.py` & `linora-2.0.0rc0/linora/server/message/_BotDingTalk.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/utils/message/_BotFeiShu.py` & `linora-2.0.0rc0/linora/server/message/_BotFeiShu.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora/utils/pip/_pip.py` & `linora-2.0.0rc0/linora/utils/pip/_pip.py`

 * *Files identical despite different names*

### Comparing `linora-1.6.0/linora.egg-info/PKG-INFO` & `linora-2.0.0rc0/linora.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linora
-Version: 1.6.0
+Version: 2.0.0rc0
 Summary: Simple and efficient tools for data mining and data analysis.
 Home-page: https://github.com/Hourout/linora
 Author: JinQing Lee
 Author-email: hourout@163.com
 License: Apache License Version 2.0
 Description: ![](https://github.com/Hourout/linora/blob/master/image/linora.png)
```

### Comparing `linora-1.6.0/linora.egg-info/SOURCES.txt` & `linora-2.0.0rc0/linora.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -53,15 +53,20 @@
 linora/data/datasets/__init__.py
 linora/data/datasets/_config_path.py
 linora/data/datasets/_mnist.py
 linora/data/datasets/_utils.py
 linora/data/datasets/_weather.py
 linora/feature_column/__init__.py
 linora/feature_column/_categorical.py
+linora/feature_column/_datetime.py
 linora/feature_column/_feature.py
+linora/feature_column/_feature_categorical.py
+linora/feature_column/_feature_datetime.py
+linora/feature_column/_feature_normalize.py
+linora/feature_column/_feature_numerical.py
 linora/feature_column/_normalize.py
 linora/feature_column/_numerical.py
 linora/feature_column/boundary/__init__.py
 linora/feature_column/boundary/_boundary.py
 linora/feature_selection/__init__.py
 linora/feature_selection/_credit.py
 linora/feature_selection/_select.py
@@ -95,14 +100,15 @@
 linora/image/_image_util.py
 linora/metrics/__init__.py
 linora/metrics/_classification.py
 linora/metrics/_image.py
 linora/metrics/_metrics.py
 linora/metrics/_rank.py
 linora/metrics/_regression.py
+linora/metrics/_text.py
 linora/metrics/_utils.py
 linora/metrics/distance/__init__.py
 linora/metrics/distance/_distance.py
 linora/metrics/distance/_divergence.py
 linora/parallel/__init__.py
 linora/parallel/_process.py
 linora/parallel/_thread.py
@@ -131,14 +137,21 @@
 linora/param_search/XGBRegressor/_RandomSearch.py
 linora/param_search/XGBRegressor/__init__.py
 linora/sample/__init__.py
 linora/sample/_fold.py
 linora/sample/_random_walker.py
 linora/sample/_sampling.py
 linora/sample/_timeseries_kfold.py
+linora/server/__init__.py
+linora/server/_email.py
+linora/server/_email_utils.py
+linora/server/_schedulers.py
+linora/server/message/_BotDingTalk.py
+linora/server/message/_BotFeiShu.py
+linora/server/message/__init__.py
 linora/text/__init__.py
 linora/text/_sequence.py
 linora/text/_util.py
 linora/text/_vectorizer.py
 linora/text/_word_processing.py
 linora/train/__init__.py
 linora/train/_callback.py
@@ -158,8 +171,11 @@
 linora/utils/_logger.py
 linora/utils/_progbar.py
 linora/utils/_schedulers.py
 linora/utils/message/_BotDingTalk.py
 linora/utils/message/_BotFeiShu.py
 linora/utils/message/__init__.py
 linora/utils/pip/__init__.py
-linora/utils/pip/_pip.py
+linora/utils/pip/_pip.py
+linora/vedio/__init__.py
+linora/vedio/_vedio_io.py
+linora/vedio/_vedio_util.py
```

### Comparing `linora-1.6.0/setup.py` & `linora-2.0.0rc0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 def readme():
     with io.open('README.md', encoding='utf-8') as f:
         return f.read()
 
 setup(name='linora',
-      version='1.6.0',
+      version='2.0.0rc0',
       install_requires=[
           'pandas>=1.5.2', 
           'Pillow>=9.3.0',
           'joblib>=1.2.0',
           'requests>=2.28.0',
           'rarfile'
       ],
```

