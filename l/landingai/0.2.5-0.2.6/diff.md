# Comparing `tmp/landingai-0.2.5.tar.gz` & `tmp/landingai-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "landingai-0.2.5.tar", max compression
+gzip compressed data, was "landingai-0.2.6.tar", max compression
```

## Comparing `landingai-0.2.5.tar` & `landingai-0.2.6.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0     1063 2023-07-14 12:14:28.628564 landingai-0.2.5/LICENSE.md
--rw-r--r--   0        0        0     6743 2023-07-14 12:14:28.628564 landingai-0.2.5/README.md
--rw-r--r--   0        0        0      354 2023-07-14 12:14:28.660565 landingai-0.2.5/landingai/__init__.py
--rw-r--r--   0        0        0     6451 2023-07-14 12:14:28.660565 landingai-0.2.5/landingai/common.py
--rw-r--r--   0        0        0       72 2023-07-14 12:14:28.660565 landingai-0.2.5/landingai/data_management/__init__.py
--rw-r--r--   0        0        0     8714 2023-07-14 12:14:28.660565 landingai-0.2.5/landingai/data_management/client.py
--rw-r--r--   0        0        0    21135 2023-07-14 12:14:28.660565 landingai-0.2.5/landingai/data_management/media.py
--rw-r--r--   0        0        0     4722 2023-07-14 12:14:28.660565 landingai-0.2.5/landingai/data_management/metadata.py
--rw-r--r--   0        0        0     2188 2023-07-14 12:14:28.660565 landingai-0.2.5/landingai/data_management/utils.py
--rw-r--r--   0        0        0     9730 2023-07-14 12:14:28.660565 landingai-0.2.5/landingai/exceptions.py
--rw-r--r--   0        0        0  1594400 2023-07-14 12:14:28.668565 landingai-0.2.5/landingai/fonts/default_font_ch_en.ttf
--rw-r--r--   0        0        0     4750 2023-07-14 12:14:28.668565 landingai-0.2.5/landingai/notebook_utils.py
--rw-r--r--   0        0        0      420 2023-07-14 12:14:28.668565 landingai-0.2.5/landingai/pipeline/__init__.py
--rw-r--r--   0        0        0    16449 2023-07-14 12:14:28.672565 landingai-0.2.5/landingai/pipeline/frameset.py
--rw-r--r--   0        0        0    17016 2023-07-14 12:14:28.672565 landingai-0.2.5/landingai/pipeline/image_source.py
--rw-r--r--   0        0        0     1339 2023-07-14 12:14:28.672565 landingai-0.2.5/landingai/pipeline/postprocessing.py
--rw-r--r--   0        0        0     8389 2023-07-14 12:14:28.672565 landingai-0.2.5/landingai/postprocess.py
--rw-r--r--   0        0        0    25559 2023-07-14 12:14:28.672565 landingai-0.2.5/landingai/predict.py
--rw-r--r--   0        0        0     6462 2023-07-14 12:14:28.672565 landingai-0.2.5/landingai/st_utils.py
--rw-r--r--   0        0        0       40 2023-07-14 12:14:28.672565 landingai-0.2.5/landingai/storage/__init__.py
--rw-r--r--   0        0        0     4439 2023-07-14 12:14:28.672565 landingai-0.2.5/landingai/storage/data_access.py
--rw-r--r--   0        0        0     4340 2023-07-14 12:14:28.672565 landingai-0.2.5/landingai/storage/snowflake.py
--rw-r--r--   0        0        0     1503 2023-07-14 12:14:28.672565 landingai-0.2.5/landingai/telemetry.py
--rw-r--r--   0        0        0     1685 2023-07-14 12:14:28.672565 landingai-0.2.5/landingai/transform.py
--rw-r--r--   0        0        0     1598 2023-07-14 12:14:28.672565 landingai-0.2.5/landingai/utils.py
--rw-r--r--   0        0        0    13403 2023-07-14 12:14:28.672565 landingai-0.2.5/landingai/visualize.py
--rw-r--r--   0        0        0     2606 2023-07-14 12:14:29.360574 landingai-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     7988 1970-01-01 00:00:00.000000 landingai-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-07-14 23:22:44.010675 landingai-0.2.6/LICENSE.md
+-rw-r--r--   0        0        0     6743 2023-07-14 23:22:44.010675 landingai-0.2.6/README.md
+-rw-r--r--   0        0        0      354 2023-07-14 23:22:44.046676 landingai-0.2.6/landingai/__init__.py
+-rw-r--r--   0        0        0     6451 2023-07-14 23:22:44.046676 landingai-0.2.6/landingai/common.py
+-rw-r--r--   0        0        0       72 2023-07-14 23:22:44.046676 landingai-0.2.6/landingai/data_management/__init__.py
+-rw-r--r--   0        0        0     8714 2023-07-14 23:22:44.046676 landingai-0.2.6/landingai/data_management/client.py
+-rw-r--r--   0        0        0    21135 2023-07-14 23:22:44.046676 landingai-0.2.6/landingai/data_management/media.py
+-rw-r--r--   0        0        0     4722 2023-07-14 23:22:44.046676 landingai-0.2.6/landingai/data_management/metadata.py
+-rw-r--r--   0        0        0     2188 2023-07-14 23:22:44.046676 landingai-0.2.6/landingai/data_management/utils.py
+-rw-r--r--   0        0        0     9730 2023-07-14 23:22:44.046676 landingai-0.2.6/landingai/exceptions.py
+-rw-r--r--   0        0        0  1594400 2023-07-14 23:22:44.058676 landingai-0.2.6/landingai/fonts/default_font_ch_en.ttf
+-rw-r--r--   0        0        0     5915 2023-07-14 23:22:44.058676 landingai-0.2.6/landingai/image_source_ops.py
+-rw-r--r--   0        0        0     1502 2023-07-14 23:22:44.058676 landingai-0.2.6/landingai/notebook_utils.py
+-rw-r--r--   0        0        0      420 2023-07-14 23:22:44.058676 landingai-0.2.6/landingai/pipeline/__init__.py
+-rw-r--r--   0        0        0    16449 2023-07-14 23:22:44.058676 landingai-0.2.6/landingai/pipeline/frameset.py
+-rw-r--r--   0        0        0    11810 2023-07-14 23:22:44.058676 landingai-0.2.6/landingai/pipeline/image_source.py
+-rw-r--r--   0        0        0     1339 2023-07-14 23:22:44.058676 landingai-0.2.6/landingai/pipeline/postprocessing.py
+-rw-r--r--   0        0        0     8389 2023-07-14 23:22:44.058676 landingai-0.2.6/landingai/postprocess.py
+-rw-r--r--   0        0        0    25559 2023-07-14 23:22:44.058676 landingai-0.2.6/landingai/predict.py
+-rw-r--r--   0        0        0     6462 2023-07-14 23:22:44.058676 landingai-0.2.6/landingai/st_utils.py
+-rw-r--r--   0        0        0       40 2023-07-14 23:22:44.058676 landingai-0.2.6/landingai/storage/__init__.py
+-rw-r--r--   0        0        0     4439 2023-07-14 23:22:44.058676 landingai-0.2.6/landingai/storage/data_access.py
+-rw-r--r--   0        0        0     4340 2023-07-14 23:22:44.058676 landingai-0.2.6/landingai/storage/snowflake.py
+-rw-r--r--   0        0        0     1503 2023-07-14 23:22:44.058676 landingai-0.2.6/landingai/telemetry.py
+-rw-r--r--   0        0        0     1685 2023-07-14 23:22:44.058676 landingai-0.2.6/landingai/transform.py
+-rw-r--r--   0        0        0     1598 2023-07-14 23:22:44.058676 landingai-0.2.6/landingai/utils.py
+-rw-r--r--   0        0        0    13403 2023-07-14 23:22:44.058676 landingai-0.2.6/landingai/visualize.py
+-rw-r--r--   0        0        0     2606 2023-07-14 23:22:44.886702 landingai-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     7988 1970-01-01 00:00:00.000000 landingai-0.2.6/PKG-INFO
```

### Comparing `landingai-0.2.5/LICENSE.md` & `landingai-0.2.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `landingai-0.2.5/README.md` & `landingai-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `landingai-0.2.5/landingai/common.py` & `landingai-0.2.6/landingai/common.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.5/landingai/data_management/client.py` & `landingai-0.2.6/landingai/data_management/client.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.5/landingai/data_management/media.py` & `landingai-0.2.6/landingai/data_management/media.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.5/landingai/data_management/metadata.py` & `landingai-0.2.6/landingai/data_management/metadata.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.5/landingai/data_management/utils.py` & `landingai-0.2.6/landingai/data_management/utils.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.5/landingai/exceptions.py` & `landingai-0.2.6/landingai/exceptions.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.5/landingai/fonts/default_font_ch_en.ttf` & `landingai-0.2.6/landingai/fonts/default_font_ch_en.ttf`

 * *Files identical despite different names*

### Comparing `landingai-0.2.5/landingai/notebook_utils.py` & `landingai-0.2.6/landingai/image_source_ops.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,62 +1,92 @@
-"""This module contains common notebook utilities that are used across the example notebooks in this repo.
-It's only intended for examples provided by this repo. When using the SDK in your own project, you don't need to use this module.
-"""
-import tempfile
-from functools import lru_cache
-from pathlib import Path
-from typing import Callable, Union
-
-
-def is_running_in_colab_notebook() -> bool:
-    """Return True if the code is running in a Google Colab notebook."""
-    try:
-        from IPython import get_ipython
+"""Operations (create, probe, save, etc) around images, videos from various sources (webcam, video, RTSP stream etc)."""
 
