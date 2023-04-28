# Comparing `tmp/roof_mask_Yv8-0.5.7.tar.gz` & `tmp/roof_mask_Yv8-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roof_mask_Yv8-0.5.7.tar", last modified: Fri Apr 21 14:44:43 2023, max compression
+gzip compressed data, was "roof_mask_Yv8-0.5.8.tar", last modified: Fri Apr 28 21:02:22 2023, max compression
```

## Comparing `roof_mask_Yv8-0.5.7.tar` & `roof_mask_Yv8-0.5.8.tar`

### file list

```diff
@@ -1,303 +1,303 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-21 14:44:01.121030 roof_mask_Yv8-0.5.7/
--rwxrwxrwx   0 root         (0) root         (0)      143 2023-04-19 16:56:54.000000 roof_mask_Yv8-0.5.7/.gitignore
--rwxrwxrwx   0 root         (0) root         (0)       41 2023-04-20 18:44:18.000000 roof_mask_Yv8-0.5.7/MANIFEST.in
--rwxrwxrwx   0 root         (0) root         (0)      426 2023-04-21 14:44:43.363770 roof_mask_Yv8-0.5.7/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.7/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-21 14:44:01.166004 roof_mask_Yv8-0.5.7/detectron2/
--rwxrwxrwx   0 root         (0) root         (0)      258 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.7/detectron2/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-21 14:44:01.216974 roof_mask_Yv8-0.5.7/detectron2/checkpoint/
--rwxrwxrwx   0 root         (0) root         (0)      347 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.7/detectron2/checkpoint/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    17782 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.7/detectron2/checkpoint/c2_model_loading.py
--rwxrwxrwx   0 root         (0) root         (0)     5685 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.7/detectron2/checkpoint/catalog.py
--rwxrwxrwx   0 root         (0) root         (0)     5258 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.7/detectron2/checkpoint/detection_checkpoint.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-21 14:44:01.280938 roof_mask_Yv8-0.5.7/detectron2/config/
--rwxrwxrwx   0 root         (0) root         (0)      599 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.7/detectron2/config/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     7890 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.7/detectron2/config/compat.py
--rwxrwxrwx   0 root         (0) root         (0)     9211 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.7/detectron2/config/config.py
--rwxrwxrwx   0 root         (0) root         (0)    29512 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.7/detectron2/config/defaults.py
--rwxrwxrwx   0 root         (0) root         (0)     2719 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.7/detectron2/config/instantiate.py
--rwxrwxrwx   0 root         (0) root         (0)    14944 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.7/detectron2/config/lazy.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-21 14:44:01.323913 roof_mask_Yv8-0.5.7/detectron2/data/
--rwxrwxrwx   0 root         (0) root         (0)      644 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.7/detectron2/data/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     7378 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.7/detectron2/data/benchmark.py
--rwxrwxrwx   0 root         (0) root         (0)    20605 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.7/detectron2/data/build.py
--rwxrwxrwx   0 root         (0) root         (0)     7224 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.7/detectron2/data/catalog.py
--rwxrwxrwx   0 root         (0) root         (0)     9164 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.7/detectron2/data/common.py
--rwxrwxrwx   0 root         (0) root         (0)     8169 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.7/detectron2/data/dataset_mapper.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-21 14:44:01.389875 roof_mask_Yv8-0.5.7/detectron2/data/datasets/
--rwxrwxrwx   0 root         (0) root         (0)      347 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.7/detectron2/data/datasets/README.md
--rwxrwxrwx   0 root         (0) root         (0)      523 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.7/detectron2/data/datasets/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    10174 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.7/detectron2/data/datasets/builtin.py
--rwxrwxrwx   0 root         (0) root         (0)    21841 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.7/detectron2/data/datasets/builtin_meta.py
--rwxrwxrwx   0 root         (0) root         (0)    13167 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.7/detectron2/data/datasets/cityscapes.py
--rwxrwxrwx   0 root         (0) root         (0)     7821 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.7/detectron2/data/datasets/cityscapes_panoptic.py
--rwxrwxrwx   0 root         (0) root         (0)    23465 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.7/detectron2/data/datasets/coco.py
--rwxrwxrwx   0 root         (0) root         (0)     8977 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.7/detectron2/data/datasets/coco_panoptic.py
--rwxrwxrwx   0 root         (0) root         (0)     9623 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.7/detectron2/data/datasets/lvis.py
--rwxrwxrwx   0 root         (0) root         (0)   223757 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.7/detectron2/data/datasets/lvis_v0_5_categories.py
--rwxrwxrwx   0 root         (0) root         (0)   219177 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.7/detectron2/data/datasets/lvis_v1_categories.py
--rwxrwxrwx   0 root         (0) root         (0)    39414 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.7/detectron2/data/datasets/lvis_v1_category_image_count.py
--rwxrwxrwx   0 root         (0) root         (0)     3128 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.7/detectron2/data/datasets/pascal_voc.py
--rwxrwxrwx   0 root         (0) root         (0)      169 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.7/detectron2/data/datasets/register_coco.py
--rwxrwxrwx   0 root         (0) root         (0)    22841 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.7/detectron2/data/detection_utils.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-21 14:44:01.434848 roof_mask_Yv8-0.5.7/detectron2/data/samplers/
--rwxrwxrwx   0 root         (0) root         (0)      412 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.7/detectron2/data/samplers/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    11789 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.7/detectron2/data/samplers/distributed_sampler.py
--rwxrwxrwx   0 root         (0) root         (0)     1944 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.7/detectron2/data/samplers/grouped_batch_sampler.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-21 14:44:01.501810 roof_mask_Yv8-0.5.7/detectron2/data/transforms/
--rwxrwxrwx   0 root         (0) root         (0)      466 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.7/detectron2/data/transforms/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    14117 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.7/detectron2/data/transforms/augmentation.py
--rwxrwxrwx   0 root         (0) root         (0)    23069 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.7/detectron2/data/transforms/augmentation_impl.py
--rwxrwxrwx   0 root         (0) root         (0)    12629 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.7/detectron2/data/transforms/transform.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-21 14:44:01.548783 roof_mask_Yv8-0.5.7/detectron2/engine/
--rwxrwxrwx   0 root         (0) root         (0)      340 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.7/detectron2/engine/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    26868 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.7/detectron2/engine/defaults.py
--rwxrwxrwx   0 root         (0) root         (0)    25497 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.7/detectron2/engine/hooks.py
--rwxrwxrwx   0 root         (0) root         (0)     4089 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.7/detectron2/engine/launch.py
--rwxrwxrwx   0 root         (0) root         (0)    14104 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.7/detectron2/engine/train_loop.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-21 14:44:01.593757 roof_mask_Yv8-0.5.7/detectron2/evaluation/
--rwxrwxrwx   0 root         (0) root         (0)      671 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.7/detectron2/evaluation/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     8369 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.7/detectron2/evaluation/cityscapes_evaluation.py
--rwxrwxrwx   0 root         (0) root         (0)    30423 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.7/detectron2/evaluation/coco_evaluation.py
--rwxrwxrwx   0 root         (0) root         (0)     8156 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.7/detectron2/evaluation/evaluator.py
--rwxrwxrwx   0 root         (0) root         (0)     5078 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.7/detectron2/evaluation/fast_eval_api.py
--rwxrwxrwx   0 root         (0) root         (0)    15018 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.7/detectron2/evaluation/lvis_evaluation.py
--rwxrwxrwx   0 root         (0) root         (0)     7500 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.7/detectron2/evaluation/panoptic_evaluation.py
--rwxrwxrwx   0 root         (0) root         (0)    10862 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.7/detectron2/evaluation/pascal_voc_evaluation.py
--rwxrwxrwx   0 root         (0) root         (0)     7608 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.7/detectron2/evaluation/rotated_coco_evaluation.py
--rwxrwxrwx   0 root         (0) root         (0)     8191 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.7/detectron2/evaluation/sem_seg_evaluation.py
--rwxrwxrwx   0 root         (0) root         (0)     2614 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.7/detectron2/evaluation/testing.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-21 14:44:01.643728 roof_mask_Yv8-0.5.7/detectron2/export/
--rwxrwxrwx   0 root         (0) root         (0)      513 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.7/detectron2/export/README.md
--rwxrwxrwx   0 root         (0) root         (0)      336 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.7/detectron2/export/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     9280 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.7/detectron2/export/api.py
--rwxrwxrwx   0 root         (0) root         (0)    21035 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.7/detectron2/export/c10.py
--rwxrwxrwx   0 root         (0) root         (0)     7803 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.7/detectron2/export/caffe2_export.py
--rwxrwxrwx   0 root         (0) root         (0)     6674 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.7/detectron2/export/caffe2_inference.py
--rwxrwxrwx   0 root         (0) root         (0)    17034 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.7/detectron2/export/caffe2_modeling.py
--rwxrwxrwx   0 root         (0) root         (0)     5033 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.7/detectron2/export/caffe2_patch.py
--rwxrwxrwx   0 root         (0) root         (0)    11807 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.7/detectron2/export/flatten.py
--rwxrwxrwx   0 root         (0) root         (0)    38071 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.7/detectron2/export/shared.py
--rwxrwxrwx   0 root         (0) root         (0)     5008 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.7/detectron2/export/torchscript.py
--rwxrwxrwx   0 root         (0) root         (0)    11526 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.7/detectron2/export/torchscript_patch.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-21 14:44:01.710691 roof_mask_Yv8-0.5.7/detectron2/layers/
--rwxrwxrwx   0 root         (0) root         (0)      839 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.7/detectron2/layers/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     5764 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.7/detectron2/layers/aspp.py
--rwxrwxrwx   0 root         (0) root         (0)    12131 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.7/detectron2/layers/batch_norm.py
--rwxrwxrwx   0 root         (0) root         (0)     3024 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.7/detectron2/layers/blocks.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-21 14:44:01.811632 roof_mask_Yv8-0.5.7/detectron2/layers/csrc/
--rwxrwxrwx   0 root         (0) root         (0)      122 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.7/detectron2/layers/csrc/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-21 14:44:01.861603 roof_mask_Yv8-0.5.7/detectron2/layers/csrc/ROIAlignRotated/
--rwxrwxrwx   0 root         (0) root         (0)     2870 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.7/detectron2/layers/csrc/ROIAlignRotated/ROIAlignRotated.h
--rwxrwxrwx   0 root         (0) root         (0)    16031 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.7/detectron2/layers/csrc/ROIAlignRotated/ROIAlignRotated_cpu.cpp
--rwxrwxrwx   0 root         (0) root         (0)    13876 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.7/detectron2/layers/csrc/ROIAlignRotated/ROIAlignRotated_cuda.cu
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-21 14:44:01.909575 roof_mask_Yv8-0.5.7/detectron2/layers/csrc/box_iou_rotated/
--rwxrwxrwx   0 root         (0) root         (0)      988 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.7/detectron2/layers/csrc/box_iou_rotated/box_iou_rotated.h
--rwxrwxrwx   0 root         (0) root         (0)     1090 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.7/detectron2/layers/csrc/box_iou_rotated/box_iou_rotated_cpu.cpp
--rwxrwxrwx   0 root         (0) root         (0)     4454 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.7/detectron2/layers/csrc/box_iou_rotated/box_iou_rotated_cuda.cu
--rwxrwxrwx   0 root         (0) root         (0)    10844 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.7/detectron2/layers/csrc/box_iou_rotated/box_iou_rotated_utils.h
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-21 14:44:01.956549 roof_mask_Yv8-0.5.7/detectron2/layers/csrc/cocoeval/
--rwxrwxrwx   0 root         (0) root         (0)    20746 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.7/detectron2/layers/csrc/cocoeval/cocoeval.cpp
--rwxrwxrwx   0 root         (0) root         (0)     3515 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.7/detectron2/layers/csrc/cocoeval/cocoeval.h
--rwxrwxrwx   0 root         (0) root         (0)      622 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.7/detectron2/layers/csrc/cuda_version.cu
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-21 14:44:02.004521 roof_mask_Yv8-0.5.7/detectron2/layers/csrc/deformable/
--rwxrwxrwx   0 root         (0) root         (0)     8384 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.7/detectron2/layers/csrc/deformable/deform_conv.h
--rwxrwxrwx   0 root         (0) root         (0)    31785 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.7/detectron2/layers/csrc/deformable/deform_conv_cuda.cu
--rwxrwxrwx   0 root         (0) root         (0)    44279 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.7/detectron2/layers/csrc/deformable/deform_conv_cuda_kernel.cu
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-21 14:44:02.051494 roof_mask_Yv8-0.5.7/detectron2/layers/csrc/nms_rotated/
--rwxrwxrwx   0 root         (0) root         (0)     1089 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.7/detectron2/layers/csrc/nms_rotated/nms_rotated.h
--rwxrwxrwx   0 root         (0) root         (0)     2307 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.7/detectron2/layers/csrc/nms_rotated/nms_rotated_cpu.cpp
--rwxrwxrwx   0 root         (0) root         (0)     4859 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.7/detectron2/layers/csrc/nms_rotated/nms_rotated_cuda.cu
--rwxrwxrwx   0 root         (0) root         (0)     3167 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.7/detectron2/layers/csrc/vision.cpp
--rwxrwxrwx   0 root         (0) root         (0)    16978 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.7/detectron2/layers/deform_conv.py
--rwxrwxrwx   0 root         (0) root         (0)     4204 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.7/detectron2/layers/losses.py
--rwxrwxrwx   0 root         (0) root         (0)    10881 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.7/detectron2/layers/mask_ops.py
--rwxrwxrwx   0 root         (0) root         (0)     6490 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.7/detectron2/layers/nms.py
--rwxrwxrwx   0 root         (0) root         (0)     3098 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.7/detectron2/layers/roi_align.py
--rwxrwxrwx   0 root         (0) root         (0)     3302 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.7/detectron2/layers/roi_align_rotated.py
--rwxrwxrwx   0 root         (0) root         (0)      652 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.7/detectron2/layers/rotated_boxes.py
--rwxrwxrwx   0 root         (0) root         (0)      661 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.7/detectron2/layers/shape_spec.py
--rwxrwxrwx   0 root         (0) root         (0)     4893 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.7/detectron2/layers/wrappers.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-21 14:44:02.086473 roof_mask_Yv8-0.5.7/detectron2/modeling/
--rwxrwxrwx   0 root         (0) root         (0)     1475 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.7/detectron2/modeling/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    15443 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.7/detectron2/modeling/anchor_generator.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-21 14:44:02.135445 roof_mask_Yv8-0.5.7/detectron2/modeling/backbone/
--rwxrwxrwx   0 root         (0) root         (0)      475 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.7/detectron2/modeling/backbone/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1543 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.7/detectron2/modeling/backbone/backbone.py
--rwxrwxrwx   0 root         (0) root         (0)     1015 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.7/detectron2/modeling/backbone/build.py
--rwxrwxrwx   0 root         (0) root         (0)    10055 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.7/detectron2/modeling/backbone/fpn.py
--rwxrwxrwx   0 root         (0) root         (0)    16656 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.7/detectron2/modeling/backbone/regnet.py
--rwxrwxrwx   0 root         (0) root         (0)    23658 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.7/detectron2/modeling/backbone/resnet.py
--rwxrwxrwx   0 root         (0) root         (0)    15123 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.7/detectron2/modeling/box_regression.py
--rwxrwxrwx   0 root         (0) root         (0)     6264 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.7/detectron2/modeling/matcher.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-21 14:44:02.189414 roof_mask_Yv8-0.5.7/detectron2/modeling/meta_arch/
--rwxrwxrwx   0 root         (0) root         (0)      508 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.7/detectron2/modeling/meta_arch/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      814 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.7/detectron2/modeling/meta_arch/build.py
--rwxrwxrwx   0 root         (0) root         (0)    11550 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.7/detectron2/modeling/meta_arch/dense_detector.py
--rwxrwxrwx   0 root         (0) root         (0)    13213 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.7/detectron2/modeling/meta_arch/fcos.py
--rwxrwxrwx   0 root         (0) root         (0)    10335 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.7/detectron2/modeling/meta_arch/panoptic_fpn.py
--rwxrwxrwx   0 root         (0) root         (0)    13710 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.7/detectron2/modeling/meta_arch/rcnn.py
--rwxrwxrwx   0 root         (0) root         (0)    18265 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.7/detectron2/modeling/meta_arch/retinanet.py
--rwxrwxrwx   0 root         (0) root         (0)     9720 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.7/detectron2/modeling/meta_arch/semantic_seg.py
--rwxrwxrwx   0 root         (0) root         (0)    10832 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.7/detectron2/modeling/mmdet_wrapper.py
--rwxrwxrwx   0 root         (0) root         (0)    11316 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.7/detectron2/modeling/poolers.py
--rwxrwxrwx   0 root         (0) root         (0)     4046 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.7/detectron2/modeling/postprocessing.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-21 14:44:02.252379 roof_mask_Yv8-0.5.7/detectron2/modeling/proposal_generator/
--rwxrwxrwx   0 root         (0) root         (0)      231 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.7/detectron2/modeling/proposal_generator/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      836 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.7/detectron2/modeling/proposal_generator/build.py
--rwxrwxrwx   0 root         (0) root         (0)     8128 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.7/detectron2/modeling/proposal_generator/proposal_utils.py
--rwxrwxrwx   0 root         (0) root         (0)    23814 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.7/detectron2/modeling/proposal_generator/rpn.py
--rwxrwxrwx   0 root         (0) root         (0)     8807 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.7/detectron2/modeling/proposal_generator/rrpn.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-21 14:44:02.356319 roof_mask_Yv8-0.5.7/detectron2/modeling/roi_heads/
--rwxrwxrwx   0 root         (0) root         (0)      768 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.7/detectron2/modeling/roi_heads/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     4077 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.7/detectron2/modeling/roi_heads/box_head.py
--rwxrwxrwx   0 root         (0) root         (0)    12990 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.7/detectron2/modeling/roi_heads/cascade_rcnn.py
--rwxrwxrwx   0 root         (0) root         (0)    25274 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.7/detectron2/modeling/roi_heads/fast_rcnn.py
--rwxrwxrwx   0 root         (0) root         (0)    11156 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.7/detectron2/modeling/roi_heads/keypoint_head.py
--rwxrwxrwx   0 root         (0) root         (0)    12169 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.7/detectron2/modeling/roi_heads/mask_head.py
--rwxrwxrwx   0 root         (0) root         (0)    37701 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.7/detectron2/modeling/roi_heads/roi_heads.py
--rwxrwxrwx   0 root         (0) root         (0)    11158 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.7/detectron2/modeling/roi_heads/rotated_fast_rcnn.py
--rwxrwxrwx   0 root         (0) root         (0)     2334 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.7/detectron2/modeling/sampling.py
--rwxrwxrwx   0 root         (0) root         (0)    12416 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.7/detectron2/modeling/test_time_augmentation.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-21 14:44:02.402292 roof_mask_Yv8-0.5.7/detectron2/solver/
--rwxrwxrwx   0 root         (0) root         (0)      298 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.7/detectron2/solver/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    11127 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.7/detectron2/solver/build.py
--rwxrwxrwx   0 root         (0) root         (0)     8648 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.7/detectron2/solver/lr_scheduler.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-21 14:44:02.449266 roof_mask_Yv8-0.5.7/detectron2/structures/
--rwxrwxrwx   0 root         (0) root         (0)      645 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.7/detectron2/structures/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    14429 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.7/detectron2/structures/boxes.py
--rwxrwxrwx   0 root         (0) root         (0)     4557 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.7/detectron2/structures/image_list.py
--rwxrwxrwx   0 root         (0) root         (0)     6542 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.7/detectron2/structures/instances.py
--rwxrwxrwx   0 root         (0) root         (0)     9030 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.7/detectron2/structures/keypoints.py
--rwxrwxrwx   0 root         (0) root         (0)    19802 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.7/detectron2/structures/masks.py
--rwxrwxrwx   0 root         (0) root         (0)    18853 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.7/detectron2/structures/rotated_boxes.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-21 14:44:02.495238 roof_mask_Yv8-0.5.7/detectron2/tracking/
--rwxrwxrwx   0 root         (0) root         (0)      580 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.7/detectron2/tracking/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     2216 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.7/detectron2/tracking/base_tracker.py
--rwxrwxrwx   0 root         (0) root         (0)    11858 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.7/detectron2/tracking/bbox_iou_tracker.py
--rwxrwxrwx   0 root         (0) root         (0)     7486 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.7/detectron2/tracking/hungarian_tracker.py
--rwxrwxrwx   0 root         (0) root         (0)     4142 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.7/detectron2/tracking/iou_weighted_hungarian_bbox_iou_tracker.py
--rwxrwxrwx   0 root         (0) root         (0)     1106 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.7/detectron2/tracking/utils.py
--rwxrwxrwx   0 root         (0) root         (0)     5288 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.7/detectron2/tracking/vanilla_hungarian_bbox_iou_tracker.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-21 14:44:02.539213 roof_mask_Yv8-0.5.7/detectron2/utils/
--rwxrwxrwx   0 root         (0) root         (0)      175 2023-04-18 18:45:49.000000 roof_mask_Yv8-0.5.7/detectron2/utils/README.md
--rwxrwxrwx   0 root         (0) root         (0)       51 2023-04-18 18:45:50.000000 roof_mask_Yv8-0.5.7/detectron2/utils/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     6017 2023-04-18 18:45:48.000000 roof_mask_Yv8-0.5.7/detectron2/utils/analysis.py
--rwxrwxrwx   0 root         (0) root         (0)     8391 2023-04-18 18:45:48.000000 roof_mask_Yv8-0.5.7/detectron2/utils/collect_env.py
--rwxrwxrwx   0 root         (0) root         (0)     4096 2023-04-18 18:45:48.000000 roof_mask_Yv8-0.5.7/detectron2/utils/colormap.py
--rwxrwxrwx   0 root         (0) root         (0)     5610 2023-04-18 18:45:48.000000 roof_mask_Yv8-0.5.7/detectron2/utils/comm.py
--rwxrwxrwx   0 root         (0) root         (0)     1838 2023-04-18 18:45:48.000000 roof_mask_Yv8-0.5.7/detectron2/utils/develop.py
--rwxrwxrwx   0 root         (0) root         (0)     5644 2023-04-18 18:45:48.000000 roof_mask_Yv8-0.5.7/detectron2/utils/env.py
--rwxrwxrwx   0 root         (0) root         (0)    17024 2023-04-18 18:45:49.000000 roof_mask_Yv8-0.5.7/detectron2/utils/events.py
--rwxrwxrwx   0 root         (0) root         (0)     1189 2023-04-18 18:45:49.000000 roof_mask_Yv8-0.5.7/detectron2/utils/file_io.py
--rwxrwxrwx   0 root         (0) root         (0)     7807 2023-04-18 18:45:49.000000 roof_mask_Yv8-0.5.7/detectron2/utils/logger.py
--rwxrwxrwx   0 root         (0) root         (0)     2583 2023-04-18 18:45:49.000000 roof_mask_Yv8-0.5.7/detectron2/utils/memory.py
--rwxrwxrwx   0 root         (0) root         (0)     1874 2023-04-18 18:45:49.000000 roof_mask_Yv8-0.5.7/detectron2/utils/registry.py
--rwxrwxrwx   0 root         (0) root         (0)     1064 2023-04-18 18:45:49.000000 roof_mask_Yv8-0.5.7/detectron2/utils/serialize.py
--rwxrwxrwx   0 root         (0) root         (0)     4833 2023-04-18 18:45:49.000000 roof_mask_Yv8-0.5.7/detectron2/utils/testing.py
--rwxrwxrwx   0 root         (0) root         (0)    11319 2023-04-18 18:45:49.000000 roof_mask_Yv8-0.5.7/detectron2/utils/video_visualizer.py
--rwxrwxrwx   0 root         (0) root         (0)    51159 2023-04-18 18:45:49.000000 roof_mask_Yv8-0.5.7/detectron2/utils/visualizer.py
--rwxrwxrwx   0 root         (0) root         (0)    52915 2023-04-18 18:45:49.000000 roof_mask_Yv8-0.5.7/detectron2/utils/visualizer_new.py
--rwxrwxrwx   0 root         (0) root         (0)      107 2023-04-17 21:19:17.000000 roof_mask_Yv8-0.5.7/readme.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-21 14:44:02.630160 roof_mask_Yv8-0.5.7/roof_mask_Yv8.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)      426 2023-04-21 14:44:31.000000 roof_mask_Yv8-0.5.7/roof_mask_Yv8.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     9337 2023-04-21 14:44:00.000000 roof_mask_Yv8-0.5.7/roof_mask_Yv8.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-21 14:44:31.000000 roof_mask_Yv8-0.5.7/roof_mask_Yv8.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       33 2023-04-21 14:44:31.000000 roof_mask_Yv8-0.5.7/roof_mask_Yv8.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-04-21 14:44:43.411771 roof_mask_Yv8-0.5.7/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      632 2023-04-21 14:44:04.000000 roof_mask_Yv8-0.5.7/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-21 14:44:02.680132 roof_mask_Yv8-0.5.7/tests/
--rwxrwxrwx   0 root         (0) root         (0)     3211 2023-04-19 15:22:00.000000 roof_mask_Yv8-0.5.7/tests/test.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-21 14:44:02.724106 roof_mask_Yv8-0.5.7/ultralytics/
--rwxrwxrwx   0 root         (0) root         (0)      295 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.7/ultralytics/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-21 14:44:02.821050 roof_mask_Yv8-0.5.7/ultralytics/hub/
--rwxrwxrwx   0 root         (0) root         (0)     3421 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.7/ultralytics/hub/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     5206 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.7/ultralytics/hub/auth.py
--rwxrwxrwx   0 root         (0) root         (0)     8690 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.7/ultralytics/hub/session.py
--rwxrwxrwx   0 root         (0) root         (0)     9723 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.7/ultralytics/hub/utils.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-21 14:44:02.891010 roof_mask_Yv8-0.5.7/ultralytics/nn/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.7/ultralytics/nn/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    24083 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.7/ultralytics/nn/autobackend.py
--rwxrwxrwx   0 root         (0) root         (0)    11839 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.7/ultralytics/nn/autoshape.py
--rwxrwxrwx   0 root         (0) root         (0)    20062 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.7/ultralytics/nn/modules.py
--rwxrwxrwx   0 root         (0) root         (0)    26619 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.7/ultralytics/nn/tasks.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-21 14:44:02.959970 roof_mask_Yv8-0.5.7/ultralytics/yolo/
--rwxrwxrwx   0 root         (0) root         (0)       93 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.7/ultralytics/yolo/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-21 14:44:03.010941 roof_mask_Yv8-0.5.7/ultralytics/yolo/cfg/
--rwxrwxrwx   0 root         (0) root         (0)    17582 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.7/ultralytics/yolo/cfg/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     6237 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.7/ultralytics/yolo/cfg/default.yaml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-21 14:44:03.054916 roof_mask_Yv8-0.5.7/ultralytics/yolo/data/
--rwxrwxrwx   0 root         (0) root         (0)      483 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.7/ultralytics/yolo/data/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    31285 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.7/ultralytics/yolo/data/augment.py
--rwxrwxrwx   0 root         (0) root         (0)     8919 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.7/ultralytics/yolo/data/base.py
--rwxrwxrwx   0 root         (0) root         (0)     8614 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.7/ultralytics/yolo/data/build.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-21 14:44:03.127874 roof_mask_Yv8-0.5.7/ultralytics/yolo/data/dataloaders/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.7/ultralytics/yolo/data/dataloaders/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    15194 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.7/ultralytics/yolo/data/dataloaders/stream_loaders.py
--rwxrwxrwx   0 root         (0) root         (0)    17226 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.7/ultralytics/yolo/data/dataloaders/v5augmentations.py
--rwxrwxrwx   0 root         (0) root         (0)    49861 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.7/ultralytics/yolo/data/dataloaders/v5loader.py
--rwxrwxrwx   0 root         (0) root         (0)    12740 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.7/ultralytics/yolo/data/dataset.py
--rwxrwxrwx   0 root         (0) root         (0)     1330 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.7/ultralytics/yolo/data/dataset_wrappers.py
--rwxrwxrwx   0 root         (0) root         (0)    22728 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.7/ultralytics/yolo/data/utils.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-21 14:44:03.162854 roof_mask_Yv8-0.5.7/ultralytics/yolo/engine/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.7/ultralytics/yolo/engine/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    41854 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.7/ultralytics/yolo/engine/exporter.py
--rwxrwxrwx   0 root         (0) root         (0)    21469 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.7/ultralytics/yolo/engine/model.py
--rwxrwxrwx   0 root         (0) root         (0)    14720 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.7/ultralytics/yolo/engine/predictor.py
--rwxrwxrwx   0 root         (0) root         (0)    17378 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.7/ultralytics/yolo/engine/results.py
--rwxrwxrwx   0 root         (0) root         (0)    29843 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.7/ultralytics/yolo/engine/trainer.py
--rwxrwxrwx   0 root         (0) root         (0)    10358 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.7/ultralytics/yolo/engine/validator.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-21 14:44:03.210826 roof_mask_Yv8-0.5.7/ultralytics/yolo/utils/
--rwxrwxrwx   0 root         (0) root         (0)    25215 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.7/ultralytics/yolo/utils/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     3823 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.7/ultralytics/yolo/utils/autobatch.py
--rwxrwxrwx   0 root         (0) root         (0)     5414 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.7/ultralytics/yolo/utils/benchmarks.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-21 14:44:03.276788 roof_mask_Yv8-0.5.7/ultralytics/yolo/utils/callbacks/
--rwxrwxrwx   0 root         (0) root         (0)      171 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.7/ultralytics/yolo/utils/callbacks/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     3783 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.7/ultralytics/yolo/utils/callbacks/base.py
--rwxrwxrwx   0 root         (0) root         (0)     5286 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.7/ultralytics/yolo/utils/callbacks/clearml.py
--rwxrwxrwx   0 root         (0) root         (0)    11929 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.7/ultralytics/yolo/utils/callbacks/comet.py
--rwxrwxrwx   0 root         (0) root         (0)     3189 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.7/ultralytics/yolo/utils/callbacks/hub.py
--rwxrwxrwx   0 root         (0) root         (0)     2512 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.7/ultralytics/yolo/utils/callbacks/mlflow.py
--rwxrwxrwx   0 root         (0) root         (0)      385 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.7/ultralytics/yolo/utils/callbacks/raytune.py
--rwxrwxrwx   0 root         (0) root         (0)     1297 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.7/ultralytics/yolo/utils/callbacks/tensorboard.py
--rwxrwxrwx   0 root         (0) root         (0)     1593 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.7/ultralytics/yolo/utils/callbacks/wb.py
--rwxrwxrwx   0 root         (0) root         (0)    14190 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.7/ultralytics/yolo/utils/checks.py
--rwxrwxrwx   0 root         (0) root         (0)     2412 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.7/ultralytics/yolo/utils/dist.py
--rwxrwxrwx   0 root         (0) root         (0)    10052 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.7/ultralytics/yolo/utils/downloads.py
--rwxrwxrwx   0 root         (0) root         (0)      251 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.7/ultralytics/yolo/utils/errors.py
--rwxrwxrwx   0 root         (0) root         (0)     3105 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.7/ultralytics/yolo/utils/files.py
--rwxrwxrwx   0 root         (0) root         (0)    11394 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.7/ultralytics/yolo/utils/instance.py
--rwxrwxrwx   0 root         (0) root         (0)     2889 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.7/ultralytics/yolo/utils/loss.py
--rwxrwxrwx   0 root         (0) root         (0)    35693 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.7/ultralytics/yolo/utils/metrics.py
--rwxrwxrwx   0 root         (0) root         (0)    28503 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.7/ultralytics/yolo/utils/ops.py
--rwxrwxrwx   0 root         (0) root         (0)    20613 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.7/ultralytics/yolo/utils/plotting.py
--rwxrwxrwx   0 root         (0) root         (0)    10233 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.7/ultralytics/yolo/utils/tal.py
--rwxrwxrwx   0 root         (0) root         (0)    19694 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.7/ultralytics/yolo/utils/torch_utils.py
--rwxrwxrwx   0 root         (0) root         (0)     2302 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.7/ultralytics/yolo/utils/tuner.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-21 14:44:03.312768 roof_mask_Yv8-0.5.7/ultralytics/yolo/v8/
--rwxrwxrwx   0 root         (0) root         (0)      157 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.7/ultralytics/yolo/v8/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-21 14:44:03.366736 roof_mask_Yv8-0.5.7/ultralytics/yolo/v8/classify/
--rwxrwxrwx   0 root         (0) root         (0)      390 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.7/ultralytics/yolo/v8/classify/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1459 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.7/ultralytics/yolo/v8/classify/predict.py
--rwxrwxrwx   0 root         (0) root         (0)     6388 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.7/ultralytics/yolo/v8/classify/train.py
--rwxrwxrwx   0 root         (0) root         (0)     2933 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.7/ultralytics/yolo/v8/classify/val.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-21 14:44:03.411712 roof_mask_Yv8-0.5.7/ultralytics/yolo/v8/detect/
--rwxrwxrwx   0 root         (0) root         (0)      276 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.7/ultralytics/yolo/v8/detect/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     2005 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.7/ultralytics/yolo/v8/detect/predict.py
--rwxrwxrwx   0 root         (0) root         (0)     9886 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.7/ultralytics/yolo/v8/detect/train.py
--rwxrwxrwx   0 root         (0) root         (0)    12516 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.7/ultralytics/yolo/v8/detect/val.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-21 14:44:03.471676 roof_mask_Yv8-0.5.7/ultralytics/yolo/v8/pose/
--rwxrwxrwx   0 root         (0) root         (0)      246 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.7/ultralytics/yolo/v8/pose/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     2076 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.7/ultralytics/yolo/v8/pose/predict.py
--rwxrwxrwx   0 root         (0) root         (0)     7145 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.7/ultralytics/yolo/v8/pose/train.py
--rwxrwxrwx   0 root         (0) root         (0)    10050 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.7/ultralytics/yolo/v8/pose/val.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-21 14:44:03.537638 roof_mask_Yv8-0.5.7/ultralytics/yolo/v8/segment/
--rwxrwxrwx   0 root         (0) root         (0)      294 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.7/ultralytics/yolo/v8/segment/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     2657 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.7/ultralytics/yolo/v8/segment/predict.py
--rwxrwxrwx   0 root         (0) root         (0)     7664 2023-04-17 21:04:31.000000 roof_mask_Yv8-0.5.7/ultralytics/yolo/v8/segment/train.py
--rwxrwxrwx   0 root         (0) root         (0)    11922 2023-04-17 21:04:31.000000 roof_mask_Yv8-0.5.7/ultralytics/yolo/v8/segment/val.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-21 14:44:03.603600 roof_mask_Yv8-0.5.7/yolo_roof/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-17 21:04:31.000000 roof_mask_Yv8-0.5.7/yolo_roof/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    33279 2023-04-19 14:59:59.000000 roof_mask_Yv8-0.5.7/yolo_roof/detect_functions.py
--rwxrwxrwx   0 root         (0) root         (0)    21398 2023-04-21 14:44:43.000000 roof_mask_Yv8-0.5.7/yolo_roof/geo_functions.py
--rwxrwxrwx   0 root         (0) root         (0)    41759 2023-04-18 18:11:13.000000 roof_mask_Yv8-0.5.7/yolo_roof/report_functions.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:39.966410 roof_mask_Yv8-0.5.8/
+-rwxrwxrwx   0 root         (0) root         (0)      149 2023-04-27 19:14:59.000000 roof_mask_Yv8-0.5.8/.gitignore
+-rwxrwxrwx   0 root         (0) root         (0)       41 2023-04-20 18:44:18.000000 roof_mask_Yv8-0.5.8/MANIFEST.in
+-rwxrwxrwx   0 root         (0) root         (0)      473 2023-04-28 21:02:21.955967 roof_mask_Yv8-0.5.8/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.8/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:40.015382 roof_mask_Yv8-0.5.8/detectron2/
+-rwxrwxrwx   0 root         (0) root         (0)      258 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.8/detectron2/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:40.080345 roof_mask_Yv8-0.5.8/detectron2/checkpoint/
+-rwxrwxrwx   0 root         (0) root         (0)      347 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.8/detectron2/checkpoint/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    17782 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.8/detectron2/checkpoint/c2_model_loading.py
+-rwxrwxrwx   0 root         (0) root         (0)     5685 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.8/detectron2/checkpoint/catalog.py
+-rwxrwxrwx   0 root         (0) root         (0)     5258 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.8/detectron2/checkpoint/detection_checkpoint.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:40.145308 roof_mask_Yv8-0.5.8/detectron2/config/
+-rwxrwxrwx   0 root         (0) root         (0)      599 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.8/detectron2/config/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     7890 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.8/detectron2/config/compat.py
+-rwxrwxrwx   0 root         (0) root         (0)     9211 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.8/detectron2/config/config.py
+-rwxrwxrwx   0 root         (0) root         (0)    29512 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.8/detectron2/config/defaults.py
+-rwxrwxrwx   0 root         (0) root         (0)     2719 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.8/detectron2/config/instantiate.py
+-rwxrwxrwx   0 root         (0) root         (0)    14944 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.8/detectron2/config/lazy.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:40.204274 roof_mask_Yv8-0.5.8/detectron2/data/
+-rwxrwxrwx   0 root         (0) root         (0)      644 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.8/detectron2/data/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     7378 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.8/detectron2/data/benchmark.py
+-rwxrwxrwx   0 root         (0) root         (0)    20605 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.8/detectron2/data/build.py
+-rwxrwxrwx   0 root         (0) root         (0)     7224 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.8/detectron2/data/catalog.py
+-rwxrwxrwx   0 root         (0) root         (0)     9164 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.8/detectron2/data/common.py
+-rwxrwxrwx   0 root         (0) root         (0)     8169 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.8/detectron2/data/dataset_mapper.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:40.267238 roof_mask_Yv8-0.5.8/detectron2/data/datasets/
+-rwxrwxrwx   0 root         (0) root         (0)      347 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.8/detectron2/data/datasets/README.md
+-rwxrwxrwx   0 root         (0) root         (0)      523 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.8/detectron2/data/datasets/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    10174 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.8/detectron2/data/datasets/builtin.py
+-rwxrwxrwx   0 root         (0) root         (0)    21841 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.8/detectron2/data/datasets/builtin_meta.py
+-rwxrwxrwx   0 root         (0) root         (0)    13167 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.8/detectron2/data/datasets/cityscapes.py
+-rwxrwxrwx   0 root         (0) root         (0)     7821 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.8/detectron2/data/datasets/cityscapes_panoptic.py
+-rwxrwxrwx   0 root         (0) root         (0)    23465 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.8/detectron2/data/datasets/coco.py
+-rwxrwxrwx   0 root         (0) root         (0)     8977 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.8/detectron2/data/datasets/coco_panoptic.py
+-rwxrwxrwx   0 root         (0) root         (0)     9623 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.8/detectron2/data/datasets/lvis.py
+-rwxrwxrwx   0 root         (0) root         (0)   223757 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.8/detectron2/data/datasets/lvis_v0_5_categories.py
+-rwxrwxrwx   0 root         (0) root         (0)   219177 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.8/detectron2/data/datasets/lvis_v1_categories.py
+-rwxrwxrwx   0 root         (0) root         (0)    39414 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.8/detectron2/data/datasets/lvis_v1_category_image_count.py
+-rwxrwxrwx   0 root         (0) root         (0)     3128 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.8/detectron2/data/datasets/pascal_voc.py
+-rwxrwxrwx   0 root         (0) root         (0)      169 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.8/detectron2/data/datasets/register_coco.py
+-rwxrwxrwx   0 root         (0) root         (0)    22841 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.8/detectron2/data/detection_utils.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:40.341196 roof_mask_Yv8-0.5.8/detectron2/data/samplers/
+-rwxrwxrwx   0 root         (0) root         (0)      412 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.8/detectron2/data/samplers/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    11789 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.8/detectron2/data/samplers/distributed_sampler.py
+-rwxrwxrwx   0 root         (0) root         (0)     1944 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.8/detectron2/data/samplers/grouped_batch_sampler.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:40.415153 roof_mask_Yv8-0.5.8/detectron2/data/transforms/
+-rwxrwxrwx   0 root         (0) root         (0)      466 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.8/detectron2/data/transforms/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    14117 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.8/detectron2/data/transforms/augmentation.py
+-rwxrwxrwx   0 root         (0) root         (0)    23069 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.8/detectron2/data/transforms/augmentation_impl.py
+-rwxrwxrwx   0 root         (0) root         (0)    12629 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.8/detectron2/data/transforms/transform.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:40.469122 roof_mask_Yv8-0.5.8/detectron2/engine/
+-rwxrwxrwx   0 root         (0) root         (0)      340 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.8/detectron2/engine/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    26868 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.8/detectron2/engine/defaults.py
+-rwxrwxrwx   0 root         (0) root         (0)    25497 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.8/detectron2/engine/hooks.py
+-rwxrwxrwx   0 root         (0) root         (0)     4089 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.8/detectron2/engine/launch.py
+-rwxrwxrwx   0 root         (0) root         (0)    14104 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.8/detectron2/engine/train_loop.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:40.536084 roof_mask_Yv8-0.5.8/detectron2/evaluation/
+-rwxrwxrwx   0 root         (0) root         (0)      671 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.8/detectron2/evaluation/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     8369 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.8/detectron2/evaluation/cityscapes_evaluation.py
+-rwxrwxrwx   0 root         (0) root         (0)    30423 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.8/detectron2/evaluation/coco_evaluation.py
+-rwxrwxrwx   0 root         (0) root         (0)     8156 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.8/detectron2/evaluation/evaluator.py
+-rwxrwxrwx   0 root         (0) root         (0)     5078 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.8/detectron2/evaluation/fast_eval_api.py
+-rwxrwxrwx   0 root         (0) root         (0)    15018 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.8/detectron2/evaluation/lvis_evaluation.py
+-rwxrwxrwx   0 root         (0) root         (0)     7500 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.8/detectron2/evaluation/panoptic_evaluation.py
+-rwxrwxrwx   0 root         (0) root         (0)    10862 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.8/detectron2/evaluation/pascal_voc_evaluation.py
+-rwxrwxrwx   0 root         (0) root         (0)     7608 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.8/detectron2/evaluation/rotated_coco_evaluation.py
+-rwxrwxrwx   0 root         (0) root         (0)     8191 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.8/detectron2/evaluation/sem_seg_evaluation.py
+-rwxrwxrwx   0 root         (0) root         (0)     2614 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.8/detectron2/evaluation/testing.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:40.612041 roof_mask_Yv8-0.5.8/detectron2/export/
+-rwxrwxrwx   0 root         (0) root         (0)      513 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.8/detectron2/export/README.md
+-rwxrwxrwx   0 root         (0) root         (0)      336 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.8/detectron2/export/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     9280 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.8/detectron2/export/api.py
+-rwxrwxrwx   0 root         (0) root         (0)    21035 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.8/detectron2/export/c10.py
+-rwxrwxrwx   0 root         (0) root         (0)     7803 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.8/detectron2/export/caffe2_export.py
+-rwxrwxrwx   0 root         (0) root         (0)     6674 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.8/detectron2/export/caffe2_inference.py
+-rwxrwxrwx   0 root         (0) root         (0)    17034 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.8/detectron2/export/caffe2_modeling.py
+-rwxrwxrwx   0 root         (0) root         (0)     5033 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.8/detectron2/export/caffe2_patch.py
+-rwxrwxrwx   0 root         (0) root         (0)    11807 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.8/detectron2/export/flatten.py
+-rwxrwxrwx   0 root         (0) root         (0)    38071 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.8/detectron2/export/shared.py
+-rwxrwxrwx   0 root         (0) root         (0)     5008 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.8/detectron2/export/torchscript.py
+-rwxrwxrwx   0 root         (0) root         (0)    11526 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.8/detectron2/export/torchscript_patch.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:40.696993 roof_mask_Yv8-0.5.8/detectron2/layers/
+-rwxrwxrwx   0 root         (0) root         (0)      839 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.8/detectron2/layers/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     5764 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.8/detectron2/layers/aspp.py
+-rwxrwxrwx   0 root         (0) root         (0)    12131 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.8/detectron2/layers/batch_norm.py
+-rwxrwxrwx   0 root         (0) root         (0)     3024 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.8/detectron2/layers/blocks.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:40.776947 roof_mask_Yv8-0.5.8/detectron2/layers/csrc/
+-rwxrwxrwx   0 root         (0) root         (0)      122 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.8/detectron2/layers/csrc/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:40.857900 roof_mask_Yv8-0.5.8/detectron2/layers/csrc/ROIAlignRotated/
+-rwxrwxrwx   0 root         (0) root         (0)     2870 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.8/detectron2/layers/csrc/ROIAlignRotated/ROIAlignRotated.h
+-rwxrwxrwx   0 root         (0) root         (0)    16031 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.8/detectron2/layers/csrc/ROIAlignRotated/ROIAlignRotated_cpu.cpp
+-rwxrwxrwx   0 root         (0) root         (0)    13876 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.8/detectron2/layers/csrc/ROIAlignRotated/ROIAlignRotated_cuda.cu
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:40.933856 roof_mask_Yv8-0.5.8/detectron2/layers/csrc/box_iou_rotated/
+-rwxrwxrwx   0 root         (0) root         (0)      988 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.8/detectron2/layers/csrc/box_iou_rotated/box_iou_rotated.h
+-rwxrwxrwx   0 root         (0) root         (0)     1090 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.8/detectron2/layers/csrc/box_iou_rotated/box_iou_rotated_cpu.cpp
+-rwxrwxrwx   0 root         (0) root         (0)     4454 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.8/detectron2/layers/csrc/box_iou_rotated/box_iou_rotated_cuda.cu
+-rwxrwxrwx   0 root         (0) root         (0)    10844 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.8/detectron2/layers/csrc/box_iou_rotated/box_iou_rotated_utils.h
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:41.238682 roof_mask_Yv8-0.5.8/detectron2/layers/csrc/cocoeval/
+-rwxrwxrwx   0 root         (0) root         (0)    20746 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.8/detectron2/layers/csrc/cocoeval/cocoeval.cpp
+-rwxrwxrwx   0 root         (0) root         (0)     3515 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.8/detectron2/layers/csrc/cocoeval/cocoeval.h
+-rwxrwxrwx   0 root         (0) root         (0)      622 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.8/detectron2/layers/csrc/cuda_version.cu
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:41.307643 roof_mask_Yv8-0.5.8/detectron2/layers/csrc/deformable/
+-rwxrwxrwx   0 root         (0) root         (0)     8384 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.8/detectron2/layers/csrc/deformable/deform_conv.h
+-rwxrwxrwx   0 root         (0) root         (0)    31785 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.8/detectron2/layers/csrc/deformable/deform_conv_cuda.cu
+-rwxrwxrwx   0 root         (0) root         (0)    44279 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.8/detectron2/layers/csrc/deformable/deform_conv_cuda_kernel.cu
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:41.368609 roof_mask_Yv8-0.5.8/detectron2/layers/csrc/nms_rotated/
+-rwxrwxrwx   0 root         (0) root         (0)     1089 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.8/detectron2/layers/csrc/nms_rotated/nms_rotated.h
+-rwxrwxrwx   0 root         (0) root         (0)     2307 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.8/detectron2/layers/csrc/nms_rotated/nms_rotated_cpu.cpp
+-rwxrwxrwx   0 root         (0) root         (0)     4859 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.8/detectron2/layers/csrc/nms_rotated/nms_rotated_cuda.cu
+-rwxrwxrwx   0 root         (0) root         (0)     3167 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.8/detectron2/layers/csrc/vision.cpp
+-rwxrwxrwx   0 root         (0) root         (0)    16978 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.8/detectron2/layers/deform_conv.py
+-rwxrwxrwx   0 root         (0) root         (0)     4204 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.8/detectron2/layers/losses.py
+-rwxrwxrwx   0 root         (0) root         (0)    10881 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.8/detectron2/layers/mask_ops.py
+-rwxrwxrwx   0 root         (0) root         (0)     6490 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.8/detectron2/layers/nms.py
+-rwxrwxrwx   0 root         (0) root         (0)     3098 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.8/detectron2/layers/roi_align.py
+-rwxrwxrwx   0 root         (0) root         (0)     3302 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.8/detectron2/layers/roi_align_rotated.py
+-rwxrwxrwx   0 root         (0) root         (0)      652 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.8/detectron2/layers/rotated_boxes.py
+-rwxrwxrwx   0 root         (0) root         (0)      661 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.8/detectron2/layers/shape_spec.py
+-rwxrwxrwx   0 root         (0) root         (0)     4893 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.8/detectron2/layers/wrappers.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:41.416581 roof_mask_Yv8-0.5.8/detectron2/modeling/
+-rwxrwxrwx   0 root         (0) root         (0)     1475 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.8/detectron2/modeling/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    15443 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.8/detectron2/modeling/anchor_generator.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:41.485541 roof_mask_Yv8-0.5.8/detectron2/modeling/backbone/
+-rwxrwxrwx   0 root         (0) root         (0)      475 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.8/detectron2/modeling/backbone/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1543 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.8/detectron2/modeling/backbone/backbone.py
+-rwxrwxrwx   0 root         (0) root         (0)     1015 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.8/detectron2/modeling/backbone/build.py
+-rwxrwxrwx   0 root         (0) root         (0)    10055 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.8/detectron2/modeling/backbone/fpn.py
+-rwxrwxrwx   0 root         (0) root         (0)    16656 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.8/detectron2/modeling/backbone/regnet.py
+-rwxrwxrwx   0 root         (0) root         (0)    23658 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.8/detectron2/modeling/backbone/resnet.py
+-rwxrwxrwx   0 root         (0) root         (0)    15123 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.8/detectron2/modeling/box_regression.py
+-rwxrwxrwx   0 root         (0) root         (0)     6264 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.8/detectron2/modeling/matcher.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:41.546506 roof_mask_Yv8-0.5.8/detectron2/modeling/meta_arch/
+-rwxrwxrwx   0 root         (0) root         (0)      508 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.8/detectron2/modeling/meta_arch/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      814 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.8/detectron2/modeling/meta_arch/build.py
+-rwxrwxrwx   0 root         (0) root         (0)    11550 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.8/detectron2/modeling/meta_arch/dense_detector.py
+-rwxrwxrwx   0 root         (0) root         (0)    13213 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.8/detectron2/modeling/meta_arch/fcos.py
+-rwxrwxrwx   0 root         (0) root         (0)    10335 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.8/detectron2/modeling/meta_arch/panoptic_fpn.py
+-rwxrwxrwx   0 root         (0) root         (0)    13710 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.8/detectron2/modeling/meta_arch/rcnn.py
+-rwxrwxrwx   0 root         (0) root         (0)    18265 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.8/detectron2/modeling/meta_arch/retinanet.py
+-rwxrwxrwx   0 root         (0) root         (0)     9720 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.8/detectron2/modeling/meta_arch/semantic_seg.py
+-rwxrwxrwx   0 root         (0) root         (0)    10832 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.8/detectron2/modeling/mmdet_wrapper.py
+-rwxrwxrwx   0 root         (0) root         (0)    11316 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.8/detectron2/modeling/poolers.py
+-rwxrwxrwx   0 root         (0) root         (0)     4046 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.8/detectron2/modeling/postprocessing.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:41.609471 roof_mask_Yv8-0.5.8/detectron2/modeling/proposal_generator/
+-rwxrwxrwx   0 root         (0) root         (0)      231 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.8/detectron2/modeling/proposal_generator/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      836 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.8/detectron2/modeling/proposal_generator/build.py
+-rwxrwxrwx   0 root         (0) root         (0)     8128 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.8/detectron2/modeling/proposal_generator/proposal_utils.py
+-rwxrwxrwx   0 root         (0) root         (0)    23814 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.8/detectron2/modeling/proposal_generator/rpn.py
+-rwxrwxrwx   0 root         (0) root         (0)     8807 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.8/detectron2/modeling/proposal_generator/rrpn.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:41.676432 roof_mask_Yv8-0.5.8/detectron2/modeling/roi_heads/
+-rwxrwxrwx   0 root         (0) root         (0)      768 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.8/detectron2/modeling/roi_heads/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4077 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.8/detectron2/modeling/roi_heads/box_head.py
+-rwxrwxrwx   0 root         (0) root         (0)    12990 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.8/detectron2/modeling/roi_heads/cascade_rcnn.py
+-rwxrwxrwx   0 root         (0) root         (0)    25274 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.8/detectron2/modeling/roi_heads/fast_rcnn.py
+-rwxrwxrwx   0 root         (0) root         (0)    11156 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.8/detectron2/modeling/roi_heads/keypoint_head.py
+-rwxrwxrwx   0 root         (0) root         (0)    12169 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.8/detectron2/modeling/roi_heads/mask_head.py
+-rwxrwxrwx   0 root         (0) root         (0)    37701 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.8/detectron2/modeling/roi_heads/roi_heads.py
+-rwxrwxrwx   0 root         (0) root         (0)    11158 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.8/detectron2/modeling/roi_heads/rotated_fast_rcnn.py
+-rwxrwxrwx   0 root         (0) root         (0)     2334 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.8/detectron2/modeling/sampling.py
+-rwxrwxrwx   0 root         (0) root         (0)    12416 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.8/detectron2/modeling/test_time_augmentation.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:41.730401 roof_mask_Yv8-0.5.8/detectron2/solver/
+-rwxrwxrwx   0 root         (0) root         (0)      298 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.8/detectron2/solver/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    11127 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.8/detectron2/solver/build.py
+-rwxrwxrwx   0 root         (0) root         (0)     8648 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.8/detectron2/solver/lr_scheduler.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:41.812354 roof_mask_Yv8-0.5.8/detectron2/structures/
+-rwxrwxrwx   0 root         (0) root         (0)      645 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.8/detectron2/structures/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    14429 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.8/detectron2/structures/boxes.py
+-rwxrwxrwx   0 root         (0) root         (0)     4557 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.8/detectron2/structures/image_list.py
+-rwxrwxrwx   0 root         (0) root         (0)     6542 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.8/detectron2/structures/instances.py
+-rwxrwxrwx   0 root         (0) root         (0)     9030 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.8/detectron2/structures/keypoints.py
+-rwxrwxrwx   0 root         (0) root         (0)    19802 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.8/detectron2/structures/masks.py
+-rwxrwxrwx   0 root         (0) root         (0)    18853 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.8/detectron2/structures/rotated_boxes.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:41.876318 roof_mask_Yv8-0.5.8/detectron2/tracking/
+-rwxrwxrwx   0 root         (0) root         (0)      580 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.8/detectron2/tracking/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     2216 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.8/detectron2/tracking/base_tracker.py
+-rwxrwxrwx   0 root         (0) root         (0)    11858 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.8/detectron2/tracking/bbox_iou_tracker.py
+-rwxrwxrwx   0 root         (0) root         (0)     7486 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.8/detectron2/tracking/hungarian_tracker.py
+-rwxrwxrwx   0 root         (0) root         (0)     4142 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.8/detectron2/tracking/iou_weighted_hungarian_bbox_iou_tracker.py
+-rwxrwxrwx   0 root         (0) root         (0)     1106 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.8/detectron2/tracking/utils.py
+-rwxrwxrwx   0 root         (0) root         (0)     5288 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.8/detectron2/tracking/vanilla_hungarian_bbox_iou_tracker.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:41.946280 roof_mask_Yv8-0.5.8/detectron2/utils/
+-rwxrwxrwx   0 root         (0) root         (0)      175 2023-04-18 18:45:49.000000 roof_mask_Yv8-0.5.8/detectron2/utils/README.md
+-rwxrwxrwx   0 root         (0) root         (0)       51 2023-04-18 18:45:50.000000 roof_mask_Yv8-0.5.8/detectron2/utils/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     6017 2023-04-18 18:45:48.000000 roof_mask_Yv8-0.5.8/detectron2/utils/analysis.py
+-rwxrwxrwx   0 root         (0) root         (0)     8391 2023-04-18 18:45:48.000000 roof_mask_Yv8-0.5.8/detectron2/utils/collect_env.py
+-rwxrwxrwx   0 root         (0) root         (0)     4096 2023-04-18 18:45:48.000000 roof_mask_Yv8-0.5.8/detectron2/utils/colormap.py
+-rwxrwxrwx   0 root         (0) root         (0)     5610 2023-04-18 18:45:48.000000 roof_mask_Yv8-0.5.8/detectron2/utils/comm.py
+-rwxrwxrwx   0 root         (0) root         (0)     1838 2023-04-18 18:45:48.000000 roof_mask_Yv8-0.5.8/detectron2/utils/develop.py
+-rwxrwxrwx   0 root         (0) root         (0)     5644 2023-04-18 18:45:48.000000 roof_mask_Yv8-0.5.8/detectron2/utils/env.py
+-rwxrwxrwx   0 root         (0) root         (0)    17024 2023-04-18 18:45:49.000000 roof_mask_Yv8-0.5.8/detectron2/utils/events.py
+-rwxrwxrwx   0 root         (0) root         (0)     1189 2023-04-18 18:45:49.000000 roof_mask_Yv8-0.5.8/detectron2/utils/file_io.py
+-rwxrwxrwx   0 root         (0) root         (0)     7807 2023-04-18 18:45:49.000000 roof_mask_Yv8-0.5.8/detectron2/utils/logger.py
+-rwxrwxrwx   0 root         (0) root         (0)     2583 2023-04-18 18:45:49.000000 roof_mask_Yv8-0.5.8/detectron2/utils/memory.py
+-rwxrwxrwx   0 root         (0) root         (0)     1874 2023-04-18 18:45:49.000000 roof_mask_Yv8-0.5.8/detectron2/utils/registry.py
+-rwxrwxrwx   0 root         (0) root         (0)     1064 2023-04-18 18:45:49.000000 roof_mask_Yv8-0.5.8/detectron2/utils/serialize.py
+-rwxrwxrwx   0 root         (0) root         (0)     4833 2023-04-18 18:45:49.000000 roof_mask_Yv8-0.5.8/detectron2/utils/testing.py
+-rwxrwxrwx   0 root         (0) root         (0)    11319 2023-04-18 18:45:49.000000 roof_mask_Yv8-0.5.8/detectron2/utils/video_visualizer.py
+-rwxrwxrwx   0 root         (0) root         (0)    51159 2023-04-18 18:45:49.000000 roof_mask_Yv8-0.5.8/detectron2/utils/visualizer.py
+-rwxrwxrwx   0 root         (0) root         (0)    52915 2023-04-18 18:45:49.000000 roof_mask_Yv8-0.5.8/detectron2/utils/visualizer_new.py
+-rwxrwxrwx   0 root         (0) root         (0)      107 2023-04-17 21:19:17.000000 roof_mask_Yv8-0.5.8/readme.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:41.991252 roof_mask_Yv8-0.5.8/roof_mask_Yv8.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)      473 2023-04-28 21:01:37.000000 roof_mask_Yv8-0.5.8/roof_mask_Yv8.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     9347 2023-04-28 21:01:39.000000 roof_mask_Yv8-0.5.8/roof_mask_Yv8.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-28 21:01:37.000000 roof_mask_Yv8-0.5.8/roof_mask_Yv8.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       33 2023-04-28 21:01:37.000000 roof_mask_Yv8-0.5.8/roof_mask_Yv8.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:42.062211 roof_mask_Yv8-0.5.8/scoring/
+-rwxrwxrwx   0 root         (0) root         (0)     4374 2023-04-27 20:39:18.000000 roof_mask_Yv8-0.5.8/scoring/score_yolov8.py
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-04-28 21:02:22.035967 roof_mask_Yv8-0.5.8/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      632 2023-04-28 21:01:16.000000 roof_mask_Yv8-0.5.8/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:42.138168 roof_mask_Yv8-0.5.8/ultralytics/
+-rwxrwxrwx   0 root         (0) root         (0)      295 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.8/ultralytics/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:42.214124 roof_mask_Yv8-0.5.8/ultralytics/hub/
+-rwxrwxrwx   0 root         (0) root         (0)     3421 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.8/ultralytics/hub/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     5206 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.8/ultralytics/hub/auth.py
+-rwxrwxrwx   0 root         (0) root         (0)     8690 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.8/ultralytics/hub/session.py
+-rwxrwxrwx   0 root         (0) root         (0)     9723 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.8/ultralytics/hub/utils.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:42.274090 roof_mask_Yv8-0.5.8/ultralytics/nn/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.8/ultralytics/nn/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    24083 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.8/ultralytics/nn/autobackend.py
+-rwxrwxrwx   0 root         (0) root         (0)    11839 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.8/ultralytics/nn/autoshape.py
+-rwxrwxrwx   0 root         (0) root         (0)    20062 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.8/ultralytics/nn/modules.py
+-rwxrwxrwx   0 root         (0) root         (0)    26619 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.8/ultralytics/nn/tasks.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:42.332057 roof_mask_Yv8-0.5.8/ultralytics/yolo/
+-rwxrwxrwx   0 root         (0) root         (0)       93 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:42.399019 roof_mask_Yv8-0.5.8/ultralytics/yolo/cfg/
+-rwxrwxrwx   0 root         (0) root         (0)    17582 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/cfg/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     6237 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/cfg/default.yaml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:42.461983 roof_mask_Yv8-0.5.8/ultralytics/yolo/data/
+-rwxrwxrwx   0 root         (0) root         (0)      483 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/data/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    31285 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/data/augment.py
+-rwxrwxrwx   0 root         (0) root         (0)     8919 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/data/base.py
+-rwxrwxrwx   0 root         (0) root         (0)     8614 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/data/build.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:42.526945 roof_mask_Yv8-0.5.8/ultralytics/yolo/data/dataloaders/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/data/dataloaders/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    15194 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/data/dataloaders/stream_loaders.py
+-rwxrwxrwx   0 root         (0) root         (0)    17226 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/data/dataloaders/v5augmentations.py
+-rwxrwxrwx   0 root         (0) root         (0)    49861 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/data/dataloaders/v5loader.py
+-rwxrwxrwx   0 root         (0) root         (0)    12740 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/data/dataset.py
+-rwxrwxrwx   0 root         (0) root         (0)     1330 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/data/dataset_wrappers.py
+-rwxrwxrwx   0 root         (0) root         (0)    22728 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/data/utils.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:42.573919 roof_mask_Yv8-0.5.8/ultralytics/yolo/engine/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/engine/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    41854 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/engine/exporter.py
+-rwxrwxrwx   0 root         (0) root         (0)    21469 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/engine/model.py
+-rwxrwxrwx   0 root         (0) root         (0)    14720 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/engine/predictor.py
+-rwxrwxrwx   0 root         (0) root         (0)    17378 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/engine/results.py
+-rwxrwxrwx   0 root         (0) root         (0)    29843 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/engine/trainer.py
+-rwxrwxrwx   0 root         (0) root         (0)    10358 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/engine/validator.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:42.630886 roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/
+-rwxrwxrwx   0 root         (0) root         (0)    25215 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3823 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/autobatch.py
+-rwxrwxrwx   0 root         (0) root         (0)     5414 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/benchmarks.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:42.696849 roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/callbacks/
+-rwxrwxrwx   0 root         (0) root         (0)      171 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/callbacks/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3783 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/callbacks/base.py
+-rwxrwxrwx   0 root         (0) root         (0)     5286 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/callbacks/clearml.py
+-rwxrwxrwx   0 root         (0) root         (0)    11929 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/callbacks/comet.py
+-rwxrwxrwx   0 root         (0) root         (0)     3189 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/callbacks/hub.py
+-rwxrwxrwx   0 root         (0) root         (0)     2512 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/callbacks/mlflow.py
+-rwxrwxrwx   0 root         (0) root         (0)      385 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/callbacks/raytune.py
+-rwxrwxrwx   0 root         (0) root         (0)     1297 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/callbacks/tensorboard.py
+-rwxrwxrwx   0 root         (0) root         (0)     1593 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/callbacks/wb.py
+-rwxrwxrwx   0 root         (0) root         (0)    14190 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/checks.py
+-rwxrwxrwx   0 root         (0) root         (0)     2412 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/dist.py
+-rwxrwxrwx   0 root         (0) root         (0)    10052 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/downloads.py
+-rwxrwxrwx   0 root         (0) root         (0)      251 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/errors.py
+-rwxrwxrwx   0 root         (0) root         (0)     3105 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/files.py
+-rwxrwxrwx   0 root         (0) root         (0)    11394 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/instance.py
+-rwxrwxrwx   0 root         (0) root         (0)     2889 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/loss.py
+-rwxrwxrwx   0 root         (0) root         (0)    35693 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/metrics.py
+-rwxrwxrwx   0 root         (0) root         (0)    28503 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/ops.py
+-rwxrwxrwx   0 root         (0) root         (0)    20613 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/plotting.py
+-rwxrwxrwx   0 root         (0) root         (0)    10233 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/tal.py
+-rwxrwxrwx   0 root         (0) root         (0)    19694 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/torch_utils.py
+-rwxrwxrwx   0 root         (0) root         (0)     2302 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/tuner.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:42.748818 roof_mask_Yv8-0.5.8/ultralytics/yolo/v8/
+-rwxrwxrwx   0 root         (0) root         (0)      157 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/v8/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:42.804786 roof_mask_Yv8-0.5.8/ultralytics/yolo/v8/classify/
+-rwxrwxrwx   0 root         (0) root         (0)      390 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/v8/classify/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1459 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/v8/classify/predict.py
+-rwxrwxrwx   0 root         (0) root         (0)     6388 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/v8/classify/train.py
+-rwxrwxrwx   0 root         (0) root         (0)     2933 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/v8/classify/val.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:42.873747 roof_mask_Yv8-0.5.8/ultralytics/yolo/v8/detect/
+-rwxrwxrwx   0 root         (0) root         (0)      276 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/v8/detect/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     2005 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/v8/detect/predict.py
+-rwxrwxrwx   0 root         (0) root         (0)     9886 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/v8/detect/train.py
+-rwxrwxrwx   0 root         (0) root         (0)    12516 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/v8/detect/val.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:42.933713 roof_mask_Yv8-0.5.8/ultralytics/yolo/v8/pose/
+-rwxrwxrwx   0 root         (0) root         (0)      246 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/v8/pose/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     2076 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/v8/pose/predict.py
+-rwxrwxrwx   0 root         (0) root         (0)     7145 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/v8/pose/train.py
+-rwxrwxrwx   0 root         (0) root         (0)    10050 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/v8/pose/val.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:42.999675 roof_mask_Yv8-0.5.8/ultralytics/yolo/v8/segment/
+-rwxrwxrwx   0 root         (0) root         (0)      294 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/v8/segment/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     2657 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/v8/segment/predict.py
+-rwxrwxrwx   0 root         (0) root         (0)     7664 2023-04-17 21:04:31.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/v8/segment/train.py
+-rwxrwxrwx   0 root         (0) root         (0)    11922 2023-04-17 21:04:31.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/v8/segment/val.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:43.049647 roof_mask_Yv8-0.5.8/yolo_roof/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-17 21:04:31.000000 roof_mask_Yv8-0.5.8/yolo_roof/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    34971 2023-04-27 21:40:20.000000 roof_mask_Yv8-0.5.8/yolo_roof/detect_functions.py
+-rwxrwxrwx   0 root         (0) root         (0)    21398 2023-04-21 14:28:18.000000 roof_mask_Yv8-0.5.8/yolo_roof/geo_functions.py
+-rwxrwxrwx   0 root         (0) root         (0)    49443 2023-04-28 19:31:42.000000 roof_mask_Yv8-0.5.8/yolo_roof/report_functions.py
```

### Comparing `roof_mask_Yv8-0.5.7/detectron2/checkpoint/c2_model_loading.py` & `roof_mask_Yv8-0.5.8/detectron2/checkpoint/c2_model_loading.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/checkpoint/catalog.py` & `roof_mask_Yv8-0.5.8/detectron2/checkpoint/catalog.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/checkpoint/detection_checkpoint.py` & `roof_mask_Yv8-0.5.8/detectron2/checkpoint/detection_checkpoint.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/config/__init__.py` & `roof_mask_Yv8-0.5.8/detectron2/config/__init__.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/config/compat.py` & `roof_mask_Yv8-0.5.8/detectron2/config/compat.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/config/config.py` & `roof_mask_Yv8-0.5.8/detectron2/config/config.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/config/defaults.py` & `roof_mask_Yv8-0.5.8/detectron2/config/defaults.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/config/instantiate.py` & `roof_mask_Yv8-0.5.8/detectron2/config/instantiate.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/config/lazy.py` & `roof_mask_Yv8-0.5.8/detectron2/config/lazy.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/data/__init__.py` & `roof_mask_Yv8-0.5.8/detectron2/data/__init__.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/data/benchmark.py` & `roof_mask_Yv8-0.5.8/detectron2/data/benchmark.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/data/build.py` & `roof_mask_Yv8-0.5.8/detectron2/data/build.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/data/catalog.py` & `roof_mask_Yv8-0.5.8/detectron2/data/catalog.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/data/common.py` & `roof_mask_Yv8-0.5.8/detectron2/data/common.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/data/dataset_mapper.py` & `roof_mask_Yv8-0.5.8/detectron2/data/dataset_mapper.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/data/datasets/__init__.py` & `roof_mask_Yv8-0.5.8/detectron2/data/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/data/datasets/builtin.py` & `roof_mask_Yv8-0.5.8/detectron2/data/datasets/builtin.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/data/datasets/builtin_meta.py` & `roof_mask_Yv8-0.5.8/detectron2/data/datasets/builtin_meta.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/data/datasets/cityscapes.py` & `roof_mask_Yv8-0.5.8/detectron2/data/datasets/cityscapes.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/data/datasets/cityscapes_panoptic.py` & `roof_mask_Yv8-0.5.8/detectron2/data/datasets/cityscapes_panoptic.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/data/datasets/coco.py` & `roof_mask_Yv8-0.5.8/detectron2/data/datasets/coco.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/data/datasets/coco_panoptic.py` & `roof_mask_Yv8-0.5.8/detectron2/data/datasets/coco_panoptic.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/data/datasets/lvis.py` & `roof_mask_Yv8-0.5.8/detectron2/data/datasets/lvis.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/data/datasets/lvis_v0_5_categories.py` & `roof_mask_Yv8-0.5.8/detectron2/data/datasets/lvis_v0_5_categories.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/data/datasets/lvis_v1_categories.py` & `roof_mask_Yv8-0.5.8/detectron2/data/datasets/lvis_v1_categories.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/data/datasets/lvis_v1_category_image_count.py` & `roof_mask_Yv8-0.5.8/detectron2/data/datasets/lvis_v1_category_image_count.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/data/datasets/pascal_voc.py` & `roof_mask_Yv8-0.5.8/detectron2/data/datasets/pascal_voc.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/data/detection_utils.py` & `roof_mask_Yv8-0.5.8/detectron2/data/detection_utils.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/data/samplers/distributed_sampler.py` & `roof_mask_Yv8-0.5.8/detectron2/data/samplers/distributed_sampler.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/data/samplers/grouped_batch_sampler.py` & `roof_mask_Yv8-0.5.8/detectron2/data/samplers/grouped_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/data/transforms/augmentation.py` & `roof_mask_Yv8-0.5.8/detectron2/data/transforms/augmentation.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/data/transforms/augmentation_impl.py` & `roof_mask_Yv8-0.5.8/detectron2/data/transforms/augmentation_impl.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/data/transforms/transform.py` & `roof_mask_Yv8-0.5.8/detectron2/data/transforms/transform.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/engine/defaults.py` & `roof_mask_Yv8-0.5.8/detectron2/engine/defaults.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/engine/hooks.py` & `roof_mask_Yv8-0.5.8/detectron2/engine/hooks.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/engine/launch.py` & `roof_mask_Yv8-0.5.8/detectron2/engine/launch.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/engine/train_loop.py` & `roof_mask_Yv8-0.5.8/detectron2/engine/train_loop.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/evaluation/__init__.py` & `roof_mask_Yv8-0.5.8/detectron2/evaluation/__init__.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/evaluation/cityscapes_evaluation.py` & `roof_mask_Yv8-0.5.8/detectron2/evaluation/cityscapes_evaluation.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/evaluation/coco_evaluation.py` & `roof_mask_Yv8-0.5.8/detectron2/evaluation/coco_evaluation.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/evaluation/evaluator.py` & `roof_mask_Yv8-0.5.8/detectron2/evaluation/evaluator.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/evaluation/fast_eval_api.py` & `roof_mask_Yv8-0.5.8/detectron2/evaluation/fast_eval_api.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/evaluation/lvis_evaluation.py` & `roof_mask_Yv8-0.5.8/detectron2/evaluation/lvis_evaluation.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/evaluation/panoptic_evaluation.py` & `roof_mask_Yv8-0.5.8/detectron2/evaluation/panoptic_evaluation.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/evaluation/pascal_voc_evaluation.py` & `roof_mask_Yv8-0.5.8/detectron2/evaluation/pascal_voc_evaluation.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/evaluation/rotated_coco_evaluation.py` & `roof_mask_Yv8-0.5.8/detectron2/evaluation/rotated_coco_evaluation.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/evaluation/sem_seg_evaluation.py` & `roof_mask_Yv8-0.5.8/detectron2/evaluation/sem_seg_evaluation.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/evaluation/testing.py` & `roof_mask_Yv8-0.5.8/detectron2/evaluation/testing.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/export/README.md` & `roof_mask_Yv8-0.5.8/detectron2/export/README.md`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/export/api.py` & `roof_mask_Yv8-0.5.8/detectron2/export/api.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/export/c10.py` & `roof_mask_Yv8-0.5.8/detectron2/export/c10.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/export/caffe2_export.py` & `roof_mask_Yv8-0.5.8/detectron2/export/caffe2_export.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/export/caffe2_inference.py` & `roof_mask_Yv8-0.5.8/detectron2/export/caffe2_inference.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/export/caffe2_modeling.py` & `roof_mask_Yv8-0.5.8/detectron2/export/caffe2_modeling.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/export/caffe2_patch.py` & `roof_mask_Yv8-0.5.8/detectron2/export/caffe2_patch.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/export/flatten.py` & `roof_mask_Yv8-0.5.8/detectron2/export/flatten.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/export/shared.py` & `roof_mask_Yv8-0.5.8/detectron2/export/shared.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/export/torchscript.py` & `roof_mask_Yv8-0.5.8/detectron2/export/torchscript.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/export/torchscript_patch.py` & `roof_mask_Yv8-0.5.8/detectron2/export/torchscript_patch.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/layers/__init__.py` & `roof_mask_Yv8-0.5.8/detectron2/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/layers/aspp.py` & `roof_mask_Yv8-0.5.8/detectron2/layers/aspp.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/layers/batch_norm.py` & `roof_mask_Yv8-0.5.8/detectron2/layers/batch_norm.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/layers/blocks.py` & `roof_mask_Yv8-0.5.8/detectron2/layers/blocks.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/layers/csrc/ROIAlignRotated/ROIAlignRotated.h` & `roof_mask_Yv8-0.5.8/detectron2/layers/csrc/ROIAlignRotated/ROIAlignRotated.h`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/layers/csrc/ROIAlignRotated/ROIAlignRotated_cpu.cpp` & `roof_mask_Yv8-0.5.8/detectron2/layers/csrc/ROIAlignRotated/ROIAlignRotated_cpu.cpp`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/layers/csrc/ROIAlignRotated/ROIAlignRotated_cuda.cu` & `roof_mask_Yv8-0.5.8/detectron2/layers/csrc/ROIAlignRotated/ROIAlignRotated_cuda.cu`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/layers/csrc/box_iou_rotated/box_iou_rotated.h` & `roof_mask_Yv8-0.5.8/detectron2/layers/csrc/box_iou_rotated/box_iou_rotated.h`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/layers/csrc/box_iou_rotated/box_iou_rotated_cpu.cpp` & `roof_mask_Yv8-0.5.8/detectron2/layers/csrc/box_iou_rotated/box_iou_rotated_cpu.cpp`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/layers/csrc/box_iou_rotated/box_iou_rotated_cuda.cu` & `roof_mask_Yv8-0.5.8/detectron2/layers/csrc/box_iou_rotated/box_iou_rotated_cuda.cu`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/layers/csrc/box_iou_rotated/box_iou_rotated_utils.h` & `roof_mask_Yv8-0.5.8/detectron2/layers/csrc/box_iou_rotated/box_iou_rotated_utils.h`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/layers/csrc/cocoeval/cocoeval.cpp` & `roof_mask_Yv8-0.5.8/detectron2/layers/csrc/cocoeval/cocoeval.cpp`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/layers/csrc/cocoeval/cocoeval.h` & `roof_mask_Yv8-0.5.8/detectron2/layers/csrc/cocoeval/cocoeval.h`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/layers/csrc/cuda_version.cu` & `roof_mask_Yv8-0.5.8/detectron2/layers/csrc/cuda_version.cu`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/layers/csrc/deformable/deform_conv.h` & `roof_mask_Yv8-0.5.8/detectron2/layers/csrc/deformable/deform_conv.h`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/layers/csrc/deformable/deform_conv_cuda.cu` & `roof_mask_Yv8-0.5.8/detectron2/layers/csrc/deformable/deform_conv_cuda.cu`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/layers/csrc/deformable/deform_conv_cuda_kernel.cu` & `roof_mask_Yv8-0.5.8/detectron2/layers/csrc/deformable/deform_conv_cuda_kernel.cu`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/layers/csrc/nms_rotated/nms_rotated.h` & `roof_mask_Yv8-0.5.8/detectron2/layers/csrc/nms_rotated/nms_rotated.h`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/layers/csrc/nms_rotated/nms_rotated_cpu.cpp` & `roof_mask_Yv8-0.5.8/detectron2/layers/csrc/nms_rotated/nms_rotated_cpu.cpp`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/layers/csrc/nms_rotated/nms_rotated_cuda.cu` & `roof_mask_Yv8-0.5.8/detectron2/layers/csrc/nms_rotated/nms_rotated_cuda.cu`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/layers/csrc/vision.cpp` & `roof_mask_Yv8-0.5.8/detectron2/layers/csrc/vision.cpp`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/layers/deform_conv.py` & `roof_mask_Yv8-0.5.8/detectron2/layers/deform_conv.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/layers/losses.py` & `roof_mask_Yv8-0.5.8/detectron2/layers/losses.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/layers/mask_ops.py` & `roof_mask_Yv8-0.5.8/detectron2/layers/mask_ops.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/layers/nms.py` & `roof_mask_Yv8-0.5.8/detectron2/layers/nms.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/layers/roi_align.py` & `roof_mask_Yv8-0.5.8/detectron2/layers/roi_align.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/layers/roi_align_rotated.py` & `roof_mask_Yv8-0.5.8/detectron2/layers/roi_align_rotated.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/layers/rotated_boxes.py` & `roof_mask_Yv8-0.5.8/detectron2/layers/rotated_boxes.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/layers/shape_spec.py` & `roof_mask_Yv8-0.5.8/detectron2/layers/shape_spec.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/layers/wrappers.py` & `roof_mask_Yv8-0.5.8/detectron2/layers/wrappers.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/modeling/__init__.py` & `roof_mask_Yv8-0.5.8/detectron2/modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/modeling/anchor_generator.py` & `roof_mask_Yv8-0.5.8/detectron2/modeling/anchor_generator.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/modeling/backbone/backbone.py` & `roof_mask_Yv8-0.5.8/detectron2/modeling/backbone/backbone.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/modeling/backbone/build.py` & `roof_mask_Yv8-0.5.8/detectron2/modeling/backbone/build.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/modeling/backbone/fpn.py` & `roof_mask_Yv8-0.5.8/detectron2/modeling/backbone/fpn.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/modeling/backbone/regnet.py` & `roof_mask_Yv8-0.5.8/detectron2/modeling/backbone/regnet.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/modeling/backbone/resnet.py` & `roof_mask_Yv8-0.5.8/detectron2/modeling/backbone/resnet.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/modeling/box_regression.py` & `roof_mask_Yv8-0.5.8/detectron2/modeling/box_regression.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/modeling/matcher.py` & `roof_mask_Yv8-0.5.8/detectron2/modeling/matcher.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/modeling/meta_arch/build.py` & `roof_mask_Yv8-0.5.8/detectron2/modeling/meta_arch/build.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/modeling/meta_arch/dense_detector.py` & `roof_mask_Yv8-0.5.8/detectron2/modeling/meta_arch/dense_detector.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/modeling/meta_arch/fcos.py` & `roof_mask_Yv8-0.5.8/detectron2/modeling/meta_arch/fcos.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/modeling/meta_arch/panoptic_fpn.py` & `roof_mask_Yv8-0.5.8/detectron2/modeling/meta_arch/panoptic_fpn.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/modeling/meta_arch/rcnn.py` & `roof_mask_Yv8-0.5.8/detectron2/modeling/meta_arch/rcnn.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/modeling/meta_arch/retinanet.py` & `roof_mask_Yv8-0.5.8/detectron2/modeling/meta_arch/retinanet.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/modeling/meta_arch/semantic_seg.py` & `roof_mask_Yv8-0.5.8/detectron2/modeling/meta_arch/semantic_seg.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/modeling/mmdet_wrapper.py` & `roof_mask_Yv8-0.5.8/detectron2/modeling/mmdet_wrapper.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/modeling/poolers.py` & `roof_mask_Yv8-0.5.8/detectron2/modeling/poolers.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/modeling/postprocessing.py` & `roof_mask_Yv8-0.5.8/detectron2/modeling/postprocessing.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/modeling/proposal_generator/build.py` & `roof_mask_Yv8-0.5.8/detectron2/modeling/proposal_generator/build.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/modeling/proposal_generator/proposal_utils.py` & `roof_mask_Yv8-0.5.8/detectron2/modeling/proposal_generator/proposal_utils.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/modeling/proposal_generator/rpn.py` & `roof_mask_Yv8-0.5.8/detectron2/modeling/proposal_generator/rpn.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/modeling/proposal_generator/rrpn.py` & `roof_mask_Yv8-0.5.8/detectron2/modeling/proposal_generator/rrpn.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/modeling/roi_heads/__init__.py` & `roof_mask_Yv8-0.5.8/detectron2/modeling/roi_heads/__init__.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/modeling/roi_heads/box_head.py` & `roof_mask_Yv8-0.5.8/detectron2/modeling/roi_heads/box_head.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/modeling/roi_heads/cascade_rcnn.py` & `roof_mask_Yv8-0.5.8/detectron2/modeling/roi_heads/cascade_rcnn.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/modeling/roi_heads/fast_rcnn.py` & `roof_mask_Yv8-0.5.8/detectron2/modeling/roi_heads/fast_rcnn.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/modeling/roi_heads/keypoint_head.py` & `roof_mask_Yv8-0.5.8/detectron2/modeling/roi_heads/keypoint_head.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/modeling/roi_heads/mask_head.py` & `roof_mask_Yv8-0.5.8/detectron2/modeling/roi_heads/mask_head.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/modeling/roi_heads/roi_heads.py` & `roof_mask_Yv8-0.5.8/detectron2/modeling/roi_heads/roi_heads.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/modeling/roi_heads/rotated_fast_rcnn.py` & `roof_mask_Yv8-0.5.8/detectron2/modeling/roi_heads/rotated_fast_rcnn.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/modeling/sampling.py` & `roof_mask_Yv8-0.5.8/detectron2/modeling/sampling.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/modeling/test_time_augmentation.py` & `roof_mask_Yv8-0.5.8/detectron2/modeling/test_time_augmentation.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/solver/build.py` & `roof_mask_Yv8-0.5.8/detectron2/solver/build.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/solver/lr_scheduler.py` & `roof_mask_Yv8-0.5.8/detectron2/solver/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/structures/__init__.py` & `roof_mask_Yv8-0.5.8/detectron2/structures/__init__.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/structures/boxes.py` & `roof_mask_Yv8-0.5.8/detectron2/structures/boxes.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/structures/image_list.py` & `roof_mask_Yv8-0.5.8/detectron2/structures/image_list.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/structures/instances.py` & `roof_mask_Yv8-0.5.8/detectron2/structures/instances.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/structures/keypoints.py` & `roof_mask_Yv8-0.5.8/detectron2/structures/keypoints.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/structures/masks.py` & `roof_mask_Yv8-0.5.8/detectron2/structures/masks.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/structures/rotated_boxes.py` & `roof_mask_Yv8-0.5.8/detectron2/structures/rotated_boxes.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/tracking/__init__.py` & `roof_mask_Yv8-0.5.8/detectron2/tracking/__init__.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/tracking/base_tracker.py` & `roof_mask_Yv8-0.5.8/detectron2/tracking/base_tracker.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/tracking/bbox_iou_tracker.py` & `roof_mask_Yv8-0.5.8/detectron2/tracking/bbox_iou_tracker.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/tracking/hungarian_tracker.py` & `roof_mask_Yv8-0.5.8/detectron2/tracking/hungarian_tracker.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/tracking/iou_weighted_hungarian_bbox_iou_tracker.py` & `roof_mask_Yv8-0.5.8/detectron2/tracking/iou_weighted_hungarian_bbox_iou_tracker.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/tracking/utils.py` & `roof_mask_Yv8-0.5.8/detectron2/tracking/utils.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/tracking/vanilla_hungarian_bbox_iou_tracker.py` & `roof_mask_Yv8-0.5.8/detectron2/tracking/vanilla_hungarian_bbox_iou_tracker.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/utils/analysis.py` & `roof_mask_Yv8-0.5.8/detectron2/utils/analysis.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/utils/collect_env.py` & `roof_mask_Yv8-0.5.8/detectron2/utils/collect_env.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/utils/colormap.py` & `roof_mask_Yv8-0.5.8/detectron2/utils/colormap.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/utils/comm.py` & `roof_mask_Yv8-0.5.8/detectron2/utils/comm.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/utils/develop.py` & `roof_mask_Yv8-0.5.8/detectron2/utils/develop.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/utils/env.py` & `roof_mask_Yv8-0.5.8/detectron2/utils/env.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/utils/events.py` & `roof_mask_Yv8-0.5.8/detectron2/utils/events.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/utils/file_io.py` & `roof_mask_Yv8-0.5.8/detectron2/utils/file_io.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/utils/logger.py` & `roof_mask_Yv8-0.5.8/detectron2/utils/logger.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/utils/memory.py` & `roof_mask_Yv8-0.5.8/detectron2/utils/memory.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/utils/registry.py` & `roof_mask_Yv8-0.5.8/detectron2/utils/registry.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/utils/serialize.py` & `roof_mask_Yv8-0.5.8/detectron2/utils/serialize.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/utils/testing.py` & `roof_mask_Yv8-0.5.8/detectron2/utils/testing.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/utils/video_visualizer.py` & `roof_mask_Yv8-0.5.8/detectron2/utils/video_visualizer.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/utils/visualizer.py` & `roof_mask_Yv8-0.5.8/detectron2/utils/visualizer.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/detectron2/utils/visualizer_new.py` & `roof_mask_Yv8-0.5.8/detectron2/utils/visualizer_new.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/roof_mask_Yv8.egg-info/SOURCES.txt` & `roof_mask_Yv8-0.5.8/roof_mask_Yv8.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -172,15 +172,15 @@
 detectron2/utils/video_visualizer.py
 detectron2/utils/visualizer.py
 detectron2/utils/visualizer_new.py
 roof_mask_Yv8.egg-info/PKG-INFO
 roof_mask_Yv8.egg-info/SOURCES.txt
 roof_mask_Yv8.egg-info/dependency_links.txt
 roof_mask_Yv8.egg-info/top_level.txt
