# Comparing `tmp/pancollection-0.3.5-py3-none-any.whl.zip` & `tmp/pancollection-0.3.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,96 +1,79 @@
-Zip file size: 144329 bytes, number of entries: 94
+Zip file size: 120091 bytes, number of entries: 77
 -rw-rw-rw-  2.0 fat   122081 b- defN 23-Jun-17 17:03 pancollection/PanCollection_colab.ipynb
 -rw-rw-rw-  2.0 fat      321 b- defN 23-Jun-10 06:32 pancollection/__init__.py
--rw-rw-rw-  2.0 fat     1178 b- defN 23-Jun-22 19:31 pancollection/run_pansharpening.py
+-rw-rw-rw-  2.0 fat     1187 b- defN 23-Jul-14 14:22 pancollection/run_pansharpening.py
 -rw-rw-rw-  2.0 fat     2805 b- defN 23-Jun-10 06:32 pancollection/run_test_pansharpening.py
+-rw-rw-rw-  2.0 fat     2121 b- defN 23-Jun-28 15:04 pancollection/run_train_model.py
 -rw-rw-rw-  2.0 fat       72 b- defN 23-Jun-10 06:23 pancollection/common/__init__.py
--rw-rw-rw-  2.0 fat      641 b- defN 23-Jun-10 06:32 pancollection/common/builder.py
--rw-rw-rw-  2.0 fat    14450 b- defN 23-Jun-22 04:05 pancollection/common/dataset.py
+-rw-rw-rw-  2.0 fat      651 b- defN 23-Jul-01 06:23 pancollection/common/builder.py
+-rw-rw-rw-  2.0 fat    14791 b- defN 23-Jul-07 16:49 pancollection/common/dataset.py
 -rw-rw-rw-  2.0 fat     2238 b- defN 23-Jun-10 06:23 pancollection/common/dataset_hp.py
--rw-rw-rw-  2.0 fat    16414 b- defN 23-Jun-10 06:23 pancollection/common/evaluate.py
+-rw-rw-rw-  2.0 fat    18749 b- defN 23-Jul-01 06:21 pancollection/common/evaluate.py
 -rw-rw-rw-  2.0 fat     7372 b- defN 23-Jun-22 08:32 pancollection/common/psdata.py
 -rw-rw-rw-  2.0 fat     4959 b- defN 23-Jun-10 06:29 pancollection/common/test_panloader.py
 -rw-rw-rw-  2.0 fat     3833 b- defN 23-Jun-10 06:33 pancollection/common/train_panloader.py
 -rw-rw-rw-  2.0 fat     3833 b- defN 23-Jun-17 16:41 pancollection/common/valid_panloader.py
 -rw-rw-rw-  2.0 fat     2320 b- defN 23-Jun-10 06:29 pancollection/common/FS_index/D_lambda_K.py
 -rw-rw-rw-  2.0 fat     2392 b- defN 23-Jun-10 06:23 pancollection/common/FS_index/HQNR.py
 -rw-rw-rw-  2.0 fat     2213 b- defN 23-Jun-10 06:23 pancollection/common/FS_index/MTF.py
 -rw-rw-rw-  2.0 fat     2224 b- defN 23-Jun-10 06:23 pancollection/common/FS_index/MTF_pan.py
 -rw-rw-rw-  2.0 fat      113 b- defN 23-Jun-10 06:29 pancollection/common/FS_index/__init__.py
 -rw-rw-rw-  2.0 fat     2593 b- defN 23-Jun-10 06:23 pancollection/common/FS_index/genMTF.py
 -rw-rw-rw-  2.0 fat      730 b- defN 23-Jun-10 06:23 pancollection/common/FS_index/genMTF_pan.py
 -rw-rw-rw-  2.0 fat     5515 b- defN 23-Jun-10 06:23 pancollection/common/FS_index/imresize.py
--rw-rw-rw-  2.0 fat     9046 b- defN 23-Jun-10 06:29 pancollection/common/FS_index/indexes_evaluation_FS.py
+-rw-rw-rw-  2.0 fat    10043 b- defN 23-Jun-24 09:55 pancollection/common/FS_index/indexes_evaluation_FS.py
 -rw-rw-rw-  2.0 fat     3106 b- defN 23-Jun-10 06:23 pancollection/common/FS_index/interp23.py
 -rw-rw-rw-  2.0 fat     6354 b- defN 23-Jun-10 06:29 pancollection/common/FS_index/my_D_s.py
 -rw-rw-rw-  2.0 fat     8336 b- defN 23-Jun-10 06:29 pancollection/common/FS_index/my_q2n.py
 -rw-rw-rw-  2.0 fat     1237 b- defN 23-Jun-10 06:23 pancollection/common/FS_index/tools.py
+-rw-rw-rw-  2.0 fat      136 b- defN 23-Jun-24 09:47 pancollection/common/tests/__init__.py
 -rw-rw-rw-  2.0 fat      336 b- defN 23-Jun-10 06:23 pancollection/configs/__init__.py
--rw-rw-rw-  2.0 fat     1169 b- defN 23-Jun-10 06:23 pancollection/configs/configs.py
+-rw-rw-rw-  2.0 fat     1226 b- defN 23-Jun-25 04:12 pancollection/configs/configs.py
 -rw-rw-rw-  2.0 fat      822 b- defN 23-Jun-21 17:30 pancollection/configs/hook_configs.py
 -rw-rw-rw-  2.0 fat      846 b- defN 23-Jun-10 06:23 pancollection/configs/load_ckpt_configs.py
 -rw-rw-rw-  2.0 fat     3713 b- defN 23-Jun-17 17:13 pancollection/configs/option_DCFNet.py
 -rw-rw-rw-  2.0 fat     3740 b- defN 23-Jun-17 17:13 pancollection/configs/option_LAGNet.py
 -rw-rw-rw-  2.0 fat     3625 b- defN 23-Jun-17 17:13 pancollection/configs/option_bdpn.py
 -rw-rw-rw-  2.0 fat     3537 b- defN 23-Jun-17 17:13 pancollection/configs/option_dicnn.py
 -rw-rw-rw-  2.0 fat     3584 b- defN 23-Jun-17 17:13 pancollection/configs/option_drpnn.py
 -rw-rw-rw-  2.0 fat     4121 b- defN 23-Jun-21 18:03 pancollection/configs/option_fusionnet.py
 -rw-rw-rw-  2.0 fat     3580 b- defN 23-Jun-17 17:13 pancollection/configs/option_msdcnn.py
 -rw-rw-rw-  2.0 fat     3748 b- defN 23-Jun-17 17:13 pancollection/configs/option_pannet.py
 -rw-rw-rw-  2.0 fat     3629 b- defN 23-Jun-17 17:13 pancollection/configs/option_pnn.py
 -rw-rw-rw-  2.0 fat      508 b- defN 23-Jun-10 06:23 pancollection/models/__init__.py