-        return get_ipython().__class__.__module__ == "google.colab._shell"  # type: ignore
-    except ImportError:
-        return False  # Probably standard Python interpreter
-
-
-def is_running_in_jupyter_notebook() -> bool:
-    """Return True if the code is running in a Jupyter notebook."""
-    try:
-        from IPython import get_ipython
+import io
+from pathlib import Path
+from typing import List, Optional, Tuple, Union
 
-        # See: https://stackoverflow.com/questions/15411967/how-can-i-check-if-code-is-executed-in-the-ipython-notebook
-        shell = get_ipython().__class__.__name__
-        if shell == "ZMQInteractiveShell":
-            return True  # Jupyter notebook or qtconsole
-        elif shell == "TerminalInteractiveShell":
-            return False  # Terminal running IPython
-        else:
-            return False  # Other type (?)
-    except ImportError:
-        return False  # Probably standard Python interpreter
-
-
-@lru_cache(maxsize=None)
-def is_running_in_notebook() -> bool:
-    """Return True if the code is running in a notebook."""
-    return is_running_in_colab_notebook() or is_running_in_jupyter_notebook()
-
-
-def read_from_notebook_webcam(webcam_source: Union[str, int] = 0) -> Callable[[], str]:
-    """Return a function that reads an image from the webcam in notebook."""
-    # Define function to acquire images either directly from the local webcam (i.e. jupyter notebook)or from the web browser (i.e. collab)
-    local_cache_dir = Path(tempfile.mkdtemp())
-    filename = str(local_cache_dir / "photo.jpg")
-    # Detect if we are running on Google's colab
+import cv2
+import numpy as np
+import PIL.Image
+
+
+def probe_video(video_file: str, samples_per_second: float) -> Tuple[int, int, float]:
+    """Probe a video file to get some metadata before sampling images.
+    Parameters
+    ----------
+    video_file: The local path to the video file
+    samples_per_second: Number of images to sample per second
+    Returns
+    -------
+    A tuple of three values
+        - The total number of frames,
+        - The number of frames to sample,
+        - The video length in seconds.
+    """
+    if not Path(video_file).exists():
+        raise FileNotFoundError(f"Video file {video_file} does not exist.")
+    cap = cv2.VideoCapture(video_file)
+    fps = cap.get(cv2.CAP_PROP_FPS)
+    total_frames = int(cap.get(cv2.CAP_PROP_FRAME_COUNT))
+    video_length_seconds = total_frames / fps
+    sample_size = int(video_length_seconds * samples_per_second)
+    cap.release()
+    return (total_frames, sample_size, video_length_seconds)
+
+
+def sample_images_from_video(
+    video_file: str, output_dir: Path, samples_per_second: float = 1
+) -> List[str]:
+    """Sample images from a video file.
+    Parameters
+    ----------
+    video_file: The local path to the video file
+    output_dir: The local directory path that stores the sampled images
+    samples_per_second: The number of images to sample per second
+    Returns
+    -------
+    a list of local file paths to the sampled images
+    """
+    output_dir.mkdir(parents=True, exist_ok=True)
+    total_frames, sample_size, _ = probe_video(video_file, samples_per_second)
+    # Calculate the frame interval based on the desired frame rate
+    sample_interval = int(total_frames / sample_size)
+    frame_count = 0
+    output = []
+    cap = cv2.VideoCapture(video_file)
+    while cap.isOpened():
+        ret, frame = cap.read()
+        # Check if end of video file
+        if not ret:
+            break
+        # Check if the current frame should be saved
+        if frame_count % sample_interval == 0:
+            output_file_path = str(output_dir / f"{frame_count}.jpg")
+            cv2.imwrite(output_file_path, frame)
+            output.append(output_file_path)
+        frame_count += 1
+    cap.release()
+    return output
+
+
+def take_photo_from_webcam(webcam_source: Union[str, int] = 0) -> PIL.Image.Image:
+    """Open a Window and allow users to take a photo from the webcam.
+    It supports running on both local environment and Google's colab notebooks.
+    For Google colab, it will open a window to allow users to take a photo from the webcam by pressing the "Capture" button.
+    For local environment, it will open a window to allow users to take a photo from the webcam by pressing the "space" button.
+    """
     try:
