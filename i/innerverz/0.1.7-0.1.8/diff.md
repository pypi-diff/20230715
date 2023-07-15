# Comparing `tmp/innerverz-0.1.7.tar.gz` & `tmp/innerverz-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "innerverz-0.1.7.tar", last modified: Wed Jul 12 10:07:39 2023, max compression
+gzip compressed data, was "innerverz-0.1.8.tar", last modified: Sat Jul 15 15:18:04 2023, max compression
```

## Comparing `innerverz-0.1.7.tar` & `innerverz-0.1.8.tar`

### file list

```diff
@@ -1,161 +1,161 @@
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-12 10:07:39.064154 innerverz-0.1.7/
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-12 10:07:39.030870 innerverz-0.1.7/Innerverz/
--rw-r--r--   0 jjy        (501) staff       (20)     1730 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/__init__.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-12 10:07:39.031149 innerverz-0.1.7/Innerverz/data_process/
--rw-r--r--   0 jjy        (501) staff       (20)       30 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/data_process/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     3488 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/data_process/main.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-12 10:07:39.032109 innerverz-0.1.7/Innerverz/deblurrer/
--rw-r--r--   0 jjy        (501) staff       (20)       27 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/deblurrer/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     2611 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/deblurrer/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     3609 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/deblurrer/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)      843 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/deblurrer/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-12 10:07:39.032883 innerverz-0.1.7/Innerverz/deca/
--rw-r--r--   0 jjy        (501) staff       (20)       23 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/deca/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)    24633 2023-07-12 10:01:18.000000 innerverz-0.1.7/Innerverz/deca/main.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-12 10:07:39.034973 innerverz-0.1.7/Innerverz/deca/models/
--rw-r--r--   0 jjy        (501) staff       (20)    12950 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/deca/models/FLAME.py
--rw-r--r--   0 jjy        (501) staff       (20)        0 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/deca/models/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     2464 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/deca/models/decoders.py
--rw-r--r--   0 jjy        (501) staff       (20)     1983 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/deca/models/detectors.py
--rw-r--r--   0 jjy        (501) staff       (20)     1427 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/deca/models/encoders.py
--rw-r--r--   0 jjy        (501) staff       (20)     1983 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/deca/models/face_detectors.py
--rw-r--r--   0 jjy        (501) staff       (20)    13786 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/deca/models/lbs.py
--rw-r--r--   0 jjy        (501) staff       (20)     8386 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/deca/models/resnet.py
--rw-r--r--   0 jjy        (501) staff       (20)     1200 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/deca/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-12 10:07:39.036152 innerverz-0.1.7/Innerverz/deca/utils/
--rw-r--r--   0 jjy        (501) staff       (20)        0 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/deca/utils/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     5036 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/deca/utils/cfg.py
--rw-r--r--   0 jjy        (501) staff       (20)    19673 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/deca/utils/lmks_756.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-12 10:07:39.036426 innerverz-0.1.7/Innerverz/deca/utils/rasterizer/
--rw-r--r--   0 jjy        (501) staff       (20)        0 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/deca/utils/rasterizer/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)      706 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/deca/utils/rasterizer/setup.py
--rw-r--r--   0 jjy        (501) staff       (20)    22281 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/deca/utils/renderer.py
--rw-r--r--   0 jjy        (501) staff       (20)    12710 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/deca/utils/rotation_converter.py
--rw-r--r--   0 jjy        (501) staff       (20)     5574 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/deca/utils/tensor_cropper.py
--rw-r--r--   0 jjy        (501) staff       (20)    11870 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/deca/utils/tracker_utils.py
--rw-r--r--   0 jjy        (501) staff       (20)    26664 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/deca/utils/util.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-12 10:07:39.037035 innerverz-0.1.7/Innerverz/deep3dmm/
--rw-r--r--   0 jjy        (501) staff       (20)       27 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/deep3dmm/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     3598 2023-07-12 10:01:35.000000 innerverz-0.1.7/Innerverz/deep3dmm/main.py
--rw-r--r--   0 jjy        (501) staff       (20)    25860 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/deep3dmm/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)      627 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/deep3dmm/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-12 10:07:39.037917 innerverz-0.1.7/Innerverz/face_alignment/
--rw-r--r--   0 jjy        (501) staff       (20)      125 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/face_alignment/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     6646 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/face_alignment/graphic_utils.py
--rw-r--r--   0 jjy        (501) staff       (20)     5089 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/face_alignment/landmark.py
--rw-r--r--   0 jjy        (501) staff       (20)     8059 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/face_alignment/main.py
--rw-r--r--   0 jjy        (501) staff       (20)    12774 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/face_alignment/retina_face.py
--rw-r--r--   0 jjy        (501) staff       (20)      640 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/face_alignment/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-12 10:07:39.038344 innerverz-0.1.7/Innerverz/face_alignment/utils/
--rw-r--r--   0 jjy        (501) staff       (20)       24 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/face_alignment/utils/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     3354 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/face_alignment/utils/face_align.py
--rw-r--r--   0 jjy        (501) staff       (20)     4933 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/face_alignment/utils/transform.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-12 10:07:39.038876 innerverz-0.1.7/Innerverz/face_color_transfer/
--rw-r--r--   0 jjy        (501) staff       (20)       22 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/face_color_transfer/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     5595 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/face_color_transfer/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     8503 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/face_color_transfer/nets.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-12 10:07:39.039619 innerverz-0.1.7/Innerverz/face_color_transfer/sub_nets/
--rw-r--r--   0 jjy        (501) staff       (20)      100 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/face_color_transfer/sub_nets/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     7018 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/face_color_transfer/sub_nets/blend_net.py
--rw-r--r--   0 jjy        (501) staff       (20)     3642 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/face_color_transfer/sub_nets/discriminator.py
--rw-r--r--   0 jjy        (501) staff       (20)     3788 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/face_color_transfer/sub_nets/vgg19_net.py
--rw-r--r--   0 jjy        (501) staff       (20)     9366 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/face_color_transfer/sub_nets/warp_net.py
--rw-r--r--   0 jjy        (501) staff       (20)     2015 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/face_color_transfer/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-12 10:07:39.040583 innerverz-0.1.7/Innerverz/face_enhancer/
--rw-r--r--   0 jjy        (501) staff       (20)       30 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/face_enhancer/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     3881 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/face_enhancer/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     4079 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/face_enhancer/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)      768 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/face_enhancer/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-12 10:07:39.041020 innerverz-0.1.7/Innerverz/face_matting/
--rw-r--r--   0 jjy        (501) staff       (20)       30 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/face_matting/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     8110 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/face_matting/main.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-12 10:07:39.041546 innerverz-0.1.7/Innerverz/face_matting/nets/
--rw-r--r--   0 jjy        (501) staff       (20)       68 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/face_matting/nets/__init__.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-12 10:07:39.041836 innerverz-0.1.7/Innerverz/face_matting/nets/decoders/
--rw-r--r--   0 jjy        (501) staff       (20)      219 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/face_matting/nets/decoders/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     8175 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/face_matting/nets/decoders/resnet_decoder.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-12 10:07:39.042166 innerverz-0.1.7/Innerverz/face_matting/nets/encoders/
--rw-r--r--   0 jjy        (501) staff       (20)    24822 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/face_matting/nets/encoders/MatteFormer.py
--rw-r--r--   0 jjy        (501) staff       (20)        0 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/face_matting/nets/encoders/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     4386 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/face_matting/nets/generators.py
--rw-r--r--   0 jjy        (501) staff       (20)     2650 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/face_matting/nets/ops.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-12 10:07:39.042412 innerverz-0.1.7/Innerverz/face_matting/nets/raft/
--rw-r--r--   0 jjy        (501) staff       (20)       20 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/face_matting/nets/raft/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     4009 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/face_matting/nets/raft/main.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-12 10:07:39.044651 innerverz-0.1.7/Innerverz/face_matting/nets/raft/utils/
--rw-r--r--   0 jjy        (501) staff       (20)       94 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/face_matting/nets/raft/utils/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     3079 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/face_matting/nets/raft/utils/corr.py
--rw-r--r--   0 jjy        (501) staff       (20)     8847 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/face_matting/nets/raft/utils/extractor.py
--rw-r--r--   0 jjy        (501) staff       (20)     3984 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/face_matting/nets/raft/utils/update.py
--rw-r--r--   0 jjy        (501) staff       (20)     6502 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/face_matting/nets/raft/utils/util.py
--rw-r--r--   0 jjy        (501) staff       (20)     4796 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/face_matting/nets/utils.py
--rw-r--r--   0 jjy        (501) staff       (20)     3157 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/face_matting/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-12 10:07:39.045203 innerverz-0.1.7/Innerverz/face_parser/
--rw-r--r--   0 jjy        (501) staff       (20)       28 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/face_parser/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     2894 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/face_parser/main.py
--rw-r--r--   0 jjy        (501) staff       (20)    11822 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/face_parser/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)      689 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/face_parser/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-12 10:07:39.046172 innerverz-0.1.7/Innerverz/face_reshaper/
--rw-r--r--   0 jjy        (501) staff       (20)       31 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/face_reshaper/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     3916 2023-07-12 10:02:03.000000 innerverz-0.1.7/Innerverz/face_reshaper/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     4248 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/face_reshaper/nets.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-12 10:07:39.046800 innerverz-0.1.7/Innerverz/face_reshaper/sub_nets/
--rw-r--r--   0 jjy        (501) staff       (20)     4670 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/face_reshaper/sub_nets/LadderEncoder.py
--rw-r--r--   0 jjy        (501) staff       (20)        0 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/face_reshaper/sub_nets/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     2839 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/face_reshaper/sub_nets/dense_motion.py
--rw-r--r--   0 jjy        (501) staff       (20)    14452 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/face_reshaper/sub_nets/util.py
--rw-r--r--   0 jjy        (501) staff       (20)     4694 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/face_reshaper/test.py
--rw-r--r--   0 jjy        (501) staff       (20)     1750 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/face_reshaper/util.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-12 10:07:39.047208 innerverz-0.1.7/Innerverz/face_reshaper/vis_utils/
--rw-r--r--   0 jjy        (501) staff       (20)        0 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/face_reshaper/vis_utils/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)      885 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/face_reshaper/vis_utils/vis_68.py
--rw-r--r--   0 jjy        (501) staff       (20)    10261 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/face_reshaper/vis_utils/vis_756.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-12 10:07:39.047801 innerverz-0.1.7/Innerverz/head_color_transfer/
--rw-r--r--   0 jjy        (501) staff       (20)       22 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/head_color_transfer/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     5773 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/head_color_transfer/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     8742 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/head_color_transfer/nets.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-12 10:07:39.049352 innerverz-0.1.7/Innerverz/head_color_transfer/sub_nets/
--rw-r--r--   0 jjy        (501) staff       (20)      100 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/head_color_transfer/sub_nets/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     7018 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/head_color_transfer/sub_nets/blend_net.py
--rw-r--r--   0 jjy        (501) staff       (20)     3642 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/head_color_transfer/sub_nets/discriminator.py
--rw-r--r--   0 jjy        (501) staff       (20)     3788 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/head_color_transfer/sub_nets/vgg19_net.py
--rw-r--r--   0 jjy        (501) staff       (20)     9366 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/head_color_transfer/sub_nets/warp_net.py
--rw-r--r--   0 jjy        (501) staff       (20)     1965 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/head_color_transfer/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-12 10:07:39.049895 innerverz-0.1.7/Innerverz/id_extractor/
--rw-r--r--   0 jjy        (501) staff       (20)       29 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/id_extractor/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     2443 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/id_extractor/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     5192 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/id_extractor/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)      693 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/id_extractor/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-12 10:07:39.050589 innerverz-0.1.7/Innerverz/reage/
--rw-r--r--   0 jjy        (501) staff       (20)       23 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/reage/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     2618 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/reage/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     3843 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/reage/net.py
--rw-r--r--   0 jjy        (501) staff       (20)    13178 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/reage/net_utils.py
--rw-r--r--   0 jjy        (501) staff       (20)      763 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/reage/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-12 10:07:39.051126 innerverz-0.1.7/Innerverz/relighter/
--rw-r--r--   0 jjy        (501) staff       (20)       27 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/relighter/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     3213 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/relighter/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     4546 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/relighter/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)     3030 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/relighter/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-12 10:07:39.051770 innerverz-0.1.7/Innerverz/upsampler/
--rw-r--r--   0 jjy        (501) staff       (20)       28 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/upsampler/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     2429 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/upsampler/main.py
--rw-r--r--   0 jjy        (501) staff       (20)    36818 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/upsampler/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)      830 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/upsampler/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-12 10:07:39.055139 innerverz-0.1.7/Innerverz/utils/
--rw-r--r--   0 jjy        (501) staff       (20)      109 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/utils/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     1438 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/utils/download.py
--rw-r--r--   0 jjy        (501) staff       (20)     1152 2023-07-12 10:02:23.000000 innerverz-0.1.7/Innerverz/utils/input.py
--rw-r--r--   0 jjy        (501) staff       (20)    15896 2023-07-12 10:00:49.000000 innerverz-0.1.7/Innerverz/utils/utils.py
--rw-r--r--   0 jjy        (501) staff       (20)     1073 2023-05-23 07:04:26.000000 innerverz-0.1.7/LICENSE.txt
--rw-r--r--   0 jjy        (501) staff       (20)      229 2023-07-12 10:07:39.064317 innerverz-0.1.7/PKG-INFO
--rw-r--r--   0 jjy        (501) staff       (20)       10 2023-05-23 07:04:26.000000 innerverz-0.1.7/README.md
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-12 10:07:39.057568 innerverz-0.1.7/innerverz.egg-info/
--rw-r--r--   0 jjy        (501) staff       (20)      229 2023-07-12 10:07:38.000000 innerverz-0.1.7/innerverz.egg-info/PKG-INFO
--rw-r--r--   0 jjy        (501) staff       (20)     8881 2023-07-12 10:07:38.000000 innerverz-0.1.7/innerverz.egg-info/SOURCES.txt
--rw-r--r--   0 jjy        (501) staff       (20)        1 2023-07-12 10:07:38.000000 innerverz-0.1.7/innerverz.egg-info/dependency_links.txt
--rw-r--r--   0 jjy        (501) staff       (20)       74 2023-07-12 10:07:38.000000 innerverz-0.1.7/innerverz.egg-info/requires.txt
--rw-r--r--   0 jjy        (501) staff       (20)       10 2023-07-12 10:07:38.000000 innerverz-0.1.7/innerverz.egg-info/top_level.txt
--rw-r--r--   0 jjy        (501) staff       (20)       89 2023-05-23 07:04:26.000000 innerverz-0.1.7/pyproject.toml
--rw-r--r--   0 jjy        (501) staff       (20)       38 2023-07-12 10:07:39.064697 innerverz-0.1.7/setup.cfg
--rw-r--r--   0 jjy        (501) staff       (20)      808 2023-07-12 06:40:39.000000 innerverz-0.1.7/setup.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-15 15:18:04.984509 innerverz-0.1.8/
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-15 15:18:04.957028 innerverz-0.1.8/Innerverz/
+-rw-r--r--   0 jjy        (501) staff       (20)     1730 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/__init__.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-15 15:18:04.957489 innerverz-0.1.8/Innerverz/data_process/
+-rw-r--r--   0 jjy        (501) staff       (20)       30 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/data_process/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3488 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/data_process/main.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-15 15:18:04.958321 innerverz-0.1.8/Innerverz/deblurrer/
+-rw-r--r--   0 jjy        (501) staff       (20)       27 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/deblurrer/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2611 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/deblurrer/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3609 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/deblurrer/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      843 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/deblurrer/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-15 15:18:04.958836 innerverz-0.1.8/Innerverz/deca/
+-rw-r--r--   0 jjy        (501) staff       (20)       23 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/deca/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)    24633 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/deca/main.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-15 15:18:04.959937 innerverz-0.1.8/Innerverz/deca/models/
+-rw-r--r--   0 jjy        (501) staff       (20)    12950 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/deca/models/FLAME.py
+-rw-r--r--   0 jjy        (501) staff       (20)        0 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/deca/models/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2464 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/deca/models/decoders.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1983 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/deca/models/detectors.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1427 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/deca/models/encoders.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1983 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/deca/models/face_detectors.py
+-rw-r--r--   0 jjy        (501) staff       (20)    13786 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/deca/models/lbs.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8386 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/deca/models/resnet.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1200 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/deca/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-15 15:18:04.961061 innerverz-0.1.8/Innerverz/deca/utils/
+-rw-r--r--   0 jjy        (501) staff       (20)        0 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/deca/utils/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5036 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/deca/utils/cfg.py
+-rw-r--r--   0 jjy        (501) staff       (20)    19673 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/deca/utils/lmks_756.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-15 15:18:04.961364 innerverz-0.1.8/Innerverz/deca/utils/rasterizer/
+-rw-r--r--   0 jjy        (501) staff       (20)        0 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/deca/utils/rasterizer/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)      706 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/deca/utils/rasterizer/setup.py
+-rw-r--r--   0 jjy        (501) staff       (20)    22281 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/deca/utils/renderer.py
+-rw-r--r--   0 jjy        (501) staff       (20)    12710 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/deca/utils/rotation_converter.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5574 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/deca/utils/tensor_cropper.py
+-rw-r--r--   0 jjy        (501) staff       (20)    11870 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/deca/utils/tracker_utils.py
+-rw-r--r--   0 jjy        (501) staff       (20)    26664 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/deca/utils/util.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-15 15:18:04.961997 innerverz-0.1.8/Innerverz/deep3dmm/
+-rw-r--r--   0 jjy        (501) staff       (20)       27 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/deep3dmm/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3598 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/deep3dmm/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)    25860 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/deep3dmm/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      627 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/deep3dmm/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-15 15:18:04.963199 innerverz-0.1.8/Innerverz/face_alignment/
+-rw-r--r--   0 jjy        (501) staff       (20)      125 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/face_alignment/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     6646 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/face_alignment/graphic_utils.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5089 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/face_alignment/landmark.py
+-rw-r--r--   0 jjy        (501) staff       (20)     9221 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/face_alignment/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)    12774 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/face_alignment/retina_face.py
+-rw-r--r--   0 jjy        (501) staff       (20)      640 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/face_alignment/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-15 15:18:04.963640 innerverz-0.1.8/Innerverz/face_alignment/utils/
+-rw-r--r--   0 jjy        (501) staff       (20)       24 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/face_alignment/utils/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3354 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/face_alignment/utils/face_align.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4933 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/face_alignment/utils/transform.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-15 15:18:04.964396 innerverz-0.1.8/Innerverz/face_color_transfer/
+-rw-r--r--   0 jjy        (501) staff       (20)       22 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/face_color_transfer/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5595 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/face_color_transfer/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8503 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/face_color_transfer/nets.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-15 15:18:04.965309 innerverz-0.1.8/Innerverz/face_color_transfer/sub_nets/
+-rw-r--r--   0 jjy        (501) staff       (20)      100 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/face_color_transfer/sub_nets/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     7018 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/face_color_transfer/sub_nets/blend_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3642 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/face_color_transfer/sub_nets/discriminator.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3788 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/face_color_transfer/sub_nets/vgg19_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     9366 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/face_color_transfer/sub_nets/warp_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2015 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/face_color_transfer/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-15 15:18:04.965911 innerverz-0.1.8/Innerverz/face_enhancer/
+-rw-r--r--   0 jjy        (501) staff       (20)       30 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/face_enhancer/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3881 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/face_enhancer/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4079 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/face_enhancer/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      768 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/face_enhancer/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-15 15:18:04.966373 innerverz-0.1.8/Innerverz/face_matting/
+-rw-r--r--   0 jjy        (501) staff       (20)       30 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/face_matting/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8110 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/face_matting/main.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-15 15:18:04.966978 innerverz-0.1.8/Innerverz/face_matting/nets/
+-rw-r--r--   0 jjy        (501) staff       (20)       68 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/face_matting/nets/__init__.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-15 15:18:04.967264 innerverz-0.1.8/Innerverz/face_matting/nets/decoders/
+-rw-r--r--   0 jjy        (501) staff       (20)      219 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/face_matting/nets/decoders/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8175 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/face_matting/nets/decoders/resnet_decoder.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-15 15:18:04.967576 innerverz-0.1.8/Innerverz/face_matting/nets/encoders/
+-rw-r--r--   0 jjy        (501) staff       (20)    24822 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/face_matting/nets/encoders/MatteFormer.py
+-rw-r--r--   0 jjy        (501) staff       (20)        0 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/face_matting/nets/encoders/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4386 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/face_matting/nets/generators.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2650 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/face_matting/nets/ops.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-15 15:18:04.967821 innerverz-0.1.8/Innerverz/face_matting/nets/raft/
+-rw-r--r--   0 jjy        (501) staff       (20)       20 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/face_matting/nets/raft/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4009 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/face_matting/nets/raft/main.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-15 15:18:04.968570 innerverz-0.1.8/Innerverz/face_matting/nets/raft/utils/
+-rw-r--r--   0 jjy        (501) staff       (20)       94 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/face_matting/nets/raft/utils/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3079 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/face_matting/nets/raft/utils/corr.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8847 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/face_matting/nets/raft/utils/extractor.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3984 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/face_matting/nets/raft/utils/update.py
+-rw-r--r--   0 jjy        (501) staff       (20)     6502 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/face_matting/nets/raft/utils/util.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4819 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/face_matting/nets/utils.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3157 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/face_matting/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-15 15:18:04.969302 innerverz-0.1.8/Innerverz/face_parser/
+-rw-r--r--   0 jjy        (501) staff       (20)       28 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/face_parser/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2894 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/face_parser/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)    11822 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/face_parser/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      689 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/face_parser/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-15 15:18:04.970137 innerverz-0.1.8/Innerverz/face_reshaper/
+-rw-r--r--   0 jjy        (501) staff       (20)       31 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/face_reshaper/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3916 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/face_reshaper/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4248 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/face_reshaper/nets.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-15 15:18:04.971121 innerverz-0.1.8/Innerverz/face_reshaper/sub_nets/
+-rw-r--r--   0 jjy        (501) staff       (20)     4670 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/face_reshaper/sub_nets/LadderEncoder.py
+-rw-r--r--   0 jjy        (501) staff       (20)        0 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/face_reshaper/sub_nets/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2839 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/face_reshaper/sub_nets/dense_motion.py
+-rw-r--r--   0 jjy        (501) staff       (20)    14452 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/face_reshaper/sub_nets/util.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4694 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/face_reshaper/test.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1750 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/face_reshaper/util.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-15 15:18:04.971640 innerverz-0.1.8/Innerverz/face_reshaper/vis_utils/
+-rw-r--r--   0 jjy        (501) staff       (20)        0 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/face_reshaper/vis_utils/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)      885 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/face_reshaper/vis_utils/vis_68.py
+-rw-r--r--   0 jjy        (501) staff       (20)    10213 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/face_reshaper/vis_utils/vis_756.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-15 15:18:04.972241 innerverz-0.1.8/Innerverz/head_color_transfer/
+-rw-r--r--   0 jjy        (501) staff       (20)       22 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/head_color_transfer/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5773 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/head_color_transfer/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8742 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/head_color_transfer/nets.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-15 15:18:04.972960 innerverz-0.1.8/Innerverz/head_color_transfer/sub_nets/
+-rw-r--r--   0 jjy        (501) staff       (20)      100 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/head_color_transfer/sub_nets/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     7018 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/head_color_transfer/sub_nets/blend_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3642 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/head_color_transfer/sub_nets/discriminator.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3788 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/head_color_transfer/sub_nets/vgg19_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     9366 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/head_color_transfer/sub_nets/warp_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1965 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/head_color_transfer/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-15 15:18:04.973587 innerverz-0.1.8/Innerverz/id_extractor/
+-rw-r--r--   0 jjy        (501) staff       (20)       29 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/id_extractor/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2443 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/id_extractor/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5192 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/id_extractor/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      693 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/id_extractor/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-15 15:18:04.974419 innerverz-0.1.8/Innerverz/reage/
+-rw-r--r--   0 jjy        (501) staff       (20)       23 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/reage/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2618 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/reage/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3843 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/reage/net.py
+-rw-r--r--   0 jjy        (501) staff       (20)    13178 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/reage/net_utils.py
+-rw-r--r--   0 jjy        (501) staff       (20)      763 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/reage/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-15 15:18:04.975077 innerverz-0.1.8/Innerverz/relighter/
+-rw-r--r--   0 jjy        (501) staff       (20)       27 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/relighter/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3213 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/relighter/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4546 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/relighter/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3030 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/relighter/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-15 15:18:04.975962 innerverz-0.1.8/Innerverz/upsampler/
+-rw-r--r--   0 jjy        (501) staff       (20)       28 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/upsampler/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2429 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/upsampler/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)    36818 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/upsampler/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      830 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/upsampler/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-15 15:18:04.976573 innerverz-0.1.8/Innerverz/utils/
+-rw-r--r--   0 jjy        (501) staff       (20)      109 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/utils/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1438 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/utils/download.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1152 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/utils/input.py
+-rw-r--r--   0 jjy        (501) staff       (20)    15896 2023-07-15 15:17:28.000000 innerverz-0.1.8/Innerverz/utils/utils.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1073 2023-05-23 07:04:26.000000 innerverz-0.1.8/LICENSE.txt
+-rw-r--r--   0 jjy        (501) staff       (20)      229 2023-07-15 15:18:04.984649 innerverz-0.1.8/PKG-INFO
+-rw-r--r--   0 jjy        (501) staff       (20)       10 2023-05-23 07:04:26.000000 innerverz-0.1.8/README.md
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-15 15:18:04.977337 innerverz-0.1.8/innerverz.egg-info/
+-rw-r--r--   0 jjy        (501) staff       (20)      229 2023-07-15 15:18:04.000000 innerverz-0.1.8/innerverz.egg-info/PKG-INFO
+-rw-r--r--   0 jjy        (501) staff       (20)     8881 2023-07-15 15:18:04.000000 innerverz-0.1.8/innerverz.egg-info/SOURCES.txt
+-rw-r--r--   0 jjy        (501) staff       (20)        1 2023-07-15 15:18:04.000000 innerverz-0.1.8/innerverz.egg-info/dependency_links.txt
+-rw-r--r--   0 jjy        (501) staff       (20)       74 2023-07-15 15:18:04.000000 innerverz-0.1.8/innerverz.egg-info/requires.txt
+-rw-r--r--   0 jjy        (501) staff       (20)       10 2023-07-15 15:18:04.000000 innerverz-0.1.8/innerverz.egg-info/top_level.txt
+-rw-r--r--   0 jjy        (501) staff       (20)       89 2023-05-23 07:04:26.000000 innerverz-0.1.8/pyproject.toml
+-rw-r--r--   0 jjy        (501) staff       (20)       38 2023-07-15 15:18:04.985052 innerverz-0.1.8/setup.cfg
+-rw-r--r--   0 jjy        (501) staff       (20)      808 2023-07-15 15:17:51.000000 innerverz-0.1.8/setup.py
```

### Comparing `innerverz-0.1.7/Innerverz/__init__.py` & `innerverz-0.1.8/Innerverz/__init__.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/data_process/main.py` & `innerverz-0.1.8/Innerverz/data_process/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/deblurrer/main.py` & `innerverz-0.1.8/Innerverz/deblurrer/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/deblurrer/nets.py` & `innerverz-0.1.8/Innerverz/deblurrer/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/deblurrer/test.py` & `innerverz-0.1.8/Innerverz/deblurrer/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/deca/main.py` & `innerverz-0.1.8/Innerverz/deca/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/deca/models/FLAME.py` & `innerverz-0.1.8/Innerverz/deca/models/FLAME.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/deca/models/decoders.py` & `innerverz-0.1.8/Innerverz/deca/models/decoders.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/deca/models/detectors.py` & `innerverz-0.1.8/Innerverz/deca/models/detectors.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/deca/models/encoders.py` & `innerverz-0.1.8/Innerverz/deca/models/encoders.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/deca/models/face_detectors.py` & `innerverz-0.1.8/Innerverz/deca/models/face_detectors.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/deca/models/lbs.py` & `innerverz-0.1.8/Innerverz/deca/models/lbs.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/deca/models/resnet.py` & `innerverz-0.1.8/Innerverz/deca/models/resnet.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/deca/test.py` & `innerverz-0.1.8/Innerverz/deca/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/deca/utils/cfg.py` & `innerverz-0.1.8/Innerverz/deca/utils/cfg.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/deca/utils/lmks_756.py` & `innerverz-0.1.8/Innerverz/deca/utils/lmks_756.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/deca/utils/rasterizer/setup.py` & `innerverz-0.1.8/Innerverz/deca/utils/rasterizer/setup.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/deca/utils/renderer.py` & `innerverz-0.1.8/Innerverz/deca/utils/renderer.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/deca/utils/rotation_converter.py` & `innerverz-0.1.8/Innerverz/deca/utils/rotation_converter.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/deca/utils/tensor_cropper.py` & `innerverz-0.1.8/Innerverz/deca/utils/tensor_cropper.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/deca/utils/tracker_utils.py` & `innerverz-0.1.8/Innerverz/deca/utils/tracker_utils.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/deca/utils/util.py` & `innerverz-0.1.8/Innerverz/deca/utils/util.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/deep3dmm/main.py` & `innerverz-0.1.8/Innerverz/deep3dmm/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/deep3dmm/nets.py` & `innerverz-0.1.8/Innerverz/deep3dmm/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/deep3dmm/test.py` & `innerverz-0.1.8/Innerverz/deep3dmm/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/face_alignment/graphic_utils.py` & `innerverz-0.1.8/Innerverz/face_alignment/graphic_utils.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/face_alignment/landmark.py` & `innerverz-0.1.8/Innerverz/face_alignment/landmark.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/face_alignment/main.py` & `innerverz-0.1.8/Innerverz/face_alignment/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,14 +14,15 @@
         
         "invz" : algorithm costumed by Innerverz.co    
         
         Methods
         --------
         - get_face
         - detect_lmk
