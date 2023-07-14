# Comparing `tmp/whisperspeech-0.0.1.tar.gz` & `tmp/WhisperSpeech-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whisperspeech-0.0.1.tar", last modified: Thu Jul 13 18:07:25 2023, max compression
+gzip compressed data, was "WhisperSpeech-0.0.2.tar", last modified: Fri Jul 14 22:51:48 2023, max compression
```

## Comparing `whisperspeech-0.0.1.tar` & `WhisperSpeech-0.0.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 18:07:25.482848 whisperspeech-0.0.1/
--rw-r--r--   0 root         (0) root         (0)     1091 2023-05-15 17:24:12.000000 whisperspeech-0.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      111 2023-05-15 17:24:12.000000 whisperspeech-0.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6789 2023-07-13 18:07:25.482848 whisperspeech-0.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5972 2023-07-13 17:54:10.000000 whisperspeech-0.0.1/README.md
--rw-r--r--   0 root         (0) root         (0)     1241 2023-07-13 18:07:22.000000 whisperspeech-0.0.1/settings.ini
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-13 18:07:25.482848 whisperspeech-0.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2560 2023-05-15 17:24:12.000000 whisperspeech-0.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 18:07:25.482848 whisperspeech-0.0.1/spear_tts_pytorch/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-13 17:53:29.000000 whisperspeech-0.0.1/spear_tts_pytorch/__init__.py
--rw-r--r--   0 root         (0) root         (0)    67322 2023-07-13 17:54:11.000000 whisperspeech-0.0.1/spear_tts_pytorch/_modidx.py
--rw-r--r--   0 root         (0) root         (0)     5422 2023-07-13 11:51:18.000000 whisperspeech-0.0.1/spear_tts_pytorch/a2a.py
--rw-r--r--   0 root         (0) root         (0)      960 2023-07-13 17:54:11.000000 whisperspeech-0.0.1/spear_tts_pytorch/a2wav.py
--rw-r--r--   0 root         (0) root         (0)     1983 2023-07-13 17:53:29.000000 whisperspeech-0.0.1/spear_tts_pytorch/extract_acoustic.py
--rw-r--r--   0 root         (0) root         (0)     2570 2023-07-13 17:54:11.000000 whisperspeech-0.0.1/spear_tts_pytorch/extract_semb.py
--rw-r--r--   0 root         (0) root         (0)     9636 2023-07-13 17:54:10.000000 whisperspeech-0.0.1/spear_tts_pytorch/extract_stoks.py
--rw-r--r--   0 root         (0) root         (0)    10094 2023-07-13 17:54:10.000000 whisperspeech-0.0.1/spear_tts_pytorch/modules.py
--rw-r--r--   0 root         (0) root         (0)      965 2023-07-13 17:54:11.000000 whisperspeech-0.0.1/spear_tts_pytorch/pipeline.py
--rw-r--r--   0 root         (0) root         (0)    16936 2023-07-13 17:54:11.000000 whisperspeech-0.0.1/spear_tts_pytorch/s2a_delar_mup.py
--rw-r--r--   0 root         (0) root         (0)    11508 2023-07-13 17:54:11.000000 whisperspeech-0.0.1/spear_tts_pytorch/t2s_up.py
--rw-r--r--   0 root         (0) root         (0)     8654 2023-07-13 17:54:10.000000 whisperspeech-0.0.1/spear_tts_pytorch/train.py
--rw-r--r--   0 root         (0) root         (0)     9750 2023-07-13 17:54:11.000000 whisperspeech-0.0.1/spear_tts_pytorch/train_multi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 18:07:25.482848 whisperspeech-0.0.1/whisperspeech.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6789 2023-07-13 18:07:25.000000 whisperspeech-0.0.1/whisperspeech.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      711 2023-07-13 18:07:25.000000 whisperspeech-0.0.1/whisperspeech.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 18:07:25.000000 whisperspeech-0.0.1/whisperspeech.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      285 2023-07-13 18:07:25.000000 whisperspeech-0.0.1/whisperspeech.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 18:07:25.000000 whisperspeech-0.0.1/whisperspeech.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       97 2023-07-13 18:07:25.000000 whisperspeech-0.0.1/whisperspeech.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-13 18:07:25.000000 whisperspeech-0.0.1/whisperspeech.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 22:51:48.598960 WhisperSpeech-0.0.2/
+-rw-r--r--   0 root         (0) root         (0)     1091 2023-05-15 17:24:12.000000 WhisperSpeech-0.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      111 2023-05-15 17:24:12.000000 WhisperSpeech-0.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6789 2023-07-14 22:51:48.598960 WhisperSpeech-0.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5972 2023-07-13 17:54:10.000000 WhisperSpeech-0.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 22:51:48.598960 WhisperSpeech-0.0.2/WhisperSpeech.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6789 2023-07-14 22:51:48.000000 WhisperSpeech-0.0.2/WhisperSpeech.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      659 2023-07-14 22:51:48.000000 WhisperSpeech-0.0.2/WhisperSpeech.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 22:51:48.000000 WhisperSpeech-0.0.2/WhisperSpeech.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      297 2023-07-14 22:51:48.000000 WhisperSpeech-0.0.2/WhisperSpeech.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 16:42:35.000000 WhisperSpeech-0.0.2/WhisperSpeech.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       97 2023-07-14 22:51:48.000000 WhisperSpeech-0.0.2/WhisperSpeech.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-07-14 22:51:48.000000 WhisperSpeech-0.0.2/WhisperSpeech.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1253 2023-07-14 22:51:41.000000 WhisperSpeech-0.0.2/settings.ini
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-14 22:51:48.598960 WhisperSpeech-0.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2560 2023-05-15 17:24:12.000000 WhisperSpeech-0.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 22:51:48.598960 WhisperSpeech-0.0.2/whisperspeech/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-14 22:45:12.000000 WhisperSpeech-0.0.2/whisperspeech/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58342 2023-07-14 22:45:12.000000 WhisperSpeech-0.0.2/whisperspeech/_modidx.py
+-rw-r--r--   0 root         (0) root         (0)     5422 2023-07-13 11:51:18.000000 WhisperSpeech-0.0.2/whisperspeech/a2a.py
+-rw-r--r--   0 root         (0) root         (0)     1108 2023-07-14 22:45:12.000000 WhisperSpeech-0.0.2/whisperspeech/a2wav.py
+-rw-r--r--   0 root         (0) root         (0)     1983 2023-07-14 22:45:12.000000 WhisperSpeech-0.0.2/whisperspeech/extract_acoustic.py
+-rw-r--r--   0 root         (0) root         (0)     2570 2023-07-14 22:45:12.000000 WhisperSpeech-0.0.2/whisperspeech/extract_semb.py
+-rw-r--r--   0 root         (0) root         (0)     9636 2023-07-14 22:45:12.000000 WhisperSpeech-0.0.2/whisperspeech/extract_stoks.py
+-rw-r--r--   0 root         (0) root         (0)    10094 2023-07-14 22:45:12.000000 WhisperSpeech-0.0.2/whisperspeech/modules.py
+-rw-r--r--   0 root         (0) root         (0)     1167 2023-07-14 22:45:12.000000 WhisperSpeech-0.0.2/whisperspeech/pipeline.py
+-rw-r--r--   0 root         (0) root         (0)    16932 2023-07-14 22:45:12.000000 WhisperSpeech-0.0.2/whisperspeech/s2a_delar_mup.py
+-rw-r--r--   0 root         (0) root         (0)    12102 2023-07-14 22:45:12.000000 WhisperSpeech-0.0.2/whisperspeech/t2s_up.py
+-rw-r--r--   0 root         (0) root         (0)     8705 2023-07-14 22:45:12.000000 WhisperSpeech-0.0.2/whisperspeech/train.py
+-rw-r--r--   0 root         (0) root         (0)     9800 2023-07-14 22:45:12.000000 WhisperSpeech-0.0.2/whisperspeech/train_multi.py
```

### Comparing `whisperspeech-0.0.1/LICENSE` & `WhisperSpeech-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `whisperspeech-0.0.1/PKG-INFO` & `WhisperSpeech-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
-Name: whisperspeech
-Version: 0.0.1
+Name: WhisperSpeech
+Version: 0.0.2
 Summary: An Open Source text-to-speech system built by inverting Whisper
-Home-page: https://github.com/collabora/whisperspeech
+Home-page: https://github.com/collabora/WhisperSpeech
 Author: Jakub Piotr Cłapa
 Author-email: jpc@collabora.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `whisperspeech-0.0.1/README.md` & `WhisperSpeech-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `whisperspeech-0.0.1/settings.ini` & `WhisperSpeech-0.0.2/settings.ini`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