-tests/test.py
+scoring/score_yolov8.py
 ultralytics/__init__.py
 ultralytics/hub/__init__.py
 ultralytics/hub/auth.py
 ultralytics/hub/session.py
 ultralytics/hub/utils.py
 ultralytics/nn/__init__.py
 ultralytics/nn/autobackend.py
```

### Comparing `roof_mask_Yv8-0.5.7/setup.py` & `roof_mask_Yv8-0.5.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ## test upload
 import setuptools
 
 setuptools.setup(
     name = "roof_mask_Yv8",
-    version = "0.5.7",
+    version = "0.5.8",
     author = "Ruixu",
     author_email = "lrxjason@gmail.com",
     description = "upload pip package test",
     long_description = 'package supporing Yolo_v8 roof model backend.',
     long_description_content_type="text/markdown",
     url="https://github.com/lrxjason/roof_model_test/",
     packages=setuptools.find_packages(),
```

### Comparing `roof_mask_Yv8-0.5.7/ultralytics/hub/__init__.py` & `roof_mask_Yv8-0.5.8/ultralytics/hub/__init__.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/ultralytics/hub/auth.py` & `roof_mask_Yv8-0.5.8/ultralytics/hub/auth.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/ultralytics/hub/session.py` & `roof_mask_Yv8-0.5.8/ultralytics/hub/session.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/ultralytics/hub/utils.py` & `roof_mask_Yv8-0.5.8/ultralytics/hub/utils.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/ultralytics/nn/autobackend.py` & `roof_mask_Yv8-0.5.8/ultralytics/nn/autobackend.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/ultralytics/nn/autoshape.py` & `roof_mask_Yv8-0.5.8/ultralytics/nn/autoshape.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/ultralytics/nn/modules.py` & `roof_mask_Yv8-0.5.8/ultralytics/nn/modules.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/ultralytics/nn/tasks.py` & `roof_mask_Yv8-0.5.8/ultralytics/nn/tasks.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/ultralytics/yolo/cfg/__init__.py` & `roof_mask_Yv8-0.5.8/ultralytics/yolo/cfg/__init__.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/ultralytics/yolo/cfg/default.yaml` & `roof_mask_Yv8-0.5.8/ultralytics/yolo/cfg/default.yaml`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/ultralytics/yolo/data/augment.py` & `roof_mask_Yv8-0.5.8/ultralytics/yolo/data/augment.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/ultralytics/yolo/data/base.py` & `roof_mask_Yv8-0.5.8/ultralytics/yolo/data/base.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/ultralytics/yolo/data/build.py` & `roof_mask_Yv8-0.5.8/ultralytics/yolo/data/build.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/ultralytics/yolo/data/dataloaders/stream_loaders.py` & `roof_mask_Yv8-0.5.8/ultralytics/yolo/data/dataloaders/stream_loaders.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/ultralytics/yolo/data/dataloaders/v5augmentations.py` & `roof_mask_Yv8-0.5.8/ultralytics/yolo/data/dataloaders/v5augmentations.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/ultralytics/yolo/data/dataloaders/v5loader.py` & `roof_mask_Yv8-0.5.8/ultralytics/yolo/data/dataloaders/v5loader.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/ultralytics/yolo/data/dataset.py` & `roof_mask_Yv8-0.5.8/ultralytics/yolo/data/dataset.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/ultralytics/yolo/data/dataset_wrappers.py` & `roof_mask_Yv8-0.5.8/ultralytics/yolo/data/dataset_wrappers.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/ultralytics/yolo/data/utils.py` & `roof_mask_Yv8-0.5.8/ultralytics/yolo/data/utils.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/ultralytics/yolo/engine/exporter.py` & `roof_mask_Yv8-0.5.8/ultralytics/yolo/engine/exporter.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/ultralytics/yolo/engine/model.py` & `roof_mask_Yv8-0.5.8/ultralytics/yolo/engine/model.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/ultralytics/yolo/engine/predictor.py` & `roof_mask_Yv8-0.5.8/ultralytics/yolo/engine/predictor.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/ultralytics/yolo/engine/results.py` & `roof_mask_Yv8-0.5.8/ultralytics/yolo/engine/results.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/ultralytics/yolo/engine/trainer.py` & `roof_mask_Yv8-0.5.8/ultralytics/yolo/engine/trainer.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/ultralytics/yolo/engine/validator.py` & `roof_mask_Yv8-0.5.8/ultralytics/yolo/engine/validator.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/ultralytics/yolo/utils/__init__.py` & `roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/ultralytics/yolo/utils/autobatch.py` & `roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/autobatch.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/ultralytics/yolo/utils/benchmarks.py` & `roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/benchmarks.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/ultralytics/yolo/utils/callbacks/base.py` & `roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/ultralytics/yolo/utils/callbacks/clearml.py` & `roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/callbacks/clearml.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/ultralytics/yolo/utils/callbacks/comet.py` & `roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/callbacks/comet.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/ultralytics/yolo/utils/callbacks/hub.py` & `roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/callbacks/hub.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/ultralytics/yolo/utils/callbacks/mlflow.py` & `roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/callbacks/mlflow.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/ultralytics/yolo/utils/callbacks/tensorboard.py` & `roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/callbacks/tensorboard.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/ultralytics/yolo/utils/callbacks/wb.py` & `roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/callbacks/wb.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/ultralytics/yolo/utils/checks.py` & `roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/checks.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/ultralytics/yolo/utils/dist.py` & `roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/dist.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/ultralytics/yolo/utils/downloads.py` & `roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/downloads.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/ultralytics/yolo/utils/files.py` & `roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/files.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/ultralytics/yolo/utils/instance.py` & `roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/instance.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/ultralytics/yolo/utils/loss.py` & `roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/loss.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/ultralytics/yolo/utils/metrics.py` & `roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/ultralytics/yolo/utils/ops.py` & `roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/ops.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/ultralytics/yolo/utils/plotting.py` & `roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/ultralytics/yolo/utils/tal.py` & `roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/tal.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/ultralytics/yolo/utils/torch_utils.py` & `roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/ultralytics/yolo/utils/tuner.py` & `roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/tuner.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/ultralytics/yolo/v8/classify/predict.py` & `roof_mask_Yv8-0.5.8/ultralytics/yolo/v8/classify/predict.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/ultralytics/yolo/v8/classify/train.py` & `roof_mask_Yv8-0.5.8/ultralytics/yolo/v8/classify/train.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/ultralytics/yolo/v8/classify/val.py` & `roof_mask_Yv8-0.5.8/ultralytics/yolo/v8/classify/val.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/ultralytics/yolo/v8/detect/predict.py` & `roof_mask_Yv8-0.5.8/ultralytics/yolo/v8/detect/predict.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/ultralytics/yolo/v8/detect/train.py` & `roof_mask_Yv8-0.5.8/ultralytics/yolo/v8/detect/train.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/ultralytics/yolo/v8/detect/val.py` & `roof_mask_Yv8-0.5.8/ultralytics/yolo/v8/detect/val.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/ultralytics/yolo/v8/pose/predict.py` & `roof_mask_Yv8-0.5.8/ultralytics/yolo/v8/pose/predict.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/ultralytics/yolo/v8/pose/train.py` & `roof_mask_Yv8-0.5.8/ultralytics/yolo/v8/pose/train.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/ultralytics/yolo/v8/pose/val.py` & `roof_mask_Yv8-0.5.8/ultralytics/yolo/v8/pose/val.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/ultralytics/yolo/v8/segment/predict.py` & `roof_mask_Yv8-0.5.8/ultralytics/yolo/v8/segment/predict.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/ultralytics/yolo/v8/segment/train.py` & `roof_mask_Yv8-0.5.8/ultralytics/yolo/v8/segment/train.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/ultralytics/yolo/v8/segment/val.py` & `roof_mask_Yv8-0.5.8/ultralytics/yolo/v8/segment/val.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/yolo_roof/detect_functions.py` & `roof_mask_Yv8-0.5.8/yolo_roof/detect_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -281,15 +281,15 @@
                 #         image_path, total_instances, time.time() - start_time
                 #     )
                 # )
 
                 for each_class_id in set(all_labels):
                     each_class_masks = [each_mask for each_mask, each_label in zip(all_masks, all_labels) if each_label == each_class_id and each_mask.is_valid]
                     union_masks = unary_union(each_class_masks)
-                    label_names = metadata.get("thing_classes", None)
+                    # label_names = metadata.get("thing_classes", None)
                     # print(union_masks.geom_type)
                     if union_masks.geom_type == 'MultiPolygon':
                         for current_mask in union_masks.geoms:
                             shapely_bounding_box = current_mask.bounds
                             coco_box_format = np.array(
                                 [int(shapely_bounding_box[0]),
                                  int(shapely_bounding_box[1]),
@@ -376,74 +376,99 @@
                                 all_masks.append(Polygon(list1))
                                 all_scores.append(scores[idx])
                                 all_labels.append(int(classes[idx]))
                     
                 for each_class_id in set(all_labels):
                     each_class_masks = [each_mask for each_mask, each_label in zip(all_masks, all_labels) if each_label == each_class_id and each_mask.is_valid]
                     union_masks = unary_union(each_class_masks)
-                    label_names = metadata.get("thing_classes", None)
-                    # print(type(union_masks))
-                    if union_masks.geom_type == 'MultiPolygon':
-                        for current_mask in union_masks.geoms:
-                            if current_mask.area < 100:
-                                continue
-                            
-                            shapely_bounding_box = current_mask.bounds
-                            coco_box_format = np.array(
-                                [int(shapely_bounding_box[0]),
-                                 int(shapely_bounding_box[1]),
-                                 int(shapely_bounding_box[2]-shapely_bounding_box[0]),
-                                 int(shapely_bounding_box[3]-shapely_bounding_box[1])]
-                            ).tolist()
-                        
-                            current_polygon_list = current_mask.exterior.coords
-                            current_polygon_list_xy = current_mask.exterior.coords.xy
-
-                            coco_segmentation_format = np.array(current_mask.exterior.coords).reshape(1, len(current_mask.exterior.coords) * 2).tolist()
-                            # append annotation to coco jason file list
-                            new_annotations.append({"id": ann_id,
-                                                    "image_id": new_image_id,
-                                                    "category_id": each_class_id,
-                                                    "iscrowd": 0,
-                                                    # "area": current_mask.area,
-                                                    "bbox": coco_box_format,
-                                                    "segmentation": coco_segmentation_format
-                                                    })
-                            # get new annotation id
-                            ann_id += 1
-                    elif union_masks.geom_type == 'Polygon':
+                    
+                    # if union is single polygon just weighted the score by areas
+                    if union_masks.geom_type == 'Polygon':
                         if union_masks.area < 100:
                             continue
-                            
+                        
+                        union_scores = []
+                        union_areas = []
+                        for each_mask, each_score, each_label in zip(all_masks, all_scores, all_labels):
+                            if each_label == each_class_id and each_mask.is_valid:
+                                union_scores.append(each_score)
+                                union_areas.append(each_mask.area)
+                        
+                        area_np = np.array(union_areas)
+                        tmp_score = area_np[:, np.newaxis] * np.array(union_scores)
+                        coco_score = tmp_score.sum(axis=0)/tmp_score.sum()
+
                         shapely_bounding_box = union_masks.bounds
                         coco_box_format = np.array(
                             [int(shapely_bounding_box[0]),
                              int(shapely_bounding_box[1]),
                              int(shapely_bounding_box[2]-shapely_bounding_box[0]),
                              int(shapely_bounding_box[3]-shapely_bounding_box[1])]
                         ).tolist()
-                        
+
                         current_polygon_list = union_masks.exterior.coords
                         current_polygon_list_xy = union_masks.exterior.coords.xy
 
                         coco_segmentation_format = np.array(current_polygon_list).reshape(1, len(union_masks.exterior.coords) * 2).tolist()
                         # append annotation to coco jason file list
                         new_annotations.append({"id": ann_id,
                                                 "image_id": new_image_id,
                                                 "category_id": each_class_id,
                                                 "iscrowd": 0,
-                                                # "area": union_masks.area,
+                                                "area": union_masks.area,
                                                 "bbox": coco_box_format,
+                                                "scores": coco_score.tolist(),
                                                 "segmentation": coco_segmentation_format
                                                 })
                         # get new annotation id
                         ann_id += 1
+                    elif union_masks.geom_type == 'MultiPolygon':
+                        for current_mask in union_masks.geoms:
+                            if current_mask.area < 100:
+                                continue
+                
+                            union_scores = []
+                            union_areas = []
+                            for each_mask, each_score, each_label in zip(all_masks, all_scores, all_labels):
+                                if each_label == each_class_id and each_mask.is_valid:
+                                    if each_mask.intersects(current_mask):
+                                        union_scores.append(each_score)
+                                        union_areas.append(each_mask.area)
+ 
+                            area_np = np.array(union_areas)
+                            tmp_score = area_np[:, np.newaxis] * np.array(union_scores)
+                            coco_score = tmp_score.sum(axis=0)/tmp_score.sum()
+
+                            shapely_bounding_box = current_mask.bounds
+                            coco_box_format = np.array(
+                                [int(shapely_bounding_box[0]),
+                                 int(shapely_bounding_box[1]),
+                                 int(shapely_bounding_box[2]-shapely_bounding_box[0]),
+                                 int(shapely_bounding_box[3]-shapely_bounding_box[1])]
+                            ).tolist()
+
+                            current_polygon_list = current_mask.exterior.coords
+                            current_polygon_list_xy = current_mask.exterior.coords.xy
+
+                            coco_segmentation_format = np.array(current_polygon_list).reshape(1, len(current_mask.exterior.coords) * 2).tolist()
+                            # append annotation to coco jason file list
+                            new_annotations.append({"id": ann_id,
+                                                    "image_id": new_image_id,
+                                                    "category_id": each_class_id,
+                                                    "iscrowd": 0,
+                                                    "area": current_mask.area,
+                                                    "bbox": coco_box_format,
+                                                    "scores": coco_score.tolist(),
+                                                    "segmentation": coco_segmentation_format
+                                                    })
+                            # get new annotation id
+                            ann_id += 1
                     else:
-                        continue
-                        
+                        continue   
+
                 # save output image
                 
                 ################################## no output image
                 if save_image:
                     cv2.imwrite(out_filename,im0) 
                     cv2.imwrite(out_filename2,im0) 
                 ################################## no output image
@@ -637,10 +662,12 @@
             logging.info('%s already registered!' % datasetName)
 
     ############################################# Models
     # last_roof_boundary_result = mask_prediction(yolo_roof_condition_model, input_files, trainingDataset='Roof_condition', output_folder=demoFolder, thresh_hold=0.244, cut_image = False, tile_len = 960, tile_overlap = 200,save_image=False)
     
     # last_roof_boundary_result = mask_prediction(yolo_roof_condition_model, input_files, trainingDataset='Roof_condition_three_classes', output_folder=demoFolder, thresh_hold=0.245, cut_image = False, tile_len = 960, tile_overlap = 200, save_image=False)
     
-    last_roof_condition_result = mask_prediction(yolo_roof_condition_model, input_files, trainingDataset='Roof_condition_three_classes', output_folder=demoFolder, thresh_hold=0.236, cut_image = False, tile_len = 1280, tile_overlap = 200, save_image=True)
+    # last_roof_condition_result = mask_prediction(yolo_roof_condition_model, input_files, trainingDataset='Roof_condition_three_classes', output_folder=demoFolder, thresh_hold=0.236, cut_image = False, tile_len = 1280, tile_overlap = 200, save_image=True)
+
+    last_roof_condition_result = mask_prediction(yolo_roof_condition_model, input_files, trainingDataset='Roof_condition_three_classes', output_folder=demoFolder, thresh_hold=0.15, cut_image = False, tile_len = 1280, tile_overlap = 200, save_image=True)
```

### Comparing `roof_mask_Yv8-0.5.7/yolo_roof/geo_functions.py` & `roof_mask_Yv8-0.5.8/yolo_roof/geo_functions.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.7/yolo_roof/report_functions.py` & `roof_mask_Yv8-0.5.8/yolo_roof/report_functions.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from pycocotools.coco import COCO
 from tqdm import tqdm
 import json 
 import uuid
 import pandas as pd
 import math
 import cv2
+import re
 
 ### report ###
 import reportlab
 from reportlab.pdfgen import canvas
 from reportlab.pdfbase.ttfonts import TTFont
 from reportlab.pdfbase import pdfmetrics
 from reportlab.lib import colors
@@ -27,15 +28,14 @@
 from detectron2.engine.defaults import DefaultPredictor
 from detectron2.data import MetadataCatalog
 
 #### shapely ###
 import shapely
 import shapely.wkt
 from shapely.geometry import Polygon, MultiPoint
-from shapely.geometry import Polygon
 
 ## PDF
 import reportlab
 from reportlab.pdfgen import canvas
 from reportlab.pdfbase.ttfonts import TTFont
 from reportlab.pdfbase import pdfmetrics
 from reportlab.lib import colors
@@ -142,16 +142,14 @@
                  "images": new_images,
                  "annotations": new_annotations
                  }
 
     with open(new_json_file, "w") as jsonfile:
         json.dump(json_data, jsonfile, sort_keys=True, indent=4)
 