+        - detect_lmk_multi
         - align_face_from_106
         - affine_transform
         
         Return
         --------
         dicts
         '''
@@ -233,8 +234,46 @@
             - dtype : numpy array
             - shape : (106, 2)
         """
         constant_term = np.ones((lmks_106.shape[0],1))
         expanded_points = np.concatenate((lmks_106, constant_term), axis=-1)
         result = np.matmul(expanded_points, np.transpose(tfm))
         dicts['aligned_lmks_106'] = result
-        return dicts
+        return dicts
+    
+    
+    def detect_lmk_multi(self, img, pad=256, dicts={}):
+        """
+        Input
+        ---------
+            - dtype : cv2 image
+            - shape : (h, w, 3)
+            - min max : (0, 255)
+            - pad[int]
+            
+        Output
+        ---------
+            - FaceBool
+                - dtype : Bool
+            - lmks_106
+                - dtype : numpy array
+                - shape : (106, 2)
+        """
+        
+        pad_img = np.pad(img, ((pad, pad), (pad,pad), (0,0))) 
+        temp, _ = self.backbone.detect(pad_img)
+        
+        if len(temp):
+            lmks_106_list, facebool_list = [], []
+            for i in range(len(temp)):
+                bbox = temp[i][0:4]
+                pad_lmks_106 = self.lmk_detector.get(pad_img, bbox)
+                lmks_106 = pad_lmks_106 - pad
+                lmks_106_list.append(lmks_106); facebool_list.append(True)
+            dicts['lmks_106'] = lmks_106_list
+            dicts['facebool'] = facebool_list
+            return dicts
+
+        else:
+            dicts['lmks_106'] = None
+            dicts['facebool'] = False
+            return dicts
```

### Comparing `innerverz-0.1.7/Innerverz/face_alignment/retina_face.py` & `innerverz-0.1.8/Innerverz/face_alignment/retina_face.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/face_alignment/test.py` & `innerverz-0.1.8/Innerverz/face_alignment/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/face_alignment/utils/face_align.py` & `innerverz-0.1.8/Innerverz/face_alignment/utils/face_align.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/face_alignment/utils/transform.py` & `innerverz-0.1.8/Innerverz/face_alignment/utils/transform.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/face_color_transfer/main.py` & `innerverz-0.1.8/Innerverz/face_color_transfer/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/face_color_transfer/nets.py` & `innerverz-0.1.8/Innerverz/face_color_transfer/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/face_color_transfer/sub_nets/blend_net.py` & `innerverz-0.1.8/Innerverz/face_color_transfer/sub_nets/blend_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/face_color_transfer/sub_nets/discriminator.py` & `innerverz-0.1.8/Innerverz/face_color_transfer/sub_nets/discriminator.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/face_color_transfer/sub_nets/vgg19_net.py` & `innerverz-0.1.8/Innerverz/face_color_transfer/sub_nets/vgg19_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/face_color_transfer/sub_nets/warp_net.py` & `innerverz-0.1.8/Innerverz/face_color_transfer/sub_nets/warp_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/face_color_transfer/test.py` & `innerverz-0.1.8/Innerverz/face_color_transfer/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/face_enhancer/main.py` & `innerverz-0.1.8/Innerverz/face_enhancer/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/face_enhancer/nets.py` & `innerverz-0.1.8/Innerverz/face_enhancer/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/face_enhancer/test.py` & `innerverz-0.1.8/Innerverz/face_enhancer/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/face_matting/main.py` & `innerverz-0.1.8/Innerverz/face_matting/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/face_matting/nets/decoders/resnet_decoder.py` & `innerverz-0.1.8/Innerverz/face_matting/nets/decoders/resnet_decoder.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/face_matting/nets/encoders/MatteFormer.py` & `innerverz-0.1.8/Innerverz/face_matting/nets/encoders/MatteFormer.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/face_matting/nets/generators.py` & `innerverz-0.1.8/Innerverz/face_matting/nets/generators.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/face_matting/nets/ops.py` & `innerverz-0.1.8/Innerverz/face_matting/nets/ops.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/face_matting/nets/raft/main.py` & `innerverz-0.1.8/Innerverz/face_matting/nets/raft/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/face_matting/nets/raft/utils/corr.py` & `innerverz-0.1.8/Innerverz/face_matting/nets/raft/utils/corr.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/face_matting/nets/raft/utils/extractor.py` & `innerverz-0.1.8/Innerverz/face_matting/nets/raft/utils/extractor.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/face_matting/nets/raft/utils/update.py` & `innerverz-0.1.8/Innerverz/face_matting/nets/raft/utils/update.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/face_matting/nets/raft/utils/util.py` & `innerverz-0.1.8/Innerverz/face_matting/nets/raft/utils/util.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/face_matting/nets/utils.py` & `innerverz-0.1.8/Innerverz/face_matting/nets/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,16 @@
         uncertain_area_ = cv2.dilate(uncertain_area_, Kernels[width])
         uncertain_area[n,0,:,:] = uncertain_area_
 
     weight = np.zeros_like(uncertain_area)
     weight[uncertain_area == 1] = 1
 
     weight = np.array(weight, dtype=np.float)
-    weight = torch.from_numpy(weight).cuda()
+    weight = torch.from_numpy(weight).to(pred.device)
+    
 
     weight = F.interpolate(weight, size=(H,W), mode='nearest')
 
     return weight
 
 class InputPadder:
     """ Pads images such that dimensions are divisible by 8 """
@@ -145,12 +146,12 @@
         uncertain_area_ = cv2.dilate(uncertain_area_, Kernels[width])
         uncertain_area[n,0,:,:] = uncertain_area_
 
     weight = np.zeros_like(uncertain_area)
     weight[uncertain_area == 1] = 1
 
     weight = np.array(weight, dtype=np.float)
-    weight = torch.from_numpy(weight).cuda()
+    weight = torch.from_numpy(weight).to(pred.device)
 
     weight = F.interpolate(weight, size=(H,W), mode='nearest')
 
     return weight
```

### Comparing `innerverz-0.1.7/Innerverz/face_matting/test.py` & `innerverz-0.1.8/Innerverz/face_matting/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/face_parser/main.py` & `innerverz-0.1.8/Innerverz/face_parser/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/face_parser/nets.py` & `innerverz-0.1.8/Innerverz/face_parser/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/face_parser/test.py` & `innerverz-0.1.8/Innerverz/face_parser/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/face_reshaper/main.py` & `innerverz-0.1.8/Innerverz/face_reshaper/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/face_reshaper/nets.py` & `innerverz-0.1.8/Innerverz/face_reshaper/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/face_reshaper/sub_nets/LadderEncoder.py` & `innerverz-0.1.8/Innerverz/face_reshaper/sub_nets/LadderEncoder.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/face_reshaper/sub_nets/dense_motion.py` & `innerverz-0.1.8/Innerverz/face_reshaper/sub_nets/dense_motion.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/face_reshaper/sub_nets/util.py` & `innerverz-0.1.8/Innerverz/face_reshaper/sub_nets/util.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/face_reshaper/test.py` & `innerverz-0.1.8/Innerverz/face_reshaper/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/face_reshaper/util.py` & `innerverz-0.1.8/Innerverz/face_reshaper/util.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/face_reshaper/vis_utils/vis_68.py` & `innerverz-0.1.8/Innerverz/face_reshaper/vis_utils/vis_68.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/face_reshaper/vis_utils/vis_756.py` & `innerverz-0.1.8/Innerverz/face_reshaper/vis_utils/vis_756.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,42 +46,43 @@
     [592, 593],
     [593, 594],
     [594, 595],
     [595, 596],
     [596, 597],
     [597, 570],
     [570, 613],
-    [613, 503],
-    [503, 226],
+    [613, 226],
     [226, 228],
     [228, 227],
     [227, 323],
     [323, 322],
     [322, 326],
     [326, 325],
     [613, 571],
     [571, 572],
     [572, 573],
     [573, 574],
     [574, 575],
-    [575, 576],
+    [575, 610],
+    [610, 576],
     [576, 577],
     [577, 578],
     [578, 579],
     [579, 580],
     [580, 651],
     [651, 650],
     [650, 649],
     [649, 648],
     [648, 693],
     [693, 645],
     [645, 642],
-    [642, 671],
-    [671, 673],
-    [673, 639],
+    [642, 641],
+    [641, 640],
+    [640, 671],
+    [671, 639],
     [639, 697],
     [529, 430],
     [430, 429],
     [429, 363],
     [363, 364],
     [364, 427],
     [427, 428],
@@ -594,33 +595,29 @@
     [462, 461],
     [461, 450],
     [450, 630],
     [630, 171],
     [171, 182],
     [182, 183],
     [183, 197],
-    [197, 150],
-    [150, 194],
-    [194, 149],
-    [149, 148],
+    [197, 192],
+    [192, 148],
     [148, 205],
     [205, 206],
     [206, 210],
     [210, 213],
     [213, 222],
     [222, 617],
     [617, 499],
     [499, 490],
     [490, 487],
     [487, 483],
     [483, 482],
     [482, 432],
-    [432, 431],
-    [431, 433],
-    [433, 462],
+    [432, 462],
     [620, 220],
     [220, 219],
     [219, 209],
     [209, 207],
     [207, 208],
     [208, 195],
     [195, 194],
```

### Comparing `innerverz-0.1.7/Innerverz/head_color_transfer/main.py` & `innerverz-0.1.8/Innerverz/head_color_transfer/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/head_color_transfer/nets.py` & `innerverz-0.1.8/Innerverz/head_color_transfer/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/head_color_transfer/sub_nets/blend_net.py` & `innerverz-0.1.8/Innerverz/head_color_transfer/sub_nets/blend_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/head_color_transfer/sub_nets/discriminator.py` & `innerverz-0.1.8/Innerverz/head_color_transfer/sub_nets/discriminator.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/head_color_transfer/sub_nets/vgg19_net.py` & `innerverz-0.1.8/Innerverz/head_color_transfer/sub_nets/vgg19_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/head_color_transfer/sub_nets/warp_net.py` & `innerverz-0.1.8/Innerverz/head_color_transfer/sub_nets/warp_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/head_color_transfer/test.py` & `innerverz-0.1.8/Innerverz/head_color_transfer/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/id_extractor/main.py` & `innerverz-0.1.8/Innerverz/id_extractor/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/id_extractor/nets.py` & `innerverz-0.1.8/Innerverz/id_extractor/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/id_extractor/test.py` & `innerverz-0.1.8/Innerverz/id_extractor/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/reage/main.py` & `innerverz-0.1.8/Innerverz/reage/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/reage/net.py` & `innerverz-0.1.8/Innerverz/reage/net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/reage/net_utils.py` & `innerverz-0.1.8/Innerverz/reage/net_utils.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/reage/test.py` & `innerverz-0.1.8/Innerverz/reage/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/relighter/main.py` & `innerverz-0.1.8/Innerverz/relighter/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/relighter/nets.py` & `innerverz-0.1.8/Innerverz/relighter/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/relighter/test.py` & `innerverz-0.1.8/Innerverz/relighter/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/upsampler/main.py` & `innerverz-0.1.8/Innerverz/upsampler/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/upsampler/nets.py` & `innerverz-0.1.8/Innerverz/upsampler/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/upsampler/test.py` & `innerverz-0.1.8/Innerverz/upsampler/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/utils/download.py` & `innerverz-0.1.8/Innerverz/utils/download.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/utils/input.py` & `innerverz-0.1.8/Innerverz/utils/input.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/Innerverz/utils/utils.py` & `innerverz-0.1.8/Innerverz/utils/utils.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/LICENSE.txt` & `innerverz-0.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/innerverz.egg-info/SOURCES.txt` & `innerverz-0.1.8/innerverz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.7/setup.py` & `innerverz-0.1.8/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 except (IOError, ImportError, ModuleNotFoundError):
     print('WARNING: pandoc not enabled')
     long_description = open('README.md').read()
     pypandoc_enabled = False
 
 setup(
     name="innerverz",
-    version="0.1.7",
+    version="0.1.8",
     author="Innerverz",
     author_email="study@innerverz.com",
     description="innerverz package",
     long_description=long_description,
     python_requires=">=3.6",
     install_requires=requirements,
     packages=find_packages()
```