-repo = whisperspeech
+repo = WhisperSpeech
 lib_name = %(repo)s
-version = 0.0.1
+version = 0.0.2
 min_python = 3.7
 license = apache2
 
 ### nbdev ###
 doc_path = _docs
 lib_path = whisperspeech
 nbs_path = nbs
@@ -34,10 +34,10 @@
 language = English
 status = 3
 user = collabora
 
 ### Optional ###
 requirements = openai-whisper encodec pyarrow vocos scikit-learn vector_quantize_pytorch huggingface_hub
 # dev_requirements = 
-console_scripts = spear_extract_acoustic=spear_tts_pytorch.extract_acoustic:extract_acoustic
-		  spear_extract_semantic=spear_tts_pytorch.extract_semb:extract_semantic
-		  spear_extract_stoks=spear_tts_pytorch.extract_stoks:extract_stoks
+console_scripts = whisperspeech_extract_acoustic=whisperspeech.extract_acoustic:extract_acoustic
+		  whisperspeech_extract_semantic=whisperspeech.extract_semb:extract_semantic
+		  whisperspeech_extract_stoks=whisperspeech.extract_stoks:extract_stoks
```

### Comparing `whisperspeech-0.0.1/setup.py` & `WhisperSpeech-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `whisperspeech-0.0.1/spear_tts_pytorch/a2a.py` & `WhisperSpeech-0.0.2/whisperspeech/a2a.py`

 * *Files identical despite different names*