+        # Running on Google's colab or local Jupyter notebook
         from base64 import b64decode
 
         from google.colab.output import eval_js  # type: ignore
         from IPython.display import Javascript, display
 
-        def take_photo() -> str:
+        # Define function to acquire images either directly from the local webcam (i.e. jupyter notebook)or from the web browser (i.e. collab)
+        def take_photo() -> PIL.Image.Image:
             quality = 0.8
             js = Javascript(
                 """
             async function takePhoto(quality) {
                 const div = document.createElement('div');
                 const capture = document.createElement('button');
                 capture.textContent = 'Capture';
@@ -86,37 +116,36 @@
                 return canvas.toDataURL('image/jpeg', quality);
             }
             """
             )
             display(js)
             data = eval_js("takePhoto({})".format(quality))
             binary = b64decode(data.split(",")[1])
-            with open(filename, "wb") as f:
-                f.write(binary)
-                return filename
+            return PIL.Image.open(io.BytesIO(binary))
 
     except ModuleNotFoundError:
         # Capture image from local webcam using OpenCV
         import cv2
 
-        def take_photo() -> str:
+        def take_photo() -> PIL.Image.Image:
             cam = cv2.VideoCapture(webcam_source)
             cv2.namedWindow("Press space to take photo")
             cv2.startWindowThread()
