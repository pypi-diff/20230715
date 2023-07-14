# Comparing `tmp/pydelorean-1.3.4.tar.gz` & `tmp/pydelorean-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydelorean-1.3.4.tar", last modified: Sun Jul  9 03:07:34 2023, max compression
+gzip compressed data, was "pydelorean-1.3.5.tar", last modified: Fri Jul 14 22:25:34 2023, max compression
```

## Comparing `pydelorean-1.3.4.tar` & `pydelorean-1.3.5.tar`

### file list

```diff
@@ -1,28 +1,27 @@
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-09 03:07:34.465197 pydelorean-1.3.4/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)    11358 2023-06-10 12:13:51.000000 pydelorean-1.3.4/LICENSE
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2340 2023-07-09 03:07:34.465197 pydelorean-1.3.4/PKG-INFO
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1916 2023-07-09 02:55:02.000000 pydelorean-1.3.4/README.rst
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-09 03:07:34.462197 pydelorean-1.3.4/pydelorean/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1572 2023-07-09 03:00:29.000000 pydelorean-1.3.4/pydelorean/__init__.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     4186 2023-07-09 02:52:51.000000 pydelorean-1.3.4/pydelorean/delorean.py
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-09 03:07:34.464197 pydelorean-1.3.4/pydelorean/parser/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       22 2023-06-10 12:14:10.000000 pydelorean-1.3.4/pydelorean/parser/__init__.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1647 2023-07-09 02:54:21.000000 pydelorean-1.3.4/pydelorean/parser/parser.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     6011 2023-07-09 02:53:43.000000 pydelorean-1.3.4/pydelorean/parser/utils.py
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-09 03:07:34.464197 pydelorean-1.3.4/pydelorean/tools/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2533 2023-07-09 02:44:26.000000 pydelorean-1.3.4/pydelorean/tools/__init__.py
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-09 03:07:34.465197 pydelorean-1.3.4/pydelorean/tree/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       41 2023-07-09 02:51:08.000000 pydelorean-1.3.4/pydelorean/tree/__init__.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1495 2023-07-09 02:52:16.000000 pydelorean-1.3.4/pydelorean/tree/forest.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1917 2023-07-09 02:43:36.000000 pydelorean-1.3.4/pydelorean/tree/node.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      329 2023-07-09 02:43:36.000000 pydelorean-1.3.4/pydelorean/utils.py
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-09 03:07:34.463197 pydelorean-1.3.4/pydelorean.egg-info/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2340 2023-07-09 03:07:34.000000 pydelorean-1.3.4/pydelorean.egg-info/PKG-INFO
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      475 2023-07-09 03:07:34.000000 pydelorean-1.3.4/pydelorean.egg-info/SOURCES.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        1 2023-07-09 03:07:34.000000 pydelorean-1.3.4/pydelorean.egg-info/dependency_links.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       32 2023-07-09 03:07:34.000000 pydelorean-1.3.4/pydelorean.egg-info/requires.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       11 2023-07-09 03:07:34.000000 pydelorean-1.3.4/pydelorean.egg-info/top_level.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       38 2023-07-09 03:07:34.465197 pydelorean-1.3.4/setup.cfg
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      971 2023-07-09 03:07:27.000000 pydelorean-1.3.4/setup.py
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-09 03:07:34.465197 pydelorean-1.3.4/tests/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1198 2023-06-11 13:13:52.000000 pydelorean-1.3.4/tests/test_mdtree.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-14 22:25:34.370834 pydelorean-1.3.5/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)    11358 2023-05-11 12:19:37.000000 pydelorean-1.3.5/LICENSE
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2422 2023-07-14 22:25:34.370834 pydelorean-1.3.5/PKG-INFO
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1979 2023-07-10 10:39:31.000000 pydelorean-1.3.5/README.rst
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-14 22:25:34.370834 pydelorean-1.3.5/pydelorean/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1602 2023-07-10 10:39:31.000000 pydelorean-1.3.5/pydelorean/__init__.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     3887 2023-07-10 10:39:31.000000 pydelorean-1.3.5/pydelorean/delorean.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      191 2023-07-10 10:39:31.000000 pydelorean-1.3.5/pydelorean/errors.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      604 2023-07-10 10:39:31.000000 pydelorean-1.3.5/pydelorean/files.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-14 22:25:34.370834 pydelorean-1.3.5/pydelorean/parser/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       96 2023-07-10 10:39:31.000000 pydelorean-1.3.5/pydelorean/parser/__init__.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1702 2023-07-14 11:46:04.000000 pydelorean-1.3.5/pydelorean/parser/parser.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     4391 2023-07-14 11:46:04.000000 pydelorean-1.3.5/pydelorean/parser/utils.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-14 22:25:34.370834 pydelorean-1.3.5/pydelorean/tools/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2397 2023-07-14 22:23:49.000000 pydelorean-1.3.5/pydelorean/tools/__init__.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-14 22:25:34.370834 pydelorean-1.3.5/pydelorean/tree/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       41 2023-07-10 10:39:31.000000 pydelorean-1.3.5/pydelorean/tree/__init__.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1495 2023-07-10 10:39:31.000000 pydelorean-1.3.5/pydelorean/tree/forest.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1829 2023-07-14 11:46:04.000000 pydelorean-1.3.5/pydelorean/tree/node.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-14 22:25:34.370834 pydelorean-1.3.5/pydelorean.egg-info/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2422 2023-07-14 22:25:34.000000 pydelorean-1.3.5/pydelorean.egg-info/PKG-INFO
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      475 2023-07-14 22:25:34.000000 pydelorean-1.3.5/pydelorean.egg-info/SOURCES.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        1 2023-07-14 22:25:34.000000 pydelorean-1.3.5/pydelorean.egg-info/dependency_links.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       32 2023-07-14 22:25:34.000000 pydelorean-1.3.5/pydelorean.egg-info/requires.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       11 2023-07-14 22:25:34.000000 pydelorean-1.3.5/pydelorean.egg-info/top_level.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       38 2023-07-14 22:25:34.370834 pydelorean-1.3.5/setup.cfg
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      971 2023-07-14 22:25:20.000000 pydelorean-1.3.5/setup.py
```

### Comparing `pydelorean-1.3.4/LICENSE` & `pydelorean-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pydelorean-1.3.4/pydelorean/__init__.py` & `pydelorean-1.3.5/pydelorean/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 from bs4 import BeautifulSoup
-from .delorean import mdtreeify, findMetadata
+from .delorean import *
 from .tree import Forest
 import re
 