### Comparing `whisperspeech-0.0.1/spear_tts_pytorch/a2wav.py` & `WhisperSpeech-0.0.2/whisperspeech/a2wav.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 __all__ = ['Vocoder']
 
 # %% ../nbs/6. Quality-boosting vocoder.ipynb 1
 from vocos import Vocos
 import torch
 import torchaudio
 
-from IPython.display import HTML
+from IPython.display import HTML, Audio
 
 # %% ../nbs/6. Quality-boosting vocoder.ipynb 2
 class Vocoder:
     def __init__(self, repo_id="charactr/vocos-encodec-24khz"):
         self.vocos = Vocos.from_pretrained(repo_id).cuda()
     
     @torch.no_grad()
@@ -23,7 +23,11 @@
         bandwidth_id = torch.tensor({2:0,4:1,8:2}[q]).cuda()
         return self.vocos.decode(features, bandwidth_id=bandwidth_id)
         
     def decode_to_file(self, fname, atoks):
         audio = self.decode(atoks)
         torchaudio.save(fname, audio.cpu(), 24000)
         display(HTML(f'<a href="{fname}" target="_blank">Listen to {fname}</a>'))
+        
+    def decode_to_notebook(self, atoks):
+        audio = self.decode(atoks)
+        display(Audio(audio.cpu().numpy(), rate=24000))
```

### Comparing `whisperspeech-0.0.1/spear_tts_pytorch/extract_acoustic.py` & `WhisperSpeech-0.0.2/whisperspeech/extract_acoustic.py`

 * *Files identical despite different names*

### Comparing `whisperspeech-0.0.1/spear_tts_pytorch/extract_semb.py` & `WhisperSpeech-0.0.2/whisperspeech/extract_semb.py`

 * *Files identical despite different names*

### Comparing `whisperspeech-0.0.1/spear_tts_pytorch/extract_stoks.py` & `WhisperSpeech-0.0.2/whisperspeech/extract_stoks.py`

 * *Files identical despite different names*

### Comparing `whisperspeech-0.0.1/spear_tts_pytorch/modules.py` & `WhisperSpeech-0.0.2/whisperspeech/modules.py`

 * *Files identical despite different names*

### Comparing `whisperspeech-0.0.1/spear_tts_pytorch/s2a_delar_mup.py` & `WhisperSpeech-0.0.2/whisperspeech/s2a_delar_mup.py`

 * *Files 0% similar despite different names*

```diff
@@ -337,15 +337,15 @@
 
         return logits, loss
 
     #
     # inference
     #
     @classmethod