--rw-rw-rw-  2.0 fat     3005 b- defN 23-Jun-21 16:01 pancollection/models/base_model.py
+-rw-rw-rw-  2.0 fat     3738 b- defN 23-Jun-24 09:56 pancollection/models/base_model.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-10 06:23 pancollection/models/ADKNet/__init__.py
 -rw-rw-rw-  2.0 fat       18 b- defN 23-Jun-10 06:23 pancollection/models/ADKNet/ddf/__init__.py
 -rw-rw-rw-  2.0 fat    11638 b- defN 23-Jun-10 06:23 pancollection/models/ADKNet/ddf/ddf.py
 -rw-rw-rw-  2.0 fat     2289 b- defN 23-Jun-10 06:23 pancollection/models/ADKNet/ddf/setup.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-10 06:23 pancollection/models/BDPN/__init__.py
 -rw-rw-rw-  2.0 fat     3835 b- defN 23-Jun-10 06:28 pancollection/models/BDPN/bdpn_main.py
 -rw-rw-rw-  2.0 fat     7822 b- defN 23-Jun-10 06:26 pancollection/models/BDPN/model_bdpn.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-10 06:23 pancollection/models/DCFNet/__init__.py
 -rw-rw-rw-  2.0 fat    32420 b- defN 23-Jun-10 06:23 pancollection/models/DCFNet/model_fcc_dense_head.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-07 09:54 pancollection/models/DHIFNet/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-10 06:23 pancollection/models/DRPNN/__init__.py
 -rw-rw-rw-  2.0 fat     3842 b- defN 23-Jun-10 06:28 pancollection/models/DRPNN/drpnn_main.py
 -rw-rw-rw-  2.0 fat     5302 b- defN 23-Jun-10 06:23 pancollection/models/DRPNN/model_drpnn.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-10 06:23 pancollection/models/DiCNN/__init__.py
 -rw-rw-rw-  2.0 fat     3816 b- defN 23-Jun-10 06:30 pancollection/models/DiCNN/dicnn_main.py
 -rw-rw-rw-  2.0 fat     3768 b- defN 23-Jun-10 06:23 pancollection/models/DiCNN/model_dicnn.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-10 06:23 pancollection/models/FusionNet/__init__.py
 -rw-rw-rw-  2.0 fat     3494 b- defN 23-Jun-22 09:19 pancollection/models/FusionNet/fusionnet_main.py
 -rw-rw-rw-  2.0 fat     5615 b- defN 23-Jun-22 09:18 pancollection/models/FusionNet/model_fusionnet.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-10 06:23 pancollection/models/GPPNN/__init__.py
--rw-rw-rw-  2.0 fat     1644 b- defN 23-Jun-10 06:23 pancollection/models/GPPNN/metrics.py
--rw-rw-rw-  2.0 fat    38742 b- defN 23-Jun-10 06:23 pancollection/models/GPPNN/utils.py
--rw-rw-rw-  2.0 fat     4902 b- defN 23-Jun-10 06:23 pancollection/models/GPPNN/models/GPPNN.py
--rw-rw-rw-  2.0 fat      686 b- defN 23-Jun-10 06:23 pancollection/models/GPPNN/models/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-10 06:23 pancollection/models/LAGConv/__init__.py
--rw-rw-rw-  2.0 fat     2254 b- defN 23-Mar-27 06:21 pancollection/models/LAGConv/data.py
 -rw-rw-rw-  2.0 fat     6955 b- defN 23-Jun-10 06:31 pancollection/models/LAGConv/model.py
--rw-rw-rw-  2.0 fat     1990 b- defN 23-Mar-27 06:21 pancollection/models/LAGConv/test.py
--rw-rw-rw-  2.0 fat     7423 b- defN 23-Mar-27 06:21 pancollection/models/LAGConv/train.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-10 06:23 pancollection/models/MSDCNN/__init__.py
 -rw-rw-rw-  2.0 fat     5873 b- defN 23-Jun-10 06:28 pancollection/models/MSDCNN/model_msdcnn.py
 -rw-rw-rw-  2.0 fat     3831 b- defN 23-Jun-10 06:28 pancollection/models/MSDCNN/msdcnn_main.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-10 06:23 pancollection/models/MUCNN/__init__.py
--rw-rw-rw-  2.0 fat     3395 b- defN 23-Jun-10 06:23 pancollection/models/MUCNN/main_test_multi.py
--rw-rw-rw-  2.0 fat     2670 b- defN 23-Jun-10 06:23 pancollection/models/MUCNN/main_test_single.py
--rw-rw-rw-  2.0 fat     8936 b- defN 23-Jun-10 06:23 pancollection/models/MUCNN/train.py
--rw-rw-rw-  2.0 fat       81 b- defN 22-Mar-08 03:11 pancollection/models/MUCNN/lib/__init__.py
--rw-rw-rw-  2.0 fat      940 b- defN 22-Mar-08 03:11 pancollection/models/MUCNN/lib/data.py
--rw-rw-rw-  2.0 fat     3897 b- defN 22-Mar-08 03:11 pancollection/models/MUCNN/lib/datasets.py
--rw-rw-rw-  2.0 fat     5410 b- defN 22-Mar-08 03:11 pancollection/models/MUCNN/lib/evaluate.py
--rw-rw-rw-  2.0 fat     3027 b- defN 22-Mar-08 03:11 pancollection/models/MUCNN/lib/model.py
--rw-rw-rw-  2.0 fat     1328 b- defN 22-Mar-08 03:11 pancollection/models/MUCNN/lib/utils.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-10 06:23 pancollection/models/PNN/__init__.py
 -rw-rw-rw-  2.0 fat     2530 b- defN 23-Jun-10 06:23 pancollection/models/PNN/model_pnn.py
 -rw-rw-rw-  2.0 fat     4367 b- defN 23-Jun-10 06:31 pancollection/models/PNN/pnn_main.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-10 06:23 pancollection/models/PanNet/__init__.py
 -rw-rw-rw-  2.0 fat     4917 b- defN 23-Jun-10 06:23 pancollection/models/PanNet/model_pannet.py
 -rw-rw-rw-  2.0 fat     3790 b- defN 23-Jun-10 06:31 pancollection/models/PanNet/pannet_main.py
