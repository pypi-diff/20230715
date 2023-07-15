# Comparing `tmp/shap-0.8.9.tar.gz` & `tmp/shap-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/shap-0.8.9.tar", last modified: Wed Feb  7 18:20:09 2018, max compression
+gzip compressed data, was "dist/shap-0.9.1.tar", last modified: Mon Feb 12 02:59:06 2018, max compression
```

## Comparing `shap-0.8.9.tar` & `shap-0.9.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 slund1     (501) staff       (20)        0 2018-02-07 18:20:09.000000 shap-0.8.9/
--rw-r--r--   0 slund1     (501) staff       (20)      304 2018-02-07 18:20:09.000000 shap-0.8.9/PKG-INFO
-drwxr-xr-x   0 slund1     (501) staff       (20)        0 2018-02-07 18:20:09.000000 shap-0.8.9/shap/
--rw-r--r--   0 slund1     (501) staff       (20)    14371 2018-01-25 00:06:52.000000 shap-0.8.9/shap/explainer.py
--rw-r--r--   0 slund1     (501) staff       (20)     2086 2018-02-02 03:49:52.000000 shap-0.8.9/shap/datasets.py
--rw-r--r--   0 slund1     (501) staff       (20)      498 2018-01-23 19:26:20.000000 shap-0.8.9/shap/__init__.py
--rw-r--r--   0 slund1     (501) staff       (20)    25260 2018-02-07 18:18:42.000000 shap-0.8.9/shap/plots.py
-drwxr-xr-x   0 slund1     (501) staff       (20)        0 2018-02-07 18:20:09.000000 shap-0.8.9/shap.egg-info/
--rw-r--r--   0 slund1     (501) staff       (20)      304 2018-02-07 18:20:08.000000 shap-0.8.9/shap.egg-info/PKG-INFO
--rw-r--r--   0 slund1     (501) staff       (20)        1 2017-10-04 18:55:54.000000 shap-0.8.9/shap.egg-info/not-zip-safe
--rw-r--r--   0 slund1     (501) staff       (20)      240 2018-02-07 18:20:09.000000 shap-0.8.9/shap.egg-info/SOURCES.txt
--rw-r--r--   0 slund1     (501) staff       (20)       54 2018-02-07 18:20:08.000000 shap-0.8.9/shap.egg-info/requires.txt
--rw-r--r--   0 slund1     (501) staff       (20)        5 2018-02-07 18:20:08.000000 shap-0.8.9/shap.egg-info/top_level.txt
--rw-r--r--   0 slund1     (501) staff       (20)        1 2018-02-07 18:20:08.000000 shap-0.8.9/shap.egg-info/dependency_links.txt
--rw-r--r--   0 slund1     (501) staff       (20)      628 2018-02-07 18:19:00.000000 shap-0.8.9/setup.py
--rw-r--r--   0 slund1     (501) staff       (20)       59 2018-02-07 18:20:09.000000 shap-0.8.9/setup.cfg
+drwxr-xr-x   0 slund1     (501) staff       (20)        0 2018-02-12 02:59:06.000000 shap-0.9.1/
+-rw-r--r--   0 slund1     (501) staff       (20)      304 2018-02-12 02:59:06.000000 shap-0.9.1/PKG-INFO
+drwxr-xr-x   0 slund1     (501) staff       (20)        0 2018-02-12 02:59:06.000000 shap-0.9.1/shap/
+-rw-r--r--   0 slund1     (501) staff       (20)    14371 2018-01-25 00:06:52.000000 shap-0.9.1/shap/explainer.py
+-rw-r--r--   0 slund1     (501) staff       (20)     2559 2018-02-09 01:11:32.000000 shap-0.9.1/shap/datasets.py
+-rw-r--r--   0 slund1     (501) staff       (20)      498 2018-01-23 19:26:20.000000 shap-0.9.1/shap/__init__.py
+-rw-r--r--   0 slund1     (501) staff       (20)    26375 2018-02-11 22:23:20.000000 shap-0.9.1/shap/plots.py
+drwxr-xr-x   0 slund1     (501) staff       (20)        0 2018-02-12 02:59:06.000000 shap-0.9.1/shap.egg-info/
+-rw-r--r--   0 slund1     (501) staff       (20)      304 2018-02-12 02:59:05.000000 shap-0.9.1/shap.egg-info/PKG-INFO
+-rw-r--r--   0 slund1     (501) staff       (20)        1 2017-10-04 18:55:54.000000 shap-0.9.1/shap.egg-info/not-zip-safe
+-rw-r--r--   0 slund1     (501) staff       (20)      240 2018-02-12 02:59:06.000000 shap-0.9.1/shap.egg-info/SOURCES.txt
+-rw-r--r--   0 slund1     (501) staff       (20)       54 2018-02-12 02:59:05.000000 shap-0.9.1/shap.egg-info/requires.txt
+-rw-r--r--   0 slund1     (501) staff       (20)        5 2018-02-12 02:59:05.000000 shap-0.9.1/shap.egg-info/top_level.txt
+-rw-r--r--   0 slund1     (501) staff       (20)        1 2018-02-12 02:59:05.000000 shap-0.9.1/shap.egg-info/dependency_links.txt
+-rw-r--r--   0 slund1     (501) staff       (20)      628 2018-02-12 02:58:50.000000 shap-0.9.1/setup.py
+-rw-r--r--   0 slund1     (501) staff       (20)       59 2018-02-12 02:59:06.000000 shap-0.9.1/setup.cfg
```

### Comparing `shap-0.8.9/shap/explainer.py` & `shap-0.9.1/shap/explainer.py`

 * *Files identical despite different names*

### Comparing `shap-0.8.9/shap/plots.py` & `shap-0.9.1/shap/plots.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,35 +7,36 @@
 import iml
 import numpy as np
 
 try:
     import matplotlib.pyplot as pl
     import matplotlib
     from matplotlib.colors import LinearSegmentedColormap