-    def load_model(cls, repo_id="collabora/spear-tts-pytorch", filename="s2a_up.model", local_filename=None):
+    def load_model(cls, repo_id="collabora/whisperspeech", filename="s2a_up.model", local_filename=None):
         if not local_filename:
             local_filename = hf_hub_download(repo_id=repo_id, filename=filename)
         spec = torch.load(local_filename)
         model = cls(**spec['config'], tunables=Tunables(**spec['tunables']))
         model.load_state_dict(spec['state_dict'])
         model.eval()
         return model
```

### Comparing `whisperspeech-0.0.1/spear_tts_pytorch/t2s_up.py` & `WhisperSpeech-0.0.2/whisperspeech/t2s_up.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/5. Text to semantic token modeling μP.ipynb.
 
 # %% auto 0
 __all__ = ['load_datasets', 'rand', 'Tunables', 'Encoder', 'Decoder', 'TSARTransformer', 'make_model']
 
 # %% ../nbs/5. Text to semantic token modeling μP.ipynb 1
+import math
 import torch
 import torch.nn as nn
 from torch.profiler import record_function
 
 from huggingface_hub import hf_hub_download
 from fastcore.basics import store_attr
 from fastprogress import progress_bar
@@ -15,16 +16,16 @@
 # %% ../nbs/5. Text to semantic token modeling μP.ipynb 2
 from pathlib import Path
 import pylab as plt
 import pandas as pd
 
 # %% ../nbs/5. Text to semantic token modeling μP.ipynb 3
 import whisper
-from spear_tts_pytorch.train import *
-from spear_tts_pytorch.modules import *
+from whisperspeech.train import *
+from whisperspeech.modules import *
 
 # %% ../nbs/5. Text to semantic token modeling μP.ipynb 11
 def load_data(path:Path):
     data = pd.DataFrame(dict(stoks=[str(x) for x in Path(path).rglob('*.stoks')]))
     data['stoks_len'] = data['stoks'].map(lambda x: torch.load(x).shape[1]/50)
     data['text'] = data['stoks'].apply(lambda x: Path(x).with_suffix('.txt').read_text())
     data['ttoks_len'] = data['text'].map(lambda x: len(tokenizer.encode(x)))
@@ -65,96 +66,97 @@
     data['wc_err'] = data['txt_large_wc'] - data['txt_tiny_wc']
     data_clean = data[data['wc_err'].abs() < 5]
     
     val_data, train_data = data_clean[:300], data_clean[300:]
 
     return SADataset(train_data, tokenizer), SADataset(val_data, tokenizer)
 
-# %% ../nbs/5. Text to semantic token modeling μP.ipynb 32
-from dataclasses import dataclass
+# %% ../nbs/5. Text to semantic token modeling μP.ipynb 33
+import dataclasses
 import random
 
 def rand(start, end):
     return random.random() * (end - start) + start
 
-@dataclass
+@dataclasses.dataclass
 class Tunables:
