# Comparing `tmp/cruiz-1.4.0a3.tar.gz` & `tmp/cruiz-1.4.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cruiz-1.4.0a3.tar", last modified: Fri Jul 14 13:46:18 2023, max compression
+gzip compressed data, was "cruiz-1.4.0a4.tar", last modified: Sat Jul 15 20:00:44 2023, max compression
```

## Comparing `cruiz-1.4.0a3.tar` & `cruiz-1.4.0a4.tar`

### file list

```diff
@@ -1,209 +1,269 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:46:18.489237 cruiz-1.4.0a3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-07-14 13:46:18.489237 cruiz-1.4.0a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:46:18.449237 cruiz-1.4.0a3/cruiz/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-14 13:46:18.000000 cruiz-1.4.0a3/cruiz/RELEASE_VERSION.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1828 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/application.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:46:18.453237 cruiz-1.4.0a3/cruiz/commands/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/commands/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      500 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/commands/conanconf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1939 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/commands/conanenv.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6322 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/commands/conaninvocation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25561 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/commands/context.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1731 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/commands/guardedlisttoflush.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2401 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/commands/logdetails.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4189 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/commands/messagereplyprocessor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5555 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/commands/metarequestconaninvocation.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/dumpobjecttypes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3770 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/environ.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/globals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:46:18.453237 cruiz-1.4.0a3/cruiz/interop/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/interop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17403 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/interop/commandparameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/interop/commonparameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/interop/dependencygraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/interop/message.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/interop/packagebinaryparameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/interop/packageidparameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/interop/packagenode.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/interop/packagerevisionsparameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/interop/pod.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/interop/reciperevisionsparameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/interop/searchrecipesparameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:46:18.453237 cruiz-1.4.0a3/cruiz/load_recipe/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/load_recipe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/load_recipe/loadrecipewizard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:46:18.457237 cruiz-1.4.0a3/cruiz/load_recipe/pages/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/load_recipe/pages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/load_recipe/pages/initialprofilepage.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/load_recipe/pages/intropage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/load_recipe/pages/localcachepage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/load_recipe/pages/packageversionpage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    28296 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/mainwindow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:46:18.457237 cruiz-1.4.0a3/cruiz/manage_local_cache/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/manage_local_cache/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    36004 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/manage_local_cache/managelocalcachesdialog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:46:18.461237 cruiz-1.4.0a3/cruiz/manage_local_cache/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/manage_local_cache/widgets/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2465 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/manage_local_cache/widgets/addenvironmentdialog.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2425 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/manage_local_cache/widgets/addextraprofiledirectorydialog.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2525 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/manage_local_cache/widgets/addremotedialog.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      950 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/manage_local_cache/widgets/configpathorurl.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3684 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/manage_local_cache/widgets/installconfigdialog.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1902 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/manage_local_cache/widgets/keyvaluetable.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8370 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/manage_local_cache/widgets/movelocalcachedialog.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7548 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/manage_local_cache/widgets/newlocalcachewizard.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1877 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/manage_local_cache/widgets/newlocalcachewizardpages.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1683 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/manage_local_cache/widgets/progressdialogs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4933 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/manage_local_cache/widgets/remotestable.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1139 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/manage_local_cache/widgets/removeenvironmentdialog.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2239 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/manage_local_cache/widgets/runconancommanddialog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:46:18.461237 cruiz-1.4.0a3/cruiz/model/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/model/conanpackagetypeflags.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2494 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/model/graphaslistmodel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:46:18.461237 cruiz-1.4.0a3/cruiz/pyside6/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/pyside6/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:46:18.465237 cruiz-1.4.0a3/cruiz/recipe/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/recipe/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1632 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/recipe/dependencyview.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1206 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/recipe/expressioneditordialog.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1586 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/recipe/findtextdialog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:46:18.465237 cruiz-1.4.0a3/cruiz/recipe/logs/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/recipe/logs/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6022 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/recipe/logs/command.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2234 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/recipe/recipe.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    61387 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/recipe/recipewidget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:46:18.465237 cruiz-1.4.0a3/cruiz/recipe/toolbars/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/recipe/toolbars/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6621 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/recipe/toolbars/behaviour.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9887 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/recipe/toolbars/buildfeatures.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    33104 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/recipe/toolbars/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:46:18.465237 cruiz-1.4.0a3/cruiz/remote_browser/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/remote_browser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:46:18.469237 cruiz-1.4.0a3/cruiz/remote_browser/pages/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/remote_browser/pages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14857 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/remote_browser/pages/packagebinarypage.py
--rw-r--r--   0 runner    (1001) docker     (123)    17586 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/remote_browser/pages/packageidpage.py
--rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/remote_browser/pages/packagereferencepage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/remote_browser/pages/packagerevisionpage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/remote_browser/pages/page.py
--rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/remote_browser/pages/reciperevisionpage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/remote_browser/remotebrowser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2357 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resourcegeneration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:46:18.477237 cruiz-1.4.0a3/cruiz/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/001-rubbish.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/002-null.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/003-chemistry.svg
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/004-share.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/005-box.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/006-toolbox.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/007-book.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/008-cloud-computing.svg
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/009-import.svg
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/010-draw.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/012-hammer.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/013-pencil.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/014-code.svg
--rw-r--r--   0 runner    (1001) docker     (123)    17753 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/Cmake.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/about_dialog.ui
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/cruise.png
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/cruizres.qrc
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/find_text_dialog.ui
--rw-r--r--   0 runner    (1001) docker     (123)    53573 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/license-cruise.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    96863 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/license.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/load_recipe_wizard.ui
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/local_cache_add_environment.ui
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/local_cache_add_profile_directory.ui
--rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/local_cache_add_remote.ui
--rw-r--r--   0 runner    (1001) docker     (123)     7174 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/local_cache_install_config.ui
--rw-r--r--   0 runner    (1001) docker     (123)    27112 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/local_cache_manage.ui
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/local_cache_move.ui
--rw-r--r--   0 runner    (1001) docker     (123)     9596 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/local_cache_new_wizard.ui
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/local_cache_remove_environment.ui
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/local_cache_run_command_dialog.ui
--rw-r--r--   0 runner    (1001) docker     (123)    41069 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/preferences.ui
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/recipe_cmake_features_frame.ui
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/recipe_compiler_cache_configuration_dialog.ui
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/recipe_compilercache_features_frame.ui
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/recipe_cpucores_frame.ui
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/recipe_local_workflow_expression_editor.ui
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/recipe_profile_frame.ui
--rw-r--r--   0 runner    (1001) docker     (123)    34335 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/recipe_window.ui
--rw-r--r--   0 runner    (1001) docker     (123)    28688 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/remote_browser.ui
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/remote_browser_fileview.ui
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/restart.py
--rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/revealonfilesystem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:46:18.481238 cruiz-1.4.0a3/cruiz/settings/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/settings/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      582 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/settings/ensuredefaultlocalcache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:46:18.485237 cruiz-1.4.0a3/cruiz/settings/managers/
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/settings/managers/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10185 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/settings/managers/basesettings.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4871 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/settings/managers/cleansettings.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1728 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/settings/managers/cmakepreferences.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3244 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/settings/managers/compilercachepreferences.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2499 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/settings/managers/conanpreferences.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2309 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/settings/managers/fontpreferences.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6803 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/settings/managers/generalpreferences.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1890 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/settings/managers/graphvizpreferences.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3903 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/settings/managers/localcachepreferences.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14295 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/settings/managers/namedlocalcache.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1830 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/settings/managers/ninjapreferences.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3681 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/settings/managers/recentconanconfigs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3590 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/settings/managers/recentconanremotes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3564 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/settings/managers/recentrecipes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18314 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/settings/managers/recipe.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      317 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/settings/managers/restoredefaults.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7928 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/settings/managers/shortcuts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1149 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/settings/managers/valueclasses.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4187 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/settings/managers/writermixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:46:18.485237 cruiz-1.4.0a3/cruiz/settings/models/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/settings/models/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1419 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/settings/models/recentconanconfigmodel.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1345 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/settings/models/recentconanremotesmodel.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2727 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/settings/models/recipesmodel.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    54673 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/settings/preferencesdialog.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14331 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/settings/updatesettings.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5848 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/svggraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:46:18.489237 cruiz-1.4.0a3/cruiz/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/widgets/aboutcruizdialog.py
--rw-r--r--   0 runner    (1001) docker     (123)    11414 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/widgets/debugging.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1387 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/widgets/shortcutlineedit.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2050 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/widgets/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:46:18.489237 cruiz-1.4.0a3/cruiz/workers/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/workers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:46:18.489237 cruiz-1.4.0a3/cruiz/workers/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/workers/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:46:18.489237 cruiz-1.4.0a3/cruiz/workers/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/workers/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/workers/utils/colorarma_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/workers/utils/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/workers/utils/formatoptions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1493 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/workers/utils/qtlogger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/workers/utils/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/workers/utils/text2html.py
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/workers/utils/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:46:18.449237 cruiz-1.4.0a3/cruiz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-07-14 13:46:18.000000 cruiz-1.4.0a3/cruiz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-07-14 13:46:18.000000 cruiz-1.4.0a3/cruiz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 13:46:18.000000 cruiz-1.4.0a3/cruiz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-14 13:46:18.000000 cruiz-1.4.0a3/cruiz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-14 13:46:18.000000 cruiz-1.4.0a3/cruiz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-14 13:46:18.000000 cruiz-1.4.0a3/cruiz.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 13:46:18.489237 cruiz-1.4.0a3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 20:00:44.103457 cruiz-1.4.0a4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-07-15 20:00:44.103457 cruiz-1.4.0a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 20:00:44.079457 cruiz-1.4.0a4/cruiz/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-15 20:00:44.000000 cruiz-1.4.0a4/cruiz/RELEASE_VERSION.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1509 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/application.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 20:00:44.079457 cruiz-1.4.0a4/cruiz/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/commands/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      500 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/commands/conanconf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1775 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/commands/conanenv.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6269 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/commands/conaninvocation.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25477 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/commands/context.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1731 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/commands/guardedlisttoflush.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2401 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/commands/logdetails.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4189 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/commands/messagereplyprocessor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5555 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/commands/metarequestconaninvocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/dumpobjecttypes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3627 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/environ.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/globals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 20:00:44.083457 cruiz-1.4.0a4/cruiz/interop/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/interop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17403 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/interop/commandparameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/interop/commonparameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/interop/dependencygraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/interop/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/interop/packagebinaryparameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/interop/packageidparameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/interop/packagenode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/interop/packagerevisionsparameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/interop/pod.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/interop/reciperevisionsparameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/interop/searchrecipesparameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 20:00:44.083457 cruiz-1.4.0a4/cruiz/load_recipe/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/load_recipe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/load_recipe/loadrecipewizard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 20:00:44.083457 cruiz-1.4.0a4/cruiz/load_recipe/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/load_recipe/pages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/load_recipe/pages/initialprofilepage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/load_recipe/pages/intropage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/load_recipe/pages/localcachepage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/load_recipe/pages/packageversionpage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    28943 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/mainwindow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 20:00:44.083457 cruiz-1.4.0a4/cruiz/manage_local_cache/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/manage_local_cache/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    36038 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/manage_local_cache/managelocalcachesdialog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 20:00:44.087457 cruiz-1.4.0a4/cruiz/manage_local_cache/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/manage_local_cache/widgets/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2449 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/manage_local_cache/widgets/addenvironmentdialog.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2425 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/manage_local_cache/widgets/addextraprofiledirectorydialog.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2525 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/manage_local_cache/widgets/addremotedialog.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      950 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/manage_local_cache/widgets/configpathorurl.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3684 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/manage_local_cache/widgets/installconfigdialog.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1902 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/manage_local_cache/widgets/keyvaluetable.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8370 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/manage_local_cache/widgets/movelocalcachedialog.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7548 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/manage_local_cache/widgets/newlocalcachewizard.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1877 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/manage_local_cache/widgets/newlocalcachewizardpages.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1683 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/manage_local_cache/widgets/progressdialogs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4933 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/manage_local_cache/widgets/remotestable.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1139 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/manage_local_cache/widgets/removeenvironmentdialog.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2239 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/manage_local_cache/widgets/runconancommanddialog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 20:00:44.087457 cruiz-1.4.0a4/cruiz/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/model/conanpackagetypeflags.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2494 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/model/graphaslistmodel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 20:00:44.087457 cruiz-1.4.0a4/cruiz/pyside6/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/pyside6/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 20:00:44.087457 cruiz-1.4.0a4/cruiz/recipe/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/recipe/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1632 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/recipe/dependencyview.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1206 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/recipe/expressioneditordialog.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1586 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/recipe/findtextdialog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 20:00:44.087457 cruiz-1.4.0a4/cruiz/recipe/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/recipe/logs/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6022 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/recipe/logs/command.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2234 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/recipe/recipe.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    61647 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/recipe/recipewidget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 20:00:44.087457 cruiz-1.4.0a4/cruiz/recipe/toolbars/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/recipe/toolbars/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6621 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/recipe/toolbars/behaviour.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9749 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/recipe/toolbars/buildfeatures.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    34321 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/recipe/toolbars/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 20:00:44.087457 cruiz-1.4.0a4/cruiz/remote_browser/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/remote_browser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 20:00:44.087457 cruiz-1.4.0a4/cruiz/remote_browser/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/remote_browser/pages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14680 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/remote_browser/pages/packagebinarypage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17534 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/remote_browser/pages/packageidpage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7201 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/remote_browser/pages/packagereferencepage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/remote_browser/pages/packagerevisionpage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/remote_browser/pages/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/remote_browser/pages/reciperevisionpage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/remote_browser/remotebrowser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2499 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/resourcegeneration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 20:00:44.091457 cruiz-1.4.0a4/cruiz/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/resources/001-rubbish.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/resources/002-null.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/resources/003-chemistry.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/resources/004-share.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/resources/005-box.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/resources/006-toolbox.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/resources/007-book.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/resources/008-cloud-computing.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/resources/009-import.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/resources/010-draw.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/resources/012-hammer.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/resources/013-pencil.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/resources/014-code.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    17753 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/resources/Cmake.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/resources/about_dialog.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/resources/cruise.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/resources/cruizres.qrc
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/resources/find_text_dialog.ui
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 20:00:44.095457 cruiz-1.4.0a4/cruiz/resources/inverted/
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/resources/inverted/001-rubbish.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/resources/inverted/003-chemistry.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/resources/inverted/004-share.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/resources/inverted/005-box.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/resources/inverted/006-toolbox.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/resources/inverted/007-book.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/resources/inverted/008-cloud-computing.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/resources/inverted/009-import.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/resources/inverted/010-draw.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    53573 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/resources/license-cruise.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    96863 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/resources/license.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/resources/load_recipe_wizard.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/resources/local_cache_add_environment.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/resources/local_cache_add_profile_directory.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/resources/local_cache_add_remote.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     7174 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/resources/local_cache_install_config.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    27112 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/resources/local_cache_manage.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/resources/local_cache_move.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     9596 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/resources/local_cache_new_wizard.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/resources/local_cache_remove_environment.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/resources/local_cache_run_command_dialog.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    46675 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/resources/preferences.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/resources/recipe_cmake_features_frame.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/resources/recipe_compiler_cache_configuration_dialog.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/resources/recipe_compilercache_features_frame.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/resources/recipe_cpucores_frame.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/resources/recipe_local_workflow_expression_editor.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/resources/recipe_profile_frame.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    32455 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/resources/recipe_window.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    28688 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/resources/remote_browser.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/resources/remote_browser_fileview.ui
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/restart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/revealonfilesystem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 20:00:44.095457 cruiz-1.4.0a4/cruiz/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/settings/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      582 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/settings/ensuredefaultlocalcache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 20:00:44.095457 cruiz-1.4.0a4/cruiz/settings/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/settings/managers/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10185 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/settings/managers/basesettings.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4871 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/settings/managers/cleansettings.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1728 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/settings/managers/cmakepreferences.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3244 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/settings/managers/compilercachepreferences.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2499 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/settings/managers/conanpreferences.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2309 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/settings/managers/fontpreferences.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6433 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/settings/managers/generalpreferences.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1890 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/settings/managers/graphvizpreferences.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3903 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/settings/managers/localcachepreferences.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14295 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/settings/managers/namedlocalcache.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1830 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/settings/managers/ninjapreferences.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3681 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/settings/managers/recentconanconfigs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3590 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/settings/managers/recentconanremotes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3564 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/settings/managers/recentrecipes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18357 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/settings/managers/recipe.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      317 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/settings/managers/restoredefaults.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7928 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/settings/managers/shortcuts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1149 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/settings/managers/valueclasses.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4155 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/settings/managers/writermixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 20:00:44.095457 cruiz-1.4.0a4/cruiz/settings/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/settings/models/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1419 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/settings/models/recentconanconfigmodel.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1345 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/settings/models/recentconanremotesmodel.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2701 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/settings/models/recipesmodel.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    55936 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/settings/preferencesdialog.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14474 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/settings/updatesettings.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5848 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/svggraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 20:00:44.095457 cruiz-1.4.0a4/cruiz/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/widgets/aboutcruizdialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11414 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/widgets/debugging.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1211 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/widgets/shortcutlineedit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2050 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/widgets/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 20:00:44.095457 cruiz-1.4.0a4/cruiz/workers/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/workers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 20:00:44.099457 cruiz-1.4.0a4/cruiz/workers/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/workers/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 20:00:44.099457 cruiz-1.4.0a4/cruiz/workers/api/common/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/workers/api/common/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      405 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/workers/api/common/endmessagethread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 20:00:44.099457 cruiz-1.4.0a4/cruiz/workers/api/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/workers/api/v1/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      655 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/workers/api/v1/arbitrary.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      965 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/workers/api/v1/build.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2168 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/workers/api/v1/cmakebuildtool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/workers/api/v1/conanapi.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1580 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/workers/api/v1/configinstall.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1238 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/workers/api/v1/create.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      915 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/workers/api/v1/deletecmakecache.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1442 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/workers/api/v1/exportpackage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      818 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/workers/api/v1/imports.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1382 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/workers/api/v1/install.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4949 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/workers/api/v1/lockcreate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15767 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/workers/api/v1/meta.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7679 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/workers/api/v1/monkeypatch.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      971 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/workers/api/v1/package.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1706 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/workers/api/v1/packagebinary.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1341 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/workers/api/v1/packagedetails.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      763 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/workers/api/v1/packagerevisions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      758 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/workers/api/v1/reciperevisions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2171 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/workers/api/v1/remotesearch.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      699 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/workers/api/v1/removeallpackages.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      509 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/workers/api/v1/removelocks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      970 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/workers/api/v1/removepackage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      784 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/workers/api/v1/source.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1120 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/workers/api/v1/testpackage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/workers/api/v1/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 20:00:44.103457 cruiz-1.4.0a4/cruiz/workers/api/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/workers/api/v2/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1079 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/workers/api/v2/arbitrary.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      928 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/workers/api/v2/build.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1574 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/workers/api/v2/configinstall.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      795 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/workers/api/v2/create.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      862 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/workers/api/v2/exportpackage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      857 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/workers/api/v2/install.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4564 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/workers/api/v2/lockcreate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6754 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/workers/api/v2/meta.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1282 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/workers/api/v2/packagebinary.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1326 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/workers/api/v2/packagedetails.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1452 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/workers/api/v2/packagerevisions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1400 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/workers/api/v2/reciperevisions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1120 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/workers/api/v2/remotesearch.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      803 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/workers/api/v2/removeallpackages.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1048 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/workers/api/v2/removepackage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      895 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/workers/api/v2/source.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      846 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/workers/api/v2/testpackage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/workers/api/v2/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 20:00:44.103457 cruiz-1.4.0a4/cruiz/workers/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/workers/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/workers/utils/colorarma_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/workers/utils/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/workers/utils/formatoptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1493 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/workers/utils/qtlogger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/workers/utils/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/workers/utils/text2html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/cruiz/workers/utils/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 20:00:44.079457 cruiz-1.4.0a4/cruiz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-07-15 20:00:44.000000 cruiz-1.4.0a4/cruiz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8514 2023-07-15 20:00:44.000000 cruiz-1.4.0a4/cruiz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 20:00:44.000000 cruiz-1.4.0a4/cruiz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-15 20:00:44.000000 cruiz-1.4.0a4/cruiz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-15 20:00:44.000000 cruiz-1.4.0a4/cruiz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-15 20:00:44.000000 cruiz-1.4.0a4/cruiz.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 20:00:44.103457 cruiz-1.4.0a4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-07-15 20:00:21.000000 cruiz-1.4.0a4/setup.py
```

### Comparing `cruiz-1.4.0a3/LICENSE` & `cruiz-1.4.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/PKG-INFO` & `cruiz-1.4.0a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cruiz
-Version: 1.4.0a3
+Version: 1.4.0a4
 Summary: Conan recipe user interface
 Home-page: https://github.com/markfinal/cruiz
 Author: Mark Final
 Author-email: markfinal@hotmail.com
 Project-URL: Documentation, https://cruiz.readthedocs.io/en/latest/
 Project-URL: GitHub, https://github.com/markfinal/cruiz
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cruiz-1.4.0a3/README.md` & `cruiz-1.4.0a4/README.md`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/application.py` & `cruiz-1.4.0a4/cruiz/application.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,21 +4,18 @@
 The Qt application
 """
 
 from __future__ import annotations
 
 import typing
 
-import qdarkstyle
-
 from qtpy import QtCore, QtGui, QtWidgets
 
 from cruiz.settings.ensuredefaultlocalcache import ensure_default_local_cache
 from cruiz.settings.managers.fontpreferences import FontSettingsReader, FontUsage
-from cruiz.settings.managers.generalpreferences import GeneralSettingsReader
 
 
 class Application(QtWidgets.QApplication):
     """
     The application
     """
 
@@ -40,18 +37,13 @@
         # pylint: disable=undefined-variable
         return qApp  # type: ignore  # noqa: F821
 
     def on_preferences_updated(self) -> None:
         """
         Slot executed when preferences have reported an update.
         """
-        with GeneralSettingsReader() as settings:
-            use_dark_mode = settings.use_dark_mode.resolve()
-        self.setStyleSheet(
-            qdarkstyle.load_stylesheet_pyside6() if use_dark_mode else ""
-        )
         with FontSettingsReader(FontUsage.UI) as settings:
             font_details = (settings.name.resolve(), settings.size.resolve())
         if font_details[0]:
             self.setFont(QtGui.QFont(*font_details))
         else:
             self.setFont(self.default_font)
```

### Comparing `cruiz-1.4.0a3/cruiz/commands/conanenv.py` & `cruiz-1.4.0a4/cruiz/commands/conanenv.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 import logging
 import typing
 
 import cruiz.globals
 
 from cruiz.settings.managers.conanpreferences import ConanSettingsReader