+            captured_frame: Optional[np.ndarray] = None
             while True:
                 ret, frame = cam.read()
                 if not ret:
                     print("failed to grab frame")
                     exit()
                 cv2.imshow("Press space to take photo", frame)
                 k = cv2.waitKey(1)
                 if k % 256 == 32:
                     # SPACE pressed
-                    cv2.imwrite(filename, frame)
+                    captured_frame = cv2.cvtColor(frame, cv2.COLOR_BGR2RGB)
                     break
             cam.release()
             cv2.waitKey(1)
             cv2.destroyAllWindows()
             cv2.waitKey(1)
-            return filename
+            return PIL.Image.fromarray(captured_frame)
 
-    return take_photo
+    return take_photo()
```

### Comparing `landingai-0.2.5/landingai/pipeline/frameset.py` & `landingai-0.2.6/landingai/pipeline/frameset.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.5/landingai/pipeline/image_source.py` & `landingai-0.2.6/landingai/pipeline/image_source.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,22 +4,23 @@
 import shutil
 import tempfile
 import threading
 import time
 from collections.abc import Iterator
 from datetime import datetime
 from pathlib import Path
-from typing import Any, Callable
+from typing import Any
 from typing import Iterator as IteratorType
-from typing import List, Optional, Tuple, Union
+from typing import List, Optional, Union
 
 import cv2
 import numpy as np
 from pydantic import BaseModel, PrivateAttr
 