-    init_std :float = .8
-    embeddings_std :float = .3
-    embeddings_lr_scale: float = 1.8
-    output_mult :float = .25
-    query_mult :float = 116
+    init_std :float = 1
+    embeddings_std :float = .01
+    embeddings_lr_scale: float = 5
+    output_mult :float = .35
+    query_mult :float = 1
     encoder_depth_ratio :float = 0.25
         
-    lr0 :float = 4e-3
-    clip_gradient_norm :float = .1
+    lr0 :float = 3e-3
+    clip_gradient_norm :float = .2
     weight_decay :float = 1e-5
-    warmup_steps :float = 500
+    warmup_steps :float = 4000
 
     random :bool = False
-        
+
     def __post_init__(self):
         # randomize the hyperparams if requested
         if self.random:
-            self.init_std = 10**rand(-2,1)
-            self.embeddings_std = 10**rand(-1.4,-.5)
+#             self.init_std = 10**rand(-3,1)
+            self.init_std = 10**rand(-1,1)
+#             self.embeddings_std = 10**rand(-3,1)
+            self.embeddings_std = 10**rand(-3,-.7)
 #             self.embeddings_lr_scale = 2**rand(-3,3)
-            self.embeddings_lr_scale = self.embeddings_std * 10**rand(0,1)
-#             self.output_mult = 2**rand(-2,8)
-            self.output_mult = 2**rand(-3,1)
-            self.query_mult = 2**rand(2,8) ## FIXME: not implemented
+            self.embeddings_lr_scale = rand(2,6) #2**rand(0,3)
+#             self.output_mult = 2**rand(-2,3)
+            self.output_mult = rand(0.25,0.65)
+            self.query_mult = 2**rand(-2,3)
 #             self.encoder_depth_ratio = random.choice([0.25,0.5,0.75])
             self.encoder_depth_ratio = 0.25
             
-            self.lr0 = rand(2,8)*1e-3#10**rand(-3,-2)
-#             self.clip_gradient_norm = 10**rand(-2,1)
-#             self.weight_decay = 10**rand(-5,-1)
-#             self.warmup_steps = 100*(10**rand(0,1))
-            self.clip_gradient_norm = .1
-            self.weight_decay = 1e-5
-            self.warmup_steps = 100*10**rand(0,1)
+#             self.lr0 = 10**rand(-4,-1.5)
+            self.lr0 = rand(1,5)*1e-3
+            self.clip_gradient_norm = 10**rand(-3,0)
+            self.warmup_steps = 100*(10**rand(1,1.85))
 
-# %% ../nbs/5. Text to semantic token modeling μP.ipynb 34
+# %% ../nbs/5. Text to semantic token modeling μP.ipynb 35
 class Encoder(nn.Module):
-    def __init__(self, depth=6, width=384, n_head=6, length=1500, codes=1024, pos_embs=None, tunables=Tunables()):
+    def __init__(self, depth=6, width=384, n_head=6, length=1500, codes=1024, ffn_mult=4, pos_embs=None, tunables=Tunables()):
         super().__init__()
     
         self.embedding = nn.Embedding(codes, width)
 
         if pos_embs is None: pos_embs = sinusoids(length, width)
         self.register_buffer("positional_embedding", pos_embs)
 
         self.layers = nn.Sequential(*[
-            ResidualAttentionBlock(width, n_head, qk_scale=tunables.query_mult*8/math.sqrt(width/n_head)) for _ in range(depth)
+            ResidualAttentionBlock(width, n_head,
+                                   qk_scale=tunables.query_mult*8/math.sqrt(width/n_head), ffn_mult=ffn_mult) for _ in range(depth)
         ])
 
         self.ln_post = LayerNorm(width)
         
     def forward(self, Stoks):
         xin = self.embedding(Stoks)
         
         assert xin.shape[1:] == self.positional_embedding.shape, "incorrect semantic token shape"
         xin = (xin + self.positional_embedding).to(xin.dtype)
 
         return self.ln_post(self.layers(xin))
 
