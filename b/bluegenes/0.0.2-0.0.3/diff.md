# Comparing `tmp/bluegenes-0.0.2.tar.gz` & `tmp/bluegenes-0.0.3.tar.gz`

## Comparing `bluegenes-0.0.2.tar` & `bluegenes-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,15 @@
--rw-r--r--   0        0        0    15553 2020-02-02 00:00:00.000000 bluegenes-0.0.2/dox.md
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 bluegenes-0.0.2/bluegenes/__init__.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 bluegenes-0.0.2/bluegenes/errors.py
--rw-r--r--   0        0        0    34993 2020-02-02 00:00:00.000000 bluegenes-0.0.2/bluegenes/genes.py
--rw-r--r--   0        0        0    11188 2020-02-02 00:00:00.000000 bluegenes-0.0.2/bluegenes/optimization.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 bluegenes-0.0.2/tests/context.py
--rw-r--r--   0        0        0    42027 2020-02-02 00:00:00.000000 bluegenes-0.0.2/tests/test_genes.py
--rw-r--r--   0        0        0    17954 2020-02-02 00:00:00.000000 bluegenes-0.0.2/tests/test_optimization.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 bluegenes-0.0.2/.gitignore
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 bluegenes-0.0.2/license
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 bluegenes-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 bluegenes-0.0.2/readme.md
--rw-r--r--   0        0        0     5184 2020-02-02 00:00:00.000000 bluegenes-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    15559 2020-02-02 00:00:00.000000 bluegenes-0.0.3/dox.md
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 bluegenes-0.0.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 bluegenes-0.0.3/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 bluegenes-0.0.3/bluegenes/__init__.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 bluegenes-0.0.3/bluegenes/errors.py
+-rw-r--r--   0        0        0    34999 2020-02-02 00:00:00.000000 bluegenes-0.0.3/bluegenes/genes.py
+-rw-r--r--   0        0        0    11188 2020-02-02 00:00:00.000000 bluegenes-0.0.3/bluegenes/optimization.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 bluegenes-0.0.3/tests/context.py
+-rw-r--r--   0        0        0    42156 2020-02-02 00:00:00.000000 bluegenes-0.0.3/tests/test_genes.py
+-rw-r--r--   0        0        0    18166 2020-02-02 00:00:00.000000 bluegenes-0.0.3/tests/test_optimization.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 bluegenes-0.0.3/.gitignore
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 bluegenes-0.0.3/license
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 bluegenes-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     4737 2020-02-02 00:00:00.000000 bluegenes-0.0.3/readme.md
+-rw-r--r--   0        0        0     5357 2020-02-02 00:00:00.000000 bluegenes-0.0.3/PKG-INFO
```

### Comparing `bluegenes-0.0.2/dox.md` & `bluegenes-0.0.3/dox.md`

 * *Files 2% similar despite different names*

```diff
@@ -103,15 +103,15 @@
 
 ##### `substitute(index: int, gene: Gene, n_bases: int, max_base_size: int, base_factory: Callable[[None], int | float | str], factory_args: list = None, factory_kwargs: dict = None) -> Allele:` 
 
 Substitutes the Gene at the index with the given gene. If index is None, a
 random index will be used. If gene is None, adds a random gene using Gene.make,
 passing the kwargs. Returns self for chaining operations.
 
-##### `recombine(other: Allele, indices: list[int] = None, recombine_genes: bool = True, match_genes: bool = True) -> Allele:` 
+##### `recombine(other: Allele, indices: list[int] = None, recombine_genes: bool = True, match_genes: bool = False) -> Allele:` 
 
 Recombines with the other Allele, swapping at the given indices. If indices is
 None, between 1 and ceil(log(len(self.genes))) random indices will be chosen.
 Recombines individual Genes if recombine_genes is True. Recombines only Genes
 with matching names if match_genes is True. Returns the new Allele.
 
 ##### `@classmethod make(n_genes: int, n_bases: int, name: str, max_base_size: int, base_factory: Callable[[None], int | float | str], factory_args: list, factory_kwargs: dict) -> Allele:` 