+    from matplotlib.ticker import MaxNLocator
 
     cdict1 = {
           'red': ((0.0, 0.11764705882352941, 0.11764705882352941),
                   (1.0, 0.9607843137254902, 0.9607843137254902)),
 
         'green': ((0.0, 0.5333333333333333, 0.5333333333333333),
                    (1.0, 0.15294117647058825, 0.15294117647058825)),
 
          'blue':  ((0.0, 0.8980392156862745, 0.8980392156862745),
                    (1.0, 0.3411764705882353, 0.3411764705882353)),
 
         'alpha':  ((0.0, 1, 1),
                    (0.5, 0.3, 0.3),
                    (1.0, 1, 1))
-    }
+    } # #1E88E5 -> #ff0052
     red_blue = LinearSegmentedColormap('RedBlue', cdict1)
 except ImportError:
     pass
 
 def dependence_plot(ind, shap_values, features, feature_names=None, display_features=None,
-                    interaction_index="auto", color="#ff0052", axis_color="#333333",
+                    interaction_index="auto", color="#1E88E5", axis_color="#333333",
                     dot_size=16, alpha=1, title=None, show=True):
     """
     Create a SHAP dependence plot, colored by an interaction feature.
 
     Parameters
     ----------
     ind : int
@@ -49,15 +50,15 @@
 
     feature_names : list
         Names of the features (length # features)
 
     display_features : numpy.array or pandas.DataFrame
         Matrix of feature values for visual display (such as strings instead of coded values)
 
-    interaction_index : "auto" or int
+    interaction_index : "auto", None, or int
         The index of the feature used to color the plot.
     """
 
     # convert from DataFrames if we got any
     if str(type(features)) == "<class 'pandas.core.frame.DataFrame'>":
         if feature_names is None:
             feature_names = features.columns
@@ -91,19 +92,27 @@
 
     ind = convert_name(ind)
 
     # plotting SHAP interaction values
     if len(shap_values.shape) == 3 and len(ind) == 2:
         ind1 = convert_name(ind[0])
         ind2 = convert_name(ind[1])
+        if ind1 == ind2:
+            proj_shap_values = shap_values[:,ind2,:]
+        else:
+            proj_shap_values = shap_values[:,ind2,:] * 2 # off-diag values are split in half
         dependence_plot(
-            ind1, shap_values[:,ind2,:], features, feature_names=feature_names,
+            ind1, proj_shap_values, features, feature_names=feature_names,
             interaction_index=ind2, display_features=display_features, show=False
         )