-def treeify(name:str, md:str, *args, **kwargs) -> Forest:
-    
-    return mdtreeify(name, md, *args, **kwargs)
 
-# def markdownify(tree:MarkdownForest, *args, **kwargs) -> str:
-#     """_summary_
+# TODO: Check the type of the input and call the appropriate function
+# Use the newly defined File classes for this. 
+def treeify(name:str, text:str, *args, **kwargs) -> Forest:
+    
+    return mdtreeify(name, text, *args, **kwargs)
 
-#     Args:
-#         tree (MarkdownForest): _description_
 
-#     Returns:
-#         str: _description_
-#     """
+def textify(forest:Forest, *args, **kwargs) -> str:
     
-#     return mdtextify(tree, *args, **kwargs)
+    return mdtextify(forest)
+
 
+# TODO: I want to only expose treeify and textify to the user. Move this someplace else.
 def clean_markdown(md:str) -> str:
         
     # Remove the metadata
-    _, markdown_text = findMetadata(md)
+    _, markdown_text = find_metadata(md)
     
      # Create a BeautifulSoup object with the input markdown text
     soup = BeautifulSoup(markdown_text, 'html.parser')
 
     # Remove HTML tags from the document
     markdown_text = soup.get_text()
```

### Comparing `pydelorean-1.3.4/pydelorean/delorean.py` & `pydelorean-1.3.5/pydelorean/delorean.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,86 +1,73 @@
 """ This file contains the main functions for the delorean package.
 """
     
 import re
 
 import frontmatter
-from .utils import *
+from .files import *
 from .tree import *
 from .parser import *
 
 # ==================================================================================================
 #                                           TREEIFY
 # ==================================================================================================
 
 # TODO: Rename to snake_case in the future.
 
 
-def findBacklinks(input_text:str) -> list:
+def find_backlinks(input_text:str) -> list:
     """ 
     Function to find all backlinks in a given text.
     """
     
     backlinks = []
 
     # Regular expression pattern to match backlinks
     pattern = r'\[\[(.*?)\]\]'
     backlinks = re.findall(pattern, input_text)
     return backlinks
 
 
-def findTags(input_text:str) -> list:
+def find_tags(input_text:str) -> list:
     """
     Function to find all tags in a given text.
     """
     
     tags = []
 
     # Regular expression pattern to match backlinks
     pattern = r'#([a-zA-Z0-9_]+)'
     tags = re.findall(pattern, input_text)
     return tags
 
 
-def findMetadata(input_text:str):
+def find_metadata(input_text:str):
     post = frontmatter.loads(input_text)
     return post.metadata, post.content
 
 
 def mdtreeify(name:str, md:str, *args, **kwargs) -> MarkdownForest:
     """
     Converts markdown file to a MarkdownForest
     """
     