--rw-rw-rw-  2.0 fat    18431 b- defN 23-Jun-22 19:33 pancollection-0.3.5.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     9354 b- defN 23-Jun-22 19:33 pancollection-0.3.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-22 19:33 pancollection-0.3.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       14 b- defN 23-Jun-22 19:33 pancollection-0.3.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     8891 b- defN 23-Jun-22 19:33 pancollection-0.3.5.dist-info/RECORD
-94 files, 506568 bytes uncompressed, 129887 bytes compressed:  74.4%
+-rw-rw-rw-  2.0 fat    18431 b- defN 23-Jul-15 09:29 pancollection-0.3.6.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    10387 b- defN 23-Jul-15 09:29 pancollection-0.3.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-15 09:29 pancollection-0.3.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       14 b- defN 23-Jul-15 09:29 pancollection-0.3.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     7253 b- defN 23-Jul-15 09:29 pancollection-0.3.6.dist-info/RECORD
+77 files, 425377 bytes uncompressed, 108305 bytes compressed:  74.5%
```

## zipnote {}

```diff
@@ -6,14 +6,17 @@
 
 Filename: pancollection/run_pansharpening.py
 Comment: 
 
 Filename: pancollection/run_test_pansharpening.py
 Comment: 
 
+Filename: pancollection/run_train_model.py
+Comment: 
+
 Filename: pancollection/common/__init__.py
 Comment: 
 
 Filename: pancollection/common/builder.py
 Comment: 
 
 Filename: pancollection/common/dataset.py
@@ -72,14 +75,17 @@
 
 Filename: pancollection/common/FS_index/my_q2n.py
 Comment: 
 
 Filename: pancollection/common/FS_index/tools.py
 Comment: 
 
+Filename: pancollection/common/tests/__init__.py
+Comment: 
+
 Filename: pancollection/configs/__init__.py
 Comment: 
 
 Filename: pancollection/configs/configs.py
 Comment: 
 
 Filename: pancollection/configs/hook_configs.py
@@ -144,17 +150,14 @@
 
 Filename: pancollection/models/DCFNet/__init__.py
 Comment: 
 
 Filename: pancollection/models/DCFNet/model_fcc_dense_head.py
 Comment: 
 
-Filename: pancollection/models/DHIFNet/__init__.py
-Comment: 
-
 Filename: pancollection/models/DRPNN/__init__.py
 Comment: 
 
 Filename: pancollection/models/DRPNN/drpnn_main.py
 Comment: 
 
 Filename: pancollection/models/DRPNN/model_drpnn.py
@@ -174,83 +177,29 @@
 
 Filename: pancollection/models/FusionNet/fusionnet_main.py
 Comment: 
 
 Filename: pancollection/models/FusionNet/model_fusionnet.py
 Comment: 
 
-Filename: pancollection/models/GPPNN/__init__.py
-Comment: 
-
-Filename: pancollection/models/GPPNN/metrics.py
-Comment: 
-
-Filename: pancollection/models/GPPNN/utils.py
-Comment: 
-
-Filename: pancollection/models/GPPNN/models/GPPNN.py
-Comment: 
-
-Filename: pancollection/models/GPPNN/models/__init__.py
-Comment: 
-
 Filename: pancollection/models/LAGConv/__init__.py
 Comment: 
 
-Filename: pancollection/models/LAGConv/data.py
-Comment: 
-
 Filename: pancollection/models/LAGConv/model.py
 Comment: 
 
-Filename: pancollection/models/LAGConv/test.py
-Comment: 
-
-Filename: pancollection/models/LAGConv/train.py
-Comment: 
-
 Filename: pancollection/models/MSDCNN/__init__.py
 Comment: 
 
 Filename: pancollection/models/MSDCNN/model_msdcnn.py
 Comment: 
 
 Filename: pancollection/models/MSDCNN/msdcnn_main.py
 Comment: 
 
-Filename: pancollection/models/MUCNN/__init__.py
-Comment: 
-
-Filename: pancollection/models/MUCNN/main_test_multi.py
-Comment: 
-
-Filename: pancollection/models/MUCNN/main_test_single.py
-Comment: 
-
-Filename: pancollection/models/MUCNN/train.py
-Comment: 
-
-Filename: pancollection/models/MUCNN/lib/__init__.py
-Comment: 
-
-Filename: pancollection/models/MUCNN/lib/data.py
-Comment: 
-
-Filename: pancollection/models/MUCNN/lib/datasets.py
-Comment: 
-
-Filename: pancollection/models/MUCNN/lib/evaluate.py
-Comment: 
-
-Filename: pancollection/models/MUCNN/lib/model.py
-Comment: 
-
-Filename: pancollection/models/MUCNN/lib/utils.py
-Comment: 
-
 Filename: pancollection/models/PNN/__init__.py
 Comment: 
 
 Filename: pancollection/models/PNN/model_pnn.py
 Comment: 
 
 Filename: pancollection/models/PNN/pnn_main.py
@@ -261,23 +210,23 @@
 
 Filename: pancollection/models/PanNet/model_pannet.py
 Comment: 
 
 Filename: pancollection/models/PanNet/pannet_main.py
 Comment: 
 
-Filename: pancollection-0.3.5.dist-info/LICENSE
+Filename: pancollection-0.3.6.dist-info/LICENSE
 Comment: 
 
-Filename: pancollection-0.3.5.dist-info/METADATA
+Filename: pancollection-0.3.6.dist-info/METADATA
 Comment: 
 
-Filename: pancollection-0.3.5.dist-info/WHEEL
+Filename: pancollection-0.3.6.dist-info/WHEEL
 Comment: 
 
-Filename: pancollection-0.3.5.dist-info/top_level.txt
+Filename: pancollection-0.3.6.dist-info/top_level.txt
 Comment: 
 
-Filename: pancollection-0.3.5.dist-info/RECORD
+Filename: pancollection-0.3.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pancollection/run_pansharpening.py

```diff
@@ -18,11 +18,11 @@
     # pan.trainer.main(cfg, pan.build_model, pan.getDataSession)
 
 if __name__ == '__main__':
     arch = 'FusionNet'
     dataset_name = 'gf2'
     cfg = dict(arch=arch, dataset_name=dataset_name, use_resume=False,
                       dataset={'train': 'gf2', 'valid': 'gf2', 'test': 'test_gf2_multiExm1.h5'},
-                      workflow=[('test', 1), ('train', 1)],  # ('valid', 1), ('test', 1),
+                      workflow=[('train', 1)],  # ('valid', 1), ('test', 1),
                       resume_from=r"".replace('\\', '/'),
-                      use_log_and_save=True)
+                      use_log=False, test='reduce', use_save=True)
     run_demo(**cfg)
```

## pancollection/common/builder.py

```diff
@@ -6,15 +6,15 @@
 import udl_vis.Basis.option
 
 def build_model(arch, task, cfg=None):
 
     if task == "pansharpening":
         from pancollection.models.base_model import PanSharpeningModel as MODELS
 
-        return MODELS.build_model(cfg)
+        return MODELS.build_model_from_task(cfg)
     else:
         raise NotImplementedError(f"It's not supported in {task}")
 
 
 def getDataSession(cfg):
 
     task = cfg.task
```

## pancollection/common/dataset.py