-
-
 def generate_referral_damage_json(demoFolder, coco_json, roof_boundary_json, new_cat, new_json_file_name):
     catIds = coco_json.getCatIds(catNms=[], supNms=[], catIds=[])
     # Obtain the category names
     categories = coco_json.loadCats(catIds)
     new_categories = [x['name'] for x in categories if x['name'] in new_cat]
     new_catIds = coco_json.getCatIds(catNms=new_categories, supNms=[], catIds=[])
     # print(new_catIds)
@@ -253,26 +251,150 @@
                  "images": new_images,
                  "annotations": new_annotations
                  }
 
     with open(new_json_file, "w") as jsonfile:
         json.dump(json_data, jsonfile, sort_keys=True, indent=4)
 
+        
+def generate_multi_model_referral_roof_boundary_based_json(demoFolder, coco_jsons, roof_boundary_json, new_cats, new_json_file_name):
+    # new json file name
+    new_json_file = os.path.join(demoFolder, new_json_file_name)
+    new_images = []
+    new_annotations = []
+    ann_id = 1
+    new_image_id = 1
+    new_catIds = []
+    category_names = []
+    new_categories =[]
+    
+    total_images = len(coco_jsons[0].getImgIds())
+    for i, new_cat in enumerate(new_cats):
+        new_categories.append({'id': i, 'name': f'{new_cats[i]}'})
+    
+    for coco_json in coco_jsons:
+        catIds = coco_json.getCatIds(catNms=[], supNms=[], catIds=[])
+        # Obtain the category names
+        categories = coco_json.loadCats(catIds)
+        category_names.append(categories)
+        new_category_names = [x['name'] for x in categories if x['name'] in new_cats]
+        new_catIds.append(coco_json.getCatIds(catNms=new_category_names, supNms=[], catIds=[]))
+    
+    for img_id in range(total_images):
+        for i, coco_json in enumerate(coco_jsons):
+            imgIds = coco_json.getImgIds()
+            # get image information
+            coco_img_info = coco_json.loadImgs(imgIds[img_id])[0]
+            # get the raw image annotations Id
+            annIds = coco_json.getAnnIds(imgIds=coco_img_info['id'])
+            # get annotations from annotation Id
+            annotations = coco_json.loadAnns(annIds)
+
+            roof_poly = Polygon()
+            # get image information
+            coco_img_info = roof_boundary_json.loadImgs(imgIds[img_id])[0]
+            # get the raw image annotations Id
+            annIds = roof_boundary_json.getAnnIds(imgIds=coco_img_info['id'])
+            # get annotations from annotation Id
+            roof_annotations = roof_boundary_json.loadAnns(annIds)
+            for ann in roof_annotations:
+                for seg in ann['segmentation']:
+                    mask = np.array(seg).reshape(len(seg) // 2, 2)
+                    poly = Polygon(mask)
+                    roof_poly = roof_poly.union(poly)
+
+            roof_poly = roof_poly.buffer(5.0)
+
+            ann_start = ann_id
+            for ann in annotations:
+                # print(ann)
+                # class selection
+                if ann['category_id'] in new_catIds[i]:
+                    # get the class name
+                    cat_name = coco_json.loadCats(ann['category_id'])[0]['name']
+                    # get new class id
+                    category_id = new_cats.index(cat_name)
+                    current_poly = Polygon()
+                    for seg in ann['segmentation']:
+                        mask = np.array(seg).reshape(len(seg) // 2, 2)
+                        new_poly = Polygon(mask)
+                        current_poly = current_poly.union(new_poly)
 
+                    if not current_poly.intersects(roof_poly):
+                        continue
+                    else:
+                        intersection_poly = current_poly.intersection(roof_poly)
+
+                    if intersection_poly.geom_type == 'MultiPolygon':
+                        for current_mask in intersection_poly.geoms:
+                            if current_mask.area < 25:
+                                continue
+                            current_polygon_list = current_mask.exterior.coords
+                            coco_segmentation_format = np.array(current_polygon_list).reshape(1, len(current_mask.exterior.coords) * 2).tolist()
+                            # append annotation to coco jason file list
+                            new_annotations.append({"id": ann_id,
+                                                    "image_id": new_image_id,
+                                                    "category_id": category_id,
+                                                    "iscrowd": 0,
+                                                    # "area": ann['area'],
+                                                    "bbox": ann['bbox'],
+                                                    "segmentation": coco_segmentation_format
+                                                    })
+                            # get new annotation id
+                            ann_id += 1
+                    elif intersection_poly.geom_type == 'Polygon':
+                        if intersection_poly.area < 25:
+                            continue
+                        current_polygon_list = intersection_poly.exterior.coords
+                        coco_segmentation_format = np.array(current_polygon_list).reshape(1, len(current_polygon_list) * 2).tolist()
+                        # append annotation to coco jason file list
+                        new_annotations.append({"id": ann_id,
+                                                "image_id": new_image_id,
+                                                "category_id": category_id,
+                                                "iscrowd": 0,
+                                                # "area": ann['area'],
+                                                "bbox": ann['bbox'],
+                                                "segmentation": coco_segmentation_format
+                                                })
+                        # get new annotation id
+                        ann_id += 1             
+
+        # get new image id
+        new_image_id += 1
+        # append image information to coco jason file list
+        new_images.append(coco_img_info)
+
+    info = {"year": 2022,
+            "version": "1.0",
+            "description": "Phase 2 data and coco json file",
+            "contributor": "Ruixu Liu, Delin Shen, Aaron Lee and Qiang Wang",
+            }
+
+    json_data = {"info": info,
+                 "categories": new_categories,
+                 "images": new_images,
+                 "annotations": new_annotations
+                 }
+
+    with open(new_json_file, "w") as jsonfile:
+        json.dump(json_data, jsonfile, sort_keys=True, indent=4)
+
+        
 class ReferralPoints:
     '''
     Read in referral rules and generate the csv format:
     Address    Total points    each referral elemten
       aaa          3              3  
     '''
 
     def __init__(self, referral_file, index):
         with open(referral_file) as f1:
             self.ref_json = json.load(f1)
         self.score = {'Address': index}
+        self.score.update(dict(('number of ' + score_cat, 0) for score_cat in self.ref_json))
         self.score.update({'Total points': 0})
         self.score.update(dict((score_cat, 0) for score_cat in self.ref_json))
         self.score.update({'Roof area (pixels)': 0})
 
         self.score_cat = [x for x in self.ref_json]
 
         self.buffer = dict((score_cat,{'area_percentage': 0, 'count': 0}) for score_cat in self.ref_json)
@@ -337,14 +459,15 @@
                     # class_label = labels[ann['category_id']]
                     # print(f'{class_label} poly_area {poly_area}')
 
                 if not self.current_poly.intersects(self.roof_poly):
                     continue
                 # if this instance is detected 'count' + 1
                 self.buffer[labels[ann['category_id']]]['count'] += 1
+                self.score['number of '+ labels[ann['category_id']]] +=1
                     
         # for each cat
         for referral_cat in self.score_cat:
             # for each value section
             for referral_value in self.ref_json[referral_cat]:
                 # for each referral type
                 for refferal_type in self.buffer[referral_cat]:
@@ -357,17 +480,16 @@
                             if referral_value['min'] <= self.buffer[referral_cat][refferal_type] < referral_value['max']:
                                 if referral_value['point'] > self.score[referral_cat]:
                                     self.set_points(referral_cat, points=referral_value['point'])
                 # print(referral_cat)
                 # print(self.buffer[referral_cat])  
 
                 
-                
 def generate_displayed_polygones(image_folder,json_file,trainingDataset):
-    allColors = [(255,0,0), (0,255,0), (0,0,255), (255,255,0), (255,0,255), (0,255,255), (75,125,255), (125,75,255), (75,255,125), (125,255,75), (255,125,75), (255,75,125)]*8
+    allColors = [(0,0,255), (255,0,0), (125,75,255), (255,255,0), (255,0,255), (0,255,255), (75,125,255), (125,75,255), (75,255,125), (125,255,75), (255,125,75), (255,75,125)]*8
     filename = str(uuid.uuid4())
     register_coco_instances(filename, {'thing_colors':allColors}, json_file, image_folder)
     metadata = MetadataCatalog.get(filename)
     dicts = DatasetCatalog.get(filename)
     model_folder = os.path.join(image_folder,'prediction_' + trainingDataset)
     print(f"Generating {trainingDataset} polygons")
     for dic in dicts:
@@ -379,62 +501,87 @@
         out_filename2_extention = os.path.splitext(os.path.basename(dic["file_name"]))[1]
         out_filename2 = os.path.basename(dic["file_name"]).replace(out_filename2_extention,'_merged'+out_filename2_extention)
         vis.save(os.path.join(image_folder,out_filename))
         # vis.save(os.path.join(model_folder,out_filename2)) # model folder is not necessary
     print("Gereating Finished.")
     return vis
 
-def generate_displayed_condition_polygones(image_folder,json_file,trainingDataset):
-    allColors = [(255,0,0), (0,255,0), (0,0,255), (255,255,0), (255,0,255), (0,255,255), (75,125,255), (125,75,255), (75,255,125), (125,255,75), (255,125,75), (255,75,125)]*8
-    filename = str(uuid.uuid4())
-    register_coco_instances(filename, {'thing_colors':allColors}, json_file, image_folder)
-    metadata = MetadataCatalog.get(filename)
-    dicts = DatasetCatalog.get(filename)
-    model_folder = os.path.join(image_folder,'prediction_' + trainingDataset)
-    print(f"Generating {trainingDataset} polygons")
-    for dic in dicts:
-        img = utils.read_image(dic["file_name"], "RGB")
-        visualizer = Vis_box(img, metadata=metadata, scale=0.3, instance_mode=ColorMode.SEGMENTATION)
-        vis = visualizer.draw_dataset_dict(dic)
-        out_filename = os.path.join(os.path.splitext(os.path.basename(dic["file_name"]))[0],trainingDataset +'_merged.jpg')
-        vis.save(os.path.join(image_folder,out_filename))
 
-    print("Gereating Finished.")
-    return vis
+def generate_displayed_condition_polygones_and_colors(image_folder,json_file,trainingDataset):
+    coco_json = COCO(json_file)
+    imgIds = coco_json.getImgIds()
+
+    print(f"Merging {trainingDataset} polygons")
+    for img_id in range(len(imgIds)):
+        # get image information
+        coco_img_info = coco_json.loadImgs(imgIds[img_id])[0]
+        # get the raw image annotations Id
+        annIds = coco_json.getAnnIds(imgIds=coco_img_info['id'])
+        # get annotations from annotation Id
+        annotations = coco_json.loadAnns(annIds)
+
+        img = cv2.imread(os.path.join(image_folder,coco_img_info['file_name']))
+
+        for i, ann in enumerate(annotations):
+            bbox = ann['bbox']
+            score = int(ann['scores'])
+
+            if score < 40:
+                condition_color = (0,0,255) # red
+            elif score >70:
+                condition_color = (0,255,0) # green
+            else:
+                condition_color = (0,255,255) # yellow
+
+            img = cv2.putText(img, str(i+1), (int(bbox[0]+5),int(bbox[1]+30)), fontFace=cv2.FONT_HERSHEY_SIMPLEX, 
+                       fontScale=1, color=condition_color, thickness=2, lineType=cv2.LINE_AA)
+            img = cv2.rectangle(img, (int(bbox[0]),int(bbox[1])), (int(bbox[0] + bbox[2]),int(bbox[1] + bbox[3])), color=condition_color, thickness=3)
+        
+        out_filename = os.path.join(os.path.splitext(coco_img_info["file_name"])[0], trainingDataset +'_merged.jpg')
+        cv2.imwrite(os.path.join(image_folder,out_filename),img)
+
+    print("Merging Finished.")
+    return img
+
 
 def generate_referral_condition_json(demoFolder, coco_json, new_json_file_name):
     catIds = coco_json.getCatIds(catNms=[], supNms=[], catIds=[])
     categories = coco_json.loadCats(catIds)    
     imgIds = coco_json.getImgIds()
     new_json_file = os.path.join(demoFolder, new_json_file_name)
     new_images = []
     new_annotations = []
     ann_id = 1
     new_image_id = 1
-
+    
+    ###
+    weights = np.array([0, 50, 100])
+    ###
+    
     for img_id in range(len(imgIds)):
         # get image information
         coco_img_info = coco_json.loadImgs(imgIds[img_id])[0]
         # get the raw image annotations Id
         annIds = coco_json.getAnnIds(imgIds=coco_img_info['id'])
         # get annotations from annotation Id
         annotations = coco_json.loadAnns(annIds)
 
         ann_start = ann_id
         for ann in annotations:
-            # print(ann)
-            # # class selection
-            # if ann['category_id'] in new_catIds:
-                
+            if ann['area'] < 100*100:
+                continue
+            score = np.array(ann['scores'])
+            new_score = weights.dot(score/score.sum())
             # append annotation to coco jason file list
             new_annotations.append({"id": ann_id,
                                     "image_id": new_image_id,
                                     "category_id": ann['category_id'],
                                     "iscrowd": 0,
-                                    # "area": ann['area'],
+                                    "area": ann['area'],
+                                    "scores": new_score,
                                     "bbox": ann['bbox'],
                                     # "segmentation": ann['segmentation']
                                     })
             # get new annotation id
             ann_id += 1
 
         # get new image id
@@ -452,60 +599,84 @@
                  "categories": categories,
                  "images": new_images,
                  "annotations": new_annotations
                  }
 
     with open(new_json_file, "w") as jsonfile:
         json.dump(json_data, jsonfile, sort_keys=True, indent=4)
-
-    
+  
     
 def generate_condition_model(file_root_path, demoFolder = 'roof_score_new_20230101'):
     pred_condition_file = os.path.join(demoFolder,'prediction_Roof_condition_three_classes/Roof_condition_three_classes_all_in_one.json')
-    red_condition = COCO(pred_condition_file)
-    generate_referral_condition_json(demoFolder, red_condition,'Referral_condition.json')
-    vis_out = generate_displayed_condition_polygones(demoFolder,os.path.join(demoFolder, 'Referral_condition.json'),'Roof_condition_three_classes')
+    pred_condition = COCO(pred_condition_file)
+    generate_referral_condition_json(demoFolder, pred_condition,'Referral_condition.json')
+    vis_out = generate_displayed_condition_polygones_and_colors(demoFolder,os.path.join(demoFolder, 'Referral_condition.json'),'Roof_condition_three_classes')
     
     referral_condition = COCO(os.path.join(demoFolder, 'Referral_condition.json'))
+    all_condition_score = []
     for referral_condition_id in referral_condition.getImgIds():
         coco_img_info = referral_condition.loadImgs(referral_condition_id)[0]
         address = os.path.splitext(coco_img_info['file_name'])[0]
-        print(address)
+        condition_dict = {'Address': address}
+        condition_dict.update({'main_condition': 0})
+        # get the image annotations ids
+        annIds = referral_condition.getAnnIds(imgIds=referral_condition_id)
+        # get annotations from annotation ids
+        annotations = referral_condition.loadAnns(annIds)
+        condition_text = ''
+        area = []
+        score = []
+        max_area = 0
+        for ann in annotations:
+            # add new area condition score
+            condition_text+=str(ann['area']) + ':' + str(int(ann['scores'])) + ','
+            # update the major area condition
+            if ann['area'] > max_area:
+                condition_dict['main_condition'] = int(ann['scores'])
+                max_area = ann['area']
+            # update the weight condition
+            area.append(ann['area'])
+            score.append(ann['scores'])
+        condition_dict.update({'Over_all_condition': np.array(area).dot(np.array(score))/sum(area)})
+        condition_dict.update({'condition_details': condition_text})
+        all_condition_score.append(condition_dict)
+        df = pd.DataFrame.from_dict([condition_dict])
+        df.to_csv(os.path.join(demoFolder,address+'/condition_referral.csv'), index=False, header=True)
+    df = pd.DataFrame.from_dict(all_condition_score)
+    df.to_csv(os.path.join(demoFolder,'all_condition.csv'), index=False, header=True)
 
-def generate_condition_and_merged_model(file_root_path, demoFolder = 'roof_score_new_20230101'):
-    # pred_damage_file = os.path.join(demoFolder,'prediction_Roof_damage/Roof_damage_all_in_one.json')
-    # pred_equip_file = os.path.join(demoFolder, 'prediction_Roof_equipment/Roof_equipment_all_in_one.json')
+def generate_merged_model_damage_equip_pdf(file_root_path, demoFolder = 'roof_score_new_20230101'):
     pred_phase3_file = os.path.join(demoFolder,'prediction_Phase3_equipment_damage/Phase3_equipment_damage_all_in_one.json')
     pred_data_all_file = os.path.join(demoFolder, 'prediction_Data_all_equipment_damage/Data_all_equipment_damage_all_in_one.json')
     pred_boundary_file =os.path.join(demoFolder, 'prediction_Roof_boundary/Roof_boundary_all_in_one.json')
-
-    # read in referral rules and create corresponding functions
-    referral_label_file = os.path.join(file_root_path,'referral_labels_20230315.json')
-
-    with open(referral_label_file) as f1:
-        ref_json = json.load(f1)
-    cat_damage = [x for x in ref_json]
-
+    # Load prediction file as COCO formate
     pred_phase3 = COCO(pred_phase3_file)
     pred_data_all = COCO(pred_data_all_file)
     pred_boundary = COCO(pred_boundary_file)
-    generate_referral_damage_json(demoFolder, pred_data_all,pred_boundary,cat_damage,'Referral_data_all.json')
-    # generate_referral_json(demoFolder, pred_data_all,cat_damage,'Referral_data_all.json')
-    with open(referral_label_file) as f1:
+    # read in referral rules and create corresponding functions
+    referral_label_file = os.path.join(file_root_path,'referral_labels_20230315.json')
+    referral_damage_label_file = os.path.join(file_root_path,'referral_labels_20230421_for_merged_damage.json')
+    referral_equip_label_file = os.path.join(file_root_path,'referral_labels_20230421_for_merged_equip.json')
+    
+    with open(referral_damage_label_file) as f1:
+        ref_json = json.load(f1)
+        cat_damage = [x for x in ref_json]
+    generate_multi_model_referral_roof_boundary_based_json(demoFolder, [pred_data_all, pred_phase3], pred_boundary,cat_damage,'Referral_damage_all.json')
+    
+    with open(referral_equip_label_file) as f1:
         ref_json = json.load(f1)
-    cat_equip = [x for x in ref_json]
+        cat_equip = [x for x in ref_json]
+    generate_multi_model_referral_roof_boundary_based_json(demoFolder, [pred_data_all, pred_phase3], pred_boundary, cat_equip,'Referral_equipment_all.json')
 
-    generate_referral_damage_json(demoFolder, pred_phase3, pred_boundary, cat_equip,'Referral_phase3.json')
-    # generate_referral_json(demoFolder, pred_phase3, cat_equip,'Referral_phase3.json')
-    vis_out = generate_displayed_polygones(demoFolder,os.path.join(demoFolder, 'Referral_data_all.json'),'Data_all_equipment_damage')
-    vis_out = generate_displayed_polygones(demoFolder,os.path.join(demoFolder, 'Referral_phase3.json'),'Phase3_equipment_damage')
+    vis_out = generate_displayed_polygones(demoFolder,os.path.join(demoFolder, 'Referral_damage_all.json'),'Damage')
+    vis_out = generate_displayed_polygones(demoFolder,os.path.join(demoFolder, 'Referral_equipment_all.json'),'Equipment')
 
     ################################### Referral
-    referral_damage = COCO(os.path.join(demoFolder, 'Referral_data_all.json'))
-    referral_equip = COCO(os.path.join(demoFolder, 'Referral_phase3.json'))
+    referral_damage = COCO(os.path.join(demoFolder, 'Referral_damage_all.json'))
+    referral_equip = COCO(os.path.join(demoFolder, 'Referral_equipment_all.json'))
     referral_output = []
     # Obtain the category ID numbers
     catIds = referral_damage.getCatIds()
     # Obtain the category names
     categories = referral_damage.loadCats(catIds)
     # Id2catname
     Damage_labels = [value['name'] for value in categories]
@@ -519,69 +690,67 @@
 
     for damage_img_id, equp_image_id in zip(referral_damage.getImgIds(), referral_equip.getImgIds()):
         assert referral_damage.loadImgs(damage_img_id) == referral_equip.loadImgs(equp_image_id)
         # get image information
         coco_img_info = referral_damage.loadImgs(damage_img_id)[0]
         address = os.path.splitext(coco_img_info['file_name'])[0]
         print(address)
-        # zoom_level = int(address[-13:-11])
 
-        # using :-14 to only keep address no zoom level and date
-        # new_referral = ReferralPoints(referral_label_file, index=address[:-14])
         new_referral = ReferralPoints(referral_label_file, index=address) 
 
         # Roof Boundary
-        # new_referral.buffer['Roof boundary'] = np.sqrt(coco_img_info['height'] * coco_img_info['width'])
-        # new_referral.buffer['Roof_boundary'] = 0.5* coco_img_info['height'] * coco_img_info['width']
-        # print(coco_img_info['height'] * coco_img_info['width'])
         new_referral.obtation_roof_boundary(pred_boundary, image_id = coco_img_info['id'])
 
-
         # Damage
         #################################################
         new_referral.update_buffer_value(referral_damage, Damage_labels, image_id = coco_img_info['id'] )
-        # if zoom_level==22:
-        #     print(new_referral.buffer['Roof_boundary']*0.0002)
-        #     print(new_referral.buffer['Water pooling']['area_percentage']*new_referral.buffer['Roof_boundary']*0.0002)
-        # else:
-        #     print(new_referral.buffer['Roof_boundary']*0.00085)
-        #     print(new_referral.buffer['Water pooling']['area_percentage']*new_referral.buffer['Roof_boundary']*0.00085)
 
         # Equipment
         #################################################
         new_referral.update_buffer_value(referral_equip, Equipment_labels, image_id = coco_img_info['id'])
 
+        # update total points
         new_referral.update_total_points()
         referral_output.append(new_referral.score)
         df = pd.DataFrame.from_dict([new_referral.score])
         df.to_csv(os.path.join(demoFolder,address+'/referral.csv'), index=False, header=True)
 
     df = pd.DataFrame.from_dict(referral_output)
     df.to_csv(os.path.join(demoFolder,'all_referral.csv'), index=False, header=True)
     image_csv = pd.read_csv(os.path.join(demoFolder,"image.csv"))
     referral_csv = pd.read_csv(os.path.join(demoFolder,"all_referral.csv"))
+    condition_csv = pd.read_csv(os.path.join(demoFolder,"all_condition.csv"))
 
-    image_csv.merge(referral_csv,how='outer',on='Address').to_csv(os.path.join(demoFolder, 'all_address.csv'), index=False, header=True)
-
+    image_csv.merge(condition_csv,how='outer',on='Address').to_csv(os.path.join(demoFolder, 'all_address.csv'), index=False, header=True)
+    all_address_csv =  pd.read_csv(os.path.join(demoFolder,"all_address.csv"))
+    all_address_csv.merge(referral_csv,how='outer',on='Address').to_csv(os.path.join(demoFolder, 'all_address.csv'), index=False, header=True)
+    
     ################################################################# PDF
     image_csv = pd.read_csv(os.path.join(demoFolder,'image.csv'))
     referral_csv = pd.read_csv(os.path.join(demoFolder,'all_referral.csv'))
     all_address_csv = pd.read_csv(os.path.join(demoFolder, 'all_address.csv'))
     # Today_date = datetime.today().strftime('%Y-%m-%d')
     # # print(Today_date)
     full_address = all_address_csv["Address"].tolist()
     insured_name = all_address_csv["InsuredName"].tolist()
     image_date = all_address_csv["Image date"].tolist()
     image_info = all_address_csv["Image info"].tolist()
     zoom_level = all_address_csv["Image level"].tolist()
+    main_roof_condition_score = all_address_csv["main_condition"].tolist()
+    overall_roof_condition_score = all_address_csv["Over_all_condition"].tolist()
+    all_roof_condition_score = all_address_csv["condition_details"].tolist()
 
     key_name = all_address_csv.columns
+    HVAC_index = all_address_csv.columns.get_loc('number of HVAC/Cooling tower')
+    Tarp_index = all_address_csv.columns.get_loc('number of Tarp')
     key_name_index = all_address_csv.columns.get_loc('Total points')
     gsd_key = all_address_csv.columns.get_loc('Image gsd (meters/pixels)')
     pixels_area_key = all_address_csv.columns.get_loc('Roof area (pixels)')
+    
+    
     # print(key_name[key_name_index])
 
     for address_index in range(len(full_address)):
         address = full_address[address_index]
         row = all_address_csv.iloc[address_index]
         print(f'index:{address_index}, address:{address}')
         if np.isnan(row[key_name_index]):
@@ -595,16 +764,16 @@
         url = f'https://apps.nearmap.com/maps/#/@{url_lat},{url_lon},{url_zoom_level}z,0d/V/{url_date}'
 
         fileName = os.path.join(demoFolder,address+'.pdf')
         documentTitle = f'Refferal'
         title = f'{insured_name[address_index]}'
         subTitle = address
 
-        Damage_image_name = os.path.join(demoFolder,address+'/Data_all_equipment_damage_merged.jpg')
-        Equipment_image_name = os.path.join(demoFolder,address+'/Phase3_equipment_damage_merged.jpg')
+        Damage_image_name = os.path.join(demoFolder,address+'/Damage_merged.jpg')
+        Equipment_image_name = os.path.join(demoFolder,address+'/Equipment_merged.jpg')
         # Equipment_image_name = os.path.join(demoFolder,address+'/Roof_condition_three_classes_merged.jpg')
         Roof_condition_image_name = os.path.join(demoFolder,address+'/Roof_condition_three_classes_merged.jpg')
 
         pdf = canvas.Canvas(fileName)
         pdf.setTitle(documentTitle)
         pdf.setFont("Times-Roman", 14)
         pdf.drawCentredString(300, 800, title)
@@ -618,113 +787,105 @@
 
         # information
         text = pdf.beginText(40, 740)
         text.setFont("Courier", 12)
         text.setFillColor(colors.black)
         text.textLine(f'Image date: {image_date[address_index]}')
 
-        ######################################### 100 points
-        # Range	    3	   3	        3	          3	                 3	           1	       3
-        # weight	1	   2.5	        2.5	          1	                 1	           1	       1
-        # Other damage	Staining	Water pooling	Skylight	HVAC/Cooling tower	Pipeline	Solar panel
-
-
-        total_point = 0
-        if row[key_name_index]!=0:
-            for i in range(key_name_index+1, len(key_name)):
-                if key_name[i] == 'Other damage':
-                    total_point += row[i]*1
-                elif key_name[i] == 'Staining':
-                    total_point += row[i]*2.5
-                elif key_name[i] == 'Water pooling':
-                    total_point += row[i]*2.5
-                elif key_name[i] == 'Skylight':
-                    total_point += row[i]*1
-                elif key_name[i] == 'HVAC/Cooling tower':
-                    total_point += row[i]*1
-                elif key_name[i] == 'Pipeline':
-                    total_point += row[i]*1
-                elif key_name[i] == 'Solar panel':
-                    total_point += row[i]*1
-            total_point = 100 - total_point * 5
-            if total_point> 0 :
-                line= f'Total scores: {total_point}'
+        # line = f'Roof conditon score: {roof_condition_score[address_index]}'
+        line = 'Roof condition (roof number/score) : '
+        roof_socres = re.findall(r'\:(.*?)\,',all_roof_condition_score[address_index])
+        for i in range(len(roof_socres)):
+            if i%8==0:
                 text.textLine(line)
-                text.setFillColor(colors.blue)
-            else:
-                line = 'Total scores: 0'
-                text.textLine(line)
-                text.setFillColor(colors.blue)
-        else:
-            line = 'Total scores: 100'
-            text.textLine(line)
-            text.setFillColor(colors.blue)
+                line = ''
+            line+= f'#{i+1}/{roof_socres[i]}  '
+        
+        text.textLine(line)
+        total_point = 0
 
+############################### SB referral 2.1
+        total_score = overall_roof_condition_score[address_index]
+        if key_name[i] == 'Tarp' and row[i]>0:
+            if row[Tarp_index] == 1:
+                total_score/= 2
+            else:
+                total_score/= 4
+        tmp_point = 0
+        for i in range(key_name_index+1, len(key_name)):
+            if key_name[i] == 'HVAC/Cooling tower'and row[i]>0:
+                tmp_point += row[i]*1
+            elif key_name[i] == 'Pipeline'and row[i]>0:
+                tmp_point += row[i]*1
+            elif key_name[i] == 'Solar panel'and row[i]>0:
+                tmp_point += row[i]*1
+                
+        total_score = total_score * (7-tmp_point)/7
+        
+        line= f'Overall score (condition and equipment): {int(total_score)}'
+        text.textLine(line)
+        text.setFillColor(colors.blue)
+        #################################
         for i in range(key_name_index+1, len(key_name)):
             if i == pixels_area_key:
                 gsd_area = row[gsd_key] * row[gsd_key] * row[pixels_area_key]
-                text.textLine(f'Roof area: {int(gsd_area)} m\u00b2')
+                # text.textLine(f'Roof area: {int(gsd_area)} m\u00b2')
+                text.textLine(f'Roof area: {int(gsd_area * 10.764)} ft\u00b2')
                 continue
             if int(row[i]) == 0:
                 line = key_name[i] + ': ' + 'Not detected'
                 # text.textLine(line)     # Hide no detected case
             elif int(row[i]) == 1:
-                if key_name[i] == 'Pipline' or key_name[i] =='Solar panel': 
+                if key_name[i] == 'Pipeline' or key_name[i] =='Solar panel': 
                     line = key_name[i] + ': ' + 'Detected'
                     text.textLine(line)
                 if key_name[i] == 'Staining' or key_name[i] =='Water pooling' or key_name[i] =='Other damage':
                     line = key_name[i] + ': ' + 'Minor'
                     text.textLine(line)
-                if key_name[i] == 'Skylight' or key_name[i] =='HVAC/Cooling tower':
+                if key_name[i] == 'Skylight':
                     line = key_name[i] + ': ' + 'Minimal'
                     text.textLine(line)
+                if key_name[i] =='HVAC/Cooling tower':
+                    # line = key_name[i] + ': ' + 'Minimal'
+                    line = key_name[i] + ': ' + f'Minimal ({row[HVAC_index]})'
+                    text.textLine(line)
             elif int(row[i]) == 2:
-                if key_name[i] == 'Pipline' or key_name[i] =='Solar panel': 
+                if key_name[i] == 'Pipeline' or key_name[i] =='Solar panel': 
                     line = key_name[i] + ': ' + 'Detected'
                     text.textLine(line)
                 if key_name[i] == 'Staining' or key_name[i] =='Water pooling' or key_name[i] =='Other damage':
                     line = key_name[i] + ': ' + 'Moderate'
                     text.textLine(line)
-                if key_name[i] == 'Skylight' or key_name[i] =='HVAC/Cooling tower':
+                if key_name[i] == 'Skylight' :
                     line = key_name[i] + ': ' + 'A few'
                     text.textLine(line)
+                if key_name[i] =='HVAC/Cooling tower':
+                    # line = key_name[i] + ': ' + 'A few'
+                    line = key_name[i] + ': ' + f'A few ({row[HVAC_index]})'
             else:
-                if key_name[i] == 'Pipline' or key_name[i] =='Solar panel': 
+                if key_name[i] == 'Pipeline' or key_name[i] =='Solar panel': 
                     line = key_name[i] + ': ' + 'Detected'
                     text.textLine(line)
                 if key_name[i] == 'Staining' or key_name[i] =='Water pooling' or key_name[i] =='Other damage':
                     line = key_name[i] + ': ' + 'Major'
                     text.textLine(line)
-                if key_name[i] == 'Skylight' or key_name[i] =='HVAC/Cooling tower':
+                if key_name[i] == 'Skylight':
                     line = key_name[i] + ': ' + 'Many'
                     text.textLine(line)
+                if key_name[i] =='HVAC/Cooling tower':
+                    # line = key_name[i] + ': ' + 'Many'
+                    line = key_name[i] + ': ' + f'Many ({row[HVAC_index]})'
+                    text.textLine(line)
+                
 
         pdf.drawText(text)
-    ################################################## 19 points
-        # if row[key_name_index]!=0:
-        #     line= f'Total points: {int(row[key_name_index])}'
-        #     text.textLine(line)
-        # else:
-        #     line = 'Total points: 0'
-        #     text.textLine(line)
-        # for i in range(key_name_index+1, len(key_name)):
-        #     if row[i]>0:
-        #         line = key_name[i] + ': ' + str(int(row[i]))
-        #         text.textLine(line)
-        # pdf.drawText(text)
-    ##########################################################
-
-        # images
-        # textLines = ['Image',
-        #             'Attributes',
-        #             'Condition'
-        # ]
+
         textLines = ['Condition',
-                    'Attributes',
-                    'Rare damage'
+                    'Damage',
+                    'Equipment'
         ]
         image_name = address + '.jpg'
         image_full_name = os.path.join(demoFolder,image_name)
 
         image = cv2.imread(image_full_name)
         height = image.shape[0]
         width = image.shape[1]
@@ -801,15 +962,18 @@
             text.textLine(textLines[-1])
             pdf.drawText(text)
             pdf.drawInlineImage(Equipment_image_name, 310, 40, width = draw_width, height = draw_height)
             pdf.linkURL(url, (310, 40, 310+draw_width, 40+draw_height), relative=1)
 
 
         # saving the pdf
-        pdf.save()
+        pdf.save()    
+    
+    
+    
 
 def zipdir(folder, path, ziph):
     file_path = os.path.join(folder, path)
     # ziph is zipfile handle
     if not os.path.isdir(file_path):
         if path[-3:]=='jpg': # move the orignial image to image folder
             ziph.write(file_path,path.replace('.jpg','/Image.jpg'))
```