-        pl.ylabel("SHAP interaction value for\n"+feature_names[ind1]+" and "+feature_names[ind2])
+        if ind1 == ind2:
+            pl.ylabel("SHAP main effect value for\n"+feature_names[ind1])
+        else:
+            pl.ylabel("SHAP interaction value for\n"+feature_names[ind1]+" and "+feature_names[ind2])
+
         if show:
             pl.show()
         return
 
     # get both the raw and display feature values
     xv = features[:,ind]
     xd = display_features[:,ind]
@@ -118,64 +127,68 @@
     if type(feature_names) == str:
         feature_names = [feature_names]
     name = feature_names[ind]
 
     # guess what other feature as the stongest interaction with the plotted feature
     if interaction_index == "auto":
         interaction_index = approx_interactions(ind, shap_values, features)[0]
+    interaction_index = convert_name(interaction_index)
 
     # get both the raw and display color values
     cv = features[:,interaction_index]
     cd = display_features[:,interaction_index]
     categorical_interaction = False
     clow = np.nanpercentile(features[:,interaction_index], 5)
     chigh = np.nanpercentile(features[:,interaction_index], 95)
     if type(cd[0]) == str:
         cname_map = {}
         for i in range(len(cv)):
             cname_map[cd[i]] = cv[i]
         cnames = list(cname_map.keys())
         categorical_interaction = True
-    elif clow % 1 == 0 and chigh % 1 == 0:
+    elif clow % 1 == 0 and chigh % 1 == 0 and len(set(features[:,interaction_index])) < 50:
         categorical_interaction = True
 
     # discritize colors for categorical features
     color_norm = None
     if categorical_interaction and clow != chigh:
         bounds = np.linspace(clow, chigh, chigh-clow+2)
         color_norm = matplotlib.colors.BoundaryNorm(bounds, red_blue.N)
 
-    # the actual scatter plot, TODO: adapt the dot_size to the number of data points
+    # the actual scatter plot, TODO: adapt the dot_size to the number of data points?
     pl.scatter(xv, s, s=dot_size, linewidth=0, c=features[:,interaction_index], cmap=red_blue,
-               alpha=alpha, vmin=clow, vmax=chigh, norm=color_norm)
+               alpha=alpha, vmin=clow, vmax=chigh, norm=color_norm, rasterized=len(xv) > 500)
 
-    # draw the color bar
-    norm = None
-    if type(cd[0]) == str:
-        tick_positions = [cname_map[n] for n in cnames]
-        if len(tick_positions) == 2:
-            tick_positions[0] -= 0.25
-            tick_positions[1] += 0.25
-        cb = pl.colorbar(ticks=tick_positions)
-        cb.set_ticklabels(cnames)
+    if interaction_index != ind:
+        # draw the color bar
+        norm = None
+        if type(cd[0]) == str:
+            tick_positions = [cname_map[n] for n in cnames]
+            if len(tick_positions) == 2:
+                tick_positions[0] -= 0.25
+                tick_positions[1] += 0.25
+            cb = pl.colorbar(ticks=tick_positions)
+            cb.set_ticklabels(cnames)
 
-    else:
-        cb = pl.colorbar()
-    cb.set_label(feature_names[interaction_index], size=13)
-    cb.ax.tick_params(labelsize=11)
-    if categorical_interaction:
-        cb.ax.tick_params(length=0)
-    cb.set_alpha(1)
-    cb.outline.set_visible(False)
-    bbox = cb.ax.get_window_extent().transformed(pl.gcf().dpi_scale_trans.inverted())
-    cb.ax.set_aspect((bbox.height-0.7)*20)
-    #cb.draw_all()
+        else:
+            cb = pl.colorbar()
+        cb.set_label(feature_names[interaction_index], size=13)
+        cb.ax.tick_params(labelsize=11)
+        if categorical_interaction:
+            cb.ax.tick_params(length=0)
+        cb.set_alpha(1)
+        cb.outline.set_visible(False)
+        bbox = cb.ax.get_window_extent().transformed(pl.gcf().dpi_scale_trans.inverted())
+        cb.ax.set_aspect((bbox.height-0.7)*20)
 
     # make the plot more readable
