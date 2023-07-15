# Comparing `tmp/medisynth-0.0.1.tar.gz` & `tmp/medisynth-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medisynth-0.0.1.tar", last modified: Sat Jul  8 12:11:00 2023, max compression
+gzip compressed data, was "medisynth-0.0.2.tar", last modified: Sat Jul 15 18:05:57 2023, max compression
```

## Comparing `medisynth-0.0.1.tar` & `medisynth-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 mxochicale  (1000) mxochicale  (1000)        0 2023-07-08 12:11:00.728814 medisynth-0.0.1/
--rw-rw-r--   0 mxochicale  (1000) mxochicale  (1000)     5363 2023-07-08 12:11:00.728814 medisynth-0.0.1/PKG-INFO
--rw-rw-r--   0 mxochicale  (1000) mxochicale  (1000)     4761 2023-07-08 10:06:20.000000 medisynth-0.0.1/README.md
-drwxrwxr-x   0 mxochicale  (1000) mxochicale  (1000)        0 2023-07-08 12:11:00.728814 medisynth-0.0.1/medisynth.egg-info/
--rw-rw-r--   0 mxochicale  (1000) mxochicale  (1000)     5363 2023-07-08 12:11:00.000000 medisynth-0.0.1/medisynth.egg-info/PKG-INFO
--rw-rw-r--   0 mxochicale  (1000) mxochicale  (1000)      198 2023-07-08 12:11:00.000000 medisynth-0.0.1/medisynth.egg-info/SOURCES.txt
--rw-rw-r--   0 mxochicale  (1000) mxochicale  (1000)        1 2023-07-08 12:11:00.000000 medisynth-0.0.1/medisynth.egg-info/dependency_links.txt
--rw-rw-r--   0 mxochicale  (1000) mxochicale  (1000)       35 2023-07-08 12:11:00.000000 medisynth-0.0.1/medisynth.egg-info/requires.txt
--rw-rw-r--   0 mxochicale  (1000) mxochicale  (1000)        1 2023-07-08 12:11:00.000000 medisynth-0.0.1/medisynth.egg-info/top_level.txt
--rw-rw-r--   0 mxochicale  (1000) mxochicale  (1000)       99 2023-07-08 12:08:20.000000 medisynth-0.0.1/pyproject.toml
--rw-rw-r--   0 mxochicale  (1000) mxochicale  (1000)      834 2023-07-08 12:11:00.728814 medisynth-0.0.1/setup.cfg
+drwxrwxr-x   0 mxochicale  (1000) mxochicale  (1000)        0 2023-07-15 18:05:57.972986 medisynth-0.0.2/
+-rw-rw-r--   0 mxochicale  (1000) mxochicale  (1000)     6221 2023-07-15 18:05:57.972986 medisynth-0.0.2/PKG-INFO
+-rw-rw-r--   0 mxochicale  (1000) mxochicale  (1000)     5520 2023-07-15 18:00:31.000000 medisynth-0.0.2/README.md
+drwxrwxr-x   0 mxochicale  (1000) mxochicale  (1000)        0 2023-07-15 18:05:57.972986 medisynth-0.0.2/medisynth.egg-info/
+-rw-rw-r--   0 mxochicale  (1000) mxochicale  (1000)     6221 2023-07-15 18:05:57.000000 medisynth-0.0.2/medisynth.egg-info/PKG-INFO
+-rw-rw-r--   0 mxochicale  (1000) mxochicale  (1000)      188 2023-07-15 18:05:57.000000 medisynth-0.0.2/medisynth.egg-info/SOURCES.txt
+-rw-rw-r--   0 mxochicale  (1000) mxochicale  (1000)        1 2023-07-15 18:05:57.000000 medisynth-0.0.2/medisynth.egg-info/dependency_links.txt
+-rw-rw-r--   0 mxochicale  (1000) mxochicale  (1000)       35 2023-07-15 18:05:57.000000 medisynth-0.0.2/medisynth.egg-info/requires.txt
+-rw-rw-r--   0 mxochicale  (1000) mxochicale  (1000)        1 2023-07-15 18:05:57.000000 medisynth-0.0.2/medisynth.egg-info/top_level.txt
+-rw-rw-r--   0 mxochicale  (1000) mxochicale  (1000)     1018 2023-07-15 18:00:31.000000 medisynth-0.0.2/pyproject.toml
+-rw-rw-r--   0 mxochicale  (1000) mxochicale  (1000)       38 2023-07-15 18:05:57.972986 medisynth-0.0.2/setup.cfg
```

### Comparing `medisynth-0.0.1/PKG-INFO` & `medisynth-0.0.2/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,60 +1,63 @@
-Metadata-Version: 2.1
-Name: medisynth
-Version: 0.0.1
-Summary: Ultrasound Fetal Brain Imaging Synthesis
-Home-page: https://github.com/mxochicale/medisynth
-Author: Harvey Mannering and Miguel Xochicale
-Author-email: your@email.address
-License: MIT
-Keywords: artificial intelligence,diffusion models
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.8
-Description-Content-Type: text/markdown
-
-# medisynth
+# medisynth - library for synthesis of ultrasound fetal imaging (:baby: :brain: :robot:) :warning: WIP :warning:
 [![PyPI version](https://badge.fury.io/py/medisynth.svg)](https://badge.fury.io/py/medisynth)
 
-A library for ultrasound fetal brain imaging using techniques from diffusion models
-
+medisynth is a python-based library to syntheses fetal ultrasound images using GAN, transformers and diffusion models.
+It also includes methods to quantify the quality of synthesis (FID, PSNR, SSIM, and visual touring tests).
 
-## Install
-
-```bash
+## Installation
+```
 $ pip install medisynth
 ```
 
-## Slides
+You can develop locally:
+* Generate your SSH keys as suggested [here](https://docs.github.com/en/github/authenticating-to-github/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent) (or [here](https://github.com/mxochicale/tools/blob/main/github/SSH.md))
+* Clone the repository by typing (or copying) the following line in a terminal at your selected path in your machine:
+```
+cd && mkdir -p $HOME/repositories/budai4medtech && cd  $HOME/repositories/budai4medtech
+git clone git@github.com:budai4medtech/medisynth.git
+```
+
+## References
+### Presentation
 Good practices in AI/ML for Ultrasound Fetal Brain Imaging Synthesis   
 Harvey Mannering, Sofia Miñano, and Miguel Xochicale      
 
 University College London     
 The deep learning and computer vision Journal Club       
 UCL Centre for Advance Research Computing       
 1st of June 2023, 15:00 GMT   
 
-### Abstract
+Abstract
 Medical image datasets for AI and ML methods must be diverse to generalise well unseen data (i.e. diagnoses, diseases, pathologies, scanners, demographics, etc).
 However there are few public ultrasound fetal imaging datasets due to insufficient amounts of clinical data, patient privacy, rare occurrence of abnormalities, and limited experts for data collection and validation.
 To address such challenges in Ultrasound Medical Imaging, Miguel will discuss two proposed generative adversarial networks (GAN)-based models: diffusion-super-resolution-GAN and transformer-based-GAN, to synthesise images of fetal Ultrasound brain image planes from one public dataset.
 Similarly, Miguel will present and discuss AI and ML workflow aligned to good ML practices by FDA, and methods for quality image assessment (e.g., visual Turing test and FID scores).
 Finally, a simple prototype in GitHub, google-colabs and guidelines to train it using Myriad cluster will be presented as well as applications for Medical Image Synthesis e.g., classification, augmentation, segmentation, registration and other downstream tasks, etc. will be discussed.
-The resources to reproduce the work of this talk are available at https://github.com/mxochicale/medisynth.
+The resources to reproduce the work of this talk are available at https://github.com/budai4medtech/medisynth.
 
-## Clone repository
-* Generate your SSH keys as suggested [here](https://docs.github.com/en/github/authenticating-to-github/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent) (or [here](https://github.com/mxochicale/tools/blob/main/github/SSH.md))
-* Clone the repository by typing (or copying) the following line in a terminal at your selected path in your machine:
-```
-cd && mkdir -p $HOME/repositories/$USERNAME && cd  $HOME/repositories/$USERNAME
-git clone git@github.com:mxochicale/medisynth.git
+### Citations
+BibTeX to cite
 ```
-
+@misc{iskandar2023realistic,
+      author={
+      	Michelle Iskandar and 
+      	Harvey Mannering and 
+      	Zhanxiang Sun and 
+      	Jacqueline Matthew and 
+      	Hamideh Kerdegari and 
+      	Laura Peralta and 
+      	Miguel Xochicale},
+      title={Towards Realistic Ultrasound Fetal Brain Imaging Synthesis}, 
+      year={2023},
+      eprint={2304.03941},
+      archivePrefix={arXiv},
+      primaryClass={eess.IV}
+}
+``` 
 
 ## Contributors
 Thanks goes to all these people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):  
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
 <!-- prettier-ignore-start -->
 <!-- markdownlint-disable -->
 <table>
@@ -73,39 +76,39 @@
 	<!-- CONTRIBUTOR -->
 	<td align="center">
 		<a href="https://github.com/sfmig"><img src="https://avatars1.githubusercontent.com/u/33267254?v=4?s=100" width="100px;" alt=""/>
 		<br />
 			<sub> <b>Sofia Miñano</b> </sub>        
 		</a>
 		<br />
-			<a href="https://github.com/mxochicale/medisynth/commits?author=sfmig" title="Code">💻</a> 
-			<a href="https://github.com/mxochicale/medisynth/commits?author=sfmig" title="Research">  🔬 🤔  </a>
+			<a href="https://github.com/budai4medtech/medisynth/commits?author=sfmig" title="Code">💻</a> 
+			<a href="https://github.com/budai4medtech/medisynth/commits?author=sfmig" title="Research">  🔬 🤔  </a>
 	</td>
 	<!-- CONTRIBUTOR -->
 	<td align="center">
 		<a href="https://github.com/harveymannering"><img src="https://avatars1.githubusercontent.com/u/60523103?v=4?s=100" width="100px;" alt=""/>
 		<br />
 			<sub> <b>Harvey Mannering</b> </sub>        
 		</a>
 		<br />
-			<a href="https://github.com/mxochicale/medisynth/commits?author=harveymannering" title="Code">💻</a> 
-			<a href="https://github.com/mxochicale/medisynth/commits?author=harveymannering" title="Research">  🔬 🤔  </a>
+			<a href="https://github.com/budai4medtech/medisynth/commits?author=harveymannering" title="Code">💻</a> 
+			<a href="https://github.com/budai4medtech/medisynth/commits?author=harveymannering" title="Research">  🔬 🤔  </a>
 	</td>
 	<!-- CONTRIBUTOR -->
 	<td align="center">
-		<a href="https://github.com/mxochicale"><img src="https://avatars1.githubusercontent.com/u/11370681?v=4?s=100" width="100px;" alt=""/>
+		<a href="https://github.com/budai4medtech"><img src="https://avatars1.githubusercontent.com/u/11370681?v=4?s=100" width="100px;" alt=""/>
 			<br />
 			<sub><b>Miguel Xochicale</b></sub>          
 			<br />
 		</a>
-			<a href="https://github.com/mxochicale/medisynth/commits?author=mxochicale" title="Code">💻</a> 
-			<a href="ttps://github.com/mxochicale/medisynth/commits?author=mxochicale" title="Documentation">📖  🔧 </a>
+			<a href="https://github.com/budai4medtech/medisynth/commits?author=mxochicale" title="Code">💻</a> 
+			<a href="ttps://github.com/budai4medtech/medisynth/commits?author=mxochicale" title="Documentation">📖  🔧 </a>
 	</td>
   </tr>
 </table>
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
 
 This work follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification.  
-Contributions of any kind welcome!
+Contributions of any kind welcome!
```

#### html2text {}

```diff
@@ -1,47 +1,47 @@
-Metadata-Version: 2.1 Name: medisynth Version: 0.0.1 Summary: Ultrasound Fetal
-Brain Imaging Synthesis Home-page: https://github.com/mxochicale/medisynth
-Author: Harvey Mannering and Miguel Xochicale Author-email: your@email.address
-License: MIT Keywords: artificial intelligence,diffusion models Classifier:
-Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: License :: OSI Approved :: MIT License Classifier: Programming
-Language :: Python :: 3.8 Description-Content-Type: text/markdown # medisynth
-[![PyPI version](https://badge.fury.io/py/medisynth.svg)](https://
-badge.fury.io/py/medisynth) A library for ultrasound fetal brain imaging using
-techniques from diffusion models ## Install ```bash $ pip install medisynth ```
-## Slides Good practices in AI/ML for Ultrasound Fetal Brain Imaging Synthesis
-Harvey Mannering, Sofia MiÃ±ano, and Miguel Xochicale University College London
-The deep learning and computer vision Journal Club UCL Centre for Advance
-Research Computing 1st of June 2023, 15:00 GMT ### Abstract Medical image
-datasets for AI and ML methods must be diverse to generalise well unseen data
-(i.e. diagnoses, diseases, pathologies, scanners, demographics, etc). However
-there are few public ultrasound fetal imaging datasets due to insufficient
-amounts of clinical data, patient privacy, rare occurrence of abnormalities,
-and limited experts for data collection and validation. To address such
-challenges in Ultrasound Medical Imaging, Miguel will discuss two proposed
-generative adversarial networks (GAN)-based models: diffusion-super-resolution-
-GAN and transformer-based-GAN, to synthesise images of fetal Ultrasound brain
-image planes from one public dataset. Similarly, Miguel will present and
-discuss AI and ML workflow aligned to good ML practices by FDA, and methods for
-quality image assessment (e.g., visual Turing test and FID scores). Finally, a
-simple prototype in GitHub, google-colabs and guidelines to train it using
-Myriad cluster will be presented as well as applications for Medical Image
-Synthesis e.g., classification, augmentation, segmentation, registration and
-other downstream tasks, etc. will be discussed. The resources to reproduce the
-work of this talk are available at https://github.com/mxochicale/medisynth. ##
-Clone repository * Generate your SSH keys as suggested [here](https://
-docs.github.com/en/github/authenticating-to-github/generating-a-new-ssh-key-
-and-adding-it-to-the-ssh-agent) (or [here](https://github.com/mxochicale/tools/
-blob/main/github/SSH.md)) * Clone the repository by typing (or copying) the
-following line in a terminal at your selected path in your machine: ``` cd &&
-mkdir -p $HOME/repositories/$USERNAME && cd $HOME/repositories/$USERNAME git
-clone git@github.com:mxochicale/medisynth.git ``` ## Contributors Thanks goes
-to all these people ([emoji key](https://allcontributors.org/docs/en/emoji-
-key)):
+# medisynth - library for synthesis of ultrasound fetal imaging (:baby: :brain:
+:robot:) :warning: WIP :warning: [![PyPI version](https://badge.fury.io/py/
+medisynth.svg)](https://badge.fury.io/py/medisynth) medisynth is a python-based
+library to syntheses fetal ultrasound images using GAN, transformers and
+diffusion models. It also includes methods to quantify the quality of synthesis
+(FID, PSNR, SSIM, and visual touring tests). ## Installation ``` $ pip install
+medisynth ``` You can develop locally: * Generate your SSH keys as suggested
+[here](https://docs.github.com/en/github/authenticating-to-github/generating-a-
+new-ssh-key-and-adding-it-to-the-ssh-agent) (or [here](https://github.com/
+mxochicale/tools/blob/main/github/SSH.md)) * Clone the repository by typing (or
+copying) the following line in a terminal at your selected path in your
+machine: ``` cd && mkdir -p $HOME/repositories/budai4medtech && cd $HOME/
+repositories/budai4medtech git clone git@github.com:budai4medtech/medisynth.git
+``` ## References ### Presentation Good practices in AI/ML for Ultrasound Fetal
+Brain Imaging Synthesis Harvey Mannering, Sofia MiÃ±ano, and Miguel Xochicale
+University College London The deep learning and computer vision Journal Club
+UCL Centre for Advance Research Computing 1st of June 2023, 15:00 GMT Abstract
+Medical image datasets for AI and ML methods must be diverse to generalise well
+unseen data (i.e. diagnoses, diseases, pathologies, scanners, demographics,
+etc). However there are few public ultrasound fetal imaging datasets due to
+insufficient amounts of clinical data, patient privacy, rare occurrence of
+abnormalities, and limited experts for data collection and validation. To
+address such challenges in Ultrasound Medical Imaging, Miguel will discuss two
+proposed generative adversarial networks (GAN)-based models: diffusion-super-
+resolution-GAN and transformer-based-GAN, to synthesise images of fetal
+Ultrasound brain image planes from one public dataset. Similarly, Miguel will
+present and discuss AI and ML workflow aligned to good ML practices by FDA, and
+methods for quality image assessment (e.g., visual Turing test and FID scores).
+Finally, a simple prototype in GitHub, google-colabs and guidelines to train it
+using Myriad cluster will be presented as well as applications for Medical
+Image Synthesis e.g., classification, augmentation, segmentation, registration
+and other downstream tasks, etc. will be discussed. The resources to reproduce
+the work of this talk are available at https://github.com/budai4medtech/
+medisynth. ### Citations BibTeX to cite ``` @misc{iskandar2023realistic,
+author={ Michelle Iskandar and Harvey Mannering and Zhanxiang Sun and
+Jacqueline Matthew and Hamideh Kerdegari and Laura Peralta and Miguel
+Xochicale}, title={Towards Realistic Ultrasound Fetal Brain Imaging Synthesis},
+year={2023}, eprint={2304.03941}, archivePrefix={arXiv}, primaryClass={eess.IV}
+} ``` ## Contributors Thanks goes to all these people ([emoji key](https://
+allcontributors.org/docs/en/emoji-key)):
 
                          Sofia_MiÃ±ano           Harvey_Mannering
  ADD_NAME_SURNAME                                                             Miguel_Xochicale
                          ð» ð¬_ð�      ð» ð¬_ð�       ð» ð_ð§
      ð¬_ð¤
    This work follows the [all-contributors](https://github.com/all-
 contributors/all-contributors) specification. Contributions of any kind
```

### Comparing `medisynth-0.0.1/medisynth.egg-info/PKG-INFO` & `medisynth-0.0.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,60 +1,79 @@
 Metadata-Version: 2.1
 Name: medisynth
-Version: 0.0.1
-Summary: Ultrasound Fetal Brain Imaging Synthesis
-Home-page: https://github.com/mxochicale/medisynth
-Author: Harvey Mannering and Miguel Xochicale
-Author-email: your@email.address
+Version: 0.0.2
+Summary: Python-based library for Synthesis of Ultrasound Fetal Imaging
+Author-email: Harvey Mannering <your@email.com>, Sofía Miñano <your@email.com>, Miguel Xochicale <your@email.com>
 License: MIT
+Project-URL: homepage, https://github.com/budai4medtech/medisynth
 Keywords: artificial intelligence,diffusion models
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 
-# medisynth
+# medisynth - library for synthesis of ultrasound fetal imaging (:baby: :brain: :robot:) :warning: WIP :warning:
 [![PyPI version](https://badge.fury.io/py/medisynth.svg)](https://badge.fury.io/py/medisynth)
 
-A library for ultrasound fetal brain imaging using techniques from diffusion models
+medisynth is a python-based library to syntheses fetal ultrasound images using GAN, transformers and diffusion models.
+It also includes methods to quantify the quality of synthesis (FID, PSNR, SSIM, and visual touring tests).
 
-
-## Install
-
-```bash
+## Installation
+```
 $ pip install medisynth
 ```
 
-## Slides
+You can develop locally:
+* Generate your SSH keys as suggested [here](https://docs.github.com/en/github/authenticating-to-github/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent) (or [here](https://github.com/mxochicale/tools/blob/main/github/SSH.md))
+* Clone the repository by typing (or copying) the following line in a terminal at your selected path in your machine:
+```
+cd && mkdir -p $HOME/repositories/budai4medtech && cd  $HOME/repositories/budai4medtech
+git clone git@github.com:budai4medtech/medisynth.git
+```
+
+## References
+### Presentation
 Good practices in AI/ML for Ultrasound Fetal Brain Imaging Synthesis   
 Harvey Mannering, Sofia Miñano, and Miguel Xochicale      
 
 University College London     
 The deep learning and computer vision Journal Club       
 UCL Centre for Advance Research Computing       
 1st of June 2023, 15:00 GMT   
 
-### Abstract
+Abstract
 Medical image datasets for AI and ML methods must be diverse to generalise well unseen data (i.e. diagnoses, diseases, pathologies, scanners, demographics, etc).
 However there are few public ultrasound fetal imaging datasets due to insufficient amounts of clinical data, patient privacy, rare occurrence of abnormalities, and limited experts for data collection and validation.
 To address such challenges in Ultrasound Medical Imaging, Miguel will discuss two proposed generative adversarial networks (GAN)-based models: diffusion-super-resolution-GAN and transformer-based-GAN, to synthesise images of fetal Ultrasound brain image planes from one public dataset.
 Similarly, Miguel will present and discuss AI and ML workflow aligned to good ML practices by FDA, and methods for quality image assessment (e.g., visual Turing test and FID scores).
 Finally, a simple prototype in GitHub, google-colabs and guidelines to train it using Myriad cluster will be presented as well as applications for Medical Image Synthesis e.g., classification, augmentation, segmentation, registration and other downstream tasks, etc. will be discussed.
-The resources to reproduce the work of this talk are available at https://github.com/mxochicale/medisynth.
+The resources to reproduce the work of this talk are available at https://github.com/budai4medtech/medisynth.
 
-## Clone repository
-* Generate your SSH keys as suggested [here](https://docs.github.com/en/github/authenticating-to-github/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent) (or [here](https://github.com/mxochicale/tools/blob/main/github/SSH.md))
-* Clone the repository by typing (or copying) the following line in a terminal at your selected path in your machine:
-```
-cd && mkdir -p $HOME/repositories/$USERNAME && cd  $HOME/repositories/$USERNAME
-git clone git@github.com:mxochicale/medisynth.git
+### Citations
+BibTeX to cite
 ```
-
+@misc{iskandar2023realistic,
+      author={
+      	Michelle Iskandar and 
+      	Harvey Mannering and 
+      	Zhanxiang Sun and 
+      	Jacqueline Matthew and 
+      	Hamideh Kerdegari and 
+      	Laura Peralta and 
+      	Miguel Xochicale},
+      title={Towards Realistic Ultrasound Fetal Brain Imaging Synthesis}, 
+      year={2023},
+      eprint={2304.03941},
+      archivePrefix={arXiv},
+      primaryClass={eess.IV}
+}
+``` 
 
 ## Contributors
 Thanks goes to all these people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):  
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
 <!-- prettier-ignore-start -->
 <!-- markdownlint-disable -->
 <table>
@@ -73,36 +92,36 @@
 	<!-- CONTRIBUTOR -->
 	<td align="center">
 		<a href="https://github.com/sfmig"><img src="https://avatars1.githubusercontent.com/u/33267254?v=4?s=100" width="100px;" alt=""/>
 		<br />
 			<sub> <b>Sofia Miñano</b> </sub>        
 		</a>
 		<br />
-			<a href="https://github.com/mxochicale/medisynth/commits?author=sfmig" title="Code">💻</a> 
-			<a href="https://github.com/mxochicale/medisynth/commits?author=sfmig" title="Research">  🔬 🤔  </a>
+			<a href="https://github.com/budai4medtech/medisynth/commits?author=sfmig" title="Code">💻</a> 
+			<a href="https://github.com/budai4medtech/medisynth/commits?author=sfmig" title="Research">  🔬 🤔  </a>
 	</td>
 	<!-- CONTRIBUTOR -->
 	<td align="center">
 		<a href="https://github.com/harveymannering"><img src="https://avatars1.githubusercontent.com/u/60523103?v=4?s=100" width="100px;" alt=""/>
 		<br />
 			<sub> <b>Harvey Mannering</b> </sub>        
 		</a>
 		<br />
-			<a href="https://github.com/mxochicale/medisynth/commits?author=harveymannering" title="Code">💻</a> 
-			<a href="https://github.com/mxochicale/medisynth/commits?author=harveymannering" title="Research">  🔬 🤔  </a>
+			<a href="https://github.com/budai4medtech/medisynth/commits?author=harveymannering" title="Code">💻</a> 
+			<a href="https://github.com/budai4medtech/medisynth/commits?author=harveymannering" title="Research">  🔬 🤔  </a>
 	</td>
 	<!-- CONTRIBUTOR -->
 	<td align="center">
-		<a href="https://github.com/mxochicale"><img src="https://avatars1.githubusercontent.com/u/11370681?v=4?s=100" width="100px;" alt=""/>
+		<a href="https://github.com/budai4medtech"><img src="https://avatars1.githubusercontent.com/u/11370681?v=4?s=100" width="100px;" alt=""/>
 			<br />
 			<sub><b>Miguel Xochicale</b></sub>          
 			<br />
 		</a>
-			<a href="https://github.com/mxochicale/medisynth/commits?author=mxochicale" title="Code">💻</a> 
-			<a href="ttps://github.com/mxochicale/medisynth/commits?author=mxochicale" title="Documentation">📖  🔧 </a>
+			<a href="https://github.com/budai4medtech/medisynth/commits?author=mxochicale" title="Code">💻</a> 
+			<a href="ttps://github.com/budai4medtech/medisynth/commits?author=mxochicale" title="Documentation">📖  🔧 </a>
 	</td>
   </tr>
 </table>
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
```

#### html2text {}

```diff
@@ -1,47 +1,58 @@
-Metadata-Version: 2.1 Name: medisynth Version: 0.0.1 Summary: Ultrasound Fetal
-Brain Imaging Synthesis Home-page: https://github.com/mxochicale/medisynth
-Author: Harvey Mannering and Miguel Xochicale Author-email: your@email.address
-License: MIT Keywords: artificial intelligence,diffusion models Classifier:
-Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: License :: OSI Approved :: MIT License Classifier: Programming
-Language :: Python :: 3.8 Description-Content-Type: text/markdown # medisynth
-[![PyPI version](https://badge.fury.io/py/medisynth.svg)](https://
-badge.fury.io/py/medisynth) A library for ultrasound fetal brain imaging using
-techniques from diffusion models ## Install ```bash $ pip install medisynth ```
-## Slides Good practices in AI/ML for Ultrasound Fetal Brain Imaging Synthesis
-Harvey Mannering, Sofia MiÃ±ano, and Miguel Xochicale University College London
-The deep learning and computer vision Journal Club UCL Centre for Advance
-Research Computing 1st of June 2023, 15:00 GMT ### Abstract Medical image
-datasets for AI and ML methods must be diverse to generalise well unseen data
-(i.e. diagnoses, diseases, pathologies, scanners, demographics, etc). However
-there are few public ultrasound fetal imaging datasets due to insufficient
-amounts of clinical data, patient privacy, rare occurrence of abnormalities,
-and limited experts for data collection and validation. To address such
-challenges in Ultrasound Medical Imaging, Miguel will discuss two proposed
-generative adversarial networks (GAN)-based models: diffusion-super-resolution-
-GAN and transformer-based-GAN, to synthesise images of fetal Ultrasound brain
-image planes from one public dataset. Similarly, Miguel will present and
-discuss AI and ML workflow aligned to good ML practices by FDA, and methods for
-quality image assessment (e.g., visual Turing test and FID scores). Finally, a
-simple prototype in GitHub, google-colabs and guidelines to train it using
-Myriad cluster will be presented as well as applications for Medical Image
-Synthesis e.g., classification, augmentation, segmentation, registration and
-other downstream tasks, etc. will be discussed. The resources to reproduce the
-work of this talk are available at https://github.com/mxochicale/medisynth. ##
-Clone repository * Generate your SSH keys as suggested [here](https://
-docs.github.com/en/github/authenticating-to-github/generating-a-new-ssh-key-
-and-adding-it-to-the-ssh-agent) (or [here](https://github.com/mxochicale/tools/
-blob/main/github/SSH.md)) * Clone the repository by typing (or copying) the
-following line in a terminal at your selected path in your machine: ``` cd &&
-mkdir -p $HOME/repositories/$USERNAME && cd $HOME/repositories/$USERNAME git
-clone git@github.com:mxochicale/medisynth.git ``` ## Contributors Thanks goes
-to all these people ([emoji key](https://allcontributors.org/docs/en/emoji-
-key)):
+Metadata-Version: 2.1 Name: medisynth Version: 0.0.2 Summary: Python-based
+library for Synthesis of Ultrasound Fetal Imaging Author-email: Harvey
+Mannering
+email.com>, SofÃ­a MiÃ±ano
+email.com>, Miguel Xochicale
+email.com> License: MIT Project-URL: homepage, https://github.com/
+budai4medtech/medisynth Keywords: artificial intelligence,diffusion models
+Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended Audience
+:: Developers Classifier: Topic :: Scientific/Engineering :: Artificial
+Intelligence Classifier: License :: OSI Approved :: MIT License Classifier:
+Programming Language :: Python :: 3.8 Requires-Python: >=3.11 Description-
+Content-Type: text/markdown # medisynth - library for synthesis of ultrasound
+fetal imaging (:baby: :brain: :robot:) :warning: WIP :warning: [![PyPI version]
+(https://badge.fury.io/py/medisynth.svg)](https://badge.fury.io/py/medisynth)
+medisynth is a python-based library to syntheses fetal ultrasound images using
+GAN, transformers and diffusion models. It also includes methods to quantify
+the quality of synthesis (FID, PSNR, SSIM, and visual touring tests). ##
+Installation ``` $ pip install medisynth ``` You can develop locally: *
+Generate your SSH keys as suggested [here](https://docs.github.com/en/github/
+authenticating-to-github/generating-a-new-ssh-key-and-adding-it-to-the-ssh-
+agent) (or [here](https://github.com/mxochicale/tools/blob/main/github/SSH.md))
+* Clone the repository by typing (or copying) the following line in a terminal
+at your selected path in your machine: ``` cd && mkdir -p $HOME/repositories/
+budai4medtech && cd $HOME/repositories/budai4medtech git clone git@github.com:
+budai4medtech/medisynth.git ``` ## References ### Presentation Good practices
+in AI/ML for Ultrasound Fetal Brain Imaging Synthesis Harvey Mannering, Sofia
+MiÃ±ano, and Miguel Xochicale University College London The deep learning and
+computer vision Journal Club UCL Centre for Advance Research Computing 1st of
+June 2023, 15:00 GMT Abstract Medical image datasets for AI and ML methods must
+be diverse to generalise well unseen data (i.e. diagnoses, diseases,
+pathologies, scanners, demographics, etc). However there are few public
+ultrasound fetal imaging datasets due to insufficient amounts of clinical data,
+patient privacy, rare occurrence of abnormalities, and limited experts for data
+collection and validation. To address such challenges in Ultrasound Medical
+Imaging, Miguel will discuss two proposed generative adversarial networks
+(GAN)-based models: diffusion-super-resolution-GAN and transformer-based-GAN,
+to synthesise images of fetal Ultrasound brain image planes from one public
+dataset. Similarly, Miguel will present and discuss AI and ML workflow aligned
+to good ML practices by FDA, and methods for quality image assessment (e.g.,
+visual Turing test and FID scores). Finally, a simple prototype in GitHub,
+google-colabs and guidelines to train it using Myriad cluster will be presented
+as well as applications for Medical Image Synthesis e.g., classification,
+augmentation, segmentation, registration and other downstream tasks, etc. will
+be discussed. The resources to reproduce the work of this talk are available at
+https://github.com/budai4medtech/medisynth. ### Citations BibTeX to cite ```
+@misc{iskandar2023realistic, author={ Michelle Iskandar and Harvey Mannering
+and Zhanxiang Sun and Jacqueline Matthew and Hamideh Kerdegari and Laura
+Peralta and Miguel Xochicale}, title={Towards Realistic Ultrasound Fetal Brain
+Imaging Synthesis}, year={2023}, eprint={2304.03941}, archivePrefix={arXiv},
+primaryClass={eess.IV} } ``` ## Contributors Thanks goes to all these people (
+[emoji key](https://allcontributors.org/docs/en/emoji-key)):
 
                          Sofia_MiÃ±ano           Harvey_Mannering
  ADD_NAME_SURNAME                                                             Miguel_Xochicale
                          ð» ð¬_ð�      ð» ð¬_ð�       ð» ð_ð§
      ð¬_ð¤
    This work follows the [all-contributors](https://github.com/all-
 contributors/all-contributors) specification. Contributions of any kind
```