-from cruiz.settings.managers.generalpreferences import GeneralSettingsReader
 from cruiz.settings.managers.namedlocalcache import NamedLocalCacheSettingsReader
 
 
 logger = logging.getLogger(__name__)
 
 
 def get_conan_env(
@@ -37,17 +36,15 @@
             env["CONAN_USER_HOME"] = home_dir
         if short_home_dir:
             env["CONAN_USER_HOME_SHORT"] = short_home_dir
     else:
         if home_dir:
             env["CONAN_HOME"] = home_dir
         # short home no longer needed
-    with GeneralSettingsReader() as settings:
-        use_dark_mode = settings.use_dark_mode.resolve()
-    env["CONAN_COLOR_DARK"] = "0" if use_dark_mode else "1"
+    env["CONAN_COLOR_DARK"] = "0" if cruiz.globals.is_dark_theme() else "1"
     if cruiz.globals.CONAN_MAJOR_VERSION == 1:
         with ConanSettingsReader() as settings:
             log_level = settings.log_level.resolve()
             env["CONAN_LOGGING_LEVEL"] = log_level
         env["CONAN_NON_INTERACTIVE"] = "1"
     # custom environment variables - this is where cruiz behaviour might vary
     # from Conan on the command line
```

### Comparing `cruiz-1.4.0a3/cruiz/commands/conaninvocation.py` & `cruiz-1.4.0a4/cruiz/commands/conaninvocation.py`

 * *Files 6% similar despite different names*

```diff
@@ -81,17 +81,15 @@
 
     def _disconnect_signal(self, result: typing.Any, exception: typing.Any) -> None:
         # pylint: disable=unused-argument
         self._queue_processor.completed.disconnect()
         self._last_command_running = False
 
     def _critical_failure(self, message: str) -> None:
-        QtWidgets.QMessageBox.critical(
-            None, "System failure", message  # type: ignore[call-overload]
-        )
+        QtWidgets.QMessageBox.critical(None, "System failure", message)
         sys.exit(1)
 
     def invoke(
         self,
         parameters: typing.Union[
             CommandParameters,
             SearchRecipesParameters,
```

### Comparing `cruiz-1.4.0a3/cruiz/commands/context.py` & `cruiz-1.4.0a4/cruiz/commands/context.py`

 * *Files 0% similar despite different names*

```diff
@@ -457,29 +457,25 @@
     def get_list_of_profiles(self) -> typing.List[typing.Tuple[pathlib.Path, str]]:
         """
         Return a list of all profiles in this context.
         """
         profile_paths: typing.List[typing.Tuple[pathlib.Path, str]] = []
         # TODO: Conan2 candidate: api.profiles.list() for the local-cache based profiles
         profiles_dir = QtCore.QDir(str(self.profiles_dir()))
-        for profile in profiles_dir.entryList(  # type: ignore
-            filters=QtCore.QDir.Files
-        ):
+        for profile in profiles_dir.entryList(filters=QtCore.QDir.Files):
             # local cache profiles are listed relative
             path = pathlib.Path(profiles_dir.filePath(profile))
             text = path.read_text()
             profile_paths.append((pathlib.Path(path.name), text))
         # in Conan 2, there can be no profiles at this point
         with NamedLocalCacheSettingsReader(self.cache_name) as settings:
             extra_profile_dirs = settings.extra_profile_directories.resolve()
         for _, extra_profile_dir in extra_profile_dirs.items():
             profiles_dir = QtCore.QDir(extra_profile_dir)
-            for profile in profiles_dir.entryList(  # type: ignore
-                filters=QtCore.QDir.Files
-            ):
+            for profile in profiles_dir.entryList(filters=QtCore.QDir.Files):
                 # extra profiles are listed absolute
                 path = pathlib.Path(profiles_dir.filePath(profile))
                 text = path.read_text()
                 profile_paths.append((path, text))
         return profile_paths
 
     def run_any_command(
```

### Comparing `cruiz-1.4.0a3/cruiz/commands/guardedlisttoflush.py` & `cruiz-1.4.0a4/cruiz/commands/guardedlisttoflush.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/commands/logdetails.py` & `cruiz-1.4.0a4/cruiz/commands/logdetails.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/commands/messagereplyprocessor.py` & `cruiz-1.4.0a4/cruiz/commands/messagereplyprocessor.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/commands/metarequestconaninvocation.py` & `cruiz-1.4.0a4/cruiz/commands/metarequestconaninvocation.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/constants.py` & `cruiz-1.4.0a4/cruiz/constants.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/dumpobjecttypes.py` & `cruiz-1.4.0a4/cruiz/dumpobjecttypes.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/entrypoint.py` & `cruiz-1.4.0a4/cruiz/entrypoint.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,22 +9,20 @@
 import os
 import pathlib
 import platform
 import sys
 
 from qtpy import QtCore, QtWidgets
 
-from cruiz.resourcegeneration import generate_resources
-
 
 CONAN_SPEC = importlib.util.find_spec("conans")
 if CONAN_SPEC is None:
     QtWidgets.QApplication()
     QtWidgets.QMessageBox.critical(
-        None,  # type: ignore
+        None,
         "Conan unavailable",
         "Unable to locate the conan Python package in the current environment.\n"
         "Use pip install conan[==version].",
     )
     sys.exit(-1)
 
 
@@ -32,17 +30,14 @@
     level=os.getenv("LOGLEVEL", "WARNING"),
     filename=os.getenv("LOGFILE", None),
 )
 
 
 logger = logging.getLogger(__name__)
 
-# resource generation be invoked before resources and MainWindow are imported
-generate_resources()
-
 import cruiz.pyside6.resources  # noqa: F401, E402
 
 from cruiz.application import Application  # noqa: E402
 from cruiz.mainwindow import MainWindow  # noqa: E402
 from cruiz.settings.updatesettings import (  # noqa: E402
     update_settings_to_current_version,
 )
@@ -71,15 +66,15 @@
     output_mtime = os.path.getmtime(newest_generated_file)
     return input_mtime > output_mtime
 
 
 if _are_resources_out_of_date():
     QtWidgets.QApplication()
     QtWidgets.QMessageBox.critical(
-        None,  # type: ignore
+        None,
         "Resources",
         "Resources are out of date.\n" "Please build with python3 setup.py build",
     )
     sys.exit(-1)
 
 
 QtCore.QCoreApplication.setApplicationName("cruiz")
@@ -127,12 +122,13 @@
 
     QtWidgets.QApplication.setAttribute(
         QtCore.Qt.AA_EnableHighDpiScaling, True
     )  # enable highdpi scaling
     QtWidgets.QApplication.setAttribute(
         QtCore.Qt.AA_UseHighDpiPixmaps, True
     )  # use highdpi icons
+    QtWidgets.QApplication.setStyle("fusion")
 
     app = Application(sys.argv)
     window = MainWindow()
     window.showNormal()
     sys.exit(app.exec_())
```

### Comparing `cruiz-1.4.0a3/cruiz/environ.py` & `cruiz-1.4.0a4/cruiz/environ.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/exceptions.py` & `cruiz-1.4.0a4/cruiz/exceptions.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/globals.py` & `cruiz-1.4.0a4/cruiz/globals.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,23 +8,41 @@
 from __future__ import annotations
 import typing
 
 CRUIZ_MAINWINDOW: typing.Optional[cruiz.MainWindow] = None  # type: ignore # noqa: F821
 
 CONAN_MAJOR_VERSION: int = 0
 
+CRUIZ_THEME: typing.Optional[str] = None
+
 
 def get_main_window() -> cruiz.MainWindow:  # type: ignore # noqa: F821
     """
     Get the main window for the application, asserting it is valid
     """
     assert CRUIZ_MAINWINDOW
     return CRUIZ_MAINWINDOW
 
 
+def get_theme() -> str:
+    """
+    Get the name of the current theme
+    """
+    assert CRUIZ_THEME
+    return CRUIZ_THEME
+
+
+def is_dark_theme() -> bool:
+    """
+    Is the current theme the dark theme?
+    """
+    assert CRUIZ_THEME
+    return CRUIZ_THEME == "Dark"
+
+
 def __capture_conan_version() -> None:
     global CONAN_MAJOR_VERSION
     if CONAN_MAJOR_VERSION > 0:
         return
 
     import subprocess
```

### Comparing `cruiz-1.4.0a3/cruiz/interop/commandparameters.py` & `cruiz-1.4.0a4/cruiz/interop/commandparameters.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/interop/dependencygraph.py` & `cruiz-1.4.0a4/cruiz/interop/dependencygraph.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/interop/message.py` & `cruiz-1.4.0a4/cruiz/interop/message.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/interop/packagenode.py` & `cruiz-1.4.0a4/cruiz/interop/packagenode.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/interop/pod.py` & `cruiz-1.4.0a4/cruiz/interop/pod.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/interop/reciperevisionsparameters.py` & `cruiz-1.4.0a4/cruiz/interop/reciperevisionsparameters.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/interop/searchrecipesparameters.py` & `cruiz-1.4.0a4/cruiz/interop/searchrecipesparameters.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/load_recipe/loadrecipewizard.py` & `cruiz-1.4.0a4/cruiz/load_recipe/loadrecipewizard.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/load_recipe/pages/initialprofilepage.py` & `cruiz-1.4.0a4/cruiz/load_recipe/pages/initialprofilepage.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/load_recipe/pages/localcachepage.py` & `cruiz-1.4.0a4/cruiz/load_recipe/pages/localcachepage.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/load_recipe/pages/packageversionpage.py` & `cruiz-1.4.0a4/cruiz/load_recipe/pages/packageversionpage.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,15 @@
 
     def _get_versions_from_conandata(
         self, conandata: typing.Dict[str, typing.Dict[str, str]]
     ) -> typing.Optional[typing.List[str]]:
         assert conandata
         with ConanSettingsReader() as settings:
             path_segments = settings.conandata_version_yaml_pathsegment.resolve()
-        if path_segments is None:
+        if not path_segments:
             QtWidgets.QMessageBox.information(
                 self,
                 "Cannot identify recipe version numbers from conandata.yml file",
                 "The conandata.yml beside the recipe cannot be parsed for version "
                 "numbers.\n\n"
                 "This is because cruiz cannot determine its format without a hint.\n\n"
                 "Complete the 'Preferences->Conan->Parsing conandata' setting to "
```

### Comparing `cruiz-1.4.0a3/cruiz/mainwindow.py` & `cruiz-1.4.0a4/cruiz/mainwindow.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,25 +67,33 @@
 
     # pylint: disable=too-many-instance-attributes, too-many-locals
 
     profile_dirs_changed = QtCore.Signal()
     remote_added_to_cache = QtCore.Signal(str)
     preferences_updated = QtCore.Signal()
     local_cache_changed = QtCore.Signal(str)
+    theme_changed = QtCore.Signal(str)
 
     def __del__(self) -> None:
         logger.debug("-=%d", id(self))
 
     def __init__(self) -> None:
         # pylint: disable=too-many-statements, global-statement
         super().__init__()
         log_created_widget(self, logger)
 
         assert not cruiz.globals.CRUIZ_MAINWINDOW
 
+        qApp.styleHints().colorSchemeChanged.connect(  # type: ignore # noqa: F821
+            self._on_platform_theme_changed
+        )
+        self._on_platform_theme_changed(
+            qApp.styleHints().colorScheme()  # type: ignore # noqa: F821
+        )
+
         self._systray = None
         if QtWidgets.QSystemTrayIcon.isSystemTrayAvailable():
             self._app_icon = QtGui.QIcon(":/cruiz.png")
             self._app_menu = QtWidgets.QMenu()
             self._systray = QtWidgets.QSystemTrayIcon(self._app_icon, self)
             self._systray.setContextMenu(self._app_menu)
             self._systray.show()
@@ -320,15 +328,15 @@
         with RecentRecipeSettingsReader() as recent_reader:
             uuids = recent_reader.uuids()
         has_recipe_settings_issue = False
         all_uuids_with_settings = RecipeSettings().all_uuids
         for uuid in uuids:
             with RecipeSettingsReader.from_uuid(uuid) as settings:
                 path = settings.path.resolve()
-                if path is None:
+                if not path:
                     has_recipe_settings_issue = True
                     continue
                 recipe_path = pathlib.Path(path)
                 if not recipe_path.exists():
                     has_recipe_settings_issue = True
                     # can drop through even though the path doesn't exist
                 attributes = settings.attribute_overrides.resolve()
@@ -679,7 +687,15 @@
         Is the recipe with the given UUID active (i.e. has an open tab)?
         """
         mdi_area = self.centralWidget()
         return any(
             subwindow.widget().recipe.uuid == uuid
             for subwindow in mdi_area.subWindowList()
         )
+
+    def _on_platform_theme_changed(
+        self, color_scheme: QtCore.Qt.ColorScheme  # type: ignore[name-defined]
+    ) -> None:
+        if color_scheme == QtCore.Qt.ColorScheme.Unknown:
+            color_scheme = QtCore.Qt.ColorScheme.Light
+        cruiz.globals.CRUIZ_THEME = color_scheme.name
+        self.theme_changed.emit(color_scheme.name)
```

### Comparing `cruiz-1.4.0a3/cruiz/manage_local_cache/managelocalcachesdialog.py` & `cruiz-1.4.0a4/cruiz/manage_local_cache/managelocalcachesdialog.py`

 * *Files 0% similar despite different names*

```diff
@@ -303,15 +303,15 @@
             self._ui.profilesTable.add_key_value_pair(name, profile_dir)
         self._ui.profilesList.clear()
         for i, (profile_path, profile_text) in enumerate(
             self._context.get_list_of_profiles()
         ):
             self._ui.profilesList.addItem(str(profile_path))
             item = self._ui.profilesList.item(i)
-            item.setData(QtCore.Qt.ToolTipRole, profile_text)  # type: ignore[arg-type]
+            item.setData(QtCore.Qt.ToolTipRole, profile_text)
 
     def _update_cache_config(self) -> None:
         if self._ui.configPrintRunCommands.isVisible():
             with BlockSignals(self._ui.configPrintRunCommands) as blocked_widget:
                 blocked_widget.setCheckState(
                     QtCore.Qt.Checked
                     if self._context.get_boolean_config(
@@ -533,15 +533,17 @@
             if "Toggled" not in self._modifications:
                 self._modifications["Remotes"]["Toggled"] = []
             self._modifications["Remotes"]["Toggled"].append(name)
 
         if remote in added_remotes:
             self._modifications["Remotes"]["Add"].remove(remote)
             self._modifications["Remotes"]["Add"].append(
-                dataclasses.replace(remote, enabled=state == QtCore.Qt.Checked)
+                dataclasses.replace(
+                    remote, enabled=QtCore.Qt.CheckState(state) == QtCore.Qt.Checked
+                )
             )
 
         # check that the remote was uniquely named
         remote = next(remote_iterator, None)
         assert remote is None
         self._modified.emit()
```

### Comparing `cruiz-1.4.0a3/cruiz/manage_local_cache/widgets/__init__.py` & `cruiz-1.4.0a4/cruiz/manage_local_cache/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/manage_local_cache/widgets/addenvironmentdialog.py` & `cruiz-1.4.0a4/cruiz/manage_local_cache/widgets/addenvironmentdialog.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         for key in context.get_conan_config_environment_variables():
             key_action = QtGui.QAction(key, self)
             key_action.triggered.connect(self._set_name)
             conan_environment_actions.append(key_action)
         if cruiz.globals.CONAN_MAJOR_VERSION == 1:
             # TODO: CONAN_V2_MODE is obsolete
             conan_v2_mode_action = QtGui.QAction("CONAN_V2_MODE", self)
-            conan_v2_mode_action.triggered.connect(self._set_name)  # type: ignore
+            conan_v2_mode_action.triggered.connect(self._set_name)
             conan_environment_actions.append(conan_v2_mode_action)
         self._ui.name.add_submenu_actions(
             "Conan environment variables", conan_environment_actions
         )
         self._ui.name.textChanged.connect(self._updated)
         self._ui.value.textChanged.connect(self._updated)
         self._ui.buttonBox.button(QtWidgets.QDialogButtonBox.Ok).setEnabled(False)
```

### Comparing `cruiz-1.4.0a3/cruiz/manage_local_cache/widgets/addextraprofiledirectorydialog.py` & `cruiz-1.4.0a4/cruiz/manage_local_cache/widgets/addextraprofiledirectorydialog.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/manage_local_cache/widgets/addremotedialog.py` & `cruiz-1.4.0a4/cruiz/manage_local_cache/widgets/addremotedialog.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/manage_local_cache/widgets/configpathorurl.py` & `cruiz-1.4.0a4/cruiz/manage_local_cache/widgets/configpathorurl.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/manage_local_cache/widgets/installconfigdialog.py` & `cruiz-1.4.0a4/cruiz/manage_local_cache/widgets/installconfigdialog.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/manage_local_cache/widgets/keyvaluetable.py` & `cruiz-1.4.0a4/cruiz/manage_local_cache/widgets/keyvaluetable.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/manage_local_cache/widgets/movelocalcachedialog.py` & `cruiz-1.4.0a4/cruiz/manage_local_cache/widgets/movelocalcachedialog.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/manage_local_cache/widgets/newlocalcachewizard.py` & `cruiz-1.4.0a4/cruiz/manage_local_cache/widgets/newlocalcachewizard.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/manage_local_cache/widgets/newlocalcachewizardpages.py` & `cruiz-1.4.0a4/cruiz/manage_local_cache/widgets/newlocalcachewizardpages.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/manage_local_cache/widgets/progressdialogs.py` & `cruiz-1.4.0a4/cruiz/manage_local_cache/widgets/progressdialogs.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/manage_local_cache/widgets/remotestable.py` & `cruiz-1.4.0a4/cruiz/manage_local_cache/widgets/remotestable.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/manage_local_cache/widgets/removeenvironmentdialog.py` & `cruiz-1.4.0a4/cruiz/manage_local_cache/widgets/removeenvironmentdialog.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/manage_local_cache/widgets/runconancommanddialog.py` & `cruiz-1.4.0a4/cruiz/manage_local_cache/widgets/runconancommanddialog.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/model/graphaslistmodel.py` & `cruiz-1.4.0a4/cruiz/model/graphaslistmodel.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/recipe/dependencyview.py` & `cruiz-1.4.0a4/cruiz/recipe/dependencyview.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/recipe/expressioneditordialog.py` & `cruiz-1.4.0a4/cruiz/recipe/expressioneditordialog.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/recipe/findtextdialog.py` & `cruiz-1.4.0a4/cruiz/recipe/findtextdialog.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/recipe/logs/command.py` & `cruiz-1.4.0a4/cruiz/recipe/logs/command.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/recipe/recipe.py` & `cruiz-1.4.0a4/cruiz/recipe/recipe.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/recipe/recipewidget.py` & `cruiz-1.4.0a4/cruiz/recipe/recipewidget.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         self._ui.setupUi(self)  # type: ignore[no-untyped-call]
         try:
             self._git_repository: typing.Optional[git.Repo] = git.Repo(
                 path, search_parent_directories=True
             )
         except NameError:
             self._git_repository = None
-        except git.exc.InvalidGitRepositoryError:  # type: ignore
+        except git.exc.InvalidGitRepositoryError:
             self._git_repository = None
         self._ui.paneSplitter.setStretchFactor(0, 4)
         self._ui.paneSplitter.setStretchFactor(1, 1)
         self._ui.outputPane.customContextMenuRequested.connect(self._pane_context_menu)
         self._ui.errorPane.customContextMenuRequested.connect(self._pane_context_menu)
         self._empty_widget = QtWidgets.QWidget(self)
         self._empty_widget.setFixedSize(0, 0)
@@ -354,14 +354,16 @@
             self,
         )
         self.recipe.context.command_history_widget = self._ui.conanCommandHistory
 
         self._create_statusbar()
         self._load_local_workflow_dock()
 
+        cruiz.globals.get_main_window().theme_changed.connect(self._on_theme_change)
+
     def post_init(self) -> None:
         """
         Post initialisation commands that need to be performed once the
         recipe is visible, or that might fail (e.g. recipe syntax error)
         """
         attributes = self.get_recipe_attributes()
         self._update_window_title(attributes)
@@ -395,63 +397,67 @@
         Get the attributes written into the recipe
         """
         return self.recipe.context.inspect_recipe(
             self.recipe.path, propagate_errors=True
         )
 
     def _get_options_from_recipe(
-        self, attrs: typing.Dict[str, str]
-    ) -> typing.List[typing.Tuple[str, typing.List[typing.Any], typing.Any]]:
-        if cruiz.globals.CONAN_MAJOR_VERSION == 1:
-            # this lists the possible values for the option
-            options = attrs.get("options")
-        else:
-            # don't use the 'options' key, as that has been assigned the value
-            # options_definitions is where the possible values are
-            options = attrs.get("options_definitions")
+        self, attrs: typing.Dict[str, typing.Any]
+    ) -> typing.List[
+        typing.Tuple[str, typing.Union[str, typing.List[typing.Any]], typing.Any]
+    ]:
+        # this lists the possible values for the option
+        # in Conan 2, don't use the 'options' key, as that has been assigned the value
+        options: typing.Optional[typing.Dict[str, typing.Any]] = (
+            attrs.get("options")
+            if cruiz.globals.CONAN_MAJOR_VERSION == 1
+            else attrs.get("options_definitions")
+        )
         if not options:
             return []
         default_options = attrs["default_options"]
         if isinstance(default_options, (tuple, list)):
             as_dict = {}
             for entry in default_options:
                 key, value = entry.split("=")
                 as_dict[key] = value
             default_options = as_dict
         assert isinstance(
             default_options, dict
         ), "Expected default_options to be a dict"
-        values: typing.List[typing.Tuple[str, typing.List[typing.Any], typing.Any]] = []
+        values: typing.List[
+            typing.Tuple[str, typing.Union[str, typing.List[typing.Any]], typing.Any]
+        ] = []
         assert isinstance(options, dict)
         for key, value in options.items():
             if default_options:
                 if cruiz.globals.CONAN_MAJOR_VERSION == 1:
                     default_value = default_options[key]
                 else:
                     # when the recipe is serialised,
                     # default_options come through as typed (e.g. bool)
                     # while option_definitions are all strings, so in order to compare
                     # let's do everything as strings
                     default_value = str(default_options[key])
-                if isinstance(value, list) and default_value not in value:
-                    if isinstance(value[0], bool):
+                if isinstance(value, list):
+                    if default_value not in value and isinstance(value[0], bool):
                         default_value = _strtobool(default_value)
                         assert default_value in value, (
                             f"Cannot find default value '{default_value}' in possible "
                             f"values {value}"
                         )
-                    elif (isinstance(value, str) and value == "ANY") or (
-                        isinstance(value, list) and "ANY" in value
-                    ):
-                        pass
-                    else:
-                        raise TypeError(
-                            f"Don't know how to convert '{default_value}' to type "
-                            f"'{type(value[0])}'"
-                        )
+                elif (isinstance(value, str) and value == "ANY") or (
+                    isinstance(value, list) and "ANY" in value
+                ):
+                    pass
+                else:
+                    raise TypeError(
+                        f"Don't know how to convert '{default_value}' to type "
+                        f"'{type(value[0])}'"
+                    )
                 values.append((key, value, default_value))
             else:
                 values.append((key, value, None))
         return values
 
     # TODO: why does this have to be PurePosixPath? to create such a path,
     # it cannot be pure
@@ -1089,15 +1095,15 @@
         params.version = self.recipe.version
         params.user = self.recipe.user
         params.channel = self.recipe.channel
         with RecipeSettingsReader.from_recipe(self.recipe) as settings:
             params.profile = settings.profile.resolve()
             for key, value in settings.options.resolve().items():
                 # TODO: is this the most efficient algorithm?
-                params.add_option(params.name, key, value)  # type: ignore
+                params.add_option(params.name, key, value)
             attributes = settings.attribute_overrides.resolve()
             if "extra_config_options" in attributes:
                 for keyvalue in attributes["extra_config_options"].split(","):
                     option_name, option_value = keyvalue.split("=")
                     params.add_option(None, option_name, option_value)
         self._dependency_generate_context.conancommand(
             params,
@@ -1390,7 +1396,11 @@
         action.triggered.connect(self._on_configure_package_id_copy)
         menu = QtWidgets.QMenu(self)
         menu.addAction(action)
         menu.exec_(self.sender().mapToGlobal(position))
 
     def _on_configure_package_id_copy(self) -> None:
         QtWidgets.QApplication.clipboard().setText(self._ui.configurePackageId.text())
+
+    def _on_theme_change(self) -> None:
+        attributes = self.get_recipe_attributes()
+        self._ui.commandToolbar.refresh_action_shortcuts_and_tooltips(attributes)
```

### Comparing `cruiz-1.4.0a3/cruiz/recipe/toolbars/behaviour.py` & `cruiz-1.4.0a4/cruiz/recipe/toolbars/behaviour.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/recipe/toolbars/buildfeatures.py` & `cruiz-1.4.0a4/cruiz/recipe/toolbars/buildfeatures.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,24 +47,22 @@
             verbose = settings.cmake_verbose.resolve()
         with BlockSignals(self._ui.cmakeFindDebug) as blocked_widget:
             blocked_widget.setChecked(find_debug)
         with BlockSignals(self._ui.cmakeVerbose) as blocked_widget:
             blocked_widget.setChecked(verbose)
 
     def _toggle_cmake_find_debug_mode(self, state: int) -> None:
-        is_checked = state == QtCore.Qt.Checked  # type: ignore[comparison-overlap]
         settings = RecipeSettings()
-        settings.cmake_find_debug = is_checked  # type: ignore
+        settings.cmake_find_debug = QtCore.Qt.CheckState(state) == QtCore.Qt.Checked
         assert self._uuid
         RecipeSettingsWriter.from_uuid(self._uuid).sync(settings)
 
     def _toggle_cmake_verbose(self, state: int) -> None:
-        is_checked = state == QtCore.Qt.Checked  # type: ignore[comparison-overlap]
         settings = RecipeSettings()
-        settings.cmake_verbose = is_checked  # type: ignore
+        settings.cmake_verbose = QtCore.Qt.CheckState(state) == QtCore.Qt.Checked
         assert self._uuid
         RecipeSettingsWriter.from_uuid(self._uuid).sync(settings)
 
 
 class _CompilerCacheConfigurationDialog(QtWidgets.QDialog):
     modified = QtCore.Signal()
 
@@ -192,15 +190,15 @@
             self._ui.chooseCache.setItemIcon(
                 i,
                 QtGui.QIcon(":/cruiz.png") if i == default_index else QtGui.QIcon(),
             )
         return default_compiler_cache
 
     def _toggle_use_cache(self, state: int) -> None:
-        is_checked = state == QtCore.Qt.Checked  # type: ignore[comparison-overlap]
+        is_checked = QtCore.Qt.CheckState(state) == QtCore.Qt.Checked
         settings = RecipeSettings()
         cache_name = self._ui.chooseCache.currentText() if is_checked else None
         settings.compiler_cache = cache_name  # type: ignore[assignment]
         assert self._uuid
         RecipeSettingsWriter.from_uuid(self._uuid).sync(settings)
         self._ui.chooseCache.setEnabled(is_checked)
         self.refresh_content(self._uuid)
```

### Comparing `cruiz-1.4.0a3/cruiz/recipe/toolbars/command.py` & `cruiz-1.4.0a4/cruiz/recipe/toolbars/command.py`

 * *Files 3% similar despite different names*

```diff
@@ -171,95 +171,137 @@
             cancel = settings.cancel.resolve()
             conan_remove = settings.conan_remove_package.resolve()
             if IS_CONAN_V1:
                 cmake_build_tool = settings.cmake_build_tool.resolve()
                 cmake_build_tool_verbose = settings.cmake_build_tool_verbose.resolve()
                 remove_cmakecache = settings.delete_cmake_cache.resolve()
 
-        def _configure(
-            action: QtGui.QAction, shortcut: str, params: CommandParameters
+        def _configure_conan_action(
+            action: QtGui.QAction,
+            shortcut: str,
+            params: CommandParameters,
+            icon_path: str,
         ) -> None:
             action.setShortcut(QtGui.QKeySequence(shortcut))
             action.setToolTip(self._generate_command_tooltip(params))
+            if icon_path.startswith(":/"):
+                icon = QtGui.QIcon(icon_path)
+            else:
+                icon = QtGui.QIcon(f":/icons/{cruiz.globals.get_theme()}/{icon_path}")
+            action.setIcon(icon)
 
         recipe_ui = self.parent()._ui
-        _configure(
+        _configure_conan_action(
             recipe_ui.actionCreateCommand,
             conan_create,
             self._make_conan_create_params(recipe_attributes, None),
+            "create.svg",
         )
-        _configure(
+        _configure_conan_action(
             recipe_ui.actionCreateUpdateCommand,
             conan_create_updates,
             self._make_conan_create_params(recipe_attributes, ["-u"]),
+            "create.svg",
         )
-        _configure(
+        _configure_conan_action(
             recipe_ui.actionInstallCommand,
             conan_install,
             self._make_conan_install_params(recipe_attributes, None),
+            "install.svg",
         )
-        _configure(
+        _configure_conan_action(
             recipe_ui.actionInstallUpdateCommand,
             conan_install_updates,
             self._make_conan_install_params(recipe_attributes, ["-u"]),
+            "install.svg",
         )
         if IS_CONAN_V1:
-            _configure(
+            _configure_conan_action(
                 recipe_ui.actionImportsCommand,
                 conan_imports,
                 self._make_conan_imports_params(recipe_attributes),
+                "imports.svg",
             )
-        _configure(
+        _configure_conan_action(
             recipe_ui.actionSourceCommand,
             conan_source,
             self._make_conan_source_params(recipe_attributes),
+            "source.svg",
         )
-        _configure(
+        _configure_conan_action(
             recipe_ui.actionBuildCommand,
             conan_build,
             self._make_conan_build_params(recipe_attributes),
+            "build.svg",
         )
         if IS_CONAN_V1:
-            _configure(
+            _configure_conan_action(
                 recipe_ui.actionPackageCommand,
                 conan_package,
                 self._make_conan_package_params(recipe_attributes),
+                "package.svg",
             )
-        _configure(
+        _configure_conan_action(
             recipe_ui.actionExportPackageCommand,
             conan_exportpkg,
             self._make_conan_export_package_params(recipe_attributes),
+            "exportpackage.svg",
         )
-        _configure(
+        _configure_conan_action(
             recipe_ui.actionTestCommand,
             conan_test,
             self._make_conan_test_package_params(recipe_attributes),
+            "testpackage.svg",
         )
-        recipe_ui.actionCancelCommand.setShortcut(QtGui.QKeySequence(cancel))
-        recipe_ui.actionCancelCommand.setToolTip("Cancel the currently running command")
-        _configure(
+        _configure_conan_action(
             recipe_ui.actionRemovePackageCommand,
             conan_remove,
             self._make_conan_remove_package_params(recipe_attributes),
+            "removepackage.svg",
         )
+
+        def _configure_non_conan_action(
+            action: QtGui.QAction, shortcut: str, tooltip: str, icon_path: str
+        ) -> None:
+            action.setShortcut(QtGui.QKeySequence(shortcut))
+            action.setToolTip(tooltip)
+            if icon_path.startswith(":/"):
+                icon = QtGui.QIcon(icon_path)
+            else:
+                icon = QtGui.QIcon(f":/icons/{cruiz.globals.get_theme()}/{icon_path}")
+            action.setIcon(icon)
+
+        _configure_non_conan_action(
+            recipe_ui.actionCancelCommand,
+            cancel,
+            "Cancel the currently running command",
+            ":/cancel.svg",
+        )
+
         if IS_CONAN_V1:
-            recipe_ui.actionCMakeBuildToolCommand.setShortcut(
-                QtGui.QKeySequence(cmake_build_tool)
-            )
-            recipe_ui.actionCMakeBuildToolCommand.setToolTip("CMake build")
-            recipe_ui.actionCMakeBuildToolVerboseCommand.setShortcut(
-                QtGui.QKeySequence(cmake_build_tool_verbose)
+            _configure_non_conan_action(
+                recipe_ui.actionCMakeBuildToolCommand,
+                cmake_build_tool,
+                "CMake build",
+                ":/cmakebuildtool.svg",
             )
-            recipe_ui.actionCMakeBuildToolVerboseCommand.setToolTip(
-                "CMake verbose build"
+
+            _configure_non_conan_action(
+                recipe_ui.actionCMakeBuildToolVerboseCommand,
+                cmake_build_tool_verbose,
+                "CMake verbose build",
+                ":/cmakebuildtoolverbose.svg",
             )
-            recipe_ui.actionCMakeRemoveCacheCommand.setShortcut(
-                QtGui.QKeySequence(remove_cmakecache)
+
+            _configure_non_conan_action(
+                recipe_ui.actionCMakeRemoveCacheCommand,
+                remove_cmakecache,
+                "Remove CMake cache",
+                ":/removecmakecache.svg",
             )
-            recipe_ui.actionCMakeRemoveCacheCommand.setToolTip("Remove CMake cache")
 
     def _command_started(self) -> None:
         self._idle_group.setEnabled(False)
         self._cancel_command_group.setEnabled(True)
 
     def _command_ended(self) -> None:
         self._idle_group.setEnabled(True)
@@ -423,17 +465,16 @@
                 imports_folder = settings.local_workflow_imports_folder.resolve()
                 params.imports_folder = recipe_widget.resolve_expression(imports_folder)
             if with_source_folder:
                 source_folder = settings.local_workflow_source_folder.resolve()
                 params.source_folder = recipe_widget.resolve_expression(source_folder)
             if fudge_source_folder:
                 source_folder = settings.local_workflow_source_folder.resolve()
-                if (
-                    source_folder is None
-                    and not recipe_widget.cwd_is_relative_to_recipe(workflow_cwd)
+                if not source_folder and not recipe_widget.cwd_is_relative_to_recipe(
+                    workflow_cwd
                 ):
                     # fudge due to the default source_folder changing between
                     # 'conan source' and 'conan build'
                     source_folder = "."
                 params.source_folder = recipe_widget.resolve_expression(source_folder)
             if with_build_folder:
                 build_folder = settings.local_workflow_build_folder.resolve()
```

### Comparing `cruiz-1.4.0a3/cruiz/remote_browser/pages/packagebinarypage.py` & `cruiz-1.4.0a4/cruiz/remote_browser/pages/packagebinarypage.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,20 +13,20 @@
 import tempfile
 import typing
 
 from qtpy import QtCore, QtGui, QtWidgets
 
 from qtpy import QtWebEngineCore
 
+import cruiz.globals
+
 from cruiz.interop.packagebinaryparameters import PackageBinaryParameters
 
 from cruiz.pyside6.remote_browser_fileview import Ui_remote_browser_fileview
 
-from cruiz.settings.managers.generalpreferences import GeneralSettingsReader
-
 from .page import Page
 
 
 class _FileNode:
     def __init__(self, path: str, parent: typing.Optional[_FileNode]):
         self.path = path
         self.parent = parent
@@ -180,15 +180,15 @@
                 )
         return None
 
     def flags(self, index):  # type: ignore
         default_flags = super().flags(index)
         node = index.internalPointer()
         if node.link_target:
-            return default_flags & ~QtCore.Qt.ItemIsEnabled  # type: ignore[operator]
+            return default_flags & ~QtCore.Qt.ItemIsEnabled
         return default_flags
 
 
 class _FileViewer(QtWidgets.QDialog):
     def __init__(
         self,
         root: pathlib.Path,
@@ -222,21 +222,19 @@
             html_path = archive.parent / path
             html_path = html_path.with_suffix(".html")
         else:
             with path.open("rt", encoding="utf-8") as data_file:
                 contents = data_file.readlines()
             html_path = pathlib.Path(path.with_suffix(".html"))
         html_path.parent.mkdir(parents=True, exist_ok=True)
-        with GeneralSettingsReader() as settings:
-            use_dark_mode = settings.use_dark_mode.resolve()
         with html_path.open("wt", encoding="utf-8") as html_file:
-            url_start = "https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.4.0"
+            url_start = "https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.8.0"
             html_file.write("<html>")
             html_file.write("<head>")
-            if use_dark_mode:
+            if cruiz.globals.is_dark_theme():
                 html_file.write(
                     f'<link rel="stylesheet" href="{url_start}/styles/dark.min.css">'
                 )
             else:
                 html_file.write(
                     f'<link rel="stylesheet" href="{url_start}/styles/default.min.css">'
                 )
```

### Comparing `cruiz-1.4.0a3/cruiz/remote_browser/pages/packageidpage.py` & `cruiz-1.4.0a4/cruiz/remote_browser/pages/packageidpage.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,17 +86,17 @@
 
     def columnCount(self, parent) -> int:  # type: ignore
         # pylint: disable=unused-argument
         if self._pids is None:
             return 0
         num_cols = 1  # the package id
         if self._settings:
-            num_cols += len(self._settings)  # type: ignore[arg-type]
+            num_cols += len(self._settings)
         if self._options:
-            num_cols += len(self._options)  # type: ignore[arg-type]
+            num_cols += len(self._options)
         if "requires" in self._pids[0]:
             num_cols += 1
         return num_cols
 
     def headerData(self, section, orientation, role):  # type: ignore
         if role == QtCore.Qt.DisplayRole and orientation == QtCore.Qt.Horizontal:
             num_settings = len(self._settings) if self._settings else 0
```

### Comparing `cruiz-1.4.0a3/cruiz/remote_browser/pages/packagereferencepage.py` & `cruiz-1.4.0a4/cruiz/remote_browser/pages/packagereferencepage.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         if role == QtCore.Qt.DisplayRole:
             return self._list[index.row()]
         return None
 
     def flags(self, index):  # type: ignore
         default_flags = super().flags(index)
         if "->" in self._list[index.row()]:
-            return default_flags & ~QtCore.Qt.ItemIsEnabled  # type: ignore[operator]
+            return default_flags & ~QtCore.Qt.ItemIsEnabled
         return default_flags
 
 
 class _PackageSearchValidator(QtGui.QValidator):
     """
     Validate the input given to the package search
     """
```

### Comparing `cruiz-1.4.0a3/cruiz/remote_browser/pages/packagerevisionpage.py` & `cruiz-1.4.0a4/cruiz/remote_browser/pages/packagerevisionpage.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/remote_browser/pages/page.py` & `cruiz-1.4.0a4/cruiz/remote_browser/pages/page.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/remote_browser/pages/reciperevisionpage.py` & `cruiz-1.4.0a4/cruiz/remote_browser/pages/reciperevisionpage.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/remote_browser/remotebrowser.py` & `cruiz-1.4.0a4/cruiz/remote_browser/remotebrowser.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/resourcegeneration.py` & `cruiz-1.4.0a4/cruiz/resourcegeneration.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 """
 
 import logging
 import os
 import pathlib
 import platform
 import subprocess
+import sys
 import typing
 
 SUBDIR = "pyside6"
 RCC = "pyside6-rcc"
 UIC = "pyside6-uic"
 
 
@@ -76,7 +77,10 @@
     if not resources_dir.exists():
         # resources directory does not exist in binary distributions, so early out
         logger.debug("Resource directory does not exist; compiled resources are fixed")
         return
     logger.debug("Checking for out-of-date resources...")
     _ensure_resource_file_is_up_to_date(current_dir / SUBDIR, resources_dir)
     _ensure_ui_files_are_up_to_date(current_dir / SUBDIR, resources_dir)
+    if "CRUIZ_GENERATE_RESOURCES_ONLY" in os.environ:
+        print("Completed resource generation...exiting")
+        sys.exit(0)
```

### Comparing `cruiz-1.4.0a3/cruiz/resources/001-rubbish.svg` & `cruiz-1.4.0a4/cruiz/resources/001-rubbish.svg`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/resources/002-null.svg` & `cruiz-1.4.0a4/cruiz/resources/002-null.svg`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/resources/003-chemistry.svg` & `cruiz-1.4.0a4/cruiz/resources/003-chemistry.svg`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/resources/004-share.svg` & `cruiz-1.4.0a4/cruiz/resources/004-share.svg`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/resources/005-box.svg` & `cruiz-1.4.0a4/cruiz/resources/005-box.svg`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/resources/006-toolbox.svg` & `cruiz-1.4.0a4/cruiz/resources/006-toolbox.svg`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/resources/007-book.svg` & `cruiz-1.4.0a4/cruiz/resources/007-book.svg`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/resources/008-cloud-computing.svg` & `cruiz-1.4.0a4/cruiz/resources/008-cloud-computing.svg`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/resources/009-import.svg` & `cruiz-1.4.0a4/cruiz/resources/009-import.svg`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/resources/010-draw.svg` & `cruiz-1.4.0a4/cruiz/resources/010-draw.svg`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/resources/012-hammer.svg` & `cruiz-1.4.0a4/cruiz/resources/012-hammer.svg`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/resources/013-pencil.svg` & `cruiz-1.4.0a4/cruiz/resources/013-pencil.svg`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/resources/014-code.svg` & `cruiz-1.4.0a4/cruiz/resources/014-code.svg`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/resources/Cmake.svg` & `cruiz-1.4.0a4/cruiz/resources/Cmake.svg`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/resources/about_dialog.ui` & `cruiz-1.4.0a4/cruiz/resources/about_dialog.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/resources/cruise.png` & `cruiz-1.4.0a4/cruiz/resources/cruise.png`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/resources/cruizres.qrc` & `cruiz-1.4.0a4/cruiz/resources/cruizres.qrc`

 * *Files 18% similar despite different names*

```diff
@@ -1,69 +1,111 @@
 00000000: 3c21 444f 4354 5950 4520 5243 433e 3c52  <!DOCTYPE RCC><R
 00000010: 4343 2076 6572 7369 6f6e 3d22 312e 3022  CC version="1.0"
-00000020: 3e0a 2020 3c71 7265 736f 7572 6365 3e0a  >.  <qresource>.
-00000030: 2020 2020 3c66 696c 6520 616c 6961 733d      <file alias=
-00000040: 2263 7265 6174 652e 7376 6722 3e30 3130  "create.svg">010
-00000050: 2d64 7261 772e 7376 673c 2f66 696c 653e  -draw.svg</file>
-00000060: 0a20 2020 203c 6669 6c65 2061 6c69 6173  .    <file alias
-00000070: 3d22 696d 706f 7274 732e 7376 6722 3e30  ="imports.svg">0
-00000080: 3039 2d69 6d70 6f72 742e 7376 673c 2f66  09-import.svg</f
-00000090: 696c 653e 0a20 2020 203c 6669 6c65 2061  ile>.    <file a
-000000a0: 6c69 6173 3d22 696e 7374 616c 6c2e 7376  lias="install.sv
-000000b0: 6722 3e30 3038 2d63 6c6f 7564 2d63 6f6d  g">008-cloud-com
-000000c0: 7075 7469 6e67 2e73 7667 3c2f 6669 6c65  puting.svg</file
-000000d0: 3e0a 2020 2020 3c66 696c 6520 616c 6961  >.    <file alia
-000000e0: 733d 2273 6f75 7263 652e 7376 6722 3e30  s="source.svg">0
-000000f0: 3037 2d62 6f6f 6b2e 7376 673c 2f66 696c  07-book.svg</fil
-00000100: 653e 0a20 2020 203c 6669 6c65 2061 6c69  e>.    <file ali
-00000110: 6173 3d22 6275 696c 642e 7376 6722 3e30  as="build.svg">0
-00000120: 3036 2d74 6f6f 6c62 6f78 2e73 7667 3c2f  06-toolbox.svg</
-00000130: 6669 6c65 3e0a 2020 2020 3c66 696c 6520  file>.    <file 
-00000140: 616c 6961 733d 2270 6163 6b61 6765 2e73  alias="package.s
-00000150: 7667 223e 3030 352d 626f 782e 7376 673c  vg">005-box.svg<
-00000160: 2f66 696c 653e 0a20 2020 203c 6669 6c65  /file>.    <file
-00000170: 2061 6c69 6173 3d22 6578 706f 7274 7061   alias="exportpa
-00000180: 636b 6167 652e 7376 6722 3e30 3034 2d73  ckage.svg">004-s
-00000190: 6861 7265 2e73 7667 3c2f 6669 6c65 3e0a  hare.svg</file>.
-000001a0: 2020 2020 3c66 696c 6520 616c 6961 733d      <file alias=
-000001b0: 2274 6573 7470 6163 6b61 6765 2e73 7667  "testpackage.svg
-000001c0: 223e 3030 332d 6368 656d 6973 7472 792e  ">003-chemistry.
-000001d0: 7376 673c 2f66 696c 653e 0a20 2020 203c  svg</file>.    <
-000001e0: 6669 6c65 2061 6c69 6173 3d22 6361 6e63  file alias="canc
-000001f0: 656c 2e73 7667 223e 3030 322d 6e75 6c6c  el.svg">002-null
-00000200: 2e73 7667 3c2f 6669 6c65 3e0a 2020 2020  .svg</file>.    
-00000210: 3c66 696c 6520 616c 6961 733d 2272 656d  <file alias="rem
-00000220: 6f76 6570 6163 6b61 6765 2e73 7667 223e  ovepackage.svg">
-00000230: 3030 312d 7275 6262 6973 682e 7376 673c  001-rubbish.svg<
-00000240: 2f66 696c 653e 0a20 2020 203c 6669 6c65  /file>.    <file
-00000250: 2061 6c69 6173 3d22 636d 616b 6562 7569   alias="cmakebui
-00000260: 6c64 746f 6f6c 2e73 7667 223e 436d 616b  ldtool.svg">Cmak
-00000270: 652e 7376 673c 2f66 696c 653e 0a20 2020  e.svg</file>.   
-00000280: 203c 6669 6c65 2061 6c69 6173 3d22 636d   <file alias="cm
-00000290: 616b 6562 7569 6c64 746f 6f6c 7665 7262  akebuildtoolverb
-000002a0: 6f73 652e 7376 6722 3e43 6d61 6b65 2e73  ose.svg">Cmake.s
-000002b0: 7667 3c2f 6669 6c65 3e0a 2020 2020 3c66  vg</file>.    <f
-000002c0: 696c 6520 616c 6961 733d 2272 656d 6f76  ile alias="remov
-000002d0: 6563 6d61 6b65 6361 6368 652e 7376 6722  ecmakecache.svg"
-000002e0: 3e43 6d61 6b65 2e73 7667 3c2f 6669 6c65  >Cmake.svg</file
-000002f0: 3e0a 2020 2020 3c66 696c 6520 616c 6961  >.    <file alia
-00000300: 733d 2263 7275 697a 2e70 6e67 223e 6372  s="cruiz.png">cr
-00000310: 7569 7365 2e70 6e67 3c2f 6669 6c65 3e0a  uise.png</file>.
-00000320: 2020 2020 3c66 696c 6520 616c 6961 733d      <file alias=
-00000330: 2262 7569 6c64 6162 6c65 2e73 7667 223e  "buildable.svg">
-00000340: 3031 322d 6861 6d6d 6572 2e73 7667 3c2f  012-hammer.svg</
-00000350: 6669 6c65 3e0a 2020 2020 3c66 696c 6520  file>.    <file 
-00000360: 616c 6961 733d 2262 696e 6172 6965 732e  alias="binaries.
-00000370: 7376 6722 3e30 3134 2d63 6f64 652e 7376  svg">014-code.sv
-00000380: 673c 2f66 696c 653e 0a20 2020 203c 6669  g</file>.    <fi
-00000390: 6c65 2061 6c69 6173 3d22 6564 6974 6162  le alias="editab
-000003a0: 6c65 2e73 7667 223e 3031 332d 7065 6e63  le.svg">013-penc
-000003b0: 696c 2e73 7667 3c2f 6669 6c65 3e0a 2020  il.svg</file>.  
-000003c0: 2020 3c66 696c 6520 616c 6961 733d 2269    <file alias="i
-000003d0: 636f 6e6c 6963 656e 7365 2e70 6466 223e  conlicense.pdf">
-000003e0: 6c69 6365 6e73 652e 7064 663c 2f66 696c  license.pdf</fil
-000003f0: 653e 0a20 2020 203c 6669 6c65 2061 6c69  e>.    <file ali
-00000400: 6173 3d22 6963 6f6e 6c69 6365 6e73 655f  as="iconlicense_
-00000410: 6372 7569 7365 2e70 6466 223e 6c69 6365  cruise.pdf">lice
-00000420: 6e73 652d 6372 7569 7365 2e70 6466 3c2f  nse-cruise.pdf</
-00000430: 6669 6c65 3e0a 2020 3c2f 7172 6573 6f75  file>.  </qresou
-00000440: 7263 653e 0a3c 2f52 4343 3e0a            rce>.</RCC>.
+00000020: 3e0a 2020 3c71 7265 736f 7572 6365 2070  >.  <qresource p
+00000030: 7265 6669 783d 222f 6963 6f6e 732f 4c69  refix="/icons/Li
+00000040: 6768 7422 3e0a 2020 2020 3c66 696c 6520  ght">.    <file 
+00000050: 616c 6961 733d 2263 7265 6174 652e 7376  alias="create.sv
+00000060: 6722 3e30 3130 2d64 7261 772e 7376 673c  g">010-draw.svg<
+00000070: 2f66 696c 653e 0a20 2020 203c 6669 6c65  /file>.    <file
+00000080: 2061 6c69 6173 3d22 696d 706f 7274 732e   alias="imports.
+00000090: 7376 6722 3e30 3039 2d69 6d70 6f72 742e  svg">009-import.
+000000a0: 7376 673c 2f66 696c 653e 0a20 2020 203c  svg</file>.    <
+000000b0: 6669 6c65 2061 6c69 6173 3d22 696e 7374  file alias="inst
+000000c0: 616c 6c2e 7376 6722 3e30 3038 2d63 6c6f  all.svg">008-clo
+000000d0: 7564 2d63 6f6d 7075 7469 6e67 2e73 7667  ud-computing.svg
+000000e0: 3c2f 6669 6c65 3e0a 2020 2020 3c66 696c  </file>.    <fil
+000000f0: 6520 616c 6961 733d 2273 6f75 7263 652e  e alias="source.
+00000100: 7376 6722 3e30 3037 2d62 6f6f 6b2e 7376  svg">007-book.sv
+00000110: 673c 2f66 696c 653e 0a20 2020 203c 6669  g</file>.    <fi
+00000120: 6c65 2061 6c69 6173 3d22 6275 696c 642e  le alias="build.
+00000130: 7376 6722 3e30 3036 2d74 6f6f 6c62 6f78  svg">006-toolbox
+00000140: 2e73 7667 3c2f 6669 6c65 3e0a 2020 2020  .svg</file>.    
+00000150: 3c66 696c 6520 616c 6961 733d 2270 6163  <file alias="pac
+00000160: 6b61 6765 2e73 7667 223e 3030 352d 626f  kage.svg">005-bo
+00000170: 782e 7376 673c 2f66 696c 653e 0a20 2020  x.svg</file>.   
+00000180: 203c 6669 6c65 2061 6c69 6173 3d22 6578   <file alias="ex
+00000190: 706f 7274 7061 636b 6167 652e 7376 6722  portpackage.svg"
+000001a0: 3e30 3034 2d73 6861 7265 2e73 7667 3c2f  >004-share.svg</
+000001b0: 6669 6c65 3e0a 2020 2020 3c66 696c 6520  file>.    <file 
+000001c0: 616c 6961 733d 2274 6573 7470 6163 6b61  alias="testpacka
+000001d0: 6765 2e73 7667 223e 3030 332d 6368 656d  ge.svg">003-chem
+000001e0: 6973 7472 792e 7376 673c 2f66 696c 653e  istry.svg</file>
+000001f0: 0a20 2020 203c 6669 6c65 2061 6c69 6173  .    <file alias
+00000200: 3d22 7265 6d6f 7665 7061 636b 6167 652e  ="removepackage.
+00000210: 7376 6722 3e30 3031 2d72 7562 6269 7368  svg">001-rubbish
+00000220: 2e73 7667 3c2f 6669 6c65 3e0a 2020 3c2f  .svg</file>.  </
+00000230: 7172 6573 6f75 7263 653e 0a20 203c 7172  qresource>.  <qr
+00000240: 6573 6f75 7263 6520 7072 6566 6978 3d22  esource prefix="
+00000250: 2f69 636f 6e73 2f44 6172 6b22 3e0a 2020  /icons/Dark">.  
+00000260: 2020 3c66 696c 6520 616c 6961 733d 2263    <file alias="c
+00000270: 7265 6174 652e 7376 6722 3e69 6e76 6572  reate.svg">inver
+00000280: 7465 642f 3031 302d 6472 6177 2e73 7667  ted/010-draw.svg
+00000290: 3c2f 6669 6c65 3e0a 2020 2020 3c66 696c  </file>.    <fil
+000002a0: 6520 616c 6961 733d 2269 6d70 6f72 7473  e alias="imports
+000002b0: 2e73 7667 223e 696e 7665 7274 6564 2f30  .svg">inverted/0
+000002c0: 3039 2d69 6d70 6f72 742e 7376 673c 2f66  09-import.svg</f
+000002d0: 696c 653e 0a20 2020 203c 6669 6c65 2061  ile>.    <file a
+000002e0: 6c69 6173 3d22 696e 7374 616c 6c2e 7376  lias="install.sv
+000002f0: 6722 3e69 6e76 6572 7465 642f 3030 382d  g">inverted/008-
+00000300: 636c 6f75 642d 636f 6d70 7574 696e 672e  cloud-computing.
+00000310: 7376 673c 2f66 696c 653e 0a20 2020 203c  svg</file>.    <
+00000320: 6669 6c65 2061 6c69 6173 3d22 736f 7572  file alias="sour
+00000330: 6365 2e73 7667 223e 696e 7665 7274 6564  ce.svg">inverted
+00000340: 2f30 3037 2d62 6f6f 6b2e 7376 673c 2f66  /007-book.svg</f
+00000350: 696c 653e 0a20 2020 203c 6669 6c65 2061  ile>.    <file a
+00000360: 6c69 6173 3d22 6275 696c 642e 7376 6722  lias="build.svg"
+00000370: 3e69 6e76 6572 7465 642f 3030 362d 746f  >inverted/006-to
+00000380: 6f6c 626f 782e 7376 673c 2f66 696c 653e  olbox.svg</file>
+00000390: 0a20 2020 203c 6669 6c65 2061 6c69 6173  .    <file alias
+000003a0: 3d22 7061 636b 6167 652e 7376 6722 3e69  ="package.svg">i
+000003b0: 6e76 6572 7465 642f 3030 352d 626f 782e  nverted/005-box.
+000003c0: 7376 673c 2f66 696c 653e 0a20 2020 203c  svg</file>.    <
+000003d0: 6669 6c65 2061 6c69 6173 3d22 6578 706f  file alias="expo
+000003e0: 7274 7061 636b 6167 652e 7376 6722 3e69  rtpackage.svg">i
+000003f0: 6e76 6572 7465 642f 3030 342d 7368 6172  nverted/004-shar
+00000400: 652e 7376 673c 2f66 696c 653e 0a20 2020  e.svg</file>.   
+00000410: 203c 6669 6c65 2061 6c69 6173 3d22 7465   <file alias="te
+00000420: 7374 7061 636b 6167 652e 7376 6722 3e69  stpackage.svg">i
+00000430: 6e76 6572 7465 642f 3030 332d 6368 656d  nverted/003-chem
+00000440: 6973 7472 792e 7376 673c 2f66 696c 653e  istry.svg</file>
+00000450: 0a20 2020 203c 6669 6c65 2061 6c69 6173  .    <file alias
+00000460: 3d22 7265 6d6f 7665 7061 636b 6167 652e  ="removepackage.
+00000470: 7376 6722 3e69 6e76 6572 7465 642f 3030  svg">inverted/00
+00000480: 312d 7275 6262 6973 682e 7376 673c 2f66  1-rubbish.svg</f
+00000490: 696c 653e 0a20 203c 2f71 7265 736f 7572  ile>.  </qresour
+000004a0: 6365 3e0a 2020 3c71 7265 736f 7572 6365  ce>.  <qresource
+000004b0: 3e0a 2020 2020 3c66 696c 6520 616c 6961  >.    <file alia
+000004c0: 733d 2263 6d61 6b65 6275 696c 6474 6f6f  s="cmakebuildtoo
+000004d0: 6c2e 7376 6722 3e43 6d61 6b65 2e73 7667  l.svg">Cmake.svg
+000004e0: 3c2f 6669 6c65 3e0a 2020 2020 3c66 696c  </file>.    <fil
+000004f0: 6520 616c 6961 733d 2263 6d61 6b65 6275  e alias="cmakebu
+00000500: 696c 6474 6f6f 6c76 6572 626f 7365 2e73  ildtoolverbose.s
+00000510: 7667 223e 436d 616b 652e 7376 673c 2f66  vg">Cmake.svg</f
+00000520: 696c 653e 0a20 2020 203c 6669 6c65 2061  ile>.    <file a
+00000530: 6c69 6173 3d22 7265 6d6f 7665 636d 616b  lias="removecmak
+00000540: 6563 6163 6865 2e73 7667 223e 436d 616b  ecache.svg">Cmak
+00000550: 652e 7376 673c 2f66 696c 653e 0a20 2020  e.svg</file>.   
+00000560: 203c 6669 6c65 2061 6c69 6173 3d22 6361   <file alias="ca
+00000570: 6e63 656c 2e73 7667 223e 3030 322d 6e75  ncel.svg">002-nu
+00000580: 6c6c 2e73 7667 3c2f 6669 6c65 3e0a 2020  ll.svg</file>.  
+00000590: 2020 3c66 696c 6520 616c 6961 733d 2263    <file alias="c
+000005a0: 7275 697a 2e70 6e67 223e 6372 7569 7365  ruiz.png">cruise
+000005b0: 2e70 6e67 3c2f 6669 6c65 3e0a 2020 2020  .png</file>.    
+000005c0: 3c66 696c 6520 616c 6961 733d 2262 7569  <file alias="bui
+000005d0: 6c64 6162 6c65 2e73 7667 223e 3031 322d  ldable.svg">012-
+000005e0: 6861 6d6d 6572 2e73 7667 3c2f 6669 6c65  hammer.svg</file
+000005f0: 3e0a 2020 2020 3c66 696c 6520 616c 6961  >.    <file alia
+00000600: 733d 2262 696e 6172 6965 732e 7376 6722  s="binaries.svg"
+00000610: 3e30 3134 2d63 6f64 652e 7376 673c 2f66  >014-code.svg</f
+00000620: 696c 653e 0a20 2020 203c 6669 6c65 2061  ile>.    <file a
+00000630: 6c69 6173 3d22 6564 6974 6162 6c65 2e73  lias="editable.s
+00000640: 7667 223e 3031 332d 7065 6e63 696c 2e73  vg">013-pencil.s
+00000650: 7667 3c2f 6669 6c65 3e0a 2020 2020 3c66  vg</file>.    <f
+00000660: 696c 6520 616c 6961 733d 2269 636f 6e6c  ile alias="iconl
+00000670: 6963 656e 7365 2e70 6466 223e 6c69 6365  icense.pdf">lice
+00000680: 6e73 652e 7064 663c 2f66 696c 653e 0a20  nse.pdf</file>. 
+00000690: 2020 203c 6669 6c65 2061 6c69 6173 3d22     <file alias="
+000006a0: 6963 6f6e 6c69 6365 6e73 655f 6372 7569  iconlicense_crui
+000006b0: 7365 2e70 6466 223e 6c69 6365 6e73 652d  se.pdf">license-
+000006c0: 6372 7569 7365 2e70 6466 3c2f 6669 6c65  cruise.pdf</file
+000006d0: 3e0a 2020 3c2f 7172 6573 6f75 7263 653e  >.  </qresource>
+000006e0: 0a3c 2f52 4343 3e0a                      .</RCC>.
```

### Comparing `cruiz-1.4.0a3/cruiz/resources/find_text_dialog.ui` & `cruiz-1.4.0a4/cruiz/resources/find_text_dialog.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/resources/license-cruise.pdf` & `cruiz-1.4.0a4/cruiz/resources/license-cruise.pdf`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/resources/license.pdf` & `cruiz-1.4.0a4/cruiz/resources/license.pdf`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/resources/load_recipe_wizard.ui` & `cruiz-1.4.0a4/cruiz/resources/load_recipe_wizard.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/resources/local_cache_add_environment.ui` & `cruiz-1.4.0a4/cruiz/resources/local_cache_add_environment.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/resources/local_cache_add_profile_directory.ui` & `cruiz-1.4.0a4/cruiz/resources/local_cache_add_profile_directory.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/resources/local_cache_add_remote.ui` & `cruiz-1.4.0a4/cruiz/resources/local_cache_add_remote.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/resources/local_cache_install_config.ui` & `cruiz-1.4.0a4/cruiz/resources/local_cache_install_config.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/resources/local_cache_manage.ui` & `cruiz-1.4.0a4/cruiz/resources/local_cache_manage.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/resources/local_cache_move.ui` & `cruiz-1.4.0a4/cruiz/resources/local_cache_move.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/resources/local_cache_new_wizard.ui` & `cruiz-1.4.0a4/cruiz/resources/local_cache_new_wizard.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/resources/local_cache_remove_environment.ui` & `cruiz-1.4.0a4/cruiz/resources/local_cache_remove_environment.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/resources/local_cache_run_command_dialog.ui` & `cruiz-1.4.0a4/cruiz/resources/local_cache_run_command_dialog.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/resources/preferences.ui` & `cruiz-1.4.0a4/cruiz/resources/remote_browser.ui`

 * *Files 26% similar despite different names*

#### Comparing `cruiz-1.4.0a3/cruiz/resources/preferences.ui` & `cruiz-1.4.0a4/cruiz/resources/remote_browser.ui`

```diff
@@ -1,1161 +1,878 @@
 <?xml version="1.0" encoding="utf-8"?>
 <ui version="4.0">
-  <class>PreferencesDialog</class>
-  <widget class="QDialog" name="PreferencesDialog">
+  <class>remotebrowser</class>
+  <widget class="QDockWidget" name="remotebrowser">
+    <property name="enabled">
+      <bool>true</bool>
+    </property>
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
-        <width>678</width>
-        <height>670</height>
+        <width>493</width>
+        <height>682</height>
       </rect>
     </property>
+    <property name="features">
+      <set>QDockWidget::DockWidgetClosable|QDockWidget::DockWidgetFloatable|QDockWidget::DockWidgetMovable</set>
+    </property>
     <property name="windowTitle">
-      <string>Preferences</string>
+      <string>Conan remote browser</string>
     </property>
-    <layout class="QVBoxLayout" name="verticalLayout">
-      <item>
-        <widget class="QToolBox" name="prefs_toolbox">
-          <property name="currentIndex">
-            <number>0</number>
-          </property>
-          <widget class="QWidget" name="prefs_general">
-            <property name="geometry">
-              <rect>
-                <x>0</x>
-                <y>0</y>
-                <width>639</width>
-                <height>275</height>
-              </rect>
-            </property>
-            <attribute name="label">
-              <string>General</string>
-            </attribute>
-            <layout class="QGridLayout" name="gridLayout">
-              <item row="7" column="2">
-                <widget class="QPushButton" name="prefs_general_busy_colour">
-                  <property name="text">
-                    <string/>
-                  </property>
-                </widget>
-              </item>
-              <item row="8" column="2">
-                <widget class="QPushButton" name="prefs_general_found_text_background_colour">
-                  <property name="text">
-                    <string/>
-                  </property>
-                </widget>
-              </item>
-              <item row="2" column="2">
-                <widget class="QCheckBox" name="prefs_general_usebatching">
-                  <property name="text">
-                    <string>Use batching for standard output</string>
-                  </property>
-                </widget>
-              </item>
-              <item row="6" column="2">
-                <widget class="QLineEdit" name="prefs_general_default_recipe_dir"/>
-              </item>
-              <item row="3" column="2">
-                <widget class="QCheckBox" name="prefs_general_enable_wallclock">
-                  <property name="text">
-                    <string>Enable wall clock command timing</string>
-                  </property>
-                </widget>
-              </item>
-              <item row="5" column="2">
-                <widget class="QCheckBox" name="prefs_general_enable_compact">
-                  <property name="visible">
-                    <bool>false</bool>
-                  </property>
-                  <property name="text">
-                    <string>Enable compact look</string>
-                  </property>
-                </widget>
-              </item>
-              <item row="0" column="2">
-                <widget class="QCheckBox" name="prefs_general_clearpanes">
-                  <property name="text">
-                    <string>Clear panes before running each command</string>
-                  </property>
-                </widget>
-              </item>
-              <item row="16" column="2">
-                <spacer name="verticalSpacer">
-                  <property name="orientation">
-                    <enum>Qt::Vertical</enum>
-                  </property>
-                  <property name="sizeHint" stdset="0">
-                    <size>
-                      <width>20</width>
-                      <height>40</height>
-                    </size>
-                  </property>
-                </spacer>
-              </item>
-              <item row="9" column="2">
-                <widget class="QCheckBox" name="prefs_general_new_recipe_load">
-                  <property name="visible">
-                    <bool>false</bool>
-                  </property>
-                  <property name="toolTip">
-                    <string>Enable new recipe loading behaviour.
-May help loading recipes that query version information during requirements() methods.
-However, help stop loading recipes if they have mixed versions of dependent packages in their dependency graph or mixed case names of dependent packages on case insensitive file systems.</string>
-                  </property>
-                  <property name="text">
-                    <string>New recipe loading behaviour</string>
-                  </property>
-                </widget>
-              </item>
-              <item row="7" column="0">
-                <widget class="QLabel" name="label_2">
-                  <property name="text">
-                    <string>Busy icon colour</string>
-                  </property>
-                </widget>
-              </item>
-              <item row="6" column="0">
-                <widget class="QLabel" name="label">
-                  <property name="text">
-                    <string>Default recipe browsing directory</string>
-                  </property>
-                </widget>
-              </item>
-              <item row="1" column="2">
-                <widget class="QCheckBox" name="prefs_general_combine_panes">
-                  <property name="text">
-                    <string>Combine output and error panes</string>
-                  </property>
-                </widget>
-              </item>
-              <item row="16" column="0">
-                <spacer name="verticalSpacer_3">
-                  <property name="orientation">
-                    <enum>Qt::Vertical</enum>
-                  </property>
-                  <property name="sizeHint" stdset="0">
-                    <size>
-                      <width>20</width>
-                      <height>40</height>
-                    </size>
-                  </property>
-                </spacer>
-              </item>
-              <item row="8" column="0">
-                <widget class="QLabel" name="label_30">
-                  <property name="text">
-                    <string>Found text background colour</string>
-                  </property>
-                </widget>
-              </item>
-              <item row="4" column="2">
-                <widget class="QCheckBox" name="prefs_general_enable_darkmode">
-                  <property name="toolTip">
-                    <string>Dark mode toggles immediately,  but existing Conan output will not change</string>
-                  </property>
-                  <property name="text">
-                    <string>Enable dark mode</string>
-                  </property>
-                </widget>
-              </item>
-              <item row="15" column="2">
-                <widget class="QLineEdit" name="prefs_general_recipe_editor"/>
-              </item>
-              <item row="15" column="0">
-                <widget class="QLabel" name="label_31">
-                  <property name="text">
-                    <string>Recipe editor</string>
-                  </property>
-                </widget>
-              </item>
-            </layout>
-          </widget>
-          <widget class="QWidget" name="prefs_fonts">
-            <property name="geometry">
-              <rect>
-                <x>0</x>
-                <y>0</y>
-                <width>639</width>
-                <height>233</height>
-              </rect>
-            </property>
-            <attribute name="label">
-              <string>Fonts</string>
-            </attribute>
-            <layout class="QVBoxLayout" name="verticalLayout_2">
-              <item>
-                <widget class="QGroupBox" name="groupBox">
-                  <property name="title">
-                    <string>UI font</string>
-                  </property>
-                  <layout class="QGridLayout" name="gridLayout_2">
-                    <item row="0" column="0">
-                      <widget class="QLabel" name="prefs_font_ui_label">
-                        <property name="sizePolicy">
-                          <sizepolicy hsizetype="Preferred" vsizetype="Preferred">
-                            <horstretch>1</horstretch>
-                            <verstretch>0</verstretch>
-                          </sizepolicy>
-                        </property>
-                        <property name="text">
-                          <string>The font</string>
-                        </property>
-                      </widget>
-                    </item>
-                    <item row="1" column="0">
-                      <widget class="QLabel" name="prefs_font_ui_preview">
-                        <property name="sizePolicy">
-                          <sizepolicy hsizetype="Preferred" vsizetype="Preferred">
-                            <horstretch>1</horstretch>
-                            <verstretch>0</verstretch>
-                          </sizepolicy>
+    <widget class="QWidget" name="dockWidgetContents">
+      <layout class="QVBoxLayout" name="verticalLayout">
+        <property name="leftMargin">
+          <number>0</number>
+        </property>
+        <property name="topMargin">
+          <number>0</number>
+        </property>
+        <property name="rightMargin">
+          <number>0</number>
+        </property>
+        <property name="bottomMargin">
+          <number>0</number>
+        </property>
+        <item>
+          <widget class="QStackedWidget" name="stackedWidget">
+            <property name="currentIndex">
+              <number>0</number>
+            </property>
+            <widget class="PackageReferencePage" name="pkgref">
+              <layout class="QVBoxLayout" name="verticalLayout_2">
+                <item>
+                  <widget class="QGroupBox" name="pkgref_ui_group">
+                    <property name="title">
+                      <string>Query package reference</string>
+                    </property>
+                    <layout class="QGridLayout" name="gridLayout">
+                      <item row="0" column="0">
+                        <widget class="QLabel" name="label">
+                          <property name="text">
+                            <string>Local cache name</string>
+                          </property>
+                        </widget>
+                      </item>
+                      <item row="2" column="1">
+                        <widget class="QComboBox" name="remote"/>
+                      </item>
+                      <item row="0" column="1">
+                        <widget class="QComboBox" name="local_cache_name"/>
+                      </item>
+                      <item row="4" column="1">
+                        <widget class="QLineEdit" name="search_pattern"/>
+                      </item>
+                      <item row="2" column="0">
+                        <widget class="QLabel" name="label_2">
+                          <property name="text">
+                            <string>Remote</string>
+                          </property>
+                        </widget>
+                      </item>
+                      <item row="4" column="0">
+                        <widget class="QLabel" name="label_3">
+                          <property name="text">
+                            <string>Search pattern</string>
+                          </property>
+                        </widget>
+                      </item>
+                      <item row="1" column="0" colspan="2">
+                        <widget class="QCheckBox" name="revisions">
+                          <property name="enabled">
+                            <bool>false</bool>
+                          </property>
+                          <property name="text">
+                            <string>Revisions enabled</string>
+                          </property>
+                        </widget>
+                      </item>
+                      <item row="3" column="0" colspan="2">
+                        <widget class="QCheckBox" name="alias_aware">
+                          <property name="toolTip">
+                            <string>Check this option to perform additional processing to identify alias packages</string>
+                          </property>
+                          <property name="text">
+                            <string>Alias aware</string>
+                          </property>
+                        </widget>
+                      </item>
+                    </layout>
+                  </widget>
+                </item>
+                <item>
+                  <widget class="QGroupBox" name="pkgref_groupbox">
+                    <property name="enabled">
+                      <bool>false</bool>
+                    </property>
+                    <property name="sizePolicy">
+                      <sizepolicy hsizetype="Preferred" vsizetype="Preferred">
+                        <horstretch>0</horstretch>
+                        <verstretch>0</verstretch>
+                      </sizepolicy>
+                    </property>
+                    <property name="title">
+                      <string>0 package references found</string>
+                    </property>
+                    <layout class="QVBoxLayout" name="verticalLayout_7">
+                      <property name="leftMargin">
+                        <number>0</number>
+                      </property>
+                      <property name="topMargin">
+                        <number>0</number>
+                      </property>
+                      <property name="rightMargin">
+                        <number>0</number>
+                      </property>
+                      <property name="bottomMargin">
+                        <number>0</number>
+                      </property>
+                      <item>
+                        <widget class="QListView" name="package_references">
+                          <property name="sizePolicy">
+                            <sizepolicy hsizetype="Expanding" vsizetype="Expanding">
+                              <horstretch>0</horstretch>
+                              <verstretch>0</verstretch>
+                            </sizepolicy>
+                          </property>
+                          <property name="contextMenuPolicy">
+                            <enum>Qt::CustomContextMenu</enum>
+                          </property>
+                          <property name="sizeAdjustPolicy">
+                            <enum>QAbstractScrollArea::AdjustToContents</enum>
+                          </property>
+                          <property name="editTriggers">
+                            <set>QAbstractItemView::NoEditTriggers</set>
+                          </property>
+                          <property name="alternatingRowColors">
+                            <bool>true</bool>
+                          </property>
+                        </widget>
+                      </item>
+                    </layout>
+                  </widget>
+                </item>
+                <item>
+                  <layout class="QHBoxLayout" name="horizontalLayout_5">
+                    <item>
+                      <widget class="QProgressBar" name="pkgref_progress">
+                        <property name="maximum">
+                          <number>1</number>
                         </property>
-                        <property name="text">
-                          <string>The quick brown fox jumps over the lazy dog</string>
+                        <property name="value">
+                          <number>-1</number>
                         </property>
                       </widget>
                     </item>
-                    <item row="1" column="1">
-                      <widget class="QPushButton" name="prefs_font_ui_reset">
-                        <property name="text">
-                          <string>Reset</string>
+                    <item>
+                      <widget class="QPushButton" name="pkgref_cancel">
+                        <property name="enabled">
+                          <bool>false</bool>
                         </property>
-                      </widget>
-                    </item>
-                    <item row="0" column="1">
-                      <widget class="QPushButton" name="prefs_font_ui_change">
                         <property name="text">
-                          <string>Change ...</string>
+                          <string/>
+                        </property>
+                        <property name="icon">
+                          <iconset>
+                            <normaloff>:/cancel.svg</normaloff>
+                            :/cancel.svg
+                          </iconset>
                         </property>
                       </widget>
                     </item>
                   </layout>
-                </widget>
-              </item>
-              <item>
-                <widget class="QGroupBox" name="groupBox_2">
-                  <property name="title">
-                    <string>Output panes font</string>
-                  </property>
-                  <layout class="QGridLayout" name="gridLayout_3">
-                    <item row="0" column="0">
-                      <widget class="QLabel" name="prefs_font_output_label">
-                        <property name="sizePolicy">
-                          <sizepolicy hsizetype="Preferred" vsizetype="Preferred">
-                            <horstretch>1</horstretch>
-                            <verstretch>0</verstretch>
-                          </sizepolicy>
+                </item>
+              </layout>
+            </widget>
+            <widget class="RecipeRevisionPage" name="rrev">
+              <layout class="QVBoxLayout" name="verticalLayout_3">
+                <item>
+                  <widget class="QLabel" name="rrev_pkgref">
+                    <property name="contextMenuPolicy">
+                      <enum>Qt::CustomContextMenu</enum>
+                    </property>
+                    <property name="text">
+                      <string>Package reference</string>
+                    </property>
+                  </widget>
+                </item>
+                <item>
+                  <widget class="QGroupBox" name="rrev_groupbox">
+                    <property name="enabled">
+                      <bool>false</bool>
+                    </property>
+                    <property name="title">
+                      <string>0 recipe revisions found</string>
+                    </property>
+                    <layout class="QVBoxLayout" name="verticalLayout_8">
+                      <property name="leftMargin">
+                        <number>0</number>
+                      </property>
+                      <property name="topMargin">
+                        <number>0</number>
+                      </property>
+                      <property name="rightMargin">
+                        <number>0</number>
+                      </property>
+                      <property name="bottomMargin">
+                        <number>0</number>
+                      </property>
+                      <item>
+                        <widget class="QTableView" name="recipe_revisions">
+                          <property name="contextMenuPolicy">
+                            <enum>Qt::CustomContextMenu</enum>
+                          </property>
+                          <property name="sizeAdjustPolicy">
+                            <enum>QAbstractScrollArea::AdjustToContents</enum>
+                          </property>
+                          <property name="editTriggers">
+                            <set>QAbstractItemView::NoEditTriggers</set>
+                          </property>
+                          <property name="alternatingRowColors">
+                            <bool>true</bool>
+                          </property>
+                          <property name="selectionMode">
+                            <enum>QAbstractItemView::SingleSelection</enum>
+                          </property>
+                          <property name="selectionBehavior">
+                            <enum>QAbstractItemView::SelectRows</enum>
+                          </property>
+                          <attribute name="horizontalHeaderStretchLastSection">
+                            <bool>false</bool>
+                          </attribute>
+                          <attribute name="verticalHeaderVisible">
+                            <bool>false</bool>
+                          </attribute>
+                        </widget>
+                      </item>
+                    </layout>
+                  </widget>
+                </item>
+                <item>
+                  <layout class="QHBoxLayout" name="horizontalLayout_6">
+                    <item>
+                      <widget class="QProgressBar" name="rrev_progress">
+                        <property name="maximum">
+                          <number>1</number>
                         </property>
-                        <property name="text">
-                          <string>The font</string>
+                        <property name="value">
+                          <number>-1</number>
                         </property>
                       </widget>
                     </item>
-                    <item row="1" column="0">
-                      <widget class="QLabel" name="prefs_font_output_preview">
-                        <property name="sizePolicy">
-                          <sizepolicy hsizetype="Preferred" vsizetype="Preferred">
-                            <horstretch>1</horstretch>
-                            <verstretch>0</verstretch>
-                          </sizepolicy>
+                    <item>
+                      <widget class="QPushButton" name="rrev_cancel">
+                        <property name="enabled">
+                          <bool>false</bool>
                         </property>
                         <property name="text">
-                          <string>The quick brown fox jumps over the lazy dog</string>
+                          <string/>
+                        </property>
+                        <property name="icon">
+                          <iconset>
+                            <normaloff>:/cancel.svg</normaloff>
+                            :/cancel.svg
+                          </iconset>
                         </property>
                       </widget>
                     </item>
-                    <item row="1" column="1">
-                      <widget class="QPushButton" name="prefs_font_output_reset">
-                        <property name="text">
-                          <string>Reset</string>
+                  </layout>
+                </item>
+                <item>
+                  <widget class="QWidget" name="rrev_buttons" native="true">
+                    <layout class="QHBoxLayout" name="horizontalLayout">
+                      <item>
+                        <widget class="QPushButton" name="rrev_back">
+                          <property name="text">
+                            <string>Back</string>
+                          </property>
+                        </widget>
+                      </item>
+                      <item>
+                        <spacer name="horizontalSpacer_5">
+                          <property name="orientation">
+                            <enum>Qt::Horizontal</enum>
+                          </property>
+                          <property name="sizeHint" stdset="0">
+                            <size>
+                              <width>40</width>
+                              <height>20</height>
+                            </size>
+                          </property>
+                        </spacer>
+                      </item>
+                      <item>
+                        <widget class="QPushButton" name="rrev_refresh">
+                          <property name="text">
+                            <string>Refresh</string>
+                          </property>
+                        </widget>
+                      </item>
+                    </layout>
+                  </widget>
+                </item>
+              </layout>
+            </widget>
+            <widget class="PackageIdPage" name="package_id">
+              <layout class="QVBoxLayout" name="verticalLayout_4">
+                <item>
+                  <widget class="QLabel" name="pid_pkgref">
+                    <property name="contextMenuPolicy">
+                      <enum>Qt::CustomContextMenu</enum>
+                    </property>
+                    <property name="text">
+                      <string>Package ref + revision</string>
+                    </property>
+                  </widget>
+                </item>
+                <item>
+                  <widget class="QGroupBox" name="pid_groupbox">
+                    <property name="enabled">
+                      <bool>false</bool>
+                    </property>
+                    <property name="title">
+                      <string>0 package_ids found</string>
+                    </property>
+                    <layout class="QVBoxLayout" name="verticalLayout_9">
+                      <property name="leftMargin">
+                        <number>0</number>
+                      </property>
+                      <property name="topMargin">
+                        <number>0</number>
+                      </property>
+                      <property name="rightMargin">
+                        <number>0</number>
+                      </property>
+                      <property name="bottomMargin">
+                        <number>0</number>
+                      </property>
+                      <item>
+                        <widget class="QTableView" name="package_ids">
+                          <property name="contextMenuPolicy">
+                            <enum>Qt::CustomContextMenu</enum>
+                          </property>
+                          <property name="sizeAdjustPolicy">
+                            <enum>QAbstractScrollArea::AdjustToContents</enum>
+                          </property>
+                          <property name="editTriggers">
+                            <set>QAbstractItemView::NoEditTriggers</set>
+                          </property>
+                          <property name="alternatingRowColors">
+                            <bool>true</bool>
+                          </property>
+                          <property name="selectionMode">
+                            <enum>QAbstractItemView::SingleSelection</enum>
+                          </property>
+                          <property name="selectionBehavior">
+                            <enum>QAbstractItemView::SelectRows</enum>
+                          </property>
+                          <property name="sortingEnabled">
+                            <bool>true</bool>
+                          </property>
+                          <attribute name="horizontalHeaderStretchLastSection">
+                            <bool>false</bool>
+                          </attribute>
+                          <attribute name="verticalHeaderVisible">
+                            <bool>false</bool>
+                          </attribute>
+                        </widget>
+                      </item>
+                    </layout>
+                  </widget>
+                </item>
+                <item>
+                  <widget class="QGroupBox" name="pid_filter_group">
+                    <property name="enabled">
+                      <bool>false</bool>
+                    </property>
+                    <property name="title">
+                      <string>Filtering</string>
+                    </property>
+                    <layout class="QVBoxLayout" name="verticalLayout_12">
+                      <property name="spacing">
+                        <number>6</number>
+                      </property>
+                      <property name="leftMargin">
+                        <number>0</number>
+                      </property>
+                      <property name="topMargin">
+                        <number>0</number>
+                      </property>
+                      <property name="rightMargin">
+                        <number>0</number>
+                      </property>
+                      <property name="bottomMargin">
+                        <number>0</number>
+                      </property>
+                      <item>
+                        <widget class="QTableView" name="pid_filterTable">
+                          <property name="contextMenuPolicy">
+                            <enum>Qt::CustomContextMenu</enum>
+                          </property>
+                          <property name="sizeAdjustPolicy">
+                            <enum>QAbstractScrollArea::AdjustToContents</enum>
+                          </property>
+                          <property name="editTriggers">
+                            <set>QAbstractItemView::NoEditTriggers</set>
+                          </property>
+                          <property name="alternatingRowColors">
+                            <bool>true</bool>
+                          </property>
+                          <property name="selectionMode">
+                            <enum>QAbstractItemView::SingleSelection</enum>
+                          </property>
+                          <property name="selectionBehavior">
+                            <enum>QAbstractItemView::SelectRows</enum>
+                          </property>
+                          <attribute name="horizontalHeaderStretchLastSection">
+                            <bool>false</bool>
+                          </attribute>
+                          <attribute name="verticalHeaderVisible">
+                            <bool>false</bool>
+                          </attribute>
+                        </widget>
+                      </item>
+                      <item>
+                        <layout class="QHBoxLayout" name="horizontalLayout_7">
+                          <item>
+                            <widget class="QComboBox" name="pid_filter_key">
+                              <property name="placeholderText">
+                                <string>Select filter key</string>
+                              </property>
+                            </widget>
+                          </item>
+                          <item>
+                            <widget class="QComboBox" name="pid_filter_value">
+                              <property name="placeholderText">
+                                <string>Select filter value</string>
+                              </property>
+                            </widget>
+                          </item>
+                          <item>
+                            <widget class="QPushButton" name="pid_add_filter">
+                              <property name="text">
+                                <string>Add</string>
+                              </property>
+                            </widget>
+                          </item>
+                        </layout>
+                      </item>
+                    </layout>
+                  </widget>
+                </item>
+                <item>
+                  <layout class="QHBoxLayout" name="horizontalLayout_8">
+                    <item>
+                      <widget class="QProgressBar" name="pid_progress">
+                        <property name="maximum">
+                          <number>1</number>
                         </property>
-                      </widget>
-                    </item>
-                    <item row="0" column="1">
-                      <widget class="QPushButton" name="prefs_font_output_change">
-                        <property name="text">
-                          <string>Change ...</string>
+                        <property name="value">
+                          <number>-1</number>
                         </property>
                       </widget>
                     </item>
-                  </layout>
-                </widget>
-              </item>
-              <item>
-                <spacer name="verticalSpacer_2">
-                  <property name="orientation">
-                    <enum>Qt::Vertical</enum>
-                  </property>
-                  <property name="sizeHint" stdset="0">
-                    <size>
-                      <width>20</width>
-                      <height>40</height>
-                    </size>
-                  </property>
-                </spacer>
-              </item>
-            </layout>
-          </widget>
-          <widget class="QWidget" name="prefs_conan">
-            <property name="geometry">
-              <rect>
-                <x>0</x>
-                <y>0</y>
-                <width>654</width>
-                <height>232</height>
-              </rect>
-            </property>
-            <attribute name="label">
-              <string>Conan</string>
-            </attribute>
-            <layout class="QVBoxLayout" name="verticalLayout_3">
-              <item>
-                <widget class="QGroupBox" name="groupBox_3">
-                  <property name="title">
-                    <string>Logging</string>
-                  </property>
-                  <layout class="QGridLayout" name="gridLayout_4">
-                    <item row="0" column="0">
-                      <widget class="QLabel" name="label_7">
-                        <property name="sizePolicy">
-                          <sizepolicy hsizetype="Preferred" vsizetype="Preferred">
-                            <horstretch>0</horstretch>
-                            <verstretch>0</verstretch>
-                          </sizepolicy>
+                    <item>
+                      <widget class="QPushButton" name="pid_cancel">
+                        <property name="enabled">
+                          <bool>false</bool>
                         </property>
                         <property name="text">
-                          <string>Conan logging level</string>
+                          <string/>
+                        </property>
+                        <property name="icon">
+                          <iconset>
+                            <normaloff>:/cancel.svg</normaloff>
+                            :/cancel.svg
+                          </iconset>
                         </property>
                       </widget>
                     </item>
-                    <item row="0" column="1">
-                      <widget class="QComboBox" name="prefs_conan_log_level">
-                        <property name="toolTip">
-                          <string>Log Conan commands. Only works when a single recipe has commands run on it</string>
-                        </property>
-                        <item>
+                  </layout>
+                </item>
+                <item>
+                  <widget class="QWidget" name="pid_buttons" native="true">
+                    <layout class="QHBoxLayout" name="horizontalLayout_2">
+                      <item>
+                        <widget class="QPushButton" name="pid_back">
                           <property name="text">
-                            <string>CRITICAL</string>
+                            <string>Back</string>
                           </property>
-                        </item>
-                        <item>
-                          <property name="text">
-                            <string>ERROR</string>
+                        </widget>
+                      </item>
+                      <item>
+                        <spacer name="horizontalSpacer_2">
+                          <property name="orientation">
+                            <enum>Qt::Horizontal</enum>
                           </property>
-                        </item>
-                        <item>
-                          <property name="text">
-                            <string>WARNING</string>
+                          <property name="sizeHint" stdset="0">
+                            <size>
+                              <width>40</width>
+                              <height>20</height>
+                            </size>
                           </property>
-                        </item>
-                        <item>
+                        </spacer>
+                      </item>
+                      <item>
+                        <widget class="QPushButton" name="pid_refresh">
                           <property name="text">
-                            <string>INFO</string>
+                            <string>Refresh</string>
                           </property>
-                        </item>
-                        <item>
-                          <property name="text">
-                            <string>DEBUG</string>
+                        </widget>
+                      </item>
+                      <item>
+                        <spacer name="horizontalSpacer_6">
+                          <property name="orientation">
+                            <enum>Qt::Horizontal</enum>
+                          </property>
+                          <property name="sizeHint" stdset="0">
+                            <size>
+                              <width>40</width>
+                              <height>20</height>
+                            </size>
                           </property>
-                        </item>
-                        <item>
+                        </spacer>
+                      </item>
+                      <item>
+                        <widget class="QPushButton" name="pid_restart">
                           <property name="text">
-                            <string>NOTSET</string>
+                            <string>Restart</string>
                           </property>
-                        </item>
-                      </widget>
-                    </item>
-                  </layout>
-                </widget>
-              </item>
-              <item>
-                <widget class="QGroupBox" name="groupBox_4">
-                  <property name="title">
-                    <string>Parsing conandata</string>
-                  </property>
-                  <layout class="QGridLayout" name="gridLayout_5">
-                    <item row="0" column="0">
-                      <widget class="QLabel" name="label_8">
-                        <property name="text">
-                          <string>YAML path segments to identify version list</string>
-                        </property>
-                      </widget>
-                    </item>
-                    <item row="0" column="1">
-                      <widget class="QLineEdit" name="prefs_conan_version_list_path_segment">
-                        <property name="toolTip">
-                          <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p&gt;For example, if your conandata.yml is formatted as&lt;/p&gt;&lt;p&gt;&lt;br/&gt;&lt;/p&gt;&lt;p&gt;  sources:&lt;/p&gt;&lt;p&gt;    1.2.3:&lt;/p&gt;&lt;p&gt;    ... &lt;/p&gt;&lt;p&gt;    4.5.6:&lt;/p&gt;&lt;p&gt;    ... &lt;/p&gt;&lt;p&gt;&lt;br/&gt;&lt;/p&gt;&lt;p&gt;then specify 'sources' in order to extract the version list&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
+                        </widget>
+                      </item>
+                    </layout>
+                  </widget>
+                </item>
+              </layout>
+            </widget>
+            <widget class="PackageRevisionPage" name="prev">
+              <layout class="QVBoxLayout" name="verticalLayout_5">
+                <item>
+                  <widget class="QLabel" name="prev_pkgref">
+                    <property name="contextMenuPolicy">
+                      <enum>Qt::CustomContextMenu</enum>
+                    </property>
+                    <property name="text">
+                      <string>Pkg ref + rrev + package_id</string>
+                    </property>
+                  </widget>
+                </item>
+                <item>
+                  <widget class="QGroupBox" name="prev_groupbox">
+                    <property name="enabled">
+                      <bool>false</bool>
+                    </property>
+                    <property name="title">
+                      <string>0 package revisions found</string>
+                    </property>
+                    <layout class="QVBoxLayout" name="verticalLayout_10">
+                      <property name="leftMargin">
+                        <number>0</number>
+                      </property>
+                      <property name="topMargin">
+                        <number>0</number>
+                      </property>
+                      <property name="rightMargin">
+                        <number>0</number>
+                      </property>
+                      <property name="bottomMargin">
+                        <number>0</number>
+                      </property>
+                      <item>
+                        <widget class="QTableView" name="package_revisions">
+                          <property name="contextMenuPolicy">
+                            <enum>Qt::CustomContextMenu</enum>
+                          </property>
+                          <property name="sizeAdjustPolicy">
+                            <enum>QAbstractScrollArea::AdjustToContents</enum>
+                          </property>
+                          <property name="editTriggers">
+                            <set>QAbstractItemView::NoEditTriggers</set>
+                          </property>
+                          <property name="alternatingRowColors">
+                            <bool>true</bool>
+                          </property>
+                          <property name="selectionMode">
+                            <enum>QAbstractItemView::SingleSelection</enum>
+                          </property>
+                          <property name="selectionBehavior">
+                            <enum>QAbstractItemView::SelectRows</enum>
+                          </property>
+                          <attribute name="horizontalHeaderStretchLastSection">
+                            <bool>false</bool>
+                          </attribute>
+                          <attribute name="verticalHeaderVisible">
+                            <bool>false</bool>
+                          </attribute>
+                        </widget>
+                      </item>
+                    </layout>
+                  </widget>
+                </item>
+                <item>
+                  <layout class="QHBoxLayout" name="horizontalLayout_9">
+                    <item>
+                      <widget class="QProgressBar" name="prev_progress">
+                        <property name="maximum">
+                          <number>1</number>
                         </property>
-                      </widget>
-                    </item>
-                  </layout>
-                </widget>
-              </item>
-              <item>
-                <spacer name="verticalSpacer_4">
-                  <property name="orientation">
-                    <enum>Qt::Vertical</enum>
-                  </property>
-                  <property name="sizeHint" stdset="0">
-                    <size>
-                      <width>20</width>
-                      <height>40</height>
-                    </size>
-                  </property>
-                </spacer>
-              </item>
-            </layout>
-          </widget>
-          <widget class="QWidget" name="prefs_localcache">
-            <property name="geometry">
-              <rect>
-                <x>0</x>
-                <y>0</y>
-                <width>654</width>
-                <height>232</height>
-              </rect>
-            </property>
-            <attribute name="label">
-              <string>Local cache</string>
-            </attribute>
-            <layout class="QVBoxLayout" name="verticalLayout_4">
-              <item>
-                <widget class="QGroupBox" name="groupBox_5">
-                  <property name="title">
-                    <string>New cache options</string>
-                  </property>
-                  <layout class="QGridLayout" name="gridLayout_6">
-                    <item row="0" column="0">
-                      <widget class="QLabel" name="label_9">
-                        <property name="text">
-                          <string>Config to install</string>
+                        <property name="value">
+                          <number>-1</number>
                         </property>
                       </widget>
                     </item>
-                    <item row="0" column="1">
-                      <widget class="QLineEdit" name="prefs_localcache_config_to_install"/>
-                    </item>
-                    <item row="1" column="0">
-                      <widget class="QLabel" name="label_10">
-                        <property name="text">
-                          <string>Git branch</string>
+                    <item>
+                      <widget class="QPushButton" name="prev_cancel">
+                        <property name="enabled">
+                          <bool>false</bool>
                         </property>
-                      </widget>
-                    </item>
-                    <item row="1" column="1">
-                      <widget class="QLineEdit" name="prefs_localcache_config_git_branch"/>
-                    </item>
-                  </layout>
-                </widget>
-              </item>
-              <item>
-                <widget class="QGroupBox" name="groupBox_6">
-                  <property name="title">
-                    <string>Forget caches without recipe associations</string>
-                  </property>
-                  <layout class="QGridLayout" name="gridLayout_7">
-                    <item row="0" column="1">
-                      <widget class="QPushButton" name="prefs_localcache_do_forget">
                         <property name="text">
-                          <string>Forget</string>
-                        </property>
-                      </widget>
-                    </item>
-                    <item row="0" column="0">
-                      <widget class="QComboBox" name="prefs_localcache_forget_cache">
-                        <property name="sizePolicy">
-                          <sizepolicy hsizetype="Preferred" vsizetype="Fixed">
-                            <horstretch>1</horstretch>
-                            <verstretch>0</verstretch>
-                          </sizepolicy>
+                          <string/>
+                        </property>
+                        <property name="icon">
+                          <iconset>
+                            <normaloff>:/cancel.svg</normaloff>
+                            :/cancel.svg
+                          </iconset>
                         </property>
                       </widget>
                     </item>
                   </layout>
-                </widget>
-              </item>
-              <item>
-                <spacer name="verticalSpacer_5">
-                  <property name="orientation">
-                    <enum>Qt::Vertical</enum>
-                  </property>
-                  <property name="sizeHint" stdset="0">
-                    <size>
-                      <width>20</width>
-                      <height>40</height>
-                    </size>
-                  </property>
-                </spacer>
-              </item>
-            </layout>
-          </widget>
-          <widget class="QWidget" name="prefs_graphviz">
-            <property name="geometry">
-              <rect>
-                <x>0</x>
-                <y>0</y>
-                <width>654</width>
-                <height>232</height>
-              </rect>
-            </property>
-            <attribute name="label">
-              <string>GraphViz</string>
-            </attribute>
-            <layout class="QGridLayout" name="gridLayout_8">
-              <item row="2" column="1">
-                <spacer name="verticalSpacer_8">
-                  <property name="orientation">
-                    <enum>Qt::Vertical</enum>
-                  </property>
-                  <property name="sizeHint" stdset="0">
-                    <size>
-                      <width>20</width>
-                      <height>40</height>
-                    </size>
-                  </property>
-                </spacer>
-              </item>
-              <item row="1" column="1">
-                <widget class="QLineEdit" name="prefs_graphviz_bin_directory"/>
-              </item>
-              <item row="1" column="0">
-                <widget class="QLabel" name="label_11">
-                  <property name="text">
-                    <string>GraphViz bin directory</string>
-                  </property>
-                </widget>
-              </item>
-              <item row="0" column="0" colspan="2">
-                <widget class="QLabel" name="label_29">
-                  <property name="text">
-                    <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p&gt;Download from &lt;a href=&quot;https://graphviz.org/download/&quot;&gt;&lt;span style=&quot; text-decoration: underline; color:#0068da;&quot;&gt;https://graphviz.org/download/&lt;/span&gt;&lt;/a&gt;&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
-                  </property>
-                  <property name="openExternalLinks">
-                    <bool>true</bool>
-                  </property>
-                </widget>
-              </item>
-            </layout>
-          </widget>
-          <widget class="QWidget" name="prefs_cmake">
-            <property name="geometry">
-              <rect>
-                <x>0</x>
-                <y>0</y>
-                <width>654</width>
-                <height>232</height>
-              </rect>
-            </property>
-            <attribute name="label">
-              <string>CMake</string>
-            </attribute>
-            <layout class="QGridLayout" name="gridLayout_9">
-              <item row="0" column="0">
-                <widget class="QLabel" name="label_12">
-                  <property name="text">
-                    <string>CMake bin directory</string>
-                  </property>
-                </widget>
-              </item>
-              <item row="0" column="1">
-                <widget class="QLineEdit" name="prefs_cmake_cmake_bin_directory"/>
-              </item>
-              <item row="1" column="0">
-                <widget class="QLabel" name="label_13">
-                  <property name="text">
-                    <string>Ninja bin directory</string>
-                  </property>
-                </widget>
-              </item>
-              <item row="1" column="1">
-                <widget class="QLineEdit" name="prefs_cmake_ninja_bin_directory"/>
-              </item>
-              <item row="2" column="0">
-                <spacer name="verticalSpacer_6">
-                  <property name="orientation">
-                    <enum>Qt::Vertical</enum>
-                  </property>
-                  <property name="sizeHint" stdset="0">
-                    <size>
-                      <width>20</width>
-                      <height>40</height>
-                    </size>
-                  </property>
-                </spacer>
-              </item>
-              <item row="2" column="1">
-                <spacer name="verticalSpacer_7">
-                  <property name="orientation">
-                    <enum>Qt::Vertical</enum>
-                  </property>
-                  <property name="sizeHint" stdset="0">
-                    <size>
-                      <width>20</width>
-                      <height>40</height>
-                    </size>
-                  </property>
-                </spacer>
-              </item>
-            </layout>
-          </widget>
-          <widget class="QWidget" name="prefs_compilercache">
-            <property name="geometry">
-              <rect>
-                <x>0</x>
-                <y>0</y>
-                <width>639</width>
-                <height>384</height>
-              </rect>
-            </property>
-            <attribute name="label">
-              <string>Compiler cache</string>
-            </attribute>
-            <layout class="QVBoxLayout" name="verticalLayout_5">
-              <item>
-                <widget class="QGroupBox" name="groupBox_7">
-                  <property name="title">
-                    <string>Default compiler cache</string>
-                  </property>
-                  <layout class="QVBoxLayout" name="verticalLayout_6">
-                    <item>
-                      <widget class="QComboBox" name="prefs_compilercache_default">
-                        <property name="toolTip">
-                          <string>The default compiler cache that attempts to integrate with Conan's CMake and Autotools helpers. YMMV.</string>
-                        </property>
-                        <item>
+                </item>
+                <item>
+                  <widget class="QWidget" name="prev_buttons" native="true">
+                    <layout class="QHBoxLayout" name="horizontalLayout_3">
+                      <item>
+                        <widget class="QPushButton" name="prev_back">
                           <property name="text">
-                            <string>None</string>
+                            <string>Back</string>
                           </property>
-                        </item>
-                        <item>
-                          <property name="text">
-                            <string>ccache</string>
+                        </widget>
+                      </item>
+                      <item>
+                        <spacer name="horizontalSpacer_3">
+                          <property name="orientation">
+                            <enum>Qt::Horizontal</enum>
+                          </property>
+                          <property name="sizeHint" stdset="0">
+                            <size>
+                              <width>40</width>
+                              <height>20</height>
+                            </size>
                           </property>
-                        </item>
-                        <item>
+                        </spacer>
+                      </item>
+                      <item>
+                        <widget class="QPushButton" name="prev_refresh">
                           <property name="text">
-                            <string>sccache</string>
+                            <string>Refresh</string>
+                          </property>
+                        </widget>
+                      </item>
+                      <item>
+                        <spacer name="horizontalSpacer_7">
+                          <property name="orientation">
+                            <enum>Qt::Horizontal</enum>
                           </property>
-                        </item>
-                        <item>
+                          <property name="sizeHint" stdset="0">
+                            <size>
+                              <width>40</width>
+                              <height>20</height>
+                            </size>
+                          </property>
+                        </spacer>
+                      </item>
+                      <item>
+                        <widget class="QPushButton" name="prev_restart">
                           <property name="text">
-                            <string>buildcache</string>
+                            <string>Restart</string>
                           </property>
-                        </item>
-                      </widget>
-                    </item>
-                  </layout>
-                </widget>
-              </item>
-              <item>
-                <widget class="QGroupBox" name="groupBox_8">
-                  <property name="title">
-                    <string>ccache</string>
-                  </property>
-                  <layout class="QGridLayout" name="gridLayout_10">
-                    <item row="1" column="0">
-                      <widget class="QLabel" name="label_15">
-                        <property name="text">
-                          <string>Location</string>
-                        </property>
-                      </widget>
-                    </item>
-                    <item row="1" column="1">
-                      <widget class="QLineEdit" name="prefs_compilercache_ccache_location"/>
-                    </item>
-                    <item row="0" column="0" colspan="2">
-                      <widget class="QLabel" name="label_14">
-                        <property name="text">
-                          <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p&gt;Download from &lt;a href=&quot;https://ccache.dev&quot;&gt;&lt;span style=&quot; text-decoration: underline; color:#0068da;&quot;&gt;https://ccache.dev&lt;/span&gt;&lt;/a&gt;&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
-                        </property>
-                        <property name="openExternalLinks">
-                          <bool>true</bool>
-                        </property>
-                      </widget>
-                    </item>
-                  </layout>
-                </widget>
-              </item>
-              <item>
-                <widget class="QGroupBox" name="groupBox_9">
-                  <property name="title">
-                    <string>sccache</string>
-                  </property>
-                  <layout class="QGridLayout" name="gridLayout_11">
-                    <item row="1" column="0">
-                      <widget class="QLabel" name="label_17">
-                        <property name="text">
-                          <string>Location</string>
-                        </property>
-                      </widget>
-                    </item>
-                    <item row="1" column="1">
-                      <widget class="QLineEdit" name="prefs_compilercache_sccache_location"/>
-                    </item>
-                    <item row="0" column="0" colspan="2">
-                      <widget class="QLabel" name="label_16">
-                        <property name="text">
-                          <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p&gt;Download from &lt;a href=&quot;https://github.com/mozilla/sccache&quot;&gt;&lt;span style=&quot; text-decoration: underline; color:#0068da;&quot;&gt;https://github.com/mozilla/sccache&lt;/span&gt;&lt;/a&gt;&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
+                        </widget>
+                      </item>
+                    </layout>
+                  </widget>
+                </item>
+              </layout>
+            </widget>
+            <widget class="PackageBinaryPage" name="pbinary">
+              <layout class="QVBoxLayout" name="verticalLayout_6">
+                <item>
+                  <widget class="QLabel" name="pbinary_pkgref">
+                    <property name="contextMenuPolicy">
+                      <enum>Qt::CustomContextMenu</enum>
+                    </property>
+                    <property name="text">
+                      <string>Pkg ref + rrev + package_id + prev</string>
+                    </property>
+                  </widget>
+                </item>
+                <item>
+                  <widget class="QGroupBox" name="pbinary_groupbox">
+                    <property name="enabled">
+                      <bool>false</bool>
+                    </property>
+                    <property name="title">
+                      <string>Package archive</string>
+                    </property>
+                    <layout class="QVBoxLayout" name="verticalLayout_11">
+                      <property name="leftMargin">
+                        <number>0</number>
+                      </property>
+                      <property name="topMargin">
+                        <number>0</number>
+                      </property>
+                      <property name="rightMargin">
+                        <number>0</number>
+                      </property>
+                      <property name="bottomMargin">
+                        <number>0</number>
+                      </property>
+                      <item>
+                        <widget class="QTreeView" name="package_binary">
+                          <property name="contextMenuPolicy">
+                            <enum>Qt::CustomContextMenu</enum>
+                          </property>
+                          <property name="sizeAdjustPolicy">
+                            <enum>QAbstractScrollArea::AdjustToContents</enum>
+                          </property>
+                          <property name="editTriggers">
+                            <set>QAbstractItemView::NoEditTriggers</set>
+                          </property>
+                          <property name="alternatingRowColors">
+                            <bool>true</bool>
+                          </property>
+                        </widget>
+                      </item>
+                    </layout>
+                  </widget>
+                </item>
+                <item>
+                  <layout class="QHBoxLayout" name="horizontalLayout_10">
+                    <item>
+                      <widget class="QProgressBar" name="pbinary_progress">
+                        <property name="maximum">
+                          <number>1</number>
                         </property>
-                        <property name="openExternalLinks">
-                          <bool>true</bool>
+                        <property name="value">
+                          <number>-1</number>
                         </property>
                       </widget>
                     </item>
-                  </layout>
-                </widget>
-              </item>
-              <item>
-                <widget class="QGroupBox" name="groupBox_10">
-                  <property name="title">
-                    <string>buildcache</string>
-                  </property>
-                  <layout class="QGridLayout" name="gridLayout_12">
-                    <item row="1" column="0">
-                      <widget class="QLabel" name="label_19">
-                        <property name="text">
-                          <string>Location</string>
+                    <item>
+                      <widget class="QPushButton" name="pbinary_cancel">
+                        <property name="enabled">
+                          <bool>false</bool>
                         </property>
-                      </widget>
-                    </item>
-                    <item row="1" column="1">
-                      <widget class="QLineEdit" name="prefs_compilercache_buildcache_location"/>
-                    </item>
-                    <item row="0" column="0" colspan="2">
-                      <widget class="QLabel" name="label_18">
                         <property name="text">
-                          <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p&gt;Download from &lt;a href=&quot;https://github.com/mbitsnbites/buildcache&quot;&gt;&lt;span style=&quot; text-decoration: underline; color:#0068da;&quot;&gt;https://github.com/mbitsnbites/buildcache&lt;/span&gt;&lt;/a&gt;&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
-                        </property>
-                        <property name="openExternalLinks">
-                          <bool>true</bool>
+                          <string/>
+                        </property>
+                        <property name="icon">
+                          <iconset>
+                            <normaloff>:/cancel.svg</normaloff>
+                            :/cancel.svg
+                          </iconset>
                         </property>
                       </widget>
                     </item>
                   </layout>
-                </widget>
-              </item>
-              <item>
-                <spacer name="verticalSpacer_13">
-                  <property name="orientation">
-                    <enum>Qt::Vertical</enum>
-                  </property>
-                  <property name="sizeHint" stdset="0">
-                    <size>
-                      <width>20</width>
-                      <height>40</height>
-                    </size>
-                  </property>
-                </spacer>
-              </item>
-            </layout>
-          </widget>
-          <widget class="QWidget" name="prefs_shortcuts">
-            <property name="geometry">
-              <rect>
-                <x>0</x>
-                <y>-287</y>
-                <width>639</width>
-                <height>519</height>
-              </rect>
-            </property>
-            <attribute name="label">
-              <string>Shortcuts</string>
-            </attribute>
-            <layout class="QGridLayout" name="gridLayout_13">
-              <item row="4" column="2">
-                <widget class="ShortcutLineEdit" name="prefs_shortcuts_installupdates_edit"/>
-              </item>
-              <item row="10" column="2">
-                <widget class="ShortcutLineEdit" name="prefs_shortcuts_remove_edit"/>
-              </item>
-              <item row="9" column="0">
-                <widget class="QLabel" name="label_23">
-                  <property name="text">
-                    <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p align=&quot;right&quot;&gt;&lt;img src=&quot;:/testpackage.svg&quot; width=&quot;20&quot; height=&quot;20&quot;/&gt; conan test&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
-                  </property>
-                </widget>
-              </item>
-              <item row="6" column="0">
-                <widget class="QLabel" name="label_20">
-                  <property name="text">
-                    <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p align=&quot;right&quot;&gt;&lt;img src=&quot;:/build.svg&quot; width=&quot;20&quot; height=&quot;20&quot;/&gt; conan build&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
-                  </property>
-                </widget>
-              </item>
-              <item row="3" column="2">
-                <widget class="ShortcutLineEdit" name="prefs_shortcuts_install_edit"/>
-              </item>
-              <item row="5" column="2">
-                <widget class="ShortcutLineEdit" name="prefs_shortcuts_source_edit"/>
-              </item>
-              <item row="15" column="2">
-                <spacer name="verticalSpacer_12">
-                  <property name="orientation">
-                    <enum>Qt::Vertical</enum>
-                  </property>
-                  <property name="sizeHint" stdset="0">
-                    <size>
-                      <width>20</width>
-                      <height>40</height>
-                    </size>
-                  </property>
-                </spacer>
-              </item>
-              <item row="13" column="2">
-                <widget class="ShortcutLineEdit" name="prefs_shortcuts_cmakebuildtoolverbose_edit"/>
-              </item>
-              <item row="0" column="0">
-                <widget class="QLabel" name="label_1">
-                  <property name="text">
-                    <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p align=&quot;right&quot;&gt;&lt;img src=&quot;:/create.svg&quot; width=&quot;20&quot; height=&quot;20&quot;/&gt; conan create&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
-                  </property>
-                  <property name="textFormat">
-                    <enum>Qt::RichText</enum>
-                  </property>
-                </widget>
-              </item>
-              <item row="11" column="0">
-                <widget class="QLabel" name="label_25">
-                  <property name="text">
-                    <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p align=&quot;right&quot;&gt;&lt;img src=&quot;:/cancel.svg&quot; width=&quot;20&quot; height=&quot;20&quot;/&gt; Cancel current command&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
-                  </property>
-                </widget>
-              </item>
-              <item row="8" column="0">
-                <widget class="QLabel" name="label_22">
-                  <property name="text">
-                    <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p align=&quot;right&quot;&gt;&lt;img src=&quot;:/exportpackage.svg&quot; width=&quot;20&quot; height=&quot;20&quot;/&gt; conan export-pkg&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
-                  </property>
-                </widget>
-              </item>
-              <item row="12" column="0">
-                <widget class="QLabel" name="prefs_shortcuts_cmakebuildtool_label">
-                  <property name="text">
-                    <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p align=&quot;right&quot;&gt;&lt;img src=&quot;:/cmakebuildtool.svg&quot; width=&quot;20&quot; height=&quot;20&quot;/&gt; CMake Build Tool&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
-                  </property>
-                </widget>
-              </item>
-              <item row="4" column="0">
-                <widget class="QLabel" name="label_5">
-                  <property name="text">
-                    <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p align=&quot;right&quot;&gt;&lt;img src=&quot;:/install.svg&quot; width=&quot;20&quot; height=&quot;20&quot;/&gt; conan install (update binaries)&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
-                  </property>
-                </widget>
-              </item>
-              <item row="12" column="2">
-                <widget class="ShortcutLineEdit" name="prefs_shortcuts_cmakebuildtool_edit"/>
-              </item>
-              <item row="5" column="0">
-                <widget class="QLabel" name="label_6">
-                  <property name="text">
-                    <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p align=&quot;right&quot;&gt;&lt;img src=&quot;:/source.svg&quot; width=&quot;20&quot; height=&quot;20&quot;/&gt; conan source&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
-                  </property>
-                </widget>
-              </item>
-              <item row="13" column="0">
-                <widget class="QLabel" name="prefs_shortcuts_cmakebuildtoolverbose_label">
-                  <property name="text">
-                    <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p align=&quot;right&quot;&gt;&lt;img src=&quot;:/cmakebuildtoolverbose.svg&quot; width=&quot;20&quot; height=&quot;20&quot;/&gt; CMake Build Tool (verbose)&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
-                  </property>
-                </widget>
-              </item>
-              <item row="9" column="2">
-                <widget class="ShortcutLineEdit" name="prefs_shortcuts_test_edit"/>
-              </item>
-              <item row="7" column="2">
-                <widget class="ShortcutLineEdit" name="prefs_shortcuts_package_edit"/>
-              </item>
-              <item row="14" column="2">
-                <widget class="ShortcutLineEdit" name="prefs_shortcuts_deletecmakecache_edit"/>
-              </item>
-              <item row="3" column="0">
-                <widget class="QLabel" name="label_4">
-                  <property name="text">
-                    <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p align=&quot;right&quot;&gt;&lt;img src=&quot;:/install.svg&quot; width=&quot;20&quot; height=&quot;20&quot;/&gt; conan install&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
-                  </property>
-                </widget>
-              </item>
-              <item row="11" column="2">
-                <widget class="ShortcutLineEdit" name="prefs_shortcuts_cancel_edit"/>
-              </item>
-              <item row="7" column="0">
-                <widget class="QLabel" name="prefs_shortcuts_package_label">
-                  <property name="text">
-                    <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p align=&quot;right&quot;&gt;&lt;img src=&quot;:/package.svg&quot; width=&quot;20&quot; height=&quot;20&quot;/&gt; conan package&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
-                  </property>
-                </widget>
-              </item>
-              <item row="2" column="0">
-                <widget class="QLabel" name="prefs_shortcuts_imports_label">
-                  <property name="text">
-                    <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p align=&quot;right&quot;&gt;&lt;img src=&quot;:/imports.svg&quot; width=&quot;20&quot; height=&quot;20&quot;/&gt; conan imports&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
-                  </property>
-                </widget>
-              </item>
-              <item row="14" column="0">
-                <widget class="QLabel" name="prefs_shortcuts_deletecmakecache_label">
-                  <property name="text">
-                    <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p align=&quot;right&quot;&gt;&lt;img src=&quot;:/removecmakecache.svg&quot; width=&quot;20&quot; height=&quot;20&quot;/&gt; Delete CMakeCache&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
-                  </property>
-                </widget>
-              </item>
-              <item row="8" column="2">
-                <widget class="ShortcutLineEdit" name="prefs_shortcuts_exportpackage_edit"/>
-              </item>
-              <item row="0" column="2">
-                <widget class="ShortcutLineEdit" name="prefs_shortcuts_create_edit"/>
-              </item>
-              <item row="6" column="2">
-                <widget class="ShortcutLineEdit" name="prefs_shortcuts_build_edit"/>
-              </item>
-              <item row="10" column="0">
-                <widget class="QLabel" name="label_24">
-                  <property name="text">
-                    <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p align=&quot;right&quot;&gt;&lt;img src=&quot;:/removepackage.svg&quot; width=&quot;20&quot; height=&quot;20&quot;/&gt; conan remove&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
-                  </property>
-                </widget>
-              </item>
-              <item row="2" column="2">
-                <widget class="ShortcutLineEdit" name="prefs_shortcuts_imports_edit"/>
-              </item>
-              <item row="1" column="0">
-                <widget class="QLabel" name="label_32">
-                  <property name="text">
-                    <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p align=&quot;right&quot;&gt;&lt;img src=&quot;:/create.svg&quot; width=&quot;20&quot; height=&quot;20&quot;/&gt; conan create (update binaries)&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
-                  </property>
-                  <property name="textFormat">
-                    <enum>Qt::RichText</enum>
-                  </property>
-                  <property name="alignment">
-                    <set>Qt::AlignLeading|Qt::AlignLeft|Qt::AlignVCenter</set>
-                  </property>
-                </widget>
-              </item>
-              <item row="1" column="2">
-                <widget class="ShortcutLineEdit" name="prefs_shortcuts_createupdates_edit"/>
-              </item>
-            </layout>
-          </widget>
-          <widget class="QWidget" name="prefs_recipes">
-            <property name="geometry">
-              <rect>
-                <x>0</x>
-                <y>0</y>
-                <width>654</width>
-                <height>232</height>
-              </rect>
-            </property>
-            <attribute name="label">
-              <string>Recipes</string>
-            </attribute>
-            <layout class="QVBoxLayout" name="verticalLayout_7">
-              <item>
-                <widget class="QTableView" name="prefs_recipes_table">
-                  <property name="contextMenuPolicy">
-                    <enum>Qt::CustomContextMenu</enum>
-                  </property>
-                  <property name="sizeAdjustPolicy">
-                    <enum>QAbstractScrollArea::AdjustToContents</enum>
-                  </property>
-                  <property name="editTriggers">
-                    <set>QAbstractItemView::NoEditTriggers</set>
-                  </property>
-                  <property name="alternatingRowColors">
-                    <bool>true</bool>
-                  </property>
-                  <property name="selectionMode">
-                    <enum>QAbstractItemView::SingleSelection</enum>
-                  </property>
-                  <property name="selectionBehavior">
-                    <enum>QAbstractItemView::SelectRows</enum>
-                  </property>
-                  <attribute name="horizontalHeaderStretchLastSection">
-                    <bool>true</bool>
-                  </attribute>
-                  <attribute name="verticalHeaderVisible">
-                    <bool>false</bool>
-                  </attribute>
-                </widget>
-              </item>
-              <item>
-                <spacer name="verticalSpacer_9">
-                  <property name="orientation">
-                    <enum>Qt::Vertical</enum>
-                  </property>
-                  <property name="sizeHint" stdset="0">
-                    <size>
-                      <width>20</width>
-                      <height>40</height>
-                    </size>
-                  </property>
-                </spacer>
-              </item>
-            </layout>
-          </widget>
-          <widget class="QWidget" name="prefs_recentconfigs">
-            <property name="geometry">
-              <rect>
-                <x>0</x>
-                <y>0</y>
-                <width>654</width>
-                <height>232</height>
-              </rect>
-            </property>
-            <attribute name="label">
-              <string>Recent configs</string>
-            </attribute>
-            <layout class="QVBoxLayout" name="verticalLayout_8">
-              <item>
-                <widget class="QListView" name="prefs_recentconfigs_list">
-                  <property name="contextMenuPolicy">
-                    <enum>Qt::CustomContextMenu</enum>
-                  </property>
-                  <property name="sizeAdjustPolicy">
-                    <enum>QAbstractScrollArea::AdjustToContents</enum>
-                  </property>
-                  <property name="editTriggers">
-                    <set>QAbstractItemView::NoEditTriggers</set>
-                  </property>
-                  <property name="alternatingRowColors">
-                    <bool>true</bool>
-                  </property>
-                  <property name="selectionBehavior">
-                    <enum>QAbstractItemView::SelectRows</enum>
-                  </property>
-                </widget>
-              </item>
-              <item>
-                <spacer name="verticalSpacer_10">
-                  <property name="orientation">
-                    <enum>Qt::Vertical</enum>
-                  </property>
-                  <property name="sizeHint" stdset="0">
-                    <size>
-                      <width>20</width>
-                      <height>40</height>
-                    </size>
-                  </property>
-                </spacer>
-              </item>
-            </layout>
-          </widget>
-          <widget class="QWidget" name="prefs_recentremotes">
-            <property name="geometry">
-              <rect>
-                <x>0</x>
-                <y>0</y>
-                <width>654</width>
-                <height>232</height>
-              </rect>
-            </property>
-            <attribute name="label">
-              <string>Recent remotes</string>
-            </attribute>
-            <layout class="QVBoxLayout" name="verticalLayout_9">
-              <item>
-                <widget class="QListView" name="prefs_recentremotes_list">
-                  <property name="contextMenuPolicy">
-                    <enum>Qt::CustomContextMenu</enum>
-                  </property>
-                  <property name="sizeAdjustPolicy">
-                    <enum>QAbstractScrollArea::AdjustToContents</enum>
-                  </property>
-                  <property name="editTriggers">
-                    <set>QAbstractItemView::NoEditTriggers</set>
-                  </property>
-                  <property name="alternatingRowColors">
-                    <bool>true</bool>
-                  </property>
-                  <property name="selectionBehavior">
-                    <enum>QAbstractItemView::SelectRows</enum>
-                  </property>
-                </widget>
-              </item>
-              <item>
-                <spacer name="verticalSpacer_11">
-                  <property name="orientation">
-                    <enum>Qt::Vertical</enum>
-                  </property>
-                  <property name="sizeHint" stdset="0">
-                    <size>
-                      <width>20</width>
-                      <height>40</height>
-                    </size>
-                  </property>
-                </spacer>
-              </item>
-            </layout>
-          </widget>
-        </widget>
-      </item>
-      <item>
-        <widget class="QDialogButtonBox" name="prefs_buttons">
-          <property name="orientation">
-            <enum>Qt::Horizontal</enum>
-          </property>
-          <property name="standardButtons">
-            <set>QDialogButtonBox::Apply|QDialogButtonBox::Cancel|QDialogButtonBox::Ok</set>
-          </property>
-        </widget>
-      </item>
-    </layout>
-    <action name="actionForget_recipe">
-      <property name="text">
-        <string>Forget recipe</string>
-      </property>
-    </action>
-    <action name="actionForget_config">
-      <property name="text">
-        <string>Forget config</string>
-      </property>
-    </action>
-    <action name="actionForget_remote">
-      <property name="text">
-        <string>Forget remote</string>
-      </property>
-    </action>
+                </item>
+                <item>
+                  <widget class="QWidget" name="pbinary_buttons" native="true">
+                    <layout class="QHBoxLayout" name="horizontalLayout_4">
+                      <item>
+                        <widget class="QPushButton" name="pbinary_back">
+                          <property name="text">
+                            <string>Back</string>
+                          </property>
+                        </widget>
+                      </item>
+                      <item>
+                        <spacer name="horizontalSpacer_4">
+                          <property name="orientation">
+                            <enum>Qt::Horizontal</enum>
+                          </property>
+                          <property name="sizeHint" stdset="0">
+                            <size>
+                              <width>40</width>
+                              <height>20</height>
+                            </size>
+                          </property>
+                        </spacer>
+                      </item>
+                      <item>
+                        <widget class="QPushButton" name="pbinary_restart">
+                          <property name="text">
+                            <string>Restart</string>
+                          </property>
+                        </widget>
+                      </item>
+                    </layout>
+                  </widget>
+                </item>
+              </layout>
+            </widget>
+          </widget>
+        </item>
+        <item>
+          <widget class="QPlainTextEdit" name="log">
+            <property name="contextMenuPolicy">
+              <enum>Qt::CustomContextMenu</enum>
+            </property>
+            <property name="sizeAdjustPolicy">
+              <enum>QAbstractScrollArea::AdjustToContents</enum>
+            </property>
+            <property name="readOnly">
+              <bool>true</bool>
+            </property>
+          </widget>
+        </item>
+        <item>
+          <spacer name="verticalSpacer">
+            <property name="orientation">
+              <enum>Qt::Vertical</enum>
+            </property>
+            <property name="sizeHint" stdset="0">
+              <size>
+                <width>20</width>
+                <height>40</height>
+              </size>
+            </property>
+          </spacer>
+        </item>
+      </layout>
+    </widget>
   </widget>
   <customwidgets>
     <customwidget>
-      <class>ShortcutLineEdit</class>
-      <extends>QLineEdit</extends>
-      <header>cruiz/widgets/shortcutlineedit.h</header>
+      <class>PackageReferencePage</class>
+      <extends>QWidget</extends>
+      <header>cruiz/remote_browser/pages/packagereferencepage.h</header>
+      <container>1</container>
+    </customwidget>
+    <customwidget>
+      <class>RecipeRevisionPage</class>
+      <extends>QWidget</extends>
+      <header>cruiz/remote_browser/pages/reciperevisionpage.h</header>
+      <container>1</container>
+    </customwidget>
+    <customwidget>
+      <class>PackageIdPage</class>
+      <extends>QWidget</extends>
+      <header>cruiz/remote_browser/pages/packageidpage.h</header>
+      <container>1</container>
+    </customwidget>
+    <customwidget>
+      <class>PackageRevisionPage</class>
+      <extends>QWidget</extends>
+      <header>cruiz/remote_browser/pages/packagerevisionpage.h</header>
+      <container>1</container>
+    </customwidget>
+    <customwidget>
+      <class>PackageBinaryPage</class>
+      <extends>QWidget</extends>
+      <header>cruiz/remote_browser/pages/packagebinarypage.h</header>
+      <container>1</container>
     </customwidget>
   </customwidgets>
   <resources/>
-  <connections>
-    <connection>
-      <sender>prefs_buttons</sender>
-      <signal>accepted()</signal>
-      <receiver>PreferencesDialog</receiver>
-      <slot>accept()</slot>
-      <hints>
-        <hint type="sourcelabel">
-          <x>248</x>
-          <y>254</y>
-        </hint>
-        <hint type="destinationlabel">
-          <x>157</x>
-          <y>274</y>
-        </hint>
-      </hints>
-    </connection>
-    <connection>
-      <sender>prefs_buttons</sender>
-      <signal>rejected()</signal>
-      <receiver>PreferencesDialog</receiver>
-      <slot>reject()</slot>
-      <hints>
-        <hint type="sourcelabel">
-          <x>316</x>
-          <y>260</y>
-        </hint>
-        <hint type="destinationlabel">
-          <x>286</x>
-          <y>274</y>
-        </hint>
-      </hints>
-    </connection>
-  </connections>
+  <connections/>
 </ui>
```

### Comparing `cruiz-1.4.0a3/cruiz/resources/recipe_cmake_features_frame.ui` & `cruiz-1.4.0a4/cruiz/resources/recipe_cmake_features_frame.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/resources/recipe_compiler_cache_configuration_dialog.ui` & `cruiz-1.4.0a4/cruiz/resources/recipe_compiler_cache_configuration_dialog.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/resources/recipe_compilercache_features_frame.ui` & `cruiz-1.4.0a4/cruiz/resources/recipe_compilercache_features_frame.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/resources/recipe_cpucores_frame.ui` & `cruiz-1.4.0a4/cruiz/resources/recipe_cpucores_frame.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/resources/recipe_local_workflow_expression_editor.ui` & `cruiz-1.4.0a4/cruiz/resources/recipe_local_workflow_expression_editor.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/resources/recipe_profile_frame.ui` & `cruiz-1.4.0a4/cruiz/resources/recipe_profile_frame.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/resources/recipe_window.ui` & `cruiz-1.4.0a4/cruiz/resources/recipe_window.ui`

 * *Files 4% similar despite different names*

#### Comparing `cruiz-1.4.0a3/cruiz/resources/recipe_window.ui` & `cruiz-1.4.0a4/cruiz/resources/recipe_window.ui`

```diff
@@ -857,174 +857,84 @@
               </widget>
             </widget>
           </item>
         </layout>
       </widget>
     </widget>
     <action name="actionCreateCommand">
-      <property name="icon">
-        <iconset>
-          <normaloff>:/create.svg</normaloff>
-          :/create.svg
-        </iconset>
-      </property>
       <property name="text">
         <string>Create package in local cache</string>
       </property>
     </action>
     <action name="actionCreateUpdateCommand">
-      <property name="icon">
-        <iconset>
-          <normaloff>:/create.svg</normaloff>
-          :/create.svg
-        </iconset>
-      </property>
       <property name="text">
         <string>Create package in local cache with latest dependencies</string>
       </property>
     </action>
     <action name="actionImportsCommand">
-      <property name="icon">
-        <iconset>
-          <normaloff>:/imports.svg</normaloff>
-          :/imports.svg
-        </iconset>
-      </property>
       <property name="text">
         <string>Import files from dependents</string>
       </property>
     </action>
     <action name="actionInstallCommand">
-      <property name="icon">
-        <iconset>
-          <normaloff>:/install.svg</normaloff>
-          :/install.svg
-        </iconset>
-      </property>
       <property name="text">
         <string>Download dependencies and configure</string>
       </property>
     </action>
     <action name="actionInstallUpdateCommand">
-      <property name="icon">
-        <iconset>
-          <normaloff>:/install.svg</normaloff>
-          :/install.svg
-        </iconset>
-      </property>
       <property name="text">
         <string>Download latest dependencies and configure</string>
       </property>
     </action>
     <action name="actionSourceCommand">
-      <property name="icon">
-        <iconset>
-          <normaloff>:/source.svg</normaloff>
-          :/source.svg
-        </iconset>
-      </property>
       <property name="text">
         <string>Get source code</string>
       </property>
     </action>
     <action name="actionBuildCommand">
-      <property name="icon">
-        <iconset>
-          <normaloff>:/build.svg</normaloff>
-          :/build.svg
-        </iconset>
-      </property>
       <property name="text">
         <string>Build source</string>
       </property>
     </action>
     <action name="actionPackageCommand">
-      <property name="icon">
-        <iconset>
-          <normaloff>:/package.svg</normaloff>
-          :/package.svg
-        </iconset>
-      </property>
       <property name="text">
         <string>Make local package</string>
       </property>
     </action>
     <action name="actionExportPackageCommand">
-      <property name="icon">
-        <iconset>
-          <normaloff>:/exportpackage.svg</normaloff>
-          :/exportpackage.svg
-        </iconset>
-      </property>
       <property name="text">
         <string>Export package to local cache</string>
       </property>
     </action>
     <action name="actionTestCommand">
-      <property name="icon">
-        <iconset>
-          <normaloff>:/testpackage.svg</normaloff>
-          :/testpackage.svg
-        </iconset>
-      </property>
       <property name="text">
         <string>Test package in local cache</string>
       </property>
     </action>
     <action name="actionCancelCommand">
-      <property name="icon">
-        <iconset>
-          <normaloff>:/cancel.svg</normaloff>
-          :/cancel.svg
-        </iconset>
-      </property>
       <property name="text">
         <string>Cancel running command</string>
       </property>
     </action>
     <action name="actionRemovePackageCommand">
-      <property name="icon">
-        <iconset>
-          <normaloff>:/removepackage.svg</normaloff>
-          :/removepackage.svg
-        </iconset>
-      </property>
       <property name="text">
         <string>Remove package from local cache</string>
       </property>
     </action>
     <action name="actionCMakeBuildToolCommand">
-      <property name="icon">
-        <iconset>
-          <normaloff>:/cmakebuildtool.svg</normaloff>
-          :/cmakebuildtool.svg
-        </iconset>
-      </property>
       <property name="text">
         <string>Run CMake build tool</string>
       </property>
     </action>
     <action name="actionCMakeBuildToolVerboseCommand">
-      <property name="icon">
-        <iconset>
-          <normaloff>:/cmakebuildtoolverbose.svg</normaloff>
-          :/cmakebuildtoolverbose.svg
-        </iconset>
-      </property>
       <property name="text">
         <string>Run CMake build tool (verbose)</string>
       </property>
     </action>
     <action name="actionCMakeRemoveCacheCommand">
-      <property name="icon">
-        <iconset>
-          <normaloff>:/removecmakecache.svg</normaloff>
-          :/removecmakecache.svg
-        </iconset>
-      </property>
       <property name="text">
         <string>Delete CMake cache</string>
       </property>
     </action>
     <action name="actionOpen_another_version">
       <property name="text">
         <string>Open another version of this recipe...</string>
```

### Comparing `cruiz-1.4.0a3/cruiz/resources/remote_browser_fileview.ui` & `cruiz-1.4.0a4/cruiz/resources/remote_browser_fileview.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/revealonfilesystem.py` & `cruiz-1.4.0a4/cruiz/revealonfilesystem.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,30 +39,30 @@
     QtCore.QProcess.startDetached(explorer_path, script_args)
 
 
 def _use_xdg_open(file_info: QtCore.QFileInfo) -> None:
     xdg_open_path = QtCore.QStandardPaths.findExecutable("xdg-open")
     if not xdg_open_path:
         QtWidgets.QMessageBox.critical(
-            None,  # type: ignore
+            None,
             "Cannot reveal path",
             "Unable to find the path to xdg-open",
         )
         return
     script_args = [file_info.canonicalFilePath()]
     QtCore.QProcess.startDetached(xdg_open_path, script_args)
 
 
 def reveal_on_filesystem(path: pathlib.Path) -> None:
     """
     Reveal the path in a filesystem GUI
     """
     if not path.exists():
         QtWidgets.QMessageBox.critical(
-            None, "Cannot reveal path", f"Path '{path}' does not exist"  # type: ignore
+            None, "Cannot reveal path", f"Path '{path}' does not exist"
         )
         return
     file_info = QtCore.QFileInfo(path)
     if platform.system() == "Darwin":
         _use_finder(file_info)
     elif platform.system() == "Windows":
         _use_explorer(file_info)
@@ -77,15 +77,15 @@
     Open a terminal at the given directory path.
     """
     # cannot use QProcess here, as it starts a shell in-pr5ocess, even if called
     # with startDetached
     file_info = QtCore.QFileInfo(path)
     if not file_info.exists():
         QtWidgets.QMessageBox.critical(
-            None,  # type: ignore
+            None,
             "Cannot open terminal at path",
             f"Path '{path}' does not exist",
         )
         return
     if platform.system() == "Darwin":
         app = "Terminal"
         _run_apple_script(
@@ -105,13 +105,13 @@
             # trailing $SHELL is to keep the new terminal open
             os.system(
                 "gnome-terminal -- /bin/bash -c "
                 f"'cd {file_info.canonicalFilePath()}; $SHELL'"
             )
         else:
             QtWidgets.QMessageBox.critical(
-                None,  # type: ignore
+                None,
                 "Cannot open terminal at path",
                 "Unable to detect window manager",
             )
     else:
         raise RuntimeError(f"Unrecognised platform {platform.system()}")
```

### Comparing `cruiz-1.4.0a3/cruiz/settings/ensuredefaultlocalcache.py` & `cruiz-1.4.0a4/cruiz/settings/ensuredefaultlocalcache.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/settings/managers/__init__.py` & `cruiz-1.4.0a4/cruiz/settings/managers/__init__.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/settings/managers/basesettings.py` & `cruiz-1.4.0a4/cruiz/settings/managers/basesettings.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/settings/managers/cleansettings.py` & `cruiz-1.4.0a4/cruiz/settings/managers/cleansettings.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/settings/managers/cmakepreferences.py` & `cruiz-1.4.0a4/cruiz/settings/managers/cmakepreferences.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/settings/managers/compilercachepreferences.py` & `cruiz-1.4.0a4/cruiz/settings/managers/compilercachepreferences.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/settings/managers/conanpreferences.py` & `cruiz-1.4.0a4/cruiz/settings/managers/conanpreferences.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/settings/managers/fontpreferences.py` & `cruiz-1.4.0a4/cruiz/settings/managers/fontpreferences.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/settings/managers/generalpreferences.py` & `cruiz-1.4.0a4/cruiz/settings/managers/generalpreferences.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,14 @@
                 BoolSetting,
                 default_stdout_batching_value,
                 ScalarValue,
             ),
             "enable_command_timing": SettingMeta(
                 "EnableCommandTimings", BoolSetting, False, ScalarValue
             ),
-            "use_dark_mode": SettingMeta("DarkMode", BoolSetting, False, ScalarValue),
             "use_compact_look": SettingMeta(
                 "UseCompactLook", BoolSetting, False, ScalarValue
             ),
             "default_recipe_directory": SettingMeta(
                 "DefaultRecipeDirectory", StringSetting, None, ScalarValue
             ),
             "default_recipe_editor": SettingMeta(
@@ -113,25 +112,14 @@
         return self._get_value_via_meta()
 
     @enable_command_timing.setter
     def enable_command_timing(self, value: bool) -> None:
         self._set_value_via_meta(value)
 
     @property
-    def use_dark_mode(self) -> BoolSetting:
-        """
-        Get whether dark mode is enabled
-        """
-        return self._get_value_via_meta()
-
-    @use_dark_mode.setter
-    def use_dark_mode(self, value: bool) -> None:
-        self._set_value_via_meta(value)
-
-    @property
     def use_compact_look(self) -> BoolSetting:
         """
         Get whether a compact look is enabled.
         OBSOLETE
         """
         return self._get_value_via_meta()
```

### Comparing `cruiz-1.4.0a3/cruiz/settings/managers/graphvizpreferences.py` & `cruiz-1.4.0a4/cruiz/settings/managers/graphvizpreferences.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/settings/managers/localcachepreferences.py` & `cruiz-1.4.0a4/cruiz/settings/managers/localcachepreferences.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/settings/managers/namedlocalcache.py` & `cruiz-1.4.0a4/cruiz/settings/managers/namedlocalcache.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/settings/managers/ninjapreferences.py` & `cruiz-1.4.0a4/cruiz/settings/managers/ninjapreferences.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/settings/managers/recentconanconfigs.py` & `cruiz-1.4.0a4/cruiz/settings/managers/recentconanconfigs.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/settings/managers/recentconanremotes.py` & `cruiz-1.4.0a4/cruiz/settings/managers/recentconanremotes.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/settings/managers/recentrecipes.py` & `cruiz-1.4.0a4/cruiz/settings/managers/recentrecipes.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/settings/managers/recipe.py` & `cruiz-1.4.0a4/cruiz/settings/managers/recipe.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
     def __init__(self) -> None:
         super().__init__()
         self._uuid: typing.Optional[QtCore.QUuid] = None
         self._recipe: typing.Optional[Recipe] = None
 
         if self._recipe:
-            default_profile = self._recipe.context.default_profile_filename()
+            default_profile = self._recipe.context.default_profile_filename()  # type: ignore[unreachable]  # noqa: E501
         else:
             try:
                 context = self.settings_reader.recipe.context  # type: ignore
                 default_profile = context.default_profile_filename()
             except AttributeError:
                 # this copes with there not being a context assigned
                 # a recipe upon first load
```

### Comparing `cruiz-1.4.0a3/cruiz/settings/managers/shortcuts.py` & `cruiz-1.4.0a4/cruiz/settings/managers/shortcuts.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/settings/managers/valueclasses.py` & `cruiz-1.4.0a4/cruiz/settings/managers/valueclasses.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/settings/managers/writermixin.py` & `cruiz-1.4.0a4/cruiz/settings/managers/writermixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,22 +27,22 @@
         assert hasattr(self, "_reader_for_writer")
         keys_to_set = [k for k in changes.__dict__.keys() if k.startswith("__")]
         if not keys_to_set:
             return
         # get current values from settings and fallbacks
         current_values = {}
         assert hasattr(self, "_reader_for_writer")
-        with self._reader_for_writer as settings:  # type: ignore
+        with self._reader_for_writer as settings:
             for key in keys_to_set:
                 entry = getattr(changes, key)
                 current_values[entry.key] = getattr(settings, entry.property_name)
         # delete those values changes to the fallbacks
         # set others
         with BaseSettings.Group(
-            self._reader_for_writer.group  # type: ignore
+            self._reader_for_writer.group
         ) as settings:  # TODO: should probably re-use the settings instance
             for key in keys_to_set:
                 entry = getattr(changes, key)
                 # if entry values vs current values are any of the following, the
                 # disk setting can be removed
                 # - equal
                 # - entry is falsey and the fallback is None
```

### Comparing `cruiz-1.4.0a3/cruiz/settings/models/recentconanconfigmodel.py` & `cruiz-1.4.0a4/cruiz/settings/models/recentconanconfigmodel.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/settings/models/recentconanremotesmodel.py` & `cruiz-1.4.0a4/cruiz/settings/models/recentconanremotesmodel.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/settings/models/recipesmodel.py` & `cruiz-1.4.0a4/cruiz/settings/models/recipesmodel.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,9 +81,9 @@
         return None
 
     def flags(self, index):  # type: ignore
         def_flags = super().flags(index)
         if self._uuids and cruiz.globals.get_main_window().is_recipe_active(
             self._uuids[index.row()]
         ):
-            return def_flags & ~QtCore.Qt.ItemIsEnabled  # type: ignore[operator]
+            return def_flags & ~QtCore.Qt.ItemIsEnabled
         return def_flags
```

### Comparing `cruiz-1.4.0a3/cruiz/settings/preferencesdialog.py` & `cruiz-1.4.0a4/cruiz/settings/preferencesdialog.py`

 * *Files 3% similar despite different names*

```diff
@@ -109,14 +109,17 @@
         self._ui = Ui_PreferencesDialog()
         self._ui.setupUi(self)  # type: ignore[no-untyped-call]
         # -- signals
         self.modified.connect(self._modification_applied)
         self.preferences_updated.connect(
             qApp.on_preferences_updated  # type: ignore  # noqa: F821
         )
+        cruiz.globals.get_main_window().theme_changed.connect(
+            self._refresh_shortcut_icons
+        )
         # -- toolbox
         self._ui.prefs_toolbox.currentChanged.connect(self._current_load_defaults)
         self._import_prefs = QtWidgets.QPushButton("Import...")
         self._export_prefs = QtWidgets.QPushButton("Export...")
         self._clean_prefs = QtWidgets.QPushButton("Clean...")
         self._restore_default_prefs = QtWidgets.QPushButton("Restore defaults")
         self._setup_buttons()
@@ -219,17 +222,14 @@
         )
         self._ui.prefs_general_usebatching.stateChanged.connect(
             self._general_usebatching
         )
         self._ui.prefs_general_enable_wallclock.stateChanged.connect(
             self._general_wallclock
         )
-        self._ui.prefs_general_enable_darkmode.stateChanged.connect(
-            self._general_darkmode
-        )
         self._ui.prefs_general_enable_compact.stateChanged.connect(
             self._general_compactlook
         )
         dir_icon = self.style().standardIcon(QtWidgets.QStyle.SP_DirIcon)
         open_recipedir_action = QtGui.QAction(dir_icon, "", self)
         open_recipedir_action.triggered.connect(self._general_open_recipedir)
         self._ui.prefs_general_default_recipe_dir.addAction(
@@ -423,14 +423,15 @@
         else:
             self._ui.prefs_shortcuts_cmakebuildtool_label.hide()
             self._ui.prefs_shortcuts_cmakebuildtool_edit.hide()
             self._ui.prefs_shortcuts_cmakebuildtoolverbose_label.hide()
             self._ui.prefs_shortcuts_cmakebuildtoolverbose_edit.hide()
             self._ui.prefs_shortcuts_deletecmakecache_label.hide()
             self._ui.prefs_shortcuts_deletecmakecache_edit.hide()
+        self._refresh_shortcut_icons()
 
     def _setup_recipes_toolbox(self) -> None:
         self._prefs_recipes_model = RecipesModel()
         self._ui.prefs_recipes_table.setModel(self._prefs_recipes_model)
         self._ui.prefs_recipes_table.horizontalHeader().setSectionResizeMode(
             0, QtWidgets.QHeaderView.ResizeToContents
         )
@@ -517,16 +518,14 @@
                 blocked_widget.setChecked(settings.combine_panes.resolve())
             with BlockSignals(self._ui.prefs_general_usebatching) as blocked_widget:
                 blocked_widget.setChecked(settings.use_stdout_batching.resolve())
             with BlockSignals(
                 self._ui.prefs_general_enable_wallclock
             ) as blocked_widget:
                 blocked_widget.setChecked(settings.enable_command_timing.resolve())
-            with BlockSignals(self._ui.prefs_general_enable_darkmode) as blocked_widget:
-                blocked_widget.setChecked(settings.use_dark_mode.resolve())
             with BlockSignals(self._ui.prefs_general_enable_compact) as blocked_widget:
                 blocked_widget.setChecked(settings.use_compact_look.resolve())
             with BlockSignals(
                 self._ui.prefs_general_default_recipe_dir
             ) as blocked_widget:
                 blocked_widget.setText(
                     settings.default_recipe_directory.resolve() or ""
@@ -541,46 +540,44 @@
                 blocked_widget.setText(settings.default_recipe_editor.resolve() or "")
             # Note: the following is not part of the new UI
             with BlockSignals(self._ui.prefs_general_new_recipe_load) as blocked_widget:
                 blocked_widget.setChecked(
                     settings.new_recipe_loading_behaviour.resolve()
                 )
 
-    def _general_change_boolean(self, property_name: str, state: int) -> None:
-        enabled = state == QtCore.Qt.Checked  # type: ignore[comparison-overlap]
-        setattr(self._prefs_general, property_name, enabled)
-        self.modified.emit()
-
     def _general_clearplanes(self, state: int) -> None:
-        self._prefs_general.clear_panes = state == QtCore.Qt.Checked  # type: ignore
+        self._prefs_general.clear_panes = (
+            QtCore.Qt.CheckState(state) == QtCore.Qt.Checked
+        )
         self.modified.emit()
 
     def _general_combinepanes(self, state: int) -> None:
-        self._prefs_general.combine_panes = state == QtCore.Qt.Checked  # type: ignore
+        self._prefs_general.combine_panes = (
+            QtCore.Qt.CheckState(state) == QtCore.Qt.Checked
+        )
         self.modified.emit()
         self._requires_restart()
 
     def _general_usebatching(self, state: int) -> None:
-        enabled = state == QtCore.Qt.Checked  # type: ignore[comparison-overlap]
-        self._prefs_general.use_stdout_batching = enabled  # type: ignore
+        self._prefs_general.use_stdout_batching = (
+            QtCore.Qt.CheckState(state) == QtCore.Qt.Checked
+        )
         self.modified.emit()
         self._requires_restart()
 
     def _general_wallclock(self, state: int) -> None:
-        enabled = state == QtCore.Qt.Checked  # type: ignore[comparison-overlap]
-        self._prefs_general.enable_command_timing = enabled  # type: ignore
-        self.modified.emit()
-
-    def _general_darkmode(self, state: int) -> None:
-        self._prefs_general.use_dark_mode = state == QtCore.Qt.Checked  # type: ignore
+        self._prefs_general.enable_command_timing = (
+            QtCore.Qt.CheckState(state) == QtCore.Qt.Checked
+        )
         self.modified.emit()
 
     def _general_compactlook(self, state: int) -> None:
-        enabled = state == QtCore.Qt.Checked  # type: ignore[comparison-overlap]
-        self._prefs_general.use_compact_look = enabled  # type: ignore
+        self._prefs_general.use_compact_look = (
+            QtCore.Qt.CheckState(state) == QtCore.Qt.Checked
+        )
         self.modified.emit()
 
     def _general_open_recipedir(self) -> None:
         with GeneralSettingsReader() as settings:
             last_dir = settings.default_recipe_directory.resolve()
         new_dir = QtWidgets.QFileDialog.getExistingDirectory(
             self,
@@ -629,16 +626,17 @@
             self._ui.prefs_general_recipe_editor.setText(new_path)
 
     def _general_recipe_editor(self, text: str) -> None:
         self._prefs_general.default_recipe_editor = text or None  # type: ignore
         self.modified.emit()
 
     def _general_newrecipeload(self, state: int) -> None:
-        enabled = state == QtCore.Qt.Checked  # type: ignore[comparison-overlap]
-        self._prefs_general.new_recipe_loading_behaviour = enabled  # type: ignore
+        self._prefs_general.new_recipe_loading_behaviour = (
+            QtCore.Qt.CheckState(state) == QtCore.Qt.Checked
+        )
         self.modified.emit()
 
     # -- font --
     @staticmethod
     def _font_from_details(
         details: typing.Tuple[typing.Optional[str], typing.Optional[int]]
     ) -> typing.Optional[QtGui.QFont]:
@@ -1257,7 +1255,42 @@
             (
                 "Performing a factory reset will clear all settings and restart cruiz. "
                 "Do you want to continue?"
             ),
         )
         if result == QtWidgets.QMessageBox.StandardButton.Yes:
             factory_reset()
+
+    def _refresh_shortcut_icons(self) -> None:
+        def _set_pixmap(label: QtWidgets.QLabel, name: str) -> None:
+            size = 32
+            if name.startswith(":/"):
+                icon = QtGui.QIcon(name)
+            else:
+                icon = QtGui.QIcon(f":/icons/{cruiz.globals.get_theme()}/{name}")
+            label.setPixmap(icon.pixmap(size, size))
+
+        _set_pixmap(self._ui.shortcut_conan_create, "create.svg")
+        _set_pixmap(self._ui.shortcut_conan_create_update, "create.svg")
+        _set_pixmap(self._ui.shortcut_conan_install, "install.svg")
+        _set_pixmap(self._ui.shortcut_conan_install_update, "install.svg")
+        _set_pixmap(self._ui.shortcut_conan_source, "source.svg")
+        _set_pixmap(self._ui.shortcut_conan_build, "build.svg")
+        _set_pixmap(self._ui.shortcut_conan_export_package, "exportpackage.svg")
+        _set_pixmap(self._ui.shortcut_conan_test, "testpackage.svg")
+        _set_pixmap(self._ui.shortcut_conan_remove, "removepackage.svg")
+        _set_pixmap(self._ui.shortcut_cancel_command, ":/cancel.svg")
+        if cruiz.globals.CONAN_MAJOR_VERSION == 1:
+            _set_pixmap(self._ui.shortcut_conan_imports, "imports.svg")
+            _set_pixmap(self._ui.shortcut_conan_package, "package.svg")
+            _set_pixmap(self._ui.shortcut_cmake_build_tool, ":/cmakebuildtool.svg")
+            _set_pixmap(
+                self._ui.shortcut_cmake_verbose_build_tool,
+                ":/cmakebuildtoolverbose.svg",
+            )
+            _set_pixmap(self._ui.shortcut_delete_cmake_cache, ":/removecmakecache.svg")
+        else:
+            self._ui.shortcut_conan_imports.hide()
+            self._ui.shortcut_conan_package.hide()
+            self._ui.shortcut_cmake_build_tool.hide()
+            self._ui.shortcut_cmake_verbose_build_tool.hide()
+            self._ui.shortcut_delete_cmake_cache.hide()
```

### Comparing `cruiz-1.4.0a3/cruiz/settings/updatesettings.py` & `cruiz-1.4.0a4/cruiz/settings/updatesettings.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import typing
 
 from qtpy import QtCore
 
 from .managers.basesettings import BaseSettings
 
 
-CURRENT_SETTINGS_VERSION = 8
+CURRENT_SETTINGS_VERSION = 9
 
 
 class SettingsGroup:
     """
     Context manager for using groups in QSettings
     """
 
@@ -80,14 +80,22 @@
 
     def __exit__(
         self, exc_type: typing.Any, value: typing.Any, exc_traceback: typing.Any
     ) -> None:
         self._settings.endArray()
 
 
+def _patch_settings_from_v8(settings: QtCore.QSettings) -> None:
+    """
+    Remove
+      - DarkMode
+    """
+    settings.remove("DarkMode")
+
+
 def _patch_settings_from_v7(settings: QtCore.QSettings) -> None:
     """
     Remove
       - NewLoadingBehaviour
       - UseCompactLook
     Rename
       - DefaultRenderDirectory to DefaultRecipeDirectory
```

### Comparing `cruiz-1.4.0a3/cruiz/svggraph.py` & `cruiz-1.4.0a4/cruiz/svggraph.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/version.py` & `cruiz-1.4.0a4/cruiz/version.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/widgets/aboutcruizdialog.py` & `cruiz-1.4.0a4/cruiz/widgets/aboutcruizdialog.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/widgets/debugging.py` & `cruiz-1.4.0a4/cruiz/widgets/debugging.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/widgets/shortcutlineedit.py` & `cruiz-1.4.0a4/cruiz/widgets/shortcutlineedit.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,30 +11,30 @@
     """
     A QLineEdit specifically for capturing keyboard shortcuts
     """
 
     def keyPressEvent(self, event: QtGui.QKeyEvent) -> None:
         assert event.type() == QtCore.QEvent.KeyPress
         key = event.key()
-        if key in (  # type: ignore[comparison-overlap]
+        if key in (
             QtCore.Qt.Key_unknown,
             QtCore.Qt.Key_Control,
             QtCore.Qt.Key_Shift,
             QtCore.Qt.Key_Alt,
             QtCore.Qt.Key_Meta,
         ):
             return
-        if key == QtCore.Qt.Key_Backspace:  # type: ignore[comparison-overlap]
+        if key == QtCore.Qt.Key_Backspace:
             super().keyPressEvent(event)
             return
         modifiers = event.modifiers()
         if modifiers & QtCore.Qt.ControlModifier:
-            key += QtCore.Qt.CTRL  # type: ignore[operator]
+            key += QtCore.Qt.CTRL
         if modifiers & QtCore.Qt.ShiftModifier:
-            key += QtCore.Qt.SHIFT  # type: ignore[operator]
+            key += QtCore.Qt.SHIFT
         if modifiers & QtCore.Qt.AltModifier:
-            key += QtCore.Qt.ALT  # type: ignore[operator]
+            key += QtCore.Qt.ALT
         if modifiers & QtCore.Qt.MetaModifier:
-            key += QtCore.Qt.META  # type: ignore[operator]
+            key += QtCore.Qt.META
         sequence = QtGui.QKeySequence(key)
         self.setText(sequence.toString(QtGui.QKeySequence.PortableText))
         event.accept()
```

### Comparing `cruiz-1.4.0a3/cruiz/widgets/util.py` & `cruiz-1.4.0a4/cruiz/widgets/util.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/workers/api/__init__.py` & `cruiz-1.4.0a4/cruiz/workers/api/__init__.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/workers/utils/colorarma_conversion.py` & `cruiz-1.4.0a4/cruiz/workers/utils/colorarma_conversion.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/workers/utils/env.py` & `cruiz-1.4.0a4/cruiz/workers/utils/env.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/workers/utils/formatoptions.py` & `cruiz-1.4.0a4/cruiz/workers/utils/formatoptions.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/workers/utils/qtlogger.py` & `cruiz-1.4.0a4/cruiz/workers/utils/qtlogger.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/workers/utils/stream.py` & `cruiz-1.4.0a4/cruiz/workers/utils/stream.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,74 +11,14 @@
 import typing
 
 from .colorarma_conversion import convert_from_colorama_to_html
 
 from cruiz.interop.message import Message
 
 
-if False:
-    import io
-
-    # Conan 1.30.0+ changed the assumptions on the base-class of streams used in their
-    # runner output to be based from six, so this Python 3 implementation is no longer
-    # valid it may come back in future Conan versions that are Python 3 only
-    class QueuedStreamPy3(io.RawIOBase):
-        """
-        A stream class that uses multiprocessing.Queue to send messages
-        """
-
-        def __init__(self, queue: multiprocessing.Queue[Message], message_type):
-            super().__init__()
-            self._queue = queue
-            self._message_type = message_type
-
-        # configure the IOBase
-        def seekable(self):
-            """
-            Stream is not seekable
-            """
-            return False
-
-        def writeable(self):
-            """
-            Stream is writeable
-            """
-            # pylint: disable=no-self-use
-            return True
-
-        def readable(self):
-            """
-            Stream is not readable
-            """
-            return False
-
-        def isatty(self):
-            """
-            Stream is not interactive
-            """
-            # TODO: could this be True, which asks the queue for info?
-            return False
-
-        # implement functions of interest
-        def write(self, message):
-            """
-            Write a message.
-            """
-            lines = message.split("\n")
-            for line in lines:
-                if not line:
-                    continue
-                self._queue.put(self._message_type(convert_from_colorama_to_html(line)))
-
-        def flush(self):
-            """
-            Flush the stream.
-            """
-
-
 class QueuedStreamSix(six.StringIO):
     """
     A stream class that uses multiprocessing.Queue to send messages.
     Complete messages may be passed piecemeal, so that coloured output is generated.
     This buffers up a message, so that it is passed across the process divide as a
     single HTML paragraph.
     """
```

### Comparing `cruiz-1.4.0a3/cruiz/workers/utils/text2html.py` & `cruiz-1.4.0a4/cruiz/workers/utils/text2html.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a3/cruiz/workers/utils/worker.py` & `cruiz-1.4.0a4/cruiz/workers/utils/worker.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
     def __enter__(self) -> None:
         multiprocessing.get_logger().debug("%i (child): %s", os.getpid(), self._params)
         clear_conan_env()
         if isinstance(self._params, (CommandParameters, CommonParameters)):
             set_env(self._params.added_environment, self._params.removed_environment)
         else:
-            with contextlib.suppress(TypeError):
+            with contextlib.suppress(TypeError):  # type: ignore[unreachable]
                 # can happen for other types of *Parameters classes
                 if "env" in self._params:
                     set_env(self._params["env"], [])
 
         if self._wall_clock is not None:
             self._wall_clock.start()
```

### Comparing `cruiz-1.4.0a3/cruiz.egg-info/PKG-INFO` & `cruiz-1.4.0a4/cruiz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cruiz
-Version: 1.4.0a3
+Version: 1.4.0a4
 Summary: Conan recipe user interface
 Home-page: https://github.com/markfinal/cruiz
 Author: Mark Final
 Author-email: markfinal@hotmail.com
 Project-URL: Documentation, https://cruiz.readthedocs.io/en/latest/
 Project-URL: GitHub, https://github.com/markfinal/cruiz
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cruiz-1.4.0a3/setup.py` & `cruiz-1.4.0a4/setup.py`

 * *Files identical despite different names*

