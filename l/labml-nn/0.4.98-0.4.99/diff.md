# Comparing `tmp/labml-nn-0.4.98.tar.gz` & `tmp/labml-nn-0.4.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/labml-nn-0.4.98.tar", last modified: Sun May  9 08:41:13 2021, max compression
+gzip compressed data, was "dist/labml-nn-0.4.99.tar", last modified: Fri May 21 09:36:56 2021, max compression
```

## Comparing `labml-nn-0.4.98.tar` & `labml-nn-0.4.99.tar`

### file list

```diff
@@ -1,148 +1,152 @@
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-09 08:41:13.000000 labml-nn-0.4.98/
--rw-r--r--   0 varuna     (501) staff       (20)       19 2020-09-01 05:21:10.000000 labml-nn-0.4.98/MANIFEST.in
--rw-r--r--   0 varuna     (501) staff       (20)     6196 2021-05-09 08:41:13.000000 labml-nn-0.4.98/PKG-INFO
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-09 08:41:13.000000 labml-nn-0.4.98/labml_nn/
--rw-r--r--   0 varuna     (501) staff       (20)     3339 2021-05-07 12:57:39.000000 labml-nn-0.4.98/labml_nn/__init__.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-09 08:41:13.000000 labml-nn-0.4.98/labml_nn/activations/
--rw-r--r--   0 varuna     (501) staff       (20)       25 2021-01-25 12:02:08.000000 labml-nn-0.4.98/labml_nn/activations/__init__.py
--rw-r--r--   0 varuna     (501) staff       (20)      277 2021-02-02 04:58:22.000000 labml-nn-0.4.98/labml_nn/activations/swish.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-09 08:41:13.000000 labml-nn-0.4.98/labml_nn/capsule_networks/
--rw-r--r--   0 varuna     (501) staff       (20)     7602 2021-03-05 09:47:03.000000 labml-nn-0.4.98/labml_nn/capsule_networks/__init__.py
--rw-r--r--   0 varuna     (501) staff       (20)     6499 2021-02-14 15:15:53.000000 labml-nn-0.4.98/labml_nn/capsule_networks/mnist.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-09 08:41:13.000000 labml-nn-0.4.98/labml_nn/experiments/
--rw-r--r--   0 varuna     (501) staff       (20)        0 2020-12-28 04:20:26.000000 labml-nn-0.4.98/labml_nn/experiments/__init__.py
--rw-r--r--   0 varuna     (501) staff       (20)      355 2021-04-23 08:43:21.000000 labml-nn-0.4.98/labml_nn/experiments/cifar10.py
--rw-r--r--   0 varuna     (501) staff       (20)     3302 2021-02-01 09:11:54.000000 labml-nn-0.4.98/labml_nn/experiments/mnist.py
--rw-r--r--   0 varuna     (501) staff       (20)     9161 2021-01-24 04:05:07.000000 labml-nn-0.4.98/labml_nn/experiments/nlp_autoregression.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-09 08:41:13.000000 labml-nn-0.4.98/labml_nn/gan/
--rw-r--r--   0 varuna     (501) staff       (20)      330 2021-05-07 11:16:23.000000 labml-nn-0.4.98/labml_nn/gan/__init__.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-09 08:41:13.000000 labml-nn-0.4.98/labml_nn/gan/cycle_gan/
--rw-r--r--   0 varuna     (501) staff       (20)    28903 2021-05-07 11:16:23.000000 labml-nn-0.4.98/labml_nn/gan/cycle_gan/__init__.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-09 08:41:13.000000 labml-nn-0.4.98/labml_nn/gan/dcgan/
--rw-r--r--   0 varuna     (501) staff       (20)     3894 2021-05-07 11:16:23.000000 labml-nn-0.4.98/labml_nn/gan/dcgan/__init__.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-09 08:41:13.000000 labml-nn-0.4.98/labml_nn/gan/original/
--rw-r--r--   0 varuna     (501) staff       (20)     4927 2021-05-07 11:16:23.000000 labml-nn-0.4.98/labml_nn/gan/original/__init__.py
--rw-r--r--   0 varuna     (501) staff       (20)     7964 2021-05-09 08:36:43.000000 labml-nn-0.4.98/labml_nn/gan/original/experiment.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-09 08:41:13.000000 labml-nn-0.4.98/labml_nn/gan/wasserstein/
--rw-r--r--   0 varuna     (501) staff       (20)     4660 2021-05-09 05:53:14.000000 labml-nn-0.4.98/labml_nn/gan/wasserstein/__init__.py
--rw-r--r--   0 varuna     (501) staff       (20)     1352 2021-05-07 11:16:23.000000 labml-nn-0.4.98/labml_nn/gan/wasserstein/experiment.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-09 08:41:13.000000 labml-nn-0.4.98/labml_nn/gan/wasserstein/gradient_penalty/
--rw-r--r--   0 varuna     (501) staff       (20)     2822 2021-05-09 08:21:42.000000 labml-nn-0.4.98/labml_nn/gan/wasserstein/gradient_penalty/__init__.py
--rw-r--r--   0 varuna     (501) staff       (20)     2780 2021-05-09 08:37:36.000000 labml-nn-0.4.98/labml_nn/gan/wasserstein/gradient_penalty/experiment.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-09 08:41:13.000000 labml-nn-0.4.98/labml_nn/hypernetworks/
--rw-r--r--   0 varuna     (501) staff       (20)      160 2021-01-03 05:35:36.000000 labml-nn-0.4.98/labml_nn/hypernetworks/__init__.py
--rw-r--r--   0 varuna     (501) staff       (20)     2825 2021-01-21 02:54:28.000000 labml-nn-0.4.98/labml_nn/hypernetworks/experiment.py
--rw-r--r--   0 varuna     (501) staff       (20)    11635 2021-02-27 12:23:37.000000 labml-nn-0.4.98/labml_nn/hypernetworks/hyper_lstm.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-09 08:41:13.000000 labml-nn-0.4.98/labml_nn/lstm/
--rw-r--r--   0 varuna     (501) staff       (20)     5993 2021-02-12 09:10:24.000000 labml-nn-0.4.98/labml_nn/lstm/__init__.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-09 08:41:13.000000 labml-nn-0.4.98/labml_nn/normalization/
--rw-r--r--   0 varuna     (501) staff       (20)      468 2021-04-28 06:39:53.000000 labml-nn-0.4.98/labml_nn/normalization/__init__.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-09 08:41:13.000000 labml-nn-0.4.98/labml_nn/normalization/batch_channel_norm/
--rw-r--r--   0 varuna     (501) staff       (20)    10021 2021-04-28 05:15:06.000000 labml-nn-0.4.98/labml_nn/normalization/batch_channel_norm/__init__.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-09 08:41:13.000000 labml-nn-0.4.98/labml_nn/normalization/batch_norm/
--rw-r--r--   0 varuna     (501) staff       (20)     9671 2021-02-27 12:23:43.000000 labml-nn-0.4.98/labml_nn/normalization/batch_norm/__init__.py
--rw-r--r--   0 varuna     (501) staff       (20)     1876 2021-04-23 08:43:21.000000 labml-nn-0.4.98/labml_nn/normalization/batch_norm/cifar10.py
--rw-r--r--   0 varuna     (501) staff       (20)     2425 2021-02-01 09:25:35.000000 labml-nn-0.4.98/labml_nn/normalization/batch_norm/mnist.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-09 08:41:13.000000 labml-nn-0.4.98/labml_nn/normalization/group_norm/
--rw-r--r--   0 varuna     (501) staff       (20)     6451 2021-04-28 05:15:06.000000 labml-nn-0.4.98/labml_nn/normalization/group_norm/__init__.py
--rw-r--r--   0 varuna     (501) staff       (20)     2308 2021-04-24 09:21:04.000000 labml-nn-0.4.98/labml_nn/normalization/group_norm/experiment.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-09 08:41:13.000000 labml-nn-0.4.98/labml_nn/normalization/instance_norm/
--rw-r--r--   0 varuna     (501) staff       (20)     4232 2021-04-23 09:40:56.000000 labml-nn-0.4.98/labml_nn/normalization/instance_norm/__init__.py
--rw-r--r--   0 varuna     (501) staff       (20)     2444 2021-04-24 09:20:12.000000 labml-nn-0.4.98/labml_nn/normalization/instance_norm/experiment.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-09 08:41:13.000000 labml-nn-0.4.98/labml_nn/normalization/layer_norm/
--rw-r--r--   0 varuna     (501) staff       (20)     5224 2021-04-23 08:43:21.000000 labml-nn-0.4.98/labml_nn/normalization/layer_norm/__init__.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-09 08:41:13.000000 labml-nn-0.4.98/labml_nn/normalization/weight_standardization/
--rw-r--r--   0 varuna     (501) staff       (20)     3783 2021-04-28 05:15:06.000000 labml-nn-0.4.98/labml_nn/normalization/weight_standardization/__init__.py
--rw-r--r--   0 varuna     (501) staff       (20)     1879 2021-04-28 05:15:06.000000 labml-nn-0.4.98/labml_nn/normalization/weight_standardization/conv2d.py
--rw-r--r--   0 varuna     (501) staff       (20)     2233 2021-04-28 05:15:06.000000 labml-nn-0.4.98/labml_nn/normalization/weight_standardization/experiment.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-09 08:41:13.000000 labml-nn-0.4.98/labml_nn/optimizers/
--rw-r--r--   0 varuna     (501) staff       (20)     8120 2021-01-14 01:31:38.000000 labml-nn-0.4.98/labml_nn/optimizers/__init__.py
--rw-r--r--   0 varuna     (501) staff       (20)     6777 2021-01-30 08:02:55.000000 labml-nn-0.4.98/labml_nn/optimizers/ada_belief.py
--rw-r--r--   0 varuna     (501) staff       (20)     8609 2021-01-30 11:54:24.000000 labml-nn-0.4.98/labml_nn/optimizers/adam.py
--rw-r--r--   0 varuna     (501) staff       (20)     2301 2021-01-14 01:31:38.000000 labml-nn-0.4.98/labml_nn/optimizers/adam_warmup.py
--rw-r--r--   0 varuna     (501) staff       (20)     3679 2021-01-14 04:00:24.000000 labml-nn-0.4.98/labml_nn/optimizers/adam_warmup_cosine_decay.py
--rw-r--r--   0 varuna     (501) staff       (20)     8028 2021-02-27 12:23:53.000000 labml-nn-0.4.98/labml_nn/optimizers/amsgrad.py
--rw-r--r--   0 varuna     (501) staff       (20)     4749 2021-01-14 03:58:27.000000 labml-nn-0.4.98/labml_nn/optimizers/configs.py
--rw-r--r--   0 varuna     (501) staff       (20)     4063 2021-02-02 04:57:52.000000 labml-nn-0.4.98/labml_nn/optimizers/mnist_experiment.py
--rw-r--r--   0 varuna     (501) staff       (20)     3380 2021-01-30 08:03:27.000000 labml-nn-0.4.98/labml_nn/optimizers/noam.py
--rw-r--r--   0 varuna     (501) staff       (20)     1608 2020-12-10 03:00:57.000000 labml-nn-0.4.98/labml_nn/optimizers/performance_test.py
--rw-r--r--   0 varuna     (501) staff       (20)    11246 2021-01-30 08:03:44.000000 labml-nn-0.4.98/labml_nn/optimizers/radam.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-09 08:41:13.000000 labml-nn-0.4.98/labml_nn/recurrent_highway_networks/
--rw-r--r--   0 varuna     (501) staff       (20)     5688 2021-02-11 02:23:36.000000 labml-nn-0.4.98/labml_nn/recurrent_highway_networks/__init__.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-09 08:41:13.000000 labml-nn-0.4.98/labml_nn/resnets/
--rw-r--r--   0 varuna     (501) staff       (20)        0 2021-02-27 12:12:33.000000 labml-nn-0.4.98/labml_nn/resnets/__init__.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-09 08:41:13.000000 labml-nn-0.4.98/labml_nn/resnets/models/
--rw-r--r--   0 varuna     (501) staff       (20)        0 2021-02-27 12:12:33.000000 labml-nn-0.4.98/labml_nn/resnets/models/__init__.py
--rw-r--r--   0 varuna     (501) staff       (20)     2695 2021-02-27 12:12:33.000000 labml-nn-0.4.98/labml_nn/resnets/models/mlp.py
--rw-r--r--   0 varuna     (501) staff       (20)     6659 2021-02-27 12:12:33.000000 labml-nn-0.4.98/labml_nn/resnets/models/resnet.py
--rwxr-xr-x   0 varuna     (501) staff       (20)     2160 2021-02-27 12:12:33.000000 labml-nn-0.4.98/labml_nn/resnets/pretrained_nets.py
--rwxr-xr-x   0 varuna     (501) staff       (20)     2513 2021-02-27 12:12:33.000000 labml-nn-0.4.98/labml_nn/resnets/resnet_net.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-09 08:41:13.000000 labml-nn-0.4.98/labml_nn/resnets/utils/
--rw-r--r--   0 varuna     (501) staff       (20)        0 2021-02-27 12:12:33.000000 labml-nn-0.4.98/labml_nn/resnets/utils/__init__.py
--rw-r--r--   0 varuna     (501) staff       (20)      546 2021-02-27 12:12:33.000000 labml-nn-0.4.98/labml_nn/resnets/utils/labelsmoothing.py
--rw-r--r--   0 varuna     (501) staff       (20)     4027 2021-02-27 12:12:33.000000 labml-nn-0.4.98/labml_nn/resnets/utils/train.py
--rw-r--r--   0 varuna     (501) staff       (20)     2227 2021-02-27 12:12:33.000000 labml-nn-0.4.98/labml_nn/resnets/utils/utils.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-09 08:41:13.000000 labml-nn-0.4.98/labml_nn/rl/
--rw-r--r--   0 varuna     (501) staff       (20)      826 2020-12-10 03:09:36.000000 labml-nn-0.4.98/labml_nn/rl/__init__.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-09 08:41:13.000000 labml-nn-0.4.98/labml_nn/rl/dqn/
--rw-r--r--   0 varuna     (501) staff       (20)     6294 2021-04-04 07:52:03.000000 labml-nn-0.4.98/labml_nn/rl/dqn/__init__.py
--rw-r--r--   0 varuna     (501) staff       (20)     9352 2021-04-04 07:52:03.000000 labml-nn-0.4.98/labml_nn/rl/dqn/experiment.py
--rw-r--r--   0 varuna     (501) staff       (20)     3281 2020-12-10 03:05:06.000000 labml-nn-0.4.98/labml_nn/rl/dqn/model.py
--rw-r--r--   0 varuna     (501) staff       (20)     9787 2020-12-10 03:05:47.000000 labml-nn-0.4.98/labml_nn/rl/dqn/replay_buffer.py
--rw-r--r--   0 varuna     (501) staff       (20)     4657 2020-12-10 03:10:08.000000 labml-nn-0.4.98/labml_nn/rl/game.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-09 08:41:13.000000 labml-nn-0.4.98/labml_nn/rl/ppo/
--rw-r--r--   0 varuna     (501) staff       (20)     7536 2021-03-30 06:58:44.000000 labml-nn-0.4.98/labml_nn/rl/ppo/__init__.py
--rw-r--r--   0 varuna     (501) staff       (20)    15285 2021-04-06 07:31:30.000000 labml-nn-0.4.98/labml_nn/rl/ppo/experiment.py
--rw-r--r--   0 varuna     (501) staff       (20)     3032 2021-03-30 06:56:12.000000 labml-nn-0.4.98/labml_nn/rl/ppo/gae.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-09 08:41:13.000000 labml-nn-0.4.98/labml_nn/sketch_rnn/
--rw-r--r--   0 varuna     (501) staff       (20)    25112 2021-03-04 16:11:46.000000 labml-nn-0.4.98/labml_nn/sketch_rnn/__init__.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-09 08:41:13.000000 labml-nn-0.4.98/labml_nn/transformers/
--rw-r--r--   0 varuna     (501) staff       (20)     2390 2021-03-14 02:47:06.000000 labml-nn-0.4.98/labml_nn/transformers/__init__.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-09 08:41:13.000000 labml-nn-0.4.98/labml_nn/transformers/compressive/
--rw-r--r--   0 varuna     (501) staff       (20)    13740 2021-02-27 12:23:59.000000 labml-nn-0.4.98/labml_nn/transformers/compressive/__init__.py
--rw-r--r--   0 varuna     (501) staff       (20)    13020 2021-02-19 09:22:47.000000 labml-nn-0.4.98/labml_nn/transformers/compressive/experiment.py
--rw-r--r--   0 varuna     (501) staff       (20)    10324 2021-02-05 13:40:08.000000 labml-nn-0.4.98/labml_nn/transformers/configs.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-09 08:41:13.000000 labml-nn-0.4.98/labml_nn/transformers/fast_weights/
--rw-r--r--   0 varuna     (501) staff       (20)    12990 2021-03-14 02:45:31.000000 labml-nn-0.4.98/labml_nn/transformers/fast_weights/__init__.py
--rw-r--r--   0 varuna     (501) staff       (20)     3832 2021-03-14 02:31:53.000000 labml-nn-0.4.98/labml_nn/transformers/fast_weights/experiment.py
--rw-r--r--   0 varuna     (501) staff       (20)     4216 2021-03-11 12:33:58.000000 labml-nn-0.4.98/labml_nn/transformers/fast_weights/token_wise.py
--rw-r--r--   0 varuna     (501) staff       (20)     3582 2021-02-02 04:49:08.000000 labml-nn-0.4.98/labml_nn/transformers/feed_forward.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-09 08:41:13.000000 labml-nn-0.4.98/labml_nn/transformers/feedback/
--rw-r--r--   0 varuna     (501) staff       (20)    19846 2021-03-27 06:07:13.000000 labml-nn-0.4.98/labml_nn/transformers/feedback/__init__.py
--rw-r--r--   0 varuna     (501) staff       (20)     4885 2021-02-27 12:25:00.000000 labml-nn-0.4.98/labml_nn/transformers/feedback/experiment.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-09 08:41:13.000000 labml-nn-0.4.98/labml_nn/transformers/glu_variants/
--rw-r--r--   0 varuna     (501) staff       (20)      359 2021-01-26 11:34:04.000000 labml-nn-0.4.98/labml_nn/transformers/glu_variants/__init__.py
--rw-r--r--   0 varuna     (501) staff       (20)     4296 2021-02-02 04:50:55.000000 labml-nn-0.4.98/labml_nn/transformers/glu_variants/experiment.py
--rw-r--r--   0 varuna     (501) staff       (20)    11935 2021-02-27 12:25:25.000000 labml-nn-0.4.98/labml_nn/transformers/glu_variants/simple.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-09 08:41:13.000000 labml-nn-0.4.98/labml_nn/transformers/gpt/
--rw-r--r--   0 varuna     (501) staff       (20)     8665 2021-02-27 12:25:42.000000 labml-nn-0.4.98/labml_nn/transformers/gpt/__init__.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-09 08:41:13.000000 labml-nn-0.4.98/labml_nn/transformers/knn/
--rw-r--r--   0 varuna     (501) staff       (20)     1934 2021-01-30 08:04:58.000000 labml-nn-0.4.98/labml_nn/transformers/knn/__init__.py
--rw-r--r--   0 varuna     (501) staff       (20)     5712 2020-12-10 04:21:43.000000 labml-nn-0.4.98/labml_nn/transformers/knn/build_index.py
--rw-r--r--   0 varuna     (501) staff       (20)     5907 2020-12-10 04:22:41.000000 labml-nn-0.4.98/labml_nn/transformers/knn/eval_knn.py
--rw-r--r--   0 varuna     (501) staff       (20)     4481 2021-02-02 04:51:44.000000 labml-nn-0.4.98/labml_nn/transformers/knn/train_model.py
--rw-r--r--   0 varuna     (501) staff       (20)     2210 2021-02-02 04:49:26.000000 labml-nn-0.4.98/labml_nn/transformers/label_smoothing_loss.py
--rw-r--r--   0 varuna     (501) staff       (20)     6738 2021-04-23 08:46:41.000000 labml-nn-0.4.98/labml_nn/transformers/mha.py
--rw-r--r--   0 varuna     (501) staff       (20)     8006 2021-02-07 09:35:46.000000 labml-nn-0.4.98/labml_nn/transformers/models.py
--rw-r--r--   0 varuna     (501) staff       (20)     2327 2021-02-02 04:50:07.000000 labml-nn-0.4.98/labml_nn/transformers/positional_encoding.py
--rw-r--r--   0 varuna     (501) staff       (20)      187 2021-02-05 13:40:08.000000 labml-nn-0.4.98/labml_nn/transformers/relative_mha.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-09 08:41:13.000000 labml-nn-0.4.98/labml_nn/transformers/switch/
--rw-r--r--   0 varuna     (501) staff       (20)     9937 2021-02-27 12:25:54.000000 labml-nn-0.4.98/labml_nn/transformers/switch/__init__.py
--rw-r--r--   0 varuna     (501) staff       (20)     8189 2021-02-02 04:52:08.000000 labml-nn-0.4.98/labml_nn/transformers/switch/experiment.py
--rw-r--r--   0 varuna     (501) staff       (20)      538 2021-02-05 13:40:08.000000 labml-nn-0.4.98/labml_nn/transformers/utils.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-09 08:41:13.000000 labml-nn-0.4.98/labml_nn/transformers/xl/
--rw-r--r--   0 varuna     (501) staff       (20)     5422 2021-02-27 12:26:06.000000 labml-nn-0.4.98/labml_nn/transformers/xl/__init__.py
--rw-r--r--   0 varuna     (501) staff       (20)     8779 2021-02-07 10:15:28.000000 labml-nn-0.4.98/labml_nn/transformers/xl/experiment.py
--rw-r--r--   0 varuna     (501) staff       (20)     6230 2021-02-07 09:32:13.000000 labml-nn-0.4.98/labml_nn/transformers/xl/relative_mha.py
--rw-r--r--   0 varuna     (501) staff       (20)      373 2021-02-17 11:47:38.000000 labml-nn-0.4.98/labml_nn/utils.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-09 08:41:13.000000 labml-nn-0.4.98/labml_nn.egg-info/
--rw-r--r--   0 varuna     (501) staff       (20)     6196 2021-05-09 08:41:13.000000 labml-nn-0.4.98/labml_nn.egg-info/PKG-INFO
--rw-r--r--   0 varuna     (501) staff       (20)     3871 2021-05-09 08:41:13.000000 labml-nn-0.4.98/labml_nn.egg-info/SOURCES.txt
--rw-r--r--   0 varuna     (501) staff       (20)        1 2021-05-09 08:41:13.000000 labml-nn-0.4.98/labml_nn.egg-info/dependency_links.txt
--rw-r--r--   0 varuna     (501) staff       (20)       56 2021-05-09 08:41:13.000000 labml-nn-0.4.98/labml_nn.egg-info/requires.txt
--rw-r--r--   0 varuna     (501) staff       (20)       15 2021-05-09 08:41:13.000000 labml-nn-0.4.98/labml_nn.egg-info/top_level.txt
--rw-r--r--   0 varuna     (501) staff       (20)       38 2021-05-09 08:41:13.000000 labml-nn-0.4.98/setup.cfg
--rw-r--r--   0 varuna     (501) staff       (20)     1676 2021-05-09 08:40:44.000000 labml-nn-0.4.98/setup.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-09 08:41:13.000000 labml-nn-0.4.98/utils/
--rw-r--r--   0 varuna     (501) staff       (20)        0 2021-01-27 03:27:09.000000 labml-nn-0.4.98/utils/__init__.py
--rw-r--r--   0 varuna     (501) staff       (20)     1424 2021-01-27 03:48:30.000000 labml-nn-0.4.98/utils/sitemap.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-21 09:36:56.000000 labml-nn-0.4.99/
+-rw-r--r--   0 varuna     (501) staff       (20)       19 2020-09-01 05:21:10.000000 labml-nn-0.4.99/MANIFEST.in
+-rw-r--r--   0 varuna     (501) staff       (20)     6380 2021-05-21 09:36:56.000000 labml-nn-0.4.99/PKG-INFO
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-21 09:36:56.000000 labml-nn-0.4.99/labml_nn/
+-rw-r--r--   0 varuna     (501) staff       (20)     3467 2021-05-21 09:31:47.000000 labml-nn-0.4.99/labml_nn/__init__.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-21 09:36:56.000000 labml-nn-0.4.99/labml_nn/activations/
+-rw-r--r--   0 varuna     (501) staff       (20)       25 2021-01-25 12:02:08.000000 labml-nn-0.4.99/labml_nn/activations/__init__.py
+-rw-r--r--   0 varuna     (501) staff       (20)      277 2021-02-02 04:58:22.000000 labml-nn-0.4.99/labml_nn/activations/swish.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-21 09:36:56.000000 labml-nn-0.4.99/labml_nn/capsule_networks/
+-rw-r--r--   0 varuna     (501) staff       (20)     7602 2021-03-05 09:47:03.000000 labml-nn-0.4.99/labml_nn/capsule_networks/__init__.py
+-rw-r--r--   0 varuna     (501) staff       (20)     6499 2021-02-14 15:15:53.000000 labml-nn-0.4.99/labml_nn/capsule_networks/mnist.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-21 09:36:56.000000 labml-nn-0.4.99/labml_nn/experiments/
+-rw-r--r--   0 varuna     (501) staff       (20)        0 2020-12-28 04:20:26.000000 labml-nn-0.4.99/labml_nn/experiments/__init__.py
+-rw-r--r--   0 varuna     (501) staff       (20)      355 2021-04-23 08:43:21.000000 labml-nn-0.4.99/labml_nn/experiments/cifar10.py
+-rw-r--r--   0 varuna     (501) staff       (20)     3302 2021-02-01 09:11:54.000000 labml-nn-0.4.99/labml_nn/experiments/mnist.py
+-rw-r--r--   0 varuna     (501) staff       (20)     9161 2021-01-24 04:05:07.000000 labml-nn-0.4.99/labml_nn/experiments/nlp_autoregression.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-21 09:36:56.000000 labml-nn-0.4.99/labml_nn/gan/
+-rw-r--r--   0 varuna     (501) staff       (20)      450 2021-05-21 09:31:24.000000 labml-nn-0.4.99/labml_nn/gan/__init__.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-21 09:36:56.000000 labml-nn-0.4.99/labml_nn/gan/cycle_gan/
+-rw-r--r--   0 varuna     (501) staff       (20)    28903 2021-05-07 11:16:23.000000 labml-nn-0.4.99/labml_nn/gan/cycle_gan/__init__.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-21 09:36:56.000000 labml-nn-0.4.99/labml_nn/gan/dcgan/
+-rw-r--r--   0 varuna     (501) staff       (20)     3894 2021-05-07 11:16:23.000000 labml-nn-0.4.99/labml_nn/gan/dcgan/__init__.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-21 09:36:56.000000 labml-nn-0.4.99/labml_nn/gan/original/
+-rw-r--r--   0 varuna     (501) staff       (20)     4927 2021-05-07 11:16:23.000000 labml-nn-0.4.99/labml_nn/gan/original/__init__.py
+-rw-r--r--   0 varuna     (501) staff       (20)     7964 2021-05-09 10:10:25.000000 labml-nn-0.4.99/labml_nn/gan/original/experiment.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-21 09:36:56.000000 labml-nn-0.4.99/labml_nn/gan/stylegan/
+-rw-r--r--   0 varuna     (501) staff       (20)    36594 2021-05-21 09:29:30.000000 labml-nn-0.4.99/labml_nn/gan/stylegan/__init__.py
+-rw-r--r--   0 varuna     (501) staff       (20)    17577 2021-05-21 09:29:30.000000 labml-nn-0.4.99/labml_nn/gan/stylegan/experiment.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-21 09:36:56.000000 labml-nn-0.4.99/labml_nn/gan/wasserstein/
+-rw-r--r--   0 varuna     (501) staff       (20)     4660 2021-05-09 10:10:25.000000 labml-nn-0.4.99/labml_nn/gan/wasserstein/__init__.py
+-rw-r--r--   0 varuna     (501) staff       (20)     1352 2021-05-07 11:16:23.000000 labml-nn-0.4.99/labml_nn/gan/wasserstein/experiment.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-21 09:36:56.000000 labml-nn-0.4.99/labml_nn/gan/wasserstein/gradient_penalty/
+-rw-r--r--   0 varuna     (501) staff       (20)     2822 2021-05-09 10:10:25.000000 labml-nn-0.4.99/labml_nn/gan/wasserstein/gradient_penalty/__init__.py
+-rw-r--r--   0 varuna     (501) staff       (20)     2780 2021-05-09 10:10:25.000000 labml-nn-0.4.99/labml_nn/gan/wasserstein/gradient_penalty/experiment.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-21 09:36:56.000000 labml-nn-0.4.99/labml_nn/hypernetworks/
+-rw-r--r--   0 varuna     (501) staff       (20)      160 2021-01-03 05:35:36.000000 labml-nn-0.4.99/labml_nn/hypernetworks/__init__.py
+-rw-r--r--   0 varuna     (501) staff       (20)     2825 2021-01-21 02:54:28.000000 labml-nn-0.4.99/labml_nn/hypernetworks/experiment.py
+-rw-r--r--   0 varuna     (501) staff       (20)    11635 2021-02-27 12:23:37.000000 labml-nn-0.4.99/labml_nn/hypernetworks/hyper_lstm.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-21 09:36:56.000000 labml-nn-0.4.99/labml_nn/lstm/
+-rw-r--r--   0 varuna     (501) staff       (20)     5993 2021-02-12 09:10:24.000000 labml-nn-0.4.99/labml_nn/lstm/__init__.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-21 09:36:56.000000 labml-nn-0.4.99/labml_nn/normalization/
+-rw-r--r--   0 varuna     (501) staff       (20)      468 2021-04-28 06:39:53.000000 labml-nn-0.4.99/labml_nn/normalization/__init__.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-21 09:36:56.000000 labml-nn-0.4.99/labml_nn/normalization/batch_channel_norm/
+-rw-r--r--   0 varuna     (501) staff       (20)    10021 2021-04-28 05:15:06.000000 labml-nn-0.4.99/labml_nn/normalization/batch_channel_norm/__init__.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-21 09:36:56.000000 labml-nn-0.4.99/labml_nn/normalization/batch_norm/
+-rw-r--r--   0 varuna     (501) staff       (20)     9671 2021-02-27 12:23:43.000000 labml-nn-0.4.99/labml_nn/normalization/batch_norm/__init__.py
+-rw-r--r--   0 varuna     (501) staff       (20)     1876 2021-04-23 08:43:21.000000 labml-nn-0.4.99/labml_nn/normalization/batch_norm/cifar10.py
+-rw-r--r--   0 varuna     (501) staff       (20)     2425 2021-02-01 09:25:35.000000 labml-nn-0.4.99/labml_nn/normalization/batch_norm/mnist.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-21 09:36:56.000000 labml-nn-0.4.99/labml_nn/normalization/group_norm/
+-rw-r--r--   0 varuna     (501) staff       (20)     6451 2021-04-28 05:15:06.000000 labml-nn-0.4.99/labml_nn/normalization/group_norm/__init__.py
+-rw-r--r--   0 varuna     (501) staff       (20)     2308 2021-04-24 09:21:04.000000 labml-nn-0.4.99/labml_nn/normalization/group_norm/experiment.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-21 09:36:56.000000 labml-nn-0.4.99/labml_nn/normalization/instance_norm/
+-rw-r--r--   0 varuna     (501) staff       (20)     4232 2021-04-23 09:40:56.000000 labml-nn-0.4.99/labml_nn/normalization/instance_norm/__init__.py
+-rw-r--r--   0 varuna     (501) staff       (20)     2444 2021-04-24 09:20:12.000000 labml-nn-0.4.99/labml_nn/normalization/instance_norm/experiment.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-21 09:36:56.000000 labml-nn-0.4.99/labml_nn/normalization/layer_norm/
+-rw-r--r--   0 varuna     (501) staff       (20)     5224 2021-04-23 08:43:21.000000 labml-nn-0.4.99/labml_nn/normalization/layer_norm/__init__.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-21 09:36:56.000000 labml-nn-0.4.99/labml_nn/normalization/weight_standardization/
+-rw-r--r--   0 varuna     (501) staff       (20)     3783 2021-04-28 05:15:06.000000 labml-nn-0.4.99/labml_nn/normalization/weight_standardization/__init__.py
+-rw-r--r--   0 varuna     (501) staff       (20)     1879 2021-04-28 05:15:06.000000 labml-nn-0.4.99/labml_nn/normalization/weight_standardization/conv2d.py
+-rw-r--r--   0 varuna     (501) staff       (20)     2233 2021-04-28 05:15:06.000000 labml-nn-0.4.99/labml_nn/normalization/weight_standardization/experiment.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-21 09:36:56.000000 labml-nn-0.4.99/labml_nn/optimizers/
+-rw-r--r--   0 varuna     (501) staff       (20)     8120 2021-01-14 01:31:38.000000 labml-nn-0.4.99/labml_nn/optimizers/__init__.py
+-rw-r--r--   0 varuna     (501) staff       (20)     6777 2021-01-30 08:02:55.000000 labml-nn-0.4.99/labml_nn/optimizers/ada_belief.py
+-rw-r--r--   0 varuna     (501) staff       (20)     8609 2021-01-30 11:54:24.000000 labml-nn-0.4.99/labml_nn/optimizers/adam.py
+-rw-r--r--   0 varuna     (501) staff       (20)     2301 2021-01-14 01:31:38.000000 labml-nn-0.4.99/labml_nn/optimizers/adam_warmup.py
+-rw-r--r--   0 varuna     (501) staff       (20)     3679 2021-01-14 04:00:24.000000 labml-nn-0.4.99/labml_nn/optimizers/adam_warmup_cosine_decay.py
+-rw-r--r--   0 varuna     (501) staff       (20)     8028 2021-02-27 12:23:53.000000 labml-nn-0.4.99/labml_nn/optimizers/amsgrad.py
+-rw-r--r--   0 varuna     (501) staff       (20)     4749 2021-01-14 03:58:27.000000 labml-nn-0.4.99/labml_nn/optimizers/configs.py
+-rw-r--r--   0 varuna     (501) staff       (20)     4063 2021-02-02 04:57:52.000000 labml-nn-0.4.99/labml_nn/optimizers/mnist_experiment.py
+-rw-r--r--   0 varuna     (501) staff       (20)     3380 2021-01-30 08:03:27.000000 labml-nn-0.4.99/labml_nn/optimizers/noam.py
+-rw-r--r--   0 varuna     (501) staff       (20)     1608 2020-12-10 03:00:57.000000 labml-nn-0.4.99/labml_nn/optimizers/performance_test.py
+-rw-r--r--   0 varuna     (501) staff       (20)    11246 2021-01-30 08:03:44.000000 labml-nn-0.4.99/labml_nn/optimizers/radam.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-21 09:36:56.000000 labml-nn-0.4.99/labml_nn/recurrent_highway_networks/
+-rw-r--r--   0 varuna     (501) staff       (20)     5688 2021-02-11 02:23:36.000000 labml-nn-0.4.99/labml_nn/recurrent_highway_networks/__init__.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-21 09:36:56.000000 labml-nn-0.4.99/labml_nn/resnets/
+-rw-r--r--   0 varuna     (501) staff       (20)        0 2021-02-27 12:12:33.000000 labml-nn-0.4.99/labml_nn/resnets/__init__.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-21 09:36:56.000000 labml-nn-0.4.99/labml_nn/resnets/models/
+-rw-r--r--   0 varuna     (501) staff       (20)        0 2021-02-27 12:12:33.000000 labml-nn-0.4.99/labml_nn/resnets/models/__init__.py
+-rw-r--r--   0 varuna     (501) staff       (20)     2695 2021-02-27 12:12:33.000000 labml-nn-0.4.99/labml_nn/resnets/models/mlp.py
+-rw-r--r--   0 varuna     (501) staff       (20)     6659 2021-02-27 12:12:33.000000 labml-nn-0.4.99/labml_nn/resnets/models/resnet.py
+-rwxr-xr-x   0 varuna     (501) staff       (20)     2160 2021-02-27 12:12:33.000000 labml-nn-0.4.99/labml_nn/resnets/pretrained_nets.py
+-rwxr-xr-x   0 varuna     (501) staff       (20)     2513 2021-02-27 12:12:33.000000 labml-nn-0.4.99/labml_nn/resnets/resnet_net.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-21 09:36:56.000000 labml-nn-0.4.99/labml_nn/resnets/utils/
+-rw-r--r--   0 varuna     (501) staff       (20)        0 2021-02-27 12:12:33.000000 labml-nn-0.4.99/labml_nn/resnets/utils/__init__.py
+-rw-r--r--   0 varuna     (501) staff       (20)      546 2021-02-27 12:12:33.000000 labml-nn-0.4.99/labml_nn/resnets/utils/labelsmoothing.py
+-rw-r--r--   0 varuna     (501) staff       (20)     4027 2021-02-27 12:12:33.000000 labml-nn-0.4.99/labml_nn/resnets/utils/train.py
+-rw-r--r--   0 varuna     (501) staff       (20)     2227 2021-02-27 12:12:33.000000 labml-nn-0.4.99/labml_nn/resnets/utils/utils.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-21 09:36:56.000000 labml-nn-0.4.99/labml_nn/rl/
+-rw-r--r--   0 varuna     (501) staff       (20)      826 2020-12-10 03:09:36.000000 labml-nn-0.4.99/labml_nn/rl/__init__.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-21 09:36:56.000000 labml-nn-0.4.99/labml_nn/rl/dqn/
+-rw-r--r--   0 varuna     (501) staff       (20)     6294 2021-04-04 07:52:03.000000 labml-nn-0.4.99/labml_nn/rl/dqn/__init__.py
+-rw-r--r--   0 varuna     (501) staff       (20)     9352 2021-04-04 07:52:03.000000 labml-nn-0.4.99/labml_nn/rl/dqn/experiment.py
+-rw-r--r--   0 varuna     (501) staff       (20)     3281 2020-12-10 03:05:06.000000 labml-nn-0.4.99/labml_nn/rl/dqn/model.py
+-rw-r--r--   0 varuna     (501) staff       (20)     9787 2020-12-10 03:05:47.000000 labml-nn-0.4.99/labml_nn/rl/dqn/replay_buffer.py
+-rw-r--r--   0 varuna     (501) staff       (20)     4657 2020-12-10 03:10:08.000000 labml-nn-0.4.99/labml_nn/rl/game.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-21 09:36:56.000000 labml-nn-0.4.99/labml_nn/rl/ppo/
+-rw-r--r--   0 varuna     (501) staff       (20)     7536 2021-03-30 06:58:44.000000 labml-nn-0.4.99/labml_nn/rl/ppo/__init__.py
+-rw-r--r--   0 varuna     (501) staff       (20)    15285 2021-04-06 07:31:30.000000 labml-nn-0.4.99/labml_nn/rl/ppo/experiment.py
+-rw-r--r--   0 varuna     (501) staff       (20)     3032 2021-03-30 06:56:12.000000 labml-nn-0.4.99/labml_nn/rl/ppo/gae.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-21 09:36:56.000000 labml-nn-0.4.99/labml_nn/sketch_rnn/
+-rw-r--r--   0 varuna     (501) staff       (20)    25112 2021-03-04 16:11:46.000000 labml-nn-0.4.99/labml_nn/sketch_rnn/__init__.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-21 09:36:56.000000 labml-nn-0.4.99/labml_nn/transformers/
+-rw-r--r--   0 varuna     (501) staff       (20)     2390 2021-03-14 02:47:06.000000 labml-nn-0.4.99/labml_nn/transformers/__init__.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-21 09:36:56.000000 labml-nn-0.4.99/labml_nn/transformers/compressive/
+-rw-r--r--   0 varuna     (501) staff       (20)    13740 2021-02-27 12:23:59.000000 labml-nn-0.4.99/labml_nn/transformers/compressive/__init__.py
+-rw-r--r--   0 varuna     (501) staff       (20)    13020 2021-02-19 09:22:47.000000 labml-nn-0.4.99/labml_nn/transformers/compressive/experiment.py
+-rw-r--r--   0 varuna     (501) staff       (20)    10324 2021-02-05 13:40:08.000000 labml-nn-0.4.99/labml_nn/transformers/configs.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-21 09:36:56.000000 labml-nn-0.4.99/labml_nn/transformers/fast_weights/
+-rw-r--r--   0 varuna     (501) staff       (20)    12990 2021-03-14 02:45:31.000000 labml-nn-0.4.99/labml_nn/transformers/fast_weights/__init__.py
+-rw-r--r--   0 varuna     (501) staff       (20)     3832 2021-03-14 02:31:53.000000 labml-nn-0.4.99/labml_nn/transformers/fast_weights/experiment.py
+-rw-r--r--   0 varuna     (501) staff       (20)     4216 2021-03-11 12:33:58.000000 labml-nn-0.4.99/labml_nn/transformers/fast_weights/token_wise.py
+-rw-r--r--   0 varuna     (501) staff       (20)     3582 2021-02-02 04:49:08.000000 labml-nn-0.4.99/labml_nn/transformers/feed_forward.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-21 09:36:56.000000 labml-nn-0.4.99/labml_nn/transformers/feedback/
+-rw-r--r--   0 varuna     (501) staff       (20)    19846 2021-03-27 06:07:13.000000 labml-nn-0.4.99/labml_nn/transformers/feedback/__init__.py
+-rw-r--r--   0 varuna     (501) staff       (20)     4885 2021-02-27 12:25:00.000000 labml-nn-0.4.99/labml_nn/transformers/feedback/experiment.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-21 09:36:56.000000 labml-nn-0.4.99/labml_nn/transformers/glu_variants/
+-rw-r--r--   0 varuna     (501) staff       (20)      359 2021-01-26 11:34:04.000000 labml-nn-0.4.99/labml_nn/transformers/glu_variants/__init__.py
+-rw-r--r--   0 varuna     (501) staff       (20)     4296 2021-02-02 04:50:55.000000 labml-nn-0.4.99/labml_nn/transformers/glu_variants/experiment.py
+-rw-r--r--   0 varuna     (501) staff       (20)    11935 2021-02-27 12:25:25.000000 labml-nn-0.4.99/labml_nn/transformers/glu_variants/simple.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-21 09:36:56.000000 labml-nn-0.4.99/labml_nn/transformers/gpt/
+-rw-r--r--   0 varuna     (501) staff       (20)     8665 2021-02-27 12:25:42.000000 labml-nn-0.4.99/labml_nn/transformers/gpt/__init__.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-21 09:36:56.000000 labml-nn-0.4.99/labml_nn/transformers/knn/
+-rw-r--r--   0 varuna     (501) staff       (20)     1934 2021-01-30 08:04:58.000000 labml-nn-0.4.99/labml_nn/transformers/knn/__init__.py
+-rw-r--r--   0 varuna     (501) staff       (20)     5712 2020-12-10 04:21:43.000000 labml-nn-0.4.99/labml_nn/transformers/knn/build_index.py
+-rw-r--r--   0 varuna     (501) staff       (20)     5907 2020-12-10 04:22:41.000000 labml-nn-0.4.99/labml_nn/transformers/knn/eval_knn.py
+-rw-r--r--   0 varuna     (501) staff       (20)     4481 2021-02-02 04:51:44.000000 labml-nn-0.4.99/labml_nn/transformers/knn/train_model.py
+-rw-r--r--   0 varuna     (501) staff       (20)     2210 2021-02-02 04:49:26.000000 labml-nn-0.4.99/labml_nn/transformers/label_smoothing_loss.py
+-rw-r--r--   0 varuna     (501) staff       (20)     6738 2021-04-23 08:46:41.000000 labml-nn-0.4.99/labml_nn/transformers/mha.py
+-rw-r--r--   0 varuna     (501) staff       (20)     8006 2021-02-07 09:35:46.000000 labml-nn-0.4.99/labml_nn/transformers/models.py
+-rw-r--r--   0 varuna     (501) staff       (20)     2327 2021-02-02 04:50:07.000000 labml-nn-0.4.99/labml_nn/transformers/positional_encoding.py
+-rw-r--r--   0 varuna     (501) staff       (20)      187 2021-02-05 13:40:08.000000 labml-nn-0.4.99/labml_nn/transformers/relative_mha.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-21 09:36:56.000000 labml-nn-0.4.99/labml_nn/transformers/switch/
+-rw-r--r--   0 varuna     (501) staff       (20)     9937 2021-02-27 12:25:54.000000 labml-nn-0.4.99/labml_nn/transformers/switch/__init__.py
+-rw-r--r--   0 varuna     (501) staff       (20)     8189 2021-02-02 04:52:08.000000 labml-nn-0.4.99/labml_nn/transformers/switch/experiment.py
+-rw-r--r--   0 varuna     (501) staff       (20)      538 2021-02-05 13:40:08.000000 labml-nn-0.4.99/labml_nn/transformers/utils.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-21 09:36:56.000000 labml-nn-0.4.99/labml_nn/transformers/xl/
+-rw-r--r--   0 varuna     (501) staff       (20)     5422 2021-02-27 12:26:06.000000 labml-nn-0.4.99/labml_nn/transformers/xl/__init__.py
+-rw-r--r--   0 varuna     (501) staff       (20)     8779 2021-02-07 10:15:28.000000 labml-nn-0.4.99/labml_nn/transformers/xl/experiment.py
+-rw-r--r--   0 varuna     (501) staff       (20)     6230 2021-02-07 09:32:13.000000 labml-nn-0.4.99/labml_nn/transformers/xl/relative_mha.py
+-rw-r--r--   0 varuna     (501) staff       (20)      646 2021-05-21 09:29:30.000000 labml-nn-0.4.99/labml_nn/utils.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-21 09:36:56.000000 labml-nn-0.4.99/labml_nn.egg-info/
+-rw-r--r--   0 varuna     (501) staff       (20)     6380 2021-05-21 09:36:56.000000 labml-nn-0.4.99/labml_nn.egg-info/PKG-INFO
+-rw-r--r--   0 varuna     (501) staff       (20)     3959 2021-05-21 09:36:56.000000 labml-nn-0.4.99/labml_nn.egg-info/SOURCES.txt
+-rw-r--r--   0 varuna     (501) staff       (20)        1 2021-05-21 09:36:56.000000 labml-nn-0.4.99/labml_nn.egg-info/dependency_links.txt
+-rw-r--r--   0 varuna     (501) staff       (20)       56 2021-05-21 09:36:56.000000 labml-nn-0.4.99/labml_nn.egg-info/requires.txt
+-rw-r--r--   0 varuna     (501) staff       (20)       15 2021-05-21 09:36:56.000000 labml-nn-0.4.99/labml_nn.egg-info/top_level.txt
+-rw-r--r--   0 varuna     (501) staff       (20)       38 2021-05-21 09:36:56.000000 labml-nn-0.4.99/setup.cfg
+-rw-r--r--   0 varuna     (501) staff       (20)     1676 2021-05-21 09:32:45.000000 labml-nn-0.4.99/setup.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-05-21 09:36:56.000000 labml-nn-0.4.99/utils/
+-rw-r--r--   0 varuna     (501) staff       (20)        0 2021-01-27 03:27:09.000000 labml-nn-0.4.99/utils/__init__.py
+-rw-r--r--   0 varuna     (501) staff       (20)     5404 2021-05-21 09:29:30.000000 labml-nn-0.4.99/utils/diagrams.py
+-rw-r--r--   0 varuna     (501) staff       (20)     1424 2021-01-27 03:48:30.000000 labml-nn-0.4.99/utils/sitemap.py
```

### Comparing `labml-nn-0.4.98/PKG-INFO` & `labml-nn-0.4.99/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labml-nn
-Version: 0.4.98
+Version: 0.4.99
 Summary: A collection of PyTorch implementations of neural network architectures and layers.
 Home-page: https://github.com/lab-ml/nn
 Author: Varuna Jayasiri, Nipun Wijerathne
 Author-email: vpjayasiri@gmail.com, hnipun@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://lab-ml.com/
 Description: [![Join Slack](https://img.shields.io/badge/slack-chat-green.svg?logo=slack)](https://join.slack.com/t/labforml/shared_invite/zt-egj9zvq9-Dl3hhZqobexgT7aVKnD14g/)
@@ -51,14 +51,16 @@
         #### ✨ [Capsule Networks](https://nn.labml.ai/capsule_networks/index.html)
         
         #### ✨ [Generative Adversarial Networks](https://nn.labml.ai/gan/index.html)
         * [Original GAN](https://nn.labml.ai/gan/original/index.html)
         * [GAN with deep convolutional network](https://nn.labml.ai/gan/dcgan/index.html)
         * [Cycle GAN](https://nn.labml.ai/gan/cycle_gan/index.html)
         * [Wasserstein GAN](https://nn.labml.ai/gan/wasserstein/index.html)
+        * [Wasserstein GAN with Gradient Penalty](https://nn.labml.ai/gan/wasserstein/gradient_penalty/index.html)
+        * [Style GAN 2](https://nn.labml.ai/gan/stylegan/index.html)
         
         #### ✨ [Sketch RNN](https://nn.labml.ai/sketch_rnn/index.html)
         
         #### ✨ [Reinforcement Learning](https://nn.labml.ai/rl/index.html)
         * [Proximal Policy Optimization](https://nn.labml.ai/rl/ppo/index.html) with
          [Generalized Advantage Estimation](https://nn.labml.ai/rl/ppo/gae.html)
         * [Deep Q Networks](https://nn.labml.ai/rl/dqn/index.html) with
```

### Comparing `labml-nn-0.4.98/labml_nn/__init__.py` & `labml-nn-0.4.99/labml_nn/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,14 +36,16 @@
 #### ✨ [Capsule Networks](capsule_networks/index.html)
 
 #### ✨ [Generative Adversarial Networks](gan/index.html)
 * [Original GAN](gan/original/index.html)
 * [GAN with deep convolutional network](gan/dcgan/index.html)
 * [Cycle GAN](gan/cycle_gan/index.html)
 * [Wasserstein GAN](gan/wasserstein/index.html)
+* [Wasserstein GAN with Gradient Penalty](gan/wasserstein/gradient_penalty/index.html)
+* [Style GAN 2](gan/stylegan/index.html)
 
 #### ✨ [Sketch RNN](sketch_rnn/index.html)
 
 #### ✨ [Reinforcement Learning](rl/index.html)
 * [Proximal Policy Optimization](rl/ppo/index.html) with
  [Generalized Advantage Estimation](rl/ppo/gae.html)
 * [Deep Q Networks](rl/dqn/index.html) with
```

### Comparing `labml-nn-0.4.98/labml_nn/capsule_networks/__init__.py` & `labml-nn-0.4.99/labml_nn/capsule_networks/__init__.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/capsule_networks/mnist.py` & `labml-nn-0.4.99/labml_nn/capsule_networks/mnist.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/experiments/mnist.py` & `labml-nn-0.4.99/labml_nn/experiments/mnist.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/experiments/nlp_autoregression.py` & `labml-nn-0.4.99/labml_nn/experiments/nlp_autoregression.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/gan/cycle_gan/__init__.py` & `labml-nn-0.4.99/labml_nn/gan/cycle_gan/__init__.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/gan/dcgan/__init__.py` & `labml-nn-0.4.99/labml_nn/gan/dcgan/__init__.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/gan/original/__init__.py` & `labml-nn-0.4.99/labml_nn/gan/original/__init__.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/gan/original/experiment.py` & `labml-nn-0.4.99/labml_nn/gan/original/experiment.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/gan/wasserstein/__init__.py` & `labml-nn-0.4.99/labml_nn/gan/wasserstein/__init__.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/gan/wasserstein/experiment.py` & `labml-nn-0.4.99/labml_nn/gan/wasserstein/experiment.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/gan/wasserstein/gradient_penalty/__init__.py` & `labml-nn-0.4.99/labml_nn/gan/wasserstein/gradient_penalty/__init__.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/gan/wasserstein/gradient_penalty/experiment.py` & `labml-nn-0.4.99/labml_nn/gan/wasserstein/gradient_penalty/experiment.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/hypernetworks/experiment.py` & `labml-nn-0.4.99/labml_nn/hypernetworks/experiment.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/hypernetworks/hyper_lstm.py` & `labml-nn-0.4.99/labml_nn/hypernetworks/hyper_lstm.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/lstm/__init__.py` & `labml-nn-0.4.99/labml_nn/lstm/__init__.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/normalization/batch_channel_norm/__init__.py` & `labml-nn-0.4.99/labml_nn/normalization/batch_channel_norm/__init__.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/normalization/batch_norm/__init__.py` & `labml-nn-0.4.99/labml_nn/normalization/batch_norm/__init__.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/normalization/batch_norm/cifar10.py` & `labml-nn-0.4.99/labml_nn/normalization/batch_norm/cifar10.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/normalization/batch_norm/mnist.py` & `labml-nn-0.4.99/labml_nn/normalization/batch_norm/mnist.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/normalization/group_norm/__init__.py` & `labml-nn-0.4.99/labml_nn/normalization/group_norm/__init__.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/normalization/group_norm/experiment.py` & `labml-nn-0.4.99/labml_nn/normalization/group_norm/experiment.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/normalization/instance_norm/__init__.py` & `labml-nn-0.4.99/labml_nn/normalization/instance_norm/__init__.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/normalization/instance_norm/experiment.py` & `labml-nn-0.4.99/labml_nn/normalization/instance_norm/experiment.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/normalization/layer_norm/__init__.py` & `labml-nn-0.4.99/labml_nn/normalization/layer_norm/__init__.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/normalization/weight_standardization/__init__.py` & `labml-nn-0.4.99/labml_nn/normalization/weight_standardization/__init__.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/normalization/weight_standardization/conv2d.py` & `labml-nn-0.4.99/labml_nn/normalization/weight_standardization/conv2d.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/normalization/weight_standardization/experiment.py` & `labml-nn-0.4.99/labml_nn/normalization/weight_standardization/experiment.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/optimizers/__init__.py` & `labml-nn-0.4.99/labml_nn/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/optimizers/ada_belief.py` & `labml-nn-0.4.99/labml_nn/optimizers/ada_belief.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/optimizers/adam.py` & `labml-nn-0.4.99/labml_nn/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/optimizers/adam_warmup.py` & `labml-nn-0.4.99/labml_nn/optimizers/adam_warmup.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/optimizers/adam_warmup_cosine_decay.py` & `labml-nn-0.4.99/labml_nn/optimizers/adam_warmup_cosine_decay.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/optimizers/amsgrad.py` & `labml-nn-0.4.99/labml_nn/optimizers/amsgrad.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/optimizers/configs.py` & `labml-nn-0.4.99/labml_nn/optimizers/configs.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/optimizers/mnist_experiment.py` & `labml-nn-0.4.99/labml_nn/optimizers/mnist_experiment.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/optimizers/noam.py` & `labml-nn-0.4.99/labml_nn/optimizers/noam.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/optimizers/performance_test.py` & `labml-nn-0.4.99/labml_nn/optimizers/performance_test.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/optimizers/radam.py` & `labml-nn-0.4.99/labml_nn/optimizers/radam.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/recurrent_highway_networks/__init__.py` & `labml-nn-0.4.99/labml_nn/recurrent_highway_networks/__init__.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/resnets/models/mlp.py` & `labml-nn-0.4.99/labml_nn/resnets/models/mlp.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/resnets/models/resnet.py` & `labml-nn-0.4.99/labml_nn/resnets/models/resnet.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/resnets/pretrained_nets.py` & `labml-nn-0.4.99/labml_nn/resnets/pretrained_nets.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/resnets/resnet_net.py` & `labml-nn-0.4.99/labml_nn/resnets/resnet_net.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/resnets/utils/labelsmoothing.py` & `labml-nn-0.4.99/labml_nn/resnets/utils/labelsmoothing.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/resnets/utils/train.py` & `labml-nn-0.4.99/labml_nn/resnets/utils/train.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/resnets/utils/utils.py` & `labml-nn-0.4.99/labml_nn/resnets/utils/utils.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/rl/__init__.py` & `labml-nn-0.4.99/labml_nn/rl/__init__.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/rl/dqn/__init__.py` & `labml-nn-0.4.99/labml_nn/rl/dqn/__init__.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/rl/dqn/experiment.py` & `labml-nn-0.4.99/labml_nn/rl/dqn/experiment.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/rl/dqn/model.py` & `labml-nn-0.4.99/labml_nn/rl/dqn/model.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/rl/dqn/replay_buffer.py` & `labml-nn-0.4.99/labml_nn/rl/dqn/replay_buffer.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/rl/game.py` & `labml-nn-0.4.99/labml_nn/rl/game.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/rl/ppo/__init__.py` & `labml-nn-0.4.99/labml_nn/rl/ppo/__init__.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/rl/ppo/experiment.py` & `labml-nn-0.4.99/labml_nn/rl/ppo/experiment.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/rl/ppo/gae.py` & `labml-nn-0.4.99/labml_nn/rl/ppo/gae.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/sketch_rnn/__init__.py` & `labml-nn-0.4.99/labml_nn/sketch_rnn/__init__.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/transformers/__init__.py` & `labml-nn-0.4.99/labml_nn/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/transformers/compressive/__init__.py` & `labml-nn-0.4.99/labml_nn/transformers/compressive/__init__.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/transformers/compressive/experiment.py` & `labml-nn-0.4.99/labml_nn/transformers/compressive/experiment.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/transformers/configs.py` & `labml-nn-0.4.99/labml_nn/transformers/configs.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/transformers/fast_weights/__init__.py` & `labml-nn-0.4.99/labml_nn/transformers/fast_weights/__init__.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/transformers/fast_weights/experiment.py` & `labml-nn-0.4.99/labml_nn/transformers/fast_weights/experiment.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/transformers/fast_weights/token_wise.py` & `labml-nn-0.4.99/labml_nn/transformers/fast_weights/token_wise.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/transformers/feed_forward.py` & `labml-nn-0.4.99/labml_nn/transformers/feed_forward.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/transformers/feedback/__init__.py` & `labml-nn-0.4.99/labml_nn/transformers/feedback/__init__.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/transformers/feedback/experiment.py` & `labml-nn-0.4.99/labml_nn/transformers/feedback/experiment.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/transformers/glu_variants/experiment.py` & `labml-nn-0.4.99/labml_nn/transformers/glu_variants/experiment.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/transformers/glu_variants/simple.py` & `labml-nn-0.4.99/labml_nn/transformers/glu_variants/simple.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/transformers/gpt/__init__.py` & `labml-nn-0.4.99/labml_nn/transformers/gpt/__init__.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/transformers/knn/__init__.py` & `labml-nn-0.4.99/labml_nn/transformers/knn/__init__.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/transformers/knn/build_index.py` & `labml-nn-0.4.99/labml_nn/transformers/knn/build_index.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/transformers/knn/eval_knn.py` & `labml-nn-0.4.99/labml_nn/transformers/knn/eval_knn.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/transformers/knn/train_model.py` & `labml-nn-0.4.99/labml_nn/transformers/knn/train_model.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/transformers/label_smoothing_loss.py` & `labml-nn-0.4.99/labml_nn/transformers/label_smoothing_loss.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/transformers/mha.py` & `labml-nn-0.4.99/labml_nn/transformers/mha.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/transformers/models.py` & `labml-nn-0.4.99/labml_nn/transformers/models.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/transformers/positional_encoding.py` & `labml-nn-0.4.99/labml_nn/transformers/positional_encoding.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/transformers/switch/__init__.py` & `labml-nn-0.4.99/labml_nn/transformers/switch/__init__.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/transformers/switch/experiment.py` & `labml-nn-0.4.99/labml_nn/transformers/switch/experiment.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/transformers/utils.py` & `labml-nn-0.4.99/labml_nn/transformers/utils.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/transformers/xl/__init__.py` & `labml-nn-0.4.99/labml_nn/transformers/xl/__init__.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/transformers/xl/experiment.py` & `labml-nn-0.4.99/labml_nn/transformers/xl/experiment.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn/transformers/xl/relative_mha.py` & `labml-nn-0.4.99/labml_nn/transformers/xl/relative_mha.py`

 * *Files identical despite different names*

### Comparing `labml-nn-0.4.98/labml_nn.egg-info/PKG-INFO` & `labml-nn-0.4.99/labml_nn.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labml-nn
-Version: 0.4.98
+Version: 0.4.99
 Summary: A collection of PyTorch implementations of neural network architectures and layers.
 Home-page: https://github.com/lab-ml/nn
 Author: Varuna Jayasiri, Nipun Wijerathne
 Author-email: vpjayasiri@gmail.com, hnipun@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://lab-ml.com/
 Description: [![Join Slack](https://img.shields.io/badge/slack-chat-green.svg?logo=slack)](https://join.slack.com/t/labforml/shared_invite/zt-egj9zvq9-Dl3hhZqobexgT7aVKnD14g/)
@@ -51,14 +51,16 @@
         #### ✨ [Capsule Networks](https://nn.labml.ai/capsule_networks/index.html)
         
         #### ✨ [Generative Adversarial Networks](https://nn.labml.ai/gan/index.html)
         * [Original GAN](https://nn.labml.ai/gan/original/index.html)
         * [GAN with deep convolutional network](https://nn.labml.ai/gan/dcgan/index.html)
         * [Cycle GAN](https://nn.labml.ai/gan/cycle_gan/index.html)
         * [Wasserstein GAN](https://nn.labml.ai/gan/wasserstein/index.html)
+        * [Wasserstein GAN with Gradient Penalty](https://nn.labml.ai/gan/wasserstein/gradient_penalty/index.html)
+        * [Style GAN 2](https://nn.labml.ai/gan/stylegan/index.html)
         
         #### ✨ [Sketch RNN](https://nn.labml.ai/sketch_rnn/index.html)
         
         #### ✨ [Reinforcement Learning](https://nn.labml.ai/rl/index.html)
         * [Proximal Policy Optimization](https://nn.labml.ai/rl/ppo/index.html) with
          [Generalized Advantage Estimation](https://nn.labml.ai/rl/ppo/gae.html)
         * [Deep Q Networks](https://nn.labml.ai/rl/dqn/index.html) with
```

### Comparing `labml-nn-0.4.98/labml_nn.egg-info/SOURCES.txt` & `labml-nn-0.4.99/labml_nn.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 labml_nn/experiments/mnist.py
 labml_nn/experiments/nlp_autoregression.py
 labml_nn/gan/__init__.py
 labml_nn/gan/cycle_gan/__init__.py
 labml_nn/gan/dcgan/__init__.py
 labml_nn/gan/original/__init__.py
 labml_nn/gan/original/experiment.py
+labml_nn/gan/stylegan/__init__.py
+labml_nn/gan/stylegan/experiment.py
 labml_nn/gan/wasserstein/__init__.py
 labml_nn/gan/wasserstein/experiment.py
 labml_nn/gan/wasserstein/gradient_penalty/__init__.py
 labml_nn/gan/wasserstein/gradient_penalty/experiment.py
 labml_nn/hypernetworks/__init__.py
 labml_nn/hypernetworks/experiment.py
 labml_nn/hypernetworks/hyper_lstm.py
@@ -99,8 +101,9 @@
 labml_nn/transformers/knn/train_model.py
 labml_nn/transformers/switch/__init__.py
 labml_nn/transformers/switch/experiment.py
 labml_nn/transformers/xl/__init__.py
 labml_nn/transformers/xl/experiment.py
 labml_nn/transformers/xl/relative_mha.py
 utils/__init__.py
+utils/diagrams.py
 utils/sitemap.py
```

### Comparing `labml-nn-0.4.98/setup.py` & `labml-nn-0.4.99/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("readme.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name='labml-nn',
-    version='0.4.98',
+    version='0.4.99',
     author="Varuna Jayasiri, Nipun Wijerathne",
     author_email="vpjayasiri@gmail.com, hnipun@gmail.com",
     description="A collection of PyTorch implementations of neural network architectures and layers.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lab-ml/nn",
     project_urls={
```

### Comparing `labml-nn-0.4.98/utils/sitemap.py` & `labml-nn-0.4.99/utils/sitemap.py`

 * *Files identical despite different names*