-# %% ../nbs/5. Text to semantic token modeling μP.ipynb 35
+# %% ../nbs/5. Text to semantic token modeling μP.ipynb 36
 class Decoder(nn.Module):
-    def __init__(self, depth=6, width=384, n_head=6, length=1500, codes=1024, pos_embs=None, tunables=Tunables()):
+    def __init__(self, depth=6, width=384, n_head=6, length=1500, codes=1024, ffn_mult=4, pos_embs=None, tunables=Tunables()):
         super().__init__()
         self.length = length
         self.codes = codes
     
         # embed semantic tokens
         self.embedding = nn.Embedding(codes+1, width)
         if pos_embs is None: pos_embs = sinusoids(length, width)
         self.register_buffer("positional_embedding", pos_embs)
         
         self.layers = nn.ModuleList([
-            ResidualAttentionBlock(width, n_head, qk_scale=tunables.query_mult*8/math.sqrt(width/n_head), cross_attention=True) for _ in range(depth)
+            ResidualAttentionBlock(width, n_head, cross_attention=True,
+                                   qk_scale=tunables.query_mult*8/math.sqrt(width/n_head), ffn_mult=ffn_mult) for _ in range(depth)
         ])
         self.ln_post = LayerNorm(width)
         
     def forward(self, Stoks, xenc):
         sot = self.embedding(torch.tensor([self.codes]).to(Stoks.device)).repeat(Stoks.shape[0],1,1)
         if Stoks.shape[-1] > 0:
             if Stoks.shape[-1] >= self.length:
@@ -170,32 +172,33 @@
         for l in self.layers: x = l(x, xenc, causal=True)
         
         x = self.ln_post(x)
         
         logits = (x @ self.embedding.weight.to(x.dtype).T).float()
         return logits
 
-# %% ../nbs/5. Text to semantic token modeling μP.ipynb 36
+# %% ../nbs/5. Text to semantic token modeling μP.ipynb 37
 class TSARTransformer(nn.Module):