-    pl.gcf().set_size_inches(7.5, 5)
+    if interaction_index != ind:
+        pl.gcf().set_size_inches(7.5, 5)
+    else:
+        pl.gcf().set_size_inches(6, 5)
     pl.xlabel(name, color=axis_color, fontsize=13)
     pl.ylabel("SHAP value for\n"+name, color=axis_color, fontsize=13)
     if title != None:
         pl.title(title, color=axis_color, fontsize=13)
     pl.gca().xaxis.set_ticks_position('bottom')
     pl.gca().yaxis.set_ticks_position('left')
     pl.gca().spines['right'].set_visible(False)
@@ -277,30 +290,35 @@
         shigh = np.nanpercentile(shap_values, 100 - delta)
         v = max(abs(slow), abs(shigh))
         slow = -v
         shigh = v
 
         pl.figure(figsize=(1.5*max_display+1,1*max_display+1))
         pl.subplot(1,max_display,1)
+        proj_shap_values = shap_values[:,sort_inds[0],np.hstack((sort_inds, len(sort_inds)))]
+        proj_shap_values[:,1:] *= 2 # because off diag effects are split in half
         summary_plot(
-            shap_values[:,sort_inds[0],np.hstack((sort_inds, len(sort_inds)))], features[:,sort_inds],
+            proj_shap_values, features[:,sort_inds],
             feature_names=feature_names[sort_inds],
             sort=False, show=False, color_bar=False,
             auto_size_plot=False,
             max_display=max_display
         )
         pl.xlim((slow,shigh))
         pl.xlabel("")
         title_length_limit = 11
         pl.title(shorten_text(feature_names[sort_inds[0]], title_length_limit))
         for i in range(1,max_display):
             ind = sort_inds[i]
             pl.subplot(1,max_display,i+1)
+            proj_shap_values = shap_values[:,ind,np.hstack((sort_inds, len(sort_inds)))]
+            proj_shap_values *= 2
+            proj_shap_values[:,i] /= 2 # because only off diag effects are split in half
             summary_plot(
-                shap_values[:,ind,np.hstack((sort_inds, len(sort_inds)))], features[:,sort_inds],
+                proj_shap_values, features[:,sort_inds],
                 sort=False,
                 feature_names=["" for i in range(features.shape[1])],
                 show=False,
                 color_bar=False,
                 auto_size_plot=False,
                 max_display=max_display
             )
@@ -360,17 +378,20 @@
                     vmin = np.nanpercentile(features[:,i], 1)
                     vmax = np.nanpercentile(features[:,i], 99)
                     if vmin == vmax:
                         vmin = np.min(features[:,i])
                         vmax = np.max(features[:,i])
 
                 assert features.shape[0] == len(shaps), "Feature and SHAP matrices must have the same number of rows!"
-                pl.scatter(shaps, pos+ys, cmap=red_blue, vmin=vmin, vmax=vmax, s=16, c=np.nan_to_num(features[:,i]), alpha=alpha, linewidth=0, zorder=3)
+                pl.scatter(shaps, pos+ys, cmap=red_blue, vmin=vmin, vmax=vmax, s=16,
+                           c=np.nan_to_num(features[:,i]), alpha=alpha, linewidth=0,
+                           zorder=3, rasterized=len(shaps) > 500)
             else:
-                pl.scatter(shaps, pos+ys, s=16, alpha=alpha, linewidth=0, zorder=3, color=color)
+                pl.scatter(shaps, pos+ys, s=16, alpha=alpha, linewidth=0, zorder=3,
+                           color=color, rasterized=len(shaps) > 500)
 
     elif plot_type == "violin":
         for pos,i in enumerate(feature_order):
             pl.axhline(y=pos, color="#cccccc", lw=0.5, dashes=(1,5), zorder=-1)
 
         if features is not None:
             global_low = np.nanpercentile(shap_values[:,:len(feature_names)].flatten(), 1)
```

### Comparing `shap-0.8.9/setup.py` & `shap-0.9.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 # to publish use:
 # > python setup.py sdist upload
 # which depends on ~/.pypirc
 
 setup(name='shap',
-      version='0.8.9',
+      version='0.9.1',
       description='Explains the output of any machine learning model using expectations and Shapley values.',
       url='http://github.com/slundberg/shap',
       author='Scott Lundberg',
       author_email='slund1@cs.washington.edu',
       license='MIT',
       packages=['shap'],
       install_requires=['numpy', 'scipy', 'iml>=0.3.4', 'scikit-learn', 'matplotlib', 'pandas'],
```