@@ -163,15 +163,15 @@
 
 ##### `substitute(index: int, allele: Allele, n_genes: int, n_bases: int, max_base_size: int, base_factory: Callable[[None], int | float | str], factory_args: list = None, factory_kwargs: dict = None) -> Chromosome:` 
 
 Substitutes the Allele at the index with the given allele. If index is None, a
 random index will be used. If allele is None, adds a random allele using
 Allele.make, passing the kwargs. Returns self for chaining operations.
 
-##### `recombine(other: Chromosome, indices: list[int] = None, recombine_alleles: bool = True, match_alleles: bool = True, recombine_genes: bool = True, match_genes: bool = True) -> Chromosome:` 
+##### `recombine(other: Chromosome, indices: list[int] = None, recombine_alleles: bool = True, match_alleles: bool = False, recombine_genes: bool = True, match_genes: bool = False) -> Chromosome:` 
 
 Recombines with the other Chromosome, swapping at the given indices. If indices
 is None, between 1 and ceil(log(len(self.alleles))) random indices will be
 chosen. Recombines individual Alleles if recombine_allels is True. Recombines
 only Alleles with matching names if match_alleles is True. Recombines individual
 Genes if recombine_genes is True. Recombines only Genes with matching names if
 match_genes is True. Returns the new Chromosome.
@@ -226,15 +226,15 @@
 ##### `substitute(index: int, chromosome: Chromosome, n_alleles: int, n_genes: int, n_bases: int, max_base_size: int, base_factory: Callable[[None], int | float | str], factory_args: list = None, factory_kwargs: dict = None) -> Genome:` 
 
 Substitutes the Chromosome at the index with the given chromosome. If index is
 None, a random index will be used. If chromosome is None, adds a random
 chromosome using Chromosome.make, passing the kwargs. Returns self for chaining
 operations.
 
-##### `recombine(other: Genome, indices: list[int] = None, recombine_chromosomes: bool = True, match_chromosomes: bool = True, recombine_alleles: bool = True, match_alleles: bool = True, recombine_genes: bool = True, match_genes: bool = True) -> Genome:` 
+##### `recombine(other: Genome, indices: list[int] = None, recombine_chromosomes: bool = True, match_chromosomes: bool = False, recombine_alleles: bool = True, match_alleles: bool = False, recombine_genes: bool = True, match_genes: bool = False) -> Genome:` 
 
 Recombines with the other Genome, swapping at the given indices. If indices is
 None, between 1 and ceil(log(len(self.chromosomes))) random indices will be
 chosen. Recombines individual Chromosomes if recombine_chromosomes is True.
 Recombines only Chromosomes with matching names if match_chromosomes is True.
 Recombines individual Alleles if recombine_alleles is True. Recombines only
 Alleles with matching names if match_alleles is True. Recombines individual
```

### Comparing `bluegenes-0.0.2/bluegenes/errors.py` & `bluegenes-0.0.3/bluegenes/errors.py`

 * *Files identical despite different names*

### Comparing `bluegenes-0.0.2/bluegenes/genes.py` & `bluegenes-0.0.3/bluegenes/genes.py`

 * *Files 0% similar despite different names*

```diff
@@ -270,15 +270,15 @@
         typert(gene, Gene, "gene")
 
         self.genes[index] = gene
         return self
 
     def recombine(self, other: Allele, indices: list[int] = None,
                   recombine_genes: bool = True,
-                  match_genes: bool = True) -> Allele:
+                  match_genes: bool = False) -> Allele:
         """Recombines with the other Allele, swapping at the given
             indices. If indices is None, between 1 and ceil(log(len(self.genes)))
             random indices will be chosen. Recombines individual Genes
             if recombine_genes is True. Recombines only Genes with
             matching names if match_genes is True. Returns the new
             Allele.
         """
