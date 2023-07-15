# Comparing `tmp/awblib-0.0.1.tar.gz` & `tmp/awblib-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awblib-0.0.1.tar", max compression
+gzip compressed data, was "awblib-0.0.2.tar", max compression
```

## Comparing `awblib-0.0.1.tar` & `awblib-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,11 @@
--rw-r--r--   0        0        0    11357 2023-07-12 17:18:49.483073 awblib-0.0.1/LICENSE
--rw-r--r--   0        0        0       10 2023-07-14 08:28:48.297372 awblib-0.0.1/README.md
--rw-r--r--   0        0        0      970 2023-07-13 07:19:38.326877 awblib-0.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-13 07:22:48.495072 awblib-0.0.1/src/awblib/__init__.py
--rw-r--r--   0        0        0    11853 2023-07-14 08:16:50.183169 awblib-0.0.1/src/awblib/dhm.py
--rw-r--r--   0        0        0     1592 2023-07-13 15:17:17.034350 awblib-0.0.1/src/awblib/utils.py
--rw-r--r--   0        0        0     1131 1970-01-01 00:00:00.000000 awblib-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11341 2023-07-14 18:38:08.732962 awblib-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1638 2023-07-14 18:38:08.732962 awblib-0.0.2/README.md
+-rw-r--r--   0        0        0     1509 2023-07-14 18:38:08.848963 awblib-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-14 18:38:08.848963 awblib-0.0.2/src/awblib/__init__.py
+-rw-r--r--   0        0        0     3348 2023-07-14 18:38:08.848963 awblib-0.0.2/src/awblib/aaet.py
+-rw-r--r--   0        0        0     6413 2023-07-14 18:38:08.848963 awblib-0.0.2/src/awblib/chs.py
+-rw-r--r--   0        0        0     6118 2023-07-14 18:38:08.848963 awblib-0.0.2/src/awblib/dhm.py
+-rw-r--r--   0        0        0     2618 2023-07-14 18:38:08.848963 awblib-0.0.2/src/awblib/gw.py
+-rw-r--r--   0        0        0     3131 2023-07-14 18:38:08.848963 awblib-0.0.2/src/awblib/hm.py
+-rw-r--r--   0        0        0     1921 2023-07-14 18:38:08.848963 awblib-0.0.2/src/awblib/utils.py
+-rw-r--r--   0        0        0     3340 1970-01-01 00:00:00.000000 awblib-0.0.2/PKG-INFO
```

### Comparing `awblib-0.0.1/LICENSE` & `awblib-0.0.2/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright [yyyy] [name of copyright owner]
+   Copyright 2023 Hongyu Teng
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `awblib-0.0.1/src/awblib/dhm.py` & `awblib-0.0.2/src/awblib/dhm.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,24 +7,31 @@
 
 from __future__ import annotations  # for compatibility with Python 3.8
 
 from functools import partial
 
 import jax
 import jax.numpy as jnp
-from jaxtyping import Array, Float, Integer, Num
+from jaxtyping import Array, Float, Integer
 from typing_extensions import TypeAlias
 
 RGBImage: TypeAlias = Integer[Array, "height width 3"]
 Index: TypeAlias = Integer[Array, ""]
 Coef: TypeAlias = Float[Array, ""]
 
 
-@partial(jax.jit, static_argnames=("bit_depth", ))
-def balance(image: RGBImage, bit_depth: int = 8) -> RGBImage:
+@partial(
+    jax.jit,
+    static_argnames=("bit_depth", "always_mid_fix"),
+)
+def balance(
+    image: RGBImage,
+    bit_depth: int = 8,
+    always_mid_fix: bool = False,
+) -> RGBImage:
     """Apply automatic white balance of an image, using AWB-DHM."""
 
     assert bit_depth > 0, f"bit_depth must be positive, got {bit_depth}"
     max_value: int = 2**bit_depth
 
     total_pixels: int = image.shape[0] * image.shape[1]
 
@@ -101,21 +108,25 @@
         idx: Index = jnp.where(
             # Average gray level > 63 for 8-bit images. 64 = 256 // 4
             # (gray * channels) * total_pixels >= ch * tot * (max // 4) => 64
             gray_levels.sum() >= (channels * total_pixels * max_value // 4),
             channel_idx,
             ch_.argmin(),
         )
-        """ NOTE: from the results section (fig 6) in the paper, the selected
-            channel is actually usually the one with mid level of intensity.
-            See docs/dhm/*.png for the comparison of the histogram and cdf from
-            the original paper.
-        """
-        return ch_.argmin(), jnp.ones(())
-        return idx, jnp.ones(())
+
+        if always_mid_fix:
+            """ NOTE: from the results section (fig 6) in the paper, the
+                selected channel is actually usually the one with mid level of
+                intensity.
+                See docs/dhm/*.png for the comparison of the histogram and cdf
+                from the original paper.
+            """
+            return ch_.argmin(), jnp.ones(())
+        else:
+            return idx, jnp.ones(())
 
     """ NOTE: The paper never says specifically what "majority" means. It is
         assumed that it means "more than half".
     """
     idx, k = jax.lax.cond(
         lower_half_count < total_pixels // 2,
         find_best_fit_channel_if_majority_above_half,
@@ -145,164 +156,11 @@
                 source_cdf,
                 target_cdf,
                 target_values,
             )[source_idx],
             in_axes=0,
             out_axes=2,
         )(cdf, bin_idx)).astype(int)
+    result = jnp.clip(result, 0, max_value - 1)
     assert isinstance(result, RGBImage)
 
     return result
-
-
-@partial(jax.jit, static_argnames=("bit_depth", ))
-def buggy_balance(image: RGBImage, bit_depth: int = 8) -> RGBImage:
-    """Apply automatic white balance of an image, using AWB-DHM."""
-
-    assert bit_depth > 0, f"bit_depth must be positive, got {bit_depth}"
-    max_value: int = 2**bit_depth
-
-    total_pixels: int = image.shape[0] * image.shape[1]
-
-    channels: int = image.shape[2]
-
-    # STAGE: Histogram Generation
-
-    # number of bins == max_value
-    histogram: Float[Array, "3 bins"] = (
-        jax.vmap(
-            # compute histogram for one channel
-            lambda img: jnp.histogram(
-                img,
-                # - 0.5 to make sure that the bins are centered around the values
-                bins=jnp.arange(max_value + 1) - 0.5,
-            )[0],
-            in_axes=(2, ),
-        )(image)).astype(int)
-    assert isinstance(histogram, Integer[Array, "3 bins"])
-
-    # STAGE: Histogram Analysis
-
-    # multiple of gray_levels, divide this by channels to get the true value
-    gray_levels: Integer[Array, "height width"] = image.sum(axis=2)
-    assert isinstance(gray_levels, Integer[Array, "height width"])
-
-    lower_half_count: Integer[Array, ""]
-    # equivalent to: image.mean(axis=2) < (max_value // 2)
-    lower_half_count = (gray_levels < (max_value // 2 * channels)).sum()
-    assert isinstance(lower_half_count, Integer[Array, ""])
-
-    channel_intensity: Integer[Array, "3"] = image.sum(axis=(0, 1))
-
-    def find_best_fit_channel_if_majority_above_half() -> tuple[Index, Coef]:
-        """CRITERIA I."""
-        # Step 1:
-        channel_idx: Index = channel_intensity.argmax()
-        assert isinstance(channel_idx, Index)
-
-        # Step 2:
-        """ NOTE: the paper is not clear about whether `Imax` is the maximum,
-        the average, or something else. An educated guess is that it is the
-        average, which is used here.
-        """
-        # Imax * total_pixels
-        i_max: Integer[Array, ""] = channel_intensity[channel_idx]
-        # Iavg * total_pixels
-        i_avg: Integer[Array, ""] = channel_intensity.sum()
-
-        # Iavg / Imax = (Iavg * total_pixels) / (Imax * total_pixels)
-        k: Coef = i_avg / i_max
-
-        return channel_idx, k
-
-    def find_best_fit_channel_if_majority_below_half() -> tuple[Index, Coef]:
-        """CRITERIA II."""
-        # Step 1:
-        # NOTE: the paper has a false claim that the dynamic range is 0-127
-        channel_idx: Index = channel_intensity.argmin()
-        assert isinstance(channel_idx, Index)
-
-        # Step 2:
-
-        ch_: Integer[Array, "3"]
-        # replace the omitted channel value with a big enough value.
-        ch_ = channel_intensity.at[channel_idx].set(total_pixels * max_value)
-        idx: Index = jnp.where(
-            # Average gray level > 63 for 8-bit images. 64 = 256 // 4
-            # (gray * channels) * total_pixels >= ch * tot * (max // 4) => 64
-            gray_levels.sum() >= (channels * total_pixels * max_value // 4),
-            channel_idx,
-            ch_.argmin(),
-        )
-
-        return ch_.argmin(), jnp.ones(())  # DEBUG
-        return idx, jnp.ones(())
-
-    """ NOTE: The paper never says specifically what "majority" means. It is
-        assumed that it means "more than half".
-    """
-    idx, k = jax.lax.cond(
-        lower_half_count < total_pixels // 2,
-        find_best_fit_channel_if_majority_above_half,
-        find_best_fit_channel_if_majority_below_half,
-    )
-    idx = 0  # DEBUG
-    jax.debug.print(
-        "majority above half: {cond}\nidx: {idx} k: {k}\naverage gray: {avg_gray}",
-        cond=lower_half_count < total_pixels // 2,
-        idx=idx,
-        k=k,
-        avg_gray=gray_levels.sum() / total_pixels / channels,
-    )
-    """ NOTE: the paper is not clear about this operation. I guess they want to
-        reduce the value of the best-fit channel using the scaling factor `K`.
-        This operation is only meaningful for CRITERIA I; in CRITERIA II, `K`
-        is always 1.
-    """
-    target_histogram: Integer[Array, "bins"] = jnp.histogram(
-        (image[:, :, idx] * k).round().astype(int),
-        # - 0.5 to make sure that the bins are centered around the values
-        bins=jnp.arange(max_value + 1) - 0.5,
-    )[0].astype(int)
-    assert isinstance(target_histogram, Integer[Array, "bins"])
-
-    # STAGE: Histogram Matching
-
-    # cdf * total_pixels
-    target_cdf: Integer[Array, "bins"] = jnp.cumsum(target_histogram)
-    assert isinstance(target_cdf, Integer[Array, "bins"])
-    # cdf * total_pixels
-    image_cdf: Integer[Array, "3 bins"] = jnp.cumsum(histogram, axis=1)
-    assert isinstance(image_cdf, Integer[Array, "3 bins"])
-
-    def match_one_pixel(pixel: Integer[Array, "3"]) -> Integer[Array, "3"]:
-        """Match one pixel to the target CDF."""
-        pixel_cdf: Integer[Array, "3"]
-        pixel_cdf = jax.vmap(lambda i, cdf: cdf[i])(pixel, image_cdf)
-        assert isinstance(pixel_cdf, Integer[Array, "3"])
-
-        result: Integer[Array, "3"]
-        result = jax.vmap(lambda p: target_cdf.searchsorted(p))(pixel_cdf)
-        assert isinstance(result, Integer[Array, "3"])
-
-        return result
-
-    result: RGBImage = jax.vmap(jax.vmap(match_one_pixel))(image)
-    assert isinstance(result, RGBImage)
-
-    _histogram: Float[Array, "3 bins"] = (
-        jax.vmap(
-            # compute histogram for one channel
-            lambda img: jnp.histogram(
-                img,
-                # - 0.5 to make sure that the bins are centered around the values
-                bins=jnp.arange(max_value + 1) - 0.5,
-            )[0],
-            in_axes=(2, ),
-        )(result)).astype(int)
-    _image_cdf: Integer[Array, "3 bins"] = jnp.cumsum(_histogram, axis=1)
-    _mapping: Integer[Array, "3 bins"] = jax.vmap(match_one_pixel)(jnp.vstack(
-        [jnp.arange(max_value) for _ in range(3)]).T)
-
-    return target_histogram, target_cdf, image_cdf, _mapping, _histogram, _image_cdf, result
-
-    return result
```