-    meta, cont = findMetadata(md)
+    meta, cont = find_metadata(md)
     
-    backlinks = findBacklinks(cont)
-    tags = findTags(cont)
+    backlinks = find_backlinks(cont)
+    tags = find_tags(cont)
     
     if cont == "":
         # If the file is empty, just create a root node
-        tree = Tree()
-        tree.create_node(tag=name, identifier="root").identifier
-    else:
-        # Based on the file type specified by the user, choose a parser
-        if 'type' in kwargs:
-            if kwargs['type'] == FileType.MARKDOWN:
-                parser = MarkdownParser(name, cont)
-            elif kwargs['type'] == FileType.RESTRUCTUREDTEXT:
-                parser = RestructuredParser(name, cont)
-            elif kwargs['type'] == FileType.TXT:
-                parser = TextParser(name, cont)
-            elif kwargs['type'] == FileType.YAML:
-                parser = YAMLParser(name, cont)
-            else:
-                raise ValueError("Invalid file type.")
-        else:
-            parser = MarkdownParser(name, cont)
-            
-        tree = parser.parse()
+        tree = Node("root")
+        return tree
+    
+    
+    parser = MarkdownParser(name, cont)
+    tree = parser.parse()
     
     returnForest = MarkdownForest(tree, name, metadata=meta)
     
     for backlink in backlinks:
         returnForest.add_backlink(backlink)
     for tag in tags:
         returnForest.add_tag(tag)
@@ -104,40 +91,74 @@
     pass
 
 
 # ==================================================================================================
 #                                           TEXTIFY
 # ==================================================================================================
 
-def convertRootToText(rootNode: HeaderNode) -> str:
+
+def header_node_to_text(rootNode: HeaderNode) -> str:
     
     # BASE CASE: We just have text node.
     if isinstance(rootNode, TextNode):
-        return repr(rootNode) + "\n"
+        return rootNode.text + "\n\n"
     
     # For the header node
-    headerLevel = rootNode.get_header_level()
-    returnString = '#'*headerLevel + " " + str(rootNode) + "\n"
-    for _, child in enumerate(rootNode):
-        returnString += convertRootToText(child)
+    headerLevel = rootNode.header_level
+    returnString = str(rootNode) + "\n"
+    for _, child in enumerate(rootNode.children):
+        returnString += header_node_to_text(child)
     
     return returnString    
      
-def convertDictToMetadata(metadata:dict) -> str:
+
+def convert_to_metadata(metadata_dict:dict) -> str:
     yaml = "---\n"
-    for key, value in metadata.items():
+    for key, value in metadata_dict.items():
+        
         if isinstance(value, list):
             yaml += f"{key}: \n"
             for elem in value:
                 yaml += f"  - {elem}\n"
             continue
+        
         yaml += f"{key}: {value}\n"
     yaml += "---\n"
     return yaml
 
-# FIXME: Change the mdtextify implenmentation to use the new tree structure.
-# def mdtextify(forest:MarkdownForest, *args, **kwargs) -> str:
+
+def mdtextify(forest: MarkdownForest) -> str:
+    """
+    Converts a MarkdownForest to a markdown file.
+    """
     
-#     finalText = convertDictToMetadata(forest.metadata)
-#     for i, tree in enumerate(forest):
-#         finalText += convertRootToText(tree.get_root())
-#     return finalText
+    returnString = ""
+    
+    # Get the root node
+    root = forest.root
+    
+    # Get the metadata
+    metadata = forest.get_metadata()
+    returnString = convert_to_metadata(metadata) + "\n"
+    
+    for node in root.children:
+        returnString += header_node_to_text(node) + "\n"
+    
+    return returnString
+
+
+def rsttextify(forest: RestructuredForest) -> str:
+    
+    pass
+
+
+def asciidoctextify(forest: AsciidocForest) -> str:
+    pass
+
+
+def yamltextify(forest: YamlForest) -> str:
+    pass
+
+
+def jsontextify(forest: JSONForest) -> str:
+    pass
+
```

### Comparing `pydelorean-1.3.4/pydelorean/parser/parser.py` & `pydelorean-1.3.5/pydelorean/parser/parser.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,27 +14,27 @@
     
     def __init__(self, document_name:str, text:str):
         super().__init__(document_name, text)
         
     def parse(self) -> Node:
         HEADER_PATTERN = r"^(#+\s+)(.*)"
         