```diff
@@ -1,7 +1,8 @@
+import imageio
 import torch.utils.data as data
 import torch
 import h5py
 import cv2
 import numpy as np
 import os
 # import datetime
@@ -337,25 +338,33 @@
 
 def mpl_save_fig(filename):
     plt.savefig(f"{filename}", format='svg', dpi=300, pad_inches=0, bbox_inches='tight')
 
 
 def save_results(idx, save_model_output, filename, save_fmt, output):
     if filename is None:
-        save_name = os.path.join(f"{save_model_output}",
-                                 "output_mulExm_{}.mat".format(idx))
-        sio.savemat(save_name, {'sr': output.cpu().detach().numpy()})
+        filename = os.path.join(f"{save_model_output}",
+                                 f"output_mulExm_{idx}.{save_fmt}")
+        # sio.savemat(save_name, {'sr': output.cpu().detach().numpy()})
     else:
-        filename = os.path.basename(filename).split('.')[0]
         if save_fmt != 'mat':
-            output = showimage8(output)
+            filename = os.path.basename(filename).split('.')[0]
             filename = '/'.join([save_model_output, filename + ".png"])
-            # plt.imsave(filename, output, dpi=300)
-            show_region_images(output, xywh=[50, 100, 50, 50], #sub_width="20%", sub_height="20%",
-                               sub_ax_anchor=(0, 0, 1, 1))
-            mpl_save_fig(filename)
         else:
             filename = '/'.join([save_model_output, "output_" + filename + ".mat"])
-            sio.savemat(filename, {'sr': output.cpu().detach().numpy()})
 
+    if save_fmt != 'mat':
+        try:
+            output = showimage8(output)
+        except:
+            output = output[..., [0, 2, 4]].cpu().detach().numpy()
+        # filename = '/'.join([save_model_output, filename + ".png"])
+        # plt.imsave(filename, output, dpi=300)
+        # show_region_images(output, xywh=[50, 100, 50, 50],  # sub_width="20%", sub_height="20%",
+        #                    sub_ax_anchor=(0, 0, 1, 1))
+        # mpl_save_fig(filename)
+        imageio.imsave(filename, output)
+    else:
+        # filename = '/'.join([save_model_output, "output_" + filename + ".mat"])
+        sio.savemat(filename, {'sr': output.cpu().detach().numpy()})
```

## pancollection/common/evaluate.py

```diff
@@ -1,11 +1,12 @@
 import math
 import torch
 import torch.nn.functional as F
 import numpy as np
+from .FS_index.indexes_evaluation_FS import indexes_evaluation_FS
 
 
 # 由于dat及其方差等数值舍入存在误差，最终结果有0.001左右的误差
 def q2n(gt, x, q_blocks_size, q_shift):
     '''
     '''
     if isinstance(gt, torch.Tensor):
@@ -477,16 +478,61 @@
     # gs_filter = nn.Conv2d(1, 1, kernel_size=(3, 3))
     # gs_filter.weight.data = torch.tensor([[[[0,0,0],[0,1,0],[0,0,0]]]]).float()
     # print(gs_filter.weight)
     # a_t = torch.from_numpy(a).unsqueeze(0).unsqueeze(0).float()
     # a_t_pad = nn.functional.pad(a_t, pad=(1, 1, 1, 1), mode='replicate')
     # print(a_t_pad)
     # print(gs_filter())
-    from skimage.metrics import structural_similarity
+
+    import h5py
     from scipy import io as sio
-    I_HRMS = sio.loadmat('./I_HRMS.mat')['I_HRMS'] / 2047.0
-    I_GT = sio.loadmat('./I_GT.mat')['I_GT'] / 2047.0
-    print(structural_similarity(I_HRMS, I_GT, win_size=11, data_range=1, multichannel=True, gaussian_weights=True))
-    I_HRMS = torch.from_numpy(I_HRMS).unsqueeze(0).permute(0, 3, 1, 2).cuda()
-    I_GT = torch.from_numpy(I_GT).unsqueeze(0).permute(0, 3, 1, 2).cuda()
-    print(I_GT[0, 0, :5, :5])
-    print(torch.mean(_ssim(I_HRMS, I_GT)))
+
+    ################################################################################################################
+    #  |====PSNR(Inf)====|====SSIM(1)====|====Q(1)====|===Q_avg(1)===|=====SAM(0)=====|======ERGAS(0)=======|=======CC(1)=======|=======SCC(1)=======|=======RMSE(0)=======
+    #  FusionNet 39.2423 0.0000 0.9859 0.0000 0.6548 0.0000 0.5854 0.0000 2.0508 0.0000 4.2014 0.0000 0.9800 0.0000 0.9803 0.0000 0.0122 0.0000
+    ################################################################################################################
+    I_fusionnet = sio.loadmat("tests/wv3_fusionnet_reduce_0.mat")['sr']
+    I_fusionnet /= 2047.0
+    print(I_fusionnet.shape)
+    result_our = torch.from_numpy(I_fusionnet).float().cuda().clip(0, 1)
+
+    data = h5py.File(r"D:\Datasets\pansharpening\PanCollection\test_data\test_wv3_multiExm1.h5".replace('\\', '/'))
+    print(data.keys())
+    gt = np.asarray(data['gt']) / 2047.0
+    lms = np.asarray(data['lms']) / 2047.0
+    ms = np.asarray(data['ms']) / 2047.0
+    pan = np.asarray(data['pan']) / 2047.0
+    print(gt.shape, lms.shape, ms.shape, pan.shape)
+
+    gt = torch.from_numpy(gt).float().cuda()
+
+    Qblocks_size = 32;
+    dim_cut = 30
+    reduce_metrics = analysis_accu(gt[0].permute(1, 2, 0), result_our, 4, dim_cut=dim_cut)
+    print(reduce_metrics)
+
+    ################################################################################################################
+    #     |= == D_lambda_avg(0) == = |= == == D_s_avg(0) == == = |= == == =QNR(1) == == == =
+    #     FusionNet 0.0254 0.0000 0.0291 0.0000 0.9462 0.0000
+    ################################################################################################################
+
+    I_fusionnet = sio.loadmat("tests/wv3_fusionnet_full_0.mat")['sr']
+    result_our = I_fusionnet / 2047.0
+    print(result_our.shape)
+    # result_our = torch.from_numpy(I_fusionnet).float().cuda()
+
+    data = h5py.File(r"D:\Datasets\pansharpening\PanCollection\test_data\test_wv3_OrigScale_multiExm1.h5".replace('\\', '/'))
+    print(data.keys())
+    lms = np.asarray(data['lms']) / 2047.0
+    ms = np.asarray(data['ms']) / 2047.0
+    pan = np.asarray(data['pan']) / 2047.0
+    print(lms.shape, ms.shape, pan.shape)
+    L = 11
+    dim_cut = 21
+    # thvalues = 0
+    # pan = torch.from_numpy(pan).float().cuda()
+    # lms = torch.from_numpy(lms).float().cuda()
+    # ms = torch.from_numpy(ms).float().cuda()
+    full_metrics = indexes_evaluation_FS(I_F=result_our, I_MS_LR=ms[0].transpose(1, 2, 0), I_MS=lms[0].transpose(1, 2, 0), I_PAN=pan[0].transpose(1, 2, 0),
+                                         L=L, th_values=thvalues, sensor='wv3', ratio=4, Qblocks_size=32, flagQNR=1)
+
+    print(full_metrics)
```