-    def __init__(self, depth=6, n_head=6, head_width=64, language='en',
+    def __init__(self, depth=6, n_head=6, head_width=64, ffn_mult=4, language='en',
                  ttoks_len=200, stoks_len=1500, ttoks_codes=50364, stoks_codes=1024,
                  tunables=Tunables()):
         assert language == 'en', "only english is supported right now"
         super().__init__()
         store_attr("depth,n_head,head_width,ttoks_len,stoks_len,ttoks_codes,stoks_codes,language")
 
         width = n_head * head_width
         self.width = width
         self.base_width = 3 * head_width
         self.tunables = tunables
         
         encoder_depth = int(depth * 2 * tunables.encoder_depth_ratio)
         decoder_depth = depth * 2 - encoder_depth
-        self.encoder = Encoder(length=ttoks_len, codes=ttoks_codes, width=width, n_head=n_head, depth=encoder_depth, tunables=tunables)
-        self.decoder = Decoder(length=stoks_len, codes=stoks_codes, width=width, n_head=n_head, depth=decoder_depth, tunables=tunables)
+        tformer_args = dict(width=width, n_head=n_head, ffn_mult=ffn_mult, tunables=tunables)
+        self.encoder = Encoder(length=ttoks_len, codes=ttoks_codes, depth=encoder_depth, **tformer_args)
+        self.decoder = Decoder(length=stoks_len, codes=stoks_codes, depth=decoder_depth, **tformer_args)
         
         self.tokenizer = None
         
         self.apply(self.init_transformer)
 
     def init_transformer(self, m):
         if isinstance(m, LinearHead):
@@ -230,25 +233,35 @@
                 loss = F.cross_entropy(logits.reshape(-1,logits.shape[-1]), Stoks.view(-1))
         return logits, loss
 
     #
     # inference
     #
     @classmethod
-    def load_model(cls, repo_id="collabora/spear-tts-pytorch", filename="t2s.model", local_filename=None):
+    def load_model(cls, repo_id="collabora/whisperspeech", filename="t2s_up.model", local_filename=None):
         if not local_filename:
             local_filename = hf_hub_download(repo_id=repo_id, filename=filename)
         spec = torch.load(local_filename)
-        vqmodel = cls(**spec['config'])
-        vqmodel.load_state_dict(spec['state_dict'])
-        vqmodel.eval()
-        return vqmodel
+        model = cls(**spec['config'], tunables=Tunables(**spec['tunables']))
+        model.load_state_dict(spec['state_dict'])
+        model.eval()
+        return model
+
+    def load_checkpoint(self, local_filename):
+        spec = torch.load(local_filename, map_location='cpu')
+        assert 'pytorch-lightning_version' in spec, 'not a valid PyTorch Lightning checkpoint'
+        state_dict = {k.replace('model.', ''):v
+                      for k,v in spec['state_dict'].items()}
+        self.load_state_dict(state_dict)
+        return self
 
     def save_model(self, fname):
-        torch.save(dict(config = self.__stored_args__, state_dict = self.state_dict()), fname)
+        torch.save(dict(config = self.__stored_args__,
+                        tunables = dataclasses.asdict(self.tunables),
+                        state_dict = self.state_dict()), fname)
 
     def ensure_tokenizer(self):
         assert not self.training
         if self.tokenizer is None: self.tokenizer = whisper.tokenizer.get_tokenizer(multilingual=True)
 
     @property
     def device(self):
@@ -268,18 +281,18 @@
             if top_k:
                 last_p[last_p < torch.topk(last_p, top_k).values[-1,None]] = -torch.inf
             tok = torch.multinomial((last_p / float(T)).softmax(-1), 1)
             toks[0,i] = tok
             if toks[0,i] == 1024: return toks[0,:i]
         return toks[0]
 
-# %% ../nbs/5. Text to semantic token modeling μP.ipynb 37
+# %% ../nbs/5. Text to semantic token modeling μP.ipynb 40
 def make_model(size:str, tunables:Tunables=Tunables(), dataset:SADataset=None):
     kwargs = dict(stoks_len = dataset.stoks_len, ttoks_len = dataset.ttoks_len, tunables=tunables)
     if size == 'micro':
-        return TSARTransformer(depth=3, **kwargs)
+        return TSARTransformer(depth=2, n_head=3, ffn_mult=1, **kwargs)
     if size == 'tiny':
         return TSARTransformer(depth=4, n_head=6, **kwargs)
     if size == 'base':
         return TSARTransformer(depth=6, n_head=8, **kwargs)
     if size == 'small':
         return TSARTransformer(depth=12, n_head=16, **kwargs)
```

### Comparing `whisperspeech-0.0.1/spear_tts_pytorch/train.py` & `WhisperSpeech-0.0.2/whisperspeech/train.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,15 +132,16 @@
         param_groups = groups + [
             {"names": ["other"], "params": list(other_params), "weight_decay": weight_decay },
         ]
 
         optimizer = torch.optim.AdamW(lr=lr, betas=(0.9, 0.95), fused=device!='cpu', params=param_groups)
         scaler = torch.cuda.amp.GradScaler(enabled=half)
         scheduler = torch.optim.lr_scheduler.OneCycleLR(
-            optimizer, max_lr=lr, pct_start=pct_start, steps_per_epoch=len(train_loader), epochs=epochs,
+            optimizer, pct_start=pct_start, steps_per_epoch=len(train_loader), epochs=epochs,
+            max_lr=[pg.get('lr', lr) for pg in param_groups],
             final_div_factor=25)
         
         it = 0
         next_val_it = it + 50
         next_chkpt_it = chkpt_every_iters
         next_table_it = table_row_every_iters
```

### Comparing `whisperspeech-0.0.1/spear_tts_pytorch/train_multi.py` & `WhisperSpeech-0.0.2/whisperspeech/train_multi.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,17 @@
     def __init__(self, model, model_hparams=None):
         super().__init__()
         self.model = model
         self.model_hparams = model_hparams
     
     def configure_optimizers(self):
         """ Initialize AdamW optimizer"""
+        lr = self.model_hparams['lr0']
+        weight_decay = self.model_hparams['weight_decay']
+        
         all_params = set(model.parameters())
         customized_params = set()
         groups = []
         group_map = {}
         for name,m in model.named_modules():
             if hasattr(m, 'no_weight_decay') or hasattr(m, 'lr_scale'):
                 customized_params |= set(m.parameters())
@@ -54,16 +57,15 @@
                 
         other_params = all_params - customized_params
         
         param_groups = groups + [
             {"names": ["other"], "params": list(other_params), "weight_decay": weight_decay },
         ]
 
-        optimizer = torch.optim.AdamW(lr=self.model_hparams['lr0'], betas=(0.9, 0.95),
-                                      fused=True, params=param_groups)
+        optimizer = torch.optim.AdamW(lr=lr, betas=(0.9, 0.95), params=param_groups)
         
         # modified from https://github.com/Lightning-AI/lightning/issues/5449#issuecomment-1501597319
         def num_steps_per_epoch() -> int:
             """Get number of steps"""
             # Accessing _data_source is flaky and might break
             dataset = self.trainer.fit_loop._data_source.dataloader()
             dataset_size = len(dataset)
@@ -74,15 +76,15 @@
         
         total_steps = self.model_hparams['epochs'] * num_steps_per_epoch()
         self.model_hparams['pct_start'] = min(0.3, self.model_hparams['warmup_steps'] / total_steps)
 
         lr_scheduler = torch.optim.lr_scheduler.OneCycleLR(
             optimizer,
             pct_start=self.model_hparams['pct_start'],
-            max_lr=self.model_hparams['lr0'],
+            max_lr=[pg.get('lr', lr) for pg in param_groups],
             steps_per_epoch=num_steps_per_epoch(),
             epochs=self.model_hparams['epochs'],
             final_div_factor=25
         )
 
         return [optimizer], [{'scheduler': lr_scheduler, 'interval': 'step'}]
     
@@ -168,29 +170,29 @@
 # %% ../nbs/B2. Training (Lightning).ipynb 8
 from lightning.pytorch.loggers import WandbLogger
 from lightning.pytorch.callbacks import LearningRateMonitor
 import importlib
 
 torch.set_float32_matmul_precision('medium')
 
-wandb_logger = WandbLogger(project=f"SpearTTS-{task_name}")
+wandb_logger = WandbLogger(project=f"WhisperSpeech-{task_name}")
 
 ckpt_callback = pl.callbacks.ModelCheckpoint(
      dirpath=f'{task_name}-{epochs}e',
      filename=task_name+"-{epoch}-{step}-{val_loss:.2f}",
      monitor="val_loss",
      save_top_k=4,
      every_n_epochs=1,
  )
 
 lr_monitor_callback = LearningRateMonitor(logging_interval='step')
 
 from torch.utils.data import DataLoader
 
-task = importlib.import_module("spear_tts_pytorch."+task_name)
+task = importlib.import_module("whisperspeech."+task_name)
 
 train_ds, val_ds = parse_and_call('dataset', task.load_datasets, input_args)
 
 tunables = None
 if hasattr(task, "Tunables"):
     import dataclasses
     tunables = parse_and_call('tunables', task.Tunables, tunables_args, log_to_wandb=False)
```

### Comparing `whisperspeech-0.0.1/whisperspeech.egg-info/PKG-INFO` & `WhisperSpeech-0.0.2/WhisperSpeech.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
-Name: whisperspeech
-Version: 0.0.1
+Name: WhisperSpeech
+Version: 0.0.2
 Summary: An Open Source text-to-speech system built by inverting Whisper
-Home-page: https://github.com/collabora/whisperspeech
+Home-page: https://github.com/collabora/WhisperSpeech
 Author: Jakub Piotr Cłapa
 Author-email: jpc@collabora.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