-        tree = buildTree(self.text, self.document_name, header_pattern=HEADER_PATTERN)
+        tree = build_tree(self.text, document_name=self.document_name, header_pattern=HEADER_PATTERN)
         return tree
         
 
 class RestructuredParser(Parser):
     
     def __init__(self, document_name:str, text:str):
         super().__init__(document_name, text)
         
     def parse(self) -> Node:
-        HEADER_PATTERN = r'^(\S.*)\n[=~`\'^"-]+$'
+        HEADER_PATTERN = r"^(=+|-+|`+|'+|\^+|\*+|\.+|~+|\++)\s+(.+)\s+\1$"
         
-        tree = buildTree(self.text, self.document_name, header_pattern=HEADER_PATTERN)
+        tree = build_tree(self.text, document_name=self.document_name, header_pattern=HEADER_PATTERN)
         return tree
         
 
 class TextParser(Parser):
     
     def __init__(self, document_name:str, text:str):
         super().__init__(document_name, text)
```

### Comparing `pydelorean-1.3.4/pydelorean/tools/__init__.py` & `pydelorean-1.3.5/pydelorean/tools/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,59 +1,74 @@
-from pydelorean.tree.node import TextNode
+from pydelorean.tree.node import *
+from pydelorean import treeify
 
 def get_progressive_expansion(node, **kwargs) -> list:
     
     # BASE CASE: TextNode
     if isinstance(node, TextNode):
-        return [(node.text, "")]
+        return [(node.corpus, node.corpus)]
     
-    header = node.header
-    children = node.children
-    returned_list = []
-    final_corpus = ""
-    for child in children:
-        child_corpus = get_progressive_expansion(child)
-        for child in child_corpus:
-            text = child[0] + "\n" + child[1]
-            returned_list.append((header, text))
-            final_corpus += "\n" + text
-    
-    if 'append' in kwargs and kwargs['append']:
-        returned_list.append((header, final_corpus))
-    return returned_list
+    if kwargs.get("append", False):
+        returned_list = [(node.header, node.corpus)]
+    else:
+        returned_list = []
+    for child in node.children:
+        if isinstance(child, HeaderNode):
+            child_list = get_progressive_expansion(child, append=True)
+            returned_list += [(child.header, para) for header, para in child_list]
+        elif isinstance(child, TextNode):
+            returned_list.append((node.header, child.corpus))
         
-    
-text = """
-# Appendices
+    return returned_list
+
+
+# text = """
+# ---
+# author: Keane Moraes
+# id: 1
+# tags:
+# - dune
+# - ecology
+# - fremen
+# - religion
+# - desert
+# ---
+
+# # Appendices
+
+# The appendix begins with an epigraph by Pardot Kynes in which he considers the kind of existence available when humans increase in number in a finite environment.
+
+# ## Appendix I: The Ecology of Dune.
+# This appendix details “the ecology of Dune.” It is heavily focused on the story of Pardot Kynes, Arrakis's first planetologist.
+
+# ## Appendix II: The Religion of Dune.
+# Before the coming of [[Muad'Dib]], the Fremen of Arrakis practiced a religion whose roots in the Maometh Saari are there for any scholar to see.
 
-The appendix begins with an epigraph by Pardot Kynes in which he considers the kind of existence available when humans increase in number in a finite environment.
+# ## Appendix III: Report on Bene Gesserit Motives and Purposes.
+# This appendix details a “report on Bene Gesserit motives and purpose.”
+# The narrator introduces it by noting that Lady Jessica commissioned the report directly after the “Arrakis Affair.” 
 
-## Appendix I: The Ecology of Dune.
-This appendix details “the ecology of Dune.” It is heavily focused on the story of Pardot Kynes, Arrakis's first planetologist.
+# ### Narratives
+# The document is noted as being extremely honest in tone.
 