## pancollection/common/FS_index/indexes_evaluation_FS.py

```diff
@@ -233,8 +233,33 @@
         I_F[I_F > 2 ** L] = 2 ** L
         I_F[I_F < 0] = 0
     if flagQNR:
         QNR_index, D_lambda, D_S = my_qnr(I_F, I_MS_LR, I_MS, I_PAN, ratio, Qblocks_size)
     else:
         QNR_index, D_lambda, D_S = HQNR(I_F, I_MS_LR, I_MS, I_PAN, Qblocks_size, sensor, ratio)
 
-    return QNR_index, D_lambda, D_S
+    return {"QNR": QNR_index, "D_lambda": D_lambda, "D_S": D_S}
+
+
+if __name__ == '__main__':
+    import h5py
+    import scipy.io as sio
+    import os
+
+    mat_path = "D:/Python/matlab_code/pansharpening/Pansharpening Toolbox for Distribution/hsp"
+
+    FR = sio.loadmat(os.path.join(mat_path, 'DatasetFR1.mat'))
+    I_GS = np.array(h5py.File(os.path.join(mat_path, 'I_GS.mat'), 'r')['I_GS']).transpose(2, 1, 0) / 65535.0
+
+    print(I_GS[:3, :3, 0])
+
+    I_MS_LR = FR['I_MS'].transpose(1, 0, 2) / 65535.0
+    I_PAN = FR['I_PAN'].transpose(1, 0) / 65535.0
+    print(I_GS.dtype, 2 ** 16 - 1)
+    print(I_GS.shape, type(I_GS), I_MS_LR.shape, type(I_MS_LR), I_PAN.shape, type(I_PAN))
+    # from_numpy仅支持float
+    I_GS, I_MS_LR, I_PAN = torch.from_numpy(I_GS)[:64, :64], torch.from_numpy(I_MS_LR)[:64, :64], torch.from_numpy(
+        I_PAN)[:64, :64]
+    I_GS = torch.tensor(I_GS, requires_grad=True)
+    print(I_GS.requires_grad)
+    metrics = QS(I_GS, I_MS_LR, None, I_PAN, ratio=6, S=4)
+    print(metrics)
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## pancollection/configs/configs.py

```diff
@@ -23,14 +23,15 @@
             cfg.data_dir = 'D:/Datasets/pansharpening'
 
         cfg.best_prec1 = 10000
         cfg.best_prec5 = 10000
         cfg.metrics = 'loss'
         cfg.task = "pansharpening"
         cfg.save_fmt = "mat" # fmt is mat or not mat
-        cfg.taskhead = "pansharpening"
+        # cfg.taskhead = "pansharpening"
+        cfg.test = "reduce"  # reduce/full experiment
         # * Importantly
         warning = f"Note: FusionNet, DiCNN, PNN don't have high-pass filter"
         warnings.warn(warning)
         if arch is not None:
             cfg = self.new(cfg=cfg, arch=cfg.arch, **kwargs)
         self.merge_from_dict(cfg)
```

## pancollection/models/base_model.py

```diff
@@ -5,15 +5,15 @@
 # @reference:
 import os
 
 from udl_vis.Basis.python_sub_class import ModelDispatcher
 import numpy as np
 import torch
 from torch.nn import functional as F
-from pancollection.common.evaluate import analysis_accu
+from pancollection.common.evaluate import analysis_accu, indexes_evaluation_FS
 from pancollection.common.dataset import save_results
 
 class PanSharpeningModel(ModelDispatcher, name='pansharpening'):
 
     _models = {}
 
     def __init__(self, model=None, criterion=None):
@@ -62,21 +62,30 @@
         if self.reg:
             return self.l2_regularization(loss_dict)
 
         return loss_dict
 
     def val_step(self, *args, **kwargs):
         sr, gt = self.model.val_step(*args, **kwargs)
-        result_our = torch.squeeze(sr).permute(1, 2, 0)
-        metrics = analysis_accu(gt.cuda().squeeze(0), result_our, 4)
-        if kwargs['test_mode']:
-            result_our = result_our * kwargs['img_range']
-            if kwargs['idx'] not in [220, 231, 236, 469, 766, 914]:
-                if kwargs['save_fmt'] is not None and os.path.isdir(kwargs['save_fmt']):
-                    save_results(kwargs['idx'], kwargs['save_dir'], kwargs['filename'], kwargs['save_fmt'], result_our)
-                self.SAM_list.append(metrics['SAM'].item())
-                self.ERGAS_list.append(metrics['ERGAS'].item())
-            if kwargs['idx'] == 1257:
-                print(np.mean(self.SAM_list), np.mean(self.ERGAS_list))
+        if not kwargs['test_mode']:
+            metrics = self.criterion(sr, gt)
+        else:
+            result_our = torch.squeeze(sr).permute(1, 2, 0)
+            if kwargs['test'] == "reduce":
+                metrics = analysis_accu(gt.cuda().squeeze(0), result_our, 4)
+                result_our = result_our * kwargs['img_range']
+                if kwargs['idx'] not in [220, 231, 236, 469, 766, 914]:
+                    if kwargs['save_fmt'] is not None and os.path.isdir(kwargs['save_fmt']):
+                        save_results(kwargs['idx'], kwargs['save_dir'], kwargs['filename'], kwargs['save_fmt'], result_our)
+                    self.SAM_list.append(metrics['SAM'].item())
+                    self.ERGAS_list.append(metrics['ERGAS'].item())
+                if kwargs['idx'] == 1257:
+                    print(np.mean(self.SAM_list), np.mean(self.ERGAS_list))
+            elif kwargs['test'] == 'full':
+                metrics = indexes_evaluation_FS(I_F=result_our.cpu().numpy(),
+                                                I_MS_LR=args[0]["ms"][0].permute(1, 2, 0).cpu().numpy(),
+                                                I_PAN=args[0]['pan'][0].permute(1, 2, 0).cpu().numpy(),
+                                                I_MS=args[0]["lms"][0].permute(1, 2, 0).cpu().numpy(),
+                                                L=11, th_values=0, sensor='wv3', ratio=4, Qblocks_size=32, flagQNR=1)
 
         return {'log_vars': metrics}