### Comparing `awblib-0.0.1/src/awblib/utils.py` & `awblib-0.0.2/src/awblib/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,34 +16,44 @@
 
 def visualise_histogram(
     image: np.ndarray,
     bit_depth: int = 8,
     ax: Optional[plt.Axes] = None,
     color: list[str] = ["#FF0000", "#00FF00", "#0000FF"],
     cdf: bool = False,
-):
-    """Visualise a histogram."""
+    normalise: bool = True,
+) -> float:
+    """Visualise a histogram; return Overlap Area (OA)."""
     assert image.ndim == 3, f"image must has 3 channels, got {image.ndim}"
 
     channels: int = image.shape[2]
     assert channels == 3, f"image must be RGB, got {channels} channels"
 
+    total_pixels: int = image.shape[0] * image.shape[1]
+
     assert bit_depth > 0, f"bit_depth must be positive, got {bit_depth}"
     max_value: int = 2**bit_depth
 
     histogram: np.ndarray = np.vstack([
         np.histogram(
             image[:, :, ch],
             # - 0.5 to make sure that the bins are centered around the values
             bins=np.arange(max_value + 1) - 0.5,
         )[0] for ch in range(channels)
-    ])
+    ])  # shape (channels, max_value)
+
+    overlap_area: float = (histogram.min(axis=0) / total_pixels).sum()
+
     if cdf:
         histogram = histogram.cumsum(axis=1)
 
+    # normalise
+    if normalise:
+        histogram = histogram / total_pixels
+
     assert isinstance(histogram, np.ndarray)
 
     if ax is None:
         fig, _ax = plt.subplots()
     else:
         _ax = ax
 
@@ -55,7 +65,9 @@
             histogram[ch],
             color=color[ch],
             label=f"channel {ch}",
         )
 
     if ax is None:
         fig.show()
+
+    return overlap_area
```