-## Appendix II: The Religion of Dune.
-Before the coming of [[Muad'Dib]], the Fremen of Arrakis practiced a religion whose roots in the Maometh Saari are there for any scholar to see. Many have traced the extensive borrowings from other religions. The most common example is the Hymn to Water, a direct copy from the Orange Catholic Liturgical Manual, calling for rain clouds which Arrakis had never seen. But there are more profound points of accord between the Kitab al-Ibar of the Fremen and the teachings of Bible, Ilm, and Fiqh.
+# ## Appendix IV: The Almanak eb-Ashraf (Selected Excerpts of the Noble Houses)
+# This appendix details selected excerpts about the noble Houses of Dune. The first entry discusses the Padishah Emperor Shaddam IV of House Corrino. His rule is most significant for the “Arrakis Revolt,” which historians ascribe to his poor court politics. 
 
-## Appendix III: Report on Bene Gesserit Motives and Purposes.
-This appendix details a “report on Bene Gesserit motives and purpose.”
-The narrator introduces it by noting that Lady Jessica commissioned the report directly after the “Arrakis Affair.” 
+# # Terminology of the Imperium
 
-### Narratives
-The document is noted as being extremely honest in tone.
+# Hello there
 
-## Appendix IV: The Almanak eb-Ashraf (Selected Excerpts of the Noble Houses)
-This appendix details selected excerpts about the noble Houses of Dune. The first entry discusses the Padishah Emperor Shaddam IV of House Corrino. His rule is most significant for the “Arrakis Revolt,” which historians ascribe to his poor court politics. 
+# ## Another One
 
-# Terminology of the Imperium
+# asdfas
+# """
 
-Hello there
+# forest = treeify("dune_appendices.md", text)
 
-## Another One
-asda
-"""
+# root = forest.root
+# header1 = root.children[0]
 
-# tree = treeify("appendices of dune", text)
+# ans = get_progressive_expansion(root, append=True)
 
-# headerlist = get_progressive_expansion(tree.root.children[0], append=True)
-# for pair in headerlist:
-#     print(pair)
-#     print("------------------")
+# for i in ans:
+#     print(i)
+#     print("==================================")
```

### Comparing `pydelorean-1.3.4/pydelorean/tree/forest.py` & `pydelorean-1.3.5/pydelorean/tree/forest.py`

 * *Files identical despite different names*

### Comparing `pydelorean-1.3.4/pydelorean/tree/node.py` & `pydelorean-1.3.5/pydelorean/tree/node.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,17 @@
 """_summary_
 
 """
 
-from bigtree import BaseNode, Node
+from bigtree import Node
 
 # TODO: Add all the documentation and convert to snake case soon.
 
 
 class TextNode(Node):
-    """_summary_
-
-    Args:
-        Node (_type_): _description_
-
-    Raises:
-        IndexError: _description_
-
-    Returns:
-        _type_: _description_
-    """
     
     FRACTION_PRINTABLE = 0.25
     
     def __init__(self, name:str, text:str, **kwargs):
         self.text = text
         super().__init__(name, **kwargs)
         
@@ -38,49 +27,49 @@
     def __repr__(self) -> str:
         return "(Text) " + self.text[0:min(10, int(self.FRACTION_PRINTABLE * len(self.text)))] + " ..."
     
     @property
     def text(self):
         return self._text
     
+    @property
+    def corpus(self):
+        return self._text
+    
     @text.setter
     def text(self, text:str):
         self._text = text
 
 
 class HeaderNode(Node):
-    """_summary_
-
-    Args:
-        Node (_type_): _description_
-    """
     
-    def __init__(self, name:str, header:str, headerNumber:int, **kwargs):
+    def __init__(self, header:str, headerNumber:int, **kwargs):
         self.header = header
-        self.headerNumber = headerNumber
-        self.name = header
-        self.corpus = []
-        super().__init__(name, **kwargs)
+        self._header_level = headerNumber
+        self._corpus = []
+        super().__init__(header, **kwargs)
         
     def __str__(self):
         return self.header
     
     def __repr__(self):
-        return f"(h{self.headerNumber}) {self.header}"
+        return f"(h{self._header_level}) {self.header}"
     
     @property
-    def headerLevel(self) -> int:
-        return self.headerNumber
+    def header_level(self) -> int:
+        return self._header_level
     
-    @headerLevel.setter
-    def headerLevel(self, headerNumber:int) -> None:
-        self._headerNumber = headerNumber
-        
-    def get_corpus(self) -> list:
-        return self.corpus
-    
-    def add_to_corpus(self, text:str) -> None:
-        self.corpus.append(text)
-
-
+    @header_level.setter
+    def header_level(self, headerNumber:int) -> None:
+        self._header_level = headerNumber
 
+    def __pow__(self, other):
+        self._corpus.append(other)
+        
+    @property
+    def corpus(self) -> str:
+        final_text = self.header + "\n"
+        for child in self._corpus:
+            final_text += child.corpus + "\n"
+        return final_text    
 
+
```

### Comparing `pydelorean-1.3.4/setup.py` & `pydelorean-1.3.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 from setuptools.command.test import test as TestCommand
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 LONG_DESCRIPTION = (this_directory / "README.rst").read_text()
 
-VERSION = '1.3.4'
+VERSION = '1.3.5'
 DESCRIPTION = 'A package to convert between markup language documents and a forest data structure for efficient processing.'
 
 setup(
     name = "pydelorean",
     version = VERSION,
     author = "Keane Moraes",
     author_email = 'lordvader3002@gmail.com',
```