```

## Comparing `pancollection-0.3.5.dist-info/LICENSE` & `pancollection-0.3.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pancollection-0.3.5.dist-info/METADATA` & `pancollection-0.3.6.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pancollection
-Version: 0.3.5
+Version: 0.3.6
 Summary: PanCollection based on UDL (https://github.com/XiaoXiao-Woo/UDL)
 Home-page: https://github.com/XiaoXiao-Woo/PanCollection
 Author: XiaoXiao-Woo
 Author-email: wxwsx1997@gmail.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -22,19 +22,19 @@
 Requires-Dist: imageio
 Requires-Dist: colorlog
 Requires-Dist: scipy
 Requires-Dist: h5py
 Requires-Dist: regex
 Requires-Dist: packaging
 Requires-Dist: pyyaml
-Requires-Dist: udl-vis (==0.3.5)
+Requires-Dist: udl-vis
 
 <div>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<a href="https://github.com/liangjiandeng/DLPan-Toolbox"><img src="logo/logo-dlpan.png" width="250"></a>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<a href="PanCollection.html"><img src="logo/logo-collection.png" width="250"></a>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<a href="https://liangjiandeng.github.io/PanCollection.html"><img src="logo/logo-collection.png" width="250"></a>
 </div>
 
 
 # "PanCollection" for Remote Sensing Pansharpening (Make Available on [PyPI](https://pypi.org/project/pancollection/) :tada:)
 
 [English](https://github.com/XiaoXiao-Woo/PanCollection/edit/dev/README.md) | [简体中文](https://github.com/XiaoXiao-Woo/PanCollection/edit/dev/README_zh.md)
 
@@ -127,23 +127,51 @@
 
 	run_pansharpening.py
   
 	where arch='BDPN', and configs/option_bdpn.py has: 
   
 	__cfg.eval__ = False, 
   
-	__cfg.workflow__ = [('train', 50), ('val', 1)], __cfg.dataset__ = {'train': 'wv3', 'val': 'wv3_multiExm.h5'}
+	__cfg.workflow__ = [('train', 50), ('valid', 1)], __cfg.dataset__ = {'train': 'wv3', 'valid': 'wv3_multiExm.h5'}
 	
 * A test example:
 
 	run_test_pansharpening.py
   
-	__cfg.eval__ = True or __cfg.workflow__ = [('val', 1)]
+	__cfg.eval__ = True or __cfg.workflow__ = [('test', 1)]
 
-**Step4**. How to customize the code.
+**Step4.** How to customize your model.
+```pythonn
+def run_demo():
+    import os 
+    os.environ["CUDA_DEVICE_ORDER"] = "PCI_BUS_ID"
+    os.environ["CUDA_VISIBLE_DEVICES"] = "0"
+
+    from <your_model_file> import build
+    from pancollection.configs.configs import TaskDispatcher
+    from udl_vis.AutoDL.trainer import main
+    from pancollection.common.builder import build_model, getDataSession
+    import option_<your_model_file> # please refer to https://github.com/XiaoXiao-Woo/PanCollection/blob/main/pancollection/configs/option_fusionnet.py
+
+
+    cfg = TaskDispatcher.new(task='hisr', mode='entrypoint', arch='FCFormer', **data_path,
+                             workflow=[('train', 10), ('valid', 1), ('test', 1)], resume_from="", experimental_desc="LN")
+                            #  **data_path)
+                            #  , data_dir="/Data/Datasets/hisr")
+    print(TaskDispatcher._task.keys())
+
+    main(cfg, build_model, getDataSession)
+
+if __name__ == '__main__':
+    run_demo()
+
+```
+
+
+**Step5.** How to customize the code.
 
 One model is divided into three parts:
 
 1. Record hyperparameter configurations in folder of `PanCollection/UDL/pansharpening/configs/option_<modelName>.py`. For example, you can load pretrained model by setting __model_path__ = "your_model_path" or __cfg.resume_from__ = "your_model_path".
 
 2. Set model, loss, optimizer, scheduler in folder of `PanCollection/UDL/pansharpening/models/<modelName>_main.py`.
```

## Comparing `pancollection-0.3.5.dist-info/RECORD` & `pancollection-0.3.6.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,94 +1,77 @@
 pancollection/PanCollection_colab.ipynb,sha256=XgLdbOz4EzF5f1qpS5lvB4WU9CEe-iUAx6NtFZcNnbc,122081
 pancollection/__init__.py,sha256=zuUJQjADcBUSFImCqxrST1jY4jG6b4IBYXEFZwiBVyc,321
-pancollection/run_pansharpening.py,sha256=yY_JlA_Srqa0PpLXY8LjLQn6SgyOff1lBnki1VdNqy8,1178
+pancollection/run_pansharpening.py,sha256=oK9kOO-hA2FT0hOJOJCxv4ySx5h9seyQZBgaf-T-dQk,1187
 pancollection/run_test_pansharpening.py,sha256=2_KUI1FvNyp9MpadrqdGANSUmii7DJwjm0ooZRzWi6A,2805
+pancollection/run_train_model.py,sha256=k_i4i6wUYAznYJx75PebWbpwmkXHuRY4rM8WqGW_IeQ,2121
 pancollection/common/__init__.py,sha256=tlSAsIjH2j0riZdxQGCpnTx_aA6s-FEsKmZWl6jGz0U,72
-pancollection/common/builder.py,sha256=MlU832IJIn8dRxB8p8pXT_IYortHTdOuzwZl_HwtmDk,641
-pancollection/common/dataset.py,sha256=b5fuG7aIeEb0qH4McH3lJ-G7QQTSP6V4_DOENoBF24o,14450
+pancollection/common/builder.py,sha256=Ok9Ehbuerr6SNVLKLgBRuvlPkFl_mO3bE61SK2ZYlQY,651
+pancollection/common/dataset.py,sha256=BKvIeweQlIsRrT8pvq6YXmlCoyrftYnOzBAErJCg2mw,14791
 pancollection/common/dataset_hp.py,sha256=rT8EQyH0mcu-7fkJTkRtkbJKyD4EpcURar1q4ghdFQU,2238
-pancollection/common/evaluate.py,sha256=iu-Rd8hsvacrb-Evrc00lT2D0n9xpQASdiCN11FqBrw,16414
+pancollection/common/evaluate.py,sha256=jD1VXYigvDOthXwrreTmadJWo6n59OmiudKKaZ-O0N4,18749
 pancollection/common/psdata.py,sha256=-OcSI4N_gPfvngEPT8Bjk89Ubf-IyjXB7bKBs46jGKo,7372
 pancollection/common/test_panloader.py,sha256=scEDVzms_qJibPl3Ep9ZYtnJwh3Wc3EnYo-mBkfzOZ4,4959
 pancollection/common/train_panloader.py,sha256=aCgQdAogpuIBjsaA8pCIPA7sJLNTZfvQ25oqIjBHY_8,3833
 pancollection/common/valid_panloader.py,sha256=9SG7_DY7My59id7H1_1psPQcFLqvjI7cdeUBjM9uoTA,3833
 pancollection/common/FS_index/D_lambda_K.py,sha256=LPcHWMFyIWx0GN_Nf0HqI6rjnkrKn524v46wwsWUD_k,2320
 pancollection/common/FS_index/HQNR.py,sha256=L0FGJoKlu37kQErtGAPgeMnT1R1NcbDeXrC5zlYyt0U,2392
 pancollection/common/FS_index/MTF.py,sha256=0dP5ATdI-A8GNiFvHwjXfyZ2XR3FWdFHBSqn5wL3ufY,2213
 pancollection/common/FS_index/MTF_pan.py,sha256=eTlXpxv7fvYsJjPWZQkj9bNqrTSfmnXRYCUG58X0iH8,2224
 pancollection/common/FS_index/__init__.py,sha256=Lo8zWCest-2HvgTyeq09pKF5USrpjlLrtPP60RQIewE,113
 pancollection/common/FS_index/genMTF.py,sha256=B5IB3sZZGpju6eutKsAOOG5Wmzj2TNZbMgjJgKDrmBI,2593
 pancollection/common/FS_index/genMTF_pan.py,sha256=fFuogF887wISpMWhxK0Svlgzn4dyWE3FMi6nKNwnHLU,730
 pancollection/common/FS_index/imresize.py,sha256=Tlu7IbBmxW22wxMtnBcEVgLEMFAzd4ByuGx9vG9BQbY,5515
-pancollection/common/FS_index/indexes_evaluation_FS.py,sha256=EIf0A6s6pNlroLUlzL6xFNtgVEUZ9XndwYrenoiAxzg,9046
+pancollection/common/FS_index/indexes_evaluation_FS.py,sha256=by5EkqEWh6SYe_7euq_BGPCZyV4VDGIWM7zrEckJkw8,10043
 pancollection/common/FS_index/interp23.py,sha256=4tlcJ04AKRPTHnZdb2edN6T_S2M1P6HQqzH63Js1Tno,3106
 pancollection/common/FS_index/my_D_s.py,sha256=F37bvSbGKV0VSoJ9AyPoyApqfQ2wdbuOq_xth6NyUno,6354
 pancollection/common/FS_index/my_q2n.py,sha256=WSEGtB5GGYxEFEWWYTmaIhjqPQQiX2WaYl5smh4_Xks,8336
 pancollection/common/FS_index/tools.py,sha256=sgcidGg5Z27-91kBd4hf0RhxI4iBY3peGWZ2sSVT7UQ,1237
+pancollection/common/tests/__init__.py,sha256=VIWR-WSDIwYbYbaX0TxH7XfKsf7qr6atNz9nvftfqW8,136
 pancollection/configs/__init__.py,sha256=eGUAcZdOOEy5swXc_rfnH23A-cPKTB-bmPfIaUcGRF0,336
-pancollection/configs/configs.py,sha256=4Kii3-yemu5sQhhuYkmei2fw-rzMfU9l6JKdKftjYSU,1169
+pancollection/configs/configs.py,sha256=e6AMFe1wTKOFMfJt-1ZlI--HzcLvys5G-LsZdR2Uos0,1226
 pancollection/configs/hook_configs.py,sha256=RQ8wLKsEfNRqIs2d84CBoq9NFMAmxHdJva3kl3FhCOs,822
 pancollection/configs/load_ckpt_configs.py,sha256=YYkZobjW8wqaJYsvYOhQOlBGMwoojOB6qCRYffeF87U,846
 pancollection/configs/option_DCFNet.py,sha256=79WhIKb39hgvFjzHL1urzn0U2gzv-C_x2oVHhPlBMc8,3713
 pancollection/configs/option_LAGNet.py,sha256=Wi54tWPeTiTBZmOkz36XgsZb8zFKw1cZGaSzqaSsaTo,3740
 pancollection/configs/option_bdpn.py,sha256=xV5T5I2KK0FBNrAjdgPPVPwkcuE6XuGhhE50ThEW8wE,3625
 pancollection/configs/option_dicnn.py,sha256=GPhgiJJsQtH1N_fmtlrOxdXtIPBp3NWA4ISD87s9mI0,3537
 pancollection/configs/option_drpnn.py,sha256=IxB8ERFb0ZAXG763SJOHuT4I-8IT-dHVQ9CvIyXm2ak,3584
 pancollection/configs/option_fusionnet.py,sha256=LNj5zCKDb_6HZiT_vyMlQV0cgdllsGmJ4wCAJietCz0,4121
 pancollection/configs/option_msdcnn.py,sha256=3jdA-Iwb08IxO_n-TYQOJLI5ytbeafEtcAKOdq_Ul9A,3580
 pancollection/configs/option_pannet.py,sha256=MlKJ-5_QoGdl_Db5LButOUZjnKWHX19c4Bzhn0QQZWk,3748
 pancollection/configs/option_pnn.py,sha256=ywXI5yy_43WDw5-LKpYcBJHSbASNATmgVhfVcn1VT4k,3629
 pancollection/models/__init__.py,sha256=ZobBtlefgTUPLnpnskzZWmWZxRG2DQMrE3d_SBmweWk,508
-pancollection/models/base_model.py,sha256=ZZqC_fQfXNDyo7LM8eN6YOcO_5r-8-DgOlzj8j0VUn0,3005
+pancollection/models/base_model.py,sha256=GSn4Hyst6l_8KXsQCoI_rnyCXmK76LfrH6lznPfltEY,3738
 pancollection/models/ADKNet/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pancollection/models/ADKNet/ddf/__init__.py,sha256=eGMGQOZXq5OvVjT6uoiMh3g4wglgKi21ymYcCyU9xac,18
 pancollection/models/ADKNet/ddf/ddf.py,sha256=lw7HRcw9N5DwxJmSiUtTriYMiSrRC8x0VSyMPxCehL4,11638
 pancollection/models/ADKNet/ddf/setup.py,sha256=70wAtQjbqWqolNK7vwXmeg5db_J1mogT92nipumL3gU,2289
 pancollection/models/BDPN/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pancollection/models/BDPN/bdpn_main.py,sha256=XFPWnnxhGKl_8uQjQV5xOWeknZUXGMA7oDQy0RSzehg,3835
 pancollection/models/BDPN/model_bdpn.py,sha256=7jyLRAB3U9HvqrYgGzh3MauTlJEN3nESdsX9JgVLokw,7822
 pancollection/models/DCFNet/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pancollection/models/DCFNet/model_fcc_dense_head.py,sha256=tEGID-P4vqrCFOEoRS7tXBLdreAaJADQd_9vwzRUs4Q,32420
-pancollection/models/DHIFNet/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pancollection/models/DRPNN/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pancollection/models/DRPNN/drpnn_main.py,sha256=h8u-YdGGziDyLPQXgktEBJj_K59NzTFF9M_wxhRHkHc,3842
 pancollection/models/DRPNN/model_drpnn.py,sha256=MpUjT5BIKgt_sWytM46VtHJ5P42_mjCC7Mg8dMKxNog,5302
 pancollection/models/DiCNN/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pancollection/models/DiCNN/dicnn_main.py,sha256=fY6GnitntKGThujQ8k8ozKkF15WOifDxTOGXcKXxiF4,3816
 pancollection/models/DiCNN/model_dicnn.py,sha256=RKokIGnanVYhJyDWKY5eu8fbD4TOQ6QdcX_RvMOROzI,3768
 pancollection/models/FusionNet/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pancollection/models/FusionNet/fusionnet_main.py,sha256=WZzDtTFB3c8dJd-tHKkQzaenbsxHBU7lFKHpzoO4Hkc,3494
 pancollection/models/FusionNet/model_fusionnet.py,sha256=Nj3ct6wpTv0N4J5jQ9B8xs25x_4BvzgBfYekNb_BaGM,5615
-pancollection/models/GPPNN/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-pancollection/models/GPPNN/metrics.py,sha256=rdC0ExYo3wwRBWrM1XPFNFTSQZLRJHgCNrQ7LOCBJ2s,1644
-pancollection/models/GPPNN/utils.py,sha256=klptjjlHYfAMeHz0qLvz9JVoMWCRK_JRJECXENdQyt4,38742
-pancollection/models/GPPNN/models/GPPNN.py,sha256=EApQukaW-hNmciSNkxYBMpluK58QNpaOOsaOQyY771o,4902
-pancollection/models/GPPNN/models/__init__.py,sha256=r5pNfQSdmD9svUtu2MdBaQPtXMV51PnA5SkZE5ci0yM,686
 pancollection/models/LAGConv/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-pancollection/models/LAGConv/data.py,sha256=iH9WM7IMBIqJGnsDGnuuMN3Tocb465EsPxDR_cmyRio,2254
 pancollection/models/LAGConv/model.py,sha256=8zC1Be5ZLyhLBWsbcENqQXHWlwuo1juzECwvVE8v5sQ,6955
-pancollection/models/LAGConv/test.py,sha256=p3qI1FQjI6Qblf4wIjYERg_U8jlAZ4_AylPnLE9n4Mg,1990
-pancollection/models/LAGConv/train.py,sha256=Rs88e2OIQTxkvA1Y1aKz2IsTZsVGhprvqZe3PCV3uxQ,7423
 pancollection/models/MSDCNN/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pancollection/models/MSDCNN/model_msdcnn.py,sha256=IP_RZxwZnbmilibRVtfo-TyOZRGmRBz24sheR08Y33Q,5873
 pancollection/models/MSDCNN/msdcnn_main.py,sha256=KSMOK-Gn-xoB6sgDXq3Pboeboy49ay3L_9usVTftXWY,3831
-pancollection/models/MUCNN/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-pancollection/models/MUCNN/main_test_multi.py,sha256=wWD9KsWBMSdhSpEl2p8J_LdEP1iUVsHzA6g7ev_0JgQ,3395
-pancollection/models/MUCNN/main_test_single.py,sha256=ZMd2SIMCUhBChxB-Ax82t2e7bcHORXAPeYZaW-qPwjc,2670
-pancollection/models/MUCNN/train.py,sha256=JSTG8hT7zJhK_bHwFQxc1846fS8i8GzqwhpepkFY4V8,8936
-pancollection/models/MUCNN/lib/__init__.py,sha256=PAQPr1I_yy_ynpXTtgNJho6frqiGW9WoJLiTHKQ6z5A,81
-pancollection/models/MUCNN/lib/data.py,sha256=MRXE_ixrfJgKxNEOFtZDKGw8OHCfoefsVxr2_YUoENw,940
-pancollection/models/MUCNN/lib/datasets.py,sha256=qcXRs6xbk5fdyzrSlaoTff3Z9yqmdARkspCz8nAqzV0,3897
-pancollection/models/MUCNN/lib/evaluate.py,sha256=tkjxuv3i5au1R-jKYh99C8uCXERPosClVAgR8OHk0po,5410
-pancollection/models/MUCNN/lib/model.py,sha256=yL9dAXLTk7__gpNVwh76qOXk7X6vtw_0YCUoea9BzYc,3027
-pancollection/models/MUCNN/lib/utils.py,sha256=wmuEVvH4F154WeqJeTbYC8ZfBN2sqTDpqV5qqNUrhxI,1328
 pancollection/models/PNN/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pancollection/models/PNN/model_pnn.py,sha256=Xk8HATIPmyTMpNkC5HkUVZReGOwrgYe8m1gxXNpiSig,2530
 pancollection/models/PNN/pnn_main.py,sha256=zyXYpBQR6JKcHAYDajwOAPLtZR4uRCEKFGpgzXe3af4,4367
 pancollection/models/PanNet/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pancollection/models/PanNet/model_pannet.py,sha256=sq8yXk-wNbO-IXCE3lOcdKiNx9EQet38uo2pTyuxhTc,4917
 pancollection/models/PanNet/pannet_main.py,sha256=MQsZ8cIker5EzDnAeZ4iYSZc75WQBU_aFUC7VAh1fqg,3790
-pancollection-0.3.5.dist-info/LICENSE,sha256=GJsa-V1mEVHgVM6hDJGz11Tk3k0_7PsHTB-ylHb3Fns,18431
-pancollection-0.3.5.dist-info/METADATA,sha256=lR5Ir5LJpZLj8uHjaj8rM4zvagXfSGDWw2pdxdDSJ9M,9354
-pancollection-0.3.5.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-pancollection-0.3.5.dist-info/top_level.txt,sha256=OexPvY5eXk13PnljRMKndBbgTAv_qcHUA49FjnZnHwc,14
-pancollection-0.3.5.dist-info/RECORD,,
+pancollection-0.3.6.dist-info/LICENSE,sha256=GJsa-V1mEVHgVM6hDJGz11Tk3k0_7PsHTB-ylHb3Fns,18431
+pancollection-0.3.6.dist-info/METADATA,sha256=XEp88T0fhGArs3GCKrr7yhWrzTg8W8vRTueSLWbnGNA,10387
+pancollection-0.3.6.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+pancollection-0.3.6.dist-info/top_level.txt,sha256=OexPvY5eXk13PnljRMKndBbgTAv_qcHUA49FjnZnHwc,14
+pancollection-0.3.6.dist-info/RECORD,,
```

