# Comparing `tmp/webuiapi-0.9.3-py3-none-any.whl.zip` & `tmp/webuiapi-0.9.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 12771 bytes, number of entries: 7
--rw-r--r--  2.0 unx      532 b- defN 23-Jun-05 08:45 webuiapi/__init__.py
--rw-r--r--  2.0 unx    34866 b- defN 23-Jun-05 08:45 webuiapi/webuiapi.py
--rw-r--r--  2.0 unx     1079 b- defN 23-Jun-05 08:45 webuiapi-0.9.3.dist-info/LICENSE
--rw-r--r--  2.0 unx    13529 b- defN 23-Jun-05 08:45 webuiapi-0.9.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-05 08:45 webuiapi-0.9.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Jun-05 08:45 webuiapi-0.9.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      545 b- defN 23-Jun-05 08:45 webuiapi-0.9.3.dist-info/RECORD
-7 files, 50652 bytes uncompressed, 11809 bytes compressed:  76.7%
+Zip file size: 13148 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      574 b- defN 23-Jul-15 03:54 webuiapi/__init__.py
+-rw-r--r--  2.0 unx    36360 b- defN 23-Jul-15 03:54 webuiapi/webuiapi.py
+-rw-r--r--  2.0 unx     1079 b- defN 23-Jul-15 03:55 webuiapi-0.9.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx    13790 b- defN 23-Jul-15 03:55 webuiapi-0.9.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-15 03:55 webuiapi-0.9.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Jul-15 03:55 webuiapi-0.9.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      545 b- defN 23-Jul-15 03:55 webuiapi-0.9.4.dist-info/RECORD
+7 files, 52449 bytes uncompressed, 12186 bytes compressed:  76.8%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: webuiapi/__init__.py
 Comment: 
 
 Filename: webuiapi/webuiapi.py
 Comment: 
 
-Filename: webuiapi-0.9.3.dist-info/LICENSE
+Filename: webuiapi-0.9.4.dist-info/LICENSE
 Comment: 
 
-Filename: webuiapi-0.9.3.dist-info/METADATA
+Filename: webuiapi-0.9.4.dist-info/METADATA
 Comment: 
 
-Filename: webuiapi-0.9.3.dist-info/WHEEL
+Filename: webuiapi-0.9.4.dist-info/WHEEL
 Comment: 
 
-Filename: webuiapi-0.9.3.dist-info/top_level.txt
+Filename: webuiapi-0.9.4.dist-info/top_level.txt
 Comment: 
 
-Filename: webuiapi-0.9.3.dist-info/RECORD
+Filename: webuiapi-0.9.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## webuiapi/__init__.py

```diff
@@ -6,24 +6,26 @@
     b64_img,
     raw_b64_img,
     ModelKeywordResult,
     ModelKeywordInterface,
     InstructPix2PixInterface,
     ControlNetInterface,
     ControlNetUnit,
+    RemBGInterface,
 )
 
-__version__ = "0.9.3"
+__version__ = "0.9.4"
 
 __all__ = [
     "__version__",
     "WebUIApi",
     "WebUIApiResult",
     "Upscaler",
     "HiResUpscaler",
     "b64_img",
     "ModelKeywordResult",
     "ModelKeywordInterface",
     "InstructPix2PixInterface",
     "ControlNetInterface",
     "ControlNetUnit",
+    "RemBGInterface",
 ]
```

## webuiapi/webuiapi.py