@@ -458,16 +458,16 @@
             )
         typert(allele, Allele, "allele")
 
         self.alleles[index] = allele
         return self
 
     def recombine(self, other: Chromosome, indices: list[int] = None,
-                  recombine_alleles: bool = True, match_alleles: bool = True,
-                  recombine_genes: bool = True, match_genes: bool = True
+                  recombine_alleles: bool = True, match_alleles: bool = False,
+                  recombine_genes: bool = True, match_genes: bool = False
                   ) -> Chromosome:
         """Recombines with the other Chromosome, swapping at the given
             indices. If indices is None, between 1 and ceil(log(len(self.alleles)))
             random indices will be chosen. Recombines individual Alleles
             if recombine_allels is True. Recombines only Alleles with
             matching names if match_alleles is True. Recombines
             individual Genes if recombine_genes is True. Recombines only
@@ -682,17 +682,17 @@
         typert(chromosome, Chromosome, "chromosome")
 
         self.chromosomes[index] = chromosome
         return self
 
     def recombine(self, other: Genome, indices: list[int] = None,
                   recombine_chromosomes: bool = True,
-                  match_chromosomes: bool = True,
-                  recombine_alleles: bool = True, match_alleles: bool = True,
-                  recombine_genes: bool = True, match_genes: bool = True
+                  match_chromosomes: bool = False,
+                  recombine_alleles: bool = True, match_alleles: bool = False,
+                  recombine_genes: bool = True, match_genes: bool = False
                   ) -> Genome:
         """Recombines with the other Genome, swapping at the given
             indices. If indices is None, between 1 and
             ceil(log(len(self.chromosomes))) random indices will be
             chosen. Recombines individual Chromosomes
             if recombine_chromosomes is True. Recombines only
             Chromosomes with matching names if match_chromosomes is True.
```

### Comparing `bluegenes-0.0.2/bluegenes/optimization.py` & `bluegenes-0.0.3/bluegenes/optimization.py`

 * *Files identical despite different names*

### Comparing `bluegenes-0.0.2/tests/test_genes.py` & `bluegenes-0.0.3/tests/test_genes.py`

 * *Files 1% similar despite different names*

```diff
@@ -315,27 +315,27 @@
                     swaps.append(i)
                 elif al3.genes[i] == al2.genes[i]:
                     swapped = True
                     swaps.append(i)
             swapset.add(tuple(swaps))
         assert len(swapset) >= 2
 
-    def test_recombine_recombines_underlying_Genes_with_matching_name_and_index_by_default(self):
-        allele = self.allele.recombine(self.alternate, [1])
+    def test_recombine_recombines_underlying_Genes_with_different_name_and_index_by_default(self):
+        allele = self.allele.recombine(self.other, [1])
         recombined_genes = 0
         allele_bases = [b for g in self.allele.genes for b in g.bases]
-        other_bases = [b for g in self.alternate.genes for b in g.bases]
+        other_bases = [b for g in self.other.genes for b in g.bases]
         for g in allele.genes:
             if g not in self.allele.genes and g not in self.alternate.genes:
                 recombined_genes += 1
             assert all(b in allele_bases or b in other_bases for b in g.bases)
         assert recombined_genes >= 1
 
-    def test_recombine_does_not_recombine_underlying_Genes_with_different_names_by_default(self):
-        allele = self.allele.recombine(self.other, [1])
+    def test_recombine_does_not_recombine_underlying_Genes_with_different_names_when_specified(self):
+        allele = self.allele.recombine(self.other, [1], match_genes=True)
         recombined_genes = 0
         for g in allele.genes:
             if g not in self.allele.genes and g not in self.other.genes:
                 recombined_genes += 1
         assert recombined_genes == 0
 
     def test_recombine_can_recombine_underlying_Genes_with_different_names(self):
@@ -558,15 +558,15 @@
         al3 = self.chromosome.recombine(self.other, [1], False)
         assert al3.alleles == [self.chromosome.alleles[0], *self.other.alleles[1:]]
 
         swapset = set()
         for _ in range(10):
             ch1 = self.first_chromosome()
             ch2 = self.second_chromosome()