+from landingai.image_source_ops import sample_images_from_video
 from landingai.pipeline.frameset import Frame, FrameSet
 from landingai.storage.data_access import fetch_from_uri
 
 
 class ImageSourceBase(Iterator):
     """The base class for all image sources."""
 
@@ -107,73 +108,14 @@
 
     @property
     def image_paths(self) -> List[str]:
         """Returns a list of image paths."""
         return self._image_paths
 
 
-def probe_video(video_file: str, samples_per_second: float) -> Tuple[int, int, float]:
-    """Probe a video file to get some metadata before sampling images.
-    Parameters
-    ----------
-    video_file: The local path to the video file
-    samples_per_second: Number of images to sample per second
-    Returns
-    -------
-    A tuple of three values
-        - The total number of frames,
-        - The number of frames to sample,
-        - The video length in seconds.
-    """
-    if not Path(video_file).exists():
-        raise FileNotFoundError(f"Video file {video_file} does not exist.")
-    cap = cv2.VideoCapture(video_file)
-    fps = cap.get(cv2.CAP_PROP_FPS)
-    total_frames = int(cap.get(cv2.CAP_PROP_FRAME_COUNT))
-    video_length_seconds = total_frames / fps
-    sample_size = int(video_length_seconds * samples_per_second)
-    cap.release()
-    return (total_frames, sample_size, video_length_seconds)
-
-
-def sample_images_from_video(
-    video_file: str, output_dir: Path, samples_per_second: float = 1
-) -> List[str]:
-    """Sample images from a video file.
-    Parameters
-    ----------
-    video_file: The local path to the video file
-    output_dir: The local directory path that stores the sampled images
-    samples_per_second: The number of images to sample per second
-    Returns
-    -------
-    a list of local file paths to the sampled images
-    """
-    output_dir.mkdir(parents=True, exist_ok=True)
-    total_frames, sample_size, _ = probe_video(video_file, samples_per_second)
-    # Calculate the frame interval based on the desired frame rate
-    sample_interval = int(total_frames / sample_size)
-    frame_count = 0
-    output = []
-    cap = cv2.VideoCapture(video_file)
-    while cap.isOpened():
-        ret, frame = cap.read()
-        # Check if end of video file
-        if not ret:
-            break
-        # Check if the current frame should be saved
-        if frame_count % sample_interval == 0:
-            output_file_path = str(output_dir / f"{frame_count}.jpg")
-            cv2.imwrite(output_file_path, frame)
-            output.append(output_file_path)
-        frame_count += 1
-    cap.release()
-    return output
-
-
 class VideoFile(ImageSourceBase):
     """
     The `VideoFile` class is an image source that samples frames from a video file.
 
     Example:
     ```python
         import landingai.pipeline as pl
@@ -348,88 +290,7 @@
         return self
 
     def __next__(self) -> "FrameSet":
         return self.get_latest_frame()
 
     class Config:
         arbitrary_types_allowed = True
-
-
-def read_from_notebook_webcam(webcam_source: Union[str, int] = 0) -> Callable[[], str]:
-    # Define function to acquire images either directly from the local webcam (i.e. jupyter notebook)or from the web browser (i.e. colab)
-    local_cache_dir = Path(tempfile.mkdtemp())
-    filename = str(local_cache_dir / "photo.jpg")
-    # Detect if we are running on Google's colab
-    try:
-        from base64 import b64decode
-
-        from google.colab.output import eval_js  # type: ignore
-        from IPython.display import Javascript, display
-
-        def take_photo() -> str:
-            quality = 0.8
-            js = Javascript(
-                """
-            async function takePhoto(quality) {
-                const div = document.createElement('div');
-                const capture = document.createElement('button');
-                capture.textContent = 'Capture';
-                div.appendChild(capture);
-
-                const video = document.createElement('video');
-                video.style.display = 'block';
-                const stream = await navigator.mediaDevices.getUserMedia({video: true});
-
-                document.body.appendChild(div);
-                div.appendChild(video);
-                video.srcObject = stream;
-                await video.play();
-
-                // Resize the output to fit the video element.
-                google.colab.output.setIframeHeight(document.documentElement.scrollHeight, true);
-
-                // Wait for Capture to be clicked.
-                await new Promise((resolve) => capture.onclick = resolve);
-
-                const canvas = document.createElement('canvas');
-                canvas.width = video.videoWidth;
-                canvas.height = video.videoHeight;
-                canvas.getContext('2d').drawImage(video, 0, 0);
-                stream.getVideoTracks()[0].stop();
-                div.remove();
-                return canvas.toDataURL('image/jpeg', quality);
-            }
-            """
-            )
-            display(js)
-            data = eval_js("takePhoto({})".format(quality))
-            binary = b64decode(data.split(",")[1])
-            with open(filename, "wb") as f:
-                f.write(binary)
-                return filename
-
-    except ModuleNotFoundError:
-        # Capture image from local webcam using OpenCV
-        import cv2
-
-        def take_photo() -> str:
-            cam = cv2.VideoCapture(webcam_source)
-            cv2.namedWindow("Press space to take photo")
-            cv2.startWindowThread()
-            while True:
-                ret, frame = cam.read()
-                if not ret:
-                    print("failed to grab frame")
-                    exit()
-                cv2.imshow("Press space to take photo", frame)
-                k = cv2.waitKey(1)
-                if k % 256 == 32:
-                    # SPACE pressed
-                    cv2.imwrite(filename, frame)
-                    break
-            cam.release()
-            cv2.waitKey(1)
-            cv2.destroyAllWindows()
-            cv2.waitKey(1)
-            return filename
-
-    return take_photo
```

### Comparing `landingai-0.2.5/landingai/pipeline/postprocessing.py` & `landingai-0.2.6/landingai/pipeline/postprocessing.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.5/landingai/postprocess.py` & `landingai-0.2.6/landingai/postprocess.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.5/landingai/predict.py` & `landingai-0.2.6/landingai/predict.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.5/landingai/st_utils.py` & `landingai-0.2.6/landingai/st_utils.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.5/landingai/storage/data_access.py` & `landingai-0.2.6/landingai/storage/data_access.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.5/landingai/storage/snowflake.py` & `landingai-0.2.6/landingai/storage/snowflake.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.5/landingai/telemetry.py` & `landingai-0.2.6/landingai/telemetry.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.5/landingai/transform.py` & `landingai-0.2.6/landingai/transform.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.5/landingai/utils.py` & `landingai-0.2.6/landingai/utils.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.5/landingai/visualize.py` & `landingai-0.2.6/landingai/visualize.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.5/pyproject.toml` & `landingai-0.2.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "landingai"
-version = "0.2.5"
+version = "0.2.6"
 description = "Helper library for interacting with Landing AI LandingLens"
 authors = ["Landing AI <dev@landing.ai>"]
 readme = "README.md"
 packages = [{include = "landingai"}]
 
 [tool.poetry.urls]
 "Homepage" = "https://landing.ai"
```

### Comparing `landingai-0.2.5/PKG-INFO` & `landingai-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: landingai
-Version: 0.2.5
+Version: 0.2.6
 Summary: Helper library for interacting with Landing AI LandingLens
 Author: Landing AI
 Author-email: dev@landing.ai
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