```diff
@@ -107,15 +107,16 @@
             "guidance_end": self.guidance_end,
             "control_mode": self.control_mode,
             "pixel_perfect": self.pixel_perfect,
         }
 
 
 def b64_img(image: Image) -> str:
-    return  "data:image/png;base64," + raw_b64_img(image)
+    return "data:image/png;base64," + raw_b64_img(image)
+
 
 def raw_b64_img(image: Image) -> str:
     # XXX controlnet only accepts RAW base64 without headers
     with io.BytesIO() as output_bytes:
         metadata = None
         for key, value in image.info.items():
             if isinstance(key, str) and isinstance(value, str):
@@ -197,15 +198,15 @@
         if "parameters" in r.keys():
             parameters = r["parameters"]
 
         return WebUIApiResult(images, parameters, info)
 
     async def _to_api_result_async(self, response):
         if response.status != 200:
-            raise RuntimeError(response.status, await response.text)
+            raise RuntimeError(response.status, await response.text())
 
         r = await response.json()
         images = []
         if "images" in r.keys():
             images = [Image.open(io.BytesIO(base64.b64decode(i))) for i in r["images"]]
         elif "image" in r.keys():
             images = [Image.open(io.BytesIO(base64.b64decode(r["image"])))]
@@ -621,18 +622,30 @@
         response = self.session.get(url=f"{self.baseurl}/cmd-flags")
         return response.json()
 
     def get_samplers(self):
         response = self.session.get(url=f"{self.baseurl}/samplers")
         return response.json()
 
+    def get_sd_vae(self):
+        response = self.session.get(url=f"{self.baseurl}/sd-vae")
+        return response.json()
+
     def get_upscalers(self):
         response = self.session.get(url=f"{self.baseurl}/upscalers")
         return response.json()
 
+    def get_latent_upscale_modes(self):
+        response = self.session.get(url=f"{self.baseurl}/latent-upscale-modes")
+        return response.json()
+
+    def get_loras(self):
+        response = self.session.get(url=f"{self.baseurl}/loras")
+        return response.json()
+
     def get_sd_models(self):
         response = self.session.get(url=f"{self.baseurl}/sd-models")
         return response.json()
 
     def get_hypernetworks(self):
         response = self.session.get(url=f"{self.baseurl}/hypernetworks")
         return response.json()
@@ -796,14 +809,17 @@
         keywords = result["keywords"]
         model = result["model"]
         oldhash = result["hash"]
         match_source = result["match_source"]
         return ModelKeywordResult(keywords, model, oldhash, match_source)
 
 
+
+
+
 # https://github.com/Klace/stable-diffusion-webui-instruct-pix2pix
 class InstructPix2PixInterface:
     def __init__(self, webuiapi):
         self.api = webuiapi
 
     def img2img(
         self,
@@ -834,14 +850,42 @@
             "image_cfg": image_cfg,
             "randomize_cfg": randomize_cfg,
             "output_image_width": output_image_width,
         }
         return self.api.custom_post("instruct-pix2pix/img2img", payload=payload)
 
 
+#https://github.com/AUTOMATIC1111/stable-diffusion-webui-rembg
+class RemBGInterface:
+    def __init__(self, webuiapi):
+        self.api = webuiapi
+
+    def rembg(
+        self,
+        input_image: str = "", #image string (?)
+        model: str = 'u2net',  #[None, 'u2net', 'u2netp', 'u2net_human_seg', 'u2net_cloth_seg','silueta','isnet-general-use','isnet-anime']
+        return_mask: bool = False,
+        alpha_matting: bool = False,
+        alpha_matting_foreground_threshold: int = 240,
+        alpha_matting_background_threshold: int = 10,
+        alpha_matting_erode_size: int = 10
+    ):
+
+        payload = {
+            "input_image": b64_img(input_image),
+            "model": model,
+            "return_mask": return_mask,
+            "alpha_matting":  alpha_matting,
+            "alpha_matting_foreground_threshold": alpha_matting_foreground_threshold,
+            "alpha_matting_background_threshold": alpha_matting_background_threshold,
+            "alpha_matting_erode_size": alpha_matting_erode_size
+        }
+        return self.api.custom_post("rembg", payload=payload)
+
+
 # https://github.com/Mikubill/sd-webui-controlnet
 class ControlNetInterface:
     def __init__(self, webuiapi, show_deprecation_warning=True):
         self.api = webuiapi
         self.show_deprecation_warning = show_deprecation_warning
 
     def print_deprecation_warning(self):
```

## Comparing `webuiapi-0.9.3.dist-info/LICENSE` & `webuiapi-0.9.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `webuiapi-0.9.3.dist-info/METADATA` & `webuiapi-0.9.4.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: webuiapi
-Version: 0.9.3
+Version: 0.9.4
 Summary: Python API client for AUTOMATIC1111/stable-diffusion-webui
 Home-page: https://github.com/mix1009/sdwebuiapi
 Author: ChunKoo Park
 Author-email: mix1009@gmail.com
 License: MIT
 Keywords: stable-diffuion-webui,AUTOMATIC1111,stable-diffusion,api
-Platform: UNKNOWN
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: Pillow
 
 # sdwebuiapi
 API client for AUTOMATIC1111/stable-diffusion-webui
 
 Supports txt2img, img2img, extra-single-image, extra-batch-images API calls.
@@ -436,7 +436,17 @@
 
 ```
 r = api.controlnet_detect(images=[img], module='canny')
 r.image
 ```
 
 
+### Extension support - RemBG (contributed by webcoderz)
+```
+# https://github.com/AUTOMATIC1111/stable-diffusion-webui-rembg
+rembg = webuiapi.RemBGInterface(api)
+rembg.rembg()
+
+r = rembg.rembg(input_image=img, model='u2net', return_mask=False)
+r.image
+```
+
```