-            ch3 = ch1.recombine(ch2, recombine_genes=False)
+            ch3 = ch1.recombine(ch2, match_alleles=True, recombine_genes=False)
             swapped = False
             swaps = []
             for i in range(len(ch3.alleles)):
                 if swapped and ch3.alleles[i] == ch1.alleles[i]:
                     swapped = False
                     swaps.append(i)
                 elif ch3.alleles[i] == ch2.alleles[i]:
@@ -592,16 +592,16 @@
                 if g not in main_genes and g not in other_genes:
                     recombined_genes += 1
                 assert g.name in main_gene_names or g.name in other_gene_names
                 assert all(b in main_bases or b in other_bases for b in g.bases)
         assert recombined_alleles >= 1
         assert recombined_genes >= 1
 
-    def test_recombine_does_not_recombine_underlying_Alleles_or_Genes_with_different_names_by_default(self):
-        chromosome = self.chromosome.recombine(self.other, [1])
+    def test_recombine_does_not_recombine_underlying_Alleles_or_Genes_with_different_names_when_specified(self):
+        chromosome = self.chromosome.recombine(self.other, [1], match_alleles=True)
         main_genes = [g for a in self.chromosome.alleles for g in a.genes]
         other_genes = [b for g in self.other.alleles for b in g.genes]
         recombined_alleles = 0
         recombined_genes = 0
 
         for a in chromosome.alleles:
             if a not in self.chromosome.alleles and a not in self.other.alleles:
@@ -891,15 +891,15 @@
         gm3 = self.genome.recombine(self.other, [1], False)
         assert gm3.chromosomes == [self.genome.chromosomes[0], *self.other.chromosomes[1:]]
 
         swapset = set()
         for _ in range(10):
             gm1 = self.first_genome()
             gm2 = self.second_genome()
-            gm3 = gm1.recombine(gm2, recombine_alleles=False)
+            gm3 = gm1.recombine(gm2, recombine_chromosomes=False)
             swapped = False
             swaps = []
             for i in range(len(gm3.chromosomes)):
                 if swapped and gm3.chromosomes[i] == gm1.chromosomes[i]:
                     swapped = False
                     swaps.append(i)
                 elif gm3.chromosomes[i] == gm2.chromosomes[i]:
@@ -932,16 +932,16 @@
                         recombined_genes += 1
                     assert g.name in main_gene_names or g.name in other_gene_names
                     assert all(b in main_bases or b in other_bases for b in g.bases)
         assert recombined_chromosomes >= 1
         assert recombined_alleles >= 1
         assert recombined_genes >= 1
 
-    def test_recombine_does_not_recombine_underlying_Chromosomes_or_Genes_with_different_names_by_default(self):
-        genome = self.genome.recombine(self.other, [1])
+    def test_recombine_does_not_recombine_underlying_Chromosomes_or_Genes_with_different_names_when_specified(self):
+        genome = self.genome.recombine(self.other, [1], match_chromosomes=True, match_alleles=True, match_genes=True)
         main_alleles = [a for c in self.genome.chromosomes for a in c.alleles]
         main_genes = [g for a in main_alleles for g in a.genes]
         other_alleles = [a for c in self.other.chromosomes for a in c.alleles]
         other_genes = [g for a in other_alleles for g in a.genes]
         recombined_chromosomes = 0
         recombined_alleles = 0
         recombined_genes = 0
```

### Comparing `bluegenes-0.0.2/tests/test_optimization.py` & `bluegenes-0.0.3/tests/test_optimization.py`

 * *Files 2% similar despite different names*

```diff
@@ -452,18 +452,22 @@
         target = 123
         def measure_fitness(gene: genes.Gene):
             return 1 / (1 + abs(sum(gene.bases) - target))
 
         def mutate_gene(gene: genes.Gene) -> genes.Gene:
             for i in range(len(gene.bases)):
                 val = random()
-                if val <= 0.5:
-                    gene.bases[i] += randint(0, 10)
+                if val <= 0.1:
+                    gene.bases[i] = int(gene.bases[i] / randint(1, 3))
+                elif val <= 0.2:
+                    gene.bases[i] = int(gene.bases[i] * randint(1, 3))
+                elif val <= 0.6:
+                    gene.bases[i] += randint(0, 11)
                 else:
-                    gene.bases[i] -= randint(0, 10)
+                    gene.bases[i] -= randint(0, 11)
             return gene
 
         optimization.set_hook(hook)
         count, _ = optimization.optimize_gene(
             measure_fitness, mutate_gene, max_iterations=100
         )
```

### Comparing `bluegenes-0.0.2/license` & `bluegenes-0.0.3/license`

 * *Files identical despite different names*

### Comparing `bluegenes-0.0.2/pyproject.toml` & `bluegenes-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "bluegenes"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="k98kurz", email="k98kurz@gmail.com" },
 ]
 description = "Working-man's library for genetic algorithms"
 readme = "readme.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `bluegenes-0.0.2/readme.md` & `bluegenes-0.0.3/readme.md`

 * *Files 4% similar despite different names*

```diff
@@ -76,26 +76,30 @@
     """Produces a fitness score. Passed as parameter to optimize_gene."""
     return 1 / (1 + abs(sum(gene.bases) - target))
 
 def mutate_gene(gene: Gene) -> Gene:
     """Mutates the Gene randomly. Passed as parameter to optimize_gene."""
     for i in range(len(gene.bases)):
         val = random()
-        if val <= 0.5:
-            gene.bases[i] += randint(0, 100)
+        if val <= 0.1:
+            gene.bases[i] = int(gene.bases[i] / randint(1, 3))
+        elif val <= 0.2:
+            gene.bases[i] = int(gene.bases[i] * randint(1, 3))
+        elif val <= 0.6:
+            gene.bases[i] += randint(0, 11)
         else:
-            gene.bases[i] -= randint(0, 100)
+            gene.bases[i] -= randint(0, 11)
     return gene
 
 count, population = optimize_gene(measure_fitness, mutate_gene)
 best = population[0]
 score = sum(best.bases)
 
 print(f"{count} generations passed")
-print(f"the best result had {score=} compared to {target=})")
+print(f"the best result had {score=} compared to {target=}")
 print(best)
 ```
 
 Creating custom fitness functions or artificial life simulations is left as an
 exercise to the reader.
 
 ## Testing
```

### Comparing `bluegenes-0.0.2/PKG-INFO` & `bluegenes-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluegenes
-Version: 0.0.2
+Version: 0.0.3
 Summary: Working-man's library for genetic algorithms
 Project-URL: Homepage, https://github.com/k98kurz/bluegenes-python
 Project-URL: Bug Tracker, https://github.com/k98kurz/bluegenes-python/issues
 Author-email: k98kurz <k98kurz@gmail.com>
 License-File: license
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -94,26 +94,30 @@
     """Produces a fitness score. Passed as parameter to optimize_gene."""
     return 1 / (1 + abs(sum(gene.bases) - target))
 
 def mutate_gene(gene: Gene) -> Gene:
     """Mutates the Gene randomly. Passed as parameter to optimize_gene."""
     for i in range(len(gene.bases)):
         val = random()
-        if val <= 0.5:
-            gene.bases[i] += randint(0, 100)
+        if val <= 0.1:
+            gene.bases[i] = int(gene.bases[i] / randint(1, 3))
+        elif val <= 0.2:
+            gene.bases[i] = int(gene.bases[i] * randint(1, 3))
+        elif val <= 0.6:
+            gene.bases[i] += randint(0, 11)
         else:
-            gene.bases[i] -= randint(0, 100)
+            gene.bases[i] -= randint(0, 11)
     return gene
 
 count, population = optimize_gene(measure_fitness, mutate_gene)
 best = population[0]
 score = sum(best.bases)
 
 print(f"{count} generations passed")
-print(f"the best result had {score=} compared to {target=})")
+print(f"the best result had {score=} compared to {target=}")
 print(best)
 ```
 
 Creating custom fitness functions or artificial life simulations is left as an
 exercise to the reader.
 
 ## Testing
```

