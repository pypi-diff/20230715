# Comparing `tmp/py_astrolab-0.2.0.tar.gz` & `tmp/py_astrolab-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_astrolab-0.2.0.tar", max compression
+gzip compressed data, was "py_astrolab-0.2.1.tar", max compression
```

## Comparing `py_astrolab-0.2.0.tar` & `py_astrolab-0.2.1.tar`

### file list

```diff
@@ -1,20 +1,19 @@
--rw-r--r--   0        0        0     5017 2023-05-29 18:14:56.433552 py_astrolab-0.2.0/py_astrolab/__init__.py
--rw-r--r--   0        0        0    16866 2023-07-12 12:53:57.224268 py_astrolab-0.2.0/py_astrolab/aspects.py
--rw-r--r--   0        0        0        0 2023-05-29 18:14:56.433552 py_astrolab-0.2.0/py_astrolab/charts/__init__.py
--rw-r--r--   0        0        0    73247 2023-07-12 13:04:58.545802 py_astrolab-0.2.0/py_astrolab/charts/charts_svg.py
--rw-r--r--   0        0        0    56568 2023-05-30 14:28:48.138660 py_astrolab-0.2.0/py_astrolab/charts/templates/basic.xml
--rw-r--r--   0        0        0    56755 2023-05-30 14:28:36.593933 py_astrolab-0.2.0/py_astrolab/charts/templates/extended.xml
--rw-r--r--   0        0        0    61624 2023-07-09 13:46:32.333795 py_astrolab-0.2.0/py_astrolab/charts/templates/minimal.xml
--rw-r--r--   0        0        0    73370 2023-07-09 16:34:16.735355 py_astrolab-0.2.0/py_astrolab/charts/wonderful_mistake.py
--rw-r--r--   0        0        0     5077 2023-05-29 18:14:56.449179 py_astrolab-0.2.0/py_astrolab/fetch_geonames.py
--rw-r--r--   0        0        0    12935 2023-07-08 15:20:41.033613 py_astrolab-0.2.0/py_astrolab/kr.config.json
--rw-r--r--   0        0        0    26385 2023-06-21 20:10:47.767169 py_astrolab-0.2.0/py_astrolab/main.py
--rw-r--r--   0        0        0     3149 2023-06-17 10:10:20.258711 py_astrolab-0.2.0/py_astrolab/print_all_data.py
--rw-r--r--   0        0        0     7785 2023-06-17 10:10:20.255187 py_astrolab-0.2.0/py_astrolab/relationship_score.py
--rw-r--r--   0        0        0     2361 2023-07-12 12:55:07.631989 py_astrolab-0.2.0/py_astrolab/report.py
--rw-r--r--   0        0        0     5074 2023-07-12 12:49:41.885152 py_astrolab-0.2.0/py_astrolab/types.py
--rw-r--r--   0        0        0     7171 2023-07-12 13:18:34.934445 py_astrolab-0.2.0/py_astrolab/utilities.py
--rw-r--r--   0        0        0      689 2023-07-12 13:34:09.729189 py_astrolab-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       91 2023-06-17 10:19:25.525258 py_astrolab-0.2.0/README.md
--rw-r--r--   0        0        0      975 1970-01-01 00:00:00.000000 py_astrolab-0.2.0/setup.py
--rw-r--r--   0        0        0      835 1970-01-01 00:00:00.000000 py_astrolab-0.2.0/PKG-INFO
+-rwxr-xr-x   0        0        0       91 2023-06-17 10:19:25.525258 py_astrolab-0.2.1/README.md
+-rwxr-xr-x   0        0        0     5017 2023-05-29 18:14:56.433552 py_astrolab-0.2.1/py_astrolab/__init__.py
+-rwxr-xr-x   0        0        0    16866 2023-07-12 12:53:57.224268 py_astrolab-0.2.1/py_astrolab/aspects.py
+-rwxr-xr-x   0        0        0        0 2023-05-29 18:14:56.433552 py_astrolab-0.2.1/py_astrolab/charts/__init__.py
+-rwxr-xr-x   0        0        0    75485 2023-07-15 10:08:11.386461 py_astrolab-0.2.1/py_astrolab/charts/charts_svg.py
+-rwxr-xr-x   0        0        0    56568 2023-05-30 14:28:48.138660 py_astrolab-0.2.1/py_astrolab/charts/templates/basic.xml
+-rwxr-xr-x   0        0        0    56755 2023-05-30 14:28:36.593933 py_astrolab-0.2.1/py_astrolab/charts/templates/extended.xml
+-rwxr-xr-x   0        0        0    61207 2023-07-15 10:08:23.312764 py_astrolab-0.2.1/py_astrolab/charts/templates/minimal.xml
+-rwxr-xr-x   0        0        0    73370 2023-07-09 16:34:16.735355 py_astrolab-0.2.1/py_astrolab/charts/wonderful_mistake.py
+-rwxr-xr-x   0        0        0     5077 2023-05-29 18:14:56.449179 py_astrolab-0.2.1/py_astrolab/fetch_geonames.py
+-rwxr-xr-x   0        0        0    12935 2023-07-08 15:20:41.033613 py_astrolab-0.2.1/py_astrolab/kr.config.json
+-rwxr-xr-x   0        0        0    26385 2023-06-21 20:10:47.767169 py_astrolab-0.2.1/py_astrolab/main.py
+-rwxr-xr-x   0        0        0     3149 2023-06-17 10:10:20.258711 py_astrolab-0.2.1/py_astrolab/print_all_data.py
+-rwxr-xr-x   0        0        0     7785 2023-06-17 10:10:20.255187 py_astrolab-0.2.1/py_astrolab/relationship_score.py
+-rwxr-xr-x   0        0        0     2361 2023-07-12 12:55:07.631989 py_astrolab-0.2.1/py_astrolab/report.py
+-rwxr-xr-x   0        0        0     5074 2023-07-12 12:49:41.885152 py_astrolab-0.2.1/py_astrolab/types.py
+-rwxr-xr-x   0        0        0     7171 2023-07-12 13:18:34.934445 py_astrolab-0.2.1/py_astrolab/utilities.py
+-rwxr-xr-x   0        0        0      689 2023-07-15 10:08:37.498554 py_astrolab-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      835 1970-01-01 00:00:00.000000 py_astrolab-0.2.1/PKG-INFO
```

### Comparing `py_astrolab-0.2.0/py_astrolab/__init__.py` & `py_astrolab-0.2.1/py_astrolab/__init__.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.2.0/py_astrolab/aspects.py` & `py_astrolab-0.2.1/py_astrolab/aspects.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.2.0/py_astrolab/charts/charts_svg.py` & `py_astrolab-0.2.1/py_astrolab/charts/charts_svg.py`

 * *Files 2% similar despite different names*

```diff
@@ -439,45 +439,93 @@
         return r * (math.cos(radial)+1)
 
     def __sliceToY(self, slice, r, offset):
         plus = (math.pi * offset) / 180
         radial = ((math.pi/6) * slice) + plus
         return r * ((math.sin(radial)/-1)+1)
 
-    def __zodiacSlice(self, num, r, style,  type):
-        # pie slices
-        offset = 360 - self.houses_degree_ut[6]
+    def __zodiacSlice(self, num, r, style,  type: str):
+        offset = 360 - self.houses_degree_ut[6] + num * 30
+        next_offset = offset + 30
         # check transit
         if self.chart_type == "Transit" or self.chart_type == "Composite":
             dropin = 0
+            roff = 72
         else:
             dropin = self.c1
-        slice = f'<path class="zodiac" id="zodiac{type}" d="M' + str(r) + ',' + str(r) + ' L' + str(dropin + self.__sliceToX(num, r-dropin, offset)) + ',' + str(dropin + self.__sliceToY(num, r-dropin, offset)) + ' A' + str(
-            r-dropin) + ',' + str(r-dropin) + ' 0 0,0 ' + str(dropin + self.__sliceToX(num+1, r-dropin, offset)) + ',' + str(dropin + self.__sliceToY(num+1, r-dropin, offset)) + ' z" style="' + style + '"/>'
+            roff = self.c2
+        degrees = ''
+        for i in range(num*30, (num+1)*30):
+            offset_degree = i - self.houses_degree_ut[6]
+            if offset_degree < 0:
+                offset_degree += 360
+            elif offset_degree > 360:
+                offset_degree -= 360
+            length = 5 if i % 5 == 0 else 3
+            dx1 = self.__sliceToX(0, r-self.c2, offset_degree) + self.c2
+            dy1 = self.__sliceToY(0, r-self.c2, offset_degree) + self.c2
+            dx2 = self.__sliceToX(0, r-length-self.c2, offset_degree) + length + self.c2
+            dy2 = self.__sliceToY(0, r-length-self.c2, offset_degree) + length + self.c2
+            degrees += f'<line class="{type.title()[:3]} degree" x1="{dx1}" y1="{dy1}" x2="{dx2}" y2="{dy2}" style="stroke: {self.colors_settings["paper_0"]}; stroke-width: 1px; stroke-opacity: 0;"/>'
+        x1 = self.__sliceToX(0, (r-dropin), offset) + dropin
+        y1 = self.__sliceToY(0, (r-dropin), offset) + dropin
+        x2 = self.__sliceToX(0, r-roff, offset) + roff
+        y2 = self.__sliceToY(0, r-roff, offset) + roff
+        x3 = self.__sliceToX(0, (r-dropin), next_offset) + dropin
+        y3 = self.__sliceToY(0, (r-dropin), next_offset) + dropin
+        x4 = self.__sliceToX(0, r-roff, next_offset) + roff
+        y4 = self.__sliceToY(0, r-roff, next_offset) + roff
+        # Inizia al bordo inferiore della cuspide della casa corrente
+        path_data = f"M {x1},{y1} "
+        # Vai al bordo superiore lungo la cuspide
+        path_data += f"L {x2},{y2} "
+        # Segui l'arco superiore alla prossima cuspide
+        path_data += f"A {r-roff},{r-roff} 0 0,0 {x4},{y4} "
+        # Vai al bordo inferiore lungo la cuspide
+        path_data += f"L {x3},{y3} "
+        # Segui l'arco inferiore indietro alla cuspide della casa corrente
+        path_data += f"A {r-dropin},{r-dropin} 0 0,1 {x1},{y1} "
+        # Chiudi il percorso (anche se non necessario perché le coordinate finali e iniziali coincidono)
+        path_data += "Z"
+        slice = f'<path d="{path_data}" class="zodiac" id="{type.title()[:3]} slice" style="{style}"/>'
         # symbols
         offset = offset + 15
         # check transit
         if self.chart_type == "Transit" or self.chart_type == "Composite":
             dropin = 54
         else:
             dropin = 18+self.c1
-        sign = '<g transform="translate(-13,-13)"><use x="' + str(dropin + self.__sliceToX(num, r-dropin, offset)) + '" y="' + str(
-            dropin + self.__sliceToY(num, r-dropin, offset)) + '" xlink:href="#' + type + '" /></g>'
-        return slice + '' + sign
+        sign_x = dropin + self.__sliceToX(0, r-dropin, offset)
+        sign_y = dropin + self.__sliceToY(0, r-dropin, offset)
+        sign = f'<g class="sign" id="{type.title()[:3]}" transform="translate(-13,-13)"><use x="{sign_x}" y="{sign_y}" xlink:href="#{type}" /></g>'
+        return slice + sign + degrees
 
     def __makeZodiac(self, r):
         output = ""
         for i in range(len(self.zodiac)):
             output = output + self.__zodiacSlice(i, r, "fill:" + self.colors_settings["zodiac_bg_%s" % (
                 i)] + "; fill-opacity: 1; fill-opacity: 1; stroke:#FFFFFF; stroke-opacity: 1; stroke-width: 2;", self.zodiac[i]) + ''
         return output
 
     def __makeHouses(self, r):
         path = ""
-
+        house_by_index = {
+            1: 'First',
+            2: 'Second',
+            3: 'Third',
+            4: 'Fourth',
+            5: 'Fifth',
+            6: 'Sixth',
+            7: 'Seventh',
+            8: 'Eighth',
+            9: 'Ninth',
+            10: 'Tenth',
+            11: 'Eleventh',
+            12: 'Twelfth'
+        }
         xr = 12
         for i in range(xr):
             if self.chart_type == "Transit" or self.chart_type == "Composite":
                 dropin = 160
                 roff = 72
                 t_roff = 36
             else:
@@ -533,15 +581,15 @@
                         t_y2)+'" style="stroke: '+t_linecolor+f'; stroke-width: 2px; stroke-opacity:0;"/>'
 
                 else:
                     path = path + '<text style="fill: #00f; fill-opacity: .4; font-size: 14px"><tspan x="' + \
                         str(xtext-3)+'" y="'+str(ytext+3) + \
                         '">'+str(i+1)+'</tspan></text>'
                     path = path + '<line x1="'+str(t_x1)+'" y1="'+str(t_y1)+'" x2="'+str(t_x2)+'" y2="'+str(
-                        t_y2)+'" style="stroke: '+t_linecolor+f'; stroke-width: 2px; stroke-opacity:.3;" class="house" id="house{i+1}"/>'
+                        t_y2)+'" style="stroke: '+t_linecolor+f'; stroke-width: 2px; stroke-opacity:.3;" class="house" id="{house_by_index[i+1]} House"/>'
 
             if self.chart_type == "Transit" or self.chart_type == "Composite":
                 dropin = 84
             if i+1 == 1:
                 house_number = 'I'
             elif i+1 == 4:
                 house_number = 'IV'
@@ -567,16 +615,16 @@
             path_data += f"A {r-roff},{r-roff} 0 0,0 {x4},{y4} "
             # Vai al bordo inferiore lungo la cuspide
             path_data += f"L {x3},{y3} "
             # Segui l'arco inferiore indietro alla cuspide della casa corrente
             path_data += f"A {r-dropin},{r-dropin} 0 0,1 {x1},{y1} "
             # Chiudi il percorso (anche se non necessario perché le coordinate finali e iniziali coincidono)
             path_data += "Z"
-            path = path + '<path d="'+path_data+'" class="house" id="house'+str(i+1)+'" fill="transparent" style="stroke: '+linecolor+'; stroke-width: 2px; stroke-opacity:.4;"/>'
-            path = path + '<text style="fill: #000000; fill-opacity: .4; font-size: 14px; font-weight: bold"><tspan x="' + \
+            path = path + '<path d="'+path_data+f'" class="house" id="{house_by_index[i+1]} House" fill="white" style="stroke: '+linecolor+'; stroke-width: 2px; stroke-opacity:.4;"/>'
+            path = path + f'<text class="houseLabel" id="{house_by_index[i+1]} House Label" style="fill: #000000; fill-opacity: .4; font-size: 14px; font-weight: bold"><tspan x="' + \
                 str(xtext-10)+'" y="'+str(ytext+3) + \
                 '">'+str(house_number)+'</tspan></text>'
         return path
 
     def __makePlanets(self, r):
 
         planets_degut = {}
@@ -762,19 +810,20 @@
                 int(self.houses_degree_ut[6]) / -1) + int(self.planets_degree_ut[i])
 
             planet_x = self.__sliceToX(0, (r-rplanet), offset) + rplanet
             planet_y = self.__sliceToY(0, (r-rplanet), offset) + rplanet
             if self.chart_type == "Transit" or self.chart_type == "Composite":
                 scale = 0.8
 
-            scale = 1
+            scale = 1.1
             # output planet
-            output = output + '<g transform="translate(-'+str(12*scale)+',-'+str(12*scale)+')"><g transform="scale('+str(scale)+')"><use x="' + str(
-                planet_x*(1/scale)) + '" y="' + str(planet_y*(1/scale)) + '" xlink:href="#' + self.planets_settings[i]['name'] + '" /></g></g>'
-
+            output += f''''
+                <g id="{self.planets_settings[i]["name"].title()}G" transform="translate(-{str(12*scale)}, -{str(12*scale)}) scale({str(scale)})">
+                    <use x="{str(planet_x*(1/scale))}" y="{str(planet_y*(1/scale))}" xlink:href="#{self.planets_settings[i]["name"]}"/>
+                </g>'''
         # make transit degut and display planets
         if self.chart_type == "Transit" or self.chart_type == "Composite":
             group_offset = {}
             t_planets_degut = {}
             if self.chart_type == "Transit":
                 list_range = len(self.planets_settings)-4
             else:
@@ -1449,15 +1498,14 @@
             td['makeAspects'] = self.__makeAspectsTransit(r, (r-160))
             td['makeAspectGrid'] = self.__makeAspectTransitGrid(r)
             td['makePatterns'] = ''
             td['makeAxis'] = ''
             td['chart_width'] = self.full_width
         else:
             td['transitRing'] = ""
-            td['degreeRing'] = self.__degreeRing(r)
             # circles
             td['c1'] = 'cx="' + str(r) + '" cy="' + \
                 str(r) + '" r="' + str(r-self.c1) + '"'
             td['c1style'] = 'fill: none; stroke: %s; stroke-width: 1px; ' % (
                 self.colors_settings['zodiac_radix_ring_2'])
             td['c2'] = 'cx="' + str(r) + '" cy="' + \
                 str(r) + '" r="' + str(r-self.c2) + '"'
@@ -1634,8 +1682,8 @@
     name = MakeSvgInstance(first, chart_type="Composite",
                            second_obj=second, lang="IT")
     # name.output_directory = Path.home() / "charts"
     template = name.makeTemplate()
     name.makeSVG()
     print(name.aspects_list[-1])
     name.makeSVG()
-    print(template)
+    print(template)
```

### Comparing `py_astrolab-0.2.0/py_astrolab/charts/templates/basic.xml` & `py_astrolab-0.2.1/py_astrolab/charts/templates/basic.xml`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.2.0/py_astrolab/charts/templates/extended.xml` & `py_astrolab-0.2.1/py_astrolab/charts/templates/extended.xml`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.2.0/py_astrolab/charts/templates/minimal.xml` & `py_astrolab-0.2.1/py_astrolab/charts/templates/minimal.xml`

 * *Files 2% similar despite different names*

```diff
@@ -17,3836 +17,3810 @@
 00000100: 6e73 3a78 6c69 6e6b 3d27 6874 7470 3a2f  ns:xlink='http:/
 00000110: 2f77 7777 2e77 332e 6f72 672f 3139 3939  /www.w3.org/1999
 00000120: 2f78 6c69 6e6b 2720 7769 6474 683d 2731  /xlink' width='1
 00000130: 3030 2527 2068 6569 6768 743d 2731 3030  00%' height='100
 00000140: 2527 2076 6965 7742 6f78 3d27 3020 3020  %' viewBox='0 0 
 00000150: 3535 3020 3535 3027 2070 7265 7365 7276  550 550' preserv
 00000160: 6541 7370 6563 7452 6174 696f 3d27 784d  eAspectRatio='xM
-00000170: 6964 594d 6964 273e 0d0a 2020 2020 3c74  idYMid'>..    <t
-00000180: 6974 6c65 3e4b 6572 796b 6569 6f6e 3c2f  itle>Kerykeion</
-00000190: 7469 746c 653e 0d0a 2020 2020 3c67 2074  title>..    <g t
-000001a0: 7261 6e73 666f 726d 3d27 7472 616e 736c  ransform='transl
-000001b0: 6174 6528 2463 6667 5472 616e 736c 6174  ate($cfgTranslat
-000001c0: 6529 273e 0d0a 2020 2020 2020 2020 3c67  e)'>..        <g
-000001d0: 2074 7261 6e73 666f 726d 3d27 726f 7461   transform='rota
-000001e0: 7465 2824 6366 6752 6f74 6174 6529 273e  te($cfgRotate)'>
-000001f0: 0d0a 2020 2020 2020 2020 2020 2020 3c67  ..            <g
-00000200: 2074 7261 6e73 666f 726d 3d27 7363 616c   transform='scal
-00000210: 6528 2463 6667 5a6f 6f6d 2927 3e0d 0a20  e($cfgZoom)'>.. 
-00000220: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00000230: 212d 2d20 3c72 6563 7420 783d 2730 2720  !-- <rect x='0' 
-00000240: 793d 2730 2720 7769 6474 683d 2735 3530  y='0' width='550
-00000250: 2720 6865 6967 6874 3d27 3535 3027 2073  ' height='550' s
-00000260: 7479 6c65 3d27 6669 6c6c 3a20 2470 6170  tyle='fill: $pap
-00000270: 6572 5f63 6f6c 6f72 5f31 3b27 202f 3e0d  er_color_1;' />.
-00000280: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000290: 203c 7465 7874 2078 3d27 3230 2720 793d   <text x='20' y=
-000002a0: 2733 3027 2073 7479 6c65 3d27 6669 6c6c  '30' style='fill
-000002b0: 3a20 2470 6170 6572 5f63 6f6c 6f72 5f30  : $paper_color_0
-000002c0: 3b20 666f 6e74 2d73 697a 653a 2032 3470  ; font-size: 24p
-000002d0: 7827 3e24 7374 7269 6e67 5469 746c 653c  x'>$stringTitle<
-000002e0: 2f74 6578 743e 0d0a 2020 2020 2020 2020  /text>..        
-000002f0: 2020 2020 2020 2020 3c74 6578 7420 783d          <text x=
-00000300: 2732 3027 2079 3d27 3530 2720 7374 796c  '20' y='50' styl
-00000310: 653d 2766 696c 6c3a 2024 7061 7065 725f  e='fill: $paper_
-00000320: 636f 6c6f 725f 303b 2066 6f6e 742d 7369  color_0; font-si
-00000330: 7a65 3a20 3131 7078 273e 2473 7472 696e  ze: 11px'>$strin
-00000340: 674e 616d 653c 2f74 6578 743e 0d0a 2020  gName</text>..  
-00000350: 2020 2020 2020 2020 2020 2020 2020 3c74                <t
-00000360: 6578 7420 783d 2732 3027 2079 3d27 3632  ext x='20' y='62
-00000370: 2720 7374 796c 653d 2766 696c 6c3a 2024  ' style='fill: $
-00000380: 7061 7065 725f 636f 6c6f 725f 303b 2066  paper_color_0; f
-00000390: 6f6e 742d 7369 7a65 3a20 3131 7078 273e  ont-size: 11px'>
-000003a0: 2473 7472 696e 674c 6f63 6174 696f 6e3c  $stringLocation<
-000003b0: 2f74 6578 743e 0d0a 2020 2020 2020 2020  /text>..        
-000003c0: 2020 2020 2020 2020 3c74 6578 7420 783d          <text x=
-000003d0: 2732 3027 2079 3d27 3734 2720 7374 796c  '20' y='74' styl
-000003e0: 653d 2766 696c 6c3a 2024 7061 7065 725f  e='fill: $paper_
-000003f0: 636f 6c6f 725f 303b 2066 6f6e 742d 7369  color_0; font-si
-00000400: 7a65 3a20 3131 7078 273e 2473 7472 696e  ze: 11px'>$strin
-00000410: 6744 6174 6554 696d 653c 2f74 6578 743e  gDateTime</text>
-00000420: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000430: 2020 3c74 6578 7420 783d 2732 3027 2079    <text x='20' y
-00000440: 3d27 3836 2720 7374 796c 653d 2766 696c  ='86' style='fil
-00000450: 6c3a 2024 7061 7065 725f 636f 6c6f 725f  l: $paper_color_
-00000460: 303b 2066 6f6e 742d 7369 7a65 3a20 3131  0; font-size: 11
-00000470: 7078 273e 2473 7472 696e 674c 6174 3c2f  px'>$stringLat</
-00000480: 7465 7874 3e0d 0a20 2020 2020 2020 2020  text>..         
-00000490: 2020 2020 2020 203c 7465 7874 2078 3d27         <text x='
-000004a0: 3230 2720 793d 2739 3827 2073 7479 6c65  20' y='98' style
-000004b0: 3d27 6669 6c6c 3a20 2470 6170 6572 5f63  ='fill: $paper_c
-000004c0: 6f6c 6f72 5f30 3b20 666f 6e74 2d73 697a  olor_0; font-siz
-000004d0: 653a 2031 3170 7827 3e24 7374 7269 6e67  e: 11px'>$string
-000004e0: 4c6f 6e3c 2f74 6578 743e 0d0a 2020 2020  Lon</text>..    
-000004f0: 2020 2020 2020 2020 2020 2020 3c74 6578              <tex
-00000500: 7420 783d 2732 3027 2079 3d27 3131 3027  t x='20' y='110'
-00000510: 2073 7479 6c65 3d27 6669 6c6c 3a20 2470   style='fill: $p
-00000520: 6170 6572 5f63 6f6c 6f72 5f30 3b20 666f  aper_color_0; fo
-00000530: 6e74 2d73 697a 653a 2031 3170 7827 3e24  nt-size: 11px'>$
-00000540: 7374 7269 6e67 506f 7369 7469 6f6e 3c2f  stringPosition</
-00000550: 7465 7874 3e0d 0a20 2020 2020 2020 2020  text>..         
-00000560: 2020 2020 2020 203c 7465 7874 2078 3d27         <text x='
-00000570: 3230 2720 793d 2734 3830 2720 7374 796c  20' y='480' styl
-00000580: 653d 2766 696c 6c3a 2024 7061 7065 725f  e='fill: $paper_
-00000590: 636f 6c6f 725f 303b 2066 6f6e 742d 7369  color_0; font-si
-000005a0: 7a65 3a20 3130 7078 273e 2462 6f74 746f  ze: 10px'>$botto
-000005b0: 6d4c 6566 7431 3c2f 7465 7874 3e0d 0a20  mLeft1</text>.. 
-000005c0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-000005d0: 7465 7874 2078 3d27 3230 2720 793d 2734  text x='20' y='4
-000005e0: 3934 2720 7374 796c 653d 2766 696c 6c3a  94' style='fill:
-000005f0: 2024 7061 7065 725f 636f 6c6f 725f 303b   $paper_color_0;
-00000600: 2066 6f6e 742d 7369 7a65 3a20 3130 7078   font-size: 10px
-00000610: 273e 2462 6f74 746f 6d4c 6566 7432 3c2f  '>$bottomLeft2</
-00000620: 7465 7874 3e0d 0a20 2020 2020 2020 2020  text>..         
-00000630: 2020 2020 2020 203c 7465 7874 2078 3d27         <text x='
-00000640: 3230 2720 793d 2735 3038 2720 7374 796c  20' y='508' styl
-00000650: 653d 2766 696c 6c3a 2024 7061 7065 725f  e='fill: $paper_
-00000660: 636f 6c6f 725f 303b 2066 6f6e 742d 7369  color_0; font-si
-00000670: 7a65 3a20 3130 7078 273e 2462 6f74 746f  ze: 10px'>$botto
-00000680: 6d4c 6566 7433 3c2f 7465 7874 3e0d 0a20  mLeft3</text>.. 
-00000690: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-000006a0: 7465 7874 2078 3d27 3230 2720 793d 2735  text x='20' y='5
-000006b0: 3232 2720 7374 796c 653d 2766 696c 6c3a  22' style='fill:
-000006c0: 2024 7061 7065 725f 636f 6c6f 725f 303b   $paper_color_0;
-000006d0: 2066 6f6e 742d 7369 7a65 3a20 3130 7078   font-size: 10px
-000006e0: 273e 2462 6f74 746f 6d4c 6566 7434 3c2f  '>$bottomLeft4</
-000006f0: 7465 7874 3e20 2020 2020 2020 2020 2020  text>           
-00000700: 2020 2020 2020 2d2d 3e0d 0a20 2020 2020        -->..     
-00000710: 2020 2020 2020 2020 2020 203c 212d 2d20             <!-- 
-00000720: 4c75 6e61 7220 5068 6173 6520 2d2d 3e0d  Lunar Phase -->.
-00000730: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000740: 203c 212d 2d20 3c67 2074 7261 6e73 666f   <!-- <g transfo
-00000750: 726d 3d27 7472 616e 736c 6174 6528 3230  rm='translate(20
-00000760: 2c35 3138 2927 3e0d 0a20 2020 2020 2020  ,518)'>..       
-00000770: 2020 2020 2020 2020 2020 2020 203c 6720               <g 
-00000780: 7472 616e 7366 6f72 6d3d 2772 6f74 6174  transform='rotat
-00000790: 6528 246c 756e 6172 5f70 6861 7365 5f72  e($lunar_phase_r
-000007a0: 6f74 6174 6520 3230 2031 3029 273e 0d0a  otate 20 10)'>..
-000007b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000007c0: 2020 2020 2020 2020 3c64 6566 733e 0d0a          <defs>..
-000007d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000007e0: 2020 2020 2020 2020 2020 2020 3c63 6c69              <cli
-000007f0: 7050 6174 6820 6964 3d27 6375 742d 6f66  pPath id='cut-of
-00000800: 662d 6369 7263 6c65 273e 0d0a 2020 2020  f-circle'>..    
-00000810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000820: 2020 2020 2020 2020 2020 2020 3c63 6972              <cir
-00000830: 636c 6520 6378 3d27 3230 2720 6379 3d27  cle cx='20' cy='
-00000840: 3130 2720 723d 2731 3027 202f 3e0d 0a20  10' r='10' />.. 
-00000850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000860: 2020 2020 2020 2020 2020 203c 2f63 6c69             </cli
-00000870: 7050 6174 683e 0d0a 2020 2020 2020 2020  pPath>..        
+00000170: 6964 594d 6964 273e 0d0a 2020 2020 3c67  idYMid'>..    <g
+00000180: 2074 7261 6e73 666f 726d 3d27 7472 616e   transform='tran
+00000190: 736c 6174 6528 2463 6667 5472 616e 736c  slate($cfgTransl
+000001a0: 6174 6529 273e 0d0a 2020 2020 2020 2020  ate)'>..        
+000001b0: 3c67 2074 7261 6e73 666f 726d 3d27 726f  <g transform='ro
+000001c0: 7461 7465 2824 6366 6752 6f74 6174 6529  tate($cfgRotate)
+000001d0: 273e 0d0a 2020 2020 2020 2020 2020 2020  '>..            
+000001e0: 3c67 2074 7261 6e73 666f 726d 3d27 7363  <g transform='sc
+000001f0: 616c 6528 2463 6667 5a6f 6f6d 2927 3e0d  ale($cfgZoom)'>.
+00000200: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000210: 203c 212d 2d20 3c72 6563 7420 783d 2730   <!-- <rect x='0
+00000220: 2720 793d 2730 2720 7769 6474 683d 2735  ' y='0' width='5
+00000230: 3530 2720 6865 6967 6874 3d27 3535 3027  50' height='550'
+00000240: 2073 7479 6c65 3d27 6669 6c6c 3a20 2470   style='fill: $p
+00000250: 6170 6572 5f63 6f6c 6f72 5f31 3b27 202f  aper_color_1;' /
+00000260: 3e0d 0a20 2020 2020 2020 2020 2020 2020  >..             
+00000270: 2020 203c 7465 7874 2078 3d27 3230 2720     <text x='20' 
+00000280: 793d 2733 3027 2073 7479 6c65 3d27 6669  y='30' style='fi
+00000290: 6c6c 3a20 2470 6170 6572 5f63 6f6c 6f72  ll: $paper_color
+000002a0: 5f30 3b20 666f 6e74 2d73 697a 653a 2032  _0; font-size: 2
+000002b0: 3470 7827 3e24 7374 7269 6e67 5469 746c  4px'>$stringTitl
+000002c0: 653c 2f74 6578 743e 0d0a 2020 2020 2020  e</text>..      
+000002d0: 2020 2020 2020 2020 2020 3c74 6578 7420            <text 
+000002e0: 783d 2732 3027 2079 3d27 3530 2720 7374  x='20' y='50' st
+000002f0: 796c 653d 2766 696c 6c3a 2024 7061 7065  yle='fill: $pape
+00000300: 725f 636f 6c6f 725f 303b 2066 6f6e 742d  r_color_0; font-
+00000310: 7369 7a65 3a20 3131 7078 273e 2473 7472  size: 11px'>$str
+00000320: 696e 674e 616d 653c 2f74 6578 743e 0d0a  ingName</text>..
+00000330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000340: 3c74 6578 7420 783d 2732 3027 2079 3d27  <text x='20' y='
+00000350: 3632 2720 7374 796c 653d 2766 696c 6c3a  62' style='fill:
+00000360: 2024 7061 7065 725f 636f 6c6f 725f 303b   $paper_color_0;
+00000370: 2066 6f6e 742d 7369 7a65 3a20 3131 7078   font-size: 11px
+00000380: 273e 2473 7472 696e 674c 6f63 6174 696f  '>$stringLocatio
+00000390: 6e3c 2f74 6578 743e 0d0a 2020 2020 2020  n</text>..      
+000003a0: 2020 2020 2020 2020 2020 3c74 6578 7420            <text 
+000003b0: 783d 2732 3027 2079 3d27 3734 2720 7374  x='20' y='74' st
+000003c0: 796c 653d 2766 696c 6c3a 2024 7061 7065  yle='fill: $pape
+000003d0: 725f 636f 6c6f 725f 303b 2066 6f6e 742d  r_color_0; font-
+000003e0: 7369 7a65 3a20 3131 7078 273e 2473 7472  size: 11px'>$str
+000003f0: 696e 6744 6174 6554 696d 653c 2f74 6578  ingDateTime</tex
+00000400: 743e 0d0a 2020 2020 2020 2020 2020 2020  t>..            
+00000410: 2020 2020 3c74 6578 7420 783d 2732 3027      <text x='20'
+00000420: 2079 3d27 3836 2720 7374 796c 653d 2766   y='86' style='f
+00000430: 696c 6c3a 2024 7061 7065 725f 636f 6c6f  ill: $paper_colo
+00000440: 725f 303b 2066 6f6e 742d 7369 7a65 3a20  r_0; font-size: 
+00000450: 3131 7078 273e 2473 7472 696e 674c 6174  11px'>$stringLat
+00000460: 3c2f 7465 7874 3e0d 0a20 2020 2020 2020  </text>..       
+00000470: 2020 2020 2020 2020 203c 7465 7874 2078           <text x
+00000480: 3d27 3230 2720 793d 2739 3827 2073 7479  ='20' y='98' sty
+00000490: 6c65 3d27 6669 6c6c 3a20 2470 6170 6572  le='fill: $paper
+000004a0: 5f63 6f6c 6f72 5f30 3b20 666f 6e74 2d73  _color_0; font-s
+000004b0: 697a 653a 2031 3170 7827 3e24 7374 7269  ize: 11px'>$stri
+000004c0: 6e67 4c6f 6e3c 2f74 6578 743e 0d0a 2020  ngLon</text>..  
+000004d0: 2020 2020 2020 2020 2020 2020 2020 3c74                <t
+000004e0: 6578 7420 783d 2732 3027 2079 3d27 3131  ext x='20' y='11
+000004f0: 3027 2073 7479 6c65 3d27 6669 6c6c 3a20  0' style='fill: 
+00000500: 2470 6170 6572 5f63 6f6c 6f72 5f30 3b20  $paper_color_0; 
+00000510: 666f 6e74 2d73 697a 653a 2031 3170 7827  font-size: 11px'
+00000520: 3e24 7374 7269 6e67 506f 7369 7469 6f6e  >$stringPosition
+00000530: 3c2f 7465 7874 3e0d 0a20 2020 2020 2020  </text>..       
+00000540: 2020 2020 2020 2020 203c 7465 7874 2078           <text x
+00000550: 3d27 3230 2720 793d 2734 3830 2720 7374  ='20' y='480' st
+00000560: 796c 653d 2766 696c 6c3a 2024 7061 7065  yle='fill: $pape
+00000570: 725f 636f 6c6f 725f 303b 2066 6f6e 742d  r_color_0; font-
+00000580: 7369 7a65 3a20 3130 7078 273e 2462 6f74  size: 10px'>$bot
+00000590: 746f 6d4c 6566 7431 3c2f 7465 7874 3e0d  tomLeft1</text>.
+000005a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000005b0: 203c 7465 7874 2078 3d27 3230 2720 793d   <text x='20' y=
+000005c0: 2734 3934 2720 7374 796c 653d 2766 696c  '494' style='fil
+000005d0: 6c3a 2024 7061 7065 725f 636f 6c6f 725f  l: $paper_color_
+000005e0: 303b 2066 6f6e 742d 7369 7a65 3a20 3130  0; font-size: 10
+000005f0: 7078 273e 2462 6f74 746f 6d4c 6566 7432  px'>$bottomLeft2
+00000600: 3c2f 7465 7874 3e0d 0a20 2020 2020 2020  </text>..       
+00000610: 2020 2020 2020 2020 203c 7465 7874 2078           <text x
+00000620: 3d27 3230 2720 793d 2735 3038 2720 7374  ='20' y='508' st
+00000630: 796c 653d 2766 696c 6c3a 2024 7061 7065  yle='fill: $pape
+00000640: 725f 636f 6c6f 725f 303b 2066 6f6e 742d  r_color_0; font-
+00000650: 7369 7a65 3a20 3130 7078 273e 2462 6f74  size: 10px'>$bot
+00000660: 746f 6d4c 6566 7433 3c2f 7465 7874 3e0d  tomLeft3</text>.
+00000670: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000680: 203c 7465 7874 2078 3d27 3230 2720 793d   <text x='20' y=
+00000690: 2735 3232 2720 7374 796c 653d 2766 696c  '522' style='fil
+000006a0: 6c3a 2024 7061 7065 725f 636f 6c6f 725f  l: $paper_color_
+000006b0: 303b 2066 6f6e 742d 7369 7a65 3a20 3130  0; font-size: 10
+000006c0: 7078 273e 2462 6f74 746f 6d4c 6566 7434  px'>$bottomLeft4
+000006d0: 3c2f 7465 7874 3e20 2020 2020 2020 2020  </text>         
+000006e0: 2020 2020 2020 2020 2d2d 3e0d 0a20 2020          -->..   
+000006f0: 2020 2020 2020 2020 2020 2020 203c 212d               <!-
+00000700: 2d20 4c75 6e61 7220 5068 6173 6520 2d2d  - Lunar Phase --
+00000710: 3e0d 0a20 2020 2020 2020 2020 2020 2020  >..             
+00000720: 2020 203c 212d 2d20 3c67 2074 7261 6e73     <!-- <g trans
+00000730: 666f 726d 3d27 7472 616e 736c 6174 6528  form='translate(
+00000740: 3230 2c35 3138 2927 3e0d 0a20 2020 2020  20,518)'>..     
+00000750: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00000760: 6720 7472 616e 7366 6f72 6d3d 2772 6f74  g transform='rot
+00000770: 6174 6528 246c 756e 6172 5f70 6861 7365  ate($lunar_phase
+00000780: 5f72 6f74 6174 6520 3230 2031 3029 273e  _rotate 20 10)'>
+00000790: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000007a0: 2020 2020 2020 2020 2020 3c64 6566 733e            <defs>
+000007b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000007c0: 2020 2020 2020 2020 2020 2020 2020 3c63                <c
+000007d0: 6c69 7050 6174 6820 6964 3d27 6375 742d  lipPath id='cut-
+000007e0: 6f66 662d 6369 7263 6c65 273e 0d0a 2020  off-circle'>..  
+000007f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000800: 2020 2020 2020 2020 2020 2020 2020 3c63                <c
+00000810: 6972 636c 6520 6378 3d27 3230 2720 6379  ircle cx='20' cy
+00000820: 3d27 3130 2720 723d 2731 3027 202f 3e0d  ='10' r='10' />.
+00000830: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000840: 2020 2020 2020 2020 2020 2020 203c 2f63               </c
+00000850: 6c69 7050 6174 683e 0d0a 2020 2020 2020  lipPath>..      
+00000860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000870: 2020 3c2f 6465 6673 3e0d 0a20 2020 2020    </defs>..     
 00000880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000890: 3c2f 6465 6673 3e0d 0a20 2020 2020 2020  </defs>..       
-000008a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000008b0: 203c 6369 7263 6c65 2063 783d 2732 3027   <circle cx='20'
-000008c0: 2063 793d 2731 3027 2072 3d27 3130 2720   cy='10' r='10' 
-000008d0: 7374 796c 653d 2766 696c 6c3a 2024 6c75  style='fill: $lu
-000008e0: 6e61 725f 7068 6173 655f 6267 3b27 202f  nar_phase_bg;' /
-000008f0: 3e0d 0a20 2020 2020 2020 2020 2020 2020  >..             
-00000900: 2020 2020 2020 2020 2020 203c 6369 7263             <circ
-00000910: 6c65 2063 783d 2724 6c75 6e61 725f 7068  le cx='$lunar_ph
-00000920: 6173 655f 6378 2720 6379 3d27 3130 2720  ase_cx' cy='10' 
-00000930: 723d 2724 6c75 6e61 725f 7068 6173 655f  r='$lunar_phase_
-00000940: 7227 2073 7479 6c65 3d27 6669 6c6c 3a20  r' style='fill: 
-00000950: 246c 756e 6172 5f70 6861 7365 5f66 6727  $lunar_phase_fg'
-00000960: 2063 6c69 702d 7061 7468 3d27 7572 6c28   clip-path='url(
-00000970: 2363 7574 2d6f 6666 2d63 6972 636c 6529  #cut-off-circle)
-00000980: 2720 2f3e 0d0a 2020 2020 2020 2020 2020  ' />..          
-00000990: 2020 2020 2020 2020 2020 2020 2020 3c63                <c
-000009a0: 6972 636c 6520 6378 3d27 3230 2720 6379  ircle cx='20' cy
-000009b0: 3d27 3130 2720 723d 2731 3027 2073 7479  ='10' r='10' sty
-000009c0: 6c65 3d27 6669 6c6c 3a20 6e6f 6e65 3b20  le='fill: none; 
-000009d0: 7374 726f 6b65 3a20 246c 756e 6172 5f70  stroke: $lunar_p
-000009e0: 6861 7365 5f6f 7574 6c69 6e65 3b20 7374  hase_outline; st
-000009f0: 726f 6b65 2d77 6964 7468 3a20 302e 3570  roke-width: 0.5p
-00000a00: 783b 2073 7472 6f6b 652d 6f70 6163 6974  x; stroke-opacit
-00000a10: 793a 202e 353b 2720 2f3e 0d0a 2020 2020  y: .5;' />..    
-00000a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000a30: 3c2f 673e 0d0a 2020 2020 2020 2020 2020  </g>..          
-00000a40: 2020 2020 2020 3c2f 673e 2020 2020 2020        </g>      
-00000a50: 2020 2020 2020 2020 2020 202d 2d3e 0d0a             -->..
-00000a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000a70: 3c21 2d2d 2050 6c61 6e65 7473 2028 3234  <!-- Planets (24
-00000a80: 7832 3429 202d 2d3e 0d0a 2020 2020 2020  x24) -->..      
-00000a90: 2020 2020 2020 2020 2020 3c73 796d 626f            <symbo
-00000aa0: 6c20 6964 3d27 5375 6e27 3e0d 0a20 2020  l id='Sun'>..   
-00000ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ac0: 203c 6720 7472 616e 7366 6f72 6d3d 2774   <g transform='t
-00000ad0: 7261 6e73 6c61 7465 2831 2c34 2927 3e0d  ranslate(1,4)'>.
-00000ae0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000af0: 2020 2020 2020 2020 203c 6369 7263 6c65           <circle
-00000b00: 2063 783d 2731 3027 2063 793d 2731 3027   cx='10' cy='10'
-00000b10: 2072 3d27 3927 2073 7479 6c65 3d27 6669   r='9' style='fi
-00000b20: 6c6c 3a20 6e6f 6e65 3b20 7374 726f 6b65  ll: none; stroke
-00000b30: 3a20 2470 6c61 6e65 7473 5f63 6f6c 6f72  : $planets_color
-00000b40: 5f30 3b20 7374 726f 6b65 2d77 6964 7468  _0; stroke-width
-00000b50: 3a20 3270 783b 2720 2f3e 0d0a 2020 2020  : 2px;' />..    
-00000b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b70: 2020 2020 3c63 6972 636c 6520 6378 3d27      <circle cx='
-00000b80: 3130 2720 6379 3d27 3130 2720 723d 2732  10' cy='10' r='2
-00000b90: 2720 7374 796c 653d 2766 696c 6c3a 2024  ' style='fill: $
-00000ba0: 706c 616e 6574 735f 636f 6c6f 725f 303b  planets_color_0;
-00000bb0: 2720 2f3e 0d0a 2020 2020 2020 2020 2020  ' />..          
-00000bc0: 2020 2020 2020 2020 2020 3c2f 673e 0d0a            </g>..
-00000bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000be0: 3c2f 7379 6d62 6f6c 3e0d 0a20 2020 2020  </symbol>..     
-00000bf0: 2020 2020 2020 2020 2020 203c 7379 6d62             <symb
-00000c00: 6f6c 2069 643d 274d 6f6f 6e27 3e0d 0a20  ol id='Moon'>.. 
-00000c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000c20: 2020 203c 6720 7472 616e 7366 6f72 6d3d     <g transform=
-00000c30: 2774 7261 6e73 6c61 7465 2834 2c33 2927  'translate(4,3)'
-00000c40: 3e0d 0a20 2020 2020 2020 2020 2020 2020  >..             
-00000c50: 2020 2020 2020 2020 2020 203c 6720 7472             <g tr
-00000c60: 616e 7366 6f72 6d3d 2773 6361 6c65 282e  ansform='scale(.
-00000c70: 3829 273e 0d0a 2020 2020 2020 2020 2020  8)'>..          
-00000c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000c90: 2020 3c70 6174 6820 643d 274d 2033 2e36    <path d='M 3.6
-00000ca0: 3633 3931 3934 2c31 2e30 3330 3835 3039  639194,1.0308509
-00000cb0: 2043 2032 2e37 3439 3834 3934 2c31 2e30   C 2.7498494,1.0
-00000cc0: 3635 3633 3039 2031 2e38 3732 3133 3934  656309 1.8721394
-00000cd0: 2c31 2e32 3133 3932 3039 2031 2e30 3238  ,1.2139209 1.028
-00000ce0: 3436 3934 2c31 2e34 3539 3338 3039 2043  4694,1.4593809 C
-00000cf0: 2035 2e35 3732 3937 3934 2c32 2e37 3939   5.5729794,2.799
-00000d00: 3936 3039 2038 2e38 3931 3937 3934 2c37  9609 8.8919794,7
-00000d10: 2e30 3234 3232 3039 2038 2e38 3931 3937  .0242209 8.89197
-00000d20: 3934 2c31 322e 3030 3131 3931 2043 2038  94,12.001191 C 8
-00000d30: 2e38 3931 3937 3934 2c31 362e 3937 3831  .8919794,16.9781
-00000d40: 3631 2035 2e35 3732 3937 3934 2c32 312e  61 5.5729794,21.
-00000d50: 3230 3234 3131 2031 2e30 3238 3436 3934  202411 1.0284694
-00000d60: 2c32 322e 3534 3330 3031 2043 2032 2e30  ,22.543001 C 2.0
-00000d70: 3031 3932 3934 2c32 322e 3832 3632 3231  019294,22.826221
-00000d80: 2033 2e30 3237 3938 3934 2c32 322e 3937   3.0279894,22.97
-00000d90: 3135 3331 2034 2e30 3932 3434 3934 2c32  1531 4.0924494,2
-00000da0: 322e 3937 3135 3331 2043 2031 302e 3134  2.971531 C 10.14
-00000db0: 3830 3739 2c32 322e 3937 3135 3331 2031  8079,22.971531 1
-00000dc0: 352e 3036 3237 3839 2c31 382e 3035 3638  5.062789,18.0568
-00000dd0: 3231 2031 352e 3036 3237 3839 2c31 322e  21 15.062789,12.
-00000de0: 3030 3131 3931 2043 2031 352e 3036 3237  001191 C 15.0627
-00000df0: 3839 2c35 2e39 3435 3536 3039 2031 302e  89,5.9455609 10.
-00000e00: 3134 3830 3739 2c31 2e30 3330 3835 3039  148079,1.0308509
-00000e10: 2034 2e30 3932 3434 3934 2c31 2e30 3330   4.0924494,1.030
-00000e20: 3835 3039 2043 2033 2e39 3530 3531 3934  8509 C 3.9505194
-00000e30: 2c31 2e30 3330 3835 3039 2033 2e38 3034  ,1.0308509 3.804
-00000e40: 3534 3934 2c31 2e30 3235 3439 3039 2033  5494,1.0254909 3
-00000e50: 2e36 3633 3931 3934 2c31 2e30 3330 3835  .6639194,1.03085
-00000e60: 3039 207a 2027 2073 7479 6c65 3d27 7374  09 z ' style='st
-00000e70: 726f 6b65 3a24 706c 616e 6574 735f 636f  roke:$planets_co
-00000e80: 6c6f 725f 313b 7374 726f 6b65 2d77 6964  lor_1;stroke-wid
-00000e90: 7468 3a32 7078 3b20 6669 6c6c 3a6e 6f6e  th:2px; fill:non
-00000ea0: 653b 2720 2f3e 0d0a 2020 2020 2020 2020  e;' />..        
-00000eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ec0: 3c2f 673e 0d0a 2020 2020 2020 2020 2020  </g>..          
-00000ed0: 2020 2020 2020 2020 2020 3c2f 673e 0d0a            </g>..
-00000ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ef0: 3c2f 7379 6d62 6f6c 3e0d 0a20 2020 2020  </symbol>..     
-00000f00: 2020 2020 2020 2020 2020 203c 7379 6d62             <symb
-00000f10: 6f6c 2069 643d 274d 6572 6375 7279 273e  ol id='Mercury'>
-00000f20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000f30: 2020 2020 2020 3c67 2074 7261 6e73 666f        <g transfo
-00000f40: 726d 3d27 7472 616e 736c 6174 6528 332c  rm='translate(3,
-00000f50: 3129 273e 0d0a 2020 2020 2020 2020 2020  1)'>..          
-00000f60: 2020 2020 2020 2020 2020 2020 2020 3c70                <p
-00000f70: 6174 6820 643d 274d 2031 322e 3431 3739  ath d='M 12.4179
-00000f80: 3038 2c31 312e 3039 3735 3037 2043 2031  08,11.097507 C 1
-00000f90: 322e 3436 3038 3138 2c31 332e 3630 3439  2.460818,13.6049
-00000fa0: 3136 2031 302e 3636 3832 3137 2c31 352e  16 10.668217,15.
-00000fb0: 3939 3636 3536 2038 2e32 3536 3638 3035  996656 8.2566805
-00000fc0: 2c31 362e 3637 3636 3339 2043 2036 2e31  ,16.676639 C 6.1
-00000fd0: 3138 3033 3735 2c31 372e 3332 3235 3232  180375,17.322522
-00000fe0: 2033 2e36 3430 3836 3735 2c31 362e 3631   3.6408675,16.61
-00000ff0: 3138 3639 2032 2e31 3939 3039 3135 2c31  1869 2.1990915,1
-00001000: 342e 3839 3730 3235 2043 2030 2e37 3032  4.897025 C 0.702
-00001010: 3531 3335 312c 3133 2e31 3835 3839 3420  51351,13.185894 
-00001020: 302e 3334 3730 3535 3531 2c31 302e 3537  0.34705551,10.57
-00001030: 3431 3439 2031 2e33 3738 3738 3335 2c38  4149 1.3787835,8
-00001040: 2e35 3430 3633 3720 4320 322e 3333 3039  .540637 C 2.3309
-00001050: 3036 352c 362e 3537 3738 3139 3620 342e  065,6.5778196 4.
-00001060: 3434 3438 3932 352c 352e 3233 3930 3531  4448925,5.239051
-00001070: 3520 362e 3633 3434 3338 352c 352e 3238  5 6.6344385,5.28
-00001080: 3031 3831 3220 4320 382e 3734 3336 3438  01812 C 8.743648
-00001090: 352c 352e 3238 3038 3138 3420 3130 2e37  5,5.2808184 10.7
-000010a0: 3937 3231 2c36 2e35 3138 3438 3937 2031  9721,6.5184897 1
-000010b0: 312e 3735 3536 3431 2c38 2e34 3031 3432  1.755641,8.40142
-000010c0: 3239 2043 2031 322e 3138 3837 3039 2c39  29 C 12.188709,9
-000010d0: 2e32 3239 3335 3633 2031 322e 3432 3139  .2293563 12.4219
-000010e0: 3236 2c31 302e 3136 3235 3638 2031 322e  26,10.162568 12.
-000010f0: 3431 3739 3038 2c31 312e 3039 3735 3037  417908,11.097507
-00001100: 207a 204d 2031 312e 3533 3735 3439 2c30   z M 11.537549,0
-00001110: 2e37 3934 3737 3735 3620 4320 3131 2e33  .79477756 C 11.3
-00001120: 3638 3031 312c 322e 3935 3331 3633 3620  68011,2.9531636 
-00001130: 392e 3539 3238 3130 352c 342e 3834 3933  9.5928105,4.8493
-00001140: 3934 2037 2e34 3532 3834 3535 2c35 2e31  94 7.4528455,5.1
-00001150: 3731 3132 3720 4320 352e 3439 3334 3033  71127 C 5.493403
-00001160: 352c 352e 3530 3538 3436 3720 332e 3336  5,5.5058467 3.36
-00001170: 3334 3530 352c 342e 3534 3934 3638 3620  34505,4.5494686 
-00001180: 322e 3339 3538 3133 352c 322e 3739 3436  2.3958135,2.7946
-00001190: 3538 3620 4320 322e 3034 3438 3135 352c  586 C 2.0448155,
-000011a0: 322e 3138 3138 3734 3620 312e 3832 3735  2.1818746 1.8275
-000011b0: 3735 352c 312e 3439 3330 3936 3620 312e  755,1.4930966 1.
-000011c0: 3736 3236 3834 352c 302e 3738 3939 3337  7626845,0.789937
-000011d0: 3536 204d 2036 2e36 3033 3936 3235 2c31  56 M 6.6039625,1
-000011e0: 362e 3839 3035 3138 2043 2036 2e36 3033  6.890518 C 6.603
-000011f0: 3936 3235 2c31 382e 3939 3730 3331 2036  9625,18.997031 6
-00001200: 2e36 3033 3936 3235 2c32 312e 3130 3335  .6039625,21.1035
-00001210: 3435 2036 2e36 3033 3936 3235 2c32 332e  45 6.6039625,23.
-00001220: 3231 3030 3538 204d 2033 2e39 3730 3832  210058 M 3.97082
-00001230: 3135 2c32 302e 3537 3639 3136 2043 2035  15,20.576916 C 5
-00001240: 2e37 3236 3234 3735 2c32 302e 3537 3639  .7262475,20.5769
-00001250: 3136 2037 2e34 3831 3637 3835 2c32 302e  16 7.4816785,20.
-00001260: 3537 3639 3136 2039 2e32 3337 3130 3435  576916 9.2371045
-00001270: 2c32 302e 3537 3639 3136 2720 7374 796c  ,20.576916' styl
-00001280: 653d 2773 7472 6f6b 653a 2470 6c61 6e65  e='stroke:$plane
-00001290: 7473 5f63 6f6c 6f72 5f32 3b73 7472 6f6b  ts_color_2;strok
-000012a0: 652d 7769 6474 683a 3270 783b 2066 696c  e-width:2px; fil
-000012b0: 6c3a 6e6f 6e65 3b27 202f 3e0d 0a20 2020  l:none;' />..   
-000012c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000012d0: 203c 2f67 3e0d 0a20 2020 2020 2020 2020   </g>..         
-000012e0: 2020 2020 2020 203c 2f73 796d 626f 6c3e         </symbol>
-000012f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001300: 2020 3c73 796d 626f 6c20 6964 3d27 5665    <symbol id='Ve
-00001310: 6e75 7327 3e0d 0a20 2020 2020 2020 2020  nus'>..         
-00001320: 2020 2020 2020 2020 2020 203c 6720 7472             <g tr
-00001330: 616e 7366 6f72 6d3d 2774 7261 6e73 6c61  ansform='transla
-00001340: 7465 2830 2c32 2927 3e0d 0a20 2020 2020  te(0,2)'>..     
-00001350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001360: 2020 203c 6720 7472 616e 7366 6f72 6d3d     <g transform=
-00001370: 2773 6361 6c65 282e 3929 273e 0d0a 2020  'scale(.9)'>..  
-00001380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001390: 2020 2020 2020 2020 2020 3c70 6174 6820            <path 
-000013a0: 643d 274d 2031 382e 3430 3037 3033 2c37  d='M 18.400703,7
-000013b0: 2e33 3636 3734 3833 2043 2031 382e 3432  .3667483 C 18.42
-000013c0: 3339 362c 392e 3636 3535 3332 3920 3137  396,9.6655329 17
-000013d0: 2e31 3730 3130 322c 3131 2e39 3134 3537  .170102,11.91457
-000013e0: 3920 3135 2e32 3138 3937 322c 3133 2e31  9 15.218972,13.1
-000013f0: 3133 3732 3820 4320 3133 2e31 3632 3435  13728 C 13.16245
-00001400: 392c 3134 2e34 3237 3235 3320 3130 2e33  9,14.427253 10.3
-00001410: 3839 3835 352c 3134 2e34 3736 3737 3220  89855,14.476772 
-00001420: 382e 3238 3731 3636 332c 3133 2e32 3339  8.2871663,13.239
-00001430: 3730 3920 4320 362e 3237 3335 3835 312c  709 C 6.2735851,
-00001440: 3132 2e31 3030 3532 3420 342e 3933 3336  12.100524 4.9336
-00001450: 3333 2c39 2e38 3634 3033 3233 2034 2e38  33,9.8640323 4.8
-00001460: 3937 3939 3135 2c37 2e35 3431 3438 3034  979915,7.5414804
-00001470: 2043 2034 2e38 3137 3336 3137 2c35 2e32   C 4.8173617,5.2
-00001480: 3637 3835 3932 2035 2e39 3835 3531 3936  678592 5.9855196
-00001490: 2c33 2e30 3039 3030 3031 2037 2e38 3732  ,3.0090001 7.872
-000014a0: 3838 3037 2c31 2e37 3533 3034 3731 2043  8807,1.7530471 C
-000014b0: 2039 2e38 3830 3339 3135 2c30 2e33 3635   9.8803915,0.365
-000014c0: 3039 3534 3620 3132 2e36 3438 3930 362c  09546 12.648906,
-000014d0: 302e 3231 3635 3731 3436 2031 342e 3739  0.21657146 14.79
-000014e0: 3438 3439 2c31 2e33 3735 3238 3331 2043  4849,1.3752831 C
-000014f0: 2031 362e 3836 3937 3732 2c32 2e34 3531   16.869772,2.451
-00001500: 3436 3333 2031 382e 3239 3632 3431 2c34  4633 18.296241,4
-00001510: 2e36 3733 3134 3533 2031 382e 3339 3139  .6731453 18.3919
-00001520: 3138 2c37 2e30 3138 3337 3233 2043 2031  18,7.0183723 C 1
-00001530: 382e 3339 3737 3831 2c37 2e31 3334 3339  8.397781,7.13439
-00001540: 3633 2031 382e 3430 3037 3033 2c37 2e32  63 18.400703,7.2
-00001550: 3530 3537 3233 2031 382e 3430 3037 3033  505723 18.400703
-00001560: 2c37 2e33 3636 3734 3833 207a 204d 2031  ,7.3667483 z M 1
-00001570: 312e 3634 3832 3839 2c31 342e 3133 3636  1.648289,14.1366
-00001580: 3839 2043 2031 312e 3634 3832 3839 2c31  89 C 11.648289,1
-00001590: 372e 3030 3837 3634 2031 312e 3634 3832  7.008764 11.6482
-000015a0: 3839 2c31 392e 3838 3038 3420 3131 2e36  89,19.88084 11.6
-000015b0: 3438 3238 392c 3232 2e37 3532 3931 3520  48289,22.752915 
-000015c0: 4d20 372e 3936 3531 3333 332c 3139 2e30  M 7.9651333,19.0
-000015d0: 3630 3234 3320 4320 3130 2e34 3230 3537  60243 C 10.42057
-000015e0: 2c31 392e 3036 3032 3433 2031 322e 3837  ,19.060243 12.87
-000015f0: 3630 3038 2c31 392e 3036 3032 3433 2031  6008,19.060243 1
-00001600: 352e 3333 3134 3434 2c31 392e 3036 3032  5.331444,19.0602
-00001610: 3433 2720 7374 796c 653d 2773 7472 6f6b  43' style='strok
-00001620: 653a 2470 6c61 6e65 7473 5f63 6f6c 6f72  e:$planets_color
-00001630: 5f33 3b73 7472 6f6b 652d 7769 6474 683a  _3;stroke-width:
-00001640: 3270 783b 2066 696c 6c3a 6e6f 6e65 3b27  2px; fill:none;'
-00001650: 202f 3e0d 0a20 2020 2020 2020 2020 2020   />..           
-00001660: 2020 2020 2020 2020 2020 2020 203c 2f67               </g
-00001670: 3e0d 0a20 2020 2020 2020 2020 2020 2020  >..             
-00001680: 2020 2020 2020 203c 2f67 3e0d 0a20 2020         </g>..   
-00001690: 2020 2020 2020 2020 2020 2020 203c 2f73               </s
-000016a0: 796d 626f 6c3e 0d0a 2020 2020 2020 2020  ymbol>..        
-000016b0: 2020 2020 2020 2020 3c73 796d 626f 6c20          <symbol 
-000016c0: 6964 3d27 4d61 7273 273e 0d0a 2020 2020  id='Mars'>..    
-000016d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000016e0: 3c67 2074 7261 6e73 666f 726d 3d27 7472  <g transform='tr
-000016f0: 616e 736c 6174 6528 312c 3329 273e 0d0a  anslate(1,3)'>..
-00001700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001710: 2020 2020 2020 2020 3c67 2074 7261 6e73          <g trans
-00001720: 666f 726d 3d27 7363 616c 6528 2e39 2927  form='scale(.9)'
-00001730: 3e0d 0a20 2020 2020 2020 2020 2020 2020  >..             
-00001740: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00001750: 7061 7468 2064 3d27 4d20 3139 2e38 3336  path d='M 19.836
-00001760: 3832 382c 312e 3232 3638 3538 3520 4320  828,1.2268585 C 
-00001770: 3137 2e34 3234 3432 322c 332e 3632 3538  17.424422,3.6258
-00001780: 3737 3620 3135 2e30 3132 3030 382c 362e  776 15.012008,6.
-00001790: 3032 3439 3034 3720 3132 2e35 3939 3539  0249047 12.59959
-000017a0: 342c 382e 3432 3339 3331 3720 4d20 3133  4,8.4239317 M 13
-000017b0: 2e35 3836 3133 312c 312e 3330 3332 3835  .586131,1.303285
-000017c0: 3320 4320 3135 2e36 3431 3632 322c 312e  3 C 15.641622,1.
-000017d0: 3330 3332 3835 3320 3137 2e36 3937 3130  3032853 17.69710
-000017e0: 352c 312e 3330 3332 3835 3320 3139 2e37  5,1.3032853 19.7
-000017f0: 3532 3539 352c 312e 3330 3332 3835 3320  52595,1.3032853 
-00001800: 4320 3139 2e37 3532 3539 352c 332e 3334  C 19.752595,3.34
-00001810: 3733 3638 3620 3139 2e37 3532 3630 332c  73686 19.752603,
-00001820: 352e 3339 3134 3531 3720 3139 2e37 3532  5.3914517 19.752
-00001830: 3630 332c 372e 3433 3535 3335 3727 2073  603,7.4355357' s
-00001840: 7479 6c65 3d27 7374 726f 6b65 3a24 706c  tyle='stroke:$pl
-00001850: 616e 6574 735f 636f 6c6f 725f 343b 7374  anets_color_4;st
-00001860: 726f 6b65 2d77 6964 7468 3a32 7078 3b20  roke-width:2px; 
-00001870: 6669 6c6c 3a6e 6f6e 653b 2720 2f3e 0d0a  fill:none;' />..
-00001880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001890: 2020 2020 2020 2020 2020 2020 3c70 6174              <pat
-000018a0: 6820 643d 274d 2031 352e 3230 3838 3335  h d='M 15.208835
-000018b0: 2c31 332e 3133 3737 3131 2043 2031 352e  ,13.137711 C 15.
-000018c0: 3234 3537 3837 2c31 352e 3838 3833 3039  245787,15.888309
-000018d0: 2031 332e 3439 3735 3233 2c31 382e 3534   13.497523,18.54
-000018e0: 3334 3620 3130 2e39 3639 3034 332c 3139  346 10.969043,19
-000018f0: 2e36 3137 3733 2043 2038 2e34 3538 3431  .61773 C 8.45841
-00001900: 3735 2c32 302e 3734 3930 3336 2035 2e33  75,20.749036 5.3
-00001910: 3135 3534 3238 2c32 302e 3231 3634 3120  155428,20.21641 
-00001920: 332e 3332 3336 3330 362c 3138 2e33 3132  3.3236306,18.312
-00001930: 3834 3320 4320 312e 3332 3934 3738 392c  843 C 1.3294789,
-00001940: 3136 2e35 3032 3638 3620 302e 3535 3436  16.502686 0.5546
-00001950: 3631 3237 2c31 332e 3530 3436 3738 2031  6127,13.504678 1
-00001960: 2e34 3133 3336 3135 2c31 302e 3935 3333  .4133615,10.9533
-00001970: 3032 2043 2032 2e32 3438 3537 3231 2c38  02 C 2.2485721,8
-00001980: 2e32 3833 3334 3532 2034 2e38 3030 3530  .2833452 4.80050
-00001990: 3433 2c36 2e32 3636 3030 3735 2037 2e35  43,6.2660075 7.5
-000019a0: 3935 3231 382c 362e 3038 3834 3236 3620  95218,6.0884266 
-000019b0: 4320 3130 2e32 3837 3033 322c 352e 3834  C 10.287032,5.84
-000019c0: 3637 3938 3420 3133 2e30 3232 3334 382c  67984 13.022348,
-000019d0: 372e 3332 3331 3034 3820 3134 2e33 3133  7.3231048 14.313
-000019e0: 3836 2c39 2e36 3933 3830 3831 2043 2031  86,9.6938081 C 1
-000019f0: 342e 3930 3131 3633 2c31 302e 3733 3939  4.901163,10.7399
-00001a00: 3637 2031 352e 3231 3130 3832 2c31 312e  67 15.211082,11.
-00001a10: 3933 3831 3936 2031 352e 3230 3838 3335  938196 15.208835
-00001a20: 2c31 332e 3133 3737 3131 207a 2720 7374  ,13.137711 z' st
-00001a30: 796c 653d 2773 7472 6f6b 653a 2470 6c61  yle='stroke:$pla
-00001a40: 6e65 7473 5f63 6f6c 6f72 5f34 3b73 7472  nets_color_4;str
-00001a50: 6f6b 652d 7769 6474 683a 3270 783b 2066  oke-width:2px; f
-00001a60: 696c 6c3a 6e6f 6e65 3b27 202f 3e0d 0a20  ill:none;' />.. 
-00001a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a80: 2020 2020 2020 203c 2f67 3e0d 0a20 2020         </g>..   
-00001a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001aa0: 203c 2f67 3e0d 0a20 2020 2020 2020 2020   </g>..         
-00001ab0: 2020 2020 2020 203c 2f73 796d 626f 6c3e         </symbol>
-00001ac0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001ad0: 2020 3c73 796d 626f 6c20 6964 3d27 4a75    <symbol id='Ju
-00001ae0: 7069 7465 7227 3e0d 0a20 2020 2020 2020  piter'>..       
-00001af0: 2020 2020 2020 2020 2020 2020 203c 6720               <g 
-00001b00: 7472 616e 7366 6f72 6d3d 2774 7261 6e73  transform='trans
-00001b10: 6c61 7465 2831 2c33 2927 3e0d 0a20 2020  late(1,3)'>..   
-00001b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b30: 2020 2020 203c 6720 7472 616e 7366 6f72       <g transfor
-00001b40: 6d3d 2773 6361 6c65 282e 3929 273e 0d0a  m='scale(.9)'>..
-00001b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b60: 2020 2020 2020 2020 2020 2020 3c70 6174              <pat
-00001b70: 6820 643d 274d 2031 362e 3930 3330 3038  h d='M 16.903008
-00001b80: 2c30 2e39 3938 3439 3135 3720 4c20 3136  ,0.99849157 L 16
-00001b90: 2e39 3033 3030 382c 3233 2e30 3031 3531  .903008,23.00151
-00001ba0: 3220 4d20 3230 2e35 3330 3237 382c 3137  2 M 20.530278,17
-00001bb0: 2e33 3539 3731 3220 4c20 322e 3939 3834  .359712 L 2.9984
-00001bc0: 3838 342c 3137 2e33 3539 3731 3220 4d20  884,17.359712 M 
-00001bd0: 342e 3831 3231 3138 342c 382e 3839 3730  4.8121184,8.8970
-00001be0: 3132 2043 2034 2e32 3037 3537 3834 2c38  12 C 4.2075784,8
-00001bf0: 2e38 3937 3031 3220 322e 3939 3834 3838  .897012 2.998488
-00001c00: 342c 382e 3333 3238 3332 2032 2e39 3938  4,8.332832 2.998
-00001c10: 3438 3834 2c36 2e30 3736 3131 3220 4320  4884,6.076112 C 
-00001c20: 322e 3939 3834 3838 342c 332e 3831 3933  2.9984884,3.8193
-00001c30: 3832 2035 2e34 3136 3636 3834 2c31 2e35  82 5.4166684,1.5
-00001c40: 3632 3637 3136 2037 2e38 3334 3834 3834  626716 7.8348484
-00001c50: 2c31 2e35 3632 3637 3136 2043 2031 302e  ,1.5626716 C 10.
-00001c60: 3235 3330 3238 2c31 2e35 3632 3637 3136  253028,1.5626716
-00001c70: 2031 322e 3637 3131 3938 2c33 2e32 3535   12.671198,3.255
-00001c80: 3231 3220 3132 2e36 3731 3139 382c 372e  212 12.671198,7.
-00001c90: 3230 3434 3732 2043 2031 322e 3637 3131  204472 C 12.6711
-00001ca0: 3938 2c31 312e 3135 3337 3332 2039 2e36  98,11.153732 9.6
-00001cb0: 3438 3437 3834 2c31 372e 3335 3937 3132  484784,17.359712
-00001cc0: 2033 2e36 3033 3032 3834 2c31 372e 3335   3.6030284,17.35
-00001cd0: 3937 3132 2720 7374 796c 653d 2773 7472  9712' style='str
-00001ce0: 6f6b 653a 2470 6c61 6e65 7473 5f63 6f6c  oke:$planets_col
-00001cf0: 6f72 5f35 3b73 7472 6f6b 652d 7769 6474  or_5;stroke-widt
-00001d00: 683a 3270 783b 2066 696c 6c3a 6e6f 6e65  h:2px; fill:none
-00001d10: 3b27 202f 3e0d 0a20 2020 2020 2020 2020  ;' />..         
-00001d20: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00001d30: 2f67 3e0d 0a20 2020 2020 2020 2020 2020  /g>..           
-00001d40: 2020 2020 2020 2020 203c 2f67 3e0d 0a20           </g>.. 
-00001d50: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00001d60: 2f73 796d 626f 6c3e 0d0a 2020 2020 2020  /symbol>..      
-00001d70: 2020 2020 2020 2020 2020 3c73 796d 626f            <symbo
-00001d80: 6c20 6964 3d27 5361 7475 726e 273e 0d0a  l id='Saturn'>..
-00001d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001da0: 2020 2020 3c67 2074 7261 6e73 666f 726d      <g transform
-00001db0: 3d27 7472 616e 736c 6174 6528 312c 3229  ='translate(1,2)
-00001dc0: 273e 0d0a 2020 2020 2020 2020 2020 2020  '>..            
-00001dd0: 2020 2020 2020 2020 2020 2020 3c70 6174              <pat
-00001de0: 6820 643d 274d 2038 2e33 3834 3433 3439  h d='M 8.3844349
-00001df0: 2c30 2e39 3032 3033 3233 3120 4c20 382e  ,0.90203231 L 8.
-00001e00: 3338 3434 3334 392c 3138 2e32 3938 3835  3844349,18.29885
-00001e10: 3220 4d20 352e 3433 3439 3434 392c 332e  2 M 5.4349449,3.
-00001e20: 3735 3135 3132 3320 4c20 3132 2e36 3638  7515123 L 12.668
-00001e30: 3734 352c 332e 3735 3135 3132 3320 4d20  745,3.7515123 M 
-00001e40: 3136 2e38 3233 3837 352c 3231 2e38 3938  16.823875,21.898
-00001e50: 3139 3220 4320 3136 2e32 3231 3035 352c  192 C 16.221055,
-00001e60: 3232 2e34 3938 3038 3220 3135 2e36 3138  22.498082 15.618
-00001e70: 3233 352c 3233 2e30 3937 3937 3220 3135  235,23.097972 15
-00001e80: 2e30 3135 3431 352c 3233 2e30 3937 3937  .015415,23.09797
-00001e90: 3220 4320 3134 2e34 3132 3630 352c 3233  2 C 14.412605,23
-00001ea0: 2e30 3937 3937 3220 3133 2e32 3036 3937  .097972 13.20697
-00001eb0: 352c 3232 2e34 3938 3038 3220 3133 2e32  5,22.498082 13.2
-00001ec0: 3036 3937 352c 3231 2e32 3938 3330 3220  06975,21.298302 
-00001ed0: 4320 3133 2e32 3036 3937 352c 3230 2e30  C 13.206975,20.0
-00001ee0: 3938 3532 3220 3133 2e38 3039 3738 352c  98522 13.809785,
-00001ef0: 3138 2e38 3938 3734 3220 3135 2e30 3135  18.898742 15.015
-00001f00: 3431 352c 3137 2e36 3938 3936 3220 4320  415,17.698962 C 
-00001f10: 3136 2e32 3231 3035 352c 3136 2e34 3939  16.221055,16.499
-00001f20: 3138 3220 3137 2e34 3236 3638 352c 3134  182 17.426685,14
-00001f30: 2e30 3939 3632 3220 3137 2e34 3236 3638  .099622 17.42668
-00001f40: 352c 3131 2e37 3030 3035 3220 4320 3137  5,11.700052 C 17
-00001f50: 2e34 3236 3638 352c 392e 3330 3034 3932  .426685,9.300492
-00001f60: 3320 3136 2e32 3231 3035 352c 362e 3930  3 16.221055,6.90
-00001f70: 3039 3332 3320 3133 2e38 3039 3738 352c  09323 13.809785,
-00001f80: 362e 3930 3039 3332 3320 4320 3131 2e35  6.9009323 C 11.5
-00001f90: 3239 3231 352c 362e 3930 3039 3332 3320  29215,6.9009323 
-00001fa0: 392e 3539 3030 3634 392c 382e 3130 3037  9.5900649,8.1007
-00001fb0: 3132 3320 382e 3338 3434 3334 392c 3130  123 8.3844349,10
-00001fc0: 2e35 3030 3238 3227 2073 7479 6c65 3d27  .500282' style='
-00001fd0: 7374 726f 6b65 3a24 706c 616e 6574 735f  stroke:$planets_
-00001fe0: 636f 6c6f 725f 363b 7374 726f 6b65 2d77  color_6;stroke-w
-00001ff0: 6964 7468 3a32 7078 3b20 6669 6c6c 3a6e  idth:2px; fill:n
-00002000: 6f6e 653b 2720 2f3e 0d0a 2020 2020 2020  one;' />..      
-00002010: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-00002020: 673e 0d0a 2020 2020 2020 2020 2020 2020  g>..            
-00002030: 2020 2020 3c2f 7379 6d62 6f6c 3e0d 0a20      </symbol>.. 
-00002040: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00002050: 7379 6d62 6f6c 2069 643d 2755 7261 6e75  symbol id='Uranu
-00002060: 7327 3e0d 0a20 2020 2020 2020 2020 2020  s'>..           
-00002070: 2020 2020 2020 2020 203c 6720 7472 616e           <g tran
-00002080: 7366 6f72 6d3d 2774 7261 6e73 6c61 7465  sform='translate
-00002090: 2832 2c34 2927 3e0d 0a20 2020 2020 2020  (2,4)'>..       
-000020a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000020b0: 203c 6720 7472 616e 7366 6f72 6d3d 2773   <g transform='s
-000020c0: 6361 6c65 282e 3829 273e 0d0a 2020 2020  cale(.8)'>..    
-000020d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000020e0: 2020 2020 2020 2020 3c70 6174 6820 643d          <path d=
-000020f0: 274d 2034 2e36 3737 3230 3636 2c31 362e  'M 4.6772066,16.
-00002100: 3039 3734 3233 2043 2033 2e32 3034 3234  097423 C 3.20424
-00002110: 3236 2c31 362e 3039 3734 3233 2031 2e37  26,16.097423 1.7
-00002120: 3331 3237 3736 2c31 362e 3039 3734 3233  312776,16.097423
-00002130: 2030 2e32 3538 3330 3636 312c 3136 2e30   0.25830661,16.0
-00002140: 3937 3432 3320 4320 302e 3332 3138 3530  97423 C 0.321850
-00002150: 3631 2c31 352e 3839 3438 3739 2030 2e31  61,15.894879 0.1
-00002160: 3139 3935 3636 312c 3135 2e34 3835 3039  1995661,15.48509
-00002170: 3620 302e 3337 3937 3633 3631 2c31 352e  6 0.37976361,15.
-00002180: 3433 3537 3837 2043 2031 2e31 3830 3937  435787 C 1.18097
-00002190: 3236 2c31 352e 3233 3534 3835 2031 2e39  26,15.235485 1.9
-000021a0: 3832 3138 3236 2c31 352e 3033 3531 3832  821826,15.035182
-000021b0: 2032 2e37 3833 3339 3236 2c31 342e 3833   2.7833926,14.83
-000021c0: 3438 3820 4320 322e 3738 3333 3932 362c  488 C 2.7833926,
-000021d0: 3130 2e36 3236 3430 3120 322e 3738 3333  10.626401 2.7833
-000021e0: 3932 362c 362e 3431 3739 3239 2032 2e37  926,6.417929 2.7
-000021f0: 3833 3339 3236 2c32 2e32 3039 3435 3032  833926,2.2094502
-00002200: 2043 2031 2e39 3431 3639 3936 2c31 2e39   C 1.9416996,1.9
-00002210: 3939 3032 3835 2031 2e31 3030 3030 3536  990285 1.1000056
-00002220: 2c31 2e37 3838 3630 3034 2030 2e32 3538  ,1.7886004 0.258
-00002230: 3330 3636 312c 312e 3537 3831 3738 3720  30661,1.5781787 
-00002240: 4320 302e 3332 3338 3037 3631 2c31 2e33  C 0.32380761,1.3
-00002250: 3931 3532 3433 2030 2e31 3135 3730 3236  915243 0.1157026
-00002260: 312c 302e 3933 3132 3634 3332 2030 2e33  1,0.93126432 0.3
-00002270: 3833 3530 3036 312c 302e 3934 3639 3037  8350061,0.946907
-00002280: 3232 2043 2031 2e38 3134 3733 3736 2c30  22 C 1.8147376,0
-00002290: 2e39 3436 3930 3732 3220 332e 3234 3539  .94690722 3.2459
-000022a0: 3639 362c 302e 3934 3639 3037 3232 2034  696,0.94690722 4
-000022b0: 2e36 3737 3230 3636 2c30 2e39 3436 3930  .6772066,0.94690
-000022c0: 3732 3220 4320 342e 3637 3732 3036 362c  722 C 4.6772066,
-000022d0: 352e 3939 3730 3739 3220 342e 3637 3732  5.9970792 4.6772
-000022e0: 3036 362c 3131 2e30 3437 3235 3120 342e  066,11.047251 4.
-000022f0: 3637 3732 3036 362c 3136 2e30 3937 3432  6772066,16.09742
-00002300: 3320 7a20 2720 7374 796c 653d 2773 7472  3 z ' style='str
-00002310: 6f6b 653a 2470 6c61 6e65 7473 5f63 6f6c  oke:$planets_col
-00002320: 6f72 5f37 3b73 7472 6f6b 652d 7769 6474  or_7;stroke-widt
-00002330: 683a 3170 783b 2066 696c 6c3a 2470 6c61  h:1px; fill:$pla
-00002340: 6e65 7473 5f63 6f6c 6f72 5f35 3b27 202f  nets_color_5;' /
-00002350: 3e0d 0a20 2020 2020 2020 2020 2020 2020  >..             
-00002360: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00002370: 7061 7468 2064 3d27 4d20 3138 2e35 3635  path d='M 18.565
-00002380: 3138 2c31 362e 3039 3734 3233 2043 2032  18,16.097423 C 2
-00002390: 302e 3033 3831 3531 2c31 362e 3039 3734  0.038151,16.0974
-000023a0: 3233 2032 312e 3531 3131 3136 2c31 362e  23 21.511116,16.
-000023b0: 3039 3734 3233 2032 322e 3938 3430 3831  097423 22.984081
-000023c0: 2c31 362e 3039 3734 3233 2043 2032 322e  ,16.097423 C 22.
-000023d0: 3932 3035 3433 2c31 352e 3839 3438 3739  920543,15.894879
-000023e0: 2032 332e 3132 3234 332c 3135 2e34 3835   23.12243,15.485
-000023f0: 3039 3620 3232 2e38 3632 3633 312c 3135  096 22.862631,15
-00002400: 2e34 3335 3738 3720 4320 3232 2e30 3631  .435787 C 22.061
-00002410: 3432 312c 3135 2e32 3335 3438 3520 3231  421,15.235485 21
-00002420: 2e32 3630 3231 312c 3135 2e30 3335 3138  .260211,15.03518
-00002430: 3220 3230 2e34 3538 3939 352c 3134 2e38  2 20.458995,14.8
-00002440: 3334 3838 2043 2032 302e 3435 3839 3935  3488 C 20.458995
-00002450: 2c31 302e 3632 3634 3031 2032 302e 3435  ,10.626401 20.45
-00002460: 3839 3935 2c36 2e34 3137 3932 3920 3230  8995,6.417929 20
-00002470: 2e34 3538 3939 352c 322e 3230 3934 3530  .458995,2.209450
-00002480: 3220 4320 3231 2e33 3030 3639 342c 312e  2 C 21.300694,1.
-00002490: 3939 3930 3238 3520 3232 2e31 3432 3338  9990285 22.14238
-000024a0: 382c 312e 3738 3836 3030 3420 3232 2e39  8,1.7886004 22.9
-000024b0: 3834 3038 312c 312e 3537 3831 3738 3720  84081,1.5781787 
-000024c0: 4320 3232 2e39 3138 3538 372c 312e 3339  C 22.918587,1.39
-000024d0: 3135 3234 3320 3233 2e31 3236 3639 312c  15243 23.126691,
-000024e0: 302e 3933 3132 3634 3332 2032 322e 3835  0.93126432 22.85
-000024f0: 3838 3933 2c30 2e39 3436 3930 3732 3220  8893,0.94690722 
-00002500: 4320 3231 2e34 3237 3635 362c 302e 3934  C 21.427656,0.94
-00002510: 3639 3037 3232 2031 392e 3939 3634 3138  690722 19.996418
-00002520: 2c30 2e39 3436 3930 3732 3220 3138 2e35  ,0.94690722 18.5
-00002530: 3635 3138 2c30 2e39 3436 3930 3732 3220  6518,0.94690722 
-00002540: 4320 3138 2e35 3635 3138 2c35 2e39 3937  C 18.56518,5.997
-00002550: 3037 3932 2031 382e 3536 3531 382c 3131  0792 18.56518,11
-00002560: 2e30 3437 3235 3120 3138 2e35 3635 3138  .047251 18.56518
-00002570: 2c31 362e 3039 3734 3233 207a 2027 2073  ,16.097423 z ' s
-00002580: 7479 6c65 3d27 7374 726f 6b65 3a24 706c  tyle='stroke:$pl
-00002590: 616e 6574 735f 636f 6c6f 725f 373b 7374  anets_color_7;st
-000025a0: 726f 6b65 2d77 6964 7468 3a31 7078 3b20  roke-width:1px; 
-000025b0: 6669 6c6c 3a24 706c 616e 6574 735f 636f  fill:$planets_co
-000025c0: 6c6f 725f 353b 2720 2f3e 0d0a 2020 2020  lor_5;' />..    
-000025d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000025e0: 2020 2020 2020 2020 3c70 6174 6820 643d          <path d=
-000025f0: 274d 2034 2e30 3435 3933 3536 2c38 2e35  'M 4.0459356,8.5
-00002600: 3232 3136 3532 2043 2039 2e30 3936 3130  221652 C 9.09610
-00002610: 3736 2c38 2e35 3232 3136 3532 2031 342e  76,8.5221652 14.
-00002620: 3134 3632 382c 382e 3532 3231 3635 3220  14628,8.5221652 
-00002630: 3139 2e31 3936 3435 322c 382e 3532 3231  19.196452,8.5221
-00002640: 3635 3220 4d20 3131 2e36 3231 3139 342c  652 M 11.621194,
-00002650: 302e 3934 3639 3037 3232 2043 2031 312e  0.94690722 C 11.
-00002660: 3632 3131 3934 2c36 2e34 3137 3932 3920  621194,6.417929 
-00002670: 3131 2e36 3231 3139 342c 3131 2e38 3838  11.621194,11.888
-00002680: 3934 3420 3131 2e36 3231 3139 342c 3137  944 11.621194,17
-00002690: 2e33 3539 3936 3620 4d20 3134 2e31 3436  .359966 M 14.146
-000026a0: 3234 322c 3230 2e35 3136 3334 3220 4320  242,20.516342 C 
-000026b0: 3134 2e32 3237 3935 342c 3232 2e32 3031  14.227954,22.201
-000026c0: 3130 3520 3132 2e32 3735 3636 352c 3233  105 12.275665,23
-000026d0: 2e35 3530 3330 3220 3130 2e37 3235 3637  .550302 10.72567
-000026e0: 382c 3232 2e38 3833 3032 3320 4320 392e  8,22.883023 C 9.
-000026f0: 3133 3935 3736 362c 3232 2e33 3438 3639  1395766,22.34869
-00002700: 3620 382e 3535 3230 3436 362c 3230 2e30  6 8.5520466,20.0
-00002710: 3839 3638 3520 392e 3730 3334 3937 362c  89685 9.7034976,
-00002720: 3138 2e38 3630 3837 3120 4320 3130 2e37  18.860871 C 10.7
-00002730: 3234 3037 352c 3137 2e36 3038 3138 3220  24075,17.608182 
-00002740: 3132 2e39 3539 3436 342c 3137 2e37 3436  12.959464,17.746
-00002750: 3438 3120 3133 2e37 3630 3733 312c 3139  481 13.760731,19
-00002760: 2e31 3734 3830 3820 4320 3134 2e30 3131  .174808 C 14.011
-00002770: 3333 392c 3139 2e35 3734 3120 3134 2e31  339,19.5741 14.1
-00002780: 3438 3138 2c32 302e 3034 3436 3434 2031  4818,20.044644 1
-00002790: 342e 3134 3632 3432 2c32 302e 3531 3633  4.146242,20.5163
-000027a0: 3432 207a 2027 2073 7479 6c65 3d27 7374  42 z ' style='st
-000027b0: 726f 6b65 3a24 706c 616e 6574 735f 636f  roke:$planets_co
-000027c0: 6c6f 725f 373b 7374 726f 6b65 2d77 6964  lor_7;stroke-wid
-000027d0: 7468 3a32 7078 3b20 6669 6c6c 3a6e 6f6e  th:2px; fill:non
-000027e0: 653b 2720 2f3e 0d0a 2020 2020 2020 2020  e;' />..        
-000027f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002800: 3c2f 673e 0d0a 2020 2020 2020 2020 2020  </g>..          
-00002810: 2020 2020 2020 2020 2020 3c2f 673e 0d0a            </g>..
-00002820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002830: 3c2f 7379 6d62 6f6c 3e0d 0a20 2020 2020  </symbol>..     
-00002840: 2020 2020 2020 2020 2020 203c 7379 6d62             <symb
-00002850: 6f6c 2069 643d 274e 6570 7475 6e65 273e  ol id='Neptune'>
-00002860: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002870: 2020 2020 2020 3c67 2074 7261 6e73 666f        <g transfo
-00002880: 726d 3d27 7472 616e 736c 6174 6528 322c  rm='translate(2,
-00002890: 3429 273e 0d0a 2020 2020 2020 2020 2020  4)'>..          
-000028a0: 2020 2020 2020 2020 2020 2020 2020 3c67                <g
-000028b0: 2074 7261 6e73 666f 726d 3d27 7363 616c   transform='scal
-000028c0: 6528 2e39 2927 3e0d 0a20 2020 2020 2020  e(.9)'>..       
-000028d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000028e0: 2020 2020 203c 7061 7468 2064 3d27 4d20       <path d='M 
-000028f0: 332e 3838 3633 3037 2c32 2e32 3039 3831  3.886307,2.20981
-00002900: 3334 2043 2032 2e32 3732 3832 3439 2c31  34 C 2.2728249,1
-00002910: 332e 3137 3233 3336 2034 2e39 3631 3937  3.172336 4.96197
-00002920: 3138 2c31 342e 3831 3637 3138 2031 302e  18,14.816718 10.
-00002930: 3334 3032 3635 2c31 342e 3831 3637 3138  340265,14.816718
-00002940: 2043 2031 352e 3731 3835 3637 2c31 342e   C 15.718567,14.
-00002950: 3831 3637 3138 2031 382e 3430 3737 3231  816718 18.407721
-00002960: 2c31 332e 3137 3233 3336 2031 362e 3739  ,13.172336 16.79
-00002970: 3432 3331 2c32 2e32 3039 3831 3334 204d  4231,2.2098134 M
-00002980: 2031 302e 3334 3032 3635 2c33 2e33 3036   10.340265,3.306
-00002990: 3036 3538 204c 2031 302e 3334 3032 3635  0658 L 10.340265
-000029a0: 2c32 332e 3538 3637 3336 204d 2036 2e30  ,23.586736 M 6.0
-000029b0: 3337 3632 392c 3139 2e32 3031 3732 3720  37629,19.201727 
-000029c0: 4c20 3134 2e36 3432 3930 392c 3139 2e32  L 14.642909,19.2
-000029d0: 3031 3732 3720 4d20 302e 3931 3138 3030  01727 M 0.911800
-000029e0: 3237 2c33 2e37 3233 3038 3038 204c 2033  27,3.7230808 L 3
-000029f0: 2e39 3633 3537 3935 2c31 2e34 3130 3333  .9635795,1.41033
-00002a00: 3631 204c 2036 2e32 3332 3836 3839 2c34  61 L 6.2328689,4
-00002a10: 2e35 3230 3534 3738 204d 2037 2e35 3939  .5205478 M 7.599
-00002a20: 3834 3836 2c36 2e33 3432 3132 3438 204c  8486,6.3421248 L
-00002a30: 2031 302e 3235 3930 3535 2c33 2e35 3731   10.259055,3.571
-00002a40: 3331 3038 204c 2031 322e 3937 3738 3132  3108 L 12.977812
-00002a50: 2c36 2e32 3831 3434 3238 204d 2031 342e  ,6.2814428 M 14.
-00002a60: 3430 3738 3839 2c34 2e37 3132 3035 3238  407889,4.7120528
-00002a70: 204c 2031 362e 3731 3539 3436 2c31 2e36   L 16.715946,1.6
-00002a80: 3331 3630 3835 204c 2031 392e 3733 3835  316085 L 19.7385
-00002a90: 3036 2c33 2e39 3833 3836 3238 2720 7374  06,3.9838628' st
-00002aa0: 796c 653d 2773 7472 6f6b 653a 2470 6c61  yle='stroke:$pla
-00002ab0: 6e65 7473 5f63 6f6c 6f72 5f38 3b73 7472  nets_color_8;str
-00002ac0: 6f6b 652d 7769 6474 683a 3270 783b 2066  oke-width:2px; f
-00002ad0: 696c 6c3a 6e6f 6e65 3b27 202f 3e0d 0a20  ill:none;' />.. 
-00002ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002af0: 2020 2020 2020 203c 2f67 3e0d 0a20 2020         </g>..   
-00002b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b10: 203c 2f67 3e0d 0a20 2020 2020 2020 2020   </g>..         
-00002b20: 2020 2020 2020 203c 2f73 796d 626f 6c3e         </symbol>
-00002b30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002b40: 2020 3c73 796d 626f 6c20 6964 3d27 506c    <symbol id='Pl
-00002b50: 7574 6f27 3e0d 0a20 2020 2020 2020 2020  uto'>..         
-00002b60: 2020 2020 2020 2020 2020 203c 6720 7472             <g tr
-00002b70: 616e 7366 6f72 6d3d 2774 7261 6e73 6c61  ansform='transla
-00002b80: 7465 2830 2c33 2927 3e0d 0a20 2020 2020  te(0,3)'>..     
-00002b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ba0: 2020 203c 6720 7472 616e 7366 6f72 6d3d     <g transform=
-00002bb0: 2773 6361 6c65 282e 3929 273e 0d0a 2020  'scale(.9)'>..  
-00002bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002bd0: 2020 2020 2020 2020 2020 3c70 6174 6820            <path 
-00002be0: 643d 274d 2037 2e32 3938 3833 3839 2c31  d='M 7.2988389,1
-00002bf0: 382e 3136 3936 3731 204c 2031 372e 3137  8.169671 L 17.17
-00002c00: 3032 3939 2c31 382e 3136 3936 3731 204d  0299,18.169671 M
-00002c10: 2031 322e 3233 3435 3639 2c32 332e 3130   12.234569,23.10
-00002c20: 3534 3031 204c 2031 322e 3233 3435 3639  5401 L 12.234569
-00002c30: 2c31 322e 3631 3639 3831 204d 2031 362e  ,12.616981 M 16.
-00002c40: 3535 3333 3039 2c35 2e32 3133 3336 3039  553309,5.2133609
-00002c50: 2043 2031 362e 3535 3333 3039 2c37 2e35   C 16.553309,7.5
-00002c60: 3937 3332 3039 2031 342e 3631 3834 3939  973209 14.618499
-00002c70: 2c39 2e35 3332 3133 3039 2031 322e 3233  ,9.5321309 12.23
-00002c80: 3435 3339 2c39 2e35 3332 3133 3039 2043  4539,9.5321309 C
-00002c90: 2039 2e38 3530 3538 3839 2c39 2e35 3332   9.8505889,9.532
-00002ca0: 3133 3039 2037 2e39 3135 3737 3839 2c37  1309 7.9157789,7
-00002cb0: 2e35 3937 3332 3039 2037 2e39 3135 3737  .5973209 7.91577
-00002cc0: 3839 2c35 2e32 3133 3336 3039 2043 2037  89,5.2133609 C 7
-00002cd0: 2e39 3135 3737 3839 2c32 2e38 3239 3431  .9157789,2.82941
-00002ce0: 3039 2039 2e38 3530 3538 3839 2c30 2e38  09 9.8505889,0.8
-00002cf0: 3934 3630 3038 3720 3132 2e32 3334 3533  9460087 12.23453
-00002d00: 392c 302e 3839 3436 3030 3837 2043 2031  9,0.89460087 C 1
-00002d10: 342e 3631 3834 3939 2c30 2e38 3934 3630  4.618499,0.89460
-00002d20: 3038 3720 3136 2e35 3533 3330 392c 322e  087 16.553309,2.
-00002d30: 3832 3934 3130 3920 3136 2e35 3533 3330  8294109 16.55330
-00002d40: 392c 352e 3231 3333 3630 3920 7a20 4d20  9,5.2133609 z M 
-00002d50: 3139 2e36 3338 3133 392c 352e 3231 3333  19.638139,5.2133
-00002d60: 3630 3920 4320 3139 2e36 3338 3133 392c  609 C 19.638139,
-00002d70: 392e 3330 3031 3530 3920 3136 2e33 3231  9.3001509 16.321
-00002d80: 3332 392c 3132 2e36 3136 3936 3120 3132  329,12.616961 12
-00002d90: 2e32 3334 3533 392c 3132 2e36 3136 3936  .234539,12.61696
-00002da0: 3120 4320 382e 3134 3737 3538 392c 3132  1 C 8.1477589,12
-00002db0: 2e36 3136 3936 3120 342e 3833 3039 3438  .616961 4.830948
-00002dc0: 392c 392e 3330 3031 3530 3920 342e 3833  9,9.3001509 4.83
-00002dd0: 3039 3438 392c 352e 3231 3333 3630 3920  09489,5.2133609 
-00002de0: 4320 342e 3833 3039 3438 392c 352e 3231  C 4.8309489,5.21
-00002df0: 3333 3630 3920 342e 3833 3039 3438 392c  33609 4.8309489,
-00002e00: 352e 3231 3333 3630 3920 342e 3833 3039  5.2133609 4.8309
-00002e10: 3438 392c 352e 3231 3333 3630 3927 2073  489,5.2133609' s
-00002e20: 7479 6c65 3d27 7374 726f 6b65 3a24 706c  tyle='stroke:$pl
-00002e30: 616e 6574 735f 636f 6c6f 725f 393b 2073  anets_color_9; s
-00002e40: 7472 6f6b 652d 7769 6474 683a 3270 783b  troke-width:2px;
-00002e50: 2066 696c 6c3a 6e6f 6e65 3b27 202f 3e0d   fill:none;' />.
-00002e60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002e70: 2020 2020 2020 2020 203c 2f67 3e0d 0a20           </g>.. 
-00002e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002e90: 2020 203c 2f67 3e0d 0a20 2020 2020 2020     </g>..       
-00002ea0: 2020 2020 2020 2020 203c 2f73 796d 626f           </symbo
-00002eb0: 6c3e 0d0a 2020 2020 2020 2020 2020 2020  l>..            
-00002ec0: 2020 2020 3c73 796d 626f 6c20 6964 3d27      <symbol id='
-00002ed0: 4d65 616e 5f4e 6f64 6527 3e0d 0a20 2020  Mean_Node'>..   
-00002ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ef0: 203c 6720 7472 616e 7366 6f72 6d3d 2774   <g transform='t
-00002f00: 7261 6e73 6c61 7465 2830 2c33 2927 3e0d  ranslate(0,3)'>.
-00002f10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002f20: 2020 2020 2020 2020 203c 7061 7468 2064           <path d
-00002f30: 3d27 4d20 382e 3830 3936 3034 362c 302e  ='M 8.8096046,0.
-00002f40: 3037 3536 3636 3839 3720 4320 362e 3431  075666897 C 6.41
-00002f50: 3537 3533 362c 302e 3636 3132 3339 3632  57536,0.66123962
-00002f60: 2034 2e33 3736 3737 3639 2c32 2e35 3330   4.3767769,2.530
-00002f70: 3638 3337 2033 2e36 3633 3436 3536 2c34  6837 3.6634656,4
-00002f80: 2e39 3030 3735 3134 2043 2033 2e30 3533  .9007514 C 3.053
-00002f90: 3630 3731 2c36 2e36 3830 3932 3634 2033  6071,6.6809264 3
-00002fa0: 2e36 3836 3836 3832 2c38 2e36 3233 3839  .6868682,8.62389
-00002fb0: 3031 2034 2e35 3837 3839 3838 2c31 302e  01 4.5878988,10.
-00002fc0: 3138 3634 3337 2043 2035 2e31 3332 3339  186437 C 5.13239
-00002fd0: 3937 2c31 312e 3132 3436 3232 2035 2e39  97,11.124622 5.9
-00002fe0: 3631 3537 3533 2c31 312e 3930 3839 3520  615753,11.90895 
-00002ff0: 362e 3139 3037 3330 322c 3133 2e30 3037  6.1907302,13.007
-00003000: 3930 3620 4320 362e 3539 3137 3230 322c  906 C 6.5917202,
-00003010: 3134 2e34 3834 3438 3820 362e 3438 3837  14.484488 6.4887
-00003020: 3135 362c 3136 2e33 3837 3532 3320 352e  156,16.387523 5.
-00003030: 3137 3233 3738 382c 3137 2e33 3832 3537  1723788,17.38257
-00003040: 3620 4320 342e 3333 3239 3937 342c 3138  6 C 4.3329974,18
-00003050: 2e30 3533 3431 3320 332e 3037 3735 3734  .053413 3.077574
-00003060: 312c 3137 2e34 3535 3033 3420 322e 3832  1,17.455034 2.82
-00003070: 3030 3133 362c 3136 2e34 3831 3139 3620  00136,16.481196 
-00003080: 4320 322e 3339 3136 3535 322c 3135 2e31  C 2.3916552,15.1
-00003090: 3030 3739 3320 332e 3332 3331 3839 382c  00793 3.3231898,
-000030a0: 3133 2e33 3936 3435 3620 342e 3737 3933  13.396456 4.7793
-000030b0: 3331 362c 3133 2e31 3633 3830 3620 4320  316,13.163806 C 
-000030c0: 352e 3531 3537 3836 312c 3133 2e34 3438  5.5157861,13.448
-000030d0: 3438 3920 352e 3733 3632 3335 332c 3133  489 5.7362353,13
-000030e0: 2e30 3038 3333 3120 342e 3938 3830 3531  .008331 4.988051
-000030f0: 2c31 322e 3733 3931 3031 2043 2033 2e34  ,12.739101 C 3.4
-00003100: 3736 3736 3936 2c31 312e 3938 3037 3631  767696,11.980761
-00003110: 2031 2e32 3433 3138 3936 2c31 322e 3833   1.2431896,12.83
-00003120: 3936 3920 312e 3033 3531 3437 362c 3134  969 1.0351476,14
-00003130: 2e36 3335 3339 3420 4320 302e 3737 3434  .635394 C 0.7744
-00003140: 3537 3135 2c31 362e 3239 3835 3832 2031  5715,16.298582 1
-00003150: 2e39 3532 3838 3437 2c31 372e 3939 3138  .9528847,17.9918
-00003160: 3335 2033 2e35 3839 3539 3633 2c31 382e  35 3.5895963,18.
-00003170: 3335 3734 3539 2043 2035 2e34 3237 3636  357459 C 5.42766
-00003180: 3632 2c31 382e 3939 3431 3635 2037 2e36  62,18.994165 7.6
-00003190: 3636 3138 3339 2c31 372e 3936 3835 3334  661839,17.968534
-000031a0: 2038 2e32 3937 3930 3339 2c31 362e 3131   8.2979039,16.11
-000031b0: 3031 3632 2043 2038 2e38 3537 3130 3235  0162 C 8.8571025
-000031c0: 2c31 342e 3731 3635 3237 2038 2e35 3436  ,14.716527 8.546
-000031d0: 3534 3831 2c31 332e 3138 3631 3339 2038  5481,13.186139 8
-000031e0: 2e30 3238 3938 3638 2c31 312e 3833 3236  .0289868,11.8326
-000031f0: 3533 2043 2037 2e34 3730 3238 3835 2c31  53 C 7.4702885,1
-00003200: 302e 3230 3638 3834 2036 2e32 3535 3336  0.206884 6.25536
-00003210: 3633 2c38 2e38 3730 3936 3734 2035 2e39  63,8.8709674 5.9
-00003220: 3239 3930 3536 2c37 2e31 3532 3538 3338  299056,7.1525838
-00003230: 2043 2035 2e34 3931 3436 2c35 2e34 3932   C 5.49146,5.492
-00003240: 3939 3635 2035 2e38 3837 3534 3938 2c33  9965 5.8875498,3
-00003250: 2e35 3733 3536 3239 2037 2e32 3332 3936  .5735629 7.23296
-00003260: 3037 2c32 2e34 3332 3732 3133 2043 2038  07,2.4327213 C 8
-00003270: 2e37 3338 3835 3931 2c31 2e30 3133 3434  .7388591,1.01344
-00003280: 3531 2031 312e 3331 3839 3331 2c30 2e37  51 11.318931,0.7
-00003290: 3535 3730 3832 2031 322e 3931 3938 3138  557082 12.919818
-000032a0: 2c32 2e31 3632 3737 3233 2043 2031 342e  ,2.1627723 C 14.
-000032b0: 3839 3131 3734 2c33 2e36 3736 3933 3435  891174,3.6769345
-000032c0: 2031 352e 3239 3530 3635 2c36 2e35 3639   15.295065,6.569
-000032d0: 3230 3238 2031 342e 3333 3032 3337 2c38  2028 14.330237,8
-000032e0: 2e37 3637 3139 3333 2043 2031 332e 3931  .7671933 C 13.91
-000032f0: 3034 3834 2c39 2e39 3139 3336 3538 2031  0484,9.9193658 1
-00003300: 332e 3135 3433 3533 2c31 302e 3930 3236  3.154353,10.9026
-00003310: 3739 2031 322e 3631 3538 3737 2c31 312e  79 12.615877,11.
-00003320: 3939 3132 3939 2043 2031 322e 3033 3830  991299 C 12.0380
-00003330: 3435 2c31 332e 3534 3832 3620 3132 2e30  45,13.54826 12.0
-00003340: 3830 3539 392c 3135 2e33 3634 3831 3320  80599,15.364813 
-00003350: 3132 2e37 3737 3435 352c 3136 2e38 3735  12.777455,16.875
-00003360: 3136 3320 4320 3134 2e30 3736 3934 362c  163 C 14.076946,
-00003370: 3139 2e31 3130 3934 3320 3137 2e39 3033  19.110943 17.903
-00003380: 3337 362c 3138 2e39 3435 3033 3320 3139  376,18.945033 19
-00003390: 2e30 3432 3037 382c 3136 2e36 3238 3730  .042078,16.62870
-000033a0: 3320 4320 3139 2e37 3537 3234 322c 3135  3 C 19.757242,15
-000033b0: 2e32 3631 3232 3720 3139 2e33 3036 3831  .261227 19.30681
-000033c0: 392c 3133 2e32 3434 3932 3920 3137 2e37  9,13.244929 17.7
-000033d0: 3635 392c 3132 2e36 3731 3930 3220 4320  659,12.671902 C 
-000033e0: 3136 2e37 3538 3335 2c31 322e 3231 3039  16.75835,12.2109
-000033f0: 3631 2031 352e 3436 3230 3933 2c31 322e  61 15.462093,12.
-00003400: 3434 3239 3531 2031 342e 3732 3933 3636  442951 14.729366
-00003410: 2c31 332e 3239 3030 3134 2043 2031 352e  ,13.290014 C 15.
-00003420: 3637 3938 3439 2c31 332e 3237 3631 3533  679849,13.276153
-00003430: 2031 362e 3938 3032 3934 2c31 332e 3236   16.980294,13.26
-00003440: 3237 3534 2031 372e 3334 3335 3032 2c31  2754 17.343502,1
-00003450: 342e 3336 3432 3033 2043 2031 372e 3930  4.364203 C 17.90
-00003460: 3332 3633 2c31 352e 3439 3236 3739 2031  3263,15.492679 1
-00003470: 372e 3736 3936 3737 2c31 372e 3330 3539  7.769677,17.3059
-00003480: 3732 2031 362e 3431 3439 3439 2c31 372e  72 16.414949,17.
-00003490: 3738 3138 3935 2043 2031 352e 3231 3834  781895 C 15.2184
-000034a0: 3138 2c31 382e 3133 3038 3420 3134 2e31  18,18.13084 14.1
-000034b0: 3530 3330 332c 3136 2e39 3032 3934 3720  50303,16.902947 
-000034c0: 3134 2e30 3932 3138 342c 3135 2e37 3831  14.092184,15.781
-000034d0: 3636 3620 4320 3133 2e37 3832 3131 372c  666 C 13.782117,
-000034e0: 3134 2e31 3031 3430 3320 3134 2e31 3430  14.101403 14.140
-000034f0: 3334 362c 3132 2e32 3730 3331 3520 3135  346,12.270315 15
-00003500: 2e32 3735 3139 2c31 302e 3935 3830 3432  .27519,10.958042
-00003510: 2043 2031 362e 3531 3938 3933 2c39 2e34   C 16.519893,9.4
-00003520: 3934 3837 3633 2031 372e 3235 3635 3235  948763 17.256525
-00003530: 2c37 2e35 3234 3036 3539 2031 362e 3836  ,7.5240659 16.86
-00003540: 3735 3236 2c35 2e35 3939 3437 3531 2043  7526,5.5994751 C
-00003550: 2031 362e 3336 3430 392c 322e 3536 3537   16.36409,2.5657
-00003560: 3234 3920 3133 2e36 3035 3030 312c 302e  249 13.605001,0.
-00003570: 3036 3537 3630 3534 3320 3130 2e35 3037  065760543 10.507
-00003580: 3330 392c 2d30 2e30 3034 3735 3437 3236  309,-0.004754726
-00003590: 3520 4320 392e 3934 3130 3733 2c2d 302e  5 C 9.941073,-0.
-000035a0: 3031 3538 3330 3639 3220 392e 3337 3232  015830692 9.3722
-000035b0: 3539 342c 302e 3030 3933 3437 3836 3139  594,0.0093478619
-000035c0: 2038 2e38 3039 3630 3436 2c30 2e30 3735   8.8096046,0.075
-000035d0: 3636 3638 3937 207a 2720 7374 796c 653d  666897 z' style=
-000035e0: 2766 696c 6c3a 2024 706c 616e 6574 735f  'fill: $planets_
-000035f0: 636f 6c6f 725f 3130 3b27 202f 3e0d 0a20  color_10;' />.. 
-00003600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003610: 2020 203c 2f67 3e0d 0a20 2020 2020 2020     </g>..       
-00003620: 2020 2020 2020 2020 203c 2f73 796d 626f           </symbo
-00003630: 6c3e 0d0a 2020 2020 2020 2020 2020 2020  l>..            
-00003640: 2020 2020 3c73 796d 626f 6c20 6964 3d27      <symbol id='
-00003650: 5472 7565 5f4e 6f64 6527 3e3c 2f73 796d  True_Node'></sym
-00003660: 626f 6c3e 0d0a 2020 2020 2020 2020 2020  bol>..          
-00003670: 2020 2020 2020 3c73 796d 626f 6c20 6964        <symbol id
-00003680: 3d27 3127 3e0d 0a20 2020 2020 2020 2020  ='1'>..         
-00003690: 2020 2020 2020 2020 2020 203c 7465 7874             <text
-000036a0: 2079 3d27 3230 2720 7374 796c 653d 2766   y='20' style='f
-000036b0: 6f6e 742d 7369 7a65 3a32 3270 783b 2066  ont-size:22px; f
-000036c0: 696c 6c3a 2024 706c 616e 6574 735f 636f  ill: $planets_co
-000036d0: 6c6f 725f 3132 3b27 3e41 733c 2f74 6578  lor_12;'>As</tex
-000036e0: 743e 0d0a 2020 2020 2020 2020 2020 2020  t>..            
-000036f0: 2020 2020 3c2f 7379 6d62 6f6c 3e0d 0a20      </symbol>.. 
-00003700: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00003710: 7379 6d62 6f6c 2069 643d 2731 3027 3e0d  symbol id='10'>.
-00003720: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003730: 2020 2020 203c 7465 7874 2079 3d27 3230       <text y='20
-00003740: 2720 7374 796c 653d 2766 6f6e 742d 7369  ' style='font-si
-00003750: 7a65 3a32 3070 783b 2066 696c 6c3a 2024  ze:20px; fill: $
-00003760: 706c 616e 6574 735f 636f 6c6f 725f 3133  planets_color_13
-00003770: 3b27 3e4d 633c 2f74 6578 743e 0d0a 2020  ;'>Mc</text>..  
-00003780: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-00003790: 7379 6d62 6f6c 3e0d 0a20 2020 2020 2020  symbol>..       
-000037a0: 2020 2020 2020 2020 203c 7379 6d62 6f6c           <symbol
-000037b0: 2069 643d 2737 273e 0d0a 2020 2020 2020   id='7'>..      
-000037c0: 2020 2020 2020 2020 2020 2020 2020 3c74                <t
-000037d0: 6578 7420 793d 2732 3027 2073 7479 6c65  ext y='20' style
-000037e0: 3d27 666f 6e74 2d73 697a 653a 3232 7078  ='font-size:22px
-000037f0: 3b20 6669 6c6c 3a20 2470 6c61 6e65 7473  ; fill: $planets
-00003800: 5f63 6f6c 6f72 5f31 343b 273e 4473 3c2f  _color_14;'>Ds</
-00003810: 7465 7874 3e0d 0a20 2020 2020 2020 2020  text>..         
-00003820: 2020 2020 2020 203c 2f73 796d 626f 6c3e         </symbol>
-00003830: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00003840: 2020 3c73 796d 626f 6c20 6964 3d27 3427    <symbol id='4'
-00003850: 3e0d 0a20 2020 2020 2020 2020 2020 2020  >..             
-00003860: 2020 2020 2020 203c 7465 7874 2079 3d27         <text y='
-00003870: 3230 2720 7374 796c 653d 2766 6f6e 742d  20' style='font-
-00003880: 7369 7a65 3a32 3270 783b 2066 696c 6c3a  size:22px; fill:
-00003890: 2024 706c 616e 6574 735f 636f 6c6f 725f   $planets_color_
-000038a0: 3135 3b27 3e49 633c 2f74 6578 743e 0d0a  15;'>Ic</text>..
-000038b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000038c0: 3c2f 7379 6d62 6f6c 3e20 2020 2020 2020  </symbol>       
-000038d0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-000038e0: 2020 2020 2020 2020 2020 203c 212d 2d20             <!-- 
-000038f0: 5a6f 6469 6163 202d 2d3e 0d0a 2020 2020  Zodiac -->..    
-00003900: 2020 2020 2020 2020 2020 2020 3c73 796d              <sym
-00003910: 626f 6c20 6964 3d27 6172 6965 7327 3e0d  bol id='aries'>.
-00003920: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003930: 2020 2020 203c 7061 7468 2074 7261 6e73       <path trans
-00003940: 666f 726d 3d22 7363 616c 6528 302e 3829  form="scale(0.8)
-00003950: 2220 643d 274d 2031 342e 3833 3335 3336  " d='M 14.833536
-00003960: 2c33 3120 4320 3134 2e38 3332 3138 362c  ,31 C 14.832186,
-00003970: 3239 2e37 3238 3235 2031 342e 3834 3539  29.72825 14.8459
-00003980: 3336 2c32 382e 3435 3538 3420 3134 2e37  36,28.45584 14.7
-00003990: 3830 3334 362c 3237 2e31 3835 3233 2043  80346,27.18523 C
-000039a0: 2031 342e 3634 3039 3236 2c32 342e 3233   14.640926,24.23
-000039b0: 3034 3620 3134 2e32 3731 3932 372c 3231  046 14.271927,21
-000039c0: 2e32 3839 3739 2031 332e 3736 3136 3537  .28979 13.761657
-000039d0: 2c31 382e 3337 3736 2043 2031 332e 3332  ,18.3776 C 13.32
-000039e0: 3139 3837 2c31 352e 3931 3931 3120 3132  1987,15.91911 12
-000039f0: 2e37 3837 3738 372c 3133 2e34 3639 3833  .787787,13.46983
-00003a00: 2031 312e 3939 3035 3137 2c31 312e 3130   11.990517,11.10
-00003a10: 3037 3520 4320 3131 2e35 3330 3236 372c  075 C 11.530267,
-00003a20: 392e 3736 3234 3320 3130 2e39 3932 3838  9.76243 10.99288
-00003a30: 372c 382e 3434 3931 3220 3130 2e33 3537  7,8.44912 10.357
-00003a40: 3038 372c 372e 3138 3439 2043 2039 2e37  087,7.1849 C 9.7
-00003a50: 3736 3430 3635 2c36 2e30 3534 2039 2e31  764065,6.054 9.1
-00003a60: 3134 3334 3635 2c34 2e39 3432 3936 2038  143465,4.94296 8
-00003a70: 2e32 3136 3030 3635 2c34 2e30 3334 3934  .2160065,4.03494
-00003a80: 2043 2037 2e36 3238 3234 3635 2c33 2e34   C 7.6282465,3.4
-00003a90: 3436 3520 362e 3930 3037 3236 352c 322e  465 6.9007265,2.
-00003aa0: 3934 3533 3520 362e 3036 3439 3736 352c  94535 6.0649765,
-00003ab0: 322e 3831 3632 3420 4320 352e 3332 3337  2.81624 C 5.3237
-00003ac0: 3236 362c 322e 3730 3134 3220 342e 3533  266,2.70142 4.53
-00003ad0: 3034 3636 362c 322e 3837 3537 3120 332e  04666,2.87571 3.
-00003ae0: 3933 3536 3936 362c 332e 3334 3338 3420  9356966,3.34384 
-00003af0: 4320 332e 3231 3336 3536 352c 332e 3930  C 3.2136565,3.90
-00003b00: 3531 3920 322e 3736 3534 3336 352c 342e  519 2.7654365,4.
-00003b10: 3735 3632 3520 322e 3534 3338 3336 352c  75625 2.5438365,
-00003b20: 352e 3633 3238 3920 4320 322e 3330 3533  5.63289 C 2.3053
-00003b30: 3736 352c 362e 3539 3939 3520 322e 3239  765,6.59995 2.29
-00003b40: 3539 3736 352c 372e 3631 3335 3820 322e  59765,7.61358 2.
-00003b50: 3432 3932 3136 352c 382e 3539 3733 2043  4292165,8.5973 C
-00003b60: 2032 2e36 3436 3434 3635 2c31 302e 3135   2.6464465,10.15
-00003b70: 3538 3720 332e 3236 3839 3636 352c 3131  587 3.2689665,11
-00003b80: 2e36 3332 3538 2034 2e30 3831 3534 3636  .63258 4.0815466
-00003b90: 2c31 322e 3936 3930 3820 4320 332e 3239  ,12.96908 C 3.29
-00003ba0: 3234 3436 352c 3132 2e39 3639 3038 2032  24465,12.96908 2
-00003bb0: 2e35 3033 3334 3635 2c31 322e 3936 3930  .5033465,12.9690
-00003bc0: 3820 312e 3731 3432 3436 352c 3132 2e39  8 1.7142465,12.9
-00003bd0: 3639 3038 2043 2030 2e38 3937 3234 3635  6908 C 0.8972465
-00003be0: 312c 3131 2e34 3834 3831 2030 2e32 3537  1,11.48481 0.257
-00003bf0: 3939 3635 312c 392e 3837 3239 3920 302e  99651,9.87299 0.
-00003c00: 3036 3032 3536 3531 342c 382e 3137 3839  060256514,8.1789
-00003c10: 3920 4320 2d30 2e30 3731 3230 3334 3836  9 C -0.071203486
-00003c20: 2c37 2e30 3036 3935 2030 2e30 3033 3731  ,7.00695 0.00371
-00003c30: 3635 3133 382c 352e 3739 3930 3320 302e  65138,5.79903 0.
-00003c40: 3337 3134 3936 3531 2c34 2e36 3734 3231  37149651,4.67421
-00003c50: 2043 2030 2e37 3634 3432 3635 312c 332e   C 0.76442651,3.
-00003c60: 3437 3439 3920 312e 3531 3935 3836 352c  47499 1.5195865,
-00003c70: 322e 3339 3332 2032 2e35 3233 3235 3635  2.3932 2.5232565
-00003c80: 2c31 2e36 3330 3420 4320 332e 3238 3039  ,1.6304 C 3.2809
-00003c90: 3636 352c 312e 3035 3437 3820 342e 3230  665,1.05478 4.20
-00003ca0: 3539 3336 362c 302e 3731 3236 3820 352e  59366,0.71268 5.
-00003cb0: 3135 3139 3436 362c 302e 3633 3738 3120  1519466,0.63781 
-00003cc0: 4320 362e 3139 3338 3236 352c 302e 3534  C 6.1938265,0.54
-00003cd0: 3439 3620 372e 3236 3130 3436 352c 302e  496 7.2610465,0.
-00003ce0: 3734 3631 3920 382e 3139 3039 3236 352c  74619 8.1909265,
-00003cf0: 312e 3232 3937 3620 4320 392e 3339 3938  1.22976 C 9.3998
-00003d00: 3636 352c 312e 3835 3032 3120 3130 2e33  665,1.85021 10.3
-00003d10: 3633 3637 372c 322e 3835 3934 3420 3131  63677,2.85944 11
-00003d20: 2e31 3435 3237 372c 332e 3935 3736 3620  .145277,3.95766 
-00003d30: 4320 3132 2e31 3930 3334 372c 352e 3434  C 12.190347,5.44
-00003d40: 3134 3720 3132 2e39 3635 3036 372c 372e  147 12.965067,7.
-00003d50: 3130 3130 3120 3133 2e35 3834 3238 372c  10101 13.584287,
-00003d60: 382e 3830 3338 3220 4320 3134 2e36 3330  8.80382 C 14.630
-00003d70: 3736 362c 3131 2e37 3137 3620 3135 2e32  766,11.7176 15.2
-00003d80: 3132 3632 362c 3134 2e37 3738 3631 2031  12626,14.77861 1
-00003d90: 352e 3537 3531 3436 2c31 372e 3834 3739  5.575146,17.8479
-00003da0: 3520 4320 3135 2e36 3634 3833 362c 3138  5 C 15.664836,18
-00003db0: 2e36 3136 3438 2031 352e 3733 3935 3536  .61648 15.739556
-00003dc0: 2c31 392e 3338 3637 3520 3135 2e38 3031  ,19.38675 15.801
-00003dd0: 3434 362c 3230 2e31 3538 3033 2043 2031  446,20.15803 C 1
-00003de0: 352e 3933 3336 3036 2c32 302e 3135 3830  5.933606,20.1580
-00003df0: 3320 3136 2e30 3635 3737 362c 3230 2e31  3 16.065776,20.1
-00003e00: 3538 3033 2031 362e 3139 3739 3336 2c32  5803 16.197936,2
-00003e10: 302e 3135 3830 3320 4320 3136 2e34 3331  0.15803 C 16.431
-00003e20: 3531 362c 3136 2e37 3833 3332 2031 362e  516,16.78332 16.
-00003e30: 3931 3930 3636 2c31 332e 3430 3736 3120  919066,13.40761 
-00003e40: 3137 2e39 3230 3233 362c 3130 2e31 3730  17.920236,10.170
-00003e50: 3239 2043 2031 382e 3533 3637 3436 2c38  29 C 18.536746,8
-00003e60: 2e31 3938 3836 2031 392e 3334 3332 3136  .19886 19.343216
-00003e70: 2c36 2e32 3733 3320 3230 2e34 3630 3130  ,6.2733 20.46010
-00003e80: 362c 342e 3533 3230 3920 4320 3231 2e32  6,4.53209 C 21.2
-00003e90: 3332 3936 362c 332e 3334 3234 3620 3232  32966,3.34246 22
-00003ea0: 2e31 3738 3339 362c 322e 3232 3639 3120  .178396,2.22691 
-00003eb0: 3233 2e33 3933 3233 362c 312e 3437 3437  23.393236,1.4747
-00003ec0: 3320 4320 3234 2e33 3033 3934 362c 302e  3 C 24.303946,0.
-00003ed0: 3930 3620 3235 2e33 3735 3430 362c 302e  906 25.375406,0.
-00003ee0: 3539 3331 3520 3236 2e34 3439 3833 362c  59315 26.449836,
-00003ef0: 302e 3631 3734 3420 4320 3237 2e34 3036  0.61744 C 27.406
-00003f00: 3037 362c 302e 3632 3635 2032 382e 3336  076,0.6265 28.36
-00003f10: 3633 3336 2c30 2e38 3834 3134 2032 392e  6336,0.88414 29.
-00003f20: 3137 3333 3836 2c31 2e34 3035 3731 2043  173386,1.40571 C
-00003f30: 2032 392e 3931 3832 3736 2c31 2e38 3834   29.918276,1.884
-00003f40: 3137 2033 302e 3533 3637 3236 2c32 2e35  17 30.536726,2.5
-00003f50: 3438 3235 2033 312e 3030 3733 3036 2c33  4825 31.007306,3
-00003f60: 2e32 3936 3838 2043 2033 312e 3634 3033  .29688 C 31.6403
-00003f70: 3736 2c34 2e33 3039 3831 2033 312e 3934  76,4.30981 31.94
-00003f80: 3237 3836 2c35 2e35 3033 3620 3331 2e39  2786,5.5036 31.9
-00003f90: 3930 3532 362c 362e 3639 3134 3920 4320  90526,6.69149 C 
-00003fa0: 3332 2e30 3634 3336 362c 382e 3234 3839  32.064366,8.2489
-00003fb0: 3820 3331 2e37 3030 3330 362c 392e 3739  8 31.700306,9.79
-00003fc0: 3834 3120 3331 2e31 3138 3133 362c 3131  841 31.118136,11
-00003fd0: 2e32 3334 3039 2043 2033 302e 3837 3830  .23409 C 30.8780
-00003fe0: 3536 2c31 312e 3832 3737 3420 3330 2e36  56,11.82774 30.6
-00003ff0: 3030 3734 362c 3132 2e34 3035 3834 2033  00746,12.40584 3
-00004000: 302e 3239 3637 3936 2c31 322e 3936 3930  0.296796,12.9690
-00004010: 3820 4320 3239 2e35 3033 3830 362c 3132  8 C 29.503806,12
-00004020: 2e39 3639 3038 2032 382e 3731 3038 3236  .96908 28.710826
-00004030: 2c31 322e 3936 3930 3820 3237 2e39 3137  ,12.96908 27.917
-00004040: 3833 362c 3132 2e39 3639 3038 2043 2032  836,12.96908 C 2
-00004050: 382e 3639 3536 3436 2c31 312e 3536 3832  8.695646,11.5682
-00004060: 3520 3239 2e33 3330 3930 362c 3130 2e30  5 29.330906,10.0
-00004070: 3630 3434 2032 392e 3536 3537 3536 2c38  6044 29.565756,8
-00004080: 2e34 3634 3835 2043 2032 392e 3730 3534  .46485 C 29.7054
-00004090: 3336 2c37 2e34 3930 3533 2032 392e 3638  36,7.49053 29.68
-000040a0: 3939 3736 2c36 2e34 3837 3339 2032 392e  9976,6.48739 29.
-000040b0: 3436 3937 3336 2c35 2e35 3236 3136 2043  469736,5.52616 C
-000040c0: 2032 392e 3236 3635 3836 2c34 2e36 3732   29.266586,4.672
-000040d0: 3936 2032 382e 3837 3039 3536 2c33 2e38  96 28.870956,3.8
-000040e0: 3333 3534 2032 382e 3230 3132 3736 2c33  3354 28.201276,3
-000040f0: 2e32 3530 3739 2043 2032 372e 3731 3833  .25079 C 27.7183
-00004100: 3836 2c32 2e38 3232 3633 2032 372e 3037  86,2.82263 27.07
-00004110: 3834 3636 2c32 2e35 3930 3231 2032 362e  8466,2.59021 26.
-00004120: 3433 3632 3136 2c32 2e35 3834 3436 2043  436216,2.58446 C
-00004130: 2032 352e 3638 3033 3036 2c32 2e35 3630   25.680306,2.560
-00004140: 3539 2032 342e 3935 3030 3836 2c32 2e38  59 24.950086,2.8
-00004150: 3733 3033 2032 342e 3335 3833 3336 2c33  7303 24.358336,3
-00004160: 2e33 3238 3739 2043 2032 332e 3439 3435  .32879 C 23.4945
-00004170: 3536 2c33 2e39 3933 3037 2032 322e 3834  56,3.99307 22.84
-00004180: 3439 3836 2c34 2e38 3931 3938 2032 322e  4986,4.89198 22.
-00004190: 3238 3239 3536 2c35 2e38 3136 3739 2043  282956,5.81679 C
-000041a0: 2032 312e 3435 3137 3536 2c37 2e32 3130   21.451756,7.210
-000041b0: 3732 2032 302e 3831 3134 3336 2c38 2e37  72 20.811436,8.7
-000041c0: 3130 3138 2032 302e 3235 3033 3936 2c31  1018 20.250396,1
-000041d0: 302e 3233 3132 3420 4320 3139 2e34 3337  0.23124 C 19.437
-000041e0: 3538 362c 3132 2e34 3938 3032 2031 382e  586,12.49802 18.
-000041f0: 3839 3333 3236 2c31 342e 3835 3136 3620  893326,14.85166 
-00004200: 3138 2e34 3430 3238 362c 3137 2e32 3134  18.440286,17.214
-00004210: 3332 2043 2031 372e 3833 3930 3136 2c32  32 C 17.839016,2
-00004220: 302e 3430 3332 3520 3137 2e34 3133 3231  0.40325 17.41321
-00004230: 362c 3233 2e36 3239 3120 3137 2e32 3436  6,23.6291 17.246
-00004240: 3133 362c 3236 2e38 3731 3520 4320 3137  136,26.8715 C 17
-00004250: 2e31 3833 3739 362c 3238 2e30 3138 3537  .183796,28.01857
-00004260: 2031 372e 3137 3339 3636 2c32 392e 3136   17.173966,29.16
-00004270: 3734 3520 3137 2e31 3737 3531 362c 3330  745 17.177516,30
-00004280: 2e33 3135 3935 2043 2031 372e 3137 3735  .31595 C 17.1775
-00004290: 3136 2c33 302e 3534 3339 3720 3137 2e31  16,30.54397 17.1
-000042a0: 3737 3531 362c 3330 2e37 3731 3938 2031  77516,30.77198 1
-000042b0: 372e 3137 3735 3136 2c33 3120 4320 3136  7.177516,31 C 16
-000042c0: 2e33 3936 3138 362c 3331 2031 352e 3631  .396186,31 15.61
-000042d0: 3438 3536 2c33 3120 3134 2e38 3333 3533  4856,31 14.83353
-000042e0: 362c 3331 207a 2720 7374 796c 653d 2766  6,31 z' style='f
-000042f0: 696c 6c3a 2024 7a6f 6469 6163 5f63 6f6c  ill: $zodiac_col
-00004300: 6f72 5f30 3b27 202f 3e0d 0a20 2020 2020  or_0;' />..     
-00004310: 2020 2020 2020 2020 2020 203c 2f73 796d             </sym
-00004320: 626f 6c3e 0d0a 2020 2020 2020 2020 2020  bol>..          
-00004330: 2020 2020 2020 3c73 796d 626f 6c20 6964        <symbol id
-00004340: 3d27 7461 7572 7573 273e 0d0a 2020 2020  ='taurus'>..    
-00004350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004360: 3c70 6174 6820 7472 616e 7366 6f72 6d3d  <path transform=
-00004370: 2273 6361 6c65 2830 2e38 2922 2064 3d27  "scale(0.8)" d='
-00004380: 4d20 3131 2e32 3131 3132 352c 3131 2e39  M 11.211125,11.9
-00004390: 3630 3034 3320 4320 392e 3938 3536 3139  60043 C 9.985619
-000043a0: 372c 3131 2e34 3832 3038 3520 382e 3832  7,11.482085 8.82
-000043b0: 3733 3530 372c 3130 2e37 3537 3236 3320  73507,10.757263 
-000043c0: 372e 3939 3934 3136 342c 392e 3732 3236  7.9994164,9.7226
-000043d0: 3620 4320 362e 3935 3430 3538 342c 382e  6 C 6.9540584,8.
-000043e0: 3434 3839 3530 3820 362e 3231 3139 3532  4489508 6.211952
-000043f0: 342c 362e 3936 3936 3039 3720 352e 3430  4,6.9696097 5.40
-00004400: 3638 3139 392c 352e 3534 3232 3531 3520  68199,5.5422515 
-00004410: 4320 342e 3931 3533 3333 362c 342e 3634  C 4.9153336,4.64
-00004420: 3335 3933 3120 342e 3335 3838 3435 322c  35931 4.3588452,
-00004430: 332e 3736 3034 3132 3820 332e 3630 3032  3.7604128 3.6002
-00004440: 3638 362c 332e 3036 3031 3033 3620 4320  686,3.0601036 C 
-00004450: 332e 3038 3737 3337 312c 322e 3538 3330  3.0877371,2.5830
-00004460: 3339 3920 322e 3436 3939 3433 332c 322e  399 2.4699433,2.
-00004470: 3139 3737 3132 3920 312e 3737 3931 3332  1977129 1.779132
-00004480: 312c 322e 3034 3632 3137 3820 4320 312e  1,2.0462178 C 1.
-00004490: 3435 3134 3836 372c 312e 3936 3633 3435  4514867,1.966345
-000044a0: 3120 312e 3131 3237 3639 382c 312e 3936  1 1.1127698,1.96
-000044b0: 3334 3036 3520 302e 3737 3735 3636 3438  34065 0.77756648
-000044c0: 2c31 2e39 3639 3332 3033 2043 2030 2e36  ,1.9693203 C 0.6
-000044d0: 3737 3530 3133 382c 312e 3938 3234 3830  7750138,1.982480
-000044e0: 3320 302e 3539 3833 3335 3038 2c31 2e39  3 0.59833508,1.9
-000044f0: 3734 3735 3935 2030 2e36 3333 3639 3038  747595 0.6336908
-00004500: 382c 312e 3835 3238 3333 3320 4320 302e  8,1.8528333 C 0.
-00004510: 3633 3336 3930 3838 2c31 2e32 3730 3336  63369088,1.27036
-00004520: 3138 2030 2e36 3333 3639 3038 382c 302e  18 0.63369088,0.
-00004530: 3638 3738 3930 3233 2030 2e36 3333 3639  68789023 0.63369
-00004540: 3038 382c 302e 3130 3534 3030 3434 2043  088,0.10540044 C
-00004550: 2031 2e31 3736 3933 2c30 2e31 3131 3738   1.17693,0.11178
-00004560: 3838 3420 312e 3732 3130 3239 322c 302e  884 1.7210292,0.
-00004570: 3039 3031 3539 3634 3120 322e 3236 3336  090159641 2.2636
-00004580: 3039 352c 302e 3132 3136 3939 3834 2043  095,0.12169984 C
-00004590: 2033 2e33 3439 3337 3339 2c30 2e32 3132   3.3493739,0.212
-000045a0: 3038 3539 3420 342e 3336 3635 3132 392c  08594 4.3665129,
-000045b0: 302e 3731 3538 3731 3231 2035 2e31 3931  0.71587121 5.191
-000045c0: 3739 3335 2c31 2e34 3039 3735 3535 2043  7935,1.4097555 C
-000045d0: 2036 2e32 3634 3738 3434 2c32 2e33 3031   6.2647844,2.301
-000045e0: 3333 3220 372e 3038 3838 3735 342c 332e  332 7.0888754,3.
-000045f0: 3434 3934 3832 3720 372e 3739 3131 3631  4494827 7.791161
-00004600: 342c 342e 3634 3336 3437 3920 4320 382e  4,4.6436479 C 8.
-00004610: 3239 3133 3033 342c 352e 3530 3436 3838  2913034,5.504688
-00004620: 2038 2e37 3732 3137 3537 2c36 2e33 3736   8.7721757,6.376
-00004630: 3735 3235 2039 2e32 3734 3331 3237 2c37  7525 9.2743127,7
-00004640: 2e32 3336 3630 3632 2043 2039 2e37 3538  .2366062 C 9.758
-00004650: 3830 3837 2c38 2e30 3436 3335 3639 2031  8087,8.0463569 1
-00004660: 302e 3330 3736 3438 2c38 2e38 3234 3738  0.307648,8.82478
-00004670: 3635 2031 302e 3937 3135 3339 2c39 2e34  65 10.971539,9.4
-00004680: 3938 3939 3438 2043 2031 312e 3535 3837  989948 C 11.5587
-00004690: 3137 2c31 302e 3039 3436 3939 2031 322e  17,10.094699 12.
-000046a0: 3236 3135 372c 3130 2e35 3836 3936 3720  26157,10.586967 
-000046b0: 3133 2e30 3532 3934 2c31 302e 3837 3131  13.05294,10.8711
-000046c0: 3339 2043 2031 342e 3135 3039 3636 2c31  39 C 14.150966,1
-000046d0: 312e 3237 3633 3632 2031 352e 3333 3930  1.276362 15.3390
-000046e0: 3436 2c31 312e 3335 3935 3536 2031 362e  46,11.359556 16.
-000046f0: 3530 3032 3434 2c31 312e 3331 3436 3337  500244,11.314637
-00004700: 2043 2031 372e 3534 3332 3034 2c31 312e   C 17.543204,11.
-00004710: 3236 3236 3732 2031 382e 3630 3230 3638  262672 18.602068
-00004720: 2c31 312e 3036 3936 3136 2031 392e 3532  ,11.069616 19.52
-00004730: 3937 3932 2c31 302e 3537 3137 3435 2043  9792,10.571745 C
-00004740: 2032 302e 3430 3133 3335 2c31 302e 3131   20.401335,10.11
-00004750: 3436 3637 2032 312e 3130 3338 3034 2c39  4667 21.103804,9
-00004760: 2e33 3937 3039 3134 2032 312e 3730 3030  .3970914 21.7000
-00004770: 342c 382e 3632 3637 3635 3920 4320 3232  4,8.6267659 C 22
-00004780: 2e33 3835 3038 372c 372e 3734 3131 3934  .385087,7.741194
-00004790: 3620 3232 2e39 3036 3937 2c36 2e37 3437  6 22.90697,6.747
-000047a0: 3733 3331 2032 332e 3437 3237 2c35 2e37  7331 23.4727,5.7
-000047b0: 3835 3930 3331 2043 2032 332e 3937 3332  859031 C 23.9732
-000047c0: 3939 2c34 2e39 3332 3134 3538 2032 342e  99,4.9321458 24.
-000047d0: 3434 3535 3136 2c34 2e30 3538 3630 3238  445516,4.0586028
-000047e0: 2032 352e 3033 3232 3931 2c33 2e32 3538   25.032291,3.258
-000047f0: 3930 3931 2043 2032 352e 3731 3138 3636  9091 C 25.711866
-00004800: 2c32 2e33 3234 3738 3633 2032 362e 3531  ,2.3247863 26.51
-00004810: 3636 3332 2c31 2e34 3535 3832 3437 2032  6632,1.4558247 2
-00004820: 372e 3530 3737 3636 2c30 2e38 3435 3939  7.507766,0.84599
-00004830: 3237 3720 4320 3238 2e32 3636 3437 312c  277 C 28.266471,
-00004840: 302e 3338 3332 3338 3934 2032 392e 3134  0.38323894 29.14
-00004850: 3633 3737 2c30 2e30 3936 3534 3830 3431  6377,0.096548041
-00004860: 2033 302e 3034 3038 3332 2c30 2e31 3036   30.040832,0.106
-00004870: 3635 3938 3420 4320 3330 2e34 3530 3432  65984 C 30.45042
-00004880: 362c 302e 3130 3230 3630 3234 2033 302e  6,0.10206024 30.
-00004890: 3836 3030 3734 2c30 2e31 3037 3933 3735  860074,0.1079375
-000048a0: 3420 3331 2e32 3639 3636 372c 302e 3130  4 31.269667,0.10
-000048b0: 3534 3030 3434 2043 2033 312e 3236 3936  540044 C 31.2696
-000048c0: 3637 2c30 2e37 3236 3731 3331 3520 3331  67,0.72671315 31
-000048d0: 2e32 3639 3636 372c 312e 3334 3830 3235  .269667,1.348025
-000048e0: 3820 3331 2e32 3639 3636 372c 312e 3936  8 31.269667,1.96
-000048f0: 3933 3230 3320 4320 3330 2e38 3336 3534  93203 C 30.83654
-00004900: 2c31 2e39 3636 3130 3738 2033 302e 3339  ,1.9661078 30.39
-00004910: 3533 3631 2c31 2e39 3538 3336 3838 2032  5361,1.9583688 2
-00004920: 392e 3937 3630 3638 2c32 2e30 3834 3035  9.976068,2.08405
-00004930: 3520 4320 3239 2e31 3139 3933 342c 322e  5 C 29.119934,2.
-00004940: 3331 3836 3731 3820 3238 2e34 3030 3438  3186718 28.40048
-00004950: 332c 322e 3839 3235 3634 3620 3237 2e38  3,2.8925646 27.8
-00004960: 3236 3933 392c 332e 3535 3137 3639 3320  26939,3.5517693 
-00004970: 4320 3237 2e32 3336 3032 382c 342e 3232  C 27.236028,4.22
-00004980: 3335 3836 3520 3236 2e37 3838 3236 312c  35865 26.788261,
-00004990: 352e 3030 3238 3337 3420 3236 2e33 3631  5.0028374 26.361
-000049a0: 3636 362c 352e 3738 3433 3639 3920 4320  666,5.7843699 C 
-000049b0: 3235 2e36 3233 3131 2c37 2e31 3031 3038  25.62311,7.10108
-000049c0: 3139 2032 342e 3932 3631 3638 2c38 2e34  19 24.926168,8.4
-000049d0: 3534 3339 2032 332e 3937 3439 3436 2c39  5439 23.974946,9
-000049e0: 2e36 3335 3732 3337 2043 2032 332e 3539  .6357237 C 23.59
-000049f0: 3335 3534 2c31 302e 3131 3532 3838 2032  3554,10.115288 2
-00004a00: 332e 3135 3231 3138 2c31 302e 3534 3738  3.152118,10.5478
-00004a10: 3136 2032 322e 3635 3235 3036 2c31 302e  16 22.652506,10.
-00004a20: 3930 3433 3431 2043 2032 322e 3034 3938  904341 C 22.0498
-00004a30: 312c 3131 2e33 3431 3236 3720 3231 2e33  1,11.341267 21.3
-00004a40: 3833 3337 352c 3131 2e36 3835 3332 3620  83375,11.685326 
-00004a50: 3230 2e36 3932 3231 362c 3131 2e39 3630  20.692216,11.960
-00004a60: 3034 3320 4320 3232 2e33 3438 3938 312c  043 C 22.348981,
-00004a70: 3132 2e38 3635 3235 3420 3233 2e38 3238  12.865254 23.828
-00004a80: 3330 382c 3134 2e31 3232 3634 3620 3234  308,14.122646 24
-00004a90: 2e38 3936 3333 392c 3135 2e36 3834 3033  .896339,15.68403
-00004aa0: 3120 4320 3235 2e37 3936 3530 342c 3136  1 C 25.796504,16
-00004ab0: 2e39 3836 3038 3720 3236 2e33 3934 3331  .986087 26.39431
-00004ac0: 342c 3138 2e34 3939 3135 3820 3236 2e35  4,18.499158 26.5
-00004ad0: 3932 3934 332c 3230 2e30 3730 3039 2043  92943,20.07009 C
-00004ae0: 2032 362e 3738 3636 3332 2c32 312e 3535   26.786632,21.55
-00004af0: 3231 3531 2032 362e 3637 3934 3438 2c32  2151 26.679448,2
-00004b00: 332e 3037 3737 3820 3236 2e32 3436 3339  3.07778 26.24639
-00004b10: 342c 3234 2e35 3130 3139 3420 4320 3235  4,24.510194 C 25
-00004b20: 2e37 3934 3132 352c 3235 2e39 3931 3033  .794125,25.99103
-00004b30: 3220 3234 2e39 3736 3338 342c 3237 2e33  2 24.976384,27.3
-00004b40: 3439 3530 3520 3233 2e39 3235 3937 352c  49505 23.925975,
-00004b50: 3238 2e34 3835 3030 3720 4320 3232 2e36  28.485007 C 22.6
-00004b60: 3635 3634 362c 3239 2e38 3636 3135 2032  65646,29.86615 2
-00004b70: 312e 3038 3539 3938 2c33 302e 3938 3437  1.085998,30.9847
-00004b80: 3332 2031 392e 3330 3132 3432 2c33 312e  32 19.301242,31.
-00004b90: 3537 3639 3332 2043 2031 372e 3535 3232  576932 C 17.5522
-00004ba0: 3038 2c33 322e 3135 3734 3134 2031 352e  08,32.157414 15.
-00004bb0: 3635 3238 3032 2c33 322e 3234 3636 3134  652802,32.246614
-00004bc0: 2031 332e 3834 3630 3836 2c33 312e 3930   13.846086,31.90
-00004bd0: 3237 3536 2043 2031 322e 3232 3031 3933  2756 C 12.220193
-00004be0: 2c33 312e 3538 3434 3839 2031 302e 3638  ,31.584489 10.68
-00004bf0: 3537 3635 2c33 302e 3834 3538 3520 392e  5765,30.84585 9.
-00004c00: 3430 3038 3736 372c 3239 2e38 3035 3632  4008767,29.80562
-00004c10: 3520 4320 382e 3330 3031 3432 342c 3238  5 C 8.3001424,28
-00004c20: 2e39 3233 3330 3320 372e 3333 3534 3639  .923303 7.335469
-00004c30: 342c 3237 2e38 3631 3831 3520 362e 3630  4,27.861815 6.60
-00004c40: 3637 3737 342c 3236 2e36 3532 3935 3620  67774,26.652956 
-00004c50: 4320 352e 3834 3135 3032 372c 3235 2e33  C 5.8415027,25.3
-00004c60: 3735 3233 3120 352e 3337 3036 3538 392c  75231 5.3706589,
-00004c70: 3233 2e39 3233 3431 3520 352e 3234 3738  23.923415 5.2478
-00004c80: 3436 382c 3232 2e34 3339 3731 3220 4320  468,22.439712 C 
-00004c90: 352e 3038 3233 3538 382c 3230 2e35 3936  5.0823588,20.596
-00004ca0: 3620 352e 3339 3339 3931 352c 3138 2e37  6 5.3939915,18.7
-00004cb0: 3031 3435 2036 2e32 3136 3237 3034 2c31  0145 6.2162704,1
-00004cc0: 372e 3033 3732 3132 2043 2037 2e31 3136  7.037212 C 7.116
-00004cd0: 3633 3634 2c31 352e 3139 3133 3632 2038  6364,15.191362 8
-00004ce0: 2e35 3634 3332 3234 2c31 332e 3633 3439  .5643224,13.6349
-00004cf0: 3935 2031 302e 3238 3335 3436 2c31 322e  95 10.283546,12.
-00004d00: 3531 3735 3633 2043 2031 302e 3538 3532  517563 C 10.5852
-00004d10: 3937 2c31 322e 3331 3937 3434 2031 302e  97,12.319744 10.
-00004d20: 3839 3530 3038 2c31 322e 3133 3430 3632  895008,12.134062
-00004d30: 2031 312e 3231 3131 3235 2c31 312e 3936   11.211125,11.96
-00004d40: 3030 3433 207a 204d 2031 352e 3935 3739  0043 z M 15.9579
-00004d50: 322c 3239 2e36 3035 3330 3520 4320 3137  2,29.605305 C 17
-00004d60: 2e34 3639 3637 342c 3239 2e36 3133 3933  .469674,29.61393
-00004d70: 3820 3138 2e39 3935 3730 332c 3239 2e32  8 18.995703,29.2
-00004d80: 3238 3036 3420 3230 2e32 3737 3937 342c  28064 20.277974,
-00004d90: 3238 2e34 3138 3133 2043 2032 312e 3238  28.41813 C 21.28
-00004da0: 3234 3331 2c32 372e 3738 3934 3632 2032  2431,27.789462 2
-00004db0: 322e 3135 3336 3237 2c32 362e 3935 3235  2.153627,26.9525
-00004dc0: 3333 2032 322e 3833 3739 3432 2c32 352e  33 22.837942,25.
-00004dd0: 3938 3737 3635 2043 2032 332e 3539 3634  987765 C 23.5964
-00004de0: 3038 2c32 342e 3930 3135 3236 2032 342e  08,24.901526 24.
-00004df0: 3035 3635 3833 2c32 332e 3631 3237 3935  056583,23.612795
-00004e00: 2032 342e 3136 3031 3434 2c32 322e 3239   24.160144,22.29
-00004e10: 3332 3138 2043 2032 342e 3239 3937 3535  3218 C 24.299755
-00004e20: 2c32 302e 3639 3333 3031 2032 342e 3030  ,20.693301 24.00
-00004e30: 3932 3232 2c31 392e 3033 3638 3032 2032  9222,19.036802 2
-00004e40: 332e 3231 3332 3034 2c31 372e 3633 3037  3.213204,17.6307
-00004e50: 3831 2043 2032 322e 3633 3532 3836 2c31  81 C 22.635286,1
-00004e60: 362e 3539 3739 3320 3231 2e38 3233 3731  6.59793 21.82371
-00004e70: 322c 3135 2e37 3031 3935 3520 3230 2e38  2,15.701955 20.8
-00004e80: 3832 3335 342c 3134 2e39 3836 3232 3320  82354,14.986223 
-00004e90: 4320 3139 2e39 3537 3836 392c 3134 2e32  C 19.957869,14.2
-00004ea0: 3835 3731 3320 3138 2e38 3734 3333 372c  85713 18.874337,
-00004eb0: 3133 2e37 3936 3536 3620 3137 2e37 3334  13.796566 17.734
-00004ec0: 3830 372c 3133 2e35 3732 3931 3920 4320  807,13.572919 C 
-00004ed0: 3136 2e35 3630 3537 392c 3133 2e33 3339  16.560579,13.339
-00004ee0: 3330 3620 3135 2e33 3339 3535 392c 3133  306 15.339559,13
-00004ef0: 2e33 3435 3534 3820 3134 2e31 3635 3434  .345548 14.16544
-00004f00: 312c 3133 2e35 3736 3037 3720 4320 3132  1,13.576077 C 12
-00004f10: 2e38 3832 3031 372c 3133 2e38 3336 3438  .882017,13.83648
-00004f20: 3420 3131 2e36 3730 3834 322c 3134 2e34  4 11.670842,14.4
-00004f30: 3238 3030 3920 3130 2e36 3731 3233 342c  28009 10.671234,
-00004f40: 3135 2e32 3731 3138 2043 2039 2e34 3337  15.27118 C 9.437
-00004f50: 3437 3637 2c31 362e 3239 3439 3034 2038  4767,16.294904 8
-00004f60: 2e34 3639 3038 3834 2c31 372e 3636 3339  .4690884,17.6639
-00004f70: 3634 2038 2e30 3239 3335 3534 2c31 392e  64 8.0293554,19.
-00004f80: 3231 3137 3838 2043 2037 2e36 3533 3135  211788 C 7.65315
-00004f90: 3934 2c32 302e 3532 3336 3633 2037 2e36  94,20.523663 7.6
-00004fa0: 3133 3333 3834 2c32 312e 3932 3637 3832  133384,21.926782
-00004fb0: 2037 2e38 3834 3233 3534 2c32 332e 3236   7.8842354,23.26
-00004fc0: 3235 3439 2043 2038 2e31 3530 3934 3134  2549 C 8.1509414
-00004fd0: 2c32 342e 3533 3232 3631 2038 2e37 3631  ,24.532261 8.761
-00004fe0: 3238 3737 2c32 352e 3732 3337 3235 2039  2877,25.723725 9
-00004ff0: 2e36 3230 3834 3337 2c32 362e 3639 3538  .6208437,26.6958
-00005000: 3836 2043 2031 302e 3530 3232 3838 2c32  86 C 10.502288,2
-00005010: 372e 3730 3630 3132 2031 312e 3539 3734  7.706012 11.5974
-00005020: 3034 2c32 382e 3535 3033 3838 2031 322e  04,28.550388 12.
-00005030: 3835 3430 3733 2c32 392e 3033 3938 3038  854073,29.039808
-00005040: 2043 2031 332e 3833 3830 372c 3239 2e34   C 13.83807,29.4
-00005050: 3333 3138 3520 3134 2e39 3030 3333 372c  33185 14.900337,
-00005060: 3239 2e36 3036 3630 3120 3135 2e39 3537  29.606601 15.957
-00005070: 3932 2c32 392e 3630 3533 3035 207a 2720  92,29.605305 z' 
-00005080: 7374 796c 653d 2766 696c 6c3a 2024 7a6f  style='fill: $zo
-00005090: 6469 6163 5f63 6f6c 6f72 5f31 3b27 202f  diac_color_1;' /
-000050a0: 3e0d 0a20 2020 2020 2020 2020 2020 2020  >..             
-000050b0: 2020 203c 2f73 796d 626f 6c3e 0d0a 2020     </symbol>..  
-000050c0: 2020 2020 2020 2020 2020 2020 2020 3c73                <s
-000050d0: 796d 626f 6c20 6964 3d27 6765 6d69 6e69  ymbol id='gemini
-000050e0: 273e 0d0a 2020 2020 2020 2020 2020 2020  '>..            
-000050f0: 2020 2020 2020 2020 3c70 6174 6820 7472          <path tr
-00005100: 616e 7366 6f72 6d3d 2273 6361 6c65 2830  ansform="scale(0
-00005110: 2e38 2922 2064 3d27 4d20 302e 3536 3534  .8)" d='M 0.5654
-00005120: 3932 3932 2c33 3220 4320 302e 3536 3534  9292,32 C 0.5654
-00005130: 3932 3932 2c33 312e 3231 3432 3338 2030  9292,31.214238 0
-00005140: 2e35 3635 3439 3239 322c 3330 2e34 3238  .56549292,30.428
-00005150: 3436 3520 302e 3536 3534 3932 3932 2c32  465 0.56549292,2
-00005160: 392e 3634 3237 3033 2043 2032 2e39 3637  9.642703 C 2.967
-00005170: 3531 3139 2c32 392e 3031 3131 3136 2035  5119,29.011116 5
-00005180: 2e34 3032 3335 3733 2c32 382e 3438 3631  .4023573,28.4861
-00005190: 3535 2037 2e38 3639 3737 3034 2c32 382e  55 7.8697704,28.
-000051a0: 3138 3837 3932 2043 2037 2e38 3639 3737  188792 C 7.86977
-000051b0: 3034 2c32 302e 3034 3838 3137 2037 2e38  04,20.048817 7.8
-000051c0: 3639 3737 3034 2c31 312e 3930 3838 3332  697704,11.908832
-000051d0: 2037 2e38 3639 3737 3034 2c33 2e37 3638   7.8697704,3.768
-000051e0: 3835 3731 2043 2035 2e33 3937 3631 3436  8571 C 5.3976146
-000051f0: 2c33 2e35 3338 3935 3731 2032 2e39 3530  ,3.5389571 2.950
-00005200: 3036 3239 2c33 2e30 3631 3633 3931 2030  0629,3.0616391 0
-00005210: 2e35 3635 3439 3239 322c 322e 3337 3134  .56549292,2.3714
-00005220: 3130 3820 4320 302e 3536 3534 3932 3932  108 C 0.56549292
-00005230: 2c31 2e35 3830 3934 3233 2030 2e35 3635  ,1.5809423 0.565
-00005240: 3439 3239 322c 302e 3739 3034 3733 3920  49292,0.7904739 
-00005250: 302e 3536 3534 3932 3932 2c2d 3565 2d30  0.56549292,-5e-0
-00005260: 3620 4320 342e 3133 3030 3435 392c 302e  6 C 4.1300459,0.
-00005270: 3938 3039 3330 3620 372e 3831 3834 3037  9809306 7.818407
-00005280: 382c 312e 3433 3632 3532 2031 312e 3530  8,1.436252 11.50
-00005290: 3238 3033 2c31 2e36 3432 3836 3935 2043  2803,1.6428695 C
-000052a0: 2031 342e 3639 3934 312c 312e 3831 3135   14.69941,1.8115
-000052b0: 3537 3420 3137 2e39 3035 3733 2c31 2e38  574 17.90573,1.8
-000052c0: 3037 3034 3832 2032 312e 3130 3136 3131  070482 21.101611
-000052d0: 2c31 2e36 3234 3037 3538 2043 2032 342e  ,1.6240758 C 24.
-000052e0: 3637 3732 3334 2c31 2e34 3038 3139 3120  677234,1.408191 
-000052f0: 3238 2e32 3534 3734 322c 302e 3935 3235  28.254742,0.9525
-00005300: 3638 3920 3331 2e37 3134 3432 362c 2d35  689 31.714426,-5
-00005310: 652d 3036 2043 2033 312e 3731 3434 3236  e-06 C 31.714426
-00005320: 2c30 2e37 3930 3437 3339 2033 312e 3731  ,0.7904739 31.71
-00005330: 3434 3236 2c31 2e35 3830 3934 3233 2033  4426,1.5809423 3
-00005340: 312e 3731 3434 3236 2c32 2e33 3731 3431  1.714426,2.37141
-00005350: 3038 2043 2032 392e 3332 3435 3032 2c33  08 C 29.324502,3
-00005360: 2e30 3539 3334 3831 2032 362e 3837 3238  .0593481 26.8728
-00005370: 3239 2c33 2e35 3338 3636 3731 2032 342e  29,3.5386671 24.
-00005380: 3339 3630 3435 2c33 2e37 3638 3835 3731  396045,3.7688571
-00005390: 2043 2032 342e 3339 3630 3435 2c31 312e   C 24.396045,11.
-000053a0: 3930 3838 3332 2032 342e 3339 3630 3435  908832 24.396045
-000053b0: 2c32 302e 3034 3838 3137 2032 342e 3339  ,20.048817 24.39
-000053c0: 3630 3435 2c32 382e 3138 3837 3932 2043  6045,28.188792 C
-000053d0: 2032 362e 3836 3830 3335 2c32 382e 3438   26.868035,28.48
-000053e0: 3637 3034 2032 392e 3330 3731 3637 2c32  6704 29.307167,2
-000053f0: 392e 3031 3331 3538 2033 312e 3731 3434  9.013158 31.7144
-00005400: 3236 2c32 392e 3634 3237 3033 2043 2033  26,29.642703 C 3
-00005410: 312e 3731 3434 3236 2c33 302e 3432 3834  1.714426,30.4284
-00005420: 3635 2033 312e 3731 3434 3236 2c33 312e  65 31.714426,31.
-00005430: 3231 3432 3338 2033 312e 3731 3434 3236  214238 31.714426
-00005440: 2c33 3220 4320 3236 2e30 3731 3737 2c33  ,32 C 26.07177,3
-00005450: 302e 3531 3238 3636 2032 302e 3230 3634  0.512866 20.2064
-00005460: 3332 2c32 392e 3939 3339 3238 2031 342e  32,29.993928 14.
-00005470: 3338 3332 3731 2c33 302e 3132 3932 3738  383271,30.129278
-00005480: 2043 2039 2e37 3238 3135 3336 2c33 302e   C 9.7281536,30.
-00005490: 3234 3031 3936 2035 2e30 3732 3133 3439  240196 5.0721349
-000054a0: 2c33 302e 3830 3837 3737 2030 2e35 3635  ,30.808777 0.565
-000054b0: 3439 3239 322c 3332 207a 204d 2031 302e  49292,32 z M 10.
-000054c0: 3730 3430 3533 2c32 382e 3031 3934 3120  704053,28.01941 
-000054d0: 4320 3132 2e39 3834 3434 382c 3237 2e37  C 12.984448,27.7
-000054e0: 3635 3336 3720 3135 2e32 3833 3232 342c  65367 15.283224,
-000054f0: 3237 2e37 3232 3738 3320 3137 2e35 3735  27.722783 17.575
-00005500: 3533 392c 3237 2e37 3636 3830 3820 4320  539,27.766808 C 
-00005510: 3138 2e39 3036 3838 362c 3237 2e37 3936  18.906886,27.796
-00005520: 3931 3220 3230 2e32 3338 3134 2c32 372e  912 20.23814,27.
-00005530: 3837 3030 3635 2032 312e 3536 3137 3632  870065 21.561762
-00005540: 2c32 382e 3031 3934 3120 4320 3231 2e35  ,28.01941 C 21.5
-00005550: 3631 3736 322c 3230 2e30 3031 3736 3620  61762,20.001766 
-00005560: 3231 2e35 3631 3736 322c 3131 2e39 3834  21.561762,11.984
-00005570: 3132 3120 3231 2e35 3631 3736 322c 332e  121 21.561762,3.
-00005580: 3936 3634 3737 3120 4320 3139 2e31 3839  9664771 C 19.189
-00005590: 3330 382c 342e 3132 3130 3737 3120 3136  308,4.1210771 16
-000055a0: 2e38 3130 3038 312c 342e 3133 3933 3131  .810081,4.139311
-000055b0: 3120 3134 2e34 3333 3531 352c 342e 3130  1 14.433515,4.10
-000055c0: 3933 3633 3120 4320 3133 2e31 3839 3532  93631 C 13.18952
-000055d0: 362c 342e 3039 3030 3832 3120 3131 2e39  6,4.0900821 11.9
-000055e0: 3435 3530 352c 342e 3035 3032 3034 3120  45505,4.0502041 
-000055f0: 3130 2e37 3034 3035 332c 332e 3936 3634  10.704053,3.9664
-00005600: 3737 3120 4320 3130 2e37 3034 3035 332c  771 C 10.704053,
-00005610: 3131 2e39 3834 3132 3120 3130 2e37 3034  11.984121 10.704
-00005620: 3035 332c 3230 2e30 3031 3736 3620 3130  053,20.001766 10
-00005630: 2e37 3034 3035 332c 3238 2e30 3139 3431  .704053,28.01941
-00005640: 207a 2027 2073 7479 6c65 3d27 6669 6c6c   z ' style='fill
-00005650: 3a20 247a 6f64 6961 635f 636f 6c6f 725f  : $zodiac_color_
-00005660: 323b 2720 2f3e 0d0a 2020 2020 2020 2020  2;' />..        
-00005670: 2020 2020 2020 2020 3c2f 7379 6d62 6f6c          </symbol
-00005680: 3e0d 0a20 2020 2020 2020 2020 2020 2020  >..             
-00005690: 2020 203c 7379 6d62 6f6c 2069 643d 2763     <symbol id='c
-000056a0: 616e 6365 7227 3e0d 0a20 2020 2020 2020  ancer'>..       
-000056b0: 2020 2020 2020 2020 2020 2020 203c 7061               <pa
-000056c0: 7468 2074 7261 6e73 666f 726d 3d22 7363  th transform="sc
-000056d0: 616c 6528 302e 3829 2220 643d 274d 2030  ale(0.8)" d='M 0
-000056e0: 2c32 352e 3632 3934 3832 204c 2030 2c32  ,25.629482 L 0,2
-000056f0: 322e 3930 3831 3031 2043 2035 2e32 3437  2.908101 C 5.247
-00005700: 3935 3039 2c32 352e 3330 3439 3134 2031  9509,25.304914 1
-00005710: 302e 3333 3334 3634 2c32 362e 3439 3038  0.333464,26.4908
-00005720: 3337 2031 352e 3233 3135 3531 2c32 362e  37 15.231551,26.
-00005730: 3439 3038 3337 2043 2031 382e 3434 3237  490837 C 18.4427
-00005740: 3937 2c32 362e 3439 3038 3337 2032 312e  97,26.490837 21.
-00005750: 3035 3432 3737 2c32 362e 3037 3838 3834  054277,26.078884
-00005760: 2032 332e 3036 3539 3932 2c32 352e 3234   23.065992,25.24
-00005770: 3234 3937 2043 2032 312e 3739 3134 3839  2497 C 21.791489
-00005780: 2c32 342e 3539 3333 3620 3230 2e38 3239  ,24.59336 20.829
-00005790: 3336 352c 3233 2e37 3639 3435 3520 3230  365,23.769455 20
-000057a0: 2e31 3932 3131 342c 3232 2e37 3833 3236  .192114,22.78326
-000057b0: 3720 4320 3139 2e35 3534 3836 332c 3231  7 C 19.554863,21
-000057c0: 2e37 3937 3037 3820 3139 2e32 3239 3939  .797078 19.22999
-000057d0: 2c32 302e 3633 3631 3232 2031 392e 3232  ,20.636122 19.22
-000057e0: 3939 392c 3139 2e33 3030 3339 3820 4320  999,19.300398 C 
-000057f0: 3139 2e32 3239 3939 2c31 372e 3535 3237  19.22999,17.5527
-00005800: 3232 2031 392e 3836 3732 3431 2c31 362e  22 19.867241,16.
-00005810: 3035 3437 3134 2032 312e 3132 3932 3438  054714 21.129248
-00005820: 2c31 342e 3739 3338 3931 2043 2032 322e  ,14.793891 C 22.
-00005830: 3337 3837 362c 3133 2e35 3435 3535 3120  37876,13.545551 
-00005840: 3233 2e39 3033 3136 352c 3132 2e39 3231  23.903165,12.921
-00005850: 3338 3120 3235 2e36 3532 3438 312c 3132  381 25.652481,12
-00005860: 2e39 3231 3338 3120 4320 3237 2e34 3031  .921381 C 27.401
-00005870: 3739 382c 3132 2e39 3231 3338 3120 3238  798,12.921381 28
-00005880: 2e38 3838 3731 382c 3133 2e35 3435 3535  .888718,13.54555
-00005890: 3120 3330 2e31 3338 3233 2c31 342e 3738  1 30.13823,14.78
-000058a0: 3134 3037 2043 2033 312e 3337 3532 3436  1407 C 31.375246
-000058b0: 2c31 362e 3032 3937 3437 2033 322e 3030  ,16.029747 32.00
-000058c0: 3030 3032 2c31 372e 3531 3532 3732 2033  0002,17.515272 3
-000058d0: 322e 3030 3030 3032 2c31 392e 3237 3534  2.000002,19.2754
-000058e0: 3331 2043 2033 322e 3030 3030 3032 2c32  31 C 32.000002,2
-000058f0: 322e 3035 3932 3320 3330 2e33 3030 3636  2.05923 30.30066
-00005900: 362c 3234 2e33 3831 3134 3220 3236 2e38  6,24.381142 26.8
-00005910: 3839 3439 382c 3236 2e32 3238 3638 3520  89498,26.228685 
-00005920: 4320 3233 2e34 3738 3333 312c 3238 2e30  C 23.478331,28.0
-00005930: 3736 3232 3820 3139 2e32 3035 2c32 3920  76228 19.205,29 
-00005940: 3134 2e30 3639 3530 352c 3239 2043 2039  14.069505,29 C 9
-00005950: 2e36 3231 3234 3239 2c32 3920 342e 3933  .6212429,29 4.93
-00005960: 3535 3732 392c 3237 2e38 3838 3937 3720  55729,27.888977 
-00005970: 302c 3235 2e36 3239 3438 3220 7a20 4d20  0,25.629482 z M 
-00005980: 3230 2e39 3136 3833 312c 3139 2e33 3132  20.916831,19.312
-00005990: 3838 3220 4320 3230 2e39 3136 3833 312c  882 C 20.916831,
-000059a0: 3230 2e35 3836 3138 3820 3231 2e33 3739  20.586188 21.379
-000059b0: 3135 2c32 312e 3638 3437 3238 2032 322e  15,21.684728 22.
-000059c0: 3331 3632 3834 2c32 322e 3630 3834 3939  316284,22.608499
-000059d0: 2043 2032 332e 3234 3039 3233 2c32 332e   C 23.240923,23.
-000059e0: 3533 3232 3731 2032 342e 3336 3534 3834  532271 24.365484
-000059f0: 2c32 332e 3939 3431 3537 2032 352e 3635  ,23.994157 25.65
-00005a00: 3234 3831 2c32 332e 3939 3431 3537 2043  2481,23.994157 C
-00005a10: 2032 362e 3935 3139 3734 2c32 332e 3939   26.951974,23.99
-00005a20: 3431 3537 2032 382e 3035 3135 3435 2c32  4157 28.051545,2
-00005a30: 332e 3533 3232 3731 2032 382e 3936 3336  3.532271 28.9636
-00005a40: 3838 2c32 322e 3634 3539 3439 2043 2032  88,22.645949 C 2
-00005a50: 392e 3836 3333 3337 2c32 312e 3734 3731  9.863337,21.7471
-00005a60: 3435 2033 302e 3331 3331 3631 2c32 302e  45 30.313161,20.
-00005a70: 3634 3836 3035 2033 302e 3331 3331 3631  648605 30.313161
-00005a80: 2c31 392e 3335 3033 3332 2043 2033 302e  ,19.350332 C 30.
-00005a90: 3331 3331 3631 2c31 382e 3032 3730 3931  313161,18.027091
-00005aa0: 2032 392e 3836 3333 3337 2c31 362e 3930   29.863337,16.90
-00005ab0: 3335 3835 2032 382e 3935 3131 3933 2c31  3585 28.951193,1
-00005ac0: 352e 3937 3938 3134 2043 2032 382e 3033  5.979814 C 28.03
-00005ad0: 3930 3439 2c31 352e 3035 3630 3432 2032  9049,15.056042 2
-00005ae0: 362e 3933 3934 3739 2c31 342e 3539 3431  6.939479,14.5941
-00005af0: 3536 2032 352e 3633 3939 3836 2c31 342e  56 25.639986,14.
-00005b00: 3539 3431 3536 2043 2032 342e 3332 3739  594156 C 24.3279
-00005b10: 3939 2c31 342e 3539 3431 3536 2032 332e  99,14.594156 23.
-00005b20: 3231 3539 3333 2c31 352e 3035 3630 3432  215933,15.056042
-00005b30: 2032 322e 3239 3132 3934 2c31 352e 3937   22.291294,15.97
-00005b40: 3938 3134 2043 2032 312e 3337 3931 352c  9814 C 21.37915,
-00005b50: 3136 2e38 3931 3130 3220 3230 2e39 3136  16.891102 20.916
-00005b60: 3833 312c 3138 2e30 3032 3132 3520 3230  831,18.002125 20
-00005b70: 2e39 3136 3833 312c 3139 2e33 3132 3838  .916831,19.31288
-00005b80: 3220 7a20 4d20 3332 2e30 3030 3030 322c  2 z M 32.000002,
-00005b90: 372e 3331 3633 3334 3120 4c20 3332 2e30  7.3163341 L 32.0
-00005ba0: 3030 3030 322c 3130 2e30 3337 3731 3520  00002,10.037715 
-00005bb0: 4320 3236 2e37 3339 3535 372c 372e 3634  C 26.739557,7.64
-00005bc0: 3039 3032 3520 3231 2e36 3636 3533 382c  09025 21.666538,
-00005bd0: 362e 3434 3234 3936 3220 3136 2e37 3535  6.4424962 16.755
-00005be0: 3935 362c 362e 3434 3234 3936 3220 4320  956,6.4424962 C 
-00005bf0: 3133 2e35 3537 3230 352c 362e 3434 3234  13.557205,6.4424
-00005c00: 3936 3220 3130 2e39 3333 3233 2c36 2e38  962 10.93323,6.8
-00005c10: 3534 3434 3833 2038 2e39 3039 3032 3039  544483 8.9090209
-00005c20: 2c37 2e37 3033 3331 3935 2043 2031 302e  ,7.7033195 C 10.
-00005c30: 3230 3835 3133 2c38 2e33 3532 3435 3633  208513,8.3524563
-00005c40: 2031 312e 3137 3036 3337 2c39 2e31 3736   11.170637,9.176
-00005c50: 3336 3037 2031 312e 3739 3533 3933 2c31  3607 11.795393,1
-00005c60: 302e 3136 3235 3439 2043 2031 322e 3434  0.162549 C 12.44
-00005c70: 3531 342c 3131 2e31 3438 3733 3820 3132  514,11.148738 12
-00005c80: 2e37 3537 3531 382c 3132 2e33 3039 3639  .757518,12.30969
-00005c90: 3420 3132 2e37 3537 3531 382c 3133 2e36  4 12.757518,13.6
-00005ca0: 3435 3431 3820 4320 3132 2e37 3537 3531  45418 C 12.75751
-00005cb0: 382c 3135 2e33 3933 3039 3420 3132 2e31  8,15.393094 12.1
-00005cc0: 3332 3736 322c 3136 2e38 3931 3130 3220  32762,16.891102 
-00005cd0: 3130 2e38 3730 3735 352c 3138 2e31 3531  10.870755,18.151
-00005ce0: 3932 3520 4320 392e 3630 3837 3436 392c  925 C 9.6087469,
-00005cf0: 3139 2e34 3030 3236 3520 382e 3039 3638  19.400265 8.0968
-00005d00: 3337 392c 3230 2e30 3234 3433 3520 362e  379,20.024435 6.
-00005d10: 3333 3530 3235 392c 3230 2e30 3234 3433  3350259,20.02443
-00005d20: 3520 4320 342e 3538 3537 3038 392c 3230  5 C 4.5857089,20
-00005d30: 2e30 3234 3433 3520 332e 3039 3837 3839  .024435 3.098789
-00005d40: 392c 3139 2e34 3132 3734 3920 312e 3836  9,19.412749 1.86
-00005d50: 3137 3732 392c 3138 2e31 3634 3430 3920  17729,18.164409 
-00005d60: 4320 302e 3632 3437 3536 2c31 362e 3932  C 0.624756,16.92
-00005d70: 3835 3532 2030 2c31 352e 3433 3035 3434  8552 0,15.430544
-00005d80: 2030 2c31 332e 3638 3238 3638 2043 2030   0,13.682868 C 0
-00005d90: 2c31 302e 3838 3635 3836 2031 2e36 3939  ,10.886586 1.699
-00005da0: 3333 3634 2c38 2e35 3532 3139 3037 2035  3364,8.5521907 5
-00005db0: 2e31 3130 3530 3339 2c36 2e37 3034 3634  .1105039,6.70464
-00005dc0: 3735 2043 2038 2e35 3039 3137 3639 2c34  75 C 8.5091769,4
-00005dd0: 2e38 3537 3130 3434 2031 322e 3739 3530  .8571044 12.7950
-00005de0: 3033 2c33 2e39 3333 3333 3237 2031 372e  03,3.9333327 17.
-00005df0: 3933 3034 3937 2c33 2e39 3333 3333 3237  930497,3.9333327
-00005e00: 2043 2032 322e 3337 3837 362c 332e 3933   C 22.37876,3.93
-00005e10: 3333 3332 3720 3237 2e30 3634 3433 2c35  33327 27.06443,5
-00005e20: 2e30 3536 3833 3838 2033 322e 3030 3030  .0568388 32.0000
-00005e30: 3032 2c37 2e33 3136 3333 3431 207a 204d  02,7.3163341 z M
-00005e40: 2031 312e 3038 3331 3732 2c31 332e 3633   11.083172,13.63
-00005e50: 3239 3335 2043 2031 312e 3038 3331 3732  2935 C 11.083172
-00005e60: 2c31 322e 3334 3731 3434 2031 302e 3632  ,12.347144 10.62
-00005e70: 3038 3532 2c31 312e 3234 3836 3035 2039  0852,11.248605 9
-00005e80: 2e36 3833 3731 3739 2c31 302e 3332 3438  .6837179,10.3248
-00005e90: 3334 2043 2038 2e37 3436 3538 3339 2c39  34 C 8.7465839,9
-00005ea0: 2e34 3133 3534 3533 2037 2e36 3232 3032  .4135453 7.62202
-00005eb0: 3239 2c38 2e39 3531 3635 3935 2036 2e33  29,8.9516595 6.3
-00005ec0: 3232 3533 3039 2c38 2e39 3531 3635 3935  225309,8.9516595
-00005ed0: 2043 2035 2e30 3233 3033 3739 2c38 2e39   C 5.0230379,8.9
-00005ee0: 3531 3635 3935 2033 2e39 3233 3436 3739  516595 3.9234679
-00005ef0: 2c39 2e34 3031 3036 3139 2033 2e30 3233  ,9.4010619 3.023
-00005f00: 3831 3839 2c31 302e 3239 3938 3637 2043  8189,10.299867 C
-00005f10: 2032 2e31 3234 3137 3039 2c31 312e 3139   2.1241709,11.19
-00005f20: 3836 3732 2031 2e36 3734 3334 3631 2c31  8672 1.6743461,1
-00005f30: 322e 3239 3732 3131 2031 2e36 3734 3334  2.297211 1.67434
-00005f40: 3631 2c31 332e 3539 3534 3834 2043 2031  61,13.595484 C 1
-00005f50: 2e36 3734 3334 3631 2c31 342e 3931 3837  .6743461,14.9187
-00005f60: 3235 2032 2e31 3336 3636 3539 2c31 362e  25 2.1366659,16.
-00005f70: 3034 3232 3331 2033 2e30 3438 3830 3839  042231 3.0488089
-00005f80: 2c31 362e 3936 3630 3032 2043 2033 2e39  ,16.966002 C 3.9
-00005f90: 3438 3435 3739 2c31 372e 3838 3937 3734  484579,17.889774
-00005fa0: 2035 2e30 3630 3532 3339 2c31 382e 3335   5.0605239,18.35
-00005fb0: 3136 3620 362e 3336 3030 3135 392c 3138  166 6.3600159,18
-00005fc0: 2e33 3531 3636 2043 2037 2e36 3539 3530  .35166 C 7.65950
-00005fd0: 3839 2c31 382e 3335 3136 3620 382e 3738  89,18.35166 8.78
-00005fe0: 3430 3638 392c 3137 2e38 3839 3737 3420  40689,17.889774 
-00005ff0: 392e 3639 3632 3132 392c 3136 2e39 3636  9.6962129,16.966
-00006000: 3030 3220 4320 3130 2e36 3230 3835 322c  002 C 10.620852,
-00006010: 3136 2e30 3432 3233 3120 3131 2e30 3833  16.042231 11.083
-00006020: 3137 322c 3134 2e39 3331 3230 3820 3131  172,14.931208 11
-00006030: 2e30 3833 3137 322c 3133 2e36 3332 3933  .083172,13.63293
-00006040: 3520 7a20 2720 7374 796c 653d 2766 696c  5 z ' style='fil
-00006050: 6c3a 2024 7a6f 6469 6163 5f63 6f6c 6f72  l: $zodiac_color
-00006060: 5f33 3b27 202f 3e0d 0a20 2020 2020 2020  _3;' />..       
-00006070: 2020 2020 2020 2020 203c 2f73 796d 626f           </symbo
-00006080: 6c3e 0d0a 2020 2020 2020 2020 2020 2020  l>..            
-00006090: 2020 2020 3c73 796d 626f 6c20 6964 3d27      <symbol id='
-000060a0: 6c65 6f27 3e0d 0a20 2020 2020 2020 2020  leo'>..         
-000060b0: 2020 2020 2020 2020 2020 203c 7061 7468             <path
-000060c0: 2074 7261 6e73 666f 726d 3d22 7363 616c   transform="scal
-000060d0: 6528 302e 3829 2220 643d 274d 2032 382e  e(0.8)" d='M 28.
-000060e0: 3032 3133 3731 2c32 392e 3438 3038 3231  021371,29.480821
-000060f0: 2043 2032 372e 3337 3833 3339 2c33 302e   C 27.378339,30.
-00006100: 3036 3939 3438 2032 362e 3638 3739 3932  069948 26.687992
-00006110: 2c33 302e 3631 3233 3932 2032 352e 3933  ,30.612392 25.93
-00006120: 3336 3032 2c33 312e 3035 3233 3539 2043  3602,31.052359 C
-00006130: 2032 352e 3330 3433 3934 2c33 312e 3431   25.304394,31.41
-00006140: 3837 3031 2032 342e 3632 3734 3239 2c33  8701 24.627429,3
-00006150: 312e 3731 3230 3931 2032 332e 3931 3530  1.712091 23.9150
-00006160: 3232 2c33 312e 3837 3034 3732 2043 2032  22,31.870472 C 2
-00006170: 332e 3438 3738 3037 2c33 312e 3936 3620  3.487807,31.966 
-00006180: 3233 2e30 3438 3937 372c 3332 2e30 3130  23.048977,32.010
-00006190: 3236 3220 3232 2e36 3131 3237 392c 3331  262 22.611279,31
-000061a0: 2e39 3937 3939 3820 4320 3231 2e39 3936  .997998 C 21.996
-000061b0: 3038 352c 3331 2e39 3834 3135 3720 3231  085,31.984157 21
-000061c0: 2e33 3830 3334 352c 3331 2e38 3737 3435  .380345,31.87745
-000061d0: 3420 3230 2e38 3034 3931 312c 3331 2e36  4 20.804911,31.6
-000061e0: 3536 3432 3620 4320 3230 2e32 3733 3435  56426 C 20.27345
-000061f0: 392c 3331 2e34 3533 3739 2031 392e 3738  9,31.45379 19.78
-00006200: 3034 322c 3331 2e31 3533 3930 3320 3139  042,31.153903 19
-00006210: 2e33 3530 3435 352c 3330 2e37 3832 3032  .350455,30.78202
-00006220: 3820 4320 3139 2e30 3135 3934 2c33 302e  8 C 19.01594,30.
-00006230: 3439 3337 3639 2031 382e 3731 3830 3032  493769 18.718002
-00006240: 2c33 302e 3136 3237 3537 2031 382e 3436  ,30.162757 18.46
-00006250: 3737 3632 2c32 392e 3739 3838 3436 2043  7762,29.798846 C
-00006260: 2031 382e 3135 3837 3831 2c32 392e 3334   18.158781,29.34
-00006270: 3936 3333 2031 372e 3932 3937 3832 2c32  9633 17.929782,2
-00006280: 382e 3834 3537 3339 2031 372e 3739 3437  8.845739 17.7947
-00006290: 3235 2c32 382e 3331 3734 3739 2043 2031  25,28.317479 C 1
-000062a0: 372e 3633 3539 342c 3237 2e37 3030 3837  7.63594,27.70087
-000062b0: 3120 3137 2e36 3031 3335 352c 3237 2e30  1 17.601355,27.0
-000062c0: 3536 3233 3720 3137 2e36 3538 3839 362c  56237 17.658896,
-000062d0: 3236 2e34 3233 3430 3220 4320 3137 2e37  26.423402 C 17.7
-000062e0: 3136 3438 352c 3235 2e37 3833 3837 3220  16485,25.783872 
-000062f0: 3137 2e38 3438 3031 332c 3235 2e31 3533  17.848013,25.153
-00006300: 3330 3620 3138 2e30 3038 3434 392c 3234  306 18.008449,24
-00006310: 2e35 3332 3335 3420 4320 3138 2e32 3536  .532354 C 18.256
-00006320: 3930 352c 3233 2e35 3830 3631 3120 3138  905,23.580611 18
-00006330: 2e35 3737 3837 332c 3232 2e36 3439 3335  .577873,22.64935
-00006340: 2031 382e 3932 3834 3931 2c32 312e 3733   18.928491,21.73
-00006350: 3038 3733 2043 2031 392e 3434 3439 3538  0873 C 19.444958
-00006360: 2c32 302e 3338 3337 3136 2032 302e 3033  ,20.383716 20.03
-00006370: 3031 3734 2c31 392e 3036 3339 3838 2032  0174,19.063988 2
-00006380: 302e 3634 3439 3731 2c31 372e 3735 3931  0.644971,17.7591
-00006390: 3434 2043 2032 312e 3133 3732 3035 2c31  44 C 21.137205,1
-000063a0: 362e 3731 3031 3031 2032 312e 3632 3934  6.710101 21.6294
-000063b0: 3337 2c31 352e 3636 3130 3620 3232 2e31  37,15.66106 22.1
-000063c0: 3231 3636 392c 3134 2e36 3132 3031 3720  21669,14.612017 
-000063d0: 4320 3232 2e35 3633 3232 372c 3133 2e36  C 22.563227,13.6
-000063e0: 3635 3230 3820 3232 2e39 3635 3734 332c  65208 22.965743,
-000063f0: 3132 2e36 3938 3435 2032 332e 3238 3630  12.69845 23.2860
-00006400: 3532 2c31 312e 3730 3334 3332 2043 2032  52,11.703432 C 2
-00006410: 332e 3531 3430 3939 2c31 302e 3939 3037  3.514099,10.9907
-00006420: 3120 3233 2e37 3031 3235 352c 3130 2e32  1 23.701255,10.2
-00006430: 3632 3530 3420 3233 2e38 3031 3138 312c  62504 23.801181,
-00006440: 392e 3532 3030 3238 3620 4320 3233 2e38  9.5200286 C 23.8
-00006450: 3532 3139 362c 392e 3134 3035 3734 3620  52196,9.1405746 
-00006460: 3233 2e38 3737 3538 372c 382e 3735 3733  23.877587,8.7573
-00006470: 3931 3620 3233 2e38 3639 3331 312c 382e  916 23.869311,8.
-00006480: 3337 3434 3736 3620 4320 3233 2e38 3536  3744766 C 23.856
-00006490: 3839 392c 372e 3538 3639 3331 3420 3233  899,7.5869314 23
-000064a0: 2e37 3530 3534 392c 362e 3739 3635 3631  .750549,6.796561
-000064b0: 3820 3233 2e35 3035 3330 312c 362e 3034  8 23.505301,6.04
-000064c0: 3633 3633 3520 4320 3233 2e33 3031 3035  63635 C 23.30105
-000064d0: 382c 352e 3431 3836 3035 2032 322e 3939  8,5.418605 22.99
-000064e0: 3635 3539 2c34 2e38 3232 3436 3734 2032  6559,4.8224674 2
-000064f0: 322e 3539 3734 3031 2c34 2e32 3936 3134  2.597401,4.29614
-00006500: 3231 2043 2032 322e 3337 3131 3037 2c33  21 C 22.371107,3
-00006510: 2e39 3937 3138 3831 2032 322e 3131 3538  .9971881 22.1158
-00006520: 382c 332e 3732 3033 3533 3220 3231 2e38  8,3.7203532 21.8
-00006530: 3339 3133 322c 332e 3436 3735 3333 3320  39132,3.4675333 
-00006540: 4320 3231 2e33 3739 3338 2c33 2e30 3438  C 21.37938,3.048
-00006550: 3735 3332 2032 302e 3834 3836 312c 322e  7532 20.84861,2.
-00006560: 3730 3832 3432 3420 3230 2e32 3735 3832  7082424 20.27582
-00006570: 362c 322e 3436 3630 3137 3420 4320 3139  6,2.4660174 C 19
-00006580: 2e36 3233 3230 312c 322e 3138 3834 3239  .623201,2.188429
-00006590: 2031 382e 3932 3133 3531 2c32 2e30 3337   18.921351,2.037
-000065a0: 3339 3720 3138 2e32 3135 3538 2c31 2e39  397 18.21558,1.9
-000065b0: 3833 3439 3733 2043 2031 372e 3730 3839  834973 C 17.7089
-000065c0: 3532 2c31 2e39 3435 3538 3832 2031 372e  52,1.9455882 17.
-000065d0: 3139 3836 3931 2c31 2e39 3530 3435 3832  198691,1.9504582
-000065e0: 2031 362e 3639 3333 3834 2c32 2e30 3034   16.693384,2.004
-000065f0: 3330 3534 2043 2031 362e 3031 3834 3435  3054 C 16.018445
-00006600: 2c32 2e30 3736 3536 3038 2031 352e 3335  ,2.0765608 15.35
-00006610: 3038 3238 2c32 2e32 3434 3737 3636 2031  0828,2.2447766 1
-00006620: 342e 3733 3431 3731 2c32 2e35 3331 3330  4.734171,2.53130
-00006630: 3833 2043 2031 342e 3137 3731 3035 2c32  83 C 14.177105,2
-00006640: 2e37 3838 3835 3720 3133 2e36 3635 3034  .788857 13.66504
-00006650: 332c 332e 3134 3233 3937 3520 3133 2e32  3,3.1423975 13.2
-00006660: 3234 3331 382c 332e 3536 3933 3437 3920  24318,3.5693479 
-00006670: 4320 3132 2e37 3935 3533 352c 332e 3939  C 12.795535,3.99
-00006680: 3531 3333 3320 3132 2e34 3335 3435 372c  51333 12.435457,
-00006690: 342e 3439 3132 3431 3820 3132 2e31 3732  4.4912418 12.172
-000066a0: 3731 392c 352e 3033 3538 3737 3320 4320  719,5.0358773 C 
-000066b0: 3131 2e38 3930 3039 342c 352e 3631 3831  11.890094,5.6181
-000066c0: 3436 3720 3131 2e37 3139 3634 322c 362e  467 11.719642,6.
-000066d0: 3235 3133 3038 3120 3131 2e36 3433 3934  2513081 11.64394
-000066e0: 372c 362e 3839 3331 3032 3920 4320 3131  7,6.8931029 C 11
-000066f0: 2e35 3632 3031 372c 372e 3538 3434 3332  .562017,7.584432
-00006700: 3320 3131 2e35 3832 3832 2c38 2e32 3835  3 11.58282,8.285
-00006710: 3733 3936 2031 312e 3638 3035 3333 2c38  7396 11.680533,8
-00006720: 2e39 3734 3330 3336 2043 2031 312e 3830  .9743036 C 11.80
-00006730: 3630 3831 2c39 2e38 3631 3736 3036 2031  6081,9.8617606 1
-00006740: 322e 3034 3839 3735 2c31 302e 3732 3931  2.048975,10.7291
-00006750: 3532 2031 322e 3335 3430 3333 2c31 312e  52 12.354033,11.
-00006760: 3537 3036 3931 2043 2031 322e 3539 3837  570691 C 12.5987
-00006770: 3938 2c31 322e 3234 3438 3337 2031 322e  98,12.244837 12.
-00006780: 3838 3534 3939 2c31 322e 3930 3331 3137  885499,12.903117
-00006790: 2031 332e 3139 3833 3938 2c31 332e 3534   13.198398,13.54
-000067a0: 3832 3638 2043 2031 332e 3430 3939 3634  8268 C 13.409964
-000067b0: 2c31 332e 3938 3736 3832 2031 332e 3632  ,13.987682 13.62
-000067c0: 3139 3131 2c31 342e 3432 3639 3135 2031  1911,14.426915 1
-000067d0: 332e 3833 3331 3731 2c31 342e 3836 3634  3.833171,14.8664
-000067e0: 3735 2043 2031 342e 3138 3034 3838 2c31  75 C 14.180488,1
-000067f0: 352e 3539 3620 3134 2e35 3037 3836 332c  5.596 14.507863,
-00006800: 3136 2e33 3336 3131 3620 3134 2e37 3831  16.336116 14.781
-00006810: 3734 2c31 372e 3039 3636 3634 2043 2031  74,17.096664 C 1
-00006820: 342e 3935 3436 3339 2c31 372e 3538 3039  4.954639,17.5809
-00006830: 3033 2031 352e 3130 3737 3431 2c31 382e  03 15.107741,18.
-00006840: 3037 3338 3938 2031 352e 3230 3436 3634  073898 15.204664
-00006850: 2c31 382e 3537 3934 3638 2043 2031 352e  ,18.579468 C 15.
-00006860: 3236 3036 3135 2c31 382e 3837 3434 3034  260615,18.874404
-00006870: 2031 352e 3239 3539 3035 2c31 392e 3137   15.295905,19.17
-00006880: 3434 3932 2031 352e 3238 3835 3031 2c31  4492 15.288501,1
-00006890: 392e 3437 3530 3936 2043 2031 352e 3237  9.475096 C 15.27
-000068a0: 3935 3331 2c32 302e 3132 3030 3634 2031  9531,20.120064 1
-000068b0: 352e 3136 3430 3538 2c32 302e 3736 3435  5.164058,20.7645
-000068c0: 3735 2031 342e 3933 3633 322c 3231 2e33  75 14.93632,21.3
-000068d0: 3638 3536 3320 4320 3134 2e37 3032 3536  68563 C 14.70256
-000068e0: 322c 3231 2e39 3932 3933 3820 3134 2e33  2,21.992938 14.3
-000068f0: 3531 3339 362c 3232 2e35 3730 3337 3720  51396,22.570377 
-00006900: 3133 2e39 3232 3631 342c 3233 2e30 3739  13.922614,23.079
-00006910: 3732 3920 4320 3133 2e35 3936 3136 382c  729 C 13.596168,
-00006920: 3233 2e34 3636 3736 3820 3133 2e32 3239  23.466768 13.229
-00006930: 3434 352c 3233 2e38 3230 3330 3520 3132  445,23.820305 12
-00006940: 2e38 3238 3031 2c32 342e 3132 3930 3036  .82801,24.129006
-00006950: 2043 2031 322e 3330 3034 3934 2c32 342e   C 12.300494,24.
-00006960: 3533 3436 3533 2031 312e 3730 3730 3231  534653 11.707021
-00006970: 2c32 342e 3835 3632 3737 2031 312e 3037  ,24.856277 11.07
-00006980: 3433 352c 3235 2e30 3634 3034 3120 4320  435,25.064041 C 
-00006990: 3130 2e34 3238 3035 332c 3235 2e32 3737  10.428053,25.277
-000069a0: 3930 3920 392e 3734 3439 3337 352c 3235  909 9.7449375,25
-000069b0: 2e33 3732 3139 3320 392e 3036 3530 3339  .372193 9.065039
-000069c0: 392c 3235 2e33 3633 3736 3720 4320 382e  9,25.363767 C 8.
-000069d0: 3337 3539 3539 332c 3235 2e33 3536 3836  3759593,25.35686
-000069e0: 3920 372e 3638 3535 3031 382c 3235 2e32  9 7.6855018,25.2
-000069f0: 3437 3539 3120 372e 3033 3535 3831 392c  47591 7.0355819,
-00006a00: 3235 2e30 3135 3535 3720 4320 362e 3432  25.015557 C 6.42
-00006a10: 3232 3433 372c 3234 2e37 3938 3133 3820  22437,24.798138 
-00006a20: 352e 3834 3839 3638 372c 3234 2e34 3731  5.8489687,24.471
-00006a30: 3730 3620 352e 3334 3239 3131 382c 3234  706 5.3429118,24
-00006a40: 2e30 3633 3133 3320 4320 352e 3034 3339  .063133 C 5.0439
-00006a50: 3639 352c 3233 2e38 3232 3332 3820 342e  695,23.822328 4.
-00006a60: 3736 3737 3439 312c 3233 2e35 3533 3839  7677491,23.55389
-00006a70: 3820 342e 3531 3233 3537 332c 3233 2e32  8 4.5123573,23.2
-00006a80: 3637 3520 4320 342e 3037 3535 3533 312c  675 C 4.0755531,
-00006a90: 3232 2e37 3735 3634 3820 332e 3731 3431  22.775648 3.7141
-00006aa0: 3734 322c 3232 2e32 3134 3934 3420 332e  742,22.214944 3.
-00006ab0: 3436 3136 3531 382c 3231 2e36 3036 3834  4616518,21.60684
-00006ac0: 3420 4320 332e 3230 3337 3737 372c 3230  4 C 3.2037777,20
-00006ad0: 2e39 3839 3935 2033 2e30 3539 3433 3738  .98995 3.0594378
-00006ae0: 2c32 302e 3332 3832 3539 2033 2e30 3135  ,20.328259 3.015
-00006af0: 3739 3238 2c31 392e 3636 3138 3036 2043  7928,19.661806 C
-00006b00: 2032 2e39 3639 3330 3138 2c31 382e 3935   2.9693018,18.95
-00006b10: 3534 3333 2033 2e30 3233 3138 3338 2c31  5433 3.0231838,1
-00006b20: 382e 3233 3933 3937 2033 2e32 3037 3731  8.239397 3.20771
-00006b30: 3034 2c31 372e 3535 3437 3420 4320 332e  04,17.55474 C 3.
-00006b40: 3337 3237 3232 352c 3136 2e39 3337 3233  3727225,16.93723
-00006b50: 3320 332e 3634 3437 3337 332c 3136 2e33  3 3.6447373,16.3
-00006b60: 3439 3139 3420 342e 3030 3431 3339 392c  49194 4.0041399,
-00006b70: 3135 2e38 3230 3930 3120 4320 342e 3330  15.820901 C 4.30
-00006b80: 3237 3433 2c31 352e 3337 3939 3036 2034  2743,15.379906 4
-00006b90: 2e36 3630 3732 3038 2c31 342e 3938 3130  .6607208,14.9810
-00006ba0: 3834 2035 2e30 3532 3631 3236 2c31 342e  84 5.0526126,14.
-00006bb0: 3632 3132 3733 2043 2035 2e35 3432 3133  621273 C 5.54213
-00006bc0: 3939 2c31 342e 3137 3334 3637 2036 2e31  99,14.173467 6.1
-00006bd0: 3031 3336 3239 2c31 332e 3739 3837 3334  013629,13.798734
-00006be0: 2036 2e37 3132 3139 3433 2c31 332e 3533   6.7121943,13.53
-00006bf0: 3736 3733 2043 2037 2e33 3032 3038 3837  7673 C 7.3020887
-00006c00: 2c31 332e 3238 3339 3120 372e 3933 3638  ,13.28391 7.9368
-00006c10: 3232 312c 3133 2e31 3338 3736 3120 382e  221,13.138761 8.
-00006c20: 3537 3731 3632 352c 3133 2e30 3937 3734  5771625,13.09774
-00006c30: 3920 4320 382e 3839 3731 3538 342c 3133  9 C 8.8971584,13
-00006c40: 2e30 3736 3731 3720 392e 3231 3839 3833  .076717 9.218983
-00006c50: 372c 3133 2e30 3739 3437 3320 392e 3533  7,13.079473 9.53
-00006c60: 3830 3932 332c 3133 2e31 3132 3337 3620  80923,13.112376 
-00006c70: 4320 3130 2e30 3138 3332 352c 3133 2e31  C 10.018325,13.1
-00006c80: 3630 3836 3420 3130 2e34 3931 3431 352c  60864 10.491415,
-00006c90: 3133 2e32 3637 3532 2031 302e 3935 3138  13.26752 10.9518
-00006ca0: 3737 2c31 332e 3431 3038 3531 2043 2031  77,13.410851 C 1
-00006cb0: 302e 3437 3636 3738 2c31 322e 3439 3332  0.476678,12.4932
-00006cc0: 3632 2031 302e 3035 3639 3531 2c31 312e  62 10.056951,11.
-00006cd0: 3534 3430 3535 2039 2e37 3435 3831 3636  544055 9.7458166
-00006ce0: 2c31 302e 3535 3736 3538 2043 2039 2e34  ,10.557658 C 9.4
-00006cf0: 3931 3634 322c 392e 3734 3838 3238 3620  91642,9.7488286 
-00006d00: 392e 3331 3039 3631 392c 382e 3931 3238  9.3109619,8.9128
-00006d10: 3534 3620 392e 3236 3232 3431 362c 382e  546 9.2622416,8.
-00006d20: 3036 3439 3732 3620 4320 392e 3233 3633  0649726 C 9.2363
-00006d30: 3035 2c37 2e36 3033 3133 3038 2039 2e32  05,7.6031308 9.2
-00006d40: 3530 3631 372c 372e 3133 3931 3239 3720  50617,7.1391297 
-00006d50: 392e 3330 3132 3635 392c 362e 3637 3934  9.3012659,6.6794
-00006d60: 3130 3720 4320 392e 3338 3632 3530 372c  107 C 9.3862507,
-00006d70: 352e 3931 3332 3638 3520 392e 3538 3638  5.9132685 9.5868
-00006d80: 3830 322c 352e 3135 3832 3033 3820 392e  802,5.1582038 9.
-00006d90: 3931 3237 3533 372c 342e 3435 3838 3438  9127537,4.458848
-00006da0: 3720 4320 3130 2e32 3333 3534 372c 332e  7 C 10.233547,3.
-00006db0: 3736 3634 3839 3620 3130 2e36 3735 3137  7664896 10.67517
-00006dc0: 312c 332e 3133 3235 3220 3131 2e31 3939  1,3.13252 11.199
-00006dd0: 3734 382c 322e 3537 3933 3138 3820 4320  748,2.5793188 C 
-00006de0: 3131 2e38 3531 3530 312c 312e 3839 3237  11.851501,1.8927
-00006df0: 3037 3820 3132 2e36 3139 3630 342c 312e  078 12.619604,1.
-00006e00: 3331 3434 3734 3620 3133 2e34 3637 3937  3144746 13.46797
-00006e10: 352c 302e 3839 3330 3336 3732 2043 2031  5,0.89303672 C 1
-00006e20: 342e 3233 3735 3436 2c30 2e35 3039 3130  4.237546,0.50910
-00006e30: 3738 3220 3135 2e30 3639 3536 372c 302e  782 15.069567,0.
-00006e40: 3235 3631 3731 3432 2031 352e 3931 3833  25617142 15.9183
-00006e50: 3931 2c30 2e31 3233 3038 3639 3220 4320  91,0.12308692 C 
-00006e60: 3136 2e37 3434 3435 392c 2d30 2e30 3037  16.744459,-0.007
-00006e70: 3233 3732 3833 3820 3137 2e35 3835 3435  2372838 17.58545
-00006e80: 322c 2d30 2e30 3236 3938 3737 3834 2031  2,-0.026987784 1
-00006e90: 382e 3431 3839 3737 2c30 2e30 3239 3338  8.418977,0.02938
-00006ea0: 3636 3136 2043 2031 392e 3336 3932 3935  6616 C 19.369295
-00006eb0: 2c30 2e30 3935 3336 3739 3136 2032 302e  ,0.095367916 20.
-00006ec0: 3331 3534 3834 2c30 2e32 3739 3538 3731  315484,0.2795871
-00006ed0: 3220 3231 2e32 3036 3335 382c 302e 3632  2 21.206358,0.62
-00006ee0: 3133 3736 3132 2043 2032 312e 3937 3132  137612 C 21.9712
-00006ef0: 3739 2c30 2e39 3133 3537 3930 3220 3232  79,0.91357902 22
-00006f00: 2e36 3931 3634 332c 312e 3332 3338 3037  .691643,1.323807
-00006f10: 3520 3233 2e33 3238 3433 312c 312e 3833  5 23.328431,1.83
-00006f20: 3930 3835 3620 4320 3233 2e36 3231 3036  90856 C 23.62106
-00006f30: 322c 322e 3037 3533 3636 3720 3233 2e38  2,2.0753667 23.8
-00006f40: 3937 3239 312c 322e 3333 3232 3136 3820  97291,2.3322168 
-00006f50: 3234 2e31 3530 3531 332c 322e 3631 3034  24.150513,2.6104
-00006f60: 3531 3220 4320 3234 2e36 3835 3335 362c  512 C 24.685356,
-00006f70: 332e 3139 3333 3635 3420 3235 2e31 3237  3.1933654 25.127
-00006f80: 3438 372c 332e 3836 3132 3637 3420 3235  487,3.8612674 25
-00006f90: 2e34 3533 3139 362c 342e 3538 3233 3435  .453196,4.582345
-00006fa0: 2043 2032 352e 3831 3738 3431 2c35 2e33   C 25.817841,5.3
-00006fb0: 3835 3738 3035 2032 362e 3033 3833 3437  857805 26.038347
-00006fc0: 2c36 2e32 3530 3332 3632 2032 362e 3134  ,6.2503262 26.14
-00006fd0: 3037 3139 2c37 2e31 3235 3432 3832 2043  0719,7.1254282 C
-00006fe0: 2032 362e 3230 3134 3538 2c37 2e36 3337   26.201458,7.637
-00006ff0: 3231 3731 2032 362e 3232 3038 3439 2c38  2171 26.220849,8
-00007000: 2e31 3533 3232 3736 2032 362e 3231 3234  .1532276 26.2124
-00007010: 352c 382e 3636 3833 3431 3620 4320 3236  5,8.6683416 C 26
-00007020: 2e32 3031 3732 352c 392e 3430 3639 3639  .201725,9.406969
-00007030: 3620 3236 2e31 3437 3032 332c 3130 2e31  6 26.147023,10.1
-00007040: 3436 3836 3120 3236 2e30 3131 3035 312c  46861 26.011051,
-00007050: 3130 2e38 3733 3635 3120 4320 3235 2e39  10.873651 C 25.9
-00007060: 3537 3838 392c 3131 2e31 3538 3134 3220  57889,11.158142 
-00007070: 3235 2e38 3930 3534 322c 3131 2e34 3339  25.890542,11.439
-00007080: 3937 3220 3235 2e38 3038 3535 362c 3131  972 25.808556,11
-00007090: 2e37 3137 3533 3820 4320 3235 2e36 3838  .717538 C 25.688
-000070a0: 3138 362c 3132 2e31 3337 3931 3720 3235  186,12.137917 25
-000070b0: 2e35 3336 3936 382c 3132 2e35 3438 3639  .536968,12.54869
-000070c0: 3820 3235 2e33 3739 3231 322c 3132 2e39  8 25.379212,12.9
-000070d0: 3536 3236 3120 4320 3235 2e30 3737 3936  56261 C 25.07796
-000070e0: 332c 3133 2e37 3237 3834 3720 3234 2e37  3,13.727847 24.7
-000070f0: 3435 3736 352c 3134 2e34 3836 3930 3820  45765,14.486908 
-00007100: 3234 2e34 3035 3930 382c 3135 2e32 3432  24.405908,15.242
-00007110: 3133 3120 4320 3234 2e32 3438 3631 2c31  131 C 24.24861,1
-00007120: 352e 3539 3138 3733 2032 342e 3038 3736  5.591873 24.0876
-00007130: 3038 2c31 352e 3933 3939 3236 2032 332e  08,15.939926 23.
-00007140: 3932 3639 3539 2c31 362e 3238 3831 3334  926959,16.288134
-00007150: 2043 2032 332e 3537 3339 3332 2c31 372e   C 23.573932,17.
-00007160: 3035 3838 3734 2032 332e 3232 3039 3034  058874 23.220904
-00007170: 2c31 372e 3832 3936 3135 2032 322e 3836  ,17.829615 22.86
-00007180: 3738 3736 2c31 382e 3630 3033 3535 2043  7876,18.600355 C
-00007190: 2032 322e 3237 3838 3132 2c31 392e 3838   22.278812,19.88
-000071a0: 3030 3539 2032 312e 3730 3632 3435 2c32  0059 21.706245,2
-000071b0: 312e 3136 3739 2032 312e 3138 3230 372c  1.1679 21.18207,
-000071c0: 3232 2e34 3735 3733 3120 4320 3230 2e38  22.475731 C 20.8
-000071d0: 3735 3639 332c 3233 2e32 3434 3235 3220  75693,23.244252 
-000071e0: 3230 2e35 3833 3739 362c 3234 2e30 3139  20.583796,24.019
-000071f0: 3339 3620 3230 2e33 3339 3634 392c 3234  396 20.339649,24
-00007200: 2e38 3130 3230 3720 4320 3230 2e32 3035  .810207 C 20.205
-00007210: 3336 312c 3235 2e32 3530 3632 3720 3230  361,25.250627 20
-00007220: 2e30 3833 3338 392c 3235 2e36 3936 3133  .083389,25.69613
-00007230: 3620 3230 2e30 3037 3836 352c 3236 2e31  6 20.007865,26.1
-00007240: 3530 3832 3420 4320 3139 2e39 3730 3138  50824 C 19.97018
-00007250: 362c 3236 2e33 3830 3434 3320 3139 2e39  6,26.380443 19.9
-00007260: 3436 3532 352c 3236 2e36 3133 3232 3220  46525,26.613222 
-00007270: 3139 2e39 3534 3233 312c 3236 2e38 3436  19.954231,26.846
-00007280: 3134 3520 4320 3139 2e39 3633 3837 372c  145 C 19.963877,
-00007290: 3237 2e32 3735 3032 3620 3230 2e30 3337  27.275026 20.037
-000072a0: 3831 372c 3237 2e37 3035 3736 2032 302e  817,27.70576 20.
-000072b0: 3230 3235 3233 2c32 382e 3130 3332 3633  202523,28.103263
-000072c0: 2043 2032 302e 3333 3535 3834 2c32 382e   C 20.335584,28.
-000072d0: 3432 3638 3036 2032 302e 3532 3932 3137  426806 20.529217
-000072e0: 2c32 382e 3732 3439 3320 3230 2e37 3639  ,28.72493 20.769
-000072f0: 3136 382c 3238 2e39 3739 3336 3320 4320  168,28.979363 C 
-00007300: 3231 2e30 3037 3133 312c 3239 2e32 3434  21.007131,29.244
-00007310: 3334 3820 3231 2e32 3936 3438 392c 3239  348 21.296489,29
-00007320: 2e34 3634 3536 3920 3231 2e36 3230 3537  .464569 21.62057
-00007330: 382c 3239 2e36 3133 3338 3420 4320 3231  8,29.613384 C 21
-00007340: 2e39 3636 3631 392c 3239 2e37 3733 3831  .966619,29.77381
-00007350: 3320 3232 2e33 3437 3234 2c32 392e 3835  3 22.34724,29.85
-00007360: 3137 3334 2032 322e 3732 3734 332c 3239  1734 22.72743,29
-00007370: 2e38 3633 3733 3820 4320 3233 2e30 3931  .863738 C 23.091
-00007380: 3032 362c 3239 2e38 3737 3635 3520 3233  026,29.877655 23
-00007390: 2e34 3535 3036 2c32 392e 3832 3235 3033  .45506,29.822503
-000073a0: 2032 332e 3830 3335 3737 2c32 392e 3732   23.803577,29.72
-000073b0: 3033 3433 2043 2032 342e 3331 3035 3333  0343 C 24.310533
-000073c0: 2c32 392e 3537 3137 3720 3234 2e37 3836  ,29.57177 24.786
-000073d0: 3330 332c 3239 2e33 3331 3733 3120 3235  303,29.331731 25
-000073e0: 2e32 3332 3834 372c 3239 2e30 3532 3034  .232847,29.05204
-000073f0: 3420 4320 3235 2e37 3334 3634 382c 3238  4 C 25.734648,28
-00007400: 2e37 3336 3533 3720 3236 2e32 3031 3836  .736537 26.20186
-00007410: 372c 3238 2e33 3638 3737 3920 3236 2e36  7,28.368779 26.6
-00007420: 3435 3535 312c 3237 2e39 3736 3434 3820  45551,27.976448 
-00007430: 4320 3237 2e31 3034 3135 382c 3238 2e34  C 27.104158,28.4
-00007440: 3737 3930 3620 3237 2e35 3632 3736 352c  77906 27.562765,
-00007450: 3238 2e39 3739 3336 3320 3238 2e30 3231  28.979363 28.021
-00007460: 3337 312c 3239 2e34 3830 3832 3120 7a20  371,29.480821 z 
-00007470: 4d20 342e 3734 3930 3237 352c 3139 2e32  M 4.7490275,19.2
-00007480: 3036 3736 3920 4320 342e 3734 3834 3134  06769 C 4.748414
-00007490: 322c 3139 2e37 3535 3035 3220 342e 3833  2,19.755052 4.83
-000074a0: 3336 3534 342c 3230 2e33 3035 3837 3720  36544,20.305877 
-000074b0: 352e 3032 3435 3132 312c 3230 2e38 3230  5.0245121,20.820
-000074c0: 3931 2043 2035 2e32 3032 3138 3431 2c32  91 C 5.2021841,2
-000074d0: 312e 3330 3433 3235 2035 2e34 3732 3537  1.304325 5.47257
-000074e0: 3234 2c32 312e 3735 3231 3338 2035 2e38  24,21.752138 5.8
-000074f0: 3130 3034 3933 2c32 322e 3134 3036 3434  100493,22.140644
-00007500: 2043 2036 2e30 3534 3638 3036 2c32 322e   C 6.0546806,22.
-00007510: 3432 3334 3737 2036 2e33 3334 3735 3332  423477 6.3347532
-00007520: 2c32 322e 3637 3537 3837 2036 2e36 3431  ,22.675787 6.641
-00007530: 3832 3831 2c32 322e 3838 3931 3838 2043  8281,22.889188 C
-00007540: 2037 2e30 3430 3032 3737 2c32 332e 3136   7.0400277,23.16
-00007550: 3539 3431 2037 2e34 3838 3730 3336 2c32  5941 7.4887036,2
-00007560: 332e 3336 3938 3133 2037 2e39 3539 3533  3.369813 7.95953
-00007570: 3031 2c32 332e 3438 3630 3739 2043 2038  01,23.486079 C 8
-00007580: 2e34 3233 3034 3734 2c32 332e 3630 3131  .4230474,23.6011
-00007590: 3531 2038 2e39 3034 3939 3731 2c32 332e  51 8.9049971,23.
-000075a0: 3633 3534 3837 2039 2e33 3830 3936 322c  635487 9.380962,
-000075b0: 3233 2e36 3033 3536 3420 4320 392e 3836  23.603564 C 9.86
-000075c0: 3731 3536 392c 3233 2e35 3730 3330 3820  71569,23.570308 
-000075d0: 3130 2e33 3438 3831 322c 3233 2e34 3534  10.348812,23.454
-000075e0: 3536 3420 3130 2e37 3932 3332 322c 3233  564 10.792322,23
-000075f0: 2e32 3531 3335 2043 2031 312e 3235 3933  .25135 C 11.2593
-00007600: 3039 2c32 332e 3033 3930 3138 2031 312e  09,23.039018 11.
-00007610: 3638 3033 3533 2c32 322e 3733 3239 3031  680353,22.732901
-00007620: 2031 322e 3034 3333 3736 2c32 322e 3337   12.043376,22.37
-00007630: 3137 3331 2043 2031 322e 3431 3537 3438  1731 C 12.415748
-00007640: 2c32 322e 3030 3333 3634 2031 322e 3732  ,22.003364 12.72
-00007650: 3935 3633 2c32 312e 3537 3331 3638 2031  9563,21.573168 1
-00007660: 322e 3934 3931 362c 3231 2e30 3936 3734  2.94916,21.09674
-00007670: 3820 4320 3133 2e31 3636 3133 362c 3230  8 C 13.166136,20
-00007680: 2e36 3239 3435 3520 3133 2e32 3930 3135  .629455 13.29015
-00007690: 342c 3230 2e31 3231 3231 3820 3133 2e33  4,20.121218 13.3
-000076a0: 3238 3036 352c 3139 2e36 3037 3938 3820  28065,19.607988 
-000076b0: 4320 3133 2e33 3539 3131 2c31 392e 3138  C 13.35911,19.18
-000076c0: 3034 3031 2031 332e 3333 3934 3434 2c31  0401 13.339444,1
-000076d0: 382e 3734 3833 3737 2031 332e 3236 3130  8.748377 13.2610
-000076e0: 3833 2c31 382e 3332 3636 3434 2043 2031  83,18.326644 C 1
-000076f0: 332e 3136 3935 3333 2c31 372e 3833 3234  3.169533,17.8324
-00007700: 3339 2031 322e 3939 3036 3432 2c31 372e  39 12.990642,17.
-00007710: 3335 3431 2031 322e 3733 3034 3134 2c31  3541 12.730414,1
-00007720: 362e 3932 3338 3633 2043 2031 322e 3534  6.923863 C 12.54
-00007730: 3637 3035 2c31 362e 3631 3932 3236 2031  6705,16.619226 1
-00007740: 322e 3332 3438 3334 2c31 362e 3333 3739  2.324834,16.3379
-00007750: 3720 3132 2e30 3734 382c 3136 2e30 3835  7 12.0748,16.085
-00007760: 3132 3420 4320 3131 2e37 3037 3530 312c  124 C 11.707501,
-00007770: 3135 2e37 3230 3736 3520 3131 2e32 3830  15.720765 11.280
-00007780: 3631 352c 3135 2e34 3133 3530 3320 3130  615,15.413503 10
-00007790: 2e38 3038 3130 372c 3135 2e32 3030 3734  .808107,15.20074
-000077a0: 2043 2031 302e 3335 3338 3633 2c31 342e   C 10.353863,14.
-000077b0: 3939 3436 3135 2039 2e38 3631 3030 3737  994615 9.8610077
-000077c0: 2c31 342e 3837 3833 3235 2039 2e33 3633  ,14.878325 9.363
-000077d0: 3839 3337 2c31 342e 3834 3439 3439 2043  8937,14.844949 C
-000077e0: 2038 2e38 3139 3031 3138 2c31 342e 3830   8.8190118,14.80
-000077f0: 3830 3636 2038 2e32 3635 3134 3634 2c31  8066 8.2651464,1
-00007800: 342e 3835 3835 3334 2037 2e37 3432 3936  4.858534 7.74296
-00007810: 3739 2c31 352e 3032 3236 3334 2043 2037  79,15.022634 C 7
-00007820: 2e32 3830 3134 3231 2c31 352e 3136 3636  .2801421,15.1666
-00007830: 3820 362e 3834 3637 3032 382c 3135 2e34  8 6.8467028,15.4
-00007840: 3030 3030 3920 362e 3436 3530 3733 372c  00009 6.4650737,
-00007850: 3135 2e36 3938 3231 3320 4320 362e 3035  15.698213 C 6.05
-00007860: 3836 3836 382c 3136 2e30 3135 3332 3920  86868,16.015329 
-00007870: 352e 3730 3338 3136 322c 3136 2e33 3939  5.7038162,16.399
-00007880: 3137 3420 352e 3432 3335 3138 352c 3136  174 5.4235185,16
-00007890: 2e38 3332 3032 3520 4320 352e 3135 3331  .832025 C 5.1531
-000078a0: 3438 392c 3137 2e32 3439 3233 3320 342e  489,17.249233 4.
-000078b0: 3935 3932 3938 322c 3137 2e37 3135 3633  9592982,17.71563
-000078c0: 3120 342e 3835 3339 3632 392c 3138 2e32  1 4.8539629,18.2
-000078d0: 3031 3531 3120 4320 342e 3738 3137 3935  01511 C 4.781795
-000078e0: 332c 3138 2e35 3331 3335 3620 342e 3734  3,18.531356 4.74
-000078f0: 3839 3530 352c 3138 2e38 3639 3238 3820  89505,18.869288 
-00007900: 342e 3734 3930 3237 352c 3139 2e32 3036  4.7490275,19.206
-00007910: 3736 3920 7a20 2720 7374 796c 653d 2766  769 z ' style='f
-00007920: 696c 6c3a 2024 7a6f 6469 6163 5f63 6f6c  ill: $zodiac_col
-00007930: 6f72 5f34 3b27 202f 3e0d 0a20 2020 2020  or_4;' />..     
-00007940: 2020 2020 2020 2020 2020 203c 2f73 796d             </sym
-00007950: 626f 6c3e 0d0a 2020 2020 2020 2020 2020  bol>..          
-00007960: 2020 2020 2020 3c73 796d 626f 6c20 6964        <symbol id
-00007970: 3d27 7669 7267 6f27 3e0d 0a20 2020 2020  ='virgo'>..     
-00007980: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00007990: 7061 7468 2074 7261 6e73 666f 726d 3d22  path transform="
-000079a0: 7363 616c 6528 302e 3829 2220 643d 274d  scale(0.8)" d='M
-000079b0: 2037 2e31 3633 3238 3535 2c39 2e37 3438   7.1632855,9.748
-000079c0: 3833 3633 2043 2037 2e31 3633 3238 3535  8363 C 7.1632855
-000079d0: 2c31 342e 3934 3938 3639 2037 2e31 3633  ,14.949869 7.163
-000079e0: 3238 3535 2c32 302e 3135 3039 3033 2037  2855,20.150903 7
-000079f0: 2e31 3633 3238 3535 2c32 352e 3335 3139  .1632855,25.3519
-00007a00: 3336 2043 2036 2e33 3331 3035 3435 2c32  36 C 6.3310545,2
-00007a10: 352e 3335 3139 3336 2035 2e34 3938 3832  5.351936 5.49882
-00007a20: 3335 2c32 352e 3335 3139 3336 2034 2e36  35,25.351936 4.6
-00007a30: 3636 3539 3235 2c32 352e 3335 3139 3336  665925,25.351936
-00007a40: 2043 2034 2e36 3636 3539 3235 2c31 392e   C 4.6665925,19.
-00007a50: 3332 3831 3634 2034 2e36 3636 3539 3235  328164 4.6665925
-00007a60: 2c31 332e 3330 3433 3932 2034 2e36 3636  ,13.304392 4.666
-00007a70: 3539 3235 2c37 2e32 3830 3631 3938 2043  5925,7.2806198 C
-00007a80: 2034 2e36 3637 3334 3235 2c36 2e31 3035   4.6673425,6.105
-00007a90: 3832 3636 2034 2e35 3133 3738 3235 2c34  8266 4.5137825,4
-00007aa0: 2e39 3238 3932 3837 2034 2e31 3835 3733  .9289287 4.18573
-00007ab0: 3435 2c33 2e37 3939 3838 3220 4320 332e  45,3.799882 C 3.
-00007ac0: 3837 3138 3739 352c 322e 3731 3339 3830  8718795,2.713980
-00007ad0: 3720 332e 3339 3638 3936 352c 312e 3637  7 3.3968965,1.67
-00007ae0: 3537 3630 3620 322e 3738 3934 3134 392c  57606 2.7894149,
-00007af0: 302e 3732 3234 3935 3435 2043 2032 2e37  0.72249545 C 2.7
-00007b00: 3334 3830 3037 2c30 2e36 3334 3436 3537  348007,0.6344657
-00007b10: 2032 2e36 3730 3632 3537 2c30 2e35 3432   2.6706257,0.542
-00007b20: 3635 3931 3920 322e 3631 3931 3239 332c  65919 2.6191293,
-00007b30: 302e 3435 3839 3134 3720 4320 332e 3439  0.4589147 C 3.49
-00007b40: 3632 3138 352c 302e 3435 3839 3134 3720  62185,0.4589147 
-00007b50: 342e 3337 3333 3036 352c 302e 3435 3839  4.3733065,0.4589
-00007b60: 3134 3720 352e 3235 3033 3936 352c 302e  147 5.2503965,0.
-00007b70: 3435 3839 3134 3720 4320 352e 3739 3831  4589147 C 5.7981
-00007b80: 3936 352c 312e 3230 3939 3638 3320 362e  965,1.2099683 6.
-00007b90: 3231 3339 3734 352c 322e 3035 3039 3539  2139745,2.050959
-00007ba0: 3320 362e 3532 3735 3931 352c 322e 3932  3 6.5275915,2.92
-00007bb0: 3430 3037 3320 4320 362e 3831 3431 3637  40073 C 6.814167
-00007bc0: 352c 332e 3732 3230 3834 3820 372e 3031  5,3.7220848 7.01
-00007bd0: 3737 3134 352c 342e 3534 3832 3134 3320  77145,4.5482143 
-00007be0: 372e 3136 3332 3835 352c 352e 3338 3239  7.1632855,5.3829
-00007bf0: 3435 3520 4320 372e 3630 3731 3434 352c  455 C 7.6071445,
-00007c00: 342e 3239 3539 3631 3320 382e 3132 3333  4.2959613 8.1233
-00007c10: 3637 352c 332e 3233 3535 3036 3220 382e  675,3.2355062 8.
-00007c20: 3735 3131 3336 352c 322e 3234 3138 3430  7511365,2.241840
-00007c30: 3520 4320 392e 3134 3933 3936 352c 312e  5 C 9.1493965,1.
-00007c40: 3631 3234 3630 3120 392e 3539 3332 3737  6124601 9.593277
-00007c50: 352c 312e 3031 3034 3538 3320 3130 2e30  5,1.0104583 10.0
-00007c60: 3934 3732 372c 302e 3435 3839 3134 3720  94727,0.4589147 
-00007c70: 4320 3130 2e39 3130 3339 362c 302e 3330  C 10.910396,0.30
-00007c80: 3539 3433 3535 2031 312e 3732 3630 3635  594355 11.726065
-00007c90: 2c30 2e31 3532 3937 3131 3620 3132 2e35  ,0.15297116 12.5
-00007ca0: 3431 3733 342c 342e 3434 3038 3932 3165  41734,4.4408921e
-00007cb0: 2d31 3520 4320 3133 2e31 3135 3432 382c  -15 C 13.115428,
-00007cc0: 302e 3733 3736 3233 3535 2031 332e 3535  0.73762355 13.55
-00007cd0: 3638 3538 2c31 2e35 3732 3038 3933 2031  6858,1.5720893 1
-00007ce0: 332e 3838 3631 3239 2c32 2e34 3434 3637  3.886129,2.44467
-00007cf0: 3039 2043 2031 342e 3237 3135 3935 2c33  09 C 14.271595,3
-00007d00: 2e34 3636 3033 3532 2031 342e 3530 3931  .4660352 14.5091
-00007d10: 362c 342e 3533 3832 3734 3520 3134 2e36  6,4.5382745 14.6
-00007d20: 3531 3531 322c 352e 3631 3839 3439 3220  51512,5.6189492 
-00007d30: 4320 3134 2e36 3536 3338 332c 352e 3635  C 14.656383,5.65
-00007d40: 3630 3239 3520 3134 2e36 3631 3134 312c  60295 14.661141,
-00007d50: 352e 3639 3331 3233 3420 3134 2e36 3635  5.6931234 14.665
-00007d60: 3738 362c 352e 3733 3032 3332 3320 4320  786,5.7302323 C 
-00007d70: 3135 2e30 3338 3839 332c 342e 3535 3438  15.038893,4.5548
-00007d80: 3634 3920 3135 2e35 3930 3537 312c 332e  649 15.590571,3.
-00007d90: 3434 3034 3139 3120 3136 2e32 3538 3132  4404191 16.25812
-00007da0: 322c 322e 3430 3437 3732 3620 4320 3136  2,2.4047726 C 16
-00007db0: 2e36 3936 3633 362c 312e 3732 3431 3237  .696636,1.724127
-00007dc0: 3720 3137 2e31 3835 3030 342c 312e 3037  7 17.185004,1.07
-00007dd0: 3631 3136 3620 3137 2e37 3039 3031 392c  61166 17.709019,
-00007de0: 302e 3435 3839 3134 3720 4320 3138 2e35  0.4589147 C 18.5
-00007df0: 3132 3236 372c 302e 3330 3539 3433 3535  12267,0.30594355
-00007e00: 2031 392e 3331 3535 3134 2c30 2e31 3532   19.315514,0.152
-00007e10: 3937 3131 3620 3230 2e31 3138 3736 322c  97116 20.118762,
-00007e20: 342e 3434 3038 3932 3165 2d31 3520 4320  4.4408921e-15 C 
-00007e30: 3230 2e37 3236 3535 392c 302e 3833 3934  20.726559,0.8394
-00007e40: 3536 3635 2032 312e 3232 3238 3736 2c31  5665 21.222876,1
-00007e50: 2e37 3631 3736 3132 2032 312e 3536 3532  .7617612 21.5652
-00007e60: 3435 2c32 2e37 3430 3431 3534 2043 2032  45,2.7404154 C 2
-00007e70: 312e 3839 3831 3634 2c33 2e36 3837 3230  1.898164,3.68720
-00007e80: 3335 2032 322e 3038 3530 3536 2c34 2e36  35 22.085056,4.6
-00007e90: 3833 3633 3339 2032 322e 3133 3131 3537  836339 22.131157
-00007ea0: 2c35 2e36 3835 3630 3936 2043 2032 322e  ,5.6856096 C 22.
-00007eb0: 3134 3336 3038 2c35 2e39 3237 3033 3620  143608,5.927036 
-00007ec0: 3232 2e31 3433 3639 362c 362e 3136 3837  22.143696,6.1687
-00007ed0: 3837 3320 3232 2e31 3433 3434 342c 362e  873 22.143444,6.
-00007ee0: 3431 3034 3534 3220 4320 3232 2e31 3433  4104542 C 22.143
-00007ef0: 3434 342c 372e 3932 3432 3832 3320 3232  444,7.9242823 22
-00007f00: 2e31 3433 3434 342c 392e 3433 3831 3039  .143444,9.438109
-00007f10: 3220 3232 2e31 3433 3434 342c 3130 2e39  2 22.143444,10.9
-00007f20: 3531 3933 3720 4320 3232 2e34 3831 3334  51937 C 22.48134
-00007f30: 392c 392e 3939 3830 3235 3320 3232 2e38  9,9.9980253 22.8
-00007f40: 3538 3939 322c 392e 3035 3636 3737 3920  58992,9.0566779 
-00007f50: 3233 2e33 3039 3635 392c 382e 3134 3938  23.309659,8.1498
-00007f60: 3635 2043 2032 332e 3539 3633 342c 372e  65 C 23.59634,7.
-00007f70: 3537 3533 3431 2032 332e 3931 3233 3236  575341 23.912326
-00007f80: 2c37 2e30 3133 3937 3739 2032 342e 3237  ,7.0139779 24.27
-00007f90: 3939 3137 2c36 2e34 3836 3832 3134 2043  9917,6.4868214 C
-00007fa0: 2032 342e 3936 3732 3332 2c36 2e32 3334   24.967232,6.234
-00007fb0: 3632 3534 2032 352e 3635 3435 3438 2c35  6254 25.654548,5
-00007fc0: 2e39 3832 3432 3832 2032 362e 3334 3138  .9824282 26.3418
-00007fd0: 3633 2c35 2e37 3330 3233 3233 2043 2032  63,5.7302323 C 2
-00007fe0: 372e 3134 3634 3431 2c36 2e39 3730 3637  7.146441,6.97067
-00007ff0: 3632 2032 372e 3830 3637 3537 2c38 2e33  62 27.806757,8.3
-00008000: 3038 3039 3838 2032 382e 3236 3234 3532  080988 28.262452
-00008010: 2c39 2e37 3135 3434 3735 2043 2032 382e  ,9.7154475 C 28.
-00008020: 3637 3930 3231 2c31 302e 3939 3731 3238  679021,10.997128
-00008030: 2032 382e 3932 3330 3137 2c31 322e 3333   28.923017,12.33
-00008040: 3436 3235 2032 382e 3938 3338 3739 2c31  4625 28.983879,1
-00008050: 332e 3638 3037 3938 2043 2032 392e 3034  3.680798 C 29.04
-00008060: 3939 3936 2c31 352e 3135 3138 3620 3238  9996,15.15186 28
-00008070: 2e39 3133 3737 2c31 362e 3633 3339 3736  .91377,16.633976
-00008080: 2032 382e 3535 3632 3534 2c31 382e 3036   28.556254,18.06
-00008090: 3334 3031 2043 2032 382e 3135 3936 3435  3401 C 28.159645
-000080a0: 2c31 392e 3635 3437 3937 2032 372e 3439  ,19.654797 27.49
-000080b0: 3132 3738 2c32 312e 3137 3536 3620 3236  1278,21.17566 26
-000080c0: 2e36 3038 3734 362c 3232 2e35 3537 3634  .608746,22.55764
-000080d0: 3920 4320 3235 2e37 3936 3539 352c 3233  9 C 25.796595,23
-000080e0: 2e38 3331 3637 3220 3234 2e38 3131 3934  .831672 24.81194
-000080f0: 2c32 342e 3939 3035 3332 2032 332e 3732  ,24.990532 23.72
-00008100: 3930 3533 2c32 362e 3034 3236 3231 2043  9053,26.042621 C
-00008110: 2032 332e 3337 3632 3135 2c32 362e 3338   23.376215,26.38
-00008120: 3534 3338 2032 332e 3031 3236 3738 2c32  5438 23.012678,2
-00008130: 362e 3731 3732 3238 2032 322e 3634 3032  6.717228 22.6402
-00008140: 3938 2c32 372e 3033 3837 3538 2043 2032  98,27.038758 C 2
-00008150: 322e 3733 3039 3036 2c32 372e 3730 3332  2.730906,27.7032
-00008160: 3239 2032 322e 3934 3638 3131 2c32 382e  29 22.946811,28.
-00008170: 3334 3532 3820 3233 2e32 3235 3738 312c  34528 23.225781,
-00008180: 3238 2e39 3533 3335 3420 4320 3233 2e35  28.953354 C 23.5
-00008190: 3733 3039 2c32 392e 3730 3735 3631 2032  7309,29.707561 2
-000081a0: 342e 3031 3636 3931 2c33 302e 3431 3339  4.016691,30.4139
-000081b0: 3938 2032 342e 3530 3336 3139 2c33 312e  98 24.503619,31.
-000081c0: 3038 3534 3836 2043 2032 342e 3733 3032  085486 C 24.7302
-000081d0: 3139 2c33 312e 3339 3734 3037 2032 342e  19,31.397407 24.
-000081e0: 3936 3730 3539 2c33 312e 3730 3138 3438  967059,31.701848
-000081f0: 2032 352e 3231 3135 3139 2c33 312e 3939   25.211519,31.99
-00008200: 3939 3938 2043 2032 342e 3233 3433 3732  9998 C 24.234372
-00008210: 2c33 312e 3939 3939 3938 2032 332e 3235  ,31.999998 23.25
-00008220: 3732 3236 2c33 312e 3939 3939 3938 2032  7226,31.999998 2
-00008230: 322e 3238 3030 3739 2c33 312e 3939 3939  2.280079,31.9999
-00008240: 3938 2043 2032 312e 3831 3537 3136 2c33  98 C 21.815716,3
-00008250: 312e 3431 3332 3138 2032 312e 3433 3233  1.413218 21.4323
-00008260: 3638 2c33 302e 3736 3633 3137 2032 312e  68,30.766317 21.
-00008270: 3130 3033 3435 2c33 302e 3039 3730 3731  100345,30.097071
-00008280: 2043 2032 302e 3833 3337 3436 2c32 392e   C 20.833746,29.
-00008290: 3535 3834 3535 2032 302e 3630 3037 3536  558455 20.600756
-000082a0: 2c32 392e 3030 3336 3733 2032 302e 3339  ,29.003673 20.39
-000082b0: 3230 3332 2c32 382e 3434 3033 3038 2043  2032,28.440308 C
-000082c0: 2031 392e 3339 3634 3232 2c32 392e 3030   19.396422,29.00
-000082d0: 3436 3338 2031 382e 3332 3333 3931 2c32  4638 18.323391,2
-000082e0: 392e 3432 3338 3239 2031 372e 3232 3437  9.423829 17.2247
-000082f0: 3932 2c32 392e 3734 3031 3233 2043 2031  92,29.740123 C 1
-00008300: 362e 3338 3439 3731 2c32 392e 3938 3136  6.384971,29.9816
-00008310: 3038 2031 352e 3532 3836 312c 3330 2e31  08 15.52861,30.1
-00008320: 3633 3338 3520 3134 2e36 3635 3738 362c  63385 14.665786,
-00008330: 3330 2e33 3030 3737 3320 4320 3134 2e36  30.300773 C 14.6
-00008340: 3635 3738 362c 3239 2e35 3839 3636 3220  65786,29.589662 
-00008350: 3134 2e36 3635 3738 362c 3238 2e38 3738  14.665786,28.878
-00008360: 3535 3120 3134 2e36 3635 3738 362c 3238  551 14.665786,28
-00008370: 2e31 3637 3434 2043 2031 352e 3831 3235  .16744 C 15.8125
-00008380: 3032 2c32 372e 3933 3338 3831 2031 362e  02,27.933881 16.
-00008390: 3934 3636 3031 2c32 372e 3632 3534 3236  946601,27.625426
-000083a0: 2031 382e 3033 3635 3639 2c32 372e 3139   18.036569,27.19
-000083b0: 3732 3331 2043 2031 382e 3638 3134 3833  7231 C 18.681483
-000083c0: 2c32 362e 3934 3333 3539 2031 392e 3331  ,26.943359 19.31
-000083d0: 3034 3632 2c32 362e 3634 3637 3833 2031  0462,26.646783 1
-000083e0: 392e 3930 3735 3939 2c32 362e 3239 3435  9.907599,26.2945
-000083f0: 3732 2043 2031 392e 3733 3037 3337 2c32  72 C 19.730737,2
-00008400: 352e 3139 3936 3120 3139 2e36 3433 3233  5.19961 19.64323
-00008410: 322c 3234 2e30 3930 3239 2031 392e 3634  2,24.09029 19.64
-00008420: 3637 3531 2c32 322e 3938 3131 3734 2043  6751,22.981174 C
-00008430: 2031 392e 3634 3637 342c 3137 2e39 3438   19.64674,17.948
-00008440: 3837 3720 3139 2e36 3436 3737 322c 3132  877 19.646772,12
-00008450: 2e39 3136 3537 3820 3139 2e36 3436 3733  .916578 19.64673
-00008460: 352c 372e 3838 3432 3831 3120 4320 3139  5,7.8842811 C 19
-00008470: 2e36 3434 3935 312c 362e 3935 3032 3032  .644951,6.950202
-00008480: 3420 3139 2e35 3937 3032 362c 362e 3031  4 19.597026,6.01
-00008490: 3431 3238 2031 392e 3435 3536 3737 2c35  4128 19.455677,5
-000084a0: 2e30 3839 3939 3636 2043 2031 392e 3334  .0899966 C 19.34
-000084b0: 3835 3232 2c34 2e33 3938 3235 3731 2031  8522,4.3982571 1
-000084c0: 392e 3138 3839 3536 2c33 2e37 3131 3234  9.188956,3.71124
-000084d0: 3720 3138 2e39 3330 3932 342c 332e 3035  7 18.930924,3.05
-000084e0: 3930 3935 3720 4320 3138 2e38 3330 3037  90957 C 18.83007
-000084f0: 362c 322e 3830 3530 3935 3120 3138 2e37  6,2.8050951 18.7
-00008500: 3133 3739 382c 322e 3535 3639 3733 3520  13798,2.5569735 
-00008510: 3138 2e35 3738 3531 342c 322e 3331 3933  18.578514,2.3193
-00008520: 3739 3820 4320 3137 2e37 3338 3937 372c  798 C 17.738977,
-00008530: 332e 3232 3234 3536 3920 3137 2e30 3437  3.2224569 17.047
-00008540: 3935 392c 342e 3235 3538 3334 3820 3136  959,4.2558348 16
-00008550: 2e34 3739 3730 362c 352e 3334 3735 3934  .479706,5.347594
-00008560: 3120 4320 3135 2e38 3234 3432 392c 362e  1 C 15.824429,6.
-00008570: 3630 3734 3837 3420 3135 2e33 3237 3634  6074874 15.32764
-00008580: 372c 372e 3934 3437 3739 3720 3134 2e39  7,7.9447797 14.9
-00008590: 3337 3336 332c 392e 3330 3834 3138 3720  37363,9.3084187 
-000085a0: 4320 3134 2e38 3430 3439 392c 392e 3634  C 14.840499,9.64
-000085b0: 3834 3833 3220 3134 2e37 3439 3034 392c  84832 14.749049,
-000085c0: 392e 3939 3032 3934 3320 3134 2e36 3635  9.9902943 14.665
-000085d0: 3738 362c 3130 2e33 3333 3834 2043 2031  786,10.33384 C 1
-000085e0: 342e 3636 3537 3836 2c31 352e 3333 3938  4.665786,15.3398
-000085f0: 3732 2031 342e 3636 3537 3836 2c32 302e  72 14.665786,20.
-00008600: 3334 3539 3034 2031 342e 3636 3537 3836  345904 14.665786
-00008610: 2c32 352e 3335 3139 3336 2043 2031 332e  ,25.351936 C 13.
-00008620: 3832 3934 3135 2c32 352e 3335 3139 3336  829415,25.351936
-00008630: 2031 322e 3939 3330 3433 2c32 352e 3335   12.993043,25.35
-00008640: 3139 3336 2031 322e 3135 3636 3732 2c32  1936 12.156672,2
-00008650: 352e 3335 3139 3336 2043 2031 322e 3135  5.351936 C 12.15
-00008660: 3636 3631 2c31 392e 3830 3831 3034 2031  6661,19.808104 1
-00008670: 322e 3135 3636 3934 2c31 342e 3236 3432  2.156694,14.2642
-00008680: 3732 2031 322e 3135 3636 3535 2c38 2e37  72 12.156655,8.7
-00008690: 3230 3433 3938 2043 2031 322e 3135 3438  204398 C 12.1548
-000086a0: 3636 2c37 2e36 3935 3936 3336 2031 322e  66,7.6959636 12.
-000086b0: 3131 3630 3635 2c36 2e36 3730 3132 3433  116065,6.6701243
-000086c0: 2031 312e 3939 3735 3233 2c35 2e36 3531   11.997523,5.651
-000086d0: 3938 3131 2043 2031 312e 3931 3631 3631  9811 C 11.916161
-000086e0: 2c34 2e39 3636 3532 3633 2031 312e 3739  ,4.9665263 11.79
-000086f0: 3939 3538 2c34 2e32 3833 3033 3938 2031  9958,4.2830398 1
-00008700: 312e 3630 3636 3131 2c33 2e36 3139 3531  1.606611,3.61951
-00008710: 3336 2043 2031 312e 3437 3336 3433 2c33  36 C 11.473643,3
-00008720: 2e31 3638 3438 3938 2031 312e 3330 3530  .1684898 11.3050
-00008730: 3338 2c32 2e37 3234 3436 3837 2031 312e  38,2.7244687 11.
-00008740: 3036 3335 3932 2c32 2e33 3139 3337 3938  063592,2.3193798
-00008750: 2043 2031 302e 3130 3134 3034 2c33 2e34   C 10.101404,3.4
-00008760: 3338 3036 3939 2039 2e32 3932 3138 3035  380699 9.2921805
-00008770: 2c34 2e36 3834 3236 3339 2038 2e36 3331  ,4.6842639 8.631
-00008780: 3730 3735 2c36 2e30 3032 3220 4320 382e  7075,6.0022 C 8.
-00008790: 3032 3932 3034 352c 372e 3230 3330 3433  0292045,7.203043
-000087a0: 3320 372e 3534 3736 3131 352c 382e 3436  3 7.5476115,8.46
-000087b0: 3233 3732 3220 372e 3136 3332 3835 352c  23722 7.1632855,
-000087c0: 392e 3734 3838 3336 3320 7a20 4d20 3232  9.7488363 z M 22
-000087d0: 2e31 3433 3434 342c 3234 2e37 3036 3937  .143444,24.70697
-000087e0: 3520 4320 3233 2e30 3736 3231 312c 3233  5 C 23.076211,23
-000087f0: 2e37 3630 3437 3220 3233 2e39 3039 3835  .760472 23.90985
-00008800: 392c 3232 2e37 3132 3631 3420 3234 2e35  9,22.712614 24.5
-00008810: 3837 3631 382c 3231 2e35 3638 3833 3820  87618,21.568838 
-00008820: 4320 3234 2e39 3134 3737 312c 3231 2e30  C 24.914771,21.0
-00008830: 3136 3635 3320 3235 2e32 3036 3835 312c  16653 25.206851,
-00008840: 3230 2e34 3433 3432 3920 3235 2e34 3536  20.443429 25.456
-00008850: 3138 392c 3139 2e38 3532 3034 3820 4320  189,19.852048 C 
-00008860: 3235 2e39 3239 3438 392c 3138 2e37 3137  25.929489,18.717
-00008870: 3539 3420 3236 2e32 3434 3831 372c 3137  594 26.244817,17
-00008880: 2e35 3138 3039 3620 3236 2e33 3935 3135  .518096 26.39515
-00008890: 332c 3136 2e32 3938 3437 3620 4320 3236  3,16.298476 C 26
-000088a0: 2e34 3931 3439 322c 3135 2e35 3136 3937  .491492,15.51697
-000088b0: 3120 3236 2e35 3233 3630 332c 3134 2e37  1 26.523603,14.7
-000088c0: 3237 3530 3120 3236 2e34 3930 3930 322c  27501 26.490902,
-000088d0: 3133 2e39 3430 3737 3520 4320 3236 2e34  13.940775 C 26.4
-000088e0: 3430 3939 362c 3132 2e37 3536 3135 3920  40996,12.756159 
-000088f0: 3236 2e32 3331 3232 372c 3131 2e35 3738  26.231227,11.578
-00008900: 3830 3220 3235 2e38 3732 3739 332c 3130  802 25.872793,10
-00008910: 2e34 3438 3537 2043 2032 352e 3638 3630  .44857 C 25.6860
-00008920: 3836 2c39 2e38 3538 3338 3833 2032 352e  86,9.8583883 25.
-00008930: 3435 3938 3034 2c39 2e32 3830 3834 3431  459804,9.2808441
-00008940: 2032 352e 3139 3930 3938 2c38 2e37 3139   25.199098,8.719
-00008950: 3337 3934 2043 2032 342e 3530 3432 3332  3794 C 24.504232
-00008960: 2c39 2e35 3733 3339 3620 3233 2e39 3333  ,9.573396 23.933
-00008970: 3132 362c 3130 2e35 3232 3039 3920 3233  126,10.522099 23
-00008980: 2e34 3438 3939 312c 3131 2e35 3038 3931  .448991,11.50891
-00008990: 3420 4320 3232 2e39 3236 3238 392c 3132  4 C 22.926289,12
-000089a0: 2e35 3736 3234 3520 3232 2e35 3033 3237  .576245 22.50327
-000089b0: 372c 3133 2e36 3839 3935 3720 3232 2e31  7,13.689957 22.1
-000089c0: 3433 3434 342c 3134 2e38 3231 3730 3420  43444,14.821704 
-000089d0: 4320 3232 2e31 3433 3434 342c 3138 2e31  C 22.143444,18.1
-000089e0: 3136 3739 3520 3232 2e31 3433 3434 342c  16795 22.143444,
-000089f0: 3231 2e34 3131 3838 3420 3232 2e31 3433  21.411884 22.143
-00008a00: 3434 342c 3234 2e37 3036 3937 3520 7a20  444,24.706975 z 
-00008a10: 2720 7374 796c 653d 2766 696c 6c3a 2024  ' style='fill: $
-00008a20: 7a6f 6469 6163 5f63 6f6c 6f72 5f35 3b27  zodiac_color_5;'
-00008a30: 202f 3e0d 0a20 2020 2020 2020 2020 2020   />..           
-00008a40: 2020 2020 203c 2f73 796d 626f 6c3e 0d0a       </symbol>..
-00008a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008a60: 3c73 796d 626f 6c20 6964 3d27 6c69 6272  <symbol id='libr
-00008a70: 6127 3e0d 0a20 2020 2020 2020 2020 2020  a'>..           
-00008a80: 2020 2020 2020 2020 203c 7061 7468 2074           <path t
-00008a90: 7261 6e73 666f 726d 3d22 7363 616c 6528  ransform="scale(
-00008aa0: 302e 3829 2220 643d 274d 202d 352e 3539  0.8)" d='M -5.59
-00008ab0: 3632 3565 2d30 362c 3239 2e31 3930 3730  625e-06,29.19070
-00008ac0: 3920 4320 2d35 2e35 3936 3235 652d 3036  9 C -5.59625e-06
-00008ad0: 2c32 382e 3230 3337 3232 202d 352e 3539  ,28.203722 -5.59
-00008ae0: 3632 3565 2d30 362c 3237 2e32 3136 3733  625e-06,27.21673
-00008af0: 3520 2d35 2e35 3936 3235 652d 3036 2c32  5 -5.59625e-06,2
-00008b00: 362e 3232 3937 3335 2043 2031 302e 3636  6.229735 C 10.66
-00008b10: 3636 3637 2c32 362e 3232 3937 3335 2032  6667,26.229735 2
-00008b20: 312e 3333 3333 3237 2c32 362e 3232 3937  1.333327,26.2297
-00008b30: 3335 2033 322c 3236 2e32 3239 3733 3520  35 32,26.229735 
-00008b40: 4320 3332 2c32 372e 3231 3637 3335 2033  C 32,27.216735 3
-00008b50: 322c 3238 2e32 3033 3732 3220 3332 2c32  2,28.203722 32,2
-00008b60: 392e 3139 3037 3039 2043 2032 312e 3333  9.190709 C 21.33
-00008b70: 3333 3237 2c32 392e 3139 3037 3039 2031  3327,29.190709 1
-00008b80: 302e 3636 3636 3637 2c32 392e 3139 3037  0.666667,29.1907
-00008b90: 3039 202d 352e 3539 3632 3565 2d30 362c  09 -5.59625e-06,
-00008ba0: 3239 2e31 3930 3730 3920 7a20 4d20 3132  29.190709 z M 12
-00008bb0: 2e36 3438 3735 2c31 372e 3530 3936 3120  .64875,17.50961 
-00008bc0: 4320 3132 2e36 3438 3735 2c31 382e 3433  C 12.64875,18.43
-00008bd0: 3234 3436 2031 322e 3634 3837 352c 3139  2446 12.64875,19
-00008be0: 2e33 3535 3238 3320 3132 2e36 3438 3735  .355283 12.64875
-00008bf0: 2c32 302e 3237 3831 3333 2043 2038 2e34  ,20.278133 C 8.4
-00008c00: 3332 3530 3233 2c32 302e 3237 3831 3333  325023,20.278133
-00008c10: 2034 2e32 3136 3234 3138 2c32 302e 3237   4.2162418,20.27
-00008c20: 3831 3333 202d 352e 3539 3632 3565 2d30  8133 -5.59625e-0
-00008c30: 362c 3230 2e32 3738 3133 3320 4320 2d35  6,20.278133 C -5
-00008c40: 2e35 3936 3235 652d 3036 2c31 392e 3238  .59625e-06,19.28
-00008c50: 3631 3736 202d 352e 3539 3632 3565 2d30  6176 -5.59625e-0
-00008c60: 362c 3138 2e32 3934 3233 3120 2d35 2e35  6,18.294231 -5.5
-00008c70: 3936 3235 652d 3036 2c31 372e 3330 3232  9625e-06,17.3022
-00008c80: 3836 2043 2032 2e39 3535 3831 372c 3137  86 C 2.955817,17
-00008c90: 2e33 3032 3238 3620 352e 3931 3136 3339  .302286 5.911639
-00008ca0: 362c 3137 2e33 3032 3238 3620 382e 3836  6,17.302286 8.86
-00008cb0: 3734 3632 332c 3137 2e33 3032 3238 3620  74623,17.302286 
-00008cc0: 4320 372e 3833 3330 3031 392c 3136 2e32  C 7.8330019,16.2
-00008cd0: 3538 3331 3920 372e 3031 3231 3234 372c  58319 7.0121247,
-00008ce0: 3134 2e39 3730 3432 3620 362e 3636 3235  14.970426 6.6625
-00008cf0: 3137 312c 3133 2e35 3333 3630 3820 4320  171,13.533608 C 
-00008d00: 362e 3336 3531 3036 342c 3132 2e33 3335  6.3651064,12.335
-00008d10: 3737 3220 362e 3339 3933 3832 392c 3131  772 6.3993829,11
-00008d20: 2e30 3733 3533 3820 362e 3633 3933 3833  .073538 6.639383
-00008d30: 372c 392e 3836 3930 3339 3520 4320 362e  7,9.8690395 C 6.
-00008d40: 3934 3531 3039 352c 382e 3335 3537 3631  9451095,8.355761
-00008d50: 3620 372e 3639 3233 3839 392c 362e 3934  6 7.6923899,6.94
-00008d60: 3834 3239 3320 382e 3731 3739 3837 392c  84293 8.7179879,
-00008d70: 352e 3739 3839 3230 3320 4320 392e 3837  5.7989203 C 9.87
-00008d80: 3234 3638 332c 342e 3439 3232 3736 3220  24683,4.4922762 
-00008d90: 3131 2e33 3435 3434 372c 332e 3433 3933  11.345447,3.4393
-00008da0: 3935 3720 3133 2e30 3136 3635 352c 322e  957 13.016655,2.
-00008db0: 3930 3733 3932 3720 4320 3134 2e35 3139  9073927 C 14.519
-00008dc0: 3930 392c 322e 3432 3531 3631 3320 3136  909,2.4251613 16
-00008dd0: 2e31 3430 3038 312c 322e 3333 3737 3834  .140081,2.337784
-00008de0: 3520 3137 2e36 3935 3237 312c 322e 3538  5 17.695271,2.58
-00008df0: 3934 3636 3120 4320 3139 2e32 3636 3433  94661 C 19.26643
-00008e00: 392c 322e 3834 3532 3732 3620 3230 2e37  9,2.8452726 20.7
-00008e10: 3536 3131 332c 332e 3533 3637 3532 3820  56113,3.5367528 
-00008e20: 3231 2e39 3836 3133 322c 342e 3534 3234  21.986132,4.5424
-00008e30: 3737 3220 4320 3233 2e32 3836 3939 382c  772 C 23.286998,
-00008e40: 352e 3630 3232 3431 3220 3234 2e33 3835  5.6022412 24.385
-00008e50: 3638 342c 362e 3935 3135 3133 3220 3234  684,6.9515132 24
-00008e60: 2e39 3836 3230 312c 382e 3532 3838 3838  .986201,8.528888
-00008e70: 3720 4320 3235 2e34 3633 3036 322c 392e  7 C 25.463062,9.
-00008e80: 3737 3236 3537 3920 3235 2e36 3430 3132  7726579 25.64012
-00008e90: 372c 3131 2e31 3236 3339 3420 3235 2e35  7,11.126394 25.5
-00008ea0: 3333 3535 372c 3132 2e34 3532 3136 3620  33557,12.452166 
-00008eb0: 4320 3235 2e34 3136 3637 382c 3133 2e38  C 25.416678,13.8
-00008ec0: 3230 3334 3420 3234 2e38 3738 3932 372c  20344 24.878927,
-00008ed0: 3135 2e31 3335 3930 3220 3234 2e30 3631  15.135902 24.061
-00008ee0: 3435 322c 3136 2e32 3334 3835 3820 4320  452,16.234858 C 
-00008ef0: 3233 2e37 3833 3630 332c 3136 2e36 3132  23.783603,16.612
-00008f00: 3531 3120 3233 2e34 3736 3131 382c 3136  511 23.476118,16
-00008f10: 2e39 3638 3035 3620 3233 2e31 3437 3335  .968056 23.14735
-00008f20: 2c31 372e 3330 3233 3133 2043 2032 362e  ,17.302313 C 26.
-00008f30: 3039 3832 3333 2c31 372e 3330 3233 2032  098233,17.3023 2
-00008f40: 392e 3034 3931 3136 2c31 372e 3330 3233  9.049116,17.3023
-00008f50: 2033 322c 3137 2e33 3032 3238 3620 4320   32,17.302286 C 
-00008f60: 3332 2c31 382e 3239 3432 3331 2033 322c  32,18.294231 32,
-00008f70: 3139 2e32 3836 3137 3620 3332 2c32 302e  19.286176 32,20.
-00008f80: 3237 3831 3333 2043 2032 372e 3738 3337  278133 C 27.7837
-00008f90: 3339 2c32 302e 3237 3831 3333 2032 332e  39,20.278133 23.
-00008fa0: 3536 3734 3932 2c32 302e 3237 3831 3333  567492,20.278133
-00008fb0: 2031 392e 3335 3132 3434 2c32 302e 3237   19.351244,20.27
-00008fc0: 3831 3333 2043 2031 392e 3335 3132 3434  8133 C 19.351244
-00008fd0: 2c31 392e 3335 3532 3833 2031 392e 3335  ,19.355283 19.35
-00008fe0: 3132 3434 2c31 382e 3433 3234 3436 2031  1244,18.432446 1
-00008ff0: 392e 3335 3132 3434 2c31 372e 3530 3936  9.351244,17.5096
-00009000: 3120 4320 3230 2e34 3736 3437 392c 3136  1 C 20.476479,16
-00009010: 2e37 3837 3139 3920 3231 2e34 3639 3834  .787199 21.46984
-00009020: 362c 3135 2e38 3033 3431 3320 3232 2e30  6,15.803413 22.0
-00009030: 3238 3135 2c31 342e 3537 3533 3337 2043  2815,14.575337 C
-00009040: 2032 322e 3538 3436 3033 2c31 332e 3336   22.584603,13.36
-00009050: 3239 3420 3232 2e37 3036 3839 2c31 312e  294 22.70689,11.
-00009060: 3937 3432 3820 3232 2e34 3639 3237 342c  97428 22.469274,
-00009070: 3130 2e36 3638 3937 3620 4320 3232 2e32  10.668976 C 22.2
-00009080: 3339 3735 322c 392e 3431 3736 3037 3620  39752,9.4176076 
-00009090: 3231 2e35 3734 3631 382c 382e 3237 3133  21.574618,8.2713
-000090a0: 3737 3620 3230 2e36 3731 3435 312c 372e  776 20.671451,7.
-000090b0: 3338 3332 3730 3320 4320 3139 2e37 3531  3832703 C 19.751
-000090c0: 3536 332c 362e 3435 3234 3035 2031 382e  563,6.452405 18.
-000090d0: 3536 3136 322c 352e 3737 3138 3638 2031  56162,5.771868 1
-000090e0: 372e 3236 3539 3431 2c35 2e35 3430 3936  7.265941,5.54096
-000090f0: 3639 2043 2031 352e 3732 3832 3431 2c35  69 C 15.728241,5
-00009100: 2e32 3634 3430 3620 3134 2e30 3735 3338  .264406 14.07538
-00009110: 332c 352e 3438 3634 3139 3820 3132 2e37  3,5.4864198 12.7
-00009120: 3235 3337 2c36 2e32 3935 3336 3120 4320  2537,6.295361 C 
-00009130: 3131 2e38 3233 3533 332c 362e 3833 3536  11.823533,6.8356
-00009140: 3030 3720 3131 2e30 3439 3837 342c 372e  007 11.049874,7.
-00009150: 3538 3438 3535 2031 302e 3435 3835 3435  584855 10.458545
-00009160: 2c38 2e34 3531 3537 3033 2043 2039 2e37  ,8.4515703 C 9.7
-00009170: 3533 3339 3937 2c39 2e34 3837 3431 3739  533997,9.4874179
-00009180: 2039 2e34 3037 3734 3131 2c31 302e 3734   9.4077411,10.74
-00009190: 3637 3839 2039 2e34 3331 3339 3539 2c31  6789 9.4313959,1
-000091a0: 312e 3939 3533 3437 2043 2039 2e34 3336  1.995347 C 9.436
-000091b0: 3637 3432 2c31 332e 3139 3838 3720 392e  6742,13.19887 9.
-000091c0: 3736 3931 3330 342c 3134 2e34 3039 3734  7691304,14.40974
-000091d0: 3420 3130 2e34 3437 3032 342c 3135 2e34  4 10.447024,15.4
-000091e0: 3130 3937 3920 4320 3131 2e30 3134 3231  10979 C 11.01421
-000091f0: 352c 3136 2e32 3632 3435 3720 3131 2e37  5,16.262457 11.7
-00009200: 3932 3736 322c 3136 2e39 3536 3535 3320  92762,16.956553 
-00009210: 3132 2e36 3438 3735 2c31 372e 3530 3936  12.64875,17.5096
-00009220: 3120 7a20 2720 7374 796c 653d 2766 696c  1 z ' style='fil
-00009230: 6c3a 2024 7a6f 6469 6163 5f63 6f6c 6f72  l: $zodiac_color
-00009240: 5f36 3b27 202f 3e0d 0a20 2020 2020 2020  _6;' />..       
-00009250: 2020 2020 2020 2020 203c 2f73 796d 626f           </symbo
-00009260: 6c3e 0d0a 2020 2020 2020 2020 2020 2020  l>..            
-00009270: 2020 2020 3c73 796d 626f 6c20 6964 3d27      <symbol id='
-00009280: 7363 6f72 7069 6f27 3e0d 0a20 2020 2020  scorpio'>..     
-00009290: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-000092a0: 7061 7468 2074 7261 6e73 666f 726d 3d22  path transform="
-000092b0: 7363 616c 6528 302e 3829 2220 643d 274d  scale(0.8)" d='M
-000092c0: 2032 2e30 3731 3737 352c 3235 2e31 3039   2.071775,25.109
-000092d0: 3339 3220 4320 322e 3037 3137 3534 322c  392 C 2.0717542,
-000092e0: 3139 2e32 3433 3339 3220 322e 3037 3138  19.243392 2.0718
-000092f0: 3136 362c 3133 2e33 3737 3339 3220 322e  166,13.377392 2.
-00009300: 3037 3137 3433 322c 372e 3531 3133 3932  0717432,7.511392
-00009310: 3120 4320 322e 3036 3932 3437 352c 362e  1 C 2.0692475,6.
-00009320: 3334 3332 3236 3520 312e 3935 3833 3939  3432265 1.958399
-00009330: 372c 352e 3137 3036 3932 3220 312e 3637  7,5.1706922 1.67
-00009340: 3731 3632 312c 342e 3033 3532 3632 3620  71621,4.0352626 
-00009350: 4320 312e 3433 3733 3139 362c 332e 3036  C 1.4373196,3.06
-00009360: 3632 3537 3520 312e 3036 3835 3934 2c32  62575 1.068594,2
-00009370: 2e31 3235 3134 3335 2030 2e35 3435 3338  .1251435 0.54538
-00009380: 3034 382c 312e 3237 3336 3937 3120 4320  048,1.2736971 C 
-00009390: 302e 3337 3935 3732 3038 2c31 2e30 3033  0.37957208,1.003
-000093a0: 3530 3632 2030 2e31 3938 3636 3435 382c  5062 0.19866458,
-000093b0: 302e 3734 3235 3934 2030 2e30 3033 3233  0.742594 0.00323
-000093c0: 3933 3736 342c 302e 3439 3330 3635 3120  93764,0.4930651 
-000093d0: 4320 302e 3838 3435 3038 3938 2c30 2e34  C 0.88450898,0.4
-000093e0: 3933 3036 3531 2031 2e37 3635 3737 3836  930651 1.7657786
-000093f0: 2c30 2e34 3933 3036 3531 2032 2e36 3437  ,0.4930651 2.647
-00009400: 3034 3833 2c30 2e34 3933 3036 3531 2043  0483,0.4930651 C
-00009410: 2033 2e32 3334 3035 3333 2c31 2e33 3839   3.2340533,1.389
-00009420: 3439 3331 2033 2e36 3938 3333 3233 2c32  4931 3.6983323,2
-00009430: 2e33 3635 3139 3031 2034 2e30 3335 3632  .3651901 4.03562
-00009440: 3733 2c33 2e33 3832 3334 3234 2043 2034  73,3.3823424 C 4
-00009450: 2e32 3437 3936 3133 2c34 2e30 3231 3033  .2479613,4.02103
-00009460: 3733 2034 2e34 3131 3438 3133 2c34 2e36  73 4.4114813,4.6
-00009470: 3735 3636 3620 342e 3533 3139 3836 332c  75666 4.5319863,
-00009480: 352e 3333 3738 3333 2043 2035 2e30 3438  5.337833 C 5.048
-00009490: 3531 3933 2c34 2e30 3630 3139 3738 2035  5193,4.0601978 5
-000094a0: 2e36 3834 3634 3933 2c32 2e38 3236 3833  .6846493,2.82683
-000094b0: 3839 2036 2e34 3736 3731 3733 2c31 2e36  89 6.4767173,1.6
-000094c0: 3937 3936 3520 4320 362e 3736 3939 3339  97965 C 6.769939
-000094d0: 332c 312e 3238 3031 3036 3920 372e 3038  3,1.2801069 7.08
-000094e0: 3433 3633 332c 302e 3837 3730 3638 3820  43633,0.8770688 
-000094f0: 372e 3432 3035 3932 332c 302e 3439 3330  7.4205923,0.4930
-00009500: 3635 3120 4320 382e 3231 3231 3033 332c  651 C 8.2121033,
-00009510: 302e 3333 3336 3137 3120 392e 3030 3336  0.3336171 9.0036
-00009520: 3133 332c 302e 3137 3431 3639 2039 2e37  133,0.174169 9.7
-00009530: 3935 3132 3433 2c30 2e30 3134 3732 3130  951243,0.0147210
-00009540: 3033 2043 2031 302e 3332 3138 2c30 2e36  03 C 10.3218,0.6
-00009550: 3239 3035 3834 2031 302e 3732 3739 372c  290584 10.72797,
-00009560: 312e 3334 3030 3030 3520 3131 2e30 3337  1.3400005 11.037
-00009570: 3731 342c 322e 3038 3631 3538 3520 4320  714,2.0861585 C 
-00009580: 3131 2e34 3031 3335 382c 322e 3936 3239  11.401358,2.9629
-00009590: 3235 3320 3131 2e36 3338 3033 392c 332e  253 11.638039,3.
-000095a0: 3838 3830 3031 3220 3131 2e37 3938 3132  8880012 11.79812
-000095b0: 352c 342e 3832 3233 3935 2043 2031 312e  5,4.822395 C 11.
-000095c0: 3834 3139 3732 2c35 2e30 3739 3137 3633  841972,5.0791763
-000095d0: 2031 312e 3837 3938 3837 2c35 2e33 3336   11.879887,5.336
-000095e0: 3936 3538 2031 312e 3931 3236 3139 2c35  9658 11.912619,5
-000095f0: 2e35 3935 3430 3239 2043 2031 322e 3334  .5954029 C 12.34
-00009600: 3038 3231 2c34 2e33 3630 3233 3938 2031  0821,4.3602398 1
-00009610: 322e 3935 3035 342c 332e 3139 3239 3637  2.95054,3.192967
-00009620: 3220 3133 2e36 3734 3534 332c 322e 3130  2 13.674543,2.10
-00009630: 3639 3030 3220 4320 3134 2e30 3436 3534  69002 C 14.04654
-00009640: 2c31 2e35 3438 3733 3736 2031 342e 3434  ,1.5487376 14.44
-00009650: 3839 3137 2c31 2e30 3131 3133 3736 2031  8917,1.0111376 1
-00009660: 342e 3837 3436 3634 2c30 2e34 3933 3036  4.874664,0.49306
-00009670: 3531 2043 2031 352e 3638 3234 3935 2c30  51 C 15.682495,0
-00009680: 2e33 3333 3631 3731 2031 362e 3439 3033  .3336171 16.4903
-00009690: 3235 2c30 2e31 3734 3136 3920 3137 2e32  25,0.174169 17.2
-000096a0: 3938 3135 362c 302e 3031 3437 3231 3030  98156,0.01472100
-000096b0: 3320 4320 3137 2e38 3831 3130 372c 302e  3 C 17.881107,0.
-000096c0: 3830 3238 3632 3920 3138 2e33 3436 3437  8028629 18.34647
-000096d0: 322c 312e 3637 3833 3335 3720 3138 2e36  2,1.6783357 18.6
-000096e0: 3730 3933 2c32 2e36 3034 3032 3734 2043  7093,2.6040274 C
-000096f0: 2031 392e 3032 3735 342c 332e 3631 3633   19.02754,3.6163
-00009700: 3635 3520 3139 2e32 3136 3233 382c 342e  655 19.216238,4.
-00009710: 3638 3431 3135 3620 3139 2e32 3636 3336  6841156 19.26636
-00009720: 392c 352e 3735 3532 3838 3820 4320 3139  9,5.7552888 C 19
-00009730: 2e32 3830 3034 2c36 2e30 3232 3135 3231  .28004,6.0221521
-00009740: 2031 392e 3238 3134 3434 2c36 2e32 3839   19.281444,6.289
-00009750: 3337 3733 2031 392e 3238 3130 3132 2c36  3773 19.281012,6
-00009760: 2e35 3536 3532 3339 2043 2031 392e 3238  .5565239 C 19.28
-00009770: 3130 3239 2c31 312e 3632 3730 3831 2031  1029,11.627081 1
-00009780: 392e 3238 3039 3739 2c31 362e 3639 3736  9.280979,16.6976
-00009790: 3339 2031 392e 3238 3130 3338 2c32 312e  39 19.281038,21.
-000097a0: 3736 3831 3937 2043 2031 392e 3238 3233  768197 C 19.2823
-000097b0: 3737 2c32 322e 3438 3537 3438 2031 392e  77,22.485748 19.
-000097c0: 3239 3236 3939 2c32 332e 3230 3336 3339  292699,23.203639
-000097d0: 2031 392e 3333 3430 3333 2c32 332e 3932   19.334033,23.92
-000097e0: 3031 3235 2043 2031 392e 3335 3432 3937  0125 C 19.354297
-000097f0: 2c32 342e 3234 3936 3333 2031 392e 3337  ,24.249633 19.37
-00009800: 3838 3331 2c32 342e 3537 3934 3238 2031  8831,24.579428 1
-00009810: 392e 3432 3838 3236 2c32 342e 3930 3539  9.428826,24.9059
-00009820: 3433 2043 2031 392e 3434 3434 3931 2c32  43 C 19.444491,2
-00009830: 352e 3031 3230 3535 2031 392e 3437 3232  5.012055 19.4722
-00009840: 3738 2c32 352e 3131 3539 3134 2031 392e  78,25.115914 19.
-00009850: 3530 3039 3437 2c32 352e 3231 3931 3220  500947,25.21912 
-00009860: 4320 3139 2e35 3939 3838 342c 3235 2e35  C 19.599884,25.5
-00009870: 3636 3932 3620 3139 2e37 3537 3631 352c  66926 19.757615,
-00009880: 3235 2e38 3938 3431 3820 3139 2e39 3730  25.898418 19.970
-00009890: 3532 2c32 362e 3139 3037 3631 2043 2032  52,26.190761 C 2
-000098a0: 302e 3035 3333 3831 2c32 362e 3330 3430  0.053381,26.3040
-000098b0: 3032 2032 302e 3134 3230 3639 2c32 362e  02 20.142069,26.
-000098c0: 3431 3333 3931 2032 302e 3234 3034 3237  413391 20.240427
-000098d0: 2c32 362e 3531 3335 3332 2043 2032 302e  ,26.513532 C 20.
-000098e0: 3533 3737 3331 2c32 362e 3831 3337 3338  537731,26.813738
-000098f0: 2032 302e 3930 3637 3931 2c32 372e 3033   20.906791,27.03
-00009900: 3531 3939 2032 312e 3239 3735 3333 2c32  5199 21.297533,2
-00009910: 372e 3139 3036 3520 4320 3231 2e37 3833  7.19065 C 21.783
-00009920: 3732 372c 3237 2e33 3833 3939 3720 3232  727,27.383997 22
-00009930: 2e33 3032 3132 312c 3237 2e34 3833 3638  .302121,27.48368
-00009940: 3220 3232 2e38 3231 3234 362c 3237 2e35  2 22.821246,27.5
-00009950: 3334 3236 3220 4320 3233 2e31 3436 3032  34262 C 23.14602
-00009960: 322c 3237 2e35 3636 3030 3920 3233 2e34  2,27.566009 23.4
-00009970: 3732 3437 352c 3237 2e35 3736 3030 3820  72475,27.576008 
-00009980: 3233 2e37 3938 3637 322c 3237 2e35 3734  23.798672,27.574
-00009990: 3730 3420 4320 3234 2e32 3731 3536 312c  704 C 24.271561,
-000099a0: 3237 2e35 3734 3730 3420 3234 2e37 3434  27.574704 24.744
-000099b0: 3435 322c 3237 2e35 3734 3730 3420 3235  452,27.574704 25
-000099c0: 2e32 3137 3334 322c 3237 2e35 3734 3730  .217342,27.57470
-000099d0: 3420 4320 3235 2e32 3137 3334 322c 3236  4 C 25.217342,26
-000099e0: 2e37 3532 3933 3320 3235 2e32 3137 3334  .752933 25.21734
-000099f0: 322c 3235 2e39 3331 3136 3320 3235 2e32  2,25.931163 25.2
-00009a00: 3137 3334 322c 3235 2e31 3039 3339 3220  17342,25.109392 
-00009a10: 4320 3236 2e35 3134 3736 372c 3236 2e32  C 26.514767,26.2
-00009a20: 3832 3736 3620 3237 2e38 3132 3139 322c  82766 27.812192,
-00009a30: 3237 2e34 3536 3134 2032 392e 3130 3936  27.45614 29.1096
-00009a40: 3137 2c32 382e 3632 3935 3134 2043 2032  17,28.629514 C 2
-00009a50: 372e 3831 3231 3932 2c32 392e 3735 3739  7.812192,29.7579
-00009a60: 3136 2032 362e 3531 3437 3637 2c33 302e  16 26.514767,30.
-00009a70: 3838 3633 3137 2032 352e 3231 3733 3432  886317 25.217342
-00009a80: 2c33 322e 3031 3437 3139 2043 2032 352e  ,32.014719 C 25.
-00009a90: 3231 3733 3432 2c33 312e 3231 3734 3739  217342,31.217479
-00009aa0: 2032 352e 3231 3733 3432 2c33 302e 3432   25.217342,30.42
-00009ab0: 3032 3339 2032 352e 3231 3733 3432 2c32  0239 25.217342,2
-00009ac0: 392e 3632 3239 3938 2043 2032 342e 3434  9.622998 C 24.44
-00009ad0: 3938 3339 2c32 392e 3632 3239 3331 2032  9839,29.622931 2
-00009ae0: 332e 3638 3233 3334 2c32 392e 3632 3331  3.682334,29.6231
-00009af0: 3334 2032 322e 3931 3438 332c 3239 2e36  34 22.91483,29.6
-00009b00: 3232 3839 3520 4320 3232 2e31 3735 3234  22895 C 22.17524
-00009b10: 372c 3239 2e36 3139 3238 3220 3231 2e34  7,29.619282 21.4
-00009b20: 3331 3838 392c 3239 2e35 3531 3335 2032  31889,29.55135 2
-00009b30: 302e 3731 3435 3534 2c32 392e 3336 3437  0.714554,29.3647
-00009b40: 3238 2043 2032 302e 3132 3437 3934 2c32  28 C 20.124794,2
-00009b50: 392e 3231 3130 3833 2031 392e 3535 3234  9.211083 19.5524
-00009b60: 3332 2c32 382e 3937 3230 3933 2031 392e  32,28.972093 19.
-00009b70: 3035 3139 3037 2c32 382e 3632 3036 3736  051907,28.620676
-00009b80: 2043 2031 382e 3638 3735 3531 2c32 382e   C 18.687551,28.
-00009b90: 3336 3632 3537 2031 382e 3336 3535 3433  366257 18.365543
-00009ba0: 2c32 382e 3035 3137 3336 2031 382e 3130  ,28.051736 18.10
-00009bb0: 3039 3839 2c32 372e 3639 3433 3834 2043  0989,27.694384 C
-00009bc0: 2031 372e 3732 3533 3138 2c32 372e 3138   17.725318,27.18
-00009bd0: 3934 3636 2031 372e 3436 3031 352c 3236  9466 17.46015,26
-00009be0: 2e36 3039 3435 2031 372e 3237 3237 3134  .60945 17.272714
-00009bf0: 2c32 362e 3031 3033 3438 2043 2031 372e  ,26.010348 C 17.
-00009c00: 3034 3338 3236 2c32 352e 3237 3632 3636  043826,25.276266
-00009c10: 2031 362e 3932 3534 3238 2c32 342e 3531   16.925428,24.51
-00009c20: 3138 2031 362e 3836 3631 3835 2c32 332e  18 16.866185,23.
-00009c30: 3734 3633 3634 2043 2031 362e 3833 3132  746364 C 16.8312
-00009c40: 3131 2c32 332e 3239 3534 3134 2031 362e  11,23.295414 16.
-00009c50: 3831 3934 3739 2c32 322e 3834 3320 3136  819479,22.843 16
-00009c60: 2e38 3230 3830 312c 3232 2e33 3930 3738  .820801,22.39078
-00009c70: 3520 4320 3136 2e38 3230 3739 2c31 372e  5 C 16.82079,17.
-00009c80: 3437 3335 3033 2031 362e 3832 3038 3233  473503 16.820823
-00009c90: 2c31 322e 3535 3632 3231 2031 362e 3832  ,12.556221 16.82
-00009ca0: 3037 3835 2c37 2e36 3338 3933 3832 2043  0785,7.6389382 C
-00009cb0: 2031 362e 3831 3839 3936 2c36 2e37 3632   16.818996,6.762
-00009cc0: 3231 3932 2031 362e 3737 3735 3933 2c35  2192 16.777593,5
-00009cd0: 2e38 3833 3635 3932 2031 362e 3635 3039  .8836592 16.6509
-00009ce0: 3737 2c35 2e30 3135 3435 3233 2043 2031  77,5.0154523 C 1
-00009cf0: 362e 3535 3934 372c 342e 3339 3833 3331  6.55947,4.398331
-00009d00: 3920 3136 2e34 3235 3434 342c 332e 3738  9 16.425444,3.78
-00009d10: 3434 3132 3720 3136 2e32 3033 3934 332c  44127 16.203943,
-00009d20: 332e 3230 3031 3033 3120 4320 3136 2e30  3.2001031 C 16.0
-00009d30: 3831 3939 362c 322e 3838 3032 3230 3820  81996,2.8802208 
-00009d40: 3135 2e39 3332 3633 322c 322e 3536 3936  15.932632,2.5696
-00009d50: 3230 3920 3135 2e37 3433 3639 342c 322e  209 15.743694,2.
-00009d60: 3238 3337 3839 3420 4320 3134 2e38 3135  2837894 C 14.815
-00009d70: 3331 352c 332e 3335 3534 3935 2031 342e  315,3.355495 14.
-00009d80: 3033 3835 3839 2c34 2e35 3536 3331 3138  038589,4.5563118
-00009d90: 2031 332e 3432 3038 3936 2c35 2e38 3332   13.420896,5.832
-00009da0: 3634 3639 2043 2031 322e 3734 3132 3339  6469 C 12.741239
-00009db0: 2c37 2e32 3334 3834 3738 2031 322e 3235  ,7.2348478 12.25
-00009dc0: 3032 3234 2c38 2e37 3234 3636 3320 3131  0224,8.724663 11
-00009dd0: 2e39 3132 3631 392c 3130 2e32 3434 3938  .912619,10.24498
-00009de0: 3820 4320 3131 2e39 3132 3631 392c 3135  8 C 11.912619,15
-00009df0: 2e31 3939 3739 2031 312e 3931 3236 3139  .19979 11.912619
-00009e00: 2c32 302e 3135 3435 3920 3131 2e39 3132  ,20.15459 11.912
-00009e10: 3631 392c 3235 2e31 3039 3339 3220 4320  619,25.109392 C 
-00009e20: 3131 2e30 3932 3534 392c 3235 2e31 3039  11.092549,25.109
-00009e30: 3339 3220 3130 2e32 3732 3437 382c 3235  392 10.272478,25
-00009e40: 2e31 3039 3339 3220 392e 3435 3234 3038  .109392 9.452408
-00009e50: 332c 3235 2e31 3039 3339 3220 4320 392e  3,25.109392 C 9.
-00009e60: 3435 3233 3937 332c 3139 2e35 3734 3331  4523973,19.57431
-00009e70: 3920 392e 3435 3234 3330 332c 3134 2e30  9 9.4524303,14.0
-00009e80: 3339 3234 3620 392e 3435 3233 3932 332c  39246 9.4523923,
-00009e90: 382e 3530 3431 3733 3320 4320 392e 3435  8.5041733 C 9.45
-00009ea0: 3036 3134 332c 372e 3530 3434 3038 3220  06143,7.5044082 
-00009eb0: 392e 3431 3330 3134 332c 362e 3530 3332  9.4130143,6.5032
-00009ec0: 3131 3820 392e 3239 3536 3639 332c 352e  118 9.2956693,5.
-00009ed0: 3530 3938 3239 3620 4320 392e 3231 3437  5098296 C 9.2147
-00009ee0: 3532 332c 342e 3833 3832 3237 2039 2e30  523,4.838227 9.0
-00009ef0: 3938 3630 3433 2c34 2e31 3638 3536 3835  986043,4.1685685
-00009f00: 2038 2e39 3033 3738 3833 2c33 2e35 3139   8.9037883,3.519
-00009f10: 3938 3136 2043 2038 2e37 3733 3433 3233  9816 C 8.7734323
-00009f20: 2c33 2e30 3930 3530 3833 2038 2e36 3038  ,3.0905083 8.608
-00009f30: 3033 3733 2c32 2e36 3638 3633 3720 382e  0373,2.668637 8.
-00009f40: 3337 3533 3031 332c 322e 3238 3337 3839  3753013,2.283789
-00009f50: 3420 4320 372e 3433 3335 3434 332c 332e  4 C 7.4335443,3.
-00009f60: 3334 3433 3739 2036 2e36 3434 3034 3033  344379 6.6440403
-00009f70: 2c34 2e35 3336 3932 3931 2036 2e30 3036  ,4.5369291 6.006
-00009f80: 3438 3033 2c35 2e38 3033 3639 3336 2043  4803,5.8036936 C
-00009f90: 2035 2e33 3831 3534 3833 2c37 2e30 3434   5.3815483,7.044
-00009fa0: 3134 3036 2034 2e38 3938 3730 3533 2c38  1406 4.8987053,8
-00009fb0: 2e33 3533 3839 3120 342e 3533 3139 3836  .353891 4.531986
-00009fc0: 332c 392e 3639 3330 3532 3320 4320 342e  3,9.6930523 C 4.
-00009fd0: 3533 3139 3836 332c 3134 2e38 3331 3833  5319863,14.83183
-00009fe0: 3320 342e 3533 3139 3836 332c 3139 2e39  3 4.5319863,19.9
-00009ff0: 3730 3631 3220 342e 3533 3139 3836 332c  70612 4.5319863,
-0000a000: 3235 2e31 3039 3339 3220 4320 332e 3731  25.109392 C 3.71
-0000a010: 3139 3135 332c 3235 2e31 3039 3339 3220  19153,25.109392 
-0000a020: 322e 3839 3138 3435 342c 3235 2e31 3039  2.8918454,25.109
-0000a030: 3339 3220 322e 3037 3137 3735 2c32 352e  392 2.071775,25.
-0000a040: 3130 3933 3932 207a 2720 7374 796c 653d  109392 z' style=
-0000a050: 2766 696c 6c3a 2024 7a6f 6469 6163 5f63  'fill: $zodiac_c
-0000a060: 6f6c 6f72 5f37 3b27 202f 3e0d 0a20 2020  olor_7;' />..   
-0000a070: 2020 2020 2020 2020 2020 2020 203c 2f73               </s
-0000a080: 796d 626f 6c3e 0d0a 2020 2020 2020 2020  ymbol>..        
-0000a090: 2020 2020 2020 2020 3c73 796d 626f 6c20          <symbol 
-0000a0a0: 6964 3d27 7361 6769 7474 6172 6975 7327  id='sagittarius'
-0000a0b0: 3e0d 0a20 2020 2020 2020 2020 2020 2020  >..             
-0000a0c0: 2020 2020 2020 203c 7061 7468 2074 7261         <path tra
-0000a0d0: 6e73 666f 726d 3d22 7363 616c 6528 302e  nsform="scale(0.
-0000a0e0: 3829 2220 643d 274d 2032 392e 3839 3239  8)" d='M 29.8929
-0000a0f0: 3432 2c32 2e30 3935 3837 3036 204c 2033  42,2.0958706 L 3
-0000a100: 322c 3137 2e31 3136 3237 3620 4c20 3238  2,17.116276 L 28
-0000a110: 2e39 3938 3537 392c 3137 2e35 3837 3038  .998579,17.58708
-0000a120: 3820 4c20 3237 2e34 3532 3339 332c 362e  8 L 27.452393,6.
-0000a130: 3633 3639 3233 3520 4c20 3133 2e37 3333  6369235 L 13.733
-0000a140: 3737 362c 3230 2e34 3131 3935 3720 4c20  776,20.411957 L 
-0000a150: 3230 2e31 3931 3337 392c 3236 2e38 3636  20.191379,26.866
-0000a160: 3633 204c 2031 382e 3033 3838 3435 2c32  63 L 18.038845,2
-0000a170: 392e 3032 3332 3531 204c 2031 312e 3538  9.023251 L 11.58
-0000a180: 3132 3432 2c32 322e 3535 3333 3920 4c20  1242,22.55339 L 
-0000a190: 322e 3039 3139 3031 2c33 312e 3939 3939  2.091901,31.9999
-0000a1a0: 3935 204c 2031 2e35 652d 3036 2c32 392e  95 L 1.5e-06,29.
-0000a1b0: 3930 3431 3234 204c 2039 2e34 3734 3138  904124 L 9.47418
-0000a1c0: 342c 3230 2e34 3432 3333 3220 4c20 332e  4,20.442332 L 3.
-0000a1d0: 3033 3137 342c 3133 2e39 3732 3437 204c  03174,13.97247 L
-0000a1e0: 2035 2e31 3533 3935 372c 3131 2e38 3135   5.153957,11.815
-0000a1f0: 3835 204c 2031 312e 3631 3135 362c 3138  85 L 11.61156,18
-0000a200: 2e32 3835 3731 3120 4c20 3235 2e33 3630  .285711 L 25.360
-0000a210: 3439 332c 342e 3534 3130 3532 3920 4c20  493,4.5410529 L 
-0000a220: 3134 2e34 3331 3037 362c 332e 3030 3731  14.431076,3.0071
-0000a230: 3138 3620 4c20 3134 2e39 3030 3939 362c  186 L 14.900996,
-0000a240: 2d34 2e34 3430 3839 3231 652d 3136 204c  -4.4408921e-16 L
-0000a250: 2032 392e 3839 3239 3432 2c32 2e30 3935   29.892942,2.095
-0000a260: 3837 3036 207a 2027 2073 7479 6c65 3d27  8706 z ' style='
-0000a270: 6669 6c6c 3a20 247a 6f64 6961 635f 636f  fill: $zodiac_co
-0000a280: 6c6f 725f 383b 2720 2f3e 0d0a 2020 2020  lor_8;' />..    
-0000a290: 2020 2020 2020 2020 2020 2020 3c2f 7379              </sy
-0000a2a0: 6d62 6f6c 3e0d 0a20 2020 2020 2020 2020  mbol>..         
-0000a2b0: 2020 2020 2020 203c 7379 6d62 6f6c 2069         <symbol i
-0000a2c0: 643d 2763 6170 7269 636f 726e 273e 0d0a  d='capricorn'>..
-0000a2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a2e0: 2020 2020 3c70 6174 6820 7472 616e 7366      <path transf
-0000a2f0: 6f72 6d3d 2273 6361 6c65 2830 2e38 2922  orm="scale(0.8)"
-0000a300: 2064 3d27 4d20 362e 3130 3933 3535 392c   d='M 6.1093559,
-0000a310: 3138 2e39 3034 3737 3420 4320 362e 3130  18.904774 C 6.10
-0000a320: 3932 3339 322c 3138 2e35 3839 3535 2036  92392,18.58955 6
-0000a330: 2e31 3039 3630 3432 2c31 382e 3237 3433  .1096042,18.2743
-0000a340: 3235 2036 2e31 3039 3134 3733 2c31 372e  25 6.1091473,17.
-0000a350: 3935 3931 3033 2043 2036 2e31 3033 3633  959103 C 6.10363
-0000a360: 3839 2c31 372e 3134 3632 3334 2036 2e30  89,17.146234 6.0
-0000a370: 3336 3435 3837 2c31 362e 3333 3530 3635  364587,16.335065
-0000a380: 2035 2e39 3436 3339 3638 2c31 352e 3532   5.9463968,15.52
-0000a390: 3736 3131 2043 2035 2e38 3032 3031 3933  7611 C 5.8020193
-0000a3a0: 2c31 342e 3235 3436 3432 2035 2e35 3936  ,14.254642 5.596
-0000a3b0: 3039 3433 2c31 322e 3938 3934 3635 2035  0943,12.989465 5
-0000a3c0: 2e33 3636 3533 3133 2c31 312e 3732 3933  .3665313,11.7293
-0000a3d0: 3338 2043 2035 2e32 3235 3836 3034 2c31  38 C 5.2258604,1
-0000a3e0: 302e 3935 3639 3237 2035 2e30 3730 3434  0.956927 5.07044
-0000a3f0: 2c31 302e 3138 3732 3220 342e 3930 3335  ,10.18722 4.9035
-0000a400: 3537 2c39 2e34 3230 3035 3437 2043 2034  57,9.4200547 C 4
-0000a410: 2e37 3231 3830 3237 2c38 2e35 3933 3130  .7218027,8.59310
-0000a420: 3532 2034 2e35 3236 3233 3839 2c37 2e37  52 4.5262389,7.7
-0000a430: 3638 3439 3037 2034 2e32 3835 3333 3336  684907 4.2853336
-0000a440: 2c36 2e39 3536 3532 3437 2043 2034 2e31  ,6.9565247 C 4.1
-0000a450: 3533 3230 3336 2c36 2e35 3136 3935 3534  532036,6.5169554
-0000a460: 2034 2e30 3039 3931 3339 2c36 2e30 3739   4.0099139,6.079
-0000a470: 3533 2033 2e38 3235 3133 3334 2c35 2e36  53 3.8251334,5.6
-0000a480: 3538 3838 3536 2043 2033 2e36 3538 3932  588856 C 3.65892
-0000a490: 3334 2c35 2e32 3833 3631 3531 2033 2e34  34,5.2836151 3.4
-0000a4a0: 3437 3231 3638 2c34 2e39 3236 3935 3239  472168,4.9269529
-0000a4b0: 2033 2e31 3834 3334 3939 2c34 2e36 3131   3.1843499,4.611
-0000a4c0: 3038 3838 2043 2032 2e39 3030 3932 3039  0888 C 2.9009209
-0000a4d0: 2c34 2e32 3730 3039 3239 2032 2e35 3531  ,4.2700929 2.551
-0000a4e0: 3435 3238 2c33 2e39 3832 3030 3131 2032  4528,3.9820011 2
-0000a4f0: 2e31 3534 3638 3531 2c33 2e37 3832 3336  .1546851,3.78236
-0000a500: 3431 2043 2031 2e37 3237 3238 3436 2c33  41 C 1.7272846,3
-0000a510: 2e35 3635 3232 3631 2031 2e32 3531 3938  .5652261 1.25198
-0000a520: 3437 2c33 2e34 3532 3537 3137 2030 2e37  47,3.4525717 0.7
-0000a530: 3734 3938 3437 382c 332e 3432 3230 3438  7498478,3.422048
-0000a540: 3620 4320 302e 3538 3730 3136 3737 2c33  6 C 0.58701677,3
-0000a550: 2e34 3038 3937 3036 2030 2e33 3938 3539  .4089706 0.39859
-0000a560: 3637 352c 332e 3431 3239 3732 3820 302e  675,3.4129728 0.
-0000a570: 3231 3033 3431 392c 332e 3431 3232 3935  2103419,3.412295
-0000a580: 2043 2030 2e31 3430 3230 3339 312c 332e   C 0.14020391,3.
-0000a590: 3431 3232 3935 2030 2e30 3730 3036 3436  412295 0.0700646
-0000a5a0: 3833 2c33 2e34 3132 3239 3520 2d37 2e33  83,3.412295 -7.3
-0000a5b0: 3330 3237 3765 2d30 352c 332e 3431 3232  30277e-05,3.4122
-0000a5c0: 3935 2043 202d 372e 3333 3032 3737 652d  95 C -7.330277e-
-0000a5d0: 3035 2c32 2e37 3239 3533 3335 202d 372e  05,2.7295335 -7.
-0000a5e0: 3333 3032 3737 652d 3035 2c32 2e30 3436  330277e-05,2.046
-0000a5f0: 3737 3220 2d37 2e33 3330 3237 3765 2d30  772 -7.330277e-0
-0000a600: 352c 312e 3336 3430 3130 3620 4320 302e  5,1.3640106 C 0.
-0000a610: 3632 3736 3334 3534 2c31 2e33 3634 3033  62763454,1.36403
-0000a620: 3137 2031 2e32 3535 3334 3234 2c31 2e33  17 1.2553424,1.3
-0000a630: 3633 3936 3936 2031 2e38 3833 3035 3032  639696 1.8830502
-0000a640: 2c31 2e33 3634 3034 3136 2043 2032 2e34  ,1.3640416 C 2.4
-0000a650: 3439 3434 342c 312e 3336 3538 3531 3520  49444,1.3658515 
-0000a660: 332e 3032 3130 3939 2c31 2e34 3339 3131  3.021099,1.43911
-0000a670: 3536 2033 2e35 3535 3031 312c 312e 3633  56 3.555011,1.63
-0000a680: 3433 3239 3520 4320 332e 3938 3336 3639  43295 C 3.983669
-0000a690: 342c 312e 3739 3031 3037 3120 342e 3338  4,1.7901071 4.38
-0000a6a0: 3332 3836 392c 322e 3032 3931 3538 2034  32869,2.029158 4
-0000a6b0: 2e37 3134 3738 382c 322e 3334 3331 3737  .714788,2.343177
-0000a6c0: 3420 4320 352e 3036 3932 3535 342c 322e  4 C 5.0692554,2.
-0000a6d0: 3637 3634 3830 3520 352e 3334 3335 3931  6764805 5.343591
-0000a6e0: 312c 332e 3038 3834 3836 3120 352e 3534  1,3.0884861 5.54
-0000a6f0: 3432 3334 392c 332e 3533 3031 3633 3220  42349,3.5301632 
-0000a700: 4320 352e 3834 3731 3630 382c 342e 3138  C 5.8471608,4.18
-0000a710: 3435 3437 3920 362e 3038 3633 3437 342c  45479 6.0863474,
-0000a720: 342e 3836 3634 3233 2036 2e32 3939 3537  4.866423 6.29957
-0000a730: 3634 2c35 2e35 3534 3632 3035 2043 2036  64,5.5546205 C 6
-0000a740: 2e36 3331 3632 3134 2c36 2e36 3335 3035  .6316214,6.63505
-0000a750: 3720 362e 3839 3630 3035 372c 372e 3733  7 6.8960057,7.73
-0000a760: 3530 3636 3420 372e 3133 3138 3332 322c  50664 7.1318322,
-0000a770: 382e 3834 3030 3838 3620 4320 372e 3332  8.8400886 C 7.32
-0000a780: 3737 3433 372c 392e 3736 3231 3930 3220  77437,9.7621902 
-0000a790: 372e 3530 3135 3335 392c 3130 2e36 3838  7.5015359,10.688
-0000a7a0: 3838 3320 372e 3636 3135 3438 332c 3131  883 7.6615483,11
-0000a7b0: 2e36 3137 3834 3720 4320 382e 3038 3137  .617847 C 8.0817
-0000a7c0: 3833 392c 392e 3734 3030 3139 3120 382e  839,9.7400191 8.
-0000a7d0: 3635 3231 3732 332c 372e 3839 3130 3831  6521723,7.891081
-0000a7e0: 3220 392e 3433 3635 3035 312c 362e 3133  2 9.4365051,6.13
-0000a7f0: 3139 3739 3720 4320 3130 2e31 3232 3636  19797 C 10.12266
-0000a800: 352c 342e 3539 3238 3133 3220 3130 2e39  5,4.5928132 10.9
-0000a810: 3736 3733 372c 332e 3132 3338 3233 3320  76737,3.1238233 
-0000a820: 3132 2e30 3233 3337 322c 312e 3830 3038  12.023372,1.8008
-0000a830: 3733 3620 4320 3132 2e31 3432 3434 322c  736 C 12.142442,
-0000a840: 312e 3635 3431 3739 3220 3132 2e32 3538  1.6541792 12.258
-0000a850: 3639 2c31 2e35 3030 3439 3333 2031 322e  69,1.5004933 12.
-0000a860: 3338 3536 3037 2c31 2e33 3632 3937 3238  385607,1.3629728
-0000a870: 2043 2031 332e 3438 3036 3931 2c31 2e31   C 13.480691,1.1
-0000a880: 3532 3238 3338 2031 342e 3537 3537 3737  522838 14.575777
-0000a890: 2c30 2e39 3431 3539 3334 3920 3135 2e36  ,0.94159349 15.6
-0000a8a0: 3730 3836 312c 302e 3733 3039 3034 3437  70861,0.73090447
-0000a8b0: 2043 2031 362e 3031 3034 3932 2c31 2e35   C 16.010492,1.5
-0000a8c0: 3031 3536 3539 2031 362e 3237 3438 3832  015659 16.274882
-0000a8d0: 2c32 2e33 3033 3135 3839 2031 362e 3530  ,2.3031589 16.50
-0000a8e0: 3437 3237 2c33 2e31 3132 3633 3937 2043  4727,3.1126397 C
-0000a8f0: 2031 362e 3834 3731 3233 2c34 2e33 3237   16.847123,4.327
-0000a900: 3339 3237 2031 372e 3130 3930 3231 2c35  3927 17.109021,5
-0000a910: 2e35 3633 3339 3731 2031 372e 3333 3333  .5633971 17.3333
-0000a920: 3032 2c36 2e38 3034 3930 3832 2043 2031  02,6.8049082 C 1
-0000a930: 372e 3436 3536 3835 2c37 2e35 3339 3231  7.465685,7.53921
-0000a940: 3435 2031 372e 3538 3235 3636 2c38 2e32  45 17.582566,8.2
-0000a950: 3736 3233 3036 2031 372e 3639 3035 342c  762306 17.69054,
-0000a960: 392e 3031 3434 3931 3920 4320 3137 2e38  9.0144919 C 17.8
-0000a970: 3431 3031 312c 3130 2e30 3130 3535 3420  41011,10.010554 
-0000a980: 3137 2e39 3931 3438 2c31 312e 3030 3636  17.99148,11.0066
-0000a990: 3135 2031 382e 3134 3139 3531 2c31 322e  15 18.141951,12.
-0000a9a0: 3030 3236 3736 2043 2031 382e 3233 3632  002676 C 18.2362
-0000a9b0: 3236 2c31 322e 3638 3139 3832 2031 382e  26,12.681982 18.
-0000a9c0: 3333 3034 3638 2c31 332e 3336 3133 3439  330468,13.361349
-0000a9d0: 2031 382e 3431 3330 3531 2c31 342e 3034   18.413051,14.04
-0000a9e0: 3231 3935 2043 2031 382e 3434 3836 3639  2195 C 18.448669
-0000a9f0: 2c31 342e 3334 3036 3234 2031 382e 3437  ,14.340624 18.47
-0000aa00: 3930 3639 2c31 342e 3633 3936 3538 2031  9069,14.639658 1
-0000aa10: 382e 3531 3733 342c 3134 2e39 3337 3737  8.51734,14.93777
-0000aa20: 3420 4320 3138 2e36 3138 3933 342c 3135  4 C 18.618934,15
-0000aa30: 2e37 3435 3730 3820 3138 2e37 3431 3936  .745708 18.74196
-0000aa40: 372c 3136 2e35 3531 3739 3520 3138 2e39  7,16.551795 18.9
-0000aa50: 3136 3938 372c 3137 2e33 3437 3338 3120  16987,17.347381 
-0000aa60: 4320 3138 2e39 3936 3233 342c 3137 2e37  C 18.996234,17.7
-0000aa70: 3034 3532 3220 3139 2e30 3836 3134 312c  04522 19.086141,
-0000aa80: 3138 2e30 3539 3631 3320 3139 2e31 3937  18.059613 19.197
-0000aa90: 3434 322c 3138 2e34 3038 3232 2043 2031  442,18.40822 C 1
-0000aaa0: 392e 3635 3435 3634 2c31 372e 3533 3430  9.654564,17.5340
-0000aab0: 3134 2032 302e 3230 3330 3731 2c31 362e  14 20.203071,16.
-0000aac0: 3730 3132 3735 2032 302e 3838 3037 3036  701275 20.880706
-0000aad0: 2c31 352e 3938 3133 3533 2043 2032 312e  ,15.981353 C 21.
-0000aae0: 3434 3533 3737 2c31 352e 3338 3037 3731  445377,15.380771
-0000aaf0: 2032 322e 3130 3433 3138 2c31 342e 3836   22.104318,14.86
-0000ab00: 3335 3037 2032 322e 3834 3233 3136 2c31  3507 22.842316,1
-0000ab10: 342e 3439 3235 3836 2043 2032 332e 3531  4.492586 C 23.51
-0000ab20: 3834 3334 2c31 342e 3135 3035 3733 2032  8434,14.150573 2
-0000ab30: 342e 3235 3730 3535 2c31 332e 3933 3630  4.257055,13.9360
-0000ab40: 3235 2032 352e 3030 3934 3534 2c31 332e  25 25.009454,13.
-0000ab50: 3835 3033 3034 2043 2032 352e 3536 3639  850304 C 25.5669
-0000ab60: 3839 2c31 332e 3738 3733 3620 3236 2e31  89,13.78736 26.1
-0000ab70: 3332 3231 382c 3133 2e37 3834 3836 3920  32218,13.784869 
-0000ab80: 3236 2e36 3839 3431 2c31 332e 3835 3320  26.68941,13.853 
-0000ab90: 4320 3237 2e33 3730 3631 362c 3133 2e39  C 27.370616,13.9
-0000aba0: 3336 3037 3620 3238 2e30 3338 3837 362c  36076 28.038876,
-0000abb0: 3134 2e31 3333 3120 3238 2e36 3531 3036  14.1331 28.65106
-0000abc0: 312c 3134 2e34 3434 3136 3920 4320 3239  1,14.444169 C 29
-0000abd0: 2e32 3334 3138 372c 3134 2e37 3338 3731  .234187,14.73871
-0000abe0: 3320 3239 2e37 3633 3830 352c 3135 2e31  3 29.763805,15.1
-0000abf0: 3333 3738 3520 3330 2e32 3237 3530 312c  33785 30.227501,
-0000ac00: 3135 2e35 3932 3834 3720 4320 3330 2e37  15.592847 C 30.7
-0000ac10: 3137 3133 2c31 362e 3037 3135 3137 2033  1713,16.071517 3
-0000ac20: 312e 3133 3338 3035 2c31 362e 3632 3832  1.133805,16.6282
-0000ac30: 3132 2033 312e 3433 3139 342c 3137 2e32  12 31.43194,17.2
-0000ac40: 3435 3636 3220 4320 3331 2e37 3233 3539  45662 C 31.72359
-0000ac50: 2c31 372e 3834 3536 3833 2033 312e 3930  ,17.845683 31.90
-0000ac60: 3030 3738 2c31 382e 3439 3932 3332 2033  0078,18.499232 3
-0000ac70: 312e 3936 3634 3639 2c31 392e 3136 3233  1.966469,19.1623
-0000ac80: 3938 2043 2033 322e 3031 3536 3132 2c31  98 C 32.015612,1
-0000ac90: 392e 3635 3138 3631 2033 322e 3030 3933  9.651861 32.0093
-0000aca0: 3235 2c32 302e 3134 3633 3538 2033 312e  25,20.146358 31.
-0000acb0: 3935 3736 3034 2c32 302e 3633 3533 3336  957604,20.635336
-0000acc0: 2043 2033 312e 3837 3934 322c 3231 2e33   C 31.87942,21.3
-0000acd0: 3636 3138 3720 3331 2e36 3831 3834 382c  66187 31.681848,
-0000ace0: 3232 2e30 3835 3834 3920 3331 2e33 3539  22.085849 31.359
-0000acf0: 3030 372c 3232 2e37 3436 3938 3820 4320  007,22.746988 C 
-0000ad00: 3331 2e30 3335 3434 322c 3233 2e34 3133  31.035442,23.413
-0000ad10: 3539 3620 3330 2e35 3837 3136 352c 3234  596 30.587165,24
-0000ad20: 2e30 3136 3731 3820 3330 2e30 3537 3635  .016718 30.05765
-0000ad30: 2c32 342e 3533 3339 3937 2043 2032 392e  ,24.533997 C 29.
-0000ad40: 3535 3633 3834 2c32 352e 3032 3538 3933  556384,25.025893
-0000ad50: 2032 382e 3937 3639 3137 2c32 352e 3434   28.976917,25.44
-0000ad60: 3135 3231 2032 382e 3333 3739 3833 2c32  1521 28.337983,2
-0000ad70: 352e 3733 3535 3535 2043 2032 372e 3732  5.735555 C 27.72
-0000ad80: 3034 3331 2c32 362e 3032 3136 3639 2032  0431,26.021669 2
-0000ad90: 372e 3035 3133 3238 2c32 362e 3139 3133  7.051328,26.1913
-0000ada0: 3232 2032 362e 3337 3339 382c 3236 2e32  22 26.37398,26.2
-0000adb0: 3531 3237 3120 4320 3235 2e39 3033 3534  51271 C 25.90354
-0000adc0: 392c 3236 2e32 3933 3334 3920 3235 2e34  9,26.293349 25.4
-0000add0: 3239 3530 392c 3236 2e32 3834 3235 3920  29509,26.284259 
-0000ade0: 3234 2e39 3539 3335 312c 3236 2e32 3433  24.959351,26.243
-0000adf0: 3233 3320 4320 3234 2e31 3032 3436 342c  233 C 24.102464,
-0000ae00: 3236 2e31 3636 3832 3820 3233 2e32 3537  26.166828 23.257
-0000ae10: 3134 352c 3235 2e39 3535 3232 3720 3232  145,25.955227 22
-0000ae20: 2e34 3638 3435 312c 3235 2e36 3130 3939  .468451,25.61099
-0000ae30: 3120 4320 3231 2e36 3130 3633 322c 3235  1 C 21.610632,25
-0000ae40: 2e32 3338 3632 3120 3230 2e38 3233 3530  .238621 20.82350
-0000ae50: 312c 3234 2e37 3133 3534 3720 3230 2e31  1,24.713547 20.1
-0000ae60: 3236 3036 352c 3234 2e30 3932 3630 3320  26065,24.092603 
-0000ae70: 4320 3139 2e39 3231 3034 342c 3233 2e39  C 19.921044,23.9
-0000ae80: 3130 3336 3920 3139 2e37 3233 3333 362c  10369 19.723336,
-0000ae90: 3233 2e37 3139 3935 3120 3139 2e35 3332  23.719951 19.532
-0000aea0: 3731 362c 3233 2e35 3232 3732 3420 4320  716,23.522724 C 
-0000aeb0: 3139 2e31 3131 3834 392c 3234 2e36 3235  19.111849,24.625
-0000aec0: 3639 3220 3138 2e36 3635 3233 372c 3235  692 18.665237,25
-0000aed0: 2e37 3139 3834 3420 3138 2e31 3537 3134  .719844 18.15714
-0000aee0: 2c32 362e 3738 3538 3520 4320 3137 2e38  ,26.78585 C 17.8
-0000aef0: 3430 3431 2c32 372e 3434 3634 3836 2031  4041,27.446486 1
-0000af00: 372e 3530 3134 3638 2c32 382e 3039 3830  7.501468,28.0980
-0000af10: 3735 2031 372e 3130 3638 3131 2c32 382e  75 17.106811,28.
-0000af20: 3731 3539 3838 2043 2031 362e 3836 3532  715988 C 16.8652
-0000af30: 3837 2c32 392e 3039 3038 3735 2031 362e  87,29.090875 16.
-0000af40: 3630 3339 3834 2c32 392e 3435 3538 3433  603984,29.455843
-0000af50: 2031 362e 3239 3431 3637 2c32 392e 3737   16.294167,29.77
-0000af60: 3738 3633 2043 2031 352e 3934 3836 3435  7863 C 15.948645
-0000af70: 2c33 302e 3133 3735 3332 2031 352e 3532  ,30.137532 15.52
-0000af80: 3630 3936 2c33 302e 3431 3732 3820 3135  6096,30.41728 15
-0000af90: 2e30 3734 3132 342c 3330 2e36 3235 3035  .074124,30.62505
-0000afa0: 3320 4320 3134 2e35 3030 3039 312c 3330  3 C 14.500091,30
-0000afb0: 2e38 3839 3039 3520 3133 2e38 3832 3030  .889095 13.88200
-0000afc0: 312c 3331 2e30 3435 3336 2031 332e 3235  1,31.04536 13.25
-0000afd0: 3931 3032 2c33 312e 3134 3130 3433 2043  9102,31.141043 C
-0000afe0: 2031 322e 3631 3833 3234 2c33 312e 3233   12.618324,31.23
-0000aff0: 3838 3320 3131 2e39 3639 3235 352c 3331  883 11.969255,31
-0000b000: 2e32 3731 3436 3620 3131 2e33 3231 3536  .271466 11.32156
-0000b010: 362c 3331 2e32 3638 3936 3320 4320 3130  6,31.268963 C 10
-0000b020: 2e35 3938 3236 312c 3331 2e32 3638 3936  .598261,31.26896
-0000b030: 3320 392e 3837 3439 3537 322c 3331 2e32  3 9.8749572,31.2
-0000b040: 3638 3936 3320 392e 3135 3136 3532 392c  68963 9.1516529,
-0000b050: 3331 2e32 3638 3936 3320 4320 392e 3135  31.268963 C 9.15
-0000b060: 3136 3532 392c 3330 2e35 3737 3932 3520  16529,30.577925 
-0000b070: 392e 3135 3136 3532 392c 3239 2e38 3836  9.1516529,29.886
-0000b080: 3838 3920 392e 3135 3136 3532 392c 3239  889 9.1516529,29
-0000b090: 2e31 3935 3835 3120 4320 392e 3532 3834  .195851 C 9.5284
-0000b0a0: 3139 372c 3239 2e31 3935 3734 3620 392e  197,29.195746 9.
-0000b0b0: 3930 3531 3837 372c 3239 2e31 3936 3037  9051877,29.19607
-0000b0c0: 2031 302e 3238 3139 3534 2c32 392e 3139   10.281954,29.19
-0000b0d0: 3536 3732 2043 2031 302e 3938 3030 3735  5672 C 10.980075
-0000b0e0: 2c32 392e 3139 3135 3120 3131 2e36 3830  ,29.19151 11.680
-0000b0f0: 3734 362c 3239 2e31 3434 3131 3620 3132  746,29.144116 12
-0000b100: 2e33 3635 3839 362c 3239 2e30 3034 3833  .365896,29.00483
-0000b110: 3520 4320 3132 2e38 3739 3231 322c 3238  5 C 12.879212,28
-0000b120: 2e38 3939 3138 3520 3133 2e33 3836 3431  .899185 13.38641
-0000b130: 352c 3238 2e37 3430 3535 2031 332e 3834  5,28.74055 13.84
-0000b140: 3631 3737 2c32 382e 3438 3533 3932 2043  6177,28.485392 C
-0000b150: 2031 342e 3138 3033 3836 2c32 382e 3330   14.180386,28.30
-0000b160: 3030 3937 2031 342e 3438 3634 3734 2c32  0097 14.486474,2
-0000b170: 382e 3035 3934 3520 3134 2e37 3238 3638  8.05945 14.72868
-0000b180: 2c32 372e 3736 3236 3937 2043 2031 342e  ,27.762697 C 14.
-0000b190: 3936 3835 3239 2c32 372e 3437 3031 3720  968529,27.47017 
-0000b1a0: 3135 2e31 3636 3836 2c32 372e 3134 3633  15.16686,27.1463
-0000b1b0: 3837 2031 352e 3335 3232 3038 2c32 362e  87 15.352208,26.
-0000b1c0: 3831 3734 3438 2043 2031 352e 3638 3436  817448 C 15.6846
-0000b1d0: 3835 2c32 362e 3232 3037 3238 2031 352e  85,26.220728 15.
-0000b1e0: 3936 3933 3631 2c32 352e 3539 3837 3937  969361,25.598797
-0000b1f0: 2031 362e 3233 3739 3038 2c32 342e 3937   16.237908,24.97
-0000b200: 3131 3639 2043 2031 362e 3639 3936 3239  1169 C 16.699629
-0000b210: 2c32 332e 3838 3437 3238 2031 372e 3130  ,23.884728 17.10
-0000b220: 3735 3133 2c32 322e 3737 3632 3734 2031  7513,22.776274 1
-0000b230: 372e 3439 3439 3635 2c32 312e 3636 3134  7.494965,21.6614
-0000b240: 3831 2043 2031 372e 3535 3831 312c 3231  81 C 17.55811,21
-0000b250: 2e34 3739 3335 3220 3137 2e36 3230 362c  .479352 17.6206,
-0000b260: 3231 2e32 3936 3939 3520 3137 2e36 3832  21.296995 17.682
-0000b270: 3530 322c 3231 2e31 3134 3433 3820 4320  502,21.114438 C 
-0000b280: 3137 2e33 3832 3230 362c 3230 2e35 3835  17.382206,20.585
-0000b290: 3939 3420 3137 2e31 3030 3433 352c 3230  994 17.100435,20
-0000b2a0: 2e30 3435 3733 3520 3136 2e38 3637 3435  .045735 16.86745
-0000b2b0: 2c31 392e 3438 3339 3237 2043 2031 362e  ,19.483927 C 16.
-0000b2c0: 3732 3734 3438 2c31 392e 3134 3439 3036  727448,19.144906
-0000b2d0: 2031 362e 3630 3633 3136 2c31 382e 3739   16.606316,18.79
-0000b2e0: 3639 3737 2031 362e 3532 3731 3337 2c31  6977 16.527137,1
-0000b2f0: 382e 3433 3834 3038 2043 2031 362e 3433  8.438408 C 16.43
-0000b300: 3239 3631 2c31 382e 3031 3836 3239 2031  2961,18.018629 1
-0000b310: 362e 3336 3236 3035 2c31 372e 3539 3339  6.362605,17.5939
-0000b320: 3631 2031 362e 3239 3439 3534 2c31 372e  61 16.294954,17.
-0000b330: 3136 3932 3436 2043 2031 362e 3134 3531  169246 C 16.1451
-0000b340: 3632 2c31 362e 3231 3131 3032 2031 362e  62,16.211102 16.
-0000b350: 3032 3233 3138 2c31 352e 3234 3920 3135  022318,15.249 15
-0000b360: 2e39 3033 3436 372c 3134 2e32 3836 3631  .903467,14.28661
-0000b370: 3220 4320 3135 2e36 3933 3437 382c 3132  2 C 15.693478,12
-0000b380: 2e37 3035 3938 3620 3135 2e34 3833 3438  .705986 15.48348
-0000b390: 392c 3131 2e31 3235 3336 3120 3135 2e32  9,11.125361 15.2
-0000b3a0: 3733 352c 392e 3534 3437 3334 3420 4320  735,9.5447344 C 
-0000b3b0: 3135 2e31 3230 3637 362c 382e 3338 3030  15.120676,8.3800
-0000b3c0: 3135 3320 3134 2e39 3434 3731 332c 372e  153 14.944713,7.
-0000b3d0: 3231 3735 3633 2031 342e 3730 3935 352c  217563 14.70955,
-0000b3e0: 362e 3036 3633 3436 3520 4320 3134 2e35  6.0663465 C 14.5
-0000b3f0: 3635 3539 342c 352e 3336 3935 3834 3720  65594,5.3695847 
-0000b400: 3134 2e34 3031 3834 362c 342e 3637 3537  14.401846,4.6757
-0000b410: 3035 3420 3134 2e31 3832 3832 2c33 2e39  054 14.18282,3.9
-0000b420: 3938 3330 3932 2043 2031 342e 3037 3932  983092 C 14.0792
-0000b430: 3334 2c33 2e36 3830 3838 3334 2031 332e  34,3.6808834 13.
-0000b440: 3936 3333 3434 2c33 2e33 3636 3833 3535  963344,3.3668355
-0000b450: 2031 332e 3832 3036 3438 2c33 2e30 3634   13.820648,3.064
-0000b460: 3730 3733 2043 2031 332e 3033 3333 3332  7073 C 13.033332
-0000b470: 2c33 2e39 3937 3731 3231 2031 322e 3337  ,3.9977121 12.37
-0000b480: 3036 3835 2c35 2e30 3330 3339 3735 2031  0685,5.0303975 1
-0000b490: 312e 3739 3534 3637 2c36 2e31 3035 3532  1.795467,6.10552
-0000b4a0: 3039 2043 2031 312e 3133 3039 3032 2c37  09 C 11.130902,7
-0000b4b0: 2e33 3439 3636 2031 302e 3538 3238 332c  .34966 10.58283,
-0000b4c0: 382e 3635 3331 3334 3820 3130 2e31 3038  8.6531348 10.108
-0000b4d0: 3630 362c 392e 3938 3035 3934 3520 4320  606,9.9805945 C 
-0000b4e0: 392e 3538 3737 3835 352c 3131 2e34 3237  9.5877855,11.427
-0000b4f0: 3930 3620 392e 3135 3834 3635 322c 3132  906 9.1584652,12
-0000b500: 2e39 3131 3431 3320 382e 3838 3732 3838  .911413 8.887288
-0000b510: 352c 3134 2e34 3236 3630 3320 4320 382e  5,14.426603 C 8.
-0000b520: 3639 3830 3536 342c 3135 2e34 3836 3537  6980564,15.48657
-0000b530: 3520 382e 3538 3831 3032 382c 3136 2e35  5 8.5881028,16.5
-0000b540: 3632 3438 3720 382e 3539 3238 3633 372c  62487 8.5928637,
-0000b550: 3137 2e36 3339 3835 3520 4320 382e 3539  17.639855 C 8.59
-0000b560: 3238 3633 372c 3138 2e30 3631 3439 3520  28637,18.061495 
-0000b570: 382e 3539 3238 3633 372c 3138 2e34 3833  8.5928637,18.483
-0000b580: 3133 3420 382e 3539 3238 3633 372c 3138  134 8.5928637,18
-0000b590: 2e39 3034 3737 3420 4320 372e 3736 3530  .904774 C 7.7650
-0000b5a0: 3237 332c 3138 2e39 3034 3737 3420 362e  273,18.904774 6.
-0000b5b0: 3933 3731 3932 322c 3138 2e39 3034 3737  9371922,18.90477
-0000b5c0: 3420 362e 3130 3933 3535 392c 3138 2e39  4 6.1093559,18.9
-0000b5d0: 3034 3737 3420 7a20 4d20 3230 2e30 3931  04774 z M 20.091
-0000b5e0: 3530 352c 3231 2e34 3132 3337 2043 2032  505,21.41237 C 2
-0000b5f0: 302e 3730 3339 3839 2c32 322e 3039 3133  0.703989,22.0913
-0000b600: 3033 2032 312e 3337 3632 3136 2c32 322e  03 21.376216,22.
-0000b610: 3732 3230 3220 3232 2e31 3330 3836 372c  72202 22.130867,
-0000b620: 3233 2e32 3431 3230 3620 4320 3232 2e37  23.241206 C 22.7
-0000b630: 3630 3237 362c 3233 2e36 3733 3638 2032  60276,23.67368 2
-0000b640: 332e 3435 3131 3536 2c32 342e 3032 3633  3.451156,24.0263
-0000b650: 3035 2032 342e 3138 3938 3735 2c32 342e  05 24.189875,24.
-0000b660: 3232 3831 3739 2043 2032 342e 3835 3138  228179 C 24.8518
-0000b670: 3136 2c32 342e 3431 3034 3036 2032 352e  16,24.410406 25.
-0000b680: 3535 3034 3239 2c32 342e 3436 3436 3431  550429,24.464641
-0000b690: 2032 362e 3233 3134 3037 2c32 342e 3337   26.231407,24.37
-0000b6a0: 3235 3836 2043 2032 362e 3734 3335 3132  2586 C 26.743512
-0000b6b0: 2c32 342e 3330 3335 3633 2032 372e 3234  ,24.303563 27.24
-0000b6c0: 3433 3532 2c32 342e 3134 3234 3439 2032  4352,24.142449 2
-0000b6d0: 372e 3639 3437 3337 2c32 332e 3838 3830  7.694737,23.8880
-0000b6e0: 3837 2043 2032 382e 3037 3339 3939 2c32  87 C 28.073999,2
-0000b6f0: 332e 3637 3533 3734 2032 382e 3431 3536  3.675374 28.4156
-0000b700: 3539 2c32 332e 3339 3839 3435 2032 382e  59,23.398945 28.
-0000b710: 3731 3335 3137 2c32 332e 3038 3238 3537  713517,23.082857
-0000b720: 2043 2032 392e 3038 3334 3837 2c32 322e   C 29.083487,22.
-0000b730: 3639 3632 3332 2032 392e 3338 3137 3035  696232 29.381705
-0000b740: 2c32 322e 3234 3035 3737 2032 392e 3538  ,22.240577 29.58
-0000b750: 3235 3037 2c32 312e 3734 3433 3532 2043  2507,21.744352 C
-0000b760: 2032 392e 3830 3637 3536 2c32 312e 3139   29.806756,21.19
-0000b770: 3435 3034 2032 392e 3931 3138 3934 2c32  4504 29.911894,2
-0000b780: 302e 3630 3037 3637 2032 392e 3932 3436  0.600767 29.9246
-0000b790: 3736 2c32 302e 3030 3834 3820 4320 3239  76,20.00848 C 29
-0000b7a0: 2e39 3337 3535 332c 3139 2e35 3135 3135  .937553,19.51515
-0000b7b0: 3620 3239 2e38 3739 3034 362c 3139 2e30  6 29.879046,19.0
-0000b7c0: 3137 3932 3120 3239 2e37 3239 3435 352c  17921 29.729455,
-0000b7d0: 3138 2e35 3436 3735 3620 4320 3239 2e35  18.546756 C 29.5
-0000b7e0: 3736 3730 392c 3138 2e30 3630 3535 3820  76709,18.060558 
-0000b7f0: 3239 2e33 3236 3834 312c 3137 2e36 3036  29.326841,17.606
-0000b800: 3339 3520 3239 2e30 3035 3334 2c31 372e  395 29.00534,17.
-0000b810: 3231 3134 3120 4320 3238 2e36 3531 3434  21141 C 28.65144
-0000b820: 332c 3136 2e37 3736 3531 3320 3238 2e32  3,16.776513 28.2
-0000b830: 3139 3438 392c 3136 2e34 3030 3533 3720  19489,16.400537 
-0000b840: 3237 2e37 3232 3732 372c 3136 2e31 3337  27.722727,16.137
-0000b850: 3336 3420 4320 3237 2e32 3835 3137 352c  364 C 27.285175,
-0000b860: 3135 2e39 3033 3934 3620 3236 2e38 3030  15.903946 26.800
-0000b870: 3536 332c 3135 2e37 3632 3430 3220 3236  563,15.762402 26
-0000b880: 2e33 3037 3630 322c 3135 2e37 3132 3532  .307602,15.71252
-0000b890: 3820 4320 3235 2e36 3338 3532 392c 3135  8 C 25.638529,15
-0000b8a0: 2e36 3434 3838 3920 3234 2e39 3532 3537  .644889 24.95257
-0000b8b0: 362c 3135 2e37 3235 3134 3620 3234 2e33  6,15.725146 24.3
-0000b8c0: 3232 3838 372c 3135 2e39 3633 3839 3620  22887,15.963896 
-0000b8d0: 4320 3233 2e37 3331 3738 312c 3136 2e31  C 23.731781,16.1
-0000b8e0: 3835 3738 3120 3233 2e31 3936 3933 362c  85781 23.196936,
-0000b8f0: 3136 2e35 3431 3432 2032 322e 3733 3533  16.54142 22.7353
-0000b900: 382c 3136 2e39 3639 3534 3220 4320 3232  8,16.969542 C 22
-0000b910: 2e31 3730 3139 372c 3137 2e34 3933 3337  .170197,17.49337
-0000b920: 3620 3231 2e37 3037 3137 362c 3138 2e31  6 21.707176,18.1
-0000b930: 3138 3236 3320 3231 2e33 3132 3536 2c31  18263 21.31256,1
-0000b940: 382e 3737 3737 2043 2032 302e 3831 3539  8.7777 C 20.8159
-0000b950: 3833 2c31 392e 3631 3038 3337 2032 302e  83,19.610837 20.
-0000b960: 3432 3433 3731 2c32 302e 3530 3236 3837  424371,20.502687
-0000b970: 2032 302e 3039 3135 3035 2c32 312e 3431   20.091505,21.41
-0000b980: 3233 3720 7a20 2720 7374 796c 653d 2766  237 z ' style='f
-0000b990: 696c 6c3a 2024 7a6f 6469 6163 5f63 6f6c  ill: $zodiac_col
-0000b9a0: 6f72 5f39 3b27 202f 3e0d 0a20 2020 2020  or_9;' />..     
-0000b9b0: 2020 2020 2020 2020 2020 203c 2f73 796d             </sym
-0000b9c0: 626f 6c3e 0d0a 2020 2020 2020 2020 2020  bol>..          
-0000b9d0: 2020 2020 2020 3c73 796d 626f 6c20 6964        <symbol id
-0000b9e0: 3d27 6171 7561 7269 7573 273e 0d0a 2020  ='aquarius'>..  
-0000b9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ba00: 2020 3c70 6174 6820 7472 616e 7366 6f72    <path transfor
-0000ba10: 6d3d 2273 6361 6c65 2830 2e38 2922 2064  m="scale(0.8)" d
-0000ba20: 3d27 4d20 3265 2d30 362c 3234 2e37 3031  ='M 2e-06,24.701
-0000ba30: 3635 3720 4c20 392e 3637 3731 312c 3138  657 L 9.67711,18
-0000ba40: 2e33 3232 3638 3420 4c20 3131 2e37 3937  .322684 L 11.797
-0000ba50: 3539 322c 3233 2e32 3634 3134 3220 4c20  592,23.264142 L 
-0000ba60: 3139 2e32 3839 3936 312c 3138 2e33 3232  19.289961,18.322
-0000ba70: 3638 3420 4c20 3231 2e33 3834 3734 2c32  684 L 21.38474,2
-0000ba80: 332e 3236 3431 3432 204c 2032 382e 3838  3.264142 L 28.88
-0000ba90: 3939 362c 3138 2e33 3232 3638 3420 4c20  996,18.322684 L 
-0000baa0: 3331 2e39 3837 3134 392c 3235 2e36 3030  31.987149,25.600
-0000bab0: 3130 3420 4c20 3239 2e39 3832 3333 2c32  104 L 29.98233,2
-0000bac0: 362e 3438 3537 3136 204c 2032 372e 3931  6.485716 L 27.91
-0000bad0: 3332 3533 2c32 312e 3534 3432 3538 204c  3253,21.544258 L
-0000bae0: 2032 302e 3338 3233 332c 3236 2e34 3835   20.38233,26.485
-0000baf0: 3731 3620 4c20 3138 2e32 3837 3535 312c  716 L 18.287551,
-0000bb00: 3231 2e35 3434 3235 3820 4c20 3130 2e38  21.544258 L 10.8
-0000bb10: 3230 3838 352c 3236 2e34 3835 3731 3620  20885,26.485716 
-0000bb20: 4c20 382e 3731 3332 3534 2c32 312e 3534  L 8.713254,21.54
-0000bb30: 3432 3538 204c 2031 2e31 3832 3333 312c  4258 L 1.182331,
-0000bb40: 3236 2e34 3835 3731 3620 4c20 3265 2d30  26.485716 L 2e-0
-0000bb50: 362c 3234 2e37 3031 3635 3720 7a20 4d20  6,24.701657 z M 
-0000bb60: 302e 3031 3238 3533 2c31 312e 3339 3138  0.012853,11.3918
-0000bb70: 3038 204c 2039 2e36 3839 3936 312c 3520  08 L 9.689961,5 
-0000bb80: 4c20 3131 2e38 3130 3434 332c 392e 3934  L 11.810443,9.94
-0000bb90: 3134 3538 204c 2031 392e 3331 3536 3634  1458 L 19.315664
-0000bba0: 2c35 204c 2032 312e 3431 3034 3433 2c39  ,5 L 21.410443,9
-0000bbb0: 2e39 3431 3435 3820 4c20 3238 2e39 3032  .941458 L 28.902
-0000bbc0: 3831 322c 3520 4c20 3332 2c31 322e 3237  812,5 L 32,12.27
-0000bbd0: 3734 3220 4c20 3239 2e39 3935 3138 312c  742 L 29.995181,
-0000bbe0: 3133 2e31 3633 3033 3220 4c20 3237 2e39  13.163032 L 27.9
-0000bbf0: 3236 3130 352c 382e 3232 3135 3734 204c  26105,8.221574 L
-0000bc00: 2032 302e 3338 3233 332c 3133 2e31 3633   20.38233,13.163
-0000bc10: 3033 3220 4c20 3138 2e32 3837 3535 312c  032 L 18.287551,
-0000bc20: 382e 3232 3135 3734 204c 2031 302e 3832  8.221574 L 10.82
-0000bc30: 3038 3835 2c31 332e 3136 3330 3332 204c  0885,13.163032 L
-0000bc40: 2038 2e37 3338 3935 372c 382e 3232 3135   8.738957,8.2215
-0000bc50: 3734 204c 2031 2e32 3038 3033 342c 3133  74 L 1.208034,13
-0000bc60: 2e31 3633 3033 3220 4c20 302e 3031 3238  .163032 L 0.0128
-0000bc70: 3533 2c31 312e 3339 3138 3038 207a 2027  53,11.391808 z '
-0000bc80: 2073 7479 6c65 3d27 6669 6c6c 3a20 247a   style='fill: $z
-0000bc90: 6f64 6961 635f 636f 6c6f 725f 3130 3b27  odiac_color_10;'
-0000bca0: 202f 3e0d 0a20 2020 2020 2020 2020 2020   />..           
-0000bcb0: 2020 2020 203c 2f73 796d 626f 6c3e 0d0a       </symbol>..
-0000bcc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bcd0: 3c73 796d 626f 6c20 6964 3d27 7069 7363  <symbol id='pisc
-0000bce0: 6573 273e 0d0a 2020 2020 2020 2020 2020  es'>..          
-0000bcf0: 2020 2020 2020 2020 2020 3c70 6174 6820            <path 
-0000bd00: 7472 616e 7366 6f72 6d3d 2273 6361 6c65  transform="scale
-0000bd10: 2830 2e38 2922 2064 3d27 4d20 3133 2e32  (0.8)" d='M 13.2
-0000bd20: 3838 3132 322c 3136 2e34 3933 3539 3320  88122,16.493593 
-0000bd30: 4320 3133 2e32 3838 3334 312c 3138 2e30  C 13.288341,18.0
-0000bd40: 3633 3639 3920 3133 2e30 3534 3638 2c31  63699 13.05468,1
-0000bd50: 392e 3632 3833 3632 2031 322e 3635 3939  9.628362 12.6599
-0000bd60: 3235 2c32 312e 3134 3631 3536 2043 2031  25,21.146156 C 1
-0000bd70: 322e 3335 3737 3034 2c32 322e 3330 3732  2.357704,22.3072
-0000bd80: 3434 2031 312e 3936 3332 3133 2c32 332e  44 11.963213,23.
-0000bd90: 3434 3334 3039 2031 312e 3530 3033 372c  443409 11.50037,
-0000bda0: 3234 2e35 3439 3935 3820 4320 3130 2e36  24.549958 C 10.6
-0000bdb0: 3836 3138 382c 3236 2e34 3738 3439 3320  86188,26.478493 
-0000bdc0: 392e 3636 3631 3735 372c 3238 2e33 3232  9.6661757,28.322
-0000bdd0: 3035 3320 382e 3434 3037 3139 372c 3330  053 8.4407197,30
-0000bde0: 2e30 3230 3037 3620 4320 372e 3934 3730  .020076 C 7.9470
-0000bdf0: 3935 372c 3330 2e37 3034 3635 2037 2e34  957,30.70465 7.4
-0000be00: 3230 3738 3037 2c33 312e 3336 3536 3439  207807,31.365649
-0000be10: 2036 2e38 3634 3039 3237 2c33 3220 4320   6.8640927,32 C 
-0000be20: 352e 3735 3534 3534 2c33 3220 342e 3634  5.755454,32 4.64
-0000be30: 3638 3135 332c 3332 2033 2e35 3338 3137  68153,32 3.53817
-0000be40: 3636 2c33 3220 4320 352e 3035 3232 3033  66,32 C 5.052203
-0000be50: 342c 3330 2e34 3034 3035 3520 362e 3430  4,30.404055 6.40
-0000be60: 3937 3932 372c 3238 2e36 3530 3837 3220  97927,28.650872 
-0000be70: 372e 3439 3831 3530 372c 3236 2e37 3336  7.4981507,26.736
-0000be80: 3333 3520 4320 382e 3433 3235 3034 372c  335 C 8.4325047,
-0000be90: 3235 2e30 3935 3232 3620 392e 3136 3330  25.095226 9.1630
-0000bea0: 3030 372c 3233 2e33 3334 3839 3620 392e  007,23.334896 9.
-0000beb0: 3632 3835 3737 372c 3231 2e35 3033 3537  6285777,21.50357
-0000bec0: 3920 4320 3130 2e30 3436 3233 382c 3139  9 C 10.046238,19
-0000bed0: 2e38 3638 3633 3620 3130 2e32 3531 3637  .868636 10.25167
-0000bee0: 352c 3138 2e31 3830 3731 3120 3130 2e32  5,18.180711 10.2
-0000bef0: 3530 3735 362c 3136 2e34 3933 3539 3320  50756,16.493593 
-0000bf00: 4320 382e 3038 3931 3633 372c 3136 2e34  C 8.0891637,16.4
-0000bf10: 3933 3539 3320 352e 3932 3735 3730 372c  93593 5.9275707,
-0000bf20: 3136 2e34 3933 3539 3320 332e 3736 3539  16.493593 3.7659
-0000bf30: 3739 312c 3136 2e34 3933 3539 3320 4320  791,16.493593 C 
-0000bf40: 332e 3736 3539 3739 312c 3135 2e37 3334  3.7659791,15.734
-0000bf50: 3231 3920 332e 3736 3539 3739 312c 3134  219 3.7659791,14
-0000bf60: 2e39 3734 3834 3620 332e 3736 3539 3739  .974846 3.765979
-0000bf70: 312c 3134 2e32 3135 3437 3220 4320 352e  1,14.215472 C 5.
-0000bf80: 3932 3735 3730 372c 3134 2e32 3135 3437  9275707,14.21547
-0000bf90: 3220 382e 3038 3931 3633 372c 3134 2e32  2 8.0891637,14.2
-0000bfa0: 3135 3437 3220 3130 2e32 3530 3735 362c  15472 10.250756,
-0000bfb0: 3134 2e32 3135 3437 3220 4320 3130 2e31  14.215472 C 10.1
-0000bfc0: 3535 3936 322c 3132 2e34 3937 3939 3120  55962,12.497991 
-0000bfd0: 392e 3831 3234 3836 372c 3130 2e37 3936  9.8124867,10.796
-0000bfe0: 3437 2039 2e32 3534 3634 3837 2c39 2e31  47 9.2546487,9.1
-0000bff0: 3730 3034 3320 4320 382e 3631 3035 3436  70043 C 8.610546
-0000c000: 372c 372e 3238 3634 2037 2e36 3836 3231  7,7.2864 7.68621
-0000c010: 3037 2c35 2e35 3035 3639 3120 362e 3538  07,5.505691 6.58
-0000c020: 3330 3636 372c 332e 3835 3132 3534 2043  30667,3.851254 C
-0000c030: 2035 2e36 3734 3330 3331 2c32 2e34 3837   5.6743031,2.487
-0000c040: 3930 3820 342e 3634 3531 3235 2c31 2e32  908 4.645125,1.2
-0000c050: 3037 3039 3839 2033 2e35 3338 3137 3636  070989 3.5381766
-0000c060: 2c33 652d 3037 2043 2034 2e35 3836 3036  ,3e-07 C 4.58606
-0000c070: 382c 3365 2d30 3720 352e 3633 3339 3539  8,3e-07 5.633959
-0000c080: 332c 3365 2d30 3720 362e 3638 3138 3530  3,3e-07 6.681850
-0000c090: 372c 3365 2d30 3720 4320 382e 3135 3939  7,3e-07 C 8.1599
-0000c0a0: 3339 372c 312e 3537 3538 3437 3620 392e  397,1.5758476 9.
-0000c0b0: 3436 3235 3835 372c 332e 3332 3136 3520  4625857,3.32165 
-0000c0c0: 3130 2e35 3034 3333 352c 352e 3231 3632  10.504335,5.2162
-0000c0d0: 3331 2043 2031 312e 3436 3030 3434 2c36  31 C 11.460044,6
-0000c0e0: 2e39 3530 3234 3820 3132 2e31 3933 3035  .950248 12.19305
-0000c0f0: 362c 382e 3830 3639 3139 2031 322e 3637  6,8.806919 12.67
-0000c100: 3637 3238 2c31 302e 3732 3639 3835 2043  6728,10.726985 C
-0000c110: 2031 322e 3936 3631 3731 2c31 312e 3837   12.966171,11.87
-0000c120: 3236 3435 2031 332e 3136 3833 3634 2c31  2645 13.168364,1
-0000c130: 332e 3034 3030 3036 2031 332e 3238 3831  3.040006 13.2881
-0000c140: 3232 2c31 342e 3231 3534 3732 2043 2031  22,14.215472 C 1
-0000c150: 352e 3338 3339 3035 2c31 342e 3231 3534  5.383905,14.2154
-0000c160: 3732 2031 372e 3437 3936 3838 2c31 342e  72 17.479688,14.
-0000c170: 3231 3534 3732 2031 392e 3537 3534 372c  215472 19.57547,
-0000c180: 3134 2e32 3135 3437 3220 4320 3139 2e37  14.215472 C 19.7
-0000c190: 3836 3838 322c 3132 2e31 3837 3735 3820  86882,12.187758 
-0000c1a0: 3230 2e32 3435 3838 342c 3130 2e31 3834  20.245884,10.184
-0000c1b0: 3133 2032 302e 3936 3332 3439 2c38 2e32  13 20.963249,8.2
-0000c1c0: 3735 3034 3120 4320 3231 2e36 3730 3432  75041 C 21.67042
-0000c1d0: 392c 362e 3338 3637 3732 2032 322e 3632  9,6.386772 22.62
-0000c1e0: 3836 3535 2c34 2e35 3934 3834 3920 3233  8655,4.594849 23
-0000c1f0: 2e37 3836 3533 332c 322e 3934 3439 3136  .786533,2.944916
-0000c200: 2043 2032 342e 3531 3334 3135 2c31 2e39   C 24.513415,1.9
-0000c210: 3037 3832 3239 2032 352e 3331 3735 3838  078229 25.317588
-0000c220: 2c30 2e39 3235 3536 3837 2032 362e 3138  ,0.9255687 26.18
-0000c230: 3137 3432 2c33 652d 3037 2043 2032 372e  1742,3e-07 C 27.
-0000c240: 3232 3936 3333 2c33 652d 3037 2032 382e  229633,3e-07 28.
-0000c250: 3237 3735 3235 2c33 652d 3037 2032 392e  277525,3e-07 29.
-0000c260: 3332 3534 3136 2c33 652d 3037 2043 2032  325416,3e-07 C 2
-0000c270: 372e 3835 3436 3138 2c31 2e36 3034 3038  7.854618,1.60408
-0000c280: 3837 2032 362e 3531 3838 3439 2c33 2e33  87 26.518849,3.3
-0000c290: 3430 3034 3720 3235 2e34 3234 3932 312c  40047 25.424921,
-0000c2a0: 352e 3232 3430 3136 2043 2032 342e 3437  5.224016 C 24.47
-0000c2b0: 3034 3538 2c36 2e38 3637 3033 2032 332e  0458,6.86703 23.
-0000c2c0: 3730 3439 3935 2c38 2e36 3235 3439 3820  704995,8.625498 
-0000c2d0: 3233 2e32 3135 3137 352c 3130 2e34 3633  23.215175,10.463
-0000c2e0: 3336 3420 4320 3232 2e38 3837 3534 372c  364 C 22.887547,
-0000c2f0: 3131 2e36 3839 3233 3220 3232 2e36 3833  11.689232 22.683
-0000c300: 3238 312c 3132 2e39 3438 3339 3220 3232  281,12.948392 22
-0000c310: 2e36 3132 3833 372c 3134 2e32 3135 3437  .612837,14.21547
-0000c320: 3220 4320 3234 2e37 3734 3432 382c 3134  2 C 24.774428,14
-0000c330: 2e32 3135 3437 3220 3236 2e39 3336 3032  .215472 26.93602
-0000c340: 322c 3134 2e32 3135 3437 3220 3239 2e30  2,14.215472 29.0
-0000c350: 3937 3631 342c 3134 2e32 3135 3437 3220  97614,14.215472 
-0000c360: 4320 3239 2e30 3937 3631 342c 3134 2e39  C 29.097614,14.9
-0000c370: 3734 3834 3620 3239 2e30 3937 3631 342c  74846 29.097614,
-0000c380: 3135 2e37 3334 3231 3920 3239 2e30 3937  15.734219 29.097
-0000c390: 3631 342c 3136 2e34 3933 3539 3320 4320  614,16.493593 C 
-0000c3a0: 3236 2e39 3336 3032 322c 3136 2e34 3933  26.936022,16.493
-0000c3b0: 3539 3320 3234 2e37 3734 3432 382c 3136  593 24.774428,16
-0000c3c0: 2e34 3933 3539 3320 3232 2e36 3132 3833  .493593 22.61283
-0000c3d0: 372c 3136 2e34 3933 3539 3320 4320 3232  7,16.493593 C 22
-0000c3e0: 2e36 3131 3539 312c 3138 2e33 3130 3031  .611591,18.31001
-0000c3f0: 3320 3232 2e38 3530 3534 342c 3230 2e31  3 22.850544,20.1
-0000c400: 3237 3334 3720 3233 2e33 3334 3435 342c  27347 23.334454,
-0000c410: 3231 2e38 3738 3532 3420 4320 3233 2e38  21.878524 C 23.8
-0000c420: 3337 3332 322c 3233 2e37 3037 3239 3320  37322,23.707293 
-0000c430: 3234 2e36 3034 3336 392c 3235 2e34 3539  24.604369,25.459
-0000c440: 3439 3420 3235 2e35 3730 3639 342c 3237  494 25.570694,27
-0000c450: 2e30 3930 3130 3520 4320 3236 2e36 3232  .090105 C 26.622
-0000c460: 3732 372c 3238 2e38 3637 3736 3520 3237  727,28.867765 27
-0000c470: 2e39 3035 3038 332c 3330 2e35 3032 3732  .905083,30.50272
-0000c480: 3320 3239 2e33 3235 3431 362c 3332 2043  3 29.325416,32 C
-0000c490: 2032 382e 3232 3138 3339 2c33 3220 3237   28.221839,32 27
-0000c4a0: 2e31 3138 3236 342c 3332 2032 362e 3031  .118264,32 26.01
-0000c4b0: 3436 3837 2c33 3220 4320 3234 2e36 3934  4687,32 C 24.694
-0000c4c0: 3433 352c 3330 2e35 3038 3337 3720 3233  435,30.508377 23
-0000c4d0: 2e35 3439 3139 372c 3238 2e38 3633 3331  .549197,28.86331
-0000c4e0: 3520 3232 2e35 3937 3331 332c 3237 2e31  5 22.597313,27.1
-0000c4f0: 3133 3832 3120 4320 3232 2e31 3034 3238  13821 C 22.10428
-0000c500: 2c32 362e 3230 3737 3938 2032 312e 3636  ,26.207798 21.66
-0000c510: 3035 3333 2c32 352e 3237 3439 3120 3231  0533,25.27491 21
-0000c520: 2e32 3638 3236 352c 3234 2e33 3230 3933  .268265,24.32093
-0000c530: 3520 4320 3230 2e36 3233 3633 342c 3232  5 C 20.623634,22
-0000c540: 2e37 3337 3733 3920 3230 2e31 3135 3631  .737739 20.11561
-0000c550: 332c 3231 2e30 3933 3732 3920 3139 2e38  3,21.093729 19.8
-0000c560: 3238 3932 322c 3139 2e34 3036 3732 3120  28922,19.406721 
-0000c570: 4320 3139 2e36 3635 3538 352c 3138 2e34  C 19.665585,18.4
-0000c580: 3434 3736 3820 3139 2e35 3735 3430 322c  44768 19.575402,
-0000c590: 3137 2e34 3639 3630 3320 3139 2e35 3735  17.469603 19.575
-0000c5a0: 3437 2c31 362e 3439 3335 3933 2043 2031  47,16.493593 C 1
-0000c5b0: 372e 3437 3936 3838 2c31 362e 3439 3335  7.479688,16.4935
-0000c5c0: 3933 2031 352e 3338 3339 3035 2c31 362e  93 15.383905,16.
-0000c5d0: 3439 3335 3933 2031 332e 3238 3831 3232  493593 13.288122
-0000c5e0: 2c31 362e 3439 3335 3933 207a 2027 2073  ,16.493593 z ' s
-0000c5f0: 7479 6c65 3d27 6669 6c6c 3a20 247a 6f64  tyle='fill: $zod
-0000c600: 6961 635f 636f 6c6f 725f 3131 3b27 202f  iac_color_11;' /
-0000c610: 3e0d 0a20 2020 2020 2020 2020 2020 2020  >..             
-0000c620: 2020 203c 2f73 796d 626f 6c3e 2020 2020     </symbol>    
-0000c630: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-0000c640: 2020 2020 2020 2020 2020 2020 2020 3c21                <!
-0000c650: 2d2d 2041 7370 6563 7473 2031 3278 3132  -- Aspects 12x12
-0000c660: 202d 2d3e 0d0a 2020 2020 2020 2020 2020   -->..          
-0000c670: 2020 2020 2020 3c73 796d 626f 6c20 6964        <symbol id
-0000c680: 3d27 6f72 6230 273e 0d0a 2020 2020 2020  ='orb0'>..      
-0000c690: 2020 2020 2020 2020 2020 2020 2020 3c70                <p
-0000c6a0: 6174 6820 643d 274d 2036 2e30 3639 3735  ath d='M 6.06975
-0000c6b0: 3339 2c37 2e33 3233 3438 3532 2043 2036  39,7.3234852 C 6
-0000c6c0: 2e30 3639 3735 3339 2c38 2e37 3335 3438  .0697539,8.73548
-0000c6d0: 3832 2034 2e39 3137 3336 3531 2c39 2e38  82 4.9173651,9.8
-0000c6e0: 3830 3134 3432 2033 2e34 3935 3832 3134  801442 3.4958214
-0000c6f0: 2c39 2e38 3830 3134 3432 2043 2032 2e30  ,9.8801442 C 2.0
-0000c700: 3734 3237 3735 2c39 2e38 3830 3134 3432  742775,9.8801442
-0000c710: 2030 2e39 3231 3838 3835 372c 382e 3733   0.92188857,8.73
-0000c720: 3534 3838 3220 302e 3932 3138 3838 3537  54882 0.92188857
-0000c730: 2c37 2e33 3233 3438 3532 2043 2030 2e39  ,7.3234852 C 0.9
-0000c740: 3231 3838 3835 372c 352e 3931 3134 3832  2188857,5.911482
-0000c750: 3220 322e 3037 3432 3737 352c 342e 3736  2 2.0742775,4.76
-0000c760: 3638 3237 3220 332e 3439 3538 3231 342c  68272 3.4958214,
-0000c770: 342e 3736 3638 3237 3220 4320 342e 3931  4.7668272 C 4.91
-0000c780: 3733 3635 312c 342e 3736 3638 3237 3220  73651,4.7668272 
-0000c790: 362e 3036 3937 3533 392c 352e 3931 3134  6.0697539,5.9114
-0000c7a0: 3832 3220 362e 3036 3937 3533 392c 372e  822 6.0697539,7.
-0000c7b0: 3332 3334 3835 3220 4c20 362e 3036 3937  3234852 L 6.0697
-0000c7c0: 3533 392c 372e 3332 3334 3835 3220 7a20  539,7.3234852 z 
-0000c7d0: 4d20 352e 3632 3532 3630 392c 352e 3231  M 5.6252609,5.21
-0000c7e0: 3133 3230 3220 4320 3130 2e30 3730 3139  13202 C 10.07019
-0000c7f0: 2c30 2e37 3636 3339 3031 3820 3130 2e30  ,0.76639018 10.0
-0000c800: 3730 3139 2c30 2e37 3636 3339 3031 3820  7019,0.76639018 
-0000c810: 3130 2e30 3730 3139 2c30 2e37 3636 3339  10.07019,0.76639
-0000c820: 3031 3827 2073 7479 6c65 3d27 6f70 6163  018' style='opac
-0000c830: 6974 793a 313b 6669 6c6c 3a6e 6f6e 653b  ity:1;fill:none;
-0000c840: 6669 6c6c 2d6f 7061 6369 7479 3a31 3b66  fill-opacity:1;f
-0000c850: 696c 6c2d 7275 6c65 3a6e 6f6e 7a65 726f  ill-rule:nonzero
-0000c860: 3b73 7472 6f6b 653a 2024 6f72 625f 636f  ;stroke: $orb_co
-0000c870: 6c6f 725f 303b 7374 726f 6b65 2d77 6964  lor_0;stroke-wid
-0000c880: 7468 3a31 2e34 3736 3333 3036 343b 7374  th:1.47633064;st
-0000c890: 726f 6b65 2d6c 696e 6563 6170 3a62 7574  roke-linecap:but
-0000c8a0: 743b 7374 726f 6b65 2d6c 696e 656a 6f69  t;stroke-linejoi
-0000c8b0: 6e3a 6d69 7465 723b 7374 726f 6b65 2d6d  n:miter;stroke-m
-0000c8c0: 6974 6572 6c69 6d69 743a 343b 7374 726f  iterlimit:4;stro
-0000c8d0: 6b65 2d64 6173 6861 7272 6179 3a6e 6f6e  ke-dasharray:non
-0000c8e0: 653b 7374 726f 6b65 2d6f 7061 6369 7479  e;stroke-opacity
-0000c8f0: 3a31 2720 2f3e 0d0a 2020 2020 2020 2020  :1' />..        
-0000c900: 2020 2020 2020 2020 3c2f 7379 6d62 6f6c          </symbol
-0000c910: 3e0d 0a20 2020 2020 2020 2020 2020 2020  >..             
-0000c920: 2020 203c 7379 6d62 6f6c 2069 643d 276f     <symbol id='o
-0000c930: 7262 3330 273e 0d0a 2020 2020 2020 2020  rb30'>..        
-0000c940: 2020 2020 2020 2020 2020 2020 3c70 6174              <pat
-0000c950: 6820 643d 274d 2030 2e38 3136 3735 3135  h d='M 0.8167515
-0000c960: 342c 362e 3133 3432 3339 3820 4320 3131  4,6.1342398 C 11
-0000c970: 2e33 3436 3631 352c 362e 3136 3230 3134  .346615,6.162014
-0000c980: 3820 3131 2e33 3436 3631 352c 362e 3136  8 11.346615,6.16
-0000c990: 3230 3134 3820 3131 2e33 3436 3631 352c  20148 11.346615,
-0000c9a0: 362e 3136 3230 3134 3820 4d20 3130 2e36  6.1620148 M 10.6
-0000c9b0: 3132 3138 342c 302e 3735 3939 3537 3733  12184,0.75995773
-0000c9c0: 2043 2035 2e37 3133 3834 3739 2c35 2e39   C 5.7138479,5.9
-0000c9d0: 3033 3231 3038 2035 2e37 3133 3834 3739  032108 5.7138479
-0000c9e0: 2c35 2e39 3033 3231 3038 2035 2e37 3133  ,5.9032108 5.713
-0000c9f0: 3834 3739 2c35 2e39 3033 3231 3038 204d  8479,5.9032108 M
-0000ca00: 2031 2e33 3035 3334 3531 2c30 2e37 3539   1.3053451,0.759
-0000ca10: 3935 3737 3320 4320 352e 3838 3037 3138  95773 C 5.880718
-0000ca20: 392c 362e 3139 3235 3136 3820 352e 3838  9,6.1925168 5.88
-0000ca30: 3037 3138 392c 362e 3139 3235 3136 3820  07189,6.1925168 
-0000ca40: 352e 3838 3037 3138 392c 362e 3139 3235  5.8807189,6.1925
-0000ca50: 3136 3827 2073 7479 6c65 3d27 6f70 6163  168' style='opac
-0000ca60: 6974 793a 313b 6669 6c6c 3a6e 6f6e 653b  ity:1;fill:none;
-0000ca70: 6669 6c6c 2d6f 7061 6369 7479 3a31 3b66  fill-opacity:1;f
-0000ca80: 696c 6c2d 7275 6c65 3a6e 6f6e 7a65 726f  ill-rule:nonzero
-0000ca90: 3b73 7472 6f6b 653a 2024 6f72 625f 636f  ;stroke: $orb_co
-0000caa0: 6c6f 725f 3330 3b73 7472 6f6b 652d 7769  lor_30;stroke-wi
-0000cab0: 6474 683a 312e 3437 3633 3330 3634 3b73  dth:1.47633064;s
-0000cac0: 7472 6f6b 652d 6c69 6e65 6361 703a 6275  troke-linecap:bu
-0000cad0: 7474 3b73 7472 6f6b 652d 6c69 6e65 6a6f  tt;stroke-linejo
-0000cae0: 696e 3a6d 6974 6572 3b73 7472 6f6b 652d  in:miter;stroke-
-0000caf0: 6d69 7465 726c 696d 6974 3a34 3b73 7472  miterlimit:4;str
-0000cb00: 6f6b 652d 6461 7368 6172 7261 793a 6e6f  oke-dasharray:no
-0000cb10: 6e65 3b73 7472 6f6b 652d 6f70 6163 6974  ne;stroke-opacit
-0000cb20: 793a 3127 202f 3e0d 0a20 2020 2020 2020  y:1' />..       
-0000cb30: 2020 2020 2020 2020 203c 2f73 796d 626f           </symbo
-0000cb40: 6c3e 0d0a 2020 2020 2020 2020 2020 2020  l>..            
-0000cb50: 2020 2020 3c73 796d 626f 6c20 6964 3d27      <symbol id='
-0000cb60: 6f72 6234 3527 3e0d 0a20 2020 2020 2020  orb45'>..       
-0000cb70: 2020 2020 2020 2020 2020 2020 203c 7061               <pa
-0000cb80: 7468 2064 3d27 4d20 392e 3831 3030 3137  th d='M 9.810017
-0000cb90: 382c 392e 3539 3231 3936 3620 4320 362e  8,9.5921966 C 6.
-0000cba0: 3936 3430 3635 382c 392e 3539 3231 3935  9640658,9.592195
-0000cbb0: 3620 342e 3131 3831 3132 352c 392e 3539  6 4.1181125,9.59
-0000cbc0: 3231 3936 3620 312e 3237 3231 362c 392e  21966 1.27216,9.
-0000cbd0: 3539 3231 3936 3620 4320 322e 3639 3531  5921966 C 2.6951
-0000cbe0: 3336 322c 362e 3734 3632 3434 3120 342e  362,6.7462441 4.
-0000cbf0: 3131 3831 3132 352c 332e 3930 3032 3930  1181125,3.900290
-0000cc00: 3520 352e 3534 3130 3838 382c 312e 3035  5 5.5410888,1.05
-0000cc10: 3433 3337 3927 2073 7479 6c65 3d27 6f70  43379' style='op
-0000cc20: 6163 6974 793a 313b 6669 6c6c 3a6e 6f6e  acity:1;fill:non
-0000cc30: 653b 6669 6c6c 2d6f 7061 6369 7479 3a31  e;fill-opacity:1
-0000cc40: 3b66 696c 6c2d 7275 6c65 3a6e 6f6e 7a65  ;fill-rule:nonze
-0000cc50: 726f 3b73 7472 6f6b 653a 2024 6f72 625f  ro;stroke: $orb_
-0000cc60: 636f 6c6f 725f 3435 3b73 7472 6f6b 652d  color_45;stroke-
-0000cc70: 7769 6474 683a 312e 3437 3633 3330 3634  width:1.47633064
-0000cc80: 3b73 7472 6f6b 652d 6c69 6e65 6361 703a  ;stroke-linecap:
-0000cc90: 6275 7474 3b73 7472 6f6b 652d 6c69 6e65  butt;stroke-line
-0000cca0: 6a6f 696e 3a6d 6974 6572 3b73 7472 6f6b  join:miter;strok
-0000ccb0: 652d 6d69 7465 726c 696d 6974 3a34 3b73  e-miterlimit:4;s
-0000ccc0: 7472 6f6b 652d 6461 7368 6172 7261 793a  troke-dasharray:
-0000ccd0: 6e6f 6e65 3b73 7472 6f6b 652d 6f70 6163  none;stroke-opac
-0000cce0: 6974 793a 3127 202f 3e0d 0a20 2020 2020  ity:1' />..     
-0000ccf0: 2020 2020 2020 2020 2020 203c 2f73 796d             </sym
-0000cd00: 626f 6c3e 0d0a 2020 2020 2020 2020 2020  bol>..          
-0000cd10: 2020 2020 2020 3c73 796d 626f 6c20 6964        <symbol id
-0000cd20: 3d27 6f72 6236 3027 3e0d 0a20 2020 2020  ='orb60'>..     
-0000cd30: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-0000cd40: 7061 7468 2064 3d27 4d20 302e 3838 3138  path d='M 0.8818
-0000cd50: 3234 3431 2c30 2e37 3138 3134 3736 3520  2441,0.71814765 
-0000cd60: 4320 332e 3338 3036 3837 322c 332e 3231  C 3.3806872,3.21
-0000cd70: 3736 3030 3720 352e 3837 3935 3530 322c  76007 5.8795502,
-0000cd80: 352e 3731 3730 3532 3720 382e 3337 3834  5.7170527 8.3784
-0000cd90: 3133 322c 382e 3231 3635 3035 3720 4d20  132,8.2165057 M 
-0000cda0: 382e 3631 3139 3336 322c 342e 3430 3336  8.6119362,4.4036
-0000cdb0: 3535 3720 4320 352e 3936 3430 3434 322c  557 C 5.9640442,
-0000cdc0: 342e 3430 3336 3535 3720 332e 3331 3631  4.4036557 3.3161
-0000cdd0: 3533 342c 342e 3430 3336 3535 3720 302e  534,4.4036557 0.
-0000cde0: 3636 3832 3632 3231 2c34 2e34 3033 3635  66826221,4.40365
-0000cdf0: 3537 204d 2030 2e38 3439 3235 3738 312c  57 M 0.84925781,
-0000ce00: 382e 3139 3434 3937 3720 4320 332e 3337  8.1944977 C 3.37
-0000ce10: 3634 3835 322c 352e 3732 3234 3333 3720  64852,5.7224337 
-0000ce20: 352e 3930 3337 3133 322c 332e 3235 3033  5.9037132,3.2503
-0000ce30: 3730 3720 382e 3433 3039 3430 322c 302e  707 8.4309402,0.
-0000ce40: 3737 3833 3037 3635 2720 7374 796c 653d  77830765' style=
-0000ce50: 276f 7061 6369 7479 3a31 3b66 696c 6c3a  'opacity:1;fill:
-0000ce60: 6e6f 6e65 3b66 696c 6c2d 6f70 6163 6974  none;fill-opacit
-0000ce70: 793a 313b 6669 6c6c 2d72 756c 653a 6e6f  y:1;fill-rule:no
-0000ce80: 6e7a 6572 6f3b 7374 726f 6b65 3a20 246f  nzero;stroke: $o
-0000ce90: 7262 5f63 6f6c 6f72 5f36 303b 7374 726f  rb_color_60;stro
-0000cea0: 6b65 2d77 6964 7468 3a31 2e34 3736 3333  ke-width:1.47633
-0000ceb0: 3036 343b 7374 726f 6b65 2d6c 696e 6563  064;stroke-linec
-0000cec0: 6170 3a62 7574 743b 7374 726f 6b65 2d6c  ap:butt;stroke-l
-0000ced0: 696e 656a 6f69 6e3a 6d69 7465 723b 7374  inejoin:miter;st
-0000cee0: 726f 6b65 2d6d 6974 6572 6c69 6d69 743a  roke-miterlimit:
-0000cef0: 343b 7374 726f 6b65 2d64 6173 6861 7272  4;stroke-dasharr
-0000cf00: 6179 3a6e 6f6e 653b 7374 726f 6b65 2d6f  ay:none;stroke-o
-0000cf10: 7061 6369 7479 3a31 2720 2f3e 0d0a 2020  pacity:1' />..  
-0000cf20: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-0000cf30: 7379 6d62 6f6c 3e0d 0a20 2020 2020 2020  symbol>..       
-0000cf40: 2020 2020 2020 2020 203c 7379 6d62 6f6c           <symbol
-0000cf50: 2069 643d 276f 7262 3732 273e 0d0a 2020   id='orb72'>..  
-0000cf60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cf70: 2020 3c70 6174 6820 643d 274d 2038 2e39    <path d='M 8.9
-0000cf80: 3136 3530 3434 2c35 2e36 3431 3734 3338  165044,5.6417438
-0000cf90: 2043 2038 2e39 3136 3530 3434 2c37 2e39   C 8.9165044,7.9
-0000cfa0: 3638 3736 3633 2037 2e32 3734 3238 3434  687663 7.2742844
-0000cfb0: 2c39 2e38 3535 3138 3933 2035 2e32 3438  ,9.8551893 5.248
-0000cfc0: 3530 3334 2c39 2e38 3535 3138 3933 2043  5034,9.8551893 C
-0000cfd0: 2033 2e32 3232 3732 3234 2c39 2e38 3535   3.2227224,9.855
-0000cfe0: 3138 3933 2031 2e35 3830 3530 3237 2c37  1893 1.5805027,7
-0000cff0: 2e39 3638 3736 3633 2031 2e35 3830 3530  .9687663 1.58050
-0000d000: 3237 2c35 2e36 3431 3734 3338 2043 2031  27,5.6417438 C 1
-0000d010: 2e35 3830 3530 3237 2c33 2e33 3134 3732  .5805027,3.31472
-0000d020: 3038 2033 2e32 3232 3732 3234 2c31 2e34  08 3.2227224,1.4
-0000d030: 3238 3239 3637 2035 2e32 3438 3530 3334  282967 5.2485034
-0000d040: 2c31 2e34 3238 3239 3637 2043 2037 2e32  ,1.4282967 C 7.2
-0000d050: 3734 3238 3434 2c31 2e34 3238 3239 3637  742844,1.4282967
-0000d060: 2038 2e39 3136 3530 3434 2c33 2e33 3134   8.9165044,3.314
-0000d070: 3732 3038 2038 2e39 3136 3530 3434 2c35  7208 8.9165044,5
-0000d080: 2e36 3431 3734 3338 204c 2038 2e39 3136  .6417438 L 8.916
-0000d090: 3530 3434 2c35 2e36 3431 3734 3338 207a  5044,5.6417438 z
-0000d0a0: 204d 2035 2e34 3730 3236 3334 2c36 2e37   M 5.4702634,6.7
-0000d0b0: 3436 3333 3538 2043 2039 2e30 3531 3138  463358 C 9.05118
-0000d0c0: 3034 2c31 302e 3131 3932 3238 2039 2e30  04,10.119228 9.0
-0000d0d0: 3531 3138 3034 2c31 302e 3131 3932 3238  511804,10.119228
-0000d0e0: 2039 2e30 3531 3138 3034 2c31 302e 3131   9.0511804,10.11
-0000d0f0: 3932 3238 2720 7374 796c 653d 276f 7061  9228' style='opa
-0000d100: 6369 7479 3a31 3b66 696c 6c3a 6e6f 6e65  city:1;fill:none
-0000d110: 3b66 696c 6c2d 6f70 6163 6974 793a 313b  ;fill-opacity:1;
-0000d120: 6669 6c6c 2d72 756c 653a 6e6f 6e7a 6572  fill-rule:nonzer
-0000d130: 6f3b 7374 726f 6b65 3a20 246f 7262 5f63  o;stroke: $orb_c
-0000d140: 6f6c 6f72 5f37 323b 7374 726f 6b65 2d77  olor_72;stroke-w
-0000d150: 6964 7468 3a31 2e34 3736 3333 3036 343b  idth:1.47633064;
-0000d160: 7374 726f 6b65 2d6c 696e 6563 6170 3a62  stroke-linecap:b
-0000d170: 7574 743b 7374 726f 6b65 2d6c 696e 656a  utt;stroke-linej
-0000d180: 6f69 6e3a 6d69 7465 723b 7374 726f 6b65  oin:miter;stroke
-0000d190: 2d6d 6974 6572 6c69 6d69 743a 343b 7374  -miterlimit:4;st
-0000d1a0: 726f 6b65 2d64 6173 6861 7272 6179 3a6e  roke-dasharray:n
-0000d1b0: 6f6e 653b 7374 726f 6b65 2d6f 7061 6369  one;stroke-opaci
-0000d1c0: 7479 3a31 2720 2f3e 0d0a 2020 2020 2020  ty:1' />..      
-0000d1d0: 2020 2020 2020 2020 2020 3c2f 7379 6d62            </symb
-0000d1e0: 6f6c 3e0d 0a20 2020 2020 2020 2020 2020  ol>..           
-0000d1f0: 2020 2020 203c 7379 6d62 6f6c 2069 643d       <symbol id=
-0000d200: 276f 7262 3930 273e 0d0a 2020 2020 2020  'orb90'>..      
-0000d210: 2020 2020 2020 2020 2020 2020 2020 3c72                <r
-0000d220: 6563 7420 6865 6967 6874 3d27 382e 3038  ect height='8.08
-0000d230: 3631 3935 2720 7769 6474 683d 2738 2e37  6195' width='8.7
-0000d240: 3135 3831 3336 2720 783d 2731 2e31 3833  158136' x='1.183
-0000d250: 3138 3236 2720 793d 2731 2e31 3839 3235  1826' y='1.18925
-0000d260: 3435 2720 7374 796c 653d 276f 7061 6369  45' style='opaci
-0000d270: 7479 3a31 3b66 696c 6c3a 6e6f 6e65 3b66  ty:1;fill:none;f
-0000d280: 696c 6c2d 6f70 6163 6974 793a 313b 6669  ill-opacity:1;fi
-0000d290: 6c6c 2d72 756c 653a 6e6f 6e7a 6572 6f3b  ll-rule:nonzero;
-0000d2a0: 7374 726f 6b65 3a20 246f 7262 5f63 6f6c  stroke: $orb_col
-0000d2b0: 6f72 5f39 303b 7374 726f 6b65 2d77 6964  or_90;stroke-wid
-0000d2c0: 7468 3a31 2e32 3530 3339 3531 383b 7374  th:1.25039518;st
-0000d2d0: 726f 6b65 2d6c 696e 6563 6170 3a62 7574  roke-linecap:but
-0000d2e0: 743b 7374 726f 6b65 2d6c 696e 656a 6f69  t;stroke-linejoi
-0000d2f0: 6e3a 6d69 7465 723b 7374 726f 6b65 2d6d  n:miter;stroke-m
-0000d300: 6974 6572 6c69 6d69 743a 343b 7374 726f  iterlimit:4;stro
-0000d310: 6b65 2d64 6173 6861 7272 6179 3a6e 6f6e  ke-dasharray:non
-0000d320: 653b 7374 726f 6b65 2d6f 7061 6369 7479  e;stroke-opacity
-0000d330: 3a31 2720 2f3e 0d0a 2020 2020 2020 2020  :1' />..        
-0000d340: 2020 2020 2020 2020 3c2f 7379 6d62 6f6c          </symbol
-0000d350: 3e0d 0a20 2020 2020 2020 2020 2020 2020  >..             
-0000d360: 2020 203c 7379 6d62 6f6c 2069 643d 276f     <symbol id='o
-0000d370: 7262 3132 3027 3e0d 0a20 2020 2020 2020  rb120'>..       
-0000d380: 2020 2020 2020 2020 2020 2020 203c 7061               <pa
-0000d390: 7468 2064 3d27 4d20 312e 3137 3535 3031  th d='M 1.175501
-0000d3a0: 312c 392e 3439 3739 3733 2043 2039 2e30  1,9.497973 C 9.0
-0000d3b0: 3935 3738 3639 2c39 2e34 3937 3937 3320  957869,9.497973 
-0000d3c0: 392e 3039 3537 3836 392c 392e 3439 3739  9.0957869,9.4979
-0000d3d0: 3733 2039 2e30 3935 3738 3639 2c39 2e34  73 9.0957869,9.4
-0000d3e0: 3937 3937 3320 4c20 352e 3133 3536 3433  97973 L 5.135643
-0000d3f0: 382c 312e 3436 3339 3036 3320 4320 352e  8,1.4639063 C 5.
-0000d400: 3133 3536 3433 382c 312e 3436 3339 3036  1356438,1.463906
-0000d410: 3320 352e 3133 3536 3433 382c 312e 3436  3 5.1356438,1.46
-0000d420: 3339 3036 3320 312e 3137 3535 3031 312c  39063 1.1755011,
-0000d430: 392e 3439 3739 3733 207a 2720 7374 796c  9.497973 z' styl
-0000d440: 653d 2766 696c 6c3a 6e6f 6e65 3b66 696c  e='fill:none;fil
-0000d450: 6c2d 7275 6c65 3a65 7665 6e6f 6464 3b73  l-rule:evenodd;s
-0000d460: 7472 6f6b 653a 2024 6f72 625f 636f 6c6f  troke: $orb_colo
-0000d470: 725f 3132 303b 7374 726f 6b65 2d77 6964  r_120;stroke-wid
-0000d480: 7468 3a31 2e31 3936 3534 3632 3b73 7472  th:1.1965462;str
-0000d490: 6f6b 652d 6c69 6e65 6361 703a 6275 7474  oke-linecap:butt
-0000d4a0: 3b73 7472 6f6b 652d 6c69 6e65 6a6f 696e  ;stroke-linejoin
-0000d4b0: 3a6d 6974 6572 3b73 7472 6f6b 652d 6d69  :miter;stroke-mi
-0000d4c0: 7465 726c 696d 6974 3a34 3b73 7472 6f6b  terlimit:4;strok
-0000d4d0: 652d 6461 7368 6172 7261 793a 6e6f 6e65  e-dasharray:none
-0000d4e0: 3b73 7472 6f6b 652d 6f70 6163 6974 793a  ;stroke-opacity:
-0000d4f0: 3127 202f 3e0d 0a20 2020 2020 2020 2020  1' />..         
-0000d500: 2020 2020 2020 203c 2f73 796d 626f 6c3e         </symbol>
-0000d510: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000d520: 2020 3c73 796d 626f 6c20 6964 3d27 6f72    <symbol id='or
-0000d530: 6231 3335 273e 0d0a 2020 2020 2020 2020  b135'>..        
-0000d540: 2020 2020 2020 2020 2020 2020 3c70 6174              <pat
-0000d550: 6820 643d 274d 2032 2e32 3338 3835 3832  h d='M 2.2388582
-0000d560: 2c31 2e37 3135 3639 3934 204c 2039 2e32  ,1.7156994 L 9.2
-0000d570: 3933 3831 3534 2c31 2e37 3135 3639 3934  938154,1.7156994
-0000d580: 204c 2039 2e32 3933 3831 3534 2c37 2e37   L 9.2938154,7.7
-0000d590: 3831 3138 3237 204c 2032 2e32 3338 3835  811827 L 2.23885
-0000d5a0: 3832 2c37 2e37 3831 3138 3237 204c 2032  82,7.7811827 L 2
-0000d5b0: 2e32 3338 3835 3832 2c31 2e37 3135 3639  .2388582,1.71569
-0000d5c0: 3934 207a 204d 2036 2e38 3436 3131 3034  94 z M 6.8461104
-0000d5d0: 2c35 2e35 3733 3432 3637 2043 2036 2e38  ,5.5734267 C 6.8
-0000d5e0: 3436 3131 3034 2c35 2e35 3733 3432 3637  461104,5.5734267
-0000d5f0: 2036 2e38 3436 3131 3034 2c35 2e35 3733   6.8461104,5.573
-0000d600: 3432 3637 2033 2e32 3436 3836 3532 2c31  4267 3.2468652,1
-0000d610: 302e 3337 3234 3220 4320 382e 3034 3538  0.37242 C 8.0458
-0000d620: 3538 342c 3130 2e33 3732 3432 2038 2e30  584,10.37242 8.0
-0000d630: 3435 3835 3834 2c31 302e 3337 3234 3220  458584,10.37242 
-0000d640: 382e 3034 3538 3538 342c 3130 2e33 3732  8.0458584,10.372
-0000d650: 3432 2720 7374 796c 653d 2766 696c 6c3a  42' style='fill:
-0000d660: 6e6f 6e65 3b66 696c 6c2d 7275 6c65 3a65  none;fill-rule:e
-0000d670: 7665 6e6f 6464 3b73 7472 6f6b 653a 2024  venodd;stroke: $
-0000d680: 6f72 625f 636f 6c6f 725f 3133 353b 7374  orb_color_135;st
-0000d690: 726f 6b65 2d77 6964 7468 3a31 2e31 3936  roke-width:1.196
-0000d6a0: 3534 3632 3b73 7472 6f6b 652d 6c69 6e65  5462;stroke-line
-0000d6b0: 6361 703a 6275 7474 3b73 7472 6f6b 652d  cap:butt;stroke-
-0000d6c0: 6c69 6e65 6a6f 696e 3a6d 6974 6572 3b73  linejoin:miter;s
-0000d6d0: 7472 6f6b 652d 6d69 7465 726c 696d 6974  troke-miterlimit
-0000d6e0: 3a34 3b73 7472 6f6b 652d 6461 7368 6172  :4;stroke-dashar
-0000d6f0: 7261 793a 6e6f 6e65 3b73 7472 6f6b 652d  ray:none;stroke-
-0000d700: 6f70 6163 6974 793a 3127 202f 3e0d 0a20  opacity:1' />.. 
-0000d710: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-0000d720: 2f73 796d 626f 6c3e 0d0a 2020 2020 2020  /symbol>..      
-0000d730: 2020 2020 2020 2020 2020 3c73 796d 626f            <symbo
-0000d740: 6c20 6964 3d27 6f72 6231 3434 273e 0d0a  l id='orb144'>..
-0000d750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d760: 2020 2020 3c70 6174 6820 643d 274d 2031      <path d='M 1
-0000d770: 2e34 3234 3531 3639 2c31 2e32 3936 3835  .4245169,1.29685
-0000d780: 3938 2043 2031 2e34 3234 3531 3639 2c39  98 C 1.4245169,9
-0000d790: 2e36 3736 3331 3239 2031 2e34 3234 3531  .6763129 1.42451
-0000d7a0: 3639 2c39 2e36 3736 3331 3239 2031 2e34  69,9.6763129 1.4
-0000d7b0: 3234 3531 3639 2c39 2e36 3736 3331 3239  245169,9.6763129
-0000d7c0: 204d 2031 2e39 3230 3833 3331 2c35 2e33   M 1.9208331,5.3
-0000d7d0: 3836 3832 3739 2043 2032 2e37 3732 3238  868279 C 2.77228
-0000d7e0: 3836 2c35 2e33 3335 3234 3339 2033 2e35  86,5.3352439 3.5
-0000d7f0: 3534 3135 3533 2c35 2e36 3836 3431 3239  541553,5.6864129
-0000d800: 2033 2e39 3336 3532 3337 2c36 2e32 3932   3.9365237,6.292
-0000d810: 3135 3639 2043 2034 2e33 3138 3839 322c  1569 C 4.318892,
-0000d820: 362e 3839 3739 3030 3920 342e 3233 3531  6.8979009 4.2351
-0000d830: 3631 342c 372e 3635 3237 3132 3920 332e  614,7.6527129 3.
-0000d840: 3732 3036 3632 322c 382e 3233 3830 3938  7206622,8.238098
-0000d850: 3920 4320 332e 3230 3631 3633 322c 382e  9 C 3.2061632,8.
-0000d860: 3832 3334 3834 3920 322e 3335 3035 3130  8234849 2.350510
-0000d870: 312c 392e 3133 3734 3832 3920 312e 3531  1,9.1374829 1.51
-0000d880: 3437 3437 312c 392e 3034 3736 3031 3920  47471,9.0476019 
-0000d890: 4d20 392e 3835 3238 3633 392c 352e 3538  M 9.8528639,5.58
-0000d8a0: 3531 3234 3920 4320 392e 3835 3330 3434  51249 C 9.853044
-0000d8b0: 392c 372e 3437 3933 3431 3920 382e 3836  9,7.4793419 8.86
-0000d8c0: 3439 3639 392c 392e 3031 3530 3537 3920  49699,9.0150579 
-0000d8d0: 372e 3634 3630 3533 392c 392e 3031 3530  7.6460539,9.0150
-0000d8e0: 3537 3920 4320 362e 3432 3731 3338 392c  579 C 6.4271389,
-0000d8f0: 392e 3031 3530 3537 3920 352e 3433 3930  9.0150579 5.4390
-0000d900: 3632 392c 372e 3437 3933 3431 3920 352e  629,7.4793419 5.
-0000d910: 3433 3932 3434 392c 352e 3538 3531 3234  4392449,5.585124
-0000d920: 3920 4320 352e 3433 3930 3632 392c 332e  9 C 5.4390629,3.
-0000d930: 3639 3039 3038 3820 362e 3432 3731 3338  6909088 6.427138
-0000d940: 392c 322e 3135 3531 3932 3820 372e 3634  9,2.1551928 7.64
-0000d950: 3630 3533 392c 322e 3135 3531 3932 3820  60539,2.1551928 
-0000d960: 4320 382e 3836 3439 3639 392c 322e 3135  C 8.8649699,2.15
-0000d970: 3531 3932 3820 392e 3835 3330 3434 392c  51928 9.8530449,
-0000d980: 332e 3639 3039 3038 3820 392e 3835 3238  3.6909088 9.8528
-0000d990: 3633 392c 352e 3538 3531 3234 3920 7a20  639,5.5851249 z 
-0000d9a0: 4d20 382e 3235 3830 3434 392c 372e 3236  M 8.2580449,7.26
-0000d9b0: 3237 3935 3920 4320 3130 2e31 3938 3235  27959 C 10.19825
-0000d9c0: 362c 392e 3938 3033 3637 3920 3130 2e31  6,9.9803679 10.1
-0000d9d0: 3938 3235 362c 392e 3938 3033 3637 3920  98256,9.9803679 
-0000d9e0: 3130 2e31 3938 3235 362c 392e 3938 3033  10.198256,9.9803
-0000d9f0: 3637 3927 2073 7479 6c65 3d27 6f70 6163  679' style='opac
-0000da00: 6974 793a 313b 6669 6c6c 3a6e 6f6e 653b  ity:1;fill:none;
-0000da10: 6669 6c6c 2d6f 7061 6369 7479 3a31 3b66  fill-opacity:1;f
-0000da20: 696c 6c2d 7275 6c65 3a6e 6f6e 7a65 726f  ill-rule:nonzero
-0000da30: 3b73 7472 6f6b 653a 2024 6f72 625f 636f  ;stroke: $orb_co
-0000da40: 6c6f 725f 3134 343b 7374 726f 6b65 2d77  lor_144;stroke-w
-0000da50: 6964 7468 3a31 2e34 3736 3333 3036 343b  idth:1.47633064;
-0000da60: 7374 726f 6b65 2d6c 696e 6563 6170 3a62  stroke-linecap:b
-0000da70: 7574 743b 7374 726f 6b65 2d6c 696e 656a  utt;stroke-linej
-0000da80: 6f69 6e3a 6d69 7465 723b 7374 726f 6b65  oin:miter;stroke
-0000da90: 2d6d 6974 6572 6c69 6d69 743a 343b 7374  -miterlimit:4;st
-0000daa0: 726f 6b65 2d64 6173 6861 7272 6179 3a6e  roke-dasharray:n
-0000dab0: 6f6e 653b 7374 726f 6b65 2d6f 7061 6369  one;stroke-opaci
-0000dac0: 7479 3a31 2720 2f3e 0d0a 2020 2020 2020  ty:1' />..      
-0000dad0: 2020 2020 2020 2020 2020 3c2f 7379 6d62            </symb
-0000dae0: 6f6c 3e0d 0a20 2020 2020 2020 2020 2020  ol>..           
-0000daf0: 2020 2020 203c 7379 6d62 6f6c 2069 643d       <symbol id=
-0000db00: 276f 7262 3135 3027 3e0d 0a20 2020 2020  'orb150'>..     
-0000db10: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-0000db20: 7061 7468 2064 3d27 4d20 312e 3137 3731  path d='M 1.1771
-0000db30: 3437 362c 332e 3833 3635 3532 3220 4320  476,3.8365522 C 
-0000db40: 342e 3638 3731 3032 2c33 2e38 3237 3239  4.687102,3.82729
-0000db50: 3336 2038 2e31 3937 3035 3632 2c33 2e38  36 8.1970562,3.8
-0000db60: 3138 3033 3533 2031 312e 3730 3730 3131  180353 11.707011
-0000db70: 2c33 2e38 3038 3737 3637 204d 2031 302e  ,3.8087767 M 10.
-0000db80: 3937 3235 3739 2c39 2e32 3130 3833 3431  972579,9.2108341
-0000db90: 2043 2039 2e33 3339 3830 3032 2c37 2e34   C 9.3398002,7.4
-0000dba0: 3936 3431 3631 2037 2e37 3037 3032 3232  964161 7.7070222
-0000dbb0: 2c35 2e37 3831 3939 3839 2036 2e30 3734  ,5.7819989 6.074
-0000dbc0: 3234 3334 2c34 2e30 3637 3538 3133 204d  2434,4.0675813 M
-0000dbd0: 2031 2e36 3635 3734 312c 392e 3231 3038   1.665741,9.2108
-0000dbe0: 3334 3120 4320 332e 3139 3038 3635 362c  341 C 3.1908656,
-0000dbf0: 372e 3339 3939 3831 3120 342e 3731 3539  7.3999811 4.7159
-0000dc00: 3930 342c 352e 3538 3931 3237 3920 362e  904,5.5891279 6.
-0000dc10: 3234 3131 3135 2c33 2e37 3738 3237 3438  241115,3.7782748
-0000dc20: 2720 7374 796c 653d 276f 7061 6369 7479  ' style='opacity
-0000dc30: 3a31 3b66 696c 6c3a 6e6f 6e65 3b66 696c  :1;fill:none;fil
-0000dc40: 6c2d 6f70 6163 6974 793a 313b 6669 6c6c  l-opacity:1;fill
-0000dc50: 2d72 756c 653a 6e6f 6e7a 6572 6f3b 7374  -rule:nonzero;st
-0000dc60: 726f 6b65 3a20 246f 7262 5f63 6f6c 6f72  roke: $orb_color
-0000dc70: 5f31 3530 3b73 7472 6f6b 652d 7769 6474  _150;stroke-widt
-0000dc80: 683a 312e 3437 3633 3330 3634 3b73 7472  h:1.47633064;str
-0000dc90: 6f6b 652d 6c69 6e65 6361 703a 6275 7474  oke-linecap:butt
-0000dca0: 3b73 7472 6f6b 652d 6c69 6e65 6a6f 696e  ;stroke-linejoin
-0000dcb0: 3a6d 6974 6572 3b73 7472 6f6b 652d 6d69  :miter;stroke-mi
-0000dcc0: 7465 726c 696d 6974 3a34 3b73 7472 6f6b  terlimit:4;strok
-0000dcd0: 652d 6461 7368 6172 7261 793a 6e6f 6e65  e-dasharray:none
-0000dce0: 3b73 7472 6f6b 652d 6f70 6163 6974 793a  ;stroke-opacity:
-0000dcf0: 3127 202f 3e0d 0a20 2020 2020 2020 2020  1' />..         
-0000dd00: 2020 2020 2020 203c 2f73 796d 626f 6c3e         </symbol>
-0000dd10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000dd20: 2020 3c73 796d 626f 6c20 6964 3d27 6f72    <symbol id='or
-0000dd30: 6231 3830 273e 0d0a 2020 2020 2020 2020  b180'>..        
-0000dd40: 2020 2020 2020 2020 2020 2020 3c70 6174              <pat
-0000dd50: 6820 643d 274d 2035 2e32 3436 3431 3337  h d='M 5.2464137
-0000dd60: 2c39 2e31 3032 3431 3134 2043 2035 2e32  ,9.1024114 C 5.2
-0000dd70: 3630 3736 3637 2c31 302e 3032 3331 3320  607667,10.02313 
-0000dd80: 342e 3634 3234 3034 372c 3130 2e39 3131  4.6424047,10.911
-0000dd90: 3735 3620 332e 3737 3637 3636 372c 3131  756 3.7767667,11
-0000dda0: 2e32 3233 3733 3520 4320 332e 3030 3433  .223735 C 3.0043
-0000ddb0: 3030 372c 3131 2e35 3134 3532 3220 322e  007,11.514522 2.
-0000ddc0: 3037 3536 3930 372c 3131 2e33 3435 3731  0756907,11.34571
-0000ddd0: 3320 312e 3436 3738 3136 372c 3130 2e37  3 1.4678167,10.7
-0000dde0: 3832 3838 3620 4320 302e 3837 3036 3238  82886 C 0.870628
-0000ddf0: 3637 2c31 302e 3234 3734 3620 302e 3539  67,10.24746 0.59
-0000de00: 3037 3530 3637 2c39 2e33 3831 3830 3932  075067,9.3818092
-0000de10: 2030 2e37 3737 3037 3536 372c 382e 3539   0.77707567,8.59
-0000de20: 3935 3631 3420 4320 302e 3935 3837 3238  95614 C 0.958728
-0000de30: 3637 2c37 2e37 3932 3038 3433 2031 2e36  67,7.7920843 1.6
-0000de40: 3132 3535 3537 2c37 2e31 3037 3434 3334  125557,7.1074434
-0000de50: 2032 2e34 3139 3431 3537 2c36 2e39 3039   2.4194157,6.909
-0000de60: 3932 3035 2043 2033 2e31 3930 3036 3237  9205 C 3.1900627
-0000de70: 2c36 2e37 3130 3638 2034 2e30 3632 3133  ,6.71068 4.06213
-0000de80: 3137 2c36 2e39 3435 3439 3636 2034 2e36  17,6.9454966 4.6
-0000de90: 3130 3038 3737 2c37 2e35 3238 3130 3538  100877,7.5281058
-0000dea0: 2043 2035 2e30 3132 3935 3537 2c37 2e39   C 5.0129557,7.9
-0000deb0: 3435 3335 3136 2035 2e32 3531 3739 3437  453516 5.2517947
-0000dec0: 2c38 2e35 3231 3031 3934 2035 2e32 3436  ,8.5210194 5.246
-0000ded0: 3431 3337 2c39 2e31 3032 3431 3134 207a  4137,9.1024114 z
-0000dee0: 204d 2031 312e 3234 3634 3134 2c33 2e31   M 11.246414,3.1
-0000def0: 3032 3431 3239 2043 2031 312e 3236 3037  024129 C 11.2607
-0000df00: 3635 2c34 2e30 3233 3133 3137 2031 302e  65,4.0231317 10.
-0000df10: 3634 3234 3034 2c34 2e39 3131 3735 3734  642404,4.9117574
-0000df20: 2039 2e37 3736 3736 3537 2c35 2e32 3233   9.7767657,5.223
-0000df30: 3733 3631 2043 2039 2e30 3034 3239 3937  7361 C 9.0042997
-0000df40: 2c35 2e35 3134 3532 3338 2038 2e30 3735  ,5.5145238 8.075
-0000df50: 3638 3937 2c35 2e33 3435 3731 3335 2037  6897,5.3457135 7
-0000df60: 2e34 3637 3831 3437 2c34 2e37 3832 3838  .4678147,4.78288
-0000df70: 3733 2043 2036 2e38 3730 3632 3737 2c34  73 C 6.8706277,4
-0000df80: 2e32 3437 3436 3133 2036 2e35 3930 3734  .2474613 6.59074
-0000df90: 3937 2c33 2e33 3831 3831 2036 2e37 3737  97,3.38181 6.777
-0000dfa0: 3037 3437 2c32 2e35 3939 3536 3234 2043  0747,2.5995624 C
-0000dfb0: 2036 2e39 3538 3732 3637 2c31 2e37 3932   6.9587267,1.792
-0000dfc0: 3038 3533 2037 2e36 3132 3535 3437 2c31  0853 7.6125547,1
-0000dfd0: 2e31 3037 3434 3435 2038 2e34 3139 3431  .1074445 8.41941
-0000dfe0: 3437 2c30 2e39 3039 3932 3135 2043 2039  47,0.9099215 C 9
-0000dff0: 2e31 3930 3036 3137 2c30 2e37 3130 3638  .1900617,0.71068
-0000e000: 3132 2031 302e 3036 3231 332c 302e 3934  12 10.06213,0.94
-0000e010: 3534 3938 3220 3130 2e36 3130 3038 372c  54982 10.610087,
-0000e020: 312e 3532 3831 3037 3320 4320 3131 2e30  1.5281073 C 11.0
-0000e030: 3132 3935 352c 312e 3934 3533 3532 3920  12955,1.9453529 
-0000e040: 3131 2e32 3531 3739 342c 322e 3532 3130  11.251794,2.5210
-0000e050: 3230 3620 3131 2e32 3436 3431 342c 332e  206 11.246414,3.
-0000e060: 3130 3234 3132 3920 7a20 4d20 342e 3530  1024129 z M 4.50
-0000e070: 3832 3439 372c 372e 3537 3837 3433 2043  82497,7.578743 C
-0000e080: 2035 2e35 3334 3835 3337 2c36 2e35 3934   5.5348537,6.594
-0000e090: 3532 3236 2036 2e35 3631 3435 3737 2c35  5226 6.5614577,5
-0000e0a0: 2e36 3130 3330 3232 2037 2e35 3838 3036  .6103022 7.58806
-0000e0b0: 3137 2c34 2e36 3236 3038 3138 2720 7374  17,4.6260818' st
-0000e0c0: 796c 653d 276f 7061 6369 7479 3a31 3b66  yle='opacity:1;f
-0000e0d0: 696c 6c3a 6e6f 6e65 3b66 696c 6c2d 6f70  ill:none;fill-op
-0000e0e0: 6163 6974 793a 313b 6669 6c6c 2d72 756c  acity:1;fill-rul
-0000e0f0: 653a 6e6f 6e7a 6572 6f3b 7374 726f 6b65  e:nonzero;stroke
-0000e100: 3a20 246f 7262 5f63 6f6c 6f72 5f31 3830  : $orb_color_180
-0000e110: 3b73 7472 6f6b 652d 7769 6474 683a 312e  ;stroke-width:1.
-0000e120: 3437 3633 3330 3634 3b73 7472 6f6b 652d  47633064;stroke-
-0000e130: 6c69 6e65 6361 703a 6275 7474 3b73 7472  linecap:butt;str
-0000e140: 6f6b 652d 6c69 6e65 6a6f 696e 3a6d 6974  oke-linejoin:mit
-0000e150: 6572 3b73 7472 6f6b 652d 6d69 7465 726c  er;stroke-miterl
-0000e160: 696d 6974 3a34 3b73 7472 6f6b 652d 6461  imit:4;stroke-da
-0000e170: 7368 6172 7261 793a 6e6f 6e65 3b73 7472  sharray:none;str
-0000e180: 6f6b 652d 6f70 6163 6974 793a 3127 202f  oke-opacity:1' /
-0000e190: 3e0d 0a20 2020 2020 2020 2020 2020 2020  >..             
-0000e1a0: 2020 203c 2f73 796d 626f 6c3e 2020 2020     </symbol>    
-0000e1b0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-0000e1c0: 2020 2020 2020 2020 2020 2020 2020 3c21                <!
-0000e1d0: 2d2d 2072 6574 726f 6772 6164 6520 7379  -- retrograde sy
-0000e1e0: 6d62 6f6c 2028 3132 7831 3229 202d 2d3e  mbol (12x12) -->
-0000e1f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000e200: 2020 3c73 796d 626f 6c20 6964 3d27 7265    <symbol id='re
-0000e210: 7472 6f67 7261 6465 273e 0d0a 2020 2020  trograde'>..    
-0000e220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e230: 3c70 6174 6820 643d 274d 2035 2e31 3639  <path d='M 5.169
-0000e240: 3530 3839 2c30 2e30 3635 3134 3330 3720  5089,0.06514307 
-0000e250: 4320 332e 3735 3937 3938 392c 302e 3231  C 3.7597989,0.21
-0000e260: 3539 3732 3037 2032 2e33 3331 3733 3439  597207 2.3317349
-0000e270: 2c30 2e33 3331 3439 3030 3720 302e 3931  ,0.33149007 0.91
-0000e280: 3335 3831 3931 2c30 2e32 3335 3133 3130  358191,0.2351310
-0000e290: 3720 4320 312e 3534 3930 3332 392c 302e  7 C 1.5490329,0.
-0000e2a0: 3831 3930 3232 3037 2031 2e34 3032 3438  81902207 1.40248
-0000e2b0: 3439 2c31 2e37 3130 3030 3131 2031 2e34  49,1.7100011 1.4
-0000e2c0: 3232 3833 3739 2c32 2e34 3730 3034 3331  228379,2.4700431
-0000e2d0: 2043 2031 2e34 3137 3431 3539 2c35 2e32   C 1.4174159,5.2
-0000e2e0: 3137 3434 3831 2031 2e34 3333 3737 3039  174481 1.4337709
-0000e2f0: 2c37 2e39 3635 3237 3331 2031 2e34 3134  ,7.9652731 1.414
-0000e300: 3530 3139 2c31 302e 3731 3234 3131 2043  5019,10.712411 C
-0000e310: 2031 2e35 3134 3934 3039 2c31 312e 3137   1.5149409,11.17
-0000e320: 3038 3438 2030 2e39 3637 3939 3739 312c  0848 0.96799791,
-0000e330: 3131 2e38 3334 3437 3120 302e 3930 3238  11.834471 0.9028
-0000e340: 3436 3931 2c31 312e 3936 3433 3032 2043  4691,11.964302 C
-0000e350: 2031 2e39 3937 3638 3839 2c31 312e 3936   1.9976889,11.96
-0000e360: 3433 3032 2033 2e30 3932 3532 3939 2c31  4302 3.0925299,1
-0000e370: 312e 3936 3433 3032 2034 2e31 3837 3337  1.964302 4.18737
-0000e380: 3139 2c31 312e 3936 3433 3032 2043 2033  19,11.964302 C 3
-0000e390: 2e36 3031 3834 3339 2c31 312e 3537 3739  .6018439,11.5779
-0000e3a0: 3735 2033 2e36 3531 3039 3239 2c31 302e  75 3.6510929,10.
-0000e3b0: 3832 3030 3334 2033 2e36 3431 3733 3939  820034 3.6417399
-0000e3c0: 2c31 302e 3231 3938 3338 2043 2033 2e36  ,10.219838 C 3.6
-0000e3d0: 3431 3733 3939 2c38 2e38 3937 3436 3031  417399,8.8974601
-0000e3e0: 2033 2e36 3431 3733 3939 2c37 2e35 3735   3.6417399,7.575
-0000e3f0: 3038 3331 2033 2e36 3431 3733 3939 2c36  0831 3.6417399,6
-0000e400: 2e32 3532 3730 3531 2043 2034 2e35 3032  .2527051 C 4.502
-0000e410: 3632 3539 2c37 2e33 3937 3239 3131 2035  6259,7.3972911 5
-0000e420: 2e33 3633 3531 3039 2c38 2e35 3431 3837  .3635109,8.54187
-0000e430: 3731 2036 2e32 3234 3339 3539 2c39 2e36  71 6.2243959,9.6
-0000e440: 3836 3436 3331 2043 2035 2e36 3033 3036  864631 C 5.60306
-0000e450: 3939 2c31 302e 3031 3330 3439 2035 2e30  99,10.013049 5.0
-0000e460: 3732 3134 3339 2c31 302e 3439 3733 3534  721439,10.497354
-0000e470: 2034 2e33 3639 3234 3839 2c31 302e 3637   4.3692489,10.67
-0000e480: 3233 3933 2043 2034 2e35 3735 3337 3639  2393 C 4.5753769
-0000e490: 2c31 302e 3935 3537 3036 2034 2e37 3831  ,10.955706 4.781
-0000e4a0: 3530 3339 2c31 312e 3233 3930 3220 342e  5039,11.23902 4.
-0000e4b0: 3938 3736 3331 392c 3131 2e35 3232 3333  9876319,11.52233
-0000e4c0: 3320 4320 352e 3439 3339 3231 392c 3131  3 C 5.4939219,11
-0000e4d0: 2e30 3138 3033 3620 362e 3134 3236 3338  .018036 6.142638
-0000e4e0: 392c 3130 2e36 3732 3231 3820 362e 3733  9,10.672218 6.73
-0000e4f0: 3336 3532 392c 3130 2e32 3634 3432 3120  36529,10.264421 
-0000e500: 4320 372e 3338 3937 3033 392c 3131 2e32  C 7.3897039,11.2
-0000e510: 3136 3931 3220 382e 3436 3937 3437 392c  16912 8.4697479,
-0000e520: 3132 2e30 3438 3339 3220 392e 3734 3139  12.048392 9.7419
-0000e530: 3339 392c 3132 2e30 3131 3537 3920 4320  399,12.011579 C 
-0000e540: 3130 2e31 3433 3630 332c 3132 2e30 3032  10.143603,12.002
-0000e550: 3139 3920 3131 2e30 3637 3639 312c 3131  199 11.067691,11
-0000e560: 2e38 3835 3832 3420 3131 2e30 3633 3737  .885824 11.06377
-0000e570: 352c 3131 2e36 3736 3037 3520 4320 392e  5,11.676075 C 9.
-0000e580: 3930 3034 3936 392c 3131 2e31 3238 3035  9004969,11.12805
-0000e590: 3420 392e 3030 3138 3834 392c 3130 2e31  4 9.0018849,10.1
-0000e5a0: 3739 3038 3520 382e 3430 3639 3232 392c  79085 8.4069229,
-0000e5b0: 392e 3130 3835 3034 3120 4320 382e 3936  9.1085041 C 8.96
-0000e5c0: 3730 3433 392c 382e 3637 3536 3634 3120  70439,8.6756641 
-0000e5d0: 392e 3530 3536 3238 392c 382e 3138 3730  9.5056289,8.1870
-0000e5e0: 3035 3120 3130 2e31 3737 3338 322c 372e  051 10.177382,7.
-0000e5f0: 3930 3836 3733 3120 4320 3130 2e34 3139  9086731 C 10.419
-0000e600: 3838 312c 372e 3836 3631 3530 3120 3130  881,7.8661501 10
-0000e610: 2e30 3331 3636 382c 372e 3537 3633 3537  .031668,7.576357
-0000e620: 3120 392e 3938 3135 3033 392c 372e 3431  1 9.9815039,7.41
-0000e630: 3930 3935 3120 4320 392e 3738 3936 3038  90951 C 9.789608
-0000e640: 392c 362e 3930 3632 3933 3120 392e 3632  9,6.9062931 9.62
-0000e650: 3134 3337 392c 372e 3436 3934 3636 3120  14379,7.4694661 
-0000e660: 392e 3239 3530 3833 392c 372e 3632 3339  9.2950839,7.6239
-0000e670: 3435 3120 4320 382e 3834 3533 3938 392c  451 C 8.8453989,
-0000e680: 372e 3839 3237 3638 3120 382e 3330 3738  7.8927681 8.3078
-0000e690: 3833 392c 382e 3336 3436 3031 3120 372e  839,8.3646011 7.
-0000e6a0: 3836 3134 3435 392c 382e 3434 3534 3335  8614459,8.445435
-0000e6b0: 3120 4320 372e 3235 3531 3336 392c 372e  1 C 7.2551369,7.
-0000e6c0: 3538 3938 3637 3120 362e 3634 3838 3237  5898671 6.648827
-0000e6d0: 392c 362e 3733 3432 3939 3120 362e 3034  9,6.7342991 6.04
-0000e6e0: 3235 3139 392c 352e 3837 3837 3332 3120  25199,5.8787321 
-0000e6f0: 4320 372e 3234 3531 3933 392c 352e 3631  C 7.2451939,5.61
-0000e700: 3734 3335 3120 382e 3538 3237 3833 392c  74351 8.5827839,
-0000e710: 352e 3038 3533 3839 3120 392e 3037 3034  5.0853891 9.0704
-0000e720: 3430 392c 332e 3933 3638 3938 3120 4320  409,3.9368981 C 
-0000e730: 392e 3430 3633 3133 392c 332e 3131 3230  9.4063139,3.1120
-0000e740: 3231 3120 392e 3236 3337 3333 392c 322e  211 9.2637339,2.
-0000e750: 3136 3637 3933 3120 382e 3931 3037 3838  1667931 8.910788
-0000e760: 392c 312e 3337 3334 3730 3120 4320 382e  9,1.3734701 C 8.
-0000e770: 3136 3834 3836 392c 302e 3431 3039 3131  1684869,0.410911
-0000e780: 3037 2036 2e38 3639 3230 3439 2c2d 302e  07 6.8692049,-0.
-0000e790: 3037 3234 3531 3933 3120 352e 3631 3939  072451931 5.6199
-0000e7a0: 3732 392c 302e 3032 3531 3036 3037 2043  729,0.02510607 C
-0000e7b0: 2035 2e34 3639 3332 3739 2c30 2e30 3332   5.4693279,0.032
-0000e7c0: 3837 3230 3720 352e 3331 3930 3531 392c  87207 5.3190519,
-0000e7d0: 302e 3034 3635 3130 3037 2035 2e31 3639  0.04651007 5.169
-0000e7e0: 3530 3839 2c30 2e30 3635 3134 3330 3720  5089,0.06514307 
-0000e7f0: 4c20 352e 3136 3935 3038 392c 302e 3036  L 5.1695089,0.06
-0000e800: 3531 3433 3037 207a 204d 2034 2e30 3035  514307 z M 4.005
-0000e810: 3439 3439 2c30 2e39 3833 3037 3830 3620  4949,0.98307806 
-0000e820: 4320 342e 3932 3734 3230 392c 302e 3837  C 4.9274209,0.87
-0000e830: 3531 3630 3037 2036 2e30 3735 3238 3339  516007 6.0752839
-0000e840: 2c30 2e39 3536 3539 3430 3620 362e 3631  ,0.95659406 6.61
-0000e850: 3139 3436 392c 312e 3737 3639 3832 3120  19469,1.7769821 
-0000e860: 4320 372e 3139 3935 3438 392c 322e 3734  C 7.1995489,2.74
-0000e870: 3336 3233 3120 362e 3937 3731 3737 392c  36231 6.9771779,
-0000e880: 342e 3032 3737 3234 3120 362e 3233 3838  4.0277241 6.2388
-0000e890: 3835 392c 342e 3836 3934 3030 3120 4320  859,4.8694001 C 
-0000e8a0: 352e 3630 3533 3238 392c 352e 3535 3439  5.6053289,5.5549
-0000e8b0: 3033 3120 342e 3535 3231 3035 392c 352e  031 4.5521059,5.
-0000e8c0: 3637 3830 3737 3120 332e 3634 3137 3339  6780771 3.641739
-0000e8d0: 392c 352e 3537 3237 3533 3120 4320 332e  9,5.5727531 C 3.
-0000e8e0: 3634 3137 3339 392c 342e 3036 3535 3237  6417399,4.065527
-0000e8f0: 3120 332e 3634 3137 3339 392c 322e 3535  1 3.6417399,2.55
-0000e900: 3833 3030 3120 332e 3634 3137 3339 392c  83001 3.6417399,
-0000e910: 312e 3035 3130 3733 3120 4320 332e 3736  1.0510731 C 3.76
-0000e920: 3239 3931 392c 312e 3032 3834 3038 3120  29919,1.0284081 
-0000e930: 332e 3838 3432 3432 392c 312e 3030 3537  3.8842429,1.0057
-0000e940: 3433 3120 342e 3030 3534 3934 392c 302e  431 4.0054949,0.
-0000e950: 3938 3330 3738 3036 207a 2720 7374 796c  98307806 z' styl
-0000e960: 653d 2766 696c 6c3a 2470 6170 6572 5f63  e='fill:$paper_c
-0000e970: 6f6c 6f72 5f30 3b27 202f 3e0d 0a20 2020  olor_0;' />..   
-0000e980: 2020 2020 2020 2020 2020 2020 203c 2f73               </s
-0000e990: 796d 626f 6c3e 0d0a 2020 2020 2020 2020  ymbol>..        
-0000e9a0: 2020 2020 2020 2020 3c67 2074 7261 6e73          <g trans
-0000e9b0: 666f 726d 3d27 7472 616e 736c 6174 6528  form='translate(
-0000e9c0: 3530 2c35 3029 273e 0d0a 2020 2020 2020  50,50)'>..      
-0000e9d0: 2020 2020 2020 2020 2020 2020 2020 3c67                <g
-0000e9e0: 2074 7261 6e73 666f 726d 3d27 7472 616e   transform='tran
-0000e9f0: 736c 6174 6528 2463 6972 636c 6558 2c24  slate($circleX,$
-0000ea00: 6369 7263 6c65 5929 273e 2020 2020 2020  circleY)'>      
+00000890: 2020 203c 6369 7263 6c65 2063 783d 2732     <circle cx='2
+000008a0: 3027 2063 793d 2731 3027 2072 3d27 3130  0' cy='10' r='10
+000008b0: 2720 7374 796c 653d 2766 696c 6c3a 2024  ' style='fill: $
+000008c0: 6c75 6e61 725f 7068 6173 655f 6267 3b27  lunar_phase_bg;'
+000008d0: 202f 3e0d 0a20 2020 2020 2020 2020 2020   />..           
+000008e0: 2020 2020 2020 2020 2020 2020 203c 6369               <ci
+000008f0: 7263 6c65 2063 783d 2724 6c75 6e61 725f  rcle cx='$lunar_
+00000900: 7068 6173 655f 6378 2720 6379 3d27 3130  phase_cx' cy='10
+00000910: 2720 723d 2724 6c75 6e61 725f 7068 6173  ' r='$lunar_phas
+00000920: 655f 7227 2073 7479 6c65 3d27 6669 6c6c  e_r' style='fill
+00000930: 3a20 246c 756e 6172 5f70 6861 7365 5f66  : $lunar_phase_f
+00000940: 6727 2063 6c69 702d 7061 7468 3d27 7572  g' clip-path='ur
+00000950: 6c28 2363 7574 2d6f 6666 2d63 6972 636c  l(#cut-off-circl
+00000960: 6529 2720 2f3e 0d0a 2020 2020 2020 2020  e)' />..        
+00000970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000980: 3c63 6972 636c 6520 6378 3d27 3230 2720  <circle cx='20' 
+00000990: 6379 3d27 3130 2720 723d 2731 3027 2073  cy='10' r='10' s
+000009a0: 7479 6c65 3d27 6669 6c6c 3a20 6e6f 6e65  tyle='fill: none
+000009b0: 3b20 7374 726f 6b65 3a20 246c 756e 6172  ; stroke: $lunar
+000009c0: 5f70 6861 7365 5f6f 7574 6c69 6e65 3b20  _phase_outline; 
+000009d0: 7374 726f 6b65 2d77 6964 7468 3a20 302e  stroke-width: 0.
+000009e0: 3570 783b 2073 7472 6f6b 652d 6f70 6163  5px; stroke-opac
+000009f0: 6974 793a 202e 353b 2720 2f3e 0d0a 2020  ity: .5;' />..  
+00000a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a10: 2020 3c2f 673e 0d0a 2020 2020 2020 2020    </g>..        
+00000a20: 2020 2020 2020 2020 3c2f 673e 2020 2020          </g>    
+00000a30: 2020 2020 2020 2020 2020 2020 202d 2d3e               -->
+00000a40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00000a50: 2020 3c21 2d2d 2050 6c61 6e65 7473 2028    <!-- Planets (
+00000a60: 3234 7832 3429 202d 2d3e 0d0a 2020 2020  24x24) -->..    
+00000a70: 2020 2020 2020 2020 2020 2020 3c73 796d              <sym
+00000a80: 626f 6c20 6964 3d27 5375 6e27 3e0d 0a20  bol id='Sun'>.. 
+00000a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000aa0: 2020 203c 6720 7472 616e 7366 6f72 6d3d     <g transform=
+00000ab0: 2774 7261 6e73 6c61 7465 2831 2c34 2927  'translate(1,4)'
+00000ac0: 2063 6c61 7373 3d27 706c 616e 6574 5379   class='planetSy
+00000ad0: 6d62 6f6c 273e 0d0a 2020 2020 2020 2020  mbol'>..        
+00000ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000af0: 3c63 6972 636c 6520 6378 3d27 3130 2720  <circle cx='10' 
+00000b00: 6379 3d27 3130 2720 723d 2739 2720 7374  cy='10' r='9' st
+00000b10: 796c 653d 2766 696c 6c3a 206e 6f6e 653b  yle='fill: none;
+00000b20: 2073 7472 6f6b 653a 2024 706c 616e 6574   stroke: $planet
+00000b30: 735f 636f 6c6f 725f 303b 2073 7472 6f6b  s_color_0; strok
+00000b40: 652d 7769 6474 683a 2032 7078 3b27 202f  e-width: 2px;' /
+00000b50: 3e0d 0a20 2020 2020 2020 2020 2020 2020  >..             
+00000b60: 2020 2020 2020 2020 2020 203c 6369 7263             <circ
+00000b70: 6c65 2063 783d 2731 3027 2063 793d 2731  le cx='10' cy='1
+00000b80: 3027 2072 3d27 3227 2073 7479 6c65 3d27  0' r='2' style='
+00000b90: 6669 6c6c 3a20 2470 6c61 6e65 7473 5f63  fill: $planets_c
+00000ba0: 6f6c 6f72 5f30 3b27 202f 3e0d 0a20 2020  olor_0;' />..   
+00000bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000bc0: 203c 2f67 3e0d 0a20 2020 2020 2020 2020   </g>..         
+00000bd0: 2020 2020 2020 203c 2f73 796d 626f 6c3e         </symbol>
+00000be0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00000bf0: 2020 3c73 796d 626f 6c20 6964 3d27 4d6f    <symbol id='Mo
+00000c00: 6f6e 273e 0d0a 2020 2020 2020 2020 2020  on'>..          
+00000c10: 2020 2020 2020 2020 2020 3c67 2074 7261            <g tra
+00000c20: 6e73 666f 726d 3d27 7472 616e 736c 6174  nsform='translat
+00000c30: 6528 342c 3329 2073 6361 6c65 282e 3829  e(4,3) scale(.8)
+00000c40: 2720 636c 6173 733d 2770 6c61 6e65 7453  ' class='planetS
+00000c50: 796d 626f 6c27 3e0d 0a20 2020 2020 2020  ymbol'>..       
+00000c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000c70: 203c 7061 7468 2064 3d27 4d20 332e 3636   <path d='M 3.66
+00000c80: 3339 3139 342c 312e 3033 3038 3530 3920  39194,1.0308509 
+00000c90: 4320 322e 3734 3938 3439 342c 312e 3036  C 2.7498494,1.06
+00000ca0: 3536 3330 3920 312e 3837 3231 3339 342c  56309 1.8721394,
+00000cb0: 312e 3231 3339 3230 3920 312e 3032 3834  1.2139209 1.0284
+00000cc0: 3639 342c 312e 3435 3933 3830 3920 4320  694,1.4593809 C 
+00000cd0: 352e 3537 3239 3739 342c 322e 3739 3939  5.5729794,2.7999
+00000ce0: 3630 3920 382e 3839 3139 3739 342c 372e  609 8.8919794,7.
+00000cf0: 3032 3432 3230 3920 382e 3839 3139 3739  0242209 8.891979
+00000d00: 342c 3132 2e30 3031 3139 3120 4320 382e  4,12.001191 C 8.
+00000d10: 3839 3139 3739 342c 3136 2e39 3738 3136  8919794,16.97816
+00000d20: 3120 352e 3537 3239 3739 342c 3231 2e32  1 5.5729794,21.2
+00000d30: 3032 3431 3120 312e 3032 3834 3639 342c  02411 1.0284694,
+00000d40: 3232 2e35 3433 3030 3120 4320 322e 3030  22.543001 C 2.00
+00000d50: 3139 3239 342c 3232 2e38 3236 3232 3120  19294,22.826221 
+00000d60: 332e 3032 3739 3839 342c 3232 2e39 3731  3.0279894,22.971
+00000d70: 3533 3120 342e 3039 3234 3439 342c 3232  531 4.0924494,22
+00000d80: 2e39 3731 3533 3120 4320 3130 2e31 3438  .971531 C 10.148
+00000d90: 3037 392c 3232 2e39 3731 3533 3120 3135  079,22.971531 15
+00000da0: 2e30 3632 3738 392c 3138 2e30 3536 3832  .062789,18.05682
+00000db0: 3120 3135 2e30 3632 3738 392c 3132 2e30  1 15.062789,12.0
+00000dc0: 3031 3139 3120 4320 3135 2e30 3632 3738  01191 C 15.06278
+00000dd0: 392c 352e 3934 3535 3630 3920 3130 2e31  9,5.9455609 10.1
+00000de0: 3438 3037 392c 312e 3033 3038 3530 3920  48079,1.0308509 
+00000df0: 342e 3039 3234 3439 342c 312e 3033 3038  4.0924494,1.0308
+00000e00: 3530 3920 4320 332e 3935 3035 3139 342c  509 C 3.9505194,
+00000e10: 312e 3033 3038 3530 3920 332e 3830 3435  1.0308509 3.8045
+00000e20: 3439 342c 312e 3032 3534 3930 3920 332e  494,1.0254909 3.
+00000e30: 3636 3339 3139 342c 312e 3033 3038 3530  6639194,1.030850
+00000e40: 3920 7a20 2720 7374 796c 653d 2773 7472  9 z ' style='str
+00000e50: 6f6b 653a 2470 6c61 6e65 7473 5f63 6f6c  oke:$planets_col
+00000e60: 6f72 5f31 3b73 7472 6f6b 652d 7769 6474  or_1;stroke-widt
+00000e70: 683a 3270 783b 2066 696c 6c3a 6e6f 6e65  h:2px; fill:none
+00000e80: 3b27 202f 3e0d 0a20 2020 2020 2020 2020  ;' />..         
+00000e90: 2020 2020 2020 2020 2020 203c 2f67 3e0d             </g>.
+00000ea0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000eb0: 203c 2f73 796d 626f 6c3e 0d0a 2020 2020   </symbol>..    
+00000ec0: 2020 2020 2020 2020 2020 2020 3c73 796d              <sym
+00000ed0: 626f 6c20 6964 3d27 4d65 7263 7572 7927  bol id='Mercury'
+00000ee0: 3e0d 0a20 2020 2020 2020 2020 2020 2020  >..             
+00000ef0: 2020 2020 2020 203c 6720 7472 616e 7366         <g transf
+00000f00: 6f72 6d3d 2774 7261 6e73 6c61 7465 2833  orm='translate(3
+00000f10: 2c31 2927 2063 6c61 7373 3d27 706c 616e  ,1)' class='plan
+00000f20: 6574 5379 6d62 6f6c 273e 0d0a 2020 2020  etSymbol'>..    
+00000f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000f40: 2020 2020 3c70 6174 6820 643d 274d 2031      <path d='M 1
+00000f50: 322e 3431 3739 3038 2c31 312e 3039 3735  2.417908,11.0975
+00000f60: 3037 2043 2031 322e 3436 3038 3138 2c31  07 C 12.460818,1
+00000f70: 332e 3630 3439 3136 2031 302e 3636 3832  3.604916 10.6682
+00000f80: 3137 2c31 352e 3939 3636 3536 2038 2e32  17,15.996656 8.2
+00000f90: 3536 3638 3035 2c31 362e 3637 3636 3339  566805,16.676639
+00000fa0: 2043 2036 2e31 3138 3033 3735 2c31 372e   C 6.1180375,17.
+00000fb0: 3332 3235 3232 2033 2e36 3430 3836 3735  322522 3.6408675
+00000fc0: 2c31 362e 3631 3138 3639 2032 2e31 3939  ,16.611869 2.199
+00000fd0: 3039 3135 2c31 342e 3839 3730 3235 2043  0915,14.897025 C
+00000fe0: 2030 2e37 3032 3531 3335 312c 3133 2e31   0.70251351,13.1
+00000ff0: 3835 3839 3420 302e 3334 3730 3535 3531  85894 0.34705551
+00001000: 2c31 302e 3537 3431 3439 2031 2e33 3738  ,10.574149 1.378
+00001010: 3738 3335 2c38 2e35 3430 3633 3720 4320  7835,8.540637 C 
+00001020: 322e 3333 3039 3036 352c 362e 3537 3738  2.3309065,6.5778
+00001030: 3139 3620 342e 3434 3438 3932 352c 352e  196 4.4448925,5.
+00001040: 3233 3930 3531 3520 362e 3633 3434 3338  2390515 6.634438
+00001050: 352c 352e 3238 3031 3831 3220 4320 382e  5,5.2801812 C 8.
+00001060: 3734 3336 3438 352c 352e 3238 3038 3138  7436485,5.280818
+00001070: 3420 3130 2e37 3937 3231 2c36 2e35 3138  4 10.79721,6.518
+00001080: 3438 3937 2031 312e 3735 3536 3431 2c38  4897 11.755641,8
+00001090: 2e34 3031 3432 3239 2043 2031 322e 3138  .4014229 C 12.18
+000010a0: 3837 3039 2c39 2e32 3239 3335 3633 2031  8709,9.2293563 1
+000010b0: 322e 3432 3139 3236 2c31 302e 3136 3235  2.421926,10.1625
+000010c0: 3638 2031 322e 3431 3739 3038 2c31 312e  68 12.417908,11.
+000010d0: 3039 3735 3037 207a 204d 2031 312e 3533  097507 z M 11.53
+000010e0: 3735 3439 2c30 2e37 3934 3737 3735 3620  7549,0.79477756 
+000010f0: 4320 3131 2e33 3638 3031 312c 322e 3935  C 11.368011,2.95
+00001100: 3331 3633 3620 392e 3539 3238 3130 352c  31636 9.5928105,
+00001110: 342e 3834 3933 3934 2037 2e34 3532 3834  4.849394 7.45284
+00001120: 3535 2c35 2e31 3731 3132 3720 4320 352e  55,5.171127 C 5.
+00001130: 3439 3334 3033 352c 352e 3530 3538 3436  4934035,5.505846
+00001140: 3720 332e 3336 3334 3530 352c 342e 3534  7 3.3634505,4.54
+00001150: 3934 3638 3620 322e 3339 3538 3133 352c  94686 2.3958135,
+00001160: 322e 3739 3436 3538 3620 4320 322e 3034  2.7946586 C 2.04
+00001170: 3438 3135 352c 322e 3138 3138 3734 3620  48155,2.1818746 
+00001180: 312e 3832 3735 3735 352c 312e 3439 3330  1.8275755,1.4930
+00001190: 3936 3620 312e 3736 3236 3834 352c 302e  966 1.7626845,0.
+000011a0: 3738 3939 3337 3536 204d 2036 2e36 3033  78993756 M 6.603
+000011b0: 3936 3235 2c31 362e 3839 3035 3138 2043  9625,16.890518 C
+000011c0: 2036 2e36 3033 3936 3235 2c31 382e 3939   6.6039625,18.99
+000011d0: 3730 3331 2036 2e36 3033 3936 3235 2c32  7031 6.6039625,2
+000011e0: 312e 3130 3335 3435 2036 2e36 3033 3936  1.103545 6.60396
+000011f0: 3235 2c32 332e 3231 3030 3538 204d 2033  25,23.210058 M 3
+00001200: 2e39 3730 3832 3135 2c32 302e 3537 3639  .9708215,20.5769
+00001210: 3136 2043 2035 2e37 3236 3234 3735 2c32  16 C 5.7262475,2
+00001220: 302e 3537 3639 3136 2037 2e34 3831 3637  0.576916 7.48167
+00001230: 3835 2c32 302e 3537 3639 3136 2039 2e32  85,20.576916 9.2
+00001240: 3337 3130 3435 2c32 302e 3537 3639 3136  371045,20.576916
+00001250: 2720 7374 796c 653d 2773 7472 6f6b 653a  ' style='stroke:
+00001260: 2470 6c61 6e65 7473 5f63 6f6c 6f72 5f32  $planets_color_2
+00001270: 3b73 7472 6f6b 652d 7769 6474 683a 3270  ;stroke-width:2p
+00001280: 783b 2066 696c 6c3a 6e6f 6e65 3b27 202f  x; fill:none;' /
+00001290: 3e0d 0a20 2020 2020 2020 2020 2020 2020  >..             
+000012a0: 2020 2020 2020 203c 2f67 3e0d 0a20 2020         </g>..   
+000012b0: 2020 2020 2020 2020 2020 2020 203c 2f73               </s
+000012c0: 796d 626f 6c3e 0d0a 2020 2020 2020 2020  ymbol>..        
+000012d0: 2020 2020 2020 2020 3c73 796d 626f 6c20          <symbol 
+000012e0: 6964 3d27 5665 6e75 7327 3e0d 0a20 2020  id='Venus'>..   
+000012f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001300: 203c 6720 7472 616e 7366 6f72 6d3d 2774   <g transform='t
+00001310: 7261 6e73 6c61 7465 2830 2c32 2920 7363  ranslate(0,2) sc
+00001320: 616c 6528 2e39 2927 2063 6c61 7373 3d27  ale(.9)' class='
+00001330: 706c 616e 6574 5379 6d62 6f6c 273e 0d0a  planetSymbol'>..
+00001340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001350: 2020 2020 2020 2020 3c70 6174 6820 643d          <path d=
+00001360: 274d 2031 382e 3430 3037 3033 2c37 2e33  'M 18.400703,7.3
+00001370: 3636 3734 3833 2043 2031 382e 3432 3339  667483 C 18.4239
+00001380: 362c 392e 3636 3535 3332 3920 3137 2e31  6,9.6655329 17.1
+00001390: 3730 3130 322c 3131 2e39 3134 3537 3920  70102,11.914579 
+000013a0: 3135 2e32 3138 3937 322c 3133 2e31 3133  15.218972,13.113
+000013b0: 3732 3820 4320 3133 2e31 3632 3435 392c  728 C 13.162459,
+000013c0: 3134 2e34 3237 3235 3320 3130 2e33 3839  14.427253 10.389
+000013d0: 3835 352c 3134 2e34 3736 3737 3220 382e  855,14.476772 8.
+000013e0: 3238 3731 3636 332c 3133 2e32 3339 3730  2871663,13.23970
+000013f0: 3920 4320 362e 3237 3335 3835 312c 3132  9 C 6.2735851,12
+00001400: 2e31 3030 3532 3420 342e 3933 3336 3333  .100524 4.933633
+00001410: 2c39 2e38 3634 3033 3233 2034 2e38 3937  ,9.8640323 4.897
+00001420: 3939 3135 2c37 2e35 3431 3438 3034 2043  9915,7.5414804 C
+00001430: 2034 2e38 3137 3336 3137 2c35 2e32 3637   4.8173617,5.267
+00001440: 3835 3932 2035 2e39 3835 3531 3936 2c33  8592 5.9855196,3
+00001450: 2e30 3039 3030 3031 2037 2e38 3732 3838  .0090001 7.87288
+00001460: 3037 2c31 2e37 3533 3034 3731 2043 2039  07,1.7530471 C 9
+00001470: 2e38 3830 3339 3135 2c30 2e33 3635 3039  .8803915,0.36509
+00001480: 3534 3620 3132 2e36 3438 3930 362c 302e  546 12.648906,0.
+00001490: 3231 3635 3731 3436 2031 342e 3739 3438  21657146 14.7948
+000014a0: 3439 2c31 2e33 3735 3238 3331 2043 2031  49,1.3752831 C 1
+000014b0: 362e 3836 3937 3732 2c32 2e34 3531 3436  6.869772,2.45146
+000014c0: 3333 2031 382e 3239 3632 3431 2c34 2e36  33 18.296241,4.6
+000014d0: 3733 3134 3533 2031 382e 3339 3139 3138  731453 18.391918
+000014e0: 2c37 2e30 3138 3337 3233 2043 2031 382e  ,7.0183723 C 18.
+000014f0: 3339 3737 3831 2c37 2e31 3334 3339 3633  397781,7.1343963
+00001500: 2031 382e 3430 3037 3033 2c37 2e32 3530   18.400703,7.250
+00001510: 3537 3233 2031 382e 3430 3037 3033 2c37  5723 18.400703,7
+00001520: 2e33 3636 3734 3833 207a 204d 2031 312e  .3667483 z M 11.
+00001530: 3634 3832 3839 2c31 342e 3133 3636 3839  648289,14.136689
+00001540: 2043 2031 312e 3634 3832 3839 2c31 372e   C 11.648289,17.
+00001550: 3030 3837 3634 2031 312e 3634 3832 3839  008764 11.648289
+00001560: 2c31 392e 3838 3038 3420 3131 2e36 3438  ,19.88084 11.648
+00001570: 3238 392c 3232 2e37 3532 3931 3520 4d20  289,22.752915 M 
+00001580: 372e 3936 3531 3333 332c 3139 2e30 3630  7.9651333,19.060
+00001590: 3234 3320 4320 3130 2e34 3230 3537 2c31  243 C 10.42057,1
+000015a0: 392e 3036 3032 3433 2031 322e 3837 3630  9.060243 12.8760
+000015b0: 3038 2c31 392e 3036 3032 3433 2031 352e  08,19.060243 15.
+000015c0: 3333 3134 3434 2c31 392e 3036 3032 3433  331444,19.060243
+000015d0: 2720 7374 796c 653d 2773 7472 6f6b 653a  ' style='stroke:
+000015e0: 2470 6c61 6e65 7473 5f63 6f6c 6f72 5f33  $planets_color_3
+000015f0: 3b73 7472 6f6b 652d 7769 6474 683a 3270  ;stroke-width:2p
+00001600: 783b 2066 696c 6c3a 6e6f 6e65 3b27 202f  x; fill:none;' /
+00001610: 3e0d 0a20 2020 2020 2020 2020 2020 2020  >..             
+00001620: 2020 2020 2020 203c 2f67 3e0d 0a20 2020         </g>..   
+00001630: 2020 2020 2020 2020 2020 2020 203c 2f73               </s
+00001640: 796d 626f 6c3e 0d0a 2020 2020 2020 2020  ymbol>..        
+00001650: 2020 2020 2020 2020 3c73 796d 626f 6c20          <symbol 
+00001660: 6964 3d27 4d61 7273 273e 0d0a 2020 2020  id='Mars'>..    
+00001670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001680: 3c67 2074 7261 6e73 666f 726d 3d27 7472  <g transform='tr
+00001690: 616e 736c 6174 6528 312c 3329 2073 6361  anslate(1,3) sca
+000016a0: 6c65 282e 3929 2720 636c 6173 733d 2770  le(.9)' class='p
+000016b0: 6c61 6e65 7453 796d 626f 6c27 3e0d 0a20  lanetSymbol'>.. 
+000016c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000016d0: 2020 2020 2020 203c 7061 7468 2064 3d27         <path d='
+000016e0: 4d20 3139 2e38 3336 3832 382c 312e 3232  M 19.836828,1.22
+000016f0: 3638 3538 3520 4320 3137 2e34 3234 3432  68585 C 17.42442
+00001700: 322c 332e 3632 3538 3737 3620 3135 2e30  2,3.6258776 15.0
+00001710: 3132 3030 382c 362e 3032 3439 3034 3720  12008,6.0249047 
+00001720: 3132 2e35 3939 3539 342c 382e 3432 3339  12.599594,8.4239
+00001730: 3331 3720 4d20 3133 2e35 3836 3133 312c  317 M 13.586131,
+00001740: 312e 3330 3332 3835 3320 4320 3135 2e36  1.3032853 C 15.6
+00001750: 3431 3632 322c 312e 3330 3332 3835 3320  41622,1.3032853 
+00001760: 3137 2e36 3937 3130 352c 312e 3330 3332  17.697105,1.3032
+00001770: 3835 3320 3139 2e37 3532 3539 352c 312e  853 19.752595,1.
+00001780: 3330 3332 3835 3320 4320 3139 2e37 3532  3032853 C 19.752
+00001790: 3539 352c 332e 3334 3733 3638 3620 3139  595,3.3473686 19
+000017a0: 2e37 3532 3630 332c 352e 3339 3134 3531  .752603,5.391451
+000017b0: 3720 3139 2e37 3532 3630 332c 372e 3433  7 19.752603,7.43
+000017c0: 3535 3335 3727 2073 7479 6c65 3d27 7374  55357' style='st
+000017d0: 726f 6b65 3a24 706c 616e 6574 735f 636f  roke:$planets_co
+000017e0: 6c6f 725f 343b 7374 726f 6b65 2d77 6964  lor_4;stroke-wid
+000017f0: 7468 3a32 7078 3b20 6669 6c6c 3a6e 6f6e  th:2px; fill:non
+00001800: 653b 2720 2f3e 0d0a 2020 2020 2020 2020  e;' />..        
+00001810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001820: 3c70 6174 6820 643d 274d 2031 352e 3230  <path d='M 15.20
+00001830: 3838 3335 2c31 332e 3133 3737 3131 2043  8835,13.137711 C
+00001840: 2031 352e 3234 3537 3837 2c31 352e 3838   15.245787,15.88
+00001850: 3833 3039 2031 332e 3439 3735 3233 2c31  8309 13.497523,1
+00001860: 382e 3534 3334 3620 3130 2e39 3639 3034  8.54346 10.96904
+00001870: 332c 3139 2e36 3137 3733 2043 2038 2e34  3,19.61773 C 8.4
+00001880: 3538 3431 3735 2c32 302e 3734 3930 3336  584175,20.749036
+00001890: 2035 2e33 3135 3534 3238 2c32 302e 3231   5.3155428,20.21
+000018a0: 3634 3120 332e 3332 3336 3330 362c 3138  641 3.3236306,18
+000018b0: 2e33 3132 3834 3320 4320 312e 3332 3934  .312843 C 1.3294
+000018c0: 3738 392c 3136 2e35 3032 3638 3620 302e  789,16.502686 0.
+000018d0: 3535 3436 3631 3237 2c31 332e 3530 3436  55466127,13.5046
+000018e0: 3738 2031 2e34 3133 3336 3135 2c31 302e  78 1.4133615,10.
+000018f0: 3935 3333 3032 2043 2032 2e32 3438 3537  953302 C 2.24857
+00001900: 3231 2c38 2e32 3833 3334 3532 2034 2e38  21,8.2833452 4.8
+00001910: 3030 3530 3433 2c36 2e32 3636 3030 3735  005043,6.2660075
+00001920: 2037 2e35 3935 3231 382c 362e 3038 3834   7.595218,6.0884
+00001930: 3236 3620 4320 3130 2e32 3837 3033 322c  266 C 10.287032,
+00001940: 352e 3834 3637 3938 3420 3133 2e30 3232  5.8467984 13.022
+00001950: 3334 382c 372e 3332 3331 3034 3820 3134  348,7.3231048 14
+00001960: 2e33 3133 3836 2c39 2e36 3933 3830 3831  .31386,9.6938081
+00001970: 2043 2031 342e 3930 3131 3633 2c31 302e   C 14.901163,10.
+00001980: 3733 3939 3637 2031 352e 3231 3130 3832  739967 15.211082
+00001990: 2c31 312e 3933 3831 3936 2031 352e 3230  ,11.938196 15.20
+000019a0: 3838 3335 2c31 332e 3133 3737 3131 207a  8835,13.137711 z
+000019b0: 2720 7374 796c 653d 2773 7472 6f6b 653a  ' style='stroke:
+000019c0: 2470 6c61 6e65 7473 5f63 6f6c 6f72 5f34  $planets_color_4
+000019d0: 3b73 7472 6f6b 652d 7769 6474 683a 3270  ;stroke-width:2p
+000019e0: 783b 2066 696c 6c3a 6e6f 6e65 3b27 202f  x; fill:none;' /
+000019f0: 3e0d 0a20 2020 2020 2020 2020 2020 2020  >..             
+00001a00: 2020 2020 2020 203c 2f67 3e0d 0a20 2020         </g>..   
+00001a10: 2020 2020 2020 2020 2020 2020 203c 2f73               </s
+00001a20: 796d 626f 6c3e 0d0a 2020 2020 2020 2020  ymbol>..        
+00001a30: 2020 2020 2020 2020 3c73 796d 626f 6c20          <symbol 
+00001a40: 6964 3d27 4a75 7069 7465 7227 3e0d 0a20  id='Jupiter'>.. 
+00001a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a60: 2020 203c 6720 7472 616e 7366 6f72 6d3d     <g transform=
+00001a70: 2774 7261 6e73 6c61 7465 2831 2c33 2920  'translate(1,3) 
+00001a80: 7363 616c 6528 2e39 2927 2063 6c61 7373  scale(.9)' class
+00001a90: 3d27 706c 616e 6574 5379 6d62 6f6c 273e  ='planetSymbol'>
+00001aa0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00001ab0: 2020 2020 2020 2020 2020 3c70 6174 6820            <path 
+00001ac0: 643d 274d 2031 362e 3930 3330 3038 2c30  d='M 16.903008,0
+00001ad0: 2e39 3938 3439 3135 3720 4c20 3136 2e39  .99849157 L 16.9
+00001ae0: 3033 3030 382c 3233 2e30 3031 3531 3220  03008,23.001512 
+00001af0: 4d20 3230 2e35 3330 3237 382c 3137 2e33  M 20.530278,17.3
+00001b00: 3539 3731 3220 4c20 322e 3939 3834 3838  59712 L 2.998488
+00001b10: 342c 3137 2e33 3539 3731 3220 4d20 342e  4,17.359712 M 4.
+00001b20: 3831 3231 3138 342c 382e 3839 3730 3132  8121184,8.897012
+00001b30: 2043 2034 2e32 3037 3537 3834 2c38 2e38   C 4.2075784,8.8
+00001b40: 3937 3031 3220 322e 3939 3834 3838 342c  97012 2.9984884,
+00001b50: 382e 3333 3238 3332 2032 2e39 3938 3438  8.332832 2.99848
+00001b60: 3834 2c36 2e30 3736 3131 3220 4320 322e  84,6.076112 C 2.
+00001b70: 3939 3834 3838 342c 332e 3831 3933 3832  9984884,3.819382
+00001b80: 2035 2e34 3136 3636 3834 2c31 2e35 3632   5.4166684,1.562
+00001b90: 3637 3136 2037 2e38 3334 3834 3834 2c31  6716 7.8348484,1
+00001ba0: 2e35 3632 3637 3136 2043 2031 302e 3235  .5626716 C 10.25
+00001bb0: 3330 3238 2c31 2e35 3632 3637 3136 2031  3028,1.5626716 1
+00001bc0: 322e 3637 3131 3938 2c33 2e32 3535 3231  2.671198,3.25521
+00001bd0: 3220 3132 2e36 3731 3139 382c 372e 3230  2 12.671198,7.20
+00001be0: 3434 3732 2043 2031 322e 3637 3131 3938  4472 C 12.671198
+00001bf0: 2c31 312e 3135 3337 3332 2039 2e36 3438  ,11.153732 9.648
+00001c00: 3437 3834 2c31 372e 3335 3937 3132 2033  4784,17.359712 3
+00001c10: 2e36 3033 3032 3834 2c31 372e 3335 3937  .6030284,17.3597
+00001c20: 3132 2720 7374 796c 653d 2773 7472 6f6b  12' style='strok
+00001c30: 653a 2470 6c61 6e65 7473 5f63 6f6c 6f72  e:$planets_color
+00001c40: 5f35 3b73 7472 6f6b 652d 7769 6474 683a  _5;stroke-width:
+00001c50: 3270 783b 2066 696c 6c3a 6e6f 6e65 3b27  2px; fill:none;'
+00001c60: 202f 3e0d 0a20 2020 2020 2020 2020 2020   />..           
+00001c70: 2020 2020 2020 2020 203c 2f67 3e0d 0a20           </g>.. 
+00001c80: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00001c90: 2f73 796d 626f 6c3e 0d0a 2020 2020 2020  /symbol>..      
+00001ca0: 2020 2020 2020 2020 2020 3c73 796d 626f            <symbo
+00001cb0: 6c20 6964 3d27 5361 7475 726e 273e 0d0a  l id='Saturn'>..
+00001cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001cd0: 2020 2020 3c67 2074 7261 6e73 666f 726d      <g transform
+00001ce0: 3d27 7472 616e 736c 6174 6528 312c 3229  ='translate(1,2)
+00001cf0: 2720 636c 6173 733d 2770 6c61 6e65 7453  ' class='planetS
+00001d00: 796d 626f 6c27 3e0d 0a20 2020 2020 2020  ymbol'>..       
+00001d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d20: 203c 7061 7468 2064 3d27 4d20 382e 3338   <path d='M 8.38
+00001d30: 3434 3334 392c 302e 3930 3230 3332 3331  44349,0.90203231
+00001d40: 204c 2038 2e33 3834 3433 3439 2c31 382e   L 8.3844349,18.
+00001d50: 3239 3838 3532 204d 2035 2e34 3334 3934  298852 M 5.43494
+00001d60: 3439 2c33 2e37 3531 3531 3233 204c 2031  49,3.7515123 L 1
+00001d70: 322e 3636 3837 3435 2c33 2e37 3531 3531  2.668745,3.75151
+00001d80: 3233 204d 2031 362e 3832 3338 3735 2c32  23 M 16.823875,2
+00001d90: 312e 3839 3831 3932 2043 2031 362e 3232  1.898192 C 16.22
+00001da0: 3130 3535 2c32 322e 3439 3830 3832 2031  1055,22.498082 1
+00001db0: 352e 3631 3832 3335 2c32 332e 3039 3739  5.618235,23.0979
+00001dc0: 3732 2031 352e 3031 3534 3135 2c32 332e  72 15.015415,23.
+00001dd0: 3039 3739 3732 2043 2031 342e 3431 3236  097972 C 14.4126
+00001de0: 3035 2c32 332e 3039 3739 3732 2031 332e  05,23.097972 13.
+00001df0: 3230 3639 3735 2c32 322e 3439 3830 3832  206975,22.498082
+00001e00: 2031 332e 3230 3639 3735 2c32 312e 3239   13.206975,21.29
+00001e10: 3833 3032 2043 2031 332e 3230 3639 3735  8302 C 13.206975
+00001e20: 2c32 302e 3039 3835 3232 2031 332e 3830  ,20.098522 13.80
+00001e30: 3937 3835 2c31 382e 3839 3837 3432 2031  9785,18.898742 1
+00001e40: 352e 3031 3534 3135 2c31 372e 3639 3839  5.015415,17.6989
+00001e50: 3632 2043 2031 362e 3232 3130 3535 2c31  62 C 16.221055,1
+00001e60: 362e 3439 3931 3832 2031 372e 3432 3636  6.499182 17.4266
+00001e70: 3835 2c31 342e 3039 3936 3232 2031 372e  85,14.099622 17.
+00001e80: 3432 3636 3835 2c31 312e 3730 3030 3532  426685,11.700052
+00001e90: 2043 2031 372e 3432 3636 3835 2c39 2e33   C 17.426685,9.3
+00001ea0: 3030 3439 3233 2031 362e 3232 3130 3535  004923 16.221055
+00001eb0: 2c36 2e39 3030 3933 3233 2031 332e 3830  ,6.9009323 13.80
+00001ec0: 3937 3835 2c36 2e39 3030 3933 3233 2043  9785,6.9009323 C
+00001ed0: 2031 312e 3532 3932 3135 2c36 2e39 3030   11.529215,6.900
+00001ee0: 3933 3233 2039 2e35 3930 3036 3439 2c38  9323 9.5900649,8
+00001ef0: 2e31 3030 3731 3233 2038 2e33 3834 3433  .1007123 8.38443
+00001f00: 3439 2c31 302e 3530 3032 3832 2720 7374  49,10.500282' st
+00001f10: 796c 653d 2773 7472 6f6b 653a 2470 6c61  yle='stroke:$pla
+00001f20: 6e65 7473 5f63 6f6c 6f72 5f36 3b73 7472  nets_color_6;str
+00001f30: 6f6b 652d 7769 6474 683a 3270 783b 2066  oke-width:2px; f
+00001f40: 696c 6c3a 6e6f 6e65 3b27 202f 3e0d 0a20  ill:none;' />.. 
+00001f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f60: 2020 203c 2f67 3e0d 0a20 2020 2020 2020     </g>..       
+00001f70: 2020 2020 2020 2020 203c 2f73 796d 626f           </symbo
+00001f80: 6c3e 0d0a 2020 2020 2020 2020 2020 2020  l>..            
+00001f90: 2020 2020 3c73 796d 626f 6c20 6964 3d27      <symbol id='
+00001fa0: 5572 616e 7573 273e 0d0a 2020 2020 2020  Uranus'>..      
+00001fb0: 2020 2020 2020 2020 2020 2020 2020 3c67                <g
+00001fc0: 2074 7261 6e73 666f 726d 3d27 7472 616e   transform='tran
+00001fd0: 736c 6174 6528 322c 3429 2073 6361 6c65  slate(2,4) scale
+00001fe0: 282e 3829 2720 636c 6173 733d 2770 6c61  (.8)' class='pla
+00001ff0: 6e65 7453 796d 626f 6c27 3e0d 0a20 2020  netSymbol'>..   
+00002000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002010: 2020 2020 203c 7061 7468 2064 3d27 4d20       <path d='M 
+00002020: 342e 3637 3732 3036 362c 3136 2e30 3937  4.6772066,16.097
+00002030: 3432 3320 4320 332e 3230 3432 3432 362c  423 C 3.2042426,
+00002040: 3136 2e30 3937 3432 3320 312e 3733 3132  16.097423 1.7312
+00002050: 3737 362c 3136 2e30 3937 3432 3320 302e  776,16.097423 0.
+00002060: 3235 3833 3036 3631 2c31 362e 3039 3734  25830661,16.0974
+00002070: 3233 2043 2030 2e33 3231 3835 3036 312c  23 C 0.32185061,
+00002080: 3135 2e38 3934 3837 3920 302e 3131 3939  15.894879 0.1199
+00002090: 3536 3631 2c31 352e 3438 3530 3936 2030  5661,15.485096 0
+000020a0: 2e33 3739 3736 3336 312c 3135 2e34 3335  .37976361,15.435
+000020b0: 3738 3720 4320 312e 3138 3039 3732 362c  787 C 1.1809726,
+000020c0: 3135 2e32 3335 3438 3520 312e 3938 3231  15.235485 1.9821
+000020d0: 3832 362c 3135 2e30 3335 3138 3220 322e  826,15.035182 2.
+000020e0: 3738 3333 3932 362c 3134 2e38 3334 3838  7833926,14.83488
+000020f0: 2043 2032 2e37 3833 3339 3236 2c31 302e   C 2.7833926,10.
+00002100: 3632 3634 3031 2032 2e37 3833 3339 3236  626401 2.7833926
+00002110: 2c36 2e34 3137 3932 3920 322e 3738 3333  ,6.417929 2.7833
+00002120: 3932 362c 322e 3230 3934 3530 3220 4320  926,2.2094502 C 
+00002130: 312e 3934 3136 3939 362c 312e 3939 3930  1.9416996,1.9990
+00002140: 3238 3520 312e 3130 3030 3035 362c 312e  285 1.1000056,1.
+00002150: 3738 3836 3030 3420 302e 3235 3833 3036  7886004 0.258306
+00002160: 3631 2c31 2e35 3738 3137 3837 2043 2030  61,1.5781787 C 0
+00002170: 2e33 3233 3830 3736 312c 312e 3339 3135  .32380761,1.3915
+00002180: 3234 3320 302e 3131 3537 3032 3631 2c30  243 0.11570261,0
+00002190: 2e39 3331 3236 3433 3220 302e 3338 3335  .93126432 0.3835
+000021a0: 3030 3631 2c30 2e39 3436 3930 3732 3220  0061,0.94690722 
+000021b0: 4320 312e 3831 3437 3337 362c 302e 3934  C 1.8147376,0.94
+000021c0: 3639 3037 3232 2033 2e32 3435 3936 3936  690722 3.2459696
+000021d0: 2c30 2e39 3436 3930 3732 3220 342e 3637  ,0.94690722 4.67
+000021e0: 3732 3036 362c 302e 3934 3639 3037 3232  72066,0.94690722
+000021f0: 2043 2034 2e36 3737 3230 3636 2c35 2e39   C 4.6772066,5.9
+00002200: 3937 3037 3932 2034 2e36 3737 3230 3636  970792 4.6772066
+00002210: 2c31 312e 3034 3732 3531 2034 2e36 3737  ,11.047251 4.677
+00002220: 3230 3636 2c31 362e 3039 3734 3233 207a  2066,16.097423 z
+00002230: 2027 2073 7479 6c65 3d27 7374 726f 6b65   ' style='stroke
+00002240: 3a24 706c 616e 6574 735f 636f 6c6f 725f  :$planets_color_
+00002250: 373b 7374 726f 6b65 2d77 6964 7468 3a31  7;stroke-width:1
+00002260: 7078 3b20 6669 6c6c 3a24 706c 616e 6574  px; fill:$planet
+00002270: 735f 636f 6c6f 725f 353b 2720 2f3e 0d0a  s_color_5;' />..
+00002280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002290: 2020 2020 2020 2020 3c70 6174 6820 643d          <path d=
+000022a0: 274d 2031 382e 3536 3531 382c 3136 2e30  'M 18.56518,16.0
+000022b0: 3937 3432 3320 4320 3230 2e30 3338 3135  97423 C 20.03815
+000022c0: 312c 3136 2e30 3937 3432 3320 3231 2e35  1,16.097423 21.5
+000022d0: 3131 3131 362c 3136 2e30 3937 3432 3320  11116,16.097423 
+000022e0: 3232 2e39 3834 3038 312c 3136 2e30 3937  22.984081,16.097
+000022f0: 3432 3320 4320 3232 2e39 3230 3534 332c  423 C 22.920543,
+00002300: 3135 2e38 3934 3837 3920 3233 2e31 3232  15.894879 23.122
+00002310: 3433 2c31 352e 3438 3530 3936 2032 322e  43,15.485096 22.
+00002320: 3836 3236 3331 2c31 352e 3433 3537 3837  862631,15.435787
+00002330: 2043 2032 322e 3036 3134 3231 2c31 352e   C 22.061421,15.
+00002340: 3233 3534 3835 2032 312e 3236 3032 3131  235485 21.260211
+00002350: 2c31 352e 3033 3531 3832 2032 302e 3435  ,15.035182 20.45
+00002360: 3839 3935 2c31 342e 3833 3438 3820 4320  8995,14.83488 C 
+00002370: 3230 2e34 3538 3939 352c 3130 2e36 3236  20.458995,10.626
+00002380: 3430 3120 3230 2e34 3538 3939 352c 362e  401 20.458995,6.
+00002390: 3431 3739 3239 2032 302e 3435 3839 3935  417929 20.458995
+000023a0: 2c32 2e32 3039 3435 3032 2043 2032 312e  ,2.2094502 C 21.
+000023b0: 3330 3036 3934 2c31 2e39 3939 3032 3835  300694,1.9990285
+000023c0: 2032 322e 3134 3233 3838 2c31 2e37 3838   22.142388,1.788
+000023d0: 3630 3034 2032 322e 3938 3430 3831 2c31  6004 22.984081,1
+000023e0: 2e35 3738 3137 3837 2043 2032 322e 3931  .5781787 C 22.91
+000023f0: 3835 3837 2c31 2e33 3931 3532 3433 2032  8587,1.3915243 2
+00002400: 332e 3132 3636 3931 2c30 2e39 3331 3236  3.126691,0.93126
+00002410: 3433 3220 3232 2e38 3538 3839 332c 302e  432 22.858893,0.
+00002420: 3934 3639 3037 3232 2043 2032 312e 3432  94690722 C 21.42
+00002430: 3736 3536 2c30 2e39 3436 3930 3732 3220  7656,0.94690722 
+00002440: 3139 2e39 3936 3431 382c 302e 3934 3639  19.996418,0.9469
+00002450: 3037 3232 2031 382e 3536 3531 382c 302e  0722 18.56518,0.
+00002460: 3934 3639 3037 3232 2043 2031 382e 3536  94690722 C 18.56
+00002470: 3531 382c 352e 3939 3730 3739 3220 3138  518,5.9970792 18
+00002480: 2e35 3635 3138 2c31 312e 3034 3732 3531  .56518,11.047251
+00002490: 2031 382e 3536 3531 382c 3136 2e30 3937   18.56518,16.097
+000024a0: 3432 3320 7a20 2720 7374 796c 653d 2773  423 z ' style='s
+000024b0: 7472 6f6b 653a 2470 6c61 6e65 7473 5f63  troke:$planets_c
+000024c0: 6f6c 6f72 5f37 3b73 7472 6f6b 652d 7769  olor_7;stroke-wi
+000024d0: 6474 683a 3170 783b 2066 696c 6c3a 2470  dth:1px; fill:$p
+000024e0: 6c61 6e65 7473 5f63 6f6c 6f72 5f35 3b27  lanets_color_5;'
+000024f0: 202f 3e0d 0a20 2020 2020 2020 2020 2020   />..           
+00002500: 2020 2020 2020 2020 2020 2020 203c 7061               <pa
+00002510: 7468 2064 3d27 4d20 342e 3034 3539 3335  th d='M 4.045935
+00002520: 362c 382e 3532 3231 3635 3220 4320 392e  6,8.5221652 C 9.
+00002530: 3039 3631 3037 362c 382e 3532 3231 3635  0961076,8.522165
+00002540: 3220 3134 2e31 3436 3238 2c38 2e35 3232  2 14.14628,8.522
+00002550: 3136 3532 2031 392e 3139 3634 3532 2c38  1652 19.196452,8
+00002560: 2e35 3232 3136 3532 204d 2031 312e 3632  .5221652 M 11.62
+00002570: 3131 3934 2c30 2e39 3436 3930 3732 3220  1194,0.94690722 
+00002580: 4320 3131 2e36 3231 3139 342c 362e 3431  C 11.621194,6.41
+00002590: 3739 3239 2031 312e 3632 3131 3934 2c31  7929 11.621194,1
+000025a0: 312e 3838 3839 3434 2031 312e 3632 3131  1.888944 11.6211
+000025b0: 3934 2c31 372e 3335 3939 3636 204d 2031  94,17.359966 M 1
+000025c0: 342e 3134 3632 3432 2c32 302e 3531 3633  4.146242,20.5163
+000025d0: 3432 2043 2031 342e 3232 3739 3534 2c32  42 C 14.227954,2
+000025e0: 322e 3230 3131 3035 2031 322e 3237 3536  2.201105 12.2756
+000025f0: 3635 2c32 332e 3535 3033 3032 2031 302e  65,23.550302 10.
+00002600: 3732 3536 3738 2c32 322e 3838 3330 3233  725678,22.883023
+00002610: 2043 2039 2e31 3339 3537 3636 2c32 322e   C 9.1395766,22.
+00002620: 3334 3836 3936 2038 2e35 3532 3034 3636  348696 8.5520466
+00002630: 2c32 302e 3038 3936 3835 2039 2e37 3033  ,20.089685 9.703
+00002640: 3439 3736 2c31 382e 3836 3038 3731 2043  4976,18.860871 C
+00002650: 2031 302e 3732 3430 3735 2c31 372e 3630   10.724075,17.60
+00002660: 3831 3832 2031 322e 3935 3934 3634 2c31  8182 12.959464,1
+00002670: 372e 3734 3634 3831 2031 332e 3736 3037  7.746481 13.7607
+00002680: 3331 2c31 392e 3137 3438 3038 2043 2031  31,19.174808 C 1
+00002690: 342e 3031 3133 3339 2c31 392e 3537 3431  4.011339,19.5741
+000026a0: 2031 342e 3134 3831 382c 3230 2e30 3434   14.14818,20.044
+000026b0: 3634 3420 3134 2e31 3436 3234 322c 3230  644 14.146242,20
+000026c0: 2e35 3136 3334 3220 7a20 2720 7374 796c  .516342 z ' styl
+000026d0: 653d 2773 7472 6f6b 653a 2470 6c61 6e65  e='stroke:$plane
+000026e0: 7473 5f63 6f6c 6f72 5f37 3b73 7472 6f6b  ts_color_7;strok
+000026f0: 652d 7769 6474 683a 3270 783b 2066 696c  e-width:2px; fil
+00002700: 6c3a 6e6f 6e65 3b27 202f 3e0d 0a20 2020  l:none;' />..   
+00002710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002720: 203c 2f67 3e0d 0a20 2020 2020 2020 2020   </g>..         
+00002730: 2020 2020 2020 203c 2f73 796d 626f 6c3e         </symbol>
+00002740: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002750: 2020 3c73 796d 626f 6c20 6964 3d27 4e65    <symbol id='Ne
+00002760: 7074 756e 6527 3e0d 0a20 2020 2020 2020  ptune'>..       
+00002770: 2020 2020 2020 2020 2020 2020 203c 6720               <g 
+00002780: 7472 616e 7366 6f72 6d3d 2774 7261 6e73  transform='trans
+00002790: 6c61 7465 2832 2c34 2920 7363 616c 6528  late(2,4) scale(
+000027a0: 2e39 2927 2063 6c61 7373 3d27 706c 616e  .9)' class='plan
+000027b0: 6574 5379 6d62 6f6c 273e 0d0a 2020 2020  etSymbol'>..    
+000027c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000027d0: 2020 2020 3c70 6174 6820 643d 274d 2033      <path d='M 3
+000027e0: 2e38 3836 3330 372c 322e 3230 3938 3133  .886307,2.209813
+000027f0: 3420 4320 322e 3237 3238 3234 392c 3133  4 C 2.2728249,13
+00002800: 2e31 3732 3333 3620 342e 3936 3139 3731  .172336 4.961971
+00002810: 382c 3134 2e38 3136 3731 3820 3130 2e33  8,14.816718 10.3
+00002820: 3430 3236 352c 3134 2e38 3136 3731 3820  40265,14.816718 
+00002830: 4320 3135 2e37 3138 3536 372c 3134 2e38  C 15.718567,14.8
+00002840: 3136 3731 3820 3138 2e34 3037 3732 312c  16718 18.407721,
+00002850: 3133 2e31 3732 3333 3620 3136 2e37 3934  13.172336 16.794
+00002860: 3233 312c 322e 3230 3938 3133 3420 4d20  231,2.2098134 M 
+00002870: 3130 2e33 3430 3236 352c 332e 3330 3630  10.340265,3.3060
+00002880: 3635 3820 4c20 3130 2e33 3430 3236 352c  658 L 10.340265,
+00002890: 3233 2e35 3836 3733 3620 4d20 362e 3033  23.586736 M 6.03
+000028a0: 3736 3239 2c31 392e 3230 3137 3237 204c  7629,19.201727 L
+000028b0: 2031 342e 3634 3239 3039 2c31 392e 3230   14.642909,19.20
+000028c0: 3137 3237 204d 2030 2e39 3131 3830 3032  1727 M 0.9118002
+000028d0: 372c 332e 3732 3330 3830 3820 4c20 332e  7,3.7230808 L 3.
+000028e0: 3936 3335 3739 352c 312e 3431 3033 3336  9635795,1.410336
+000028f0: 3120 4c20 362e 3233 3238 3638 392c 342e  1 L 6.2328689,4.
+00002900: 3532 3035 3437 3820 4d20 372e 3539 3938  5205478 M 7.5998
+00002910: 3438 362c 362e 3334 3231 3234 3820 4c20  486,6.3421248 L 
+00002920: 3130 2e32 3539 3035 352c 332e 3537 3133  10.259055,3.5713
+00002930: 3130 3820 4c20 3132 2e39 3737 3831 322c  108 L 12.977812,
+00002940: 362e 3238 3134 3432 3820 4d20 3134 2e34  6.2814428 M 14.4
+00002950: 3037 3838 392c 342e 3731 3230 3532 3820  07889,4.7120528 
+00002960: 4c20 3136 2e37 3135 3934 362c 312e 3633  L 16.715946,1.63
+00002970: 3136 3038 3520 4c20 3139 2e37 3338 3530  16085 L 19.73850
+00002980: 362c 332e 3938 3338 3632 3827 2073 7479  6,3.9838628' sty
+00002990: 6c65 3d27 7374 726f 6b65 3a24 706c 616e  le='stroke:$plan
+000029a0: 6574 735f 636f 6c6f 725f 383b 7374 726f  ets_color_8;stro
+000029b0: 6b65 2d77 6964 7468 3a32 7078 3b20 6669  ke-width:2px; fi
+000029c0: 6c6c 3a6e 6f6e 653b 2720 2f3e 0d0a 2020  ll:none;' />..  
+000029d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000029e0: 2020 3c2f 673e 0d0a 2020 2020 2020 2020    </g>..        
+000029f0: 2020 2020 2020 2020 3c2f 7379 6d62 6f6c          </symbol
+00002a00: 3e0d 0a20 2020 2020 2020 2020 2020 2020  >..             
+00002a10: 2020 203c 7379 6d62 6f6c 2069 643d 2750     <symbol id='P
+00002a20: 6c75 746f 273e 0d0a 2020 2020 2020 2020  luto'>..        
+00002a30: 2020 2020 2020 2020 2020 2020 3c67 2074              <g t
+00002a40: 7261 6e73 666f 726d 3d27 7472 616e 736c  ransform='transl
+00002a50: 6174 6528 302c 3329 2073 6361 6c65 282e  ate(0,3) scale(.
+00002a60: 3929 2720 636c 6173 733d 2770 6c61 6e65  9)' class='plane
+00002a70: 7453 796d 626f 6c27 3e0d 0a20 2020 2020  tSymbol'>..     
+00002a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002a90: 2020 203c 7061 7468 2064 3d27 4d20 372e     <path d='M 7.
+00002aa0: 3239 3838 3338 392c 3138 2e31 3639 3637  2988389,18.16967
+00002ab0: 3120 4c20 3137 2e31 3730 3239 392c 3138  1 L 17.170299,18
+00002ac0: 2e31 3639 3637 3120 4d20 3132 2e32 3334  .169671 M 12.234
+00002ad0: 3536 392c 3233 2e31 3035 3430 3120 4c20  569,23.105401 L 
+00002ae0: 3132 2e32 3334 3536 392c 3132 2e36 3136  12.234569,12.616
+00002af0: 3938 3120 4d20 3136 2e35 3533 3330 392c  981 M 16.553309,
+00002b00: 352e 3231 3333 3630 3920 4320 3136 2e35  5.2133609 C 16.5
+00002b10: 3533 3330 392c 372e 3539 3733 3230 3920  53309,7.5973209 
+00002b20: 3134 2e36 3138 3439 392c 392e 3533 3231  14.618499,9.5321
+00002b30: 3330 3920 3132 2e32 3334 3533 392c 392e  309 12.234539,9.
+00002b40: 3533 3231 3330 3920 4320 392e 3835 3035  5321309 C 9.8505
+00002b50: 3838 392c 392e 3533 3231 3330 3920 372e  889,9.5321309 7.
+00002b60: 3931 3537 3738 392c 372e 3539 3733 3230  9157789,7.597320
+00002b70: 3920 372e 3931 3537 3738 392c 352e 3231  9 7.9157789,5.21
+00002b80: 3333 3630 3920 4320 372e 3931 3537 3738  33609 C 7.915778
+00002b90: 392c 322e 3832 3934 3130 3920 392e 3835  9,2.8294109 9.85
+00002ba0: 3035 3838 392c 302e 3839 3436 3030 3837  05889,0.89460087
+00002bb0: 2031 322e 3233 3435 3339 2c30 2e38 3934   12.234539,0.894
+00002bc0: 3630 3038 3720 4320 3134 2e36 3138 3439  60087 C 14.61849
+00002bd0: 392c 302e 3839 3436 3030 3837 2031 362e  9,0.89460087 16.
+00002be0: 3535 3333 3039 2c32 2e38 3239 3431 3039  553309,2.8294109
+00002bf0: 2031 362e 3535 3333 3039 2c35 2e32 3133   16.553309,5.213
+00002c00: 3336 3039 207a 204d 2031 392e 3633 3831  3609 z M 19.6381
+00002c10: 3339 2c35 2e32 3133 3336 3039 2043 2031  39,5.2133609 C 1
+00002c20: 392e 3633 3831 3339 2c39 2e33 3030 3135  9.638139,9.30015
+00002c30: 3039 2031 362e 3332 3133 3239 2c31 322e  09 16.321329,12.
+00002c40: 3631 3639 3631 2031 322e 3233 3435 3339  616961 12.234539
+00002c50: 2c31 322e 3631 3639 3631 2043 2038 2e31  ,12.616961 C 8.1
+00002c60: 3437 3735 3839 2c31 322e 3631 3639 3631  477589,12.616961
+00002c70: 2034 2e38 3330 3934 3839 2c39 2e33 3030   4.8309489,9.300
+00002c80: 3135 3039 2034 2e38 3330 3934 3839 2c35  1509 4.8309489,5
+00002c90: 2e32 3133 3336 3039 2043 2034 2e38 3330  .2133609 C 4.830
+00002ca0: 3934 3839 2c35 2e32 3133 3336 3039 2034  9489,5.2133609 4
+00002cb0: 2e38 3330 3934 3839 2c35 2e32 3133 3336  .8309489,5.21336
+00002cc0: 3039 2034 2e38 3330 3934 3839 2c35 2e32  09 4.8309489,5.2
+00002cd0: 3133 3336 3039 2720 7374 796c 653d 2773  133609' style='s
+00002ce0: 7472 6f6b 653a 2470 6c61 6e65 7473 5f63  troke:$planets_c
+00002cf0: 6f6c 6f72 5f39 3b20 7374 726f 6b65 2d77  olor_9; stroke-w
+00002d00: 6964 7468 3a32 7078 3b20 6669 6c6c 3a6e  idth:2px; fill:n
+00002d10: 6f6e 653b 2720 2f3e 0d0a 2020 2020 2020  one;' />..      
+00002d20: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+00002d30: 673e 0d0a 2020 2020 2020 2020 2020 2020  g>..            
+00002d40: 2020 2020 3c2f 7379 6d62 6f6c 3e0d 0a20      </symbol>.. 
+00002d50: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00002d60: 7379 6d62 6f6c 2069 643d 274d 6561 6e5f  symbol id='Mean_
+00002d70: 4e6f 6465 273e 0d0a 2020 2020 2020 2020  Node'>..        
+00002d80: 2020 2020 2020 2020 2020 2020 3c67 2074              <g t
+00002d90: 7261 6e73 666f 726d 3d27 7472 616e 736c  ransform='transl
+00002da0: 6174 6528 302c 3329 2720 636c 6173 733d  ate(0,3)' class=
+00002db0: 2770 6c61 6e65 7453 796d 626f 6c27 3e0d  'planetSymbol'>.
+00002dc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002dd0: 2020 2020 2020 2020 203c 7061 7468 2064           <path d
+00002de0: 3d27 4d20 382e 3830 3936 3034 362c 302e  ='M 8.8096046,0.
+00002df0: 3037 3536 3636 3839 3720 4320 362e 3431  075666897 C 6.41
+00002e00: 3537 3533 362c 302e 3636 3132 3339 3632  57536,0.66123962
+00002e10: 2034 2e33 3736 3737 3639 2c32 2e35 3330   4.3767769,2.530
+00002e20: 3638 3337 2033 2e36 3633 3436 3536 2c34  6837 3.6634656,4
+00002e30: 2e39 3030 3735 3134 2043 2033 2e30 3533  .9007514 C 3.053
+00002e40: 3630 3731 2c36 2e36 3830 3932 3634 2033  6071,6.6809264 3
+00002e50: 2e36 3836 3836 3832 2c38 2e36 3233 3839  .6868682,8.62389
+00002e60: 3031 2034 2e35 3837 3839 3838 2c31 302e  01 4.5878988,10.
+00002e70: 3138 3634 3337 2043 2035 2e31 3332 3339  186437 C 5.13239
+00002e80: 3937 2c31 312e 3132 3436 3232 2035 2e39  97,11.124622 5.9
+00002e90: 3631 3537 3533 2c31 312e 3930 3839 3520  615753,11.90895 
+00002ea0: 362e 3139 3037 3330 322c 3133 2e30 3037  6.1907302,13.007
+00002eb0: 3930 3620 4320 362e 3539 3137 3230 322c  906 C 6.5917202,
+00002ec0: 3134 2e34 3834 3438 3820 362e 3438 3837  14.484488 6.4887
+00002ed0: 3135 362c 3136 2e33 3837 3532 3320 352e  156,16.387523 5.
+00002ee0: 3137 3233 3738 382c 3137 2e33 3832 3537  1723788,17.38257
+00002ef0: 3620 4320 342e 3333 3239 3937 342c 3138  6 C 4.3329974,18
+00002f00: 2e30 3533 3431 3320 332e 3037 3735 3734  .053413 3.077574
+00002f10: 312c 3137 2e34 3535 3033 3420 322e 3832  1,17.455034 2.82
+00002f20: 3030 3133 362c 3136 2e34 3831 3139 3620  00136,16.481196 
+00002f30: 4320 322e 3339 3136 3535 322c 3135 2e31  C 2.3916552,15.1
+00002f40: 3030 3739 3320 332e 3332 3331 3839 382c  00793 3.3231898,
+00002f50: 3133 2e33 3936 3435 3620 342e 3737 3933  13.396456 4.7793
+00002f60: 3331 362c 3133 2e31 3633 3830 3620 4320  316,13.163806 C 
+00002f70: 352e 3531 3537 3836 312c 3133 2e34 3438  5.5157861,13.448
+00002f80: 3438 3920 352e 3733 3632 3335 332c 3133  489 5.7362353,13
+00002f90: 2e30 3038 3333 3120 342e 3938 3830 3531  .008331 4.988051
+00002fa0: 2c31 322e 3733 3931 3031 2043 2033 2e34  ,12.739101 C 3.4
+00002fb0: 3736 3736 3936 2c31 312e 3938 3037 3631  767696,11.980761
+00002fc0: 2031 2e32 3433 3138 3936 2c31 322e 3833   1.2431896,12.83
+00002fd0: 3936 3920 312e 3033 3531 3437 362c 3134  969 1.0351476,14
+00002fe0: 2e36 3335 3339 3420 4320 302e 3737 3434  .635394 C 0.7744
+00002ff0: 3537 3135 2c31 362e 3239 3835 3832 2031  5715,16.298582 1
+00003000: 2e39 3532 3838 3437 2c31 372e 3939 3138  .9528847,17.9918
+00003010: 3335 2033 2e35 3839 3539 3633 2c31 382e  35 3.5895963,18.
+00003020: 3335 3734 3539 2043 2035 2e34 3237 3636  357459 C 5.42766
+00003030: 3632 2c31 382e 3939 3431 3635 2037 2e36  62,18.994165 7.6
+00003040: 3636 3138 3339 2c31 372e 3936 3835 3334  661839,17.968534
+00003050: 2038 2e32 3937 3930 3339 2c31 362e 3131   8.2979039,16.11
+00003060: 3031 3632 2043 2038 2e38 3537 3130 3235  0162 C 8.8571025
+00003070: 2c31 342e 3731 3635 3237 2038 2e35 3436  ,14.716527 8.546
+00003080: 3534 3831 2c31 332e 3138 3631 3339 2038  5481,13.186139 8
+00003090: 2e30 3238 3938 3638 2c31 312e 3833 3236  .0289868,11.8326
+000030a0: 3533 2043 2037 2e34 3730 3238 3835 2c31  53 C 7.4702885,1
+000030b0: 302e 3230 3638 3834 2036 2e32 3535 3336  0.206884 6.25536
+000030c0: 3633 2c38 2e38 3730 3936 3734 2035 2e39  63,8.8709674 5.9
+000030d0: 3239 3930 3536 2c37 2e31 3532 3538 3338  299056,7.1525838
+000030e0: 2043 2035 2e34 3931 3436 2c35 2e34 3932   C 5.49146,5.492
+000030f0: 3939 3635 2035 2e38 3837 3534 3938 2c33  9965 5.8875498,3
+00003100: 2e35 3733 3536 3239 2037 2e32 3332 3936  .5735629 7.23296
+00003110: 3037 2c32 2e34 3332 3732 3133 2043 2038  07,2.4327213 C 8
+00003120: 2e37 3338 3835 3931 2c31 2e30 3133 3434  .7388591,1.01344
+00003130: 3531 2031 312e 3331 3839 3331 2c30 2e37  51 11.318931,0.7
+00003140: 3535 3730 3832 2031 322e 3931 3938 3138  557082 12.919818
+00003150: 2c32 2e31 3632 3737 3233 2043 2031 342e  ,2.1627723 C 14.
+00003160: 3839 3131 3734 2c33 2e36 3736 3933 3435  891174,3.6769345
+00003170: 2031 352e 3239 3530 3635 2c36 2e35 3639   15.295065,6.569
+00003180: 3230 3238 2031 342e 3333 3032 3337 2c38  2028 14.330237,8
+00003190: 2e37 3637 3139 3333 2043 2031 332e 3931  .7671933 C 13.91
+000031a0: 3034 3834 2c39 2e39 3139 3336 3538 2031  0484,9.9193658 1
+000031b0: 332e 3135 3433 3533 2c31 302e 3930 3236  3.154353,10.9026
+000031c0: 3739 2031 322e 3631 3538 3737 2c31 312e  79 12.615877,11.
+000031d0: 3939 3132 3939 2043 2031 322e 3033 3830  991299 C 12.0380
+000031e0: 3435 2c31 332e 3534 3832 3620 3132 2e30  45,13.54826 12.0
+000031f0: 3830 3539 392c 3135 2e33 3634 3831 3320  80599,15.364813 
+00003200: 3132 2e37 3737 3435 352c 3136 2e38 3735  12.777455,16.875
+00003210: 3136 3320 4320 3134 2e30 3736 3934 362c  163 C 14.076946,
+00003220: 3139 2e31 3130 3934 3320 3137 2e39 3033  19.110943 17.903
+00003230: 3337 362c 3138 2e39 3435 3033 3320 3139  376,18.945033 19
+00003240: 2e30 3432 3037 382c 3136 2e36 3238 3730  .042078,16.62870
+00003250: 3320 4320 3139 2e37 3537 3234 322c 3135  3 C 19.757242,15
+00003260: 2e32 3631 3232 3720 3139 2e33 3036 3831  .261227 19.30681
+00003270: 392c 3133 2e32 3434 3932 3920 3137 2e37  9,13.244929 17.7
+00003280: 3635 392c 3132 2e36 3731 3930 3220 4320  659,12.671902 C 
+00003290: 3136 2e37 3538 3335 2c31 322e 3231 3039  16.75835,12.2109
+000032a0: 3631 2031 352e 3436 3230 3933 2c31 322e  61 15.462093,12.
+000032b0: 3434 3239 3531 2031 342e 3732 3933 3636  442951 14.729366
+000032c0: 2c31 332e 3239 3030 3134 2043 2031 352e  ,13.290014 C 15.
+000032d0: 3637 3938 3439 2c31 332e 3237 3631 3533  679849,13.276153
+000032e0: 2031 362e 3938 3032 3934 2c31 332e 3236   16.980294,13.26
+000032f0: 3237 3534 2031 372e 3334 3335 3032 2c31  2754 17.343502,1
+00003300: 342e 3336 3432 3033 2043 2031 372e 3930  4.364203 C 17.90
+00003310: 3332 3633 2c31 352e 3439 3236 3739 2031  3263,15.492679 1
+00003320: 372e 3736 3936 3737 2c31 372e 3330 3539  7.769677,17.3059
+00003330: 3732 2031 362e 3431 3439 3439 2c31 372e  72 16.414949,17.
+00003340: 3738 3138 3935 2043 2031 352e 3231 3834  781895 C 15.2184
+00003350: 3138 2c31 382e 3133 3038 3420 3134 2e31  18,18.13084 14.1
+00003360: 3530 3330 332c 3136 2e39 3032 3934 3720  50303,16.902947 
+00003370: 3134 2e30 3932 3138 342c 3135 2e37 3831  14.092184,15.781
+00003380: 3636 3620 4320 3133 2e37 3832 3131 372c  666 C 13.782117,
+00003390: 3134 2e31 3031 3430 3320 3134 2e31 3430  14.101403 14.140
+000033a0: 3334 362c 3132 2e32 3730 3331 3520 3135  346,12.270315 15
+000033b0: 2e32 3735 3139 2c31 302e 3935 3830 3432  .27519,10.958042
+000033c0: 2043 2031 362e 3531 3938 3933 2c39 2e34   C 16.519893,9.4
+000033d0: 3934 3837 3633 2031 372e 3235 3635 3235  948763 17.256525
+000033e0: 2c37 2e35 3234 3036 3539 2031 362e 3836  ,7.5240659 16.86
+000033f0: 3735 3236 2c35 2e35 3939 3437 3531 2043  7526,5.5994751 C
+00003400: 2031 362e 3336 3430 392c 322e 3536 3537   16.36409,2.5657
+00003410: 3234 3920 3133 2e36 3035 3030 312c 302e  249 13.605001,0.
+00003420: 3036 3537 3630 3534 3320 3130 2e35 3037  065760543 10.507
+00003430: 3330 392c 2d30 2e30 3034 3735 3437 3236  309,-0.004754726
+00003440: 3520 4320 392e 3934 3130 3733 2c2d 302e  5 C 9.941073,-0.
+00003450: 3031 3538 3330 3639 3220 392e 3337 3232  015830692 9.3722
+00003460: 3539 342c 302e 3030 3933 3437 3836 3139  594,0.0093478619
+00003470: 2038 2e38 3039 3630 3436 2c30 2e30 3735   8.8096046,0.075
+00003480: 3636 3638 3937 207a 2720 7374 796c 653d  666897 z' style=
+00003490: 2766 696c 6c3a 2024 706c 616e 6574 735f  'fill: $planets_
+000034a0: 636f 6c6f 725f 3130 3b27 202f 3e0d 0a20  color_10;' />.. 
+000034b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000034c0: 2020 203c 2f67 3e0d 0a20 2020 2020 2020     </g>..       
+000034d0: 2020 2020 2020 2020 203c 2f73 796d 626f           </symbo
+000034e0: 6c3e 0d0a 2020 2020 2020 2020 2020 2020  l>..            
+000034f0: 2020 2020 3c73 796d 626f 6c20 6964 3d27      <symbol id='
+00003500: 5472 7565 5f4e 6f64 6527 3e3c 2f73 796d  True_Node'></sym
+00003510: 626f 6c3e 0d0a 2020 2020 2020 2020 2020  bol>..          
+00003520: 2020 2020 2020 3c73 796d 626f 6c20 6964        <symbol id
+00003530: 3d27 3127 3e0d 0a20 2020 2020 2020 2020  ='1'>..         
+00003540: 2020 2020 2020 2020 2020 203c 7465 7874             <text
+00003550: 2079 3d27 3230 2720 7374 796c 653d 2766   y='20' style='f
+00003560: 6f6e 742d 7369 7a65 3a32 3270 783b 2066  ont-size:22px; f
+00003570: 696c 6c3a 2024 706c 616e 6574 735f 636f  ill: $planets_co
+00003580: 6c6f 725f 3132 3b27 3e41 733c 2f74 6578  lor_12;'>As</tex
+00003590: 743e 0d0a 2020 2020 2020 2020 2020 2020  t>..            
+000035a0: 2020 2020 3c2f 7379 6d62 6f6c 3e0d 0a20      </symbol>.. 
+000035b0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+000035c0: 7379 6d62 6f6c 2069 643d 2731 3027 3e0d  symbol id='10'>.
+000035d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000035e0: 2020 2020 203c 7465 7874 2079 3d27 3230       <text y='20
+000035f0: 2720 7374 796c 653d 2766 6f6e 742d 7369  ' style='font-si
+00003600: 7a65 3a32 3070 783b 2066 696c 6c3a 2024  ze:20px; fill: $
+00003610: 706c 616e 6574 735f 636f 6c6f 725f 3133  planets_color_13
+00003620: 3b27 3e4d 633c 2f74 6578 743e 0d0a 2020  ;'>Mc</text>..  
+00003630: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+00003640: 7379 6d62 6f6c 3e0d 0a20 2020 2020 2020  symbol>..       
+00003650: 2020 2020 2020 2020 203c 7379 6d62 6f6c           <symbol
+00003660: 2069 643d 2737 273e 0d0a 2020 2020 2020   id='7'>..      
+00003670: 2020 2020 2020 2020 2020 2020 2020 3c74                <t
+00003680: 6578 7420 793d 2732 3027 2073 7479 6c65  ext y='20' style
+00003690: 3d27 666f 6e74 2d73 697a 653a 3232 7078  ='font-size:22px
+000036a0: 3b20 6669 6c6c 3a20 2470 6c61 6e65 7473  ; fill: $planets
+000036b0: 5f63 6f6c 6f72 5f31 343b 273e 4473 3c2f  _color_14;'>Ds</
+000036c0: 7465 7874 3e0d 0a20 2020 2020 2020 2020  text>..         
+000036d0: 2020 2020 2020 203c 2f73 796d 626f 6c3e         </symbol>
+000036e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000036f0: 2020 3c73 796d 626f 6c20 6964 3d27 3427    <symbol id='4'
+00003700: 3e0d 0a20 2020 2020 2020 2020 2020 2020  >..             
+00003710: 2020 2020 2020 203c 7465 7874 2079 3d27         <text y='
+00003720: 3230 2720 7374 796c 653d 2766 6f6e 742d  20' style='font-
+00003730: 7369 7a65 3a32 3270 783b 2066 696c 6c3a  size:22px; fill:
+00003740: 2024 706c 616e 6574 735f 636f 6c6f 725f   $planets_color_
+00003750: 3135 3b27 3e49 633c 2f74 6578 743e 0d0a  15;'>Ic</text>..
+00003760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003770: 3c2f 7379 6d62 6f6c 3e20 2020 2020 2020  </symbol>       
+00003780: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00003790: 2020 2020 2020 2020 2020 203c 212d 2d20             <!-- 
+000037a0: 5a6f 6469 6163 202d 2d3e 0d0a 2020 2020  Zodiac -->..    
+000037b0: 2020 2020 2020 2020 2020 2020 3c73 796d              <sym
+000037c0: 626f 6c20 6964 3d27 6172 6965 7327 3e0d  bol id='aries'>.
+000037d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000037e0: 2020 2020 203c 7061 7468 2074 7261 6e73       <path trans
+000037f0: 666f 726d 3d22 7363 616c 6528 302e 3829  form="scale(0.8)
+00003800: 2220 643d 274d 2031 342e 3833 3335 3336  " d='M 14.833536
+00003810: 2c33 3120 4320 3134 2e38 3332 3138 362c  ,31 C 14.832186,
+00003820: 3239 2e37 3238 3235 2031 342e 3834 3539  29.72825 14.8459
+00003830: 3336 2c32 382e 3435 3538 3420 3134 2e37  36,28.45584 14.7
+00003840: 3830 3334 362c 3237 2e31 3835 3233 2043  80346,27.18523 C
+00003850: 2031 342e 3634 3039 3236 2c32 342e 3233   14.640926,24.23
+00003860: 3034 3620 3134 2e32 3731 3932 372c 3231  046 14.271927,21
+00003870: 2e32 3839 3739 2031 332e 3736 3136 3537  .28979 13.761657
+00003880: 2c31 382e 3337 3736 2043 2031 332e 3332  ,18.3776 C 13.32
+00003890: 3139 3837 2c31 352e 3931 3931 3120 3132  1987,15.91911 12
+000038a0: 2e37 3837 3738 372c 3133 2e34 3639 3833  .787787,13.46983
+000038b0: 2031 312e 3939 3035 3137 2c31 312e 3130   11.990517,11.10
+000038c0: 3037 3520 4320 3131 2e35 3330 3236 372c  075 C 11.530267,
+000038d0: 392e 3736 3234 3320 3130 2e39 3932 3838  9.76243 10.99288
+000038e0: 372c 382e 3434 3931 3220 3130 2e33 3537  7,8.44912 10.357
+000038f0: 3038 372c 372e 3138 3439 2043 2039 2e37  087,7.1849 C 9.7
+00003900: 3736 3430 3635 2c36 2e30 3534 2039 2e31  764065,6.054 9.1
+00003910: 3134 3334 3635 2c34 2e39 3432 3936 2038  143465,4.94296 8
+00003920: 2e32 3136 3030 3635 2c34 2e30 3334 3934  .2160065,4.03494
+00003930: 2043 2037 2e36 3238 3234 3635 2c33 2e34   C 7.6282465,3.4
+00003940: 3436 3520 362e 3930 3037 3236 352c 322e  465 6.9007265,2.
+00003950: 3934 3533 3520 362e 3036 3439 3736 352c  94535 6.0649765,
+00003960: 322e 3831 3632 3420 4320 352e 3332 3337  2.81624 C 5.3237
+00003970: 3236 362c 322e 3730 3134 3220 342e 3533  266,2.70142 4.53
+00003980: 3034 3636 362c 322e 3837 3537 3120 332e  04666,2.87571 3.
+00003990: 3933 3536 3936 362c 332e 3334 3338 3420  9356966,3.34384 
+000039a0: 4320 332e 3231 3336 3536 352c 332e 3930  C 3.2136565,3.90
+000039b0: 3531 3920 322e 3736 3534 3336 352c 342e  519 2.7654365,4.
+000039c0: 3735 3632 3520 322e 3534 3338 3336 352c  75625 2.5438365,
+000039d0: 352e 3633 3238 3920 4320 322e 3330 3533  5.63289 C 2.3053
+000039e0: 3736 352c 362e 3539 3939 3520 322e 3239  765,6.59995 2.29
+000039f0: 3539 3736 352c 372e 3631 3335 3820 322e  59765,7.61358 2.
+00003a00: 3432 3932 3136 352c 382e 3539 3733 2043  4292165,8.5973 C
+00003a10: 2032 2e36 3436 3434 3635 2c31 302e 3135   2.6464465,10.15
+00003a20: 3538 3720 332e 3236 3839 3636 352c 3131  587 3.2689665,11
+00003a30: 2e36 3332 3538 2034 2e30 3831 3534 3636  .63258 4.0815466
+00003a40: 2c31 322e 3936 3930 3820 4320 332e 3239  ,12.96908 C 3.29
+00003a50: 3234 3436 352c 3132 2e39 3639 3038 2032  24465,12.96908 2
+00003a60: 2e35 3033 3334 3635 2c31 322e 3936 3930  .5033465,12.9690
+00003a70: 3820 312e 3731 3432 3436 352c 3132 2e39  8 1.7142465,12.9
+00003a80: 3639 3038 2043 2030 2e38 3937 3234 3635  6908 C 0.8972465
+00003a90: 312c 3131 2e34 3834 3831 2030 2e32 3537  1,11.48481 0.257
+00003aa0: 3939 3635 312c 392e 3837 3239 3920 302e  99651,9.87299 0.
+00003ab0: 3036 3032 3536 3531 342c 382e 3137 3839  060256514,8.1789
+00003ac0: 3920 4320 2d30 2e30 3731 3230 3334 3836  9 C -0.071203486
+00003ad0: 2c37 2e30 3036 3935 2030 2e30 3033 3731  ,7.00695 0.00371
+00003ae0: 3635 3133 382c 352e 3739 3930 3320 302e  65138,5.79903 0.
+00003af0: 3337 3134 3936 3531 2c34 2e36 3734 3231  37149651,4.67421
+00003b00: 2043 2030 2e37 3634 3432 3635 312c 332e   C 0.76442651,3.
+00003b10: 3437 3439 3920 312e 3531 3935 3836 352c  47499 1.5195865,
+00003b20: 322e 3339 3332 2032 2e35 3233 3235 3635  2.3932 2.5232565
+00003b30: 2c31 2e36 3330 3420 4320 332e 3238 3039  ,1.6304 C 3.2809
+00003b40: 3636 352c 312e 3035 3437 3820 342e 3230  665,1.05478 4.20
+00003b50: 3539 3336 362c 302e 3731 3236 3820 352e  59366,0.71268 5.
+00003b60: 3135 3139 3436 362c 302e 3633 3738 3120  1519466,0.63781 
+00003b70: 4320 362e 3139 3338 3236 352c 302e 3534  C 6.1938265,0.54
+00003b80: 3439 3620 372e 3236 3130 3436 352c 302e  496 7.2610465,0.
+00003b90: 3734 3631 3920 382e 3139 3039 3236 352c  74619 8.1909265,
+00003ba0: 312e 3232 3937 3620 4320 392e 3339 3938  1.22976 C 9.3998
+00003bb0: 3636 352c 312e 3835 3032 3120 3130 2e33  665,1.85021 10.3
+00003bc0: 3633 3637 372c 322e 3835 3934 3420 3131  63677,2.85944 11
+00003bd0: 2e31 3435 3237 372c 332e 3935 3736 3620  .145277,3.95766 
+00003be0: 4320 3132 2e31 3930 3334 372c 352e 3434  C 12.190347,5.44
+00003bf0: 3134 3720 3132 2e39 3635 3036 372c 372e  147 12.965067,7.
+00003c00: 3130 3130 3120 3133 2e35 3834 3238 372c  10101 13.584287,
+00003c10: 382e 3830 3338 3220 4320 3134 2e36 3330  8.80382 C 14.630
+00003c20: 3736 362c 3131 2e37 3137 3620 3135 2e32  766,11.7176 15.2
+00003c30: 3132 3632 362c 3134 2e37 3738 3631 2031  12626,14.77861 1
+00003c40: 352e 3537 3531 3436 2c31 372e 3834 3739  5.575146,17.8479
+00003c50: 3520 4320 3135 2e36 3634 3833 362c 3138  5 C 15.664836,18
+00003c60: 2e36 3136 3438 2031 352e 3733 3935 3536  .61648 15.739556
+00003c70: 2c31 392e 3338 3637 3520 3135 2e38 3031  ,19.38675 15.801
+00003c80: 3434 362c 3230 2e31 3538 3033 2043 2031  446,20.15803 C 1
+00003c90: 352e 3933 3336 3036 2c32 302e 3135 3830  5.933606,20.1580
+00003ca0: 3320 3136 2e30 3635 3737 362c 3230 2e31  3 16.065776,20.1
+00003cb0: 3538 3033 2031 362e 3139 3739 3336 2c32  5803 16.197936,2
+00003cc0: 302e 3135 3830 3320 4320 3136 2e34 3331  0.15803 C 16.431
+00003cd0: 3531 362c 3136 2e37 3833 3332 2031 362e  516,16.78332 16.
+00003ce0: 3931 3930 3636 2c31 332e 3430 3736 3120  919066,13.40761 
+00003cf0: 3137 2e39 3230 3233 362c 3130 2e31 3730  17.920236,10.170
+00003d00: 3239 2043 2031 382e 3533 3637 3436 2c38  29 C 18.536746,8
+00003d10: 2e31 3938 3836 2031 392e 3334 3332 3136  .19886 19.343216
+00003d20: 2c36 2e32 3733 3320 3230 2e34 3630 3130  ,6.2733 20.46010
+00003d30: 362c 342e 3533 3230 3920 4320 3231 2e32  6,4.53209 C 21.2
+00003d40: 3332 3936 362c 332e 3334 3234 3620 3232  32966,3.34246 22
+00003d50: 2e31 3738 3339 362c 322e 3232 3639 3120  .178396,2.22691 
+00003d60: 3233 2e33 3933 3233 362c 312e 3437 3437  23.393236,1.4747
+00003d70: 3320 4320 3234 2e33 3033 3934 362c 302e  3 C 24.303946,0.
+00003d80: 3930 3620 3235 2e33 3735 3430 362c 302e  906 25.375406,0.
+00003d90: 3539 3331 3520 3236 2e34 3439 3833 362c  59315 26.449836,
+00003da0: 302e 3631 3734 3420 4320 3237 2e34 3036  0.61744 C 27.406
+00003db0: 3037 362c 302e 3632 3635 2032 382e 3336  076,0.6265 28.36
+00003dc0: 3633 3336 2c30 2e38 3834 3134 2032 392e  6336,0.88414 29.
+00003dd0: 3137 3333 3836 2c31 2e34 3035 3731 2043  173386,1.40571 C
+00003de0: 2032 392e 3931 3832 3736 2c31 2e38 3834   29.918276,1.884
+00003df0: 3137 2033 302e 3533 3637 3236 2c32 2e35  17 30.536726,2.5
+00003e00: 3438 3235 2033 312e 3030 3733 3036 2c33  4825 31.007306,3
+00003e10: 2e32 3936 3838 2043 2033 312e 3634 3033  .29688 C 31.6403
+00003e20: 3736 2c34 2e33 3039 3831 2033 312e 3934  76,4.30981 31.94
+00003e30: 3237 3836 2c35 2e35 3033 3620 3331 2e39  2786,5.5036 31.9
+00003e40: 3930 3532 362c 362e 3639 3134 3920 4320  90526,6.69149 C 
+00003e50: 3332 2e30 3634 3336 362c 382e 3234 3839  32.064366,8.2489
+00003e60: 3820 3331 2e37 3030 3330 362c 392e 3739  8 31.700306,9.79
+00003e70: 3834 3120 3331 2e31 3138 3133 362c 3131  841 31.118136,11
+00003e80: 2e32 3334 3039 2043 2033 302e 3837 3830  .23409 C 30.8780
+00003e90: 3536 2c31 312e 3832 3737 3420 3330 2e36  56,11.82774 30.6
+00003ea0: 3030 3734 362c 3132 2e34 3035 3834 2033  00746,12.40584 3
+00003eb0: 302e 3239 3637 3936 2c31 322e 3936 3930  0.296796,12.9690
+00003ec0: 3820 4320 3239 2e35 3033 3830 362c 3132  8 C 29.503806,12
+00003ed0: 2e39 3639 3038 2032 382e 3731 3038 3236  .96908 28.710826
+00003ee0: 2c31 322e 3936 3930 3820 3237 2e39 3137  ,12.96908 27.917
+00003ef0: 3833 362c 3132 2e39 3639 3038 2043 2032  836,12.96908 C 2
+00003f00: 382e 3639 3536 3436 2c31 312e 3536 3832  8.695646,11.5682
+00003f10: 3520 3239 2e33 3330 3930 362c 3130 2e30  5 29.330906,10.0
+00003f20: 3630 3434 2032 392e 3536 3537 3536 2c38  6044 29.565756,8
+00003f30: 2e34 3634 3835 2043 2032 392e 3730 3534  .46485 C 29.7054
+00003f40: 3336 2c37 2e34 3930 3533 2032 392e 3638  36,7.49053 29.68
+00003f50: 3939 3736 2c36 2e34 3837 3339 2032 392e  9976,6.48739 29.
+00003f60: 3436 3937 3336 2c35 2e35 3236 3136 2043  469736,5.52616 C
+00003f70: 2032 392e 3236 3635 3836 2c34 2e36 3732   29.266586,4.672
+00003f80: 3936 2032 382e 3837 3039 3536 2c33 2e38  96 28.870956,3.8
+00003f90: 3333 3534 2032 382e 3230 3132 3736 2c33  3354 28.201276,3
+00003fa0: 2e32 3530 3739 2043 2032 372e 3731 3833  .25079 C 27.7183
+00003fb0: 3836 2c32 2e38 3232 3633 2032 372e 3037  86,2.82263 27.07
+00003fc0: 3834 3636 2c32 2e35 3930 3231 2032 362e  8466,2.59021 26.
+00003fd0: 3433 3632 3136 2c32 2e35 3834 3436 2043  436216,2.58446 C
+00003fe0: 2032 352e 3638 3033 3036 2c32 2e35 3630   25.680306,2.560
+00003ff0: 3539 2032 342e 3935 3030 3836 2c32 2e38  59 24.950086,2.8
+00004000: 3733 3033 2032 342e 3335 3833 3336 2c33  7303 24.358336,3
+00004010: 2e33 3238 3739 2043 2032 332e 3439 3435  .32879 C 23.4945
+00004020: 3536 2c33 2e39 3933 3037 2032 322e 3834  56,3.99307 22.84
+00004030: 3439 3836 2c34 2e38 3931 3938 2032 322e  4986,4.89198 22.
+00004040: 3238 3239 3536 2c35 2e38 3136 3739 2043  282956,5.81679 C
+00004050: 2032 312e 3435 3137 3536 2c37 2e32 3130   21.451756,7.210
+00004060: 3732 2032 302e 3831 3134 3336 2c38 2e37  72 20.811436,8.7
+00004070: 3130 3138 2032 302e 3235 3033 3936 2c31  1018 20.250396,1
+00004080: 302e 3233 3132 3420 4320 3139 2e34 3337  0.23124 C 19.437
+00004090: 3538 362c 3132 2e34 3938 3032 2031 382e  586,12.49802 18.
+000040a0: 3839 3333 3236 2c31 342e 3835 3136 3620  893326,14.85166 
+000040b0: 3138 2e34 3430 3238 362c 3137 2e32 3134  18.440286,17.214
+000040c0: 3332 2043 2031 372e 3833 3930 3136 2c32  32 C 17.839016,2
+000040d0: 302e 3430 3332 3520 3137 2e34 3133 3231  0.40325 17.41321
+000040e0: 362c 3233 2e36 3239 3120 3137 2e32 3436  6,23.6291 17.246
+000040f0: 3133 362c 3236 2e38 3731 3520 4320 3137  136,26.8715 C 17
+00004100: 2e31 3833 3739 362c 3238 2e30 3138 3537  .183796,28.01857
+00004110: 2031 372e 3137 3339 3636 2c32 392e 3136   17.173966,29.16
+00004120: 3734 3520 3137 2e31 3737 3531 362c 3330  745 17.177516,30
+00004130: 2e33 3135 3935 2043 2031 372e 3137 3735  .31595 C 17.1775
+00004140: 3136 2c33 302e 3534 3339 3720 3137 2e31  16,30.54397 17.1
+00004150: 3737 3531 362c 3330 2e37 3731 3938 2031  77516,30.77198 1
+00004160: 372e 3137 3735 3136 2c33 3120 4320 3136  7.177516,31 C 16
+00004170: 2e33 3936 3138 362c 3331 2031 352e 3631  .396186,31 15.61
+00004180: 3438 3536 2c33 3120 3134 2e38 3333 3533  4856,31 14.83353
+00004190: 362c 3331 207a 2720 7374 796c 653d 2766  6,31 z' style='f
+000041a0: 696c 6c3a 2024 7a6f 6469 6163 5f63 6f6c  ill: $zodiac_col
+000041b0: 6f72 5f30 3b27 202f 3e0d 0a20 2020 2020  or_0;' />..     
+000041c0: 2020 2020 2020 2020 2020 203c 2f73 796d             </sym
+000041d0: 626f 6c3e 0d0a 2020 2020 2020 2020 2020  bol>..          
+000041e0: 2020 2020 2020 3c73 796d 626f 6c20 6964        <symbol id
+000041f0: 3d27 7461 7572 7573 273e 0d0a 2020 2020  ='taurus'>..    
+00004200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004210: 3c70 6174 6820 7472 616e 7366 6f72 6d3d  <path transform=
+00004220: 2273 6361 6c65 2830 2e38 2922 2064 3d27  "scale(0.8)" d='
+00004230: 4d20 3131 2e32 3131 3132 352c 3131 2e39  M 11.211125,11.9
+00004240: 3630 3034 3320 4320 392e 3938 3536 3139  60043 C 9.985619
+00004250: 372c 3131 2e34 3832 3038 3520 382e 3832  7,11.482085 8.82
+00004260: 3733 3530 372c 3130 2e37 3537 3236 3320  73507,10.757263 
+00004270: 372e 3939 3934 3136 342c 392e 3732 3236  7.9994164,9.7226
+00004280: 3620 4320 362e 3935 3430 3538 342c 382e  6 C 6.9540584,8.
+00004290: 3434 3839 3530 3820 362e 3231 3139 3532  4489508 6.211952
+000042a0: 342c 362e 3936 3936 3039 3720 352e 3430  4,6.9696097 5.40
+000042b0: 3638 3139 392c 352e 3534 3232 3531 3520  68199,5.5422515 
+000042c0: 4320 342e 3931 3533 3333 362c 342e 3634  C 4.9153336,4.64
+000042d0: 3335 3933 3120 342e 3335 3838 3435 322c  35931 4.3588452,
+000042e0: 332e 3736 3034 3132 3820 332e 3630 3032  3.7604128 3.6002
+000042f0: 3638 362c 332e 3036 3031 3033 3620 4320  686,3.0601036 C 
+00004300: 332e 3038 3737 3337 312c 322e 3538 3330  3.0877371,2.5830
+00004310: 3339 3920 322e 3436 3939 3433 332c 322e  399 2.4699433,2.
+00004320: 3139 3737 3132 3920 312e 3737 3931 3332  1977129 1.779132
+00004330: 312c 322e 3034 3632 3137 3820 4320 312e  1,2.0462178 C 1.
+00004340: 3435 3134 3836 372c 312e 3936 3633 3435  4514867,1.966345
+00004350: 3120 312e 3131 3237 3639 382c 312e 3936  1 1.1127698,1.96
+00004360: 3334 3036 3520 302e 3737 3735 3636 3438  34065 0.77756648
+00004370: 2c31 2e39 3639 3332 3033 2043 2030 2e36  ,1.9693203 C 0.6
+00004380: 3737 3530 3133 382c 312e 3938 3234 3830  7750138,1.982480
+00004390: 3320 302e 3539 3833 3335 3038 2c31 2e39  3 0.59833508,1.9
+000043a0: 3734 3735 3935 2030 2e36 3333 3639 3038  747595 0.6336908
+000043b0: 382c 312e 3835 3238 3333 3320 4320 302e  8,1.8528333 C 0.
+000043c0: 3633 3336 3930 3838 2c31 2e32 3730 3336  63369088,1.27036
+000043d0: 3138 2030 2e36 3333 3639 3038 382c 302e  18 0.63369088,0.
+000043e0: 3638 3738 3930 3233 2030 2e36 3333 3639  68789023 0.63369
+000043f0: 3038 382c 302e 3130 3534 3030 3434 2043  088,0.10540044 C
+00004400: 2031 2e31 3736 3933 2c30 2e31 3131 3738   1.17693,0.11178
+00004410: 3838 3420 312e 3732 3130 3239 322c 302e  884 1.7210292,0.
+00004420: 3039 3031 3539 3634 3120 322e 3236 3336  090159641 2.2636
+00004430: 3039 352c 302e 3132 3136 3939 3834 2043  095,0.12169984 C
+00004440: 2033 2e33 3439 3337 3339 2c30 2e32 3132   3.3493739,0.212
+00004450: 3038 3539 3420 342e 3336 3635 3132 392c  08594 4.3665129,
+00004460: 302e 3731 3538 3731 3231 2035 2e31 3931  0.71587121 5.191
+00004470: 3739 3335 2c31 2e34 3039 3735 3535 2043  7935,1.4097555 C
+00004480: 2036 2e32 3634 3738 3434 2c32 2e33 3031   6.2647844,2.301
+00004490: 3333 3220 372e 3038 3838 3735 342c 332e  332 7.0888754,3.
+000044a0: 3434 3934 3832 3720 372e 3739 3131 3631  4494827 7.791161
+000044b0: 342c 342e 3634 3336 3437 3920 4320 382e  4,4.6436479 C 8.
+000044c0: 3239 3133 3033 342c 352e 3530 3436 3838  2913034,5.504688
+000044d0: 2038 2e37 3732 3137 3537 2c36 2e33 3736   8.7721757,6.376
+000044e0: 3735 3235 2039 2e32 3734 3331 3237 2c37  7525 9.2743127,7
+000044f0: 2e32 3336 3630 3632 2043 2039 2e37 3538  .2366062 C 9.758
+00004500: 3830 3837 2c38 2e30 3436 3335 3639 2031  8087,8.0463569 1
+00004510: 302e 3330 3736 3438 2c38 2e38 3234 3738  0.307648,8.82478
+00004520: 3635 2031 302e 3937 3135 3339 2c39 2e34  65 10.971539,9.4
+00004530: 3938 3939 3438 2043 2031 312e 3535 3837  989948 C 11.5587
+00004540: 3137 2c31 302e 3039 3436 3939 2031 322e  17,10.094699 12.
+00004550: 3236 3135 372c 3130 2e35 3836 3936 3720  26157,10.586967 
+00004560: 3133 2e30 3532 3934 2c31 302e 3837 3131  13.05294,10.8711
+00004570: 3339 2043 2031 342e 3135 3039 3636 2c31  39 C 14.150966,1
+00004580: 312e 3237 3633 3632 2031 352e 3333 3930  1.276362 15.3390
+00004590: 3436 2c31 312e 3335 3935 3536 2031 362e  46,11.359556 16.
+000045a0: 3530 3032 3434 2c31 312e 3331 3436 3337  500244,11.314637
+000045b0: 2043 2031 372e 3534 3332 3034 2c31 312e   C 17.543204,11.
+000045c0: 3236 3236 3732 2031 382e 3630 3230 3638  262672 18.602068
+000045d0: 2c31 312e 3036 3936 3136 2031 392e 3532  ,11.069616 19.52
+000045e0: 3937 3932 2c31 302e 3537 3137 3435 2043  9792,10.571745 C
+000045f0: 2032 302e 3430 3133 3335 2c31 302e 3131   20.401335,10.11
+00004600: 3436 3637 2032 312e 3130 3338 3034 2c39  4667 21.103804,9
+00004610: 2e33 3937 3039 3134 2032 312e 3730 3030  .3970914 21.7000
+00004620: 342c 382e 3632 3637 3635 3920 4320 3232  4,8.6267659 C 22
+00004630: 2e33 3835 3038 372c 372e 3734 3131 3934  .385087,7.741194
+00004640: 3620 3232 2e39 3036 3937 2c36 2e37 3437  6 22.90697,6.747
+00004650: 3733 3331 2032 332e 3437 3237 2c35 2e37  7331 23.4727,5.7
+00004660: 3835 3930 3331 2043 2032 332e 3937 3332  859031 C 23.9732
+00004670: 3939 2c34 2e39 3332 3134 3538 2032 342e  99,4.9321458 24.
+00004680: 3434 3535 3136 2c34 2e30 3538 3630 3238  445516,4.0586028
+00004690: 2032 352e 3033 3232 3931 2c33 2e32 3538   25.032291,3.258
+000046a0: 3930 3931 2043 2032 352e 3731 3138 3636  9091 C 25.711866
+000046b0: 2c32 2e33 3234 3738 3633 2032 362e 3531  ,2.3247863 26.51
+000046c0: 3636 3332 2c31 2e34 3535 3832 3437 2032  6632,1.4558247 2
+000046d0: 372e 3530 3737 3636 2c30 2e38 3435 3939  7.507766,0.84599
+000046e0: 3237 3720 4320 3238 2e32 3636 3437 312c  277 C 28.266471,
+000046f0: 302e 3338 3332 3338 3934 2032 392e 3134  0.38323894 29.14
+00004700: 3633 3737 2c30 2e30 3936 3534 3830 3431  6377,0.096548041
+00004710: 2033 302e 3034 3038 3332 2c30 2e31 3036   30.040832,0.106
+00004720: 3635 3938 3420 4320 3330 2e34 3530 3432  65984 C 30.45042
+00004730: 362c 302e 3130 3230 3630 3234 2033 302e  6,0.10206024 30.
+00004740: 3836 3030 3734 2c30 2e31 3037 3933 3735  860074,0.1079375
+00004750: 3420 3331 2e32 3639 3636 372c 302e 3130  4 31.269667,0.10
+00004760: 3534 3030 3434 2043 2033 312e 3236 3936  540044 C 31.2696
+00004770: 3637 2c30 2e37 3236 3731 3331 3520 3331  67,0.72671315 31
+00004780: 2e32 3639 3636 372c 312e 3334 3830 3235  .269667,1.348025
+00004790: 3820 3331 2e32 3639 3636 372c 312e 3936  8 31.269667,1.96
+000047a0: 3933 3230 3320 4320 3330 2e38 3336 3534  93203 C 30.83654
+000047b0: 2c31 2e39 3636 3130 3738 2033 302e 3339  ,1.9661078 30.39
+000047c0: 3533 3631 2c31 2e39 3538 3336 3838 2032  5361,1.9583688 2
+000047d0: 392e 3937 3630 3638 2c32 2e30 3834 3035  9.976068,2.08405
+000047e0: 3520 4320 3239 2e31 3139 3933 342c 322e  5 C 29.119934,2.
+000047f0: 3331 3836 3731 3820 3238 2e34 3030 3438  3186718 28.40048
+00004800: 332c 322e 3839 3235 3634 3620 3237 2e38  3,2.8925646 27.8
+00004810: 3236 3933 392c 332e 3535 3137 3639 3320  26939,3.5517693 
+00004820: 4320 3237 2e32 3336 3032 382c 342e 3232  C 27.236028,4.22
+00004830: 3335 3836 3520 3236 2e37 3838 3236 312c  35865 26.788261,
+00004840: 352e 3030 3238 3337 3420 3236 2e33 3631  5.0028374 26.361
+00004850: 3636 362c 352e 3738 3433 3639 3920 4320  666,5.7843699 C 
+00004860: 3235 2e36 3233 3131 2c37 2e31 3031 3038  25.62311,7.10108
+00004870: 3139 2032 342e 3932 3631 3638 2c38 2e34  19 24.926168,8.4
+00004880: 3534 3339 2032 332e 3937 3439 3436 2c39  5439 23.974946,9
+00004890: 2e36 3335 3732 3337 2043 2032 332e 3539  .6357237 C 23.59
+000048a0: 3335 3534 2c31 302e 3131 3532 3838 2032  3554,10.115288 2
+000048b0: 332e 3135 3231 3138 2c31 302e 3534 3738  3.152118,10.5478
+000048c0: 3136 2032 322e 3635 3235 3036 2c31 302e  16 22.652506,10.
+000048d0: 3930 3433 3431 2043 2032 322e 3034 3938  904341 C 22.0498
+000048e0: 312c 3131 2e33 3431 3236 3720 3231 2e33  1,11.341267 21.3
+000048f0: 3833 3337 352c 3131 2e36 3835 3332 3620  83375,11.685326 
+00004900: 3230 2e36 3932 3231 362c 3131 2e39 3630  20.692216,11.960
+00004910: 3034 3320 4320 3232 2e33 3438 3938 312c  043 C 22.348981,
+00004920: 3132 2e38 3635 3235 3420 3233 2e38 3238  12.865254 23.828
+00004930: 3330 382c 3134 2e31 3232 3634 3620 3234  308,14.122646 24
+00004940: 2e38 3936 3333 392c 3135 2e36 3834 3033  .896339,15.68403
+00004950: 3120 4320 3235 2e37 3936 3530 342c 3136  1 C 25.796504,16
+00004960: 2e39 3836 3038 3720 3236 2e33 3934 3331  .986087 26.39431
+00004970: 342c 3138 2e34 3939 3135 3820 3236 2e35  4,18.499158 26.5
+00004980: 3932 3934 332c 3230 2e30 3730 3039 2043  92943,20.07009 C
+00004990: 2032 362e 3738 3636 3332 2c32 312e 3535   26.786632,21.55
+000049a0: 3231 3531 2032 362e 3637 3934 3438 2c32  2151 26.679448,2
+000049b0: 332e 3037 3737 3820 3236 2e32 3436 3339  3.07778 26.24639
+000049c0: 342c 3234 2e35 3130 3139 3420 4320 3235  4,24.510194 C 25
+000049d0: 2e37 3934 3132 352c 3235 2e39 3931 3033  .794125,25.99103
+000049e0: 3220 3234 2e39 3736 3338 342c 3237 2e33  2 24.976384,27.3
+000049f0: 3439 3530 3520 3233 2e39 3235 3937 352c  49505 23.925975,
+00004a00: 3238 2e34 3835 3030 3720 4320 3232 2e36  28.485007 C 22.6
+00004a10: 3635 3634 362c 3239 2e38 3636 3135 2032  65646,29.86615 2
+00004a20: 312e 3038 3539 3938 2c33 302e 3938 3437  1.085998,30.9847
+00004a30: 3332 2031 392e 3330 3132 3432 2c33 312e  32 19.301242,31.
+00004a40: 3537 3639 3332 2043 2031 372e 3535 3232  576932 C 17.5522
+00004a50: 3038 2c33 322e 3135 3734 3134 2031 352e  08,32.157414 15.
+00004a60: 3635 3238 3032 2c33 322e 3234 3636 3134  652802,32.246614
+00004a70: 2031 332e 3834 3630 3836 2c33 312e 3930   13.846086,31.90
+00004a80: 3237 3536 2043 2031 322e 3232 3031 3933  2756 C 12.220193
+00004a90: 2c33 312e 3538 3434 3839 2031 302e 3638  ,31.584489 10.68
+00004aa0: 3537 3635 2c33 302e 3834 3538 3520 392e  5765,30.84585 9.
+00004ab0: 3430 3038 3736 372c 3239 2e38 3035 3632  4008767,29.80562
+00004ac0: 3520 4320 382e 3330 3031 3432 342c 3238  5 C 8.3001424,28
+00004ad0: 2e39 3233 3330 3320 372e 3333 3534 3639  .923303 7.335469
+00004ae0: 342c 3237 2e38 3631 3831 3520 362e 3630  4,27.861815 6.60
+00004af0: 3637 3737 342c 3236 2e36 3532 3935 3620  67774,26.652956 
+00004b00: 4320 352e 3834 3135 3032 372c 3235 2e33  C 5.8415027,25.3
+00004b10: 3735 3233 3120 352e 3337 3036 3538 392c  75231 5.3706589,
+00004b20: 3233 2e39 3233 3431 3520 352e 3234 3738  23.923415 5.2478
+00004b30: 3436 382c 3232 2e34 3339 3731 3220 4320  468,22.439712 C 
+00004b40: 352e 3038 3233 3538 382c 3230 2e35 3936  5.0823588,20.596
+00004b50: 3620 352e 3339 3339 3931 352c 3138 2e37  6 5.3939915,18.7
+00004b60: 3031 3435 2036 2e32 3136 3237 3034 2c31  0145 6.2162704,1
+00004b70: 372e 3033 3732 3132 2043 2037 2e31 3136  7.037212 C 7.116
+00004b80: 3633 3634 2c31 352e 3139 3133 3632 2038  6364,15.191362 8
+00004b90: 2e35 3634 3332 3234 2c31 332e 3633 3439  .5643224,13.6349
+00004ba0: 3935 2031 302e 3238 3335 3436 2c31 322e  95 10.283546,12.
+00004bb0: 3531 3735 3633 2043 2031 302e 3538 3532  517563 C 10.5852
+00004bc0: 3937 2c31 322e 3331 3937 3434 2031 302e  97,12.319744 10.
+00004bd0: 3839 3530 3038 2c31 322e 3133 3430 3632  895008,12.134062
+00004be0: 2031 312e 3231 3131 3235 2c31 312e 3936   11.211125,11.96
+00004bf0: 3030 3433 207a 204d 2031 352e 3935 3739  0043 z M 15.9579
+00004c00: 322c 3239 2e36 3035 3330 3520 4320 3137  2,29.605305 C 17
+00004c10: 2e34 3639 3637 342c 3239 2e36 3133 3933  .469674,29.61393
+00004c20: 3820 3138 2e39 3935 3730 332c 3239 2e32  8 18.995703,29.2
+00004c30: 3238 3036 3420 3230 2e32 3737 3937 342c  28064 20.277974,
+00004c40: 3238 2e34 3138 3133 2043 2032 312e 3238  28.41813 C 21.28
+00004c50: 3234 3331 2c32 372e 3738 3934 3632 2032  2431,27.789462 2
+00004c60: 322e 3135 3336 3237 2c32 362e 3935 3235  2.153627,26.9525
+00004c70: 3333 2032 322e 3833 3739 3432 2c32 352e  33 22.837942,25.
+00004c80: 3938 3737 3635 2043 2032 332e 3539 3634  987765 C 23.5964
+00004c90: 3038 2c32 342e 3930 3135 3236 2032 342e  08,24.901526 24.
+00004ca0: 3035 3635 3833 2c32 332e 3631 3237 3935  056583,23.612795
+00004cb0: 2032 342e 3136 3031 3434 2c32 322e 3239   24.160144,22.29
+00004cc0: 3332 3138 2043 2032 342e 3239 3937 3535  3218 C 24.299755
+00004cd0: 2c32 302e 3639 3333 3031 2032 342e 3030  ,20.693301 24.00
+00004ce0: 3932 3232 2c31 392e 3033 3638 3032 2032  9222,19.036802 2
+00004cf0: 332e 3231 3332 3034 2c31 372e 3633 3037  3.213204,17.6307
+00004d00: 3831 2043 2032 322e 3633 3532 3836 2c31  81 C 22.635286,1
+00004d10: 362e 3539 3739 3320 3231 2e38 3233 3731  6.59793 21.82371
+00004d20: 322c 3135 2e37 3031 3935 3520 3230 2e38  2,15.701955 20.8
+00004d30: 3832 3335 342c 3134 2e39 3836 3232 3320  82354,14.986223 
+00004d40: 4320 3139 2e39 3537 3836 392c 3134 2e32  C 19.957869,14.2
+00004d50: 3835 3731 3320 3138 2e38 3734 3333 372c  85713 18.874337,
+00004d60: 3133 2e37 3936 3536 3620 3137 2e37 3334  13.796566 17.734
+00004d70: 3830 372c 3133 2e35 3732 3931 3920 4320  807,13.572919 C 
+00004d80: 3136 2e35 3630 3537 392c 3133 2e33 3339  16.560579,13.339
+00004d90: 3330 3620 3135 2e33 3339 3535 392c 3133  306 15.339559,13
+00004da0: 2e33 3435 3534 3820 3134 2e31 3635 3434  .345548 14.16544
+00004db0: 312c 3133 2e35 3736 3037 3720 4320 3132  1,13.576077 C 12
+00004dc0: 2e38 3832 3031 372c 3133 2e38 3336 3438  .882017,13.83648
+00004dd0: 3420 3131 2e36 3730 3834 322c 3134 2e34  4 11.670842,14.4
+00004de0: 3238 3030 3920 3130 2e36 3731 3233 342c  28009 10.671234,
+00004df0: 3135 2e32 3731 3138 2043 2039 2e34 3337  15.27118 C 9.437
+00004e00: 3437 3637 2c31 362e 3239 3439 3034 2038  4767,16.294904 8
+00004e10: 2e34 3639 3038 3834 2c31 372e 3636 3339  .4690884,17.6639
+00004e20: 3634 2038 2e30 3239 3335 3534 2c31 392e  64 8.0293554,19.
+00004e30: 3231 3137 3838 2043 2037 2e36 3533 3135  211788 C 7.65315
+00004e40: 3934 2c32 302e 3532 3336 3633 2037 2e36  94,20.523663 7.6
+00004e50: 3133 3333 3834 2c32 312e 3932 3637 3832  133384,21.926782
+00004e60: 2037 2e38 3834 3233 3534 2c32 332e 3236   7.8842354,23.26
+00004e70: 3235 3439 2043 2038 2e31 3530 3934 3134  2549 C 8.1509414
+00004e80: 2c32 342e 3533 3232 3631 2038 2e37 3631  ,24.532261 8.761
+00004e90: 3238 3737 2c32 352e 3732 3337 3235 2039  2877,25.723725 9
+00004ea0: 2e36 3230 3834 3337 2c32 362e 3639 3538  .6208437,26.6958
+00004eb0: 3836 2043 2031 302e 3530 3232 3838 2c32  86 C 10.502288,2
+00004ec0: 372e 3730 3630 3132 2031 312e 3539 3734  7.706012 11.5974
+00004ed0: 3034 2c32 382e 3535 3033 3838 2031 322e  04,28.550388 12.
+00004ee0: 3835 3430 3733 2c32 392e 3033 3938 3038  854073,29.039808
+00004ef0: 2043 2031 332e 3833 3830 372c 3239 2e34   C 13.83807,29.4
+00004f00: 3333 3138 3520 3134 2e39 3030 3333 372c  33185 14.900337,
+00004f10: 3239 2e36 3036 3630 3120 3135 2e39 3537  29.606601 15.957
+00004f20: 3932 2c32 392e 3630 3533 3035 207a 2720  92,29.605305 z' 
+00004f30: 7374 796c 653d 2766 696c 6c3a 2024 7a6f  style='fill: $zo
+00004f40: 6469 6163 5f63 6f6c 6f72 5f31 3b27 202f  diac_color_1;' /
+00004f50: 3e0d 0a20 2020 2020 2020 2020 2020 2020  >..             
+00004f60: 2020 203c 2f73 796d 626f 6c3e 0d0a 2020     </symbol>..  
+00004f70: 2020 2020 2020 2020 2020 2020 2020 3c73                <s
+00004f80: 796d 626f 6c20 6964 3d27 6765 6d69 6e69  ymbol id='gemini
+00004f90: 273e 0d0a 2020 2020 2020 2020 2020 2020  '>..            
+00004fa0: 2020 2020 2020 2020 3c70 6174 6820 7472          <path tr
+00004fb0: 616e 7366 6f72 6d3d 2273 6361 6c65 2830  ansform="scale(0
+00004fc0: 2e38 2922 2064 3d27 4d20 302e 3536 3534  .8)" d='M 0.5654
+00004fd0: 3932 3932 2c33 3220 4320 302e 3536 3534  9292,32 C 0.5654
+00004fe0: 3932 3932 2c33 312e 3231 3432 3338 2030  9292,31.214238 0
+00004ff0: 2e35 3635 3439 3239 322c 3330 2e34 3238  .56549292,30.428
+00005000: 3436 3520 302e 3536 3534 3932 3932 2c32  465 0.56549292,2
+00005010: 392e 3634 3237 3033 2043 2032 2e39 3637  9.642703 C 2.967
+00005020: 3531 3139 2c32 392e 3031 3131 3136 2035  5119,29.011116 5
+00005030: 2e34 3032 3335 3733 2c32 382e 3438 3631  .4023573,28.4861
+00005040: 3535 2037 2e38 3639 3737 3034 2c32 382e  55 7.8697704,28.
+00005050: 3138 3837 3932 2043 2037 2e38 3639 3737  188792 C 7.86977
+00005060: 3034 2c32 302e 3034 3838 3137 2037 2e38  04,20.048817 7.8
+00005070: 3639 3737 3034 2c31 312e 3930 3838 3332  697704,11.908832
+00005080: 2037 2e38 3639 3737 3034 2c33 2e37 3638   7.8697704,3.768
+00005090: 3835 3731 2043 2035 2e33 3937 3631 3436  8571 C 5.3976146
+000050a0: 2c33 2e35 3338 3935 3731 2032 2e39 3530  ,3.5389571 2.950
+000050b0: 3036 3239 2c33 2e30 3631 3633 3931 2030  0629,3.0616391 0
+000050c0: 2e35 3635 3439 3239 322c 322e 3337 3134  .56549292,2.3714
+000050d0: 3130 3820 4320 302e 3536 3534 3932 3932  108 C 0.56549292
+000050e0: 2c31 2e35 3830 3934 3233 2030 2e35 3635  ,1.5809423 0.565
+000050f0: 3439 3239 322c 302e 3739 3034 3733 3920  49292,0.7904739 
+00005100: 302e 3536 3534 3932 3932 2c2d 3565 2d30  0.56549292,-5e-0
+00005110: 3620 4320 342e 3133 3030 3435 392c 302e  6 C 4.1300459,0.
+00005120: 3938 3039 3330 3620 372e 3831 3834 3037  9809306 7.818407
+00005130: 382c 312e 3433 3632 3532 2031 312e 3530  8,1.436252 11.50
+00005140: 3238 3033 2c31 2e36 3432 3836 3935 2043  2803,1.6428695 C
+00005150: 2031 342e 3639 3934 312c 312e 3831 3135   14.69941,1.8115
+00005160: 3537 3420 3137 2e39 3035 3733 2c31 2e38  574 17.90573,1.8
+00005170: 3037 3034 3832 2032 312e 3130 3136 3131  070482 21.101611
+00005180: 2c31 2e36 3234 3037 3538 2043 2032 342e  ,1.6240758 C 24.
+00005190: 3637 3732 3334 2c31 2e34 3038 3139 3120  677234,1.408191 
+000051a0: 3238 2e32 3534 3734 322c 302e 3935 3235  28.254742,0.9525
+000051b0: 3638 3920 3331 2e37 3134 3432 362c 2d35  689 31.714426,-5
+000051c0: 652d 3036 2043 2033 312e 3731 3434 3236  e-06 C 31.714426
+000051d0: 2c30 2e37 3930 3437 3339 2033 312e 3731  ,0.7904739 31.71
+000051e0: 3434 3236 2c31 2e35 3830 3934 3233 2033  4426,1.5809423 3
+000051f0: 312e 3731 3434 3236 2c32 2e33 3731 3431  1.714426,2.37141
+00005200: 3038 2043 2032 392e 3332 3435 3032 2c33  08 C 29.324502,3
+00005210: 2e30 3539 3334 3831 2032 362e 3837 3238  .0593481 26.8728
+00005220: 3239 2c33 2e35 3338 3636 3731 2032 342e  29,3.5386671 24.
+00005230: 3339 3630 3435 2c33 2e37 3638 3835 3731  396045,3.7688571
+00005240: 2043 2032 342e 3339 3630 3435 2c31 312e   C 24.396045,11.
+00005250: 3930 3838 3332 2032 342e 3339 3630 3435  908832 24.396045
+00005260: 2c32 302e 3034 3838 3137 2032 342e 3339  ,20.048817 24.39
+00005270: 3630 3435 2c32 382e 3138 3837 3932 2043  6045,28.188792 C
+00005280: 2032 362e 3836 3830 3335 2c32 382e 3438   26.868035,28.48
+00005290: 3637 3034 2032 392e 3330 3731 3637 2c32  6704 29.307167,2
+000052a0: 392e 3031 3331 3538 2033 312e 3731 3434  9.013158 31.7144
+000052b0: 3236 2c32 392e 3634 3237 3033 2043 2033  26,29.642703 C 3
+000052c0: 312e 3731 3434 3236 2c33 302e 3432 3834  1.714426,30.4284
+000052d0: 3635 2033 312e 3731 3434 3236 2c33 312e  65 31.714426,31.
+000052e0: 3231 3432 3338 2033 312e 3731 3434 3236  214238 31.714426
+000052f0: 2c33 3220 4320 3236 2e30 3731 3737 2c33  ,32 C 26.07177,3
+00005300: 302e 3531 3238 3636 2032 302e 3230 3634  0.512866 20.2064
+00005310: 3332 2c32 392e 3939 3339 3238 2031 342e  32,29.993928 14.
+00005320: 3338 3332 3731 2c33 302e 3132 3932 3738  383271,30.129278
+00005330: 2043 2039 2e37 3238 3135 3336 2c33 302e   C 9.7281536,30.
+00005340: 3234 3031 3936 2035 2e30 3732 3133 3439  240196 5.0721349
+00005350: 2c33 302e 3830 3837 3737 2030 2e35 3635  ,30.808777 0.565
+00005360: 3439 3239 322c 3332 207a 204d 2031 302e  49292,32 z M 10.
+00005370: 3730 3430 3533 2c32 382e 3031 3934 3120  704053,28.01941 
+00005380: 4320 3132 2e39 3834 3434 382c 3237 2e37  C 12.984448,27.7
+00005390: 3635 3336 3720 3135 2e32 3833 3232 342c  65367 15.283224,
+000053a0: 3237 2e37 3232 3738 3320 3137 2e35 3735  27.722783 17.575
+000053b0: 3533 392c 3237 2e37 3636 3830 3820 4320  539,27.766808 C 
+000053c0: 3138 2e39 3036 3838 362c 3237 2e37 3936  18.906886,27.796
+000053d0: 3931 3220 3230 2e32 3338 3134 2c32 372e  912 20.23814,27.
+000053e0: 3837 3030 3635 2032 312e 3536 3137 3632  870065 21.561762
+000053f0: 2c32 382e 3031 3934 3120 4320 3231 2e35  ,28.01941 C 21.5
+00005400: 3631 3736 322c 3230 2e30 3031 3736 3620  61762,20.001766 
+00005410: 3231 2e35 3631 3736 322c 3131 2e39 3834  21.561762,11.984
+00005420: 3132 3120 3231 2e35 3631 3736 322c 332e  121 21.561762,3.
+00005430: 3936 3634 3737 3120 4320 3139 2e31 3839  9664771 C 19.189
+00005440: 3330 382c 342e 3132 3130 3737 3120 3136  308,4.1210771 16
+00005450: 2e38 3130 3038 312c 342e 3133 3933 3131  .810081,4.139311
+00005460: 3120 3134 2e34 3333 3531 352c 342e 3130  1 14.433515,4.10
+00005470: 3933 3633 3120 4320 3133 2e31 3839 3532  93631 C 13.18952
+00005480: 362c 342e 3039 3030 3832 3120 3131 2e39  6,4.0900821 11.9
+00005490: 3435 3530 352c 342e 3035 3032 3034 3120  45505,4.0502041 
+000054a0: 3130 2e37 3034 3035 332c 332e 3936 3634  10.704053,3.9664
+000054b0: 3737 3120 4320 3130 2e37 3034 3035 332c  771 C 10.704053,
+000054c0: 3131 2e39 3834 3132 3120 3130 2e37 3034  11.984121 10.704
+000054d0: 3035 332c 3230 2e30 3031 3736 3620 3130  053,20.001766 10
+000054e0: 2e37 3034 3035 332c 3238 2e30 3139 3431  .704053,28.01941
+000054f0: 207a 2027 2073 7479 6c65 3d27 6669 6c6c   z ' style='fill
+00005500: 3a20 247a 6f64 6961 635f 636f 6c6f 725f  : $zodiac_color_
+00005510: 323b 2720 2f3e 0d0a 2020 2020 2020 2020  2;' />..        
+00005520: 2020 2020 2020 2020 3c2f 7379 6d62 6f6c          </symbol
+00005530: 3e0d 0a20 2020 2020 2020 2020 2020 2020  >..             
+00005540: 2020 203c 7379 6d62 6f6c 2069 643d 2763     <symbol id='c
+00005550: 616e 6365 7227 3e0d 0a20 2020 2020 2020  ancer'>..       
+00005560: 2020 2020 2020 2020 2020 2020 203c 7061               <pa
+00005570: 7468 2074 7261 6e73 666f 726d 3d22 7363  th transform="sc
+00005580: 616c 6528 302e 3829 2220 643d 274d 2030  ale(0.8)" d='M 0
+00005590: 2c32 352e 3632 3934 3832 204c 2030 2c32  ,25.629482 L 0,2
+000055a0: 322e 3930 3831 3031 2043 2035 2e32 3437  2.908101 C 5.247
+000055b0: 3935 3039 2c32 352e 3330 3439 3134 2031  9509,25.304914 1
+000055c0: 302e 3333 3334 3634 2c32 362e 3439 3038  0.333464,26.4908
+000055d0: 3337 2031 352e 3233 3135 3531 2c32 362e  37 15.231551,26.
+000055e0: 3439 3038 3337 2043 2031 382e 3434 3237  490837 C 18.4427
+000055f0: 3937 2c32 362e 3439 3038 3337 2032 312e  97,26.490837 21.
+00005600: 3035 3432 3737 2c32 362e 3037 3838 3834  054277,26.078884
+00005610: 2032 332e 3036 3539 3932 2c32 352e 3234   23.065992,25.24
+00005620: 3234 3937 2043 2032 312e 3739 3134 3839  2497 C 21.791489
+00005630: 2c32 342e 3539 3333 3620 3230 2e38 3239  ,24.59336 20.829
+00005640: 3336 352c 3233 2e37 3639 3435 3520 3230  365,23.769455 20
+00005650: 2e31 3932 3131 342c 3232 2e37 3833 3236  .192114,22.78326
+00005660: 3720 4320 3139 2e35 3534 3836 332c 3231  7 C 19.554863,21
+00005670: 2e37 3937 3037 3820 3139 2e32 3239 3939  .797078 19.22999
+00005680: 2c32 302e 3633 3631 3232 2031 392e 3232  ,20.636122 19.22
+00005690: 3939 392c 3139 2e33 3030 3339 3820 4320  999,19.300398 C 
+000056a0: 3139 2e32 3239 3939 2c31 372e 3535 3237  19.22999,17.5527
+000056b0: 3232 2031 392e 3836 3732 3431 2c31 362e  22 19.867241,16.
+000056c0: 3035 3437 3134 2032 312e 3132 3932 3438  054714 21.129248
+000056d0: 2c31 342e 3739 3338 3931 2043 2032 322e  ,14.793891 C 22.
+000056e0: 3337 3837 362c 3133 2e35 3435 3535 3120  37876,13.545551 
+000056f0: 3233 2e39 3033 3136 352c 3132 2e39 3231  23.903165,12.921
+00005700: 3338 3120 3235 2e36 3532 3438 312c 3132  381 25.652481,12
+00005710: 2e39 3231 3338 3120 4320 3237 2e34 3031  .921381 C 27.401
+00005720: 3739 382c 3132 2e39 3231 3338 3120 3238  798,12.921381 28
+00005730: 2e38 3838 3731 382c 3133 2e35 3435 3535  .888718,13.54555
+00005740: 3120 3330 2e31 3338 3233 2c31 342e 3738  1 30.13823,14.78
+00005750: 3134 3037 2043 2033 312e 3337 3532 3436  1407 C 31.375246
+00005760: 2c31 362e 3032 3937 3437 2033 322e 3030  ,16.029747 32.00
+00005770: 3030 3032 2c31 372e 3531 3532 3732 2033  0002,17.515272 3
+00005780: 322e 3030 3030 3032 2c31 392e 3237 3534  2.000002,19.2754
+00005790: 3331 2043 2033 322e 3030 3030 3032 2c32  31 C 32.000002,2
+000057a0: 322e 3035 3932 3320 3330 2e33 3030 3636  2.05923 30.30066
+000057b0: 362c 3234 2e33 3831 3134 3220 3236 2e38  6,24.381142 26.8
+000057c0: 3839 3439 382c 3236 2e32 3238 3638 3520  89498,26.228685 
+000057d0: 4320 3233 2e34 3738 3333 312c 3238 2e30  C 23.478331,28.0
+000057e0: 3736 3232 3820 3139 2e32 3035 2c32 3920  76228 19.205,29 
+000057f0: 3134 2e30 3639 3530 352c 3239 2043 2039  14.069505,29 C 9
+00005800: 2e36 3231 3234 3239 2c32 3920 342e 3933  .6212429,29 4.93
+00005810: 3535 3732 392c 3237 2e38 3838 3937 3720  55729,27.888977 
+00005820: 302c 3235 2e36 3239 3438 3220 7a20 4d20  0,25.629482 z M 
+00005830: 3230 2e39 3136 3833 312c 3139 2e33 3132  20.916831,19.312
+00005840: 3838 3220 4320 3230 2e39 3136 3833 312c  882 C 20.916831,
+00005850: 3230 2e35 3836 3138 3820 3231 2e33 3739  20.586188 21.379
+00005860: 3135 2c32 312e 3638 3437 3238 2032 322e  15,21.684728 22.
+00005870: 3331 3632 3834 2c32 322e 3630 3834 3939  316284,22.608499
+00005880: 2043 2032 332e 3234 3039 3233 2c32 332e   C 23.240923,23.
+00005890: 3533 3232 3731 2032 342e 3336 3534 3834  532271 24.365484
+000058a0: 2c32 332e 3939 3431 3537 2032 352e 3635  ,23.994157 25.65
+000058b0: 3234 3831 2c32 332e 3939 3431 3537 2043  2481,23.994157 C
+000058c0: 2032 362e 3935 3139 3734 2c32 332e 3939   26.951974,23.99
+000058d0: 3431 3537 2032 382e 3035 3135 3435 2c32  4157 28.051545,2
+000058e0: 332e 3533 3232 3731 2032 382e 3936 3336  3.532271 28.9636
+000058f0: 3838 2c32 322e 3634 3539 3439 2043 2032  88,22.645949 C 2
+00005900: 392e 3836 3333 3337 2c32 312e 3734 3731  9.863337,21.7471
+00005910: 3435 2033 302e 3331 3331 3631 2c32 302e  45 30.313161,20.
+00005920: 3634 3836 3035 2033 302e 3331 3331 3631  648605 30.313161
+00005930: 2c31 392e 3335 3033 3332 2043 2033 302e  ,19.350332 C 30.
+00005940: 3331 3331 3631 2c31 382e 3032 3730 3931  313161,18.027091
+00005950: 2032 392e 3836 3333 3337 2c31 362e 3930   29.863337,16.90
+00005960: 3335 3835 2032 382e 3935 3131 3933 2c31  3585 28.951193,1
+00005970: 352e 3937 3938 3134 2043 2032 382e 3033  5.979814 C 28.03
+00005980: 3930 3439 2c31 352e 3035 3630 3432 2032  9049,15.056042 2
+00005990: 362e 3933 3934 3739 2c31 342e 3539 3431  6.939479,14.5941
+000059a0: 3536 2032 352e 3633 3939 3836 2c31 342e  56 25.639986,14.
+000059b0: 3539 3431 3536 2043 2032 342e 3332 3739  594156 C 24.3279
+000059c0: 3939 2c31 342e 3539 3431 3536 2032 332e  99,14.594156 23.
+000059d0: 3231 3539 3333 2c31 352e 3035 3630 3432  215933,15.056042
+000059e0: 2032 322e 3239 3132 3934 2c31 352e 3937   22.291294,15.97
+000059f0: 3938 3134 2043 2032 312e 3337 3931 352c  9814 C 21.37915,
+00005a00: 3136 2e38 3931 3130 3220 3230 2e39 3136  16.891102 20.916
+00005a10: 3833 312c 3138 2e30 3032 3132 3520 3230  831,18.002125 20
+00005a20: 2e39 3136 3833 312c 3139 2e33 3132 3838  .916831,19.31288
+00005a30: 3220 7a20 4d20 3332 2e30 3030 3030 322c  2 z M 32.000002,
+00005a40: 372e 3331 3633 3334 3120 4c20 3332 2e30  7.3163341 L 32.0
+00005a50: 3030 3030 322c 3130 2e30 3337 3731 3520  00002,10.037715 
+00005a60: 4320 3236 2e37 3339 3535 372c 372e 3634  C 26.739557,7.64
+00005a70: 3039 3032 3520 3231 2e36 3636 3533 382c  09025 21.666538,
+00005a80: 362e 3434 3234 3936 3220 3136 2e37 3535  6.4424962 16.755
+00005a90: 3935 362c 362e 3434 3234 3936 3220 4320  956,6.4424962 C 
+00005aa0: 3133 2e35 3537 3230 352c 362e 3434 3234  13.557205,6.4424
+00005ab0: 3936 3220 3130 2e39 3333 3233 2c36 2e38  962 10.93323,6.8
+00005ac0: 3534 3434 3833 2038 2e39 3039 3032 3039  544483 8.9090209
+00005ad0: 2c37 2e37 3033 3331 3935 2043 2031 302e  ,7.7033195 C 10.
+00005ae0: 3230 3835 3133 2c38 2e33 3532 3435 3633  208513,8.3524563
+00005af0: 2031 312e 3137 3036 3337 2c39 2e31 3736   11.170637,9.176
+00005b00: 3336 3037 2031 312e 3739 3533 3933 2c31  3607 11.795393,1
+00005b10: 302e 3136 3235 3439 2043 2031 322e 3434  0.162549 C 12.44
+00005b20: 3531 342c 3131 2e31 3438 3733 3820 3132  514,11.148738 12
+00005b30: 2e37 3537 3531 382c 3132 2e33 3039 3639  .757518,12.30969
+00005b40: 3420 3132 2e37 3537 3531 382c 3133 2e36  4 12.757518,13.6
+00005b50: 3435 3431 3820 4320 3132 2e37 3537 3531  45418 C 12.75751
+00005b60: 382c 3135 2e33 3933 3039 3420 3132 2e31  8,15.393094 12.1
+00005b70: 3332 3736 322c 3136 2e38 3931 3130 3220  32762,16.891102 
+00005b80: 3130 2e38 3730 3735 352c 3138 2e31 3531  10.870755,18.151
+00005b90: 3932 3520 4320 392e 3630 3837 3436 392c  925 C 9.6087469,
+00005ba0: 3139 2e34 3030 3236 3520 382e 3039 3638  19.400265 8.0968
+00005bb0: 3337 392c 3230 2e30 3234 3433 3520 362e  379,20.024435 6.
+00005bc0: 3333 3530 3235 392c 3230 2e30 3234 3433  3350259,20.02443
+00005bd0: 3520 4320 342e 3538 3537 3038 392c 3230  5 C 4.5857089,20
+00005be0: 2e30 3234 3433 3520 332e 3039 3837 3839  .024435 3.098789
+00005bf0: 392c 3139 2e34 3132 3734 3920 312e 3836  9,19.412749 1.86
+00005c00: 3137 3732 392c 3138 2e31 3634 3430 3920  17729,18.164409 
+00005c10: 4320 302e 3632 3437 3536 2c31 362e 3932  C 0.624756,16.92
+00005c20: 3835 3532 2030 2c31 352e 3433 3035 3434  8552 0,15.430544
+00005c30: 2030 2c31 332e 3638 3238 3638 2043 2030   0,13.682868 C 0
+00005c40: 2c31 302e 3838 3635 3836 2031 2e36 3939  ,10.886586 1.699
+00005c50: 3333 3634 2c38 2e35 3532 3139 3037 2035  3364,8.5521907 5
+00005c60: 2e31 3130 3530 3339 2c36 2e37 3034 3634  .1105039,6.70464
+00005c70: 3735 2043 2038 2e35 3039 3137 3639 2c34  75 C 8.5091769,4
+00005c80: 2e38 3537 3130 3434 2031 322e 3739 3530  .8571044 12.7950
+00005c90: 3033 2c33 2e39 3333 3333 3237 2031 372e  03,3.9333327 17.
+00005ca0: 3933 3034 3937 2c33 2e39 3333 3333 3237  930497,3.9333327
+00005cb0: 2043 2032 322e 3337 3837 362c 332e 3933   C 22.37876,3.93
+00005cc0: 3333 3332 3720 3237 2e30 3634 3433 2c35  33327 27.06443,5
+00005cd0: 2e30 3536 3833 3838 2033 322e 3030 3030  .0568388 32.0000
+00005ce0: 3032 2c37 2e33 3136 3333 3431 207a 204d  02,7.3163341 z M
+00005cf0: 2031 312e 3038 3331 3732 2c31 332e 3633   11.083172,13.63
+00005d00: 3239 3335 2043 2031 312e 3038 3331 3732  2935 C 11.083172
+00005d10: 2c31 322e 3334 3731 3434 2031 302e 3632  ,12.347144 10.62
+00005d20: 3038 3532 2c31 312e 3234 3836 3035 2039  0852,11.248605 9
+00005d30: 2e36 3833 3731 3739 2c31 302e 3332 3438  .6837179,10.3248
+00005d40: 3334 2043 2038 2e37 3436 3538 3339 2c39  34 C 8.7465839,9
+00005d50: 2e34 3133 3534 3533 2037 2e36 3232 3032  .4135453 7.62202
+00005d60: 3239 2c38 2e39 3531 3635 3935 2036 2e33  29,8.9516595 6.3
+00005d70: 3232 3533 3039 2c38 2e39 3531 3635 3935  225309,8.9516595
+00005d80: 2043 2035 2e30 3233 3033 3739 2c38 2e39   C 5.0230379,8.9
+00005d90: 3531 3635 3935 2033 2e39 3233 3436 3739  516595 3.9234679
+00005da0: 2c39 2e34 3031 3036 3139 2033 2e30 3233  ,9.4010619 3.023
+00005db0: 3831 3839 2c31 302e 3239 3938 3637 2043  8189,10.299867 C
+00005dc0: 2032 2e31 3234 3137 3039 2c31 312e 3139   2.1241709,11.19
+00005dd0: 3836 3732 2031 2e36 3734 3334 3631 2c31  8672 1.6743461,1
+00005de0: 322e 3239 3732 3131 2031 2e36 3734 3334  2.297211 1.67434
+00005df0: 3631 2c31 332e 3539 3534 3834 2043 2031  61,13.595484 C 1
+00005e00: 2e36 3734 3334 3631 2c31 342e 3931 3837  .6743461,14.9187
+00005e10: 3235 2032 2e31 3336 3636 3539 2c31 362e  25 2.1366659,16.
+00005e20: 3034 3232 3331 2033 2e30 3438 3830 3839  042231 3.0488089
+00005e30: 2c31 362e 3936 3630 3032 2043 2033 2e39  ,16.966002 C 3.9
+00005e40: 3438 3435 3739 2c31 372e 3838 3937 3734  484579,17.889774
+00005e50: 2035 2e30 3630 3532 3339 2c31 382e 3335   5.0605239,18.35
+00005e60: 3136 3620 362e 3336 3030 3135 392c 3138  166 6.3600159,18
+00005e70: 2e33 3531 3636 2043 2037 2e36 3539 3530  .35166 C 7.65950
+00005e80: 3839 2c31 382e 3335 3136 3620 382e 3738  89,18.35166 8.78
+00005e90: 3430 3638 392c 3137 2e38 3839 3737 3420  40689,17.889774 
+00005ea0: 392e 3639 3632 3132 392c 3136 2e39 3636  9.6962129,16.966
+00005eb0: 3030 3220 4320 3130 2e36 3230 3835 322c  002 C 10.620852,
+00005ec0: 3136 2e30 3432 3233 3120 3131 2e30 3833  16.042231 11.083
+00005ed0: 3137 322c 3134 2e39 3331 3230 3820 3131  172,14.931208 11
+00005ee0: 2e30 3833 3137 322c 3133 2e36 3332 3933  .083172,13.63293
+00005ef0: 3520 7a20 2720 7374 796c 653d 2766 696c  5 z ' style='fil
+00005f00: 6c3a 2024 7a6f 6469 6163 5f63 6f6c 6f72  l: $zodiac_color
+00005f10: 5f33 3b27 202f 3e0d 0a20 2020 2020 2020  _3;' />..       
+00005f20: 2020 2020 2020 2020 203c 2f73 796d 626f           </symbo
+00005f30: 6c3e 0d0a 2020 2020 2020 2020 2020 2020  l>..            
+00005f40: 2020 2020 3c73 796d 626f 6c20 6964 3d27      <symbol id='
+00005f50: 6c65 6f27 3e0d 0a20 2020 2020 2020 2020  leo'>..         
+00005f60: 2020 2020 2020 2020 2020 203c 7061 7468             <path
+00005f70: 2074 7261 6e73 666f 726d 3d22 7363 616c   transform="scal
+00005f80: 6528 302e 3829 2220 643d 274d 2032 382e  e(0.8)" d='M 28.
+00005f90: 3032 3133 3731 2c32 392e 3438 3038 3231  021371,29.480821
+00005fa0: 2043 2032 372e 3337 3833 3339 2c33 302e   C 27.378339,30.
+00005fb0: 3036 3939 3438 2032 362e 3638 3739 3932  069948 26.687992
+00005fc0: 2c33 302e 3631 3233 3932 2032 352e 3933  ,30.612392 25.93
+00005fd0: 3336 3032 2c33 312e 3035 3233 3539 2043  3602,31.052359 C
+00005fe0: 2032 352e 3330 3433 3934 2c33 312e 3431   25.304394,31.41
+00005ff0: 3837 3031 2032 342e 3632 3734 3239 2c33  8701 24.627429,3
+00006000: 312e 3731 3230 3931 2032 332e 3931 3530  1.712091 23.9150
+00006010: 3232 2c33 312e 3837 3034 3732 2043 2032  22,31.870472 C 2
+00006020: 332e 3438 3738 3037 2c33 312e 3936 3620  3.487807,31.966 
+00006030: 3233 2e30 3438 3937 372c 3332 2e30 3130  23.048977,32.010
+00006040: 3236 3220 3232 2e36 3131 3237 392c 3331  262 22.611279,31
+00006050: 2e39 3937 3939 3820 4320 3231 2e39 3936  .997998 C 21.996
+00006060: 3038 352c 3331 2e39 3834 3135 3720 3231  085,31.984157 21
+00006070: 2e33 3830 3334 352c 3331 2e38 3737 3435  .380345,31.87745
+00006080: 3420 3230 2e38 3034 3931 312c 3331 2e36  4 20.804911,31.6
+00006090: 3536 3432 3620 4320 3230 2e32 3733 3435  56426 C 20.27345
+000060a0: 392c 3331 2e34 3533 3739 2031 392e 3738  9,31.45379 19.78
+000060b0: 3034 322c 3331 2e31 3533 3930 3320 3139  042,31.153903 19
+000060c0: 2e33 3530 3435 352c 3330 2e37 3832 3032  .350455,30.78202
+000060d0: 3820 4320 3139 2e30 3135 3934 2c33 302e  8 C 19.01594,30.
+000060e0: 3439 3337 3639 2031 382e 3731 3830 3032  493769 18.718002
+000060f0: 2c33 302e 3136 3237 3537 2031 382e 3436  ,30.162757 18.46
+00006100: 3737 3632 2c32 392e 3739 3838 3436 2043  7762,29.798846 C
+00006110: 2031 382e 3135 3837 3831 2c32 392e 3334   18.158781,29.34
+00006120: 3936 3333 2031 372e 3932 3937 3832 2c32  9633 17.929782,2
+00006130: 382e 3834 3537 3339 2031 372e 3739 3437  8.845739 17.7947
+00006140: 3235 2c32 382e 3331 3734 3739 2043 2031  25,28.317479 C 1
+00006150: 372e 3633 3539 342c 3237 2e37 3030 3837  7.63594,27.70087
+00006160: 3120 3137 2e36 3031 3335 352c 3237 2e30  1 17.601355,27.0
+00006170: 3536 3233 3720 3137 2e36 3538 3839 362c  56237 17.658896,
+00006180: 3236 2e34 3233 3430 3220 4320 3137 2e37  26.423402 C 17.7
+00006190: 3136 3438 352c 3235 2e37 3833 3837 3220  16485,25.783872 
+000061a0: 3137 2e38 3438 3031 332c 3235 2e31 3533  17.848013,25.153
+000061b0: 3330 3620 3138 2e30 3038 3434 392c 3234  306 18.008449,24
+000061c0: 2e35 3332 3335 3420 4320 3138 2e32 3536  .532354 C 18.256
+000061d0: 3930 352c 3233 2e35 3830 3631 3120 3138  905,23.580611 18
+000061e0: 2e35 3737 3837 332c 3232 2e36 3439 3335  .577873,22.64935
+000061f0: 2031 382e 3932 3834 3931 2c32 312e 3733   18.928491,21.73
+00006200: 3038 3733 2043 2031 392e 3434 3439 3538  0873 C 19.444958
+00006210: 2c32 302e 3338 3337 3136 2032 302e 3033  ,20.383716 20.03
+00006220: 3031 3734 2c31 392e 3036 3339 3838 2032  0174,19.063988 2
+00006230: 302e 3634 3439 3731 2c31 372e 3735 3931  0.644971,17.7591
+00006240: 3434 2043 2032 312e 3133 3732 3035 2c31  44 C 21.137205,1
+00006250: 362e 3731 3031 3031 2032 312e 3632 3934  6.710101 21.6294
+00006260: 3337 2c31 352e 3636 3130 3620 3232 2e31  37,15.66106 22.1
+00006270: 3231 3636 392c 3134 2e36 3132 3031 3720  21669,14.612017 
+00006280: 4320 3232 2e35 3633 3232 372c 3133 2e36  C 22.563227,13.6
+00006290: 3635 3230 3820 3232 2e39 3635 3734 332c  65208 22.965743,
+000062a0: 3132 2e36 3938 3435 2032 332e 3238 3630  12.69845 23.2860
+000062b0: 3532 2c31 312e 3730 3334 3332 2043 2032  52,11.703432 C 2
+000062c0: 332e 3531 3430 3939 2c31 302e 3939 3037  3.514099,10.9907
+000062d0: 3120 3233 2e37 3031 3235 352c 3130 2e32  1 23.701255,10.2
+000062e0: 3632 3530 3420 3233 2e38 3031 3138 312c  62504 23.801181,
+000062f0: 392e 3532 3030 3238 3620 4320 3233 2e38  9.5200286 C 23.8
+00006300: 3532 3139 362c 392e 3134 3035 3734 3620  52196,9.1405746 
+00006310: 3233 2e38 3737 3538 372c 382e 3735 3733  23.877587,8.7573
+00006320: 3931 3620 3233 2e38 3639 3331 312c 382e  916 23.869311,8.
+00006330: 3337 3434 3736 3620 4320 3233 2e38 3536  3744766 C 23.856
+00006340: 3839 392c 372e 3538 3639 3331 3420 3233  899,7.5869314 23
+00006350: 2e37 3530 3534 392c 362e 3739 3635 3631  .750549,6.796561
+00006360: 3820 3233 2e35 3035 3330 312c 362e 3034  8 23.505301,6.04
+00006370: 3633 3633 3520 4320 3233 2e33 3031 3035  63635 C 23.30105
+00006380: 382c 352e 3431 3836 3035 2032 322e 3939  8,5.418605 22.99
+00006390: 3635 3539 2c34 2e38 3232 3436 3734 2032  6559,4.8224674 2
+000063a0: 322e 3539 3734 3031 2c34 2e32 3936 3134  2.597401,4.29614
+000063b0: 3231 2043 2032 322e 3337 3131 3037 2c33  21 C 22.371107,3
+000063c0: 2e39 3937 3138 3831 2032 322e 3131 3538  .9971881 22.1158
+000063d0: 382c 332e 3732 3033 3533 3220 3231 2e38  8,3.7203532 21.8
+000063e0: 3339 3133 322c 332e 3436 3735 3333 3320  39132,3.4675333 
+000063f0: 4320 3231 2e33 3739 3338 2c33 2e30 3438  C 21.37938,3.048
+00006400: 3735 3332 2032 302e 3834 3836 312c 322e  7532 20.84861,2.
+00006410: 3730 3832 3432 3420 3230 2e32 3735 3832  7082424 20.27582
+00006420: 362c 322e 3436 3630 3137 3420 4320 3139  6,2.4660174 C 19
+00006430: 2e36 3233 3230 312c 322e 3138 3834 3239  .623201,2.188429
+00006440: 2031 382e 3932 3133 3531 2c32 2e30 3337   18.921351,2.037
+00006450: 3339 3720 3138 2e32 3135 3538 2c31 2e39  397 18.21558,1.9
+00006460: 3833 3439 3733 2043 2031 372e 3730 3839  834973 C 17.7089
+00006470: 3532 2c31 2e39 3435 3538 3832 2031 372e  52,1.9455882 17.
+00006480: 3139 3836 3931 2c31 2e39 3530 3435 3832  198691,1.9504582
+00006490: 2031 362e 3639 3333 3834 2c32 2e30 3034   16.693384,2.004
+000064a0: 3330 3534 2043 2031 362e 3031 3834 3435  3054 C 16.018445
+000064b0: 2c32 2e30 3736 3536 3038 2031 352e 3335  ,2.0765608 15.35
+000064c0: 3038 3238 2c32 2e32 3434 3737 3636 2031  0828,2.2447766 1
+000064d0: 342e 3733 3431 3731 2c32 2e35 3331 3330  4.734171,2.53130
+000064e0: 3833 2043 2031 342e 3137 3731 3035 2c32  83 C 14.177105,2
+000064f0: 2e37 3838 3835 3720 3133 2e36 3635 3034  .788857 13.66504
+00006500: 332c 332e 3134 3233 3937 3520 3133 2e32  3,3.1423975 13.2
+00006510: 3234 3331 382c 332e 3536 3933 3437 3920  24318,3.5693479 
+00006520: 4320 3132 2e37 3935 3533 352c 332e 3939  C 12.795535,3.99
+00006530: 3531 3333 3320 3132 2e34 3335 3435 372c  51333 12.435457,
+00006540: 342e 3439 3132 3431 3820 3132 2e31 3732  4.4912418 12.172
+00006550: 3731 392c 352e 3033 3538 3737 3320 4320  719,5.0358773 C 
+00006560: 3131 2e38 3930 3039 342c 352e 3631 3831  11.890094,5.6181
+00006570: 3436 3720 3131 2e37 3139 3634 322c 362e  467 11.719642,6.
+00006580: 3235 3133 3038 3120 3131 2e36 3433 3934  2513081 11.64394
+00006590: 372c 362e 3839 3331 3032 3920 4320 3131  7,6.8931029 C 11
+000065a0: 2e35 3632 3031 372c 372e 3538 3434 3332  .562017,7.584432
+000065b0: 3320 3131 2e35 3832 3832 2c38 2e32 3835  3 11.58282,8.285
+000065c0: 3733 3936 2031 312e 3638 3035 3333 2c38  7396 11.680533,8
+000065d0: 2e39 3734 3330 3336 2043 2031 312e 3830  .9743036 C 11.80
+000065e0: 3630 3831 2c39 2e38 3631 3736 3036 2031  6081,9.8617606 1
+000065f0: 322e 3034 3839 3735 2c31 302e 3732 3931  2.048975,10.7291
+00006600: 3532 2031 322e 3335 3430 3333 2c31 312e  52 12.354033,11.
+00006610: 3537 3036 3931 2043 2031 322e 3539 3837  570691 C 12.5987
+00006620: 3938 2c31 322e 3234 3438 3337 2031 322e  98,12.244837 12.
+00006630: 3838 3534 3939 2c31 322e 3930 3331 3137  885499,12.903117
+00006640: 2031 332e 3139 3833 3938 2c31 332e 3534   13.198398,13.54
+00006650: 3832 3638 2043 2031 332e 3430 3939 3634  8268 C 13.409964
+00006660: 2c31 332e 3938 3736 3832 2031 332e 3632  ,13.987682 13.62
+00006670: 3139 3131 2c31 342e 3432 3639 3135 2031  1911,14.426915 1
+00006680: 332e 3833 3331 3731 2c31 342e 3836 3634  3.833171,14.8664
+00006690: 3735 2043 2031 342e 3138 3034 3838 2c31  75 C 14.180488,1
+000066a0: 352e 3539 3620 3134 2e35 3037 3836 332c  5.596 14.507863,
+000066b0: 3136 2e33 3336 3131 3620 3134 2e37 3831  16.336116 14.781
+000066c0: 3734 2c31 372e 3039 3636 3634 2043 2031  74,17.096664 C 1
+000066d0: 342e 3935 3436 3339 2c31 372e 3538 3039  4.954639,17.5809
+000066e0: 3033 2031 352e 3130 3737 3431 2c31 382e  03 15.107741,18.
+000066f0: 3037 3338 3938 2031 352e 3230 3436 3634  073898 15.204664
+00006700: 2c31 382e 3537 3934 3638 2043 2031 352e  ,18.579468 C 15.
+00006710: 3236 3036 3135 2c31 382e 3837 3434 3034  260615,18.874404
+00006720: 2031 352e 3239 3539 3035 2c31 392e 3137   15.295905,19.17
+00006730: 3434 3932 2031 352e 3238 3835 3031 2c31  4492 15.288501,1
+00006740: 392e 3437 3530 3936 2043 2031 352e 3237  9.475096 C 15.27
+00006750: 3935 3331 2c32 302e 3132 3030 3634 2031  9531,20.120064 1
+00006760: 352e 3136 3430 3538 2c32 302e 3736 3435  5.164058,20.7645
+00006770: 3735 2031 342e 3933 3633 322c 3231 2e33  75 14.93632,21.3
+00006780: 3638 3536 3320 4320 3134 2e37 3032 3536  68563 C 14.70256
+00006790: 322c 3231 2e39 3932 3933 3820 3134 2e33  2,21.992938 14.3
+000067a0: 3531 3339 362c 3232 2e35 3730 3337 3720  51396,22.570377 
+000067b0: 3133 2e39 3232 3631 342c 3233 2e30 3739  13.922614,23.079
+000067c0: 3732 3920 4320 3133 2e35 3936 3136 382c  729 C 13.596168,
+000067d0: 3233 2e34 3636 3736 3820 3133 2e32 3239  23.466768 13.229
+000067e0: 3434 352c 3233 2e38 3230 3330 3520 3132  445,23.820305 12
+000067f0: 2e38 3238 3031 2c32 342e 3132 3930 3036  .82801,24.129006
+00006800: 2043 2031 322e 3330 3034 3934 2c32 342e   C 12.300494,24.
+00006810: 3533 3436 3533 2031 312e 3730 3730 3231  534653 11.707021
+00006820: 2c32 342e 3835 3632 3737 2031 312e 3037  ,24.856277 11.07
+00006830: 3433 352c 3235 2e30 3634 3034 3120 4320  435,25.064041 C 
+00006840: 3130 2e34 3238 3035 332c 3235 2e32 3737  10.428053,25.277
+00006850: 3930 3920 392e 3734 3439 3337 352c 3235  909 9.7449375,25
+00006860: 2e33 3732 3139 3320 392e 3036 3530 3339  .372193 9.065039
+00006870: 392c 3235 2e33 3633 3736 3720 4320 382e  9,25.363767 C 8.
+00006880: 3337 3539 3539 332c 3235 2e33 3536 3836  3759593,25.35686
+00006890: 3920 372e 3638 3535 3031 382c 3235 2e32  9 7.6855018,25.2
+000068a0: 3437 3539 3120 372e 3033 3535 3831 392c  47591 7.0355819,
+000068b0: 3235 2e30 3135 3535 3720 4320 362e 3432  25.015557 C 6.42
+000068c0: 3232 3433 372c 3234 2e37 3938 3133 3820  22437,24.798138 
+000068d0: 352e 3834 3839 3638 372c 3234 2e34 3731  5.8489687,24.471
+000068e0: 3730 3620 352e 3334 3239 3131 382c 3234  706 5.3429118,24
+000068f0: 2e30 3633 3133 3320 4320 352e 3034 3339  .063133 C 5.0439
+00006900: 3639 352c 3233 2e38 3232 3332 3820 342e  695,23.822328 4.
+00006910: 3736 3737 3439 312c 3233 2e35 3533 3839  7677491,23.55389
+00006920: 3820 342e 3531 3233 3537 332c 3233 2e32  8 4.5123573,23.2
+00006930: 3637 3520 4320 342e 3037 3535 3533 312c  675 C 4.0755531,
+00006940: 3232 2e37 3735 3634 3820 332e 3731 3431  22.775648 3.7141
+00006950: 3734 322c 3232 2e32 3134 3934 3420 332e  742,22.214944 3.
+00006960: 3436 3136 3531 382c 3231 2e36 3036 3834  4616518,21.60684
+00006970: 3420 4320 332e 3230 3337 3737 372c 3230  4 C 3.2037777,20
+00006980: 2e39 3839 3935 2033 2e30 3539 3433 3738  .98995 3.0594378
+00006990: 2c32 302e 3332 3832 3539 2033 2e30 3135  ,20.328259 3.015
+000069a0: 3739 3238 2c31 392e 3636 3138 3036 2043  7928,19.661806 C
+000069b0: 2032 2e39 3639 3330 3138 2c31 382e 3935   2.9693018,18.95
+000069c0: 3534 3333 2033 2e30 3233 3138 3338 2c31  5433 3.0231838,1
+000069d0: 382e 3233 3933 3937 2033 2e32 3037 3731  8.239397 3.20771
+000069e0: 3034 2c31 372e 3535 3437 3420 4320 332e  04,17.55474 C 3.
+000069f0: 3337 3237 3232 352c 3136 2e39 3337 3233  3727225,16.93723
+00006a00: 3320 332e 3634 3437 3337 332c 3136 2e33  3 3.6447373,16.3
+00006a10: 3439 3139 3420 342e 3030 3431 3339 392c  49194 4.0041399,
+00006a20: 3135 2e38 3230 3930 3120 4320 342e 3330  15.820901 C 4.30
+00006a30: 3237 3433 2c31 352e 3337 3939 3036 2034  2743,15.379906 4
+00006a40: 2e36 3630 3732 3038 2c31 342e 3938 3130  .6607208,14.9810
+00006a50: 3834 2035 2e30 3532 3631 3236 2c31 342e  84 5.0526126,14.
+00006a60: 3632 3132 3733 2043 2035 2e35 3432 3133  621273 C 5.54213
+00006a70: 3939 2c31 342e 3137 3334 3637 2036 2e31  99,14.173467 6.1
+00006a80: 3031 3336 3239 2c31 332e 3739 3837 3334  013629,13.798734
+00006a90: 2036 2e37 3132 3139 3433 2c31 332e 3533   6.7121943,13.53
+00006aa0: 3736 3733 2043 2037 2e33 3032 3038 3837  7673 C 7.3020887
+00006ab0: 2c31 332e 3238 3339 3120 372e 3933 3638  ,13.28391 7.9368
+00006ac0: 3232 312c 3133 2e31 3338 3736 3120 382e  221,13.138761 8.
+00006ad0: 3537 3731 3632 352c 3133 2e30 3937 3734  5771625,13.09774
+00006ae0: 3920 4320 382e 3839 3731 3538 342c 3133  9 C 8.8971584,13
+00006af0: 2e30 3736 3731 3720 392e 3231 3839 3833  .076717 9.218983
+00006b00: 372c 3133 2e30 3739 3437 3320 392e 3533  7,13.079473 9.53
+00006b10: 3830 3932 332c 3133 2e31 3132 3337 3620  80923,13.112376 
+00006b20: 4320 3130 2e30 3138 3332 352c 3133 2e31  C 10.018325,13.1
+00006b30: 3630 3836 3420 3130 2e34 3931 3431 352c  60864 10.491415,
+00006b40: 3133 2e32 3637 3532 2031 302e 3935 3138  13.26752 10.9518
+00006b50: 3737 2c31 332e 3431 3038 3531 2043 2031  77,13.410851 C 1
+00006b60: 302e 3437 3636 3738 2c31 322e 3439 3332  0.476678,12.4932
+00006b70: 3632 2031 302e 3035 3639 3531 2c31 312e  62 10.056951,11.
+00006b80: 3534 3430 3535 2039 2e37 3435 3831 3636  544055 9.7458166
+00006b90: 2c31 302e 3535 3736 3538 2043 2039 2e34  ,10.557658 C 9.4
+00006ba0: 3931 3634 322c 392e 3734 3838 3238 3620  91642,9.7488286 
+00006bb0: 392e 3331 3039 3631 392c 382e 3931 3238  9.3109619,8.9128
+00006bc0: 3534 3620 392e 3236 3232 3431 362c 382e  546 9.2622416,8.
+00006bd0: 3036 3439 3732 3620 4320 392e 3233 3633  0649726 C 9.2363
+00006be0: 3035 2c37 2e36 3033 3133 3038 2039 2e32  05,7.6031308 9.2
+00006bf0: 3530 3631 372c 372e 3133 3931 3239 3720  50617,7.1391297 
+00006c00: 392e 3330 3132 3635 392c 362e 3637 3934  9.3012659,6.6794
+00006c10: 3130 3720 4320 392e 3338 3632 3530 372c  107 C 9.3862507,
+00006c20: 352e 3931 3332 3638 3520 392e 3538 3638  5.9132685 9.5868
+00006c30: 3830 322c 352e 3135 3832 3033 3820 392e  802,5.1582038 9.
+00006c40: 3931 3237 3533 372c 342e 3435 3838 3438  9127537,4.458848
+00006c50: 3720 4320 3130 2e32 3333 3534 372c 332e  7 C 10.233547,3.
+00006c60: 3736 3634 3839 3620 3130 2e36 3735 3137  7664896 10.67517
+00006c70: 312c 332e 3133 3235 3220 3131 2e31 3939  1,3.13252 11.199
+00006c80: 3734 382c 322e 3537 3933 3138 3820 4320  748,2.5793188 C 
+00006c90: 3131 2e38 3531 3530 312c 312e 3839 3237  11.851501,1.8927
+00006ca0: 3037 3820 3132 2e36 3139 3630 342c 312e  078 12.619604,1.
+00006cb0: 3331 3434 3734 3620 3133 2e34 3637 3937  3144746 13.46797
+00006cc0: 352c 302e 3839 3330 3336 3732 2043 2031  5,0.89303672 C 1
+00006cd0: 342e 3233 3735 3436 2c30 2e35 3039 3130  4.237546,0.50910
+00006ce0: 3738 3220 3135 2e30 3639 3536 372c 302e  782 15.069567,0.
+00006cf0: 3235 3631 3731 3432 2031 352e 3931 3833  25617142 15.9183
+00006d00: 3931 2c30 2e31 3233 3038 3639 3220 4320  91,0.12308692 C 
+00006d10: 3136 2e37 3434 3435 392c 2d30 2e30 3037  16.744459,-0.007
+00006d20: 3233 3732 3833 3820 3137 2e35 3835 3435  2372838 17.58545
+00006d30: 322c 2d30 2e30 3236 3938 3737 3834 2031  2,-0.026987784 1
+00006d40: 382e 3431 3839 3737 2c30 2e30 3239 3338  8.418977,0.02938
+00006d50: 3636 3136 2043 2031 392e 3336 3932 3935  6616 C 19.369295
+00006d60: 2c30 2e30 3935 3336 3739 3136 2032 302e  ,0.095367916 20.
+00006d70: 3331 3534 3834 2c30 2e32 3739 3538 3731  315484,0.2795871
+00006d80: 3220 3231 2e32 3036 3335 382c 302e 3632  2 21.206358,0.62
+00006d90: 3133 3736 3132 2043 2032 312e 3937 3132  137612 C 21.9712
+00006da0: 3739 2c30 2e39 3133 3537 3930 3220 3232  79,0.91357902 22
+00006db0: 2e36 3931 3634 332c 312e 3332 3338 3037  .691643,1.323807
+00006dc0: 3520 3233 2e33 3238 3433 312c 312e 3833  5 23.328431,1.83
+00006dd0: 3930 3835 3620 4320 3233 2e36 3231 3036  90856 C 23.62106
+00006de0: 322c 322e 3037 3533 3636 3720 3233 2e38  2,2.0753667 23.8
+00006df0: 3937 3239 312c 322e 3333 3232 3136 3820  97291,2.3322168 
+00006e00: 3234 2e31 3530 3531 332c 322e 3631 3034  24.150513,2.6104
+00006e10: 3531 3220 4320 3234 2e36 3835 3335 362c  512 C 24.685356,
+00006e20: 332e 3139 3333 3635 3420 3235 2e31 3237  3.1933654 25.127
+00006e30: 3438 372c 332e 3836 3132 3637 3420 3235  487,3.8612674 25
+00006e40: 2e34 3533 3139 362c 342e 3538 3233 3435  .453196,4.582345
+00006e50: 2043 2032 352e 3831 3738 3431 2c35 2e33   C 25.817841,5.3
+00006e60: 3835 3738 3035 2032 362e 3033 3833 3437  857805 26.038347
+00006e70: 2c36 2e32 3530 3332 3632 2032 362e 3134  ,6.2503262 26.14
+00006e80: 3037 3139 2c37 2e31 3235 3432 3832 2043  0719,7.1254282 C
+00006e90: 2032 362e 3230 3134 3538 2c37 2e36 3337   26.201458,7.637
+00006ea0: 3231 3731 2032 362e 3232 3038 3439 2c38  2171 26.220849,8
+00006eb0: 2e31 3533 3232 3736 2032 362e 3231 3234  .1532276 26.2124
+00006ec0: 352c 382e 3636 3833 3431 3620 4320 3236  5,8.6683416 C 26
+00006ed0: 2e32 3031 3732 352c 392e 3430 3639 3639  .201725,9.406969
+00006ee0: 3620 3236 2e31 3437 3032 332c 3130 2e31  6 26.147023,10.1
+00006ef0: 3436 3836 3120 3236 2e30 3131 3035 312c  46861 26.011051,
+00006f00: 3130 2e38 3733 3635 3120 4320 3235 2e39  10.873651 C 25.9
+00006f10: 3537 3838 392c 3131 2e31 3538 3134 3220  57889,11.158142 
+00006f20: 3235 2e38 3930 3534 322c 3131 2e34 3339  25.890542,11.439
+00006f30: 3937 3220 3235 2e38 3038 3535 362c 3131  972 25.808556,11
+00006f40: 2e37 3137 3533 3820 4320 3235 2e36 3838  .717538 C 25.688
+00006f50: 3138 362c 3132 2e31 3337 3931 3720 3235  186,12.137917 25
+00006f60: 2e35 3336 3936 382c 3132 2e35 3438 3639  .536968,12.54869
+00006f70: 3820 3235 2e33 3739 3231 322c 3132 2e39  8 25.379212,12.9
+00006f80: 3536 3236 3120 4320 3235 2e30 3737 3936  56261 C 25.07796
+00006f90: 332c 3133 2e37 3237 3834 3720 3234 2e37  3,13.727847 24.7
+00006fa0: 3435 3736 352c 3134 2e34 3836 3930 3820  45765,14.486908 
+00006fb0: 3234 2e34 3035 3930 382c 3135 2e32 3432  24.405908,15.242
+00006fc0: 3133 3120 4320 3234 2e32 3438 3631 2c31  131 C 24.24861,1
+00006fd0: 352e 3539 3138 3733 2032 342e 3038 3736  5.591873 24.0876
+00006fe0: 3038 2c31 352e 3933 3939 3236 2032 332e  08,15.939926 23.
+00006ff0: 3932 3639 3539 2c31 362e 3238 3831 3334  926959,16.288134
+00007000: 2043 2032 332e 3537 3339 3332 2c31 372e   C 23.573932,17.
+00007010: 3035 3838 3734 2032 332e 3232 3039 3034  058874 23.220904
+00007020: 2c31 372e 3832 3936 3135 2032 322e 3836  ,17.829615 22.86
+00007030: 3738 3736 2c31 382e 3630 3033 3535 2043  7876,18.600355 C
+00007040: 2032 322e 3237 3838 3132 2c31 392e 3838   22.278812,19.88
+00007050: 3030 3539 2032 312e 3730 3632 3435 2c32  0059 21.706245,2
+00007060: 312e 3136 3739 2032 312e 3138 3230 372c  1.1679 21.18207,
+00007070: 3232 2e34 3735 3733 3120 4320 3230 2e38  22.475731 C 20.8
+00007080: 3735 3639 332c 3233 2e32 3434 3235 3220  75693,23.244252 
+00007090: 3230 2e35 3833 3739 362c 3234 2e30 3139  20.583796,24.019
+000070a0: 3339 3620 3230 2e33 3339 3634 392c 3234  396 20.339649,24
+000070b0: 2e38 3130 3230 3720 4320 3230 2e32 3035  .810207 C 20.205
+000070c0: 3336 312c 3235 2e32 3530 3632 3720 3230  361,25.250627 20
+000070d0: 2e30 3833 3338 392c 3235 2e36 3936 3133  .083389,25.69613
+000070e0: 3620 3230 2e30 3037 3836 352c 3236 2e31  6 20.007865,26.1
+000070f0: 3530 3832 3420 4320 3139 2e39 3730 3138  50824 C 19.97018
+00007100: 362c 3236 2e33 3830 3434 3320 3139 2e39  6,26.380443 19.9
+00007110: 3436 3532 352c 3236 2e36 3133 3232 3220  46525,26.613222 
+00007120: 3139 2e39 3534 3233 312c 3236 2e38 3436  19.954231,26.846
+00007130: 3134 3520 4320 3139 2e39 3633 3837 372c  145 C 19.963877,
+00007140: 3237 2e32 3735 3032 3620 3230 2e30 3337  27.275026 20.037
+00007150: 3831 372c 3237 2e37 3035 3736 2032 302e  817,27.70576 20.
+00007160: 3230 3235 3233 2c32 382e 3130 3332 3633  202523,28.103263
+00007170: 2043 2032 302e 3333 3535 3834 2c32 382e   C 20.335584,28.
+00007180: 3432 3638 3036 2032 302e 3532 3932 3137  426806 20.529217
+00007190: 2c32 382e 3732 3439 3320 3230 2e37 3639  ,28.72493 20.769
+000071a0: 3136 382c 3238 2e39 3739 3336 3320 4320  168,28.979363 C 
+000071b0: 3231 2e30 3037 3133 312c 3239 2e32 3434  21.007131,29.244
+000071c0: 3334 3820 3231 2e32 3936 3438 392c 3239  348 21.296489,29
+000071d0: 2e34 3634 3536 3920 3231 2e36 3230 3537  .464569 21.62057
+000071e0: 382c 3239 2e36 3133 3338 3420 4320 3231  8,29.613384 C 21
+000071f0: 2e39 3636 3631 392c 3239 2e37 3733 3831  .966619,29.77381
+00007200: 3320 3232 2e33 3437 3234 2c32 392e 3835  3 22.34724,29.85
+00007210: 3137 3334 2032 322e 3732 3734 332c 3239  1734 22.72743,29
+00007220: 2e38 3633 3733 3820 4320 3233 2e30 3931  .863738 C 23.091
+00007230: 3032 362c 3239 2e38 3737 3635 3520 3233  026,29.877655 23
+00007240: 2e34 3535 3036 2c32 392e 3832 3235 3033  .45506,29.822503
+00007250: 2032 332e 3830 3335 3737 2c32 392e 3732   23.803577,29.72
+00007260: 3033 3433 2043 2032 342e 3331 3035 3333  0343 C 24.310533
+00007270: 2c32 392e 3537 3137 3720 3234 2e37 3836  ,29.57177 24.786
+00007280: 3330 332c 3239 2e33 3331 3733 3120 3235  303,29.331731 25
+00007290: 2e32 3332 3834 372c 3239 2e30 3532 3034  .232847,29.05204
+000072a0: 3420 4320 3235 2e37 3334 3634 382c 3238  4 C 25.734648,28
+000072b0: 2e37 3336 3533 3720 3236 2e32 3031 3836  .736537 26.20186
+000072c0: 372c 3238 2e33 3638 3737 3920 3236 2e36  7,28.368779 26.6
+000072d0: 3435 3535 312c 3237 2e39 3736 3434 3820  45551,27.976448 
+000072e0: 4320 3237 2e31 3034 3135 382c 3238 2e34  C 27.104158,28.4
+000072f0: 3737 3930 3620 3237 2e35 3632 3736 352c  77906 27.562765,
+00007300: 3238 2e39 3739 3336 3320 3238 2e30 3231  28.979363 28.021
+00007310: 3337 312c 3239 2e34 3830 3832 3120 7a20  371,29.480821 z 
+00007320: 4d20 342e 3734 3930 3237 352c 3139 2e32  M 4.7490275,19.2
+00007330: 3036 3736 3920 4320 342e 3734 3834 3134  06769 C 4.748414
+00007340: 322c 3139 2e37 3535 3035 3220 342e 3833  2,19.755052 4.83
+00007350: 3336 3534 342c 3230 2e33 3035 3837 3720  36544,20.305877 
+00007360: 352e 3032 3435 3132 312c 3230 2e38 3230  5.0245121,20.820
+00007370: 3931 2043 2035 2e32 3032 3138 3431 2c32  91 C 5.2021841,2
+00007380: 312e 3330 3433 3235 2035 2e34 3732 3537  1.304325 5.47257
+00007390: 3234 2c32 312e 3735 3231 3338 2035 2e38  24,21.752138 5.8
+000073a0: 3130 3034 3933 2c32 322e 3134 3036 3434  100493,22.140644
+000073b0: 2043 2036 2e30 3534 3638 3036 2c32 322e   C 6.0546806,22.
+000073c0: 3432 3334 3737 2036 2e33 3334 3735 3332  423477 6.3347532
+000073d0: 2c32 322e 3637 3537 3837 2036 2e36 3431  ,22.675787 6.641
+000073e0: 3832 3831 2c32 322e 3838 3931 3838 2043  8281,22.889188 C
+000073f0: 2037 2e30 3430 3032 3737 2c32 332e 3136   7.0400277,23.16
+00007400: 3539 3431 2037 2e34 3838 3730 3336 2c32  5941 7.4887036,2
+00007410: 332e 3336 3938 3133 2037 2e39 3539 3533  3.369813 7.95953
+00007420: 3031 2c32 332e 3438 3630 3739 2043 2038  01,23.486079 C 8
+00007430: 2e34 3233 3034 3734 2c32 332e 3630 3131  .4230474,23.6011
+00007440: 3531 2038 2e39 3034 3939 3731 2c32 332e  51 8.9049971,23.
+00007450: 3633 3534 3837 2039 2e33 3830 3936 322c  635487 9.380962,
+00007460: 3233 2e36 3033 3536 3420 4320 392e 3836  23.603564 C 9.86
+00007470: 3731 3536 392c 3233 2e35 3730 3330 3820  71569,23.570308 
+00007480: 3130 2e33 3438 3831 322c 3233 2e34 3534  10.348812,23.454
+00007490: 3536 3420 3130 2e37 3932 3332 322c 3233  564 10.792322,23
+000074a0: 2e32 3531 3335 2043 2031 312e 3235 3933  .25135 C 11.2593
+000074b0: 3039 2c32 332e 3033 3930 3138 2031 312e  09,23.039018 11.
+000074c0: 3638 3033 3533 2c32 322e 3733 3239 3031  680353,22.732901
+000074d0: 2031 322e 3034 3333 3736 2c32 322e 3337   12.043376,22.37
+000074e0: 3137 3331 2043 2031 322e 3431 3537 3438  1731 C 12.415748
+000074f0: 2c32 322e 3030 3333 3634 2031 322e 3732  ,22.003364 12.72
+00007500: 3935 3633 2c32 312e 3537 3331 3638 2031  9563,21.573168 1
+00007510: 322e 3934 3931 362c 3231 2e30 3936 3734  2.94916,21.09674
+00007520: 3820 4320 3133 2e31 3636 3133 362c 3230  8 C 13.166136,20
+00007530: 2e36 3239 3435 3520 3133 2e32 3930 3135  .629455 13.29015
+00007540: 342c 3230 2e31 3231 3231 3820 3133 2e33  4,20.121218 13.3
+00007550: 3238 3036 352c 3139 2e36 3037 3938 3820  28065,19.607988 
+00007560: 4320 3133 2e33 3539 3131 2c31 392e 3138  C 13.35911,19.18
+00007570: 3034 3031 2031 332e 3333 3934 3434 2c31  0401 13.339444,1
+00007580: 382e 3734 3833 3737 2031 332e 3236 3130  8.748377 13.2610
+00007590: 3833 2c31 382e 3332 3636 3434 2043 2031  83,18.326644 C 1
+000075a0: 332e 3136 3935 3333 2c31 372e 3833 3234  3.169533,17.8324
+000075b0: 3339 2031 322e 3939 3036 3432 2c31 372e  39 12.990642,17.
+000075c0: 3335 3431 2031 322e 3733 3034 3134 2c31  3541 12.730414,1
+000075d0: 362e 3932 3338 3633 2043 2031 322e 3534  6.923863 C 12.54
+000075e0: 3637 3035 2c31 362e 3631 3932 3236 2031  6705,16.619226 1
+000075f0: 322e 3332 3438 3334 2c31 362e 3333 3739  2.324834,16.3379
+00007600: 3720 3132 2e30 3734 382c 3136 2e30 3835  7 12.0748,16.085
+00007610: 3132 3420 4320 3131 2e37 3037 3530 312c  124 C 11.707501,
+00007620: 3135 2e37 3230 3736 3520 3131 2e32 3830  15.720765 11.280
+00007630: 3631 352c 3135 2e34 3133 3530 3320 3130  615,15.413503 10
+00007640: 2e38 3038 3130 372c 3135 2e32 3030 3734  .808107,15.20074
+00007650: 2043 2031 302e 3335 3338 3633 2c31 342e   C 10.353863,14.
+00007660: 3939 3436 3135 2039 2e38 3631 3030 3737  994615 9.8610077
+00007670: 2c31 342e 3837 3833 3235 2039 2e33 3633  ,14.878325 9.363
+00007680: 3839 3337 2c31 342e 3834 3439 3439 2043  8937,14.844949 C
+00007690: 2038 2e38 3139 3031 3138 2c31 342e 3830   8.8190118,14.80
+000076a0: 3830 3636 2038 2e32 3635 3134 3634 2c31  8066 8.2651464,1
+000076b0: 342e 3835 3835 3334 2037 2e37 3432 3936  4.858534 7.74296
+000076c0: 3739 2c31 352e 3032 3236 3334 2043 2037  79,15.022634 C 7
+000076d0: 2e32 3830 3134 3231 2c31 352e 3136 3636  .2801421,15.1666
+000076e0: 3820 362e 3834 3637 3032 382c 3135 2e34  8 6.8467028,15.4
+000076f0: 3030 3030 3920 362e 3436 3530 3733 372c  00009 6.4650737,
+00007700: 3135 2e36 3938 3231 3320 4320 362e 3035  15.698213 C 6.05
+00007710: 3836 3836 382c 3136 2e30 3135 3332 3920  86868,16.015329 
+00007720: 352e 3730 3338 3136 322c 3136 2e33 3939  5.7038162,16.399
+00007730: 3137 3420 352e 3432 3335 3138 352c 3136  174 5.4235185,16
+00007740: 2e38 3332 3032 3520 4320 352e 3135 3331  .832025 C 5.1531
+00007750: 3438 392c 3137 2e32 3439 3233 3320 342e  489,17.249233 4.
+00007760: 3935 3932 3938 322c 3137 2e37 3135 3633  9592982,17.71563
+00007770: 3120 342e 3835 3339 3632 392c 3138 2e32  1 4.8539629,18.2
+00007780: 3031 3531 3120 4320 342e 3738 3137 3935  01511 C 4.781795
+00007790: 332c 3138 2e35 3331 3335 3620 342e 3734  3,18.531356 4.74
+000077a0: 3839 3530 352c 3138 2e38 3639 3238 3820  89505,18.869288 
+000077b0: 342e 3734 3930 3237 352c 3139 2e32 3036  4.7490275,19.206
+000077c0: 3736 3920 7a20 2720 7374 796c 653d 2766  769 z ' style='f
+000077d0: 696c 6c3a 2024 7a6f 6469 6163 5f63 6f6c  ill: $zodiac_col
+000077e0: 6f72 5f34 3b27 202f 3e0d 0a20 2020 2020  or_4;' />..     
+000077f0: 2020 2020 2020 2020 2020 203c 2f73 796d             </sym
+00007800: 626f 6c3e 0d0a 2020 2020 2020 2020 2020  bol>..          
+00007810: 2020 2020 2020 3c73 796d 626f 6c20 6964        <symbol id
+00007820: 3d27 7669 7267 6f27 3e0d 0a20 2020 2020  ='virgo'>..     
+00007830: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00007840: 7061 7468 2074 7261 6e73 666f 726d 3d22  path transform="
+00007850: 7363 616c 6528 302e 3829 2220 643d 274d  scale(0.8)" d='M
+00007860: 2037 2e31 3633 3238 3535 2c39 2e37 3438   7.1632855,9.748
+00007870: 3833 3633 2043 2037 2e31 3633 3238 3535  8363 C 7.1632855
+00007880: 2c31 342e 3934 3938 3639 2037 2e31 3633  ,14.949869 7.163
+00007890: 3238 3535 2c32 302e 3135 3039 3033 2037  2855,20.150903 7
+000078a0: 2e31 3633 3238 3535 2c32 352e 3335 3139  .1632855,25.3519
+000078b0: 3336 2043 2036 2e33 3331 3035 3435 2c32  36 C 6.3310545,2
+000078c0: 352e 3335 3139 3336 2035 2e34 3938 3832  5.351936 5.49882
+000078d0: 3335 2c32 352e 3335 3139 3336 2034 2e36  35,25.351936 4.6
+000078e0: 3636 3539 3235 2c32 352e 3335 3139 3336  665925,25.351936
+000078f0: 2043 2034 2e36 3636 3539 3235 2c31 392e   C 4.6665925,19.
+00007900: 3332 3831 3634 2034 2e36 3636 3539 3235  328164 4.6665925
+00007910: 2c31 332e 3330 3433 3932 2034 2e36 3636  ,13.304392 4.666
+00007920: 3539 3235 2c37 2e32 3830 3631 3938 2043  5925,7.2806198 C
+00007930: 2034 2e36 3637 3334 3235 2c36 2e31 3035   4.6673425,6.105
+00007940: 3832 3636 2034 2e35 3133 3738 3235 2c34  8266 4.5137825,4
+00007950: 2e39 3238 3932 3837 2034 2e31 3835 3733  .9289287 4.18573
+00007960: 3435 2c33 2e37 3939 3838 3220 4320 332e  45,3.799882 C 3.
+00007970: 3837 3138 3739 352c 322e 3731 3339 3830  8718795,2.713980
+00007980: 3720 332e 3339 3638 3936 352c 312e 3637  7 3.3968965,1.67
+00007990: 3537 3630 3620 322e 3738 3934 3134 392c  57606 2.7894149,
+000079a0: 302e 3732 3234 3935 3435 2043 2032 2e37  0.72249545 C 2.7
+000079b0: 3334 3830 3037 2c30 2e36 3334 3436 3537  348007,0.6344657
+000079c0: 2032 2e36 3730 3632 3537 2c30 2e35 3432   2.6706257,0.542
+000079d0: 3635 3931 3920 322e 3631 3931 3239 332c  65919 2.6191293,
+000079e0: 302e 3435 3839 3134 3720 4320 332e 3439  0.4589147 C 3.49
+000079f0: 3632 3138 352c 302e 3435 3839 3134 3720  62185,0.4589147 
+00007a00: 342e 3337 3333 3036 352c 302e 3435 3839  4.3733065,0.4589
+00007a10: 3134 3720 352e 3235 3033 3936 352c 302e  147 5.2503965,0.
+00007a20: 3435 3839 3134 3720 4320 352e 3739 3831  4589147 C 5.7981
+00007a30: 3936 352c 312e 3230 3939 3638 3320 362e  965,1.2099683 6.
+00007a40: 3231 3339 3734 352c 322e 3035 3039 3539  2139745,2.050959
+00007a50: 3320 362e 3532 3735 3931 352c 322e 3932  3 6.5275915,2.92
+00007a60: 3430 3037 3320 4320 362e 3831 3431 3637  40073 C 6.814167
+00007a70: 352c 332e 3732 3230 3834 3820 372e 3031  5,3.7220848 7.01
+00007a80: 3737 3134 352c 342e 3534 3832 3134 3320  77145,4.5482143 
+00007a90: 372e 3136 3332 3835 352c 352e 3338 3239  7.1632855,5.3829
+00007aa0: 3435 3520 4320 372e 3630 3731 3434 352c  455 C 7.6071445,
+00007ab0: 342e 3239 3539 3631 3320 382e 3132 3333  4.2959613 8.1233
+00007ac0: 3637 352c 332e 3233 3535 3036 3220 382e  675,3.2355062 8.
+00007ad0: 3735 3131 3336 352c 322e 3234 3138 3430  7511365,2.241840
+00007ae0: 3520 4320 392e 3134 3933 3936 352c 312e  5 C 9.1493965,1.
+00007af0: 3631 3234 3630 3120 392e 3539 3332 3737  6124601 9.593277
+00007b00: 352c 312e 3031 3034 3538 3320 3130 2e30  5,1.0104583 10.0
+00007b10: 3934 3732 372c 302e 3435 3839 3134 3720  94727,0.4589147 
+00007b20: 4320 3130 2e39 3130 3339 362c 302e 3330  C 10.910396,0.30
+00007b30: 3539 3433 3535 2031 312e 3732 3630 3635  594355 11.726065
+00007b40: 2c30 2e31 3532 3937 3131 3620 3132 2e35  ,0.15297116 12.5
+00007b50: 3431 3733 342c 342e 3434 3038 3932 3165  41734,4.4408921e
+00007b60: 2d31 3520 4320 3133 2e31 3135 3432 382c  -15 C 13.115428,
+00007b70: 302e 3733 3736 3233 3535 2031 332e 3535  0.73762355 13.55
+00007b80: 3638 3538 2c31 2e35 3732 3038 3933 2031  6858,1.5720893 1
+00007b90: 332e 3838 3631 3239 2c32 2e34 3434 3637  3.886129,2.44467
+00007ba0: 3039 2043 2031 342e 3237 3135 3935 2c33  09 C 14.271595,3
+00007bb0: 2e34 3636 3033 3532 2031 342e 3530 3931  .4660352 14.5091
+00007bc0: 362c 342e 3533 3832 3734 3520 3134 2e36  6,4.5382745 14.6
+00007bd0: 3531 3531 322c 352e 3631 3839 3439 3220  51512,5.6189492 
+00007be0: 4320 3134 2e36 3536 3338 332c 352e 3635  C 14.656383,5.65
+00007bf0: 3630 3239 3520 3134 2e36 3631 3134 312c  60295 14.661141,
+00007c00: 352e 3639 3331 3233 3420 3134 2e36 3635  5.6931234 14.665
+00007c10: 3738 362c 352e 3733 3032 3332 3320 4320  786,5.7302323 C 
+00007c20: 3135 2e30 3338 3839 332c 342e 3535 3438  15.038893,4.5548
+00007c30: 3634 3920 3135 2e35 3930 3537 312c 332e  649 15.590571,3.
+00007c40: 3434 3034 3139 3120 3136 2e32 3538 3132  4404191 16.25812
+00007c50: 322c 322e 3430 3437 3732 3620 4320 3136  2,2.4047726 C 16
+00007c60: 2e36 3936 3633 362c 312e 3732 3431 3237  .696636,1.724127
+00007c70: 3720 3137 2e31 3835 3030 342c 312e 3037  7 17.185004,1.07
+00007c80: 3631 3136 3620 3137 2e37 3039 3031 392c  61166 17.709019,
+00007c90: 302e 3435 3839 3134 3720 4320 3138 2e35  0.4589147 C 18.5
+00007ca0: 3132 3236 372c 302e 3330 3539 3433 3535  12267,0.30594355
+00007cb0: 2031 392e 3331 3535 3134 2c30 2e31 3532   19.315514,0.152
+00007cc0: 3937 3131 3620 3230 2e31 3138 3736 322c  97116 20.118762,
+00007cd0: 342e 3434 3038 3932 3165 2d31 3520 4320  4.4408921e-15 C 
+00007ce0: 3230 2e37 3236 3535 392c 302e 3833 3934  20.726559,0.8394
+00007cf0: 3536 3635 2032 312e 3232 3238 3736 2c31  5665 21.222876,1
+00007d00: 2e37 3631 3736 3132 2032 312e 3536 3532  .7617612 21.5652
+00007d10: 3435 2c32 2e37 3430 3431 3534 2043 2032  45,2.7404154 C 2
+00007d20: 312e 3839 3831 3634 2c33 2e36 3837 3230  1.898164,3.68720
+00007d30: 3335 2032 322e 3038 3530 3536 2c34 2e36  35 22.085056,4.6
+00007d40: 3833 3633 3339 2032 322e 3133 3131 3537  836339 22.131157
+00007d50: 2c35 2e36 3835 3630 3936 2043 2032 322e  ,5.6856096 C 22.
+00007d60: 3134 3336 3038 2c35 2e39 3237 3033 3620  143608,5.927036 
+00007d70: 3232 2e31 3433 3639 362c 362e 3136 3837  22.143696,6.1687
+00007d80: 3837 3320 3232 2e31 3433 3434 342c 362e  873 22.143444,6.
+00007d90: 3431 3034 3534 3220 4320 3232 2e31 3433  4104542 C 22.143
+00007da0: 3434 342c 372e 3932 3432 3832 3320 3232  444,7.9242823 22
+00007db0: 2e31 3433 3434 342c 392e 3433 3831 3039  .143444,9.438109
+00007dc0: 3220 3232 2e31 3433 3434 342c 3130 2e39  2 22.143444,10.9
+00007dd0: 3531 3933 3720 4320 3232 2e34 3831 3334  51937 C 22.48134
+00007de0: 392c 392e 3939 3830 3235 3320 3232 2e38  9,9.9980253 22.8
+00007df0: 3538 3939 322c 392e 3035 3636 3737 3920  58992,9.0566779 
+00007e00: 3233 2e33 3039 3635 392c 382e 3134 3938  23.309659,8.1498
+00007e10: 3635 2043 2032 332e 3539 3633 342c 372e  65 C 23.59634,7.
+00007e20: 3537 3533 3431 2032 332e 3931 3233 3236  575341 23.912326
+00007e30: 2c37 2e30 3133 3937 3739 2032 342e 3237  ,7.0139779 24.27
+00007e40: 3939 3137 2c36 2e34 3836 3832 3134 2043  9917,6.4868214 C
+00007e50: 2032 342e 3936 3732 3332 2c36 2e32 3334   24.967232,6.234
+00007e60: 3632 3534 2032 352e 3635 3435 3438 2c35  6254 25.654548,5
+00007e70: 2e39 3832 3432 3832 2032 362e 3334 3138  .9824282 26.3418
+00007e80: 3633 2c35 2e37 3330 3233 3233 2043 2032  63,5.7302323 C 2
+00007e90: 372e 3134 3634 3431 2c36 2e39 3730 3637  7.146441,6.97067
+00007ea0: 3632 2032 372e 3830 3637 3537 2c38 2e33  62 27.806757,8.3
+00007eb0: 3038 3039 3838 2032 382e 3236 3234 3532  080988 28.262452
+00007ec0: 2c39 2e37 3135 3434 3735 2043 2032 382e  ,9.7154475 C 28.
+00007ed0: 3637 3930 3231 2c31 302e 3939 3731 3238  679021,10.997128
+00007ee0: 2032 382e 3932 3330 3137 2c31 322e 3333   28.923017,12.33
+00007ef0: 3436 3235 2032 382e 3938 3338 3739 2c31  4625 28.983879,1
+00007f00: 332e 3638 3037 3938 2043 2032 392e 3034  3.680798 C 29.04
+00007f10: 3939 3936 2c31 352e 3135 3138 3620 3238  9996,15.15186 28
+00007f20: 2e39 3133 3737 2c31 362e 3633 3339 3736  .91377,16.633976
+00007f30: 2032 382e 3535 3632 3534 2c31 382e 3036   28.556254,18.06
+00007f40: 3334 3031 2043 2032 382e 3135 3936 3435  3401 C 28.159645
+00007f50: 2c31 392e 3635 3437 3937 2032 372e 3439  ,19.654797 27.49
+00007f60: 3132 3738 2c32 312e 3137 3536 3620 3236  1278,21.17566 26
+00007f70: 2e36 3038 3734 362c 3232 2e35 3537 3634  .608746,22.55764
+00007f80: 3920 4320 3235 2e37 3936 3539 352c 3233  9 C 25.796595,23
+00007f90: 2e38 3331 3637 3220 3234 2e38 3131 3934  .831672 24.81194
+00007fa0: 2c32 342e 3939 3035 3332 2032 332e 3732  ,24.990532 23.72
+00007fb0: 3930 3533 2c32 362e 3034 3236 3231 2043  9053,26.042621 C
+00007fc0: 2032 332e 3337 3632 3135 2c32 362e 3338   23.376215,26.38
+00007fd0: 3534 3338 2032 332e 3031 3236 3738 2c32  5438 23.012678,2
+00007fe0: 362e 3731 3732 3238 2032 322e 3634 3032  6.717228 22.6402
+00007ff0: 3938 2c32 372e 3033 3837 3538 2043 2032  98,27.038758 C 2
+00008000: 322e 3733 3039 3036 2c32 372e 3730 3332  2.730906,27.7032
+00008010: 3239 2032 322e 3934 3638 3131 2c32 382e  29 22.946811,28.
+00008020: 3334 3532 3820 3233 2e32 3235 3738 312c  34528 23.225781,
+00008030: 3238 2e39 3533 3335 3420 4320 3233 2e35  28.953354 C 23.5
+00008040: 3733 3039 2c32 392e 3730 3735 3631 2032  7309,29.707561 2
+00008050: 342e 3031 3636 3931 2c33 302e 3431 3339  4.016691,30.4139
+00008060: 3938 2032 342e 3530 3336 3139 2c33 312e  98 24.503619,31.
+00008070: 3038 3534 3836 2043 2032 342e 3733 3032  085486 C 24.7302
+00008080: 3139 2c33 312e 3339 3734 3037 2032 342e  19,31.397407 24.
+00008090: 3936 3730 3539 2c33 312e 3730 3138 3438  967059,31.701848
+000080a0: 2032 352e 3231 3135 3139 2c33 312e 3939   25.211519,31.99
+000080b0: 3939 3938 2043 2032 342e 3233 3433 3732  9998 C 24.234372
+000080c0: 2c33 312e 3939 3939 3938 2032 332e 3235  ,31.999998 23.25
+000080d0: 3732 3236 2c33 312e 3939 3939 3938 2032  7226,31.999998 2
+000080e0: 322e 3238 3030 3739 2c33 312e 3939 3939  2.280079,31.9999
+000080f0: 3938 2043 2032 312e 3831 3537 3136 2c33  98 C 21.815716,3
+00008100: 312e 3431 3332 3138 2032 312e 3433 3233  1.413218 21.4323
+00008110: 3638 2c33 302e 3736 3633 3137 2032 312e  68,30.766317 21.
+00008120: 3130 3033 3435 2c33 302e 3039 3730 3731  100345,30.097071
+00008130: 2043 2032 302e 3833 3337 3436 2c32 392e   C 20.833746,29.
+00008140: 3535 3834 3535 2032 302e 3630 3037 3536  558455 20.600756
+00008150: 2c32 392e 3030 3336 3733 2032 302e 3339  ,29.003673 20.39
+00008160: 3230 3332 2c32 382e 3434 3033 3038 2043  2032,28.440308 C
+00008170: 2031 392e 3339 3634 3232 2c32 392e 3030   19.396422,29.00
+00008180: 3436 3338 2031 382e 3332 3333 3931 2c32  4638 18.323391,2
+00008190: 392e 3432 3338 3239 2031 372e 3232 3437  9.423829 17.2247
+000081a0: 3932 2c32 392e 3734 3031 3233 2043 2031  92,29.740123 C 1
+000081b0: 362e 3338 3439 3731 2c32 392e 3938 3136  6.384971,29.9816
+000081c0: 3038 2031 352e 3532 3836 312c 3330 2e31  08 15.52861,30.1
+000081d0: 3633 3338 3520 3134 2e36 3635 3738 362c  63385 14.665786,
+000081e0: 3330 2e33 3030 3737 3320 4320 3134 2e36  30.300773 C 14.6
+000081f0: 3635 3738 362c 3239 2e35 3839 3636 3220  65786,29.589662 
+00008200: 3134 2e36 3635 3738 362c 3238 2e38 3738  14.665786,28.878
+00008210: 3535 3120 3134 2e36 3635 3738 362c 3238  551 14.665786,28
+00008220: 2e31 3637 3434 2043 2031 352e 3831 3235  .16744 C 15.8125
+00008230: 3032 2c32 372e 3933 3338 3831 2031 362e  02,27.933881 16.
+00008240: 3934 3636 3031 2c32 372e 3632 3534 3236  946601,27.625426
+00008250: 2031 382e 3033 3635 3639 2c32 372e 3139   18.036569,27.19
+00008260: 3732 3331 2043 2031 382e 3638 3134 3833  7231 C 18.681483
+00008270: 2c32 362e 3934 3333 3539 2031 392e 3331  ,26.943359 19.31
+00008280: 3034 3632 2c32 362e 3634 3637 3833 2031  0462,26.646783 1
+00008290: 392e 3930 3735 3939 2c32 362e 3239 3435  9.907599,26.2945
+000082a0: 3732 2043 2031 392e 3733 3037 3337 2c32  72 C 19.730737,2
+000082b0: 352e 3139 3936 3120 3139 2e36 3433 3233  5.19961 19.64323
+000082c0: 322c 3234 2e30 3930 3239 2031 392e 3634  2,24.09029 19.64
+000082d0: 3637 3531 2c32 322e 3938 3131 3734 2043  6751,22.981174 C
+000082e0: 2031 392e 3634 3637 342c 3137 2e39 3438   19.64674,17.948
+000082f0: 3837 3720 3139 2e36 3436 3737 322c 3132  877 19.646772,12
+00008300: 2e39 3136 3537 3820 3139 2e36 3436 3733  .916578 19.64673
+00008310: 352c 372e 3838 3432 3831 3120 4320 3139  5,7.8842811 C 19
+00008320: 2e36 3434 3935 312c 362e 3935 3032 3032  .644951,6.950202
+00008330: 3420 3139 2e35 3937 3032 362c 362e 3031  4 19.597026,6.01
+00008340: 3431 3238 2031 392e 3435 3536 3737 2c35  4128 19.455677,5
+00008350: 2e30 3839 3939 3636 2043 2031 392e 3334  .0899966 C 19.34
+00008360: 3835 3232 2c34 2e33 3938 3235 3731 2031  8522,4.3982571 1
+00008370: 392e 3138 3839 3536 2c33 2e37 3131 3234  9.188956,3.71124
+00008380: 3720 3138 2e39 3330 3932 342c 332e 3035  7 18.930924,3.05
+00008390: 3930 3935 3720 4320 3138 2e38 3330 3037  90957 C 18.83007
+000083a0: 362c 322e 3830 3530 3935 3120 3138 2e37  6,2.8050951 18.7
+000083b0: 3133 3739 382c 322e 3535 3639 3733 3520  13798,2.5569735 
+000083c0: 3138 2e35 3738 3531 342c 322e 3331 3933  18.578514,2.3193
+000083d0: 3739 3820 4320 3137 2e37 3338 3937 372c  798 C 17.738977,
+000083e0: 332e 3232 3234 3536 3920 3137 2e30 3437  3.2224569 17.047
+000083f0: 3935 392c 342e 3235 3538 3334 3820 3136  959,4.2558348 16
+00008400: 2e34 3739 3730 362c 352e 3334 3735 3934  .479706,5.347594
+00008410: 3120 4320 3135 2e38 3234 3432 392c 362e  1 C 15.824429,6.
+00008420: 3630 3734 3837 3420 3135 2e33 3237 3634  6074874 15.32764
+00008430: 372c 372e 3934 3437 3739 3720 3134 2e39  7,7.9447797 14.9
+00008440: 3337 3336 332c 392e 3330 3834 3138 3720  37363,9.3084187 
+00008450: 4320 3134 2e38 3430 3439 392c 392e 3634  C 14.840499,9.64
+00008460: 3834 3833 3220 3134 2e37 3439 3034 392c  84832 14.749049,
+00008470: 392e 3939 3032 3934 3320 3134 2e36 3635  9.9902943 14.665
+00008480: 3738 362c 3130 2e33 3333 3834 2043 2031  786,10.33384 C 1
+00008490: 342e 3636 3537 3836 2c31 352e 3333 3938  4.665786,15.3398
+000084a0: 3732 2031 342e 3636 3537 3836 2c32 302e  72 14.665786,20.
+000084b0: 3334 3539 3034 2031 342e 3636 3537 3836  345904 14.665786
+000084c0: 2c32 352e 3335 3139 3336 2043 2031 332e  ,25.351936 C 13.
+000084d0: 3832 3934 3135 2c32 352e 3335 3139 3336  829415,25.351936
+000084e0: 2031 322e 3939 3330 3433 2c32 352e 3335   12.993043,25.35
+000084f0: 3139 3336 2031 322e 3135 3636 3732 2c32  1936 12.156672,2
+00008500: 352e 3335 3139 3336 2043 2031 322e 3135  5.351936 C 12.15
+00008510: 3636 3631 2c31 392e 3830 3831 3034 2031  6661,19.808104 1
+00008520: 322e 3135 3636 3934 2c31 342e 3236 3432  2.156694,14.2642
+00008530: 3732 2031 322e 3135 3636 3535 2c38 2e37  72 12.156655,8.7
+00008540: 3230 3433 3938 2043 2031 322e 3135 3438  204398 C 12.1548
+00008550: 3636 2c37 2e36 3935 3936 3336 2031 322e  66,7.6959636 12.
+00008560: 3131 3630 3635 2c36 2e36 3730 3132 3433  116065,6.6701243
+00008570: 2031 312e 3939 3735 3233 2c35 2e36 3531   11.997523,5.651
+00008580: 3938 3131 2043 2031 312e 3931 3631 3631  9811 C 11.916161
+00008590: 2c34 2e39 3636 3532 3633 2031 312e 3739  ,4.9665263 11.79
+000085a0: 3939 3538 2c34 2e32 3833 3033 3938 2031  9958,4.2830398 1
+000085b0: 312e 3630 3636 3131 2c33 2e36 3139 3531  1.606611,3.61951
+000085c0: 3336 2043 2031 312e 3437 3336 3433 2c33  36 C 11.473643,3
+000085d0: 2e31 3638 3438 3938 2031 312e 3330 3530  .1684898 11.3050
+000085e0: 3338 2c32 2e37 3234 3436 3837 2031 312e  38,2.7244687 11.
+000085f0: 3036 3335 3932 2c32 2e33 3139 3337 3938  063592,2.3193798
+00008600: 2043 2031 302e 3130 3134 3034 2c33 2e34   C 10.101404,3.4
+00008610: 3338 3036 3939 2039 2e32 3932 3138 3035  380699 9.2921805
+00008620: 2c34 2e36 3834 3236 3339 2038 2e36 3331  ,4.6842639 8.631
+00008630: 3730 3735 2c36 2e30 3032 3220 4320 382e  7075,6.0022 C 8.
+00008640: 3032 3932 3034 352c 372e 3230 3330 3433  0292045,7.203043
+00008650: 3320 372e 3534 3736 3131 352c 382e 3436  3 7.5476115,8.46
+00008660: 3233 3732 3220 372e 3136 3332 3835 352c  23722 7.1632855,
+00008670: 392e 3734 3838 3336 3320 7a20 4d20 3232  9.7488363 z M 22
+00008680: 2e31 3433 3434 342c 3234 2e37 3036 3937  .143444,24.70697
+00008690: 3520 4320 3233 2e30 3736 3231 312c 3233  5 C 23.076211,23
+000086a0: 2e37 3630 3437 3220 3233 2e39 3039 3835  .760472 23.90985
+000086b0: 392c 3232 2e37 3132 3631 3420 3234 2e35  9,22.712614 24.5
+000086c0: 3837 3631 382c 3231 2e35 3638 3833 3820  87618,21.568838 
+000086d0: 4320 3234 2e39 3134 3737 312c 3231 2e30  C 24.914771,21.0
+000086e0: 3136 3635 3320 3235 2e32 3036 3835 312c  16653 25.206851,
+000086f0: 3230 2e34 3433 3432 3920 3235 2e34 3536  20.443429 25.456
+00008700: 3138 392c 3139 2e38 3532 3034 3820 4320  189,19.852048 C 
+00008710: 3235 2e39 3239 3438 392c 3138 2e37 3137  25.929489,18.717
+00008720: 3539 3420 3236 2e32 3434 3831 372c 3137  594 26.244817,17
+00008730: 2e35 3138 3039 3620 3236 2e33 3935 3135  .518096 26.39515
+00008740: 332c 3136 2e32 3938 3437 3620 4320 3236  3,16.298476 C 26
+00008750: 2e34 3931 3439 322c 3135 2e35 3136 3937  .491492,15.51697
+00008760: 3120 3236 2e35 3233 3630 332c 3134 2e37  1 26.523603,14.7
+00008770: 3237 3530 3120 3236 2e34 3930 3930 322c  27501 26.490902,
+00008780: 3133 2e39 3430 3737 3520 4320 3236 2e34  13.940775 C 26.4
+00008790: 3430 3939 362c 3132 2e37 3536 3135 3920  40996,12.756159 
+000087a0: 3236 2e32 3331 3232 372c 3131 2e35 3738  26.231227,11.578
+000087b0: 3830 3220 3235 2e38 3732 3739 332c 3130  802 25.872793,10
+000087c0: 2e34 3438 3537 2043 2032 352e 3638 3630  .44857 C 25.6860
+000087d0: 3836 2c39 2e38 3538 3338 3833 2032 352e  86,9.8583883 25.
+000087e0: 3435 3938 3034 2c39 2e32 3830 3834 3431  459804,9.2808441
+000087f0: 2032 352e 3139 3930 3938 2c38 2e37 3139   25.199098,8.719
+00008800: 3337 3934 2043 2032 342e 3530 3432 3332  3794 C 24.504232
+00008810: 2c39 2e35 3733 3339 3620 3233 2e39 3333  ,9.573396 23.933
+00008820: 3132 362c 3130 2e35 3232 3039 3920 3233  126,10.522099 23
+00008830: 2e34 3438 3939 312c 3131 2e35 3038 3931  .448991,11.50891
+00008840: 3420 4320 3232 2e39 3236 3238 392c 3132  4 C 22.926289,12
+00008850: 2e35 3736 3234 3520 3232 2e35 3033 3237  .576245 22.50327
+00008860: 372c 3133 2e36 3839 3935 3720 3232 2e31  7,13.689957 22.1
+00008870: 3433 3434 342c 3134 2e38 3231 3730 3420  43444,14.821704 
+00008880: 4320 3232 2e31 3433 3434 342c 3138 2e31  C 22.143444,18.1
+00008890: 3136 3739 3520 3232 2e31 3433 3434 342c  16795 22.143444,
+000088a0: 3231 2e34 3131 3838 3420 3232 2e31 3433  21.411884 22.143
+000088b0: 3434 342c 3234 2e37 3036 3937 3520 7a20  444,24.706975 z 
+000088c0: 2720 7374 796c 653d 2766 696c 6c3a 2024  ' style='fill: $
+000088d0: 7a6f 6469 6163 5f63 6f6c 6f72 5f35 3b27  zodiac_color_5;'
+000088e0: 202f 3e0d 0a20 2020 2020 2020 2020 2020   />..           
+000088f0: 2020 2020 203c 2f73 796d 626f 6c3e 0d0a       </symbol>..
+00008900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008910: 3c73 796d 626f 6c20 6964 3d27 6c69 6272  <symbol id='libr
+00008920: 6127 3e0d 0a20 2020 2020 2020 2020 2020  a'>..           
+00008930: 2020 2020 2020 2020 203c 7061 7468 2074           <path t
+00008940: 7261 6e73 666f 726d 3d22 7363 616c 6528  ransform="scale(
+00008950: 302e 3829 2220 643d 274d 202d 352e 3539  0.8)" d='M -5.59
+00008960: 3632 3565 2d30 362c 3239 2e31 3930 3730  625e-06,29.19070
+00008970: 3920 4320 2d35 2e35 3936 3235 652d 3036  9 C -5.59625e-06
+00008980: 2c32 382e 3230 3337 3232 202d 352e 3539  ,28.203722 -5.59
+00008990: 3632 3565 2d30 362c 3237 2e32 3136 3733  625e-06,27.21673
+000089a0: 3520 2d35 2e35 3936 3235 652d 3036 2c32  5 -5.59625e-06,2
+000089b0: 362e 3232 3937 3335 2043 2031 302e 3636  6.229735 C 10.66
+000089c0: 3636 3637 2c32 362e 3232 3937 3335 2032  6667,26.229735 2
+000089d0: 312e 3333 3333 3237 2c32 362e 3232 3937  1.333327,26.2297
+000089e0: 3335 2033 322c 3236 2e32 3239 3733 3520  35 32,26.229735 
+000089f0: 4320 3332 2c32 372e 3231 3637 3335 2033  C 32,27.216735 3
+00008a00: 322c 3238 2e32 3033 3732 3220 3332 2c32  2,28.203722 32,2
+00008a10: 392e 3139 3037 3039 2043 2032 312e 3333  9.190709 C 21.33
+00008a20: 3333 3237 2c32 392e 3139 3037 3039 2031  3327,29.190709 1
+00008a30: 302e 3636 3636 3637 2c32 392e 3139 3037  0.666667,29.1907
+00008a40: 3039 202d 352e 3539 3632 3565 2d30 362c  09 -5.59625e-06,
+00008a50: 3239 2e31 3930 3730 3920 7a20 4d20 3132  29.190709 z M 12
+00008a60: 2e36 3438 3735 2c31 372e 3530 3936 3120  .64875,17.50961 
+00008a70: 4320 3132 2e36 3438 3735 2c31 382e 3433  C 12.64875,18.43
+00008a80: 3234 3436 2031 322e 3634 3837 352c 3139  2446 12.64875,19
+00008a90: 2e33 3535 3238 3320 3132 2e36 3438 3735  .355283 12.64875
+00008aa0: 2c32 302e 3237 3831 3333 2043 2038 2e34  ,20.278133 C 8.4
+00008ab0: 3332 3530 3233 2c32 302e 3237 3831 3333  325023,20.278133
+00008ac0: 2034 2e32 3136 3234 3138 2c32 302e 3237   4.2162418,20.27
+00008ad0: 3831 3333 202d 352e 3539 3632 3565 2d30  8133 -5.59625e-0
+00008ae0: 362c 3230 2e32 3738 3133 3320 4320 2d35  6,20.278133 C -5
+00008af0: 2e35 3936 3235 652d 3036 2c31 392e 3238  .59625e-06,19.28
+00008b00: 3631 3736 202d 352e 3539 3632 3565 2d30  6176 -5.59625e-0
+00008b10: 362c 3138 2e32 3934 3233 3120 2d35 2e35  6,18.294231 -5.5
+00008b20: 3936 3235 652d 3036 2c31 372e 3330 3232  9625e-06,17.3022
+00008b30: 3836 2043 2032 2e39 3535 3831 372c 3137  86 C 2.955817,17
+00008b40: 2e33 3032 3238 3620 352e 3931 3136 3339  .302286 5.911639
+00008b50: 362c 3137 2e33 3032 3238 3620 382e 3836  6,17.302286 8.86
+00008b60: 3734 3632 332c 3137 2e33 3032 3238 3620  74623,17.302286 
+00008b70: 4320 372e 3833 3330 3031 392c 3136 2e32  C 7.8330019,16.2
+00008b80: 3538 3331 3920 372e 3031 3231 3234 372c  58319 7.0121247,
+00008b90: 3134 2e39 3730 3432 3620 362e 3636 3235  14.970426 6.6625
+00008ba0: 3137 312c 3133 2e35 3333 3630 3820 4320  171,13.533608 C 
+00008bb0: 362e 3336 3531 3036 342c 3132 2e33 3335  6.3651064,12.335
+00008bc0: 3737 3220 362e 3339 3933 3832 392c 3131  772 6.3993829,11
+00008bd0: 2e30 3733 3533 3820 362e 3633 3933 3833  .073538 6.639383
+00008be0: 372c 392e 3836 3930 3339 3520 4320 362e  7,9.8690395 C 6.
+00008bf0: 3934 3531 3039 352c 382e 3335 3537 3631  9451095,8.355761
+00008c00: 3620 372e 3639 3233 3839 392c 362e 3934  6 7.6923899,6.94
+00008c10: 3834 3239 3320 382e 3731 3739 3837 392c  84293 8.7179879,
+00008c20: 352e 3739 3839 3230 3320 4320 392e 3837  5.7989203 C 9.87
+00008c30: 3234 3638 332c 342e 3439 3232 3736 3220  24683,4.4922762 
+00008c40: 3131 2e33 3435 3434 372c 332e 3433 3933  11.345447,3.4393
+00008c50: 3935 3720 3133 2e30 3136 3635 352c 322e  957 13.016655,2.
+00008c60: 3930 3733 3932 3720 4320 3134 2e35 3139  9073927 C 14.519
+00008c70: 3930 392c 322e 3432 3531 3631 3320 3136  909,2.4251613 16
+00008c80: 2e31 3430 3038 312c 322e 3333 3737 3834  .140081,2.337784
+00008c90: 3520 3137 2e36 3935 3237 312c 322e 3538  5 17.695271,2.58
+00008ca0: 3934 3636 3120 4320 3139 2e32 3636 3433  94661 C 19.26643
+00008cb0: 392c 322e 3834 3532 3732 3620 3230 2e37  9,2.8452726 20.7
+00008cc0: 3536 3131 332c 332e 3533 3637 3532 3820  56113,3.5367528 
+00008cd0: 3231 2e39 3836 3133 322c 342e 3534 3234  21.986132,4.5424
+00008ce0: 3737 3220 4320 3233 2e32 3836 3939 382c  772 C 23.286998,
+00008cf0: 352e 3630 3232 3431 3220 3234 2e33 3835  5.6022412 24.385
+00008d00: 3638 342c 362e 3935 3135 3133 3220 3234  684,6.9515132 24
+00008d10: 2e39 3836 3230 312c 382e 3532 3838 3838  .986201,8.528888
+00008d20: 3720 4320 3235 2e34 3633 3036 322c 392e  7 C 25.463062,9.
+00008d30: 3737 3236 3537 3920 3235 2e36 3430 3132  7726579 25.64012
+00008d40: 372c 3131 2e31 3236 3339 3420 3235 2e35  7,11.126394 25.5
+00008d50: 3333 3535 372c 3132 2e34 3532 3136 3620  33557,12.452166 
+00008d60: 4320 3235 2e34 3136 3637 382c 3133 2e38  C 25.416678,13.8
+00008d70: 3230 3334 3420 3234 2e38 3738 3932 372c  20344 24.878927,
+00008d80: 3135 2e31 3335 3930 3220 3234 2e30 3631  15.135902 24.061
+00008d90: 3435 322c 3136 2e32 3334 3835 3820 4320  452,16.234858 C 
+00008da0: 3233 2e37 3833 3630 332c 3136 2e36 3132  23.783603,16.612
+00008db0: 3531 3120 3233 2e34 3736 3131 382c 3136  511 23.476118,16
+00008dc0: 2e39 3638 3035 3620 3233 2e31 3437 3335  .968056 23.14735
+00008dd0: 2c31 372e 3330 3233 3133 2043 2032 362e  ,17.302313 C 26.
+00008de0: 3039 3832 3333 2c31 372e 3330 3233 2032  098233,17.3023 2
+00008df0: 392e 3034 3931 3136 2c31 372e 3330 3233  9.049116,17.3023
+00008e00: 2033 322c 3137 2e33 3032 3238 3620 4320   32,17.302286 C 
+00008e10: 3332 2c31 382e 3239 3432 3331 2033 322c  32,18.294231 32,
+00008e20: 3139 2e32 3836 3137 3620 3332 2c32 302e  19.286176 32,20.
+00008e30: 3237 3831 3333 2043 2032 372e 3738 3337  278133 C 27.7837
+00008e40: 3339 2c32 302e 3237 3831 3333 2032 332e  39,20.278133 23.
+00008e50: 3536 3734 3932 2c32 302e 3237 3831 3333  567492,20.278133
+00008e60: 2031 392e 3335 3132 3434 2c32 302e 3237   19.351244,20.27
+00008e70: 3831 3333 2043 2031 392e 3335 3132 3434  8133 C 19.351244
+00008e80: 2c31 392e 3335 3532 3833 2031 392e 3335  ,19.355283 19.35
+00008e90: 3132 3434 2c31 382e 3433 3234 3436 2031  1244,18.432446 1
+00008ea0: 392e 3335 3132 3434 2c31 372e 3530 3936  9.351244,17.5096
+00008eb0: 3120 4320 3230 2e34 3736 3437 392c 3136  1 C 20.476479,16
+00008ec0: 2e37 3837 3139 3920 3231 2e34 3639 3834  .787199 21.46984
+00008ed0: 362c 3135 2e38 3033 3431 3320 3232 2e30  6,15.803413 22.0
+00008ee0: 3238 3135 2c31 342e 3537 3533 3337 2043  2815,14.575337 C
+00008ef0: 2032 322e 3538 3436 3033 2c31 332e 3336   22.584603,13.36
+00008f00: 3239 3420 3232 2e37 3036 3839 2c31 312e  294 22.70689,11.
+00008f10: 3937 3432 3820 3232 2e34 3639 3237 342c  97428 22.469274,
+00008f20: 3130 2e36 3638 3937 3620 4320 3232 2e32  10.668976 C 22.2
+00008f30: 3339 3735 322c 392e 3431 3736 3037 3620  39752,9.4176076 
+00008f40: 3231 2e35 3734 3631 382c 382e 3237 3133  21.574618,8.2713
+00008f50: 3737 3620 3230 2e36 3731 3435 312c 372e  776 20.671451,7.
+00008f60: 3338 3332 3730 3320 4320 3139 2e37 3531  3832703 C 19.751
+00008f70: 3536 332c 362e 3435 3234 3035 2031 382e  563,6.452405 18.
+00008f80: 3536 3136 322c 352e 3737 3138 3638 2031  56162,5.771868 1
+00008f90: 372e 3236 3539 3431 2c35 2e35 3430 3936  7.265941,5.54096
+00008fa0: 3639 2043 2031 352e 3732 3832 3431 2c35  69 C 15.728241,5
+00008fb0: 2e32 3634 3430 3620 3134 2e30 3735 3338  .264406 14.07538
+00008fc0: 332c 352e 3438 3634 3139 3820 3132 2e37  3,5.4864198 12.7
+00008fd0: 3235 3337 2c36 2e32 3935 3336 3120 4320  2537,6.295361 C 
+00008fe0: 3131 2e38 3233 3533 332c 362e 3833 3536  11.823533,6.8356
+00008ff0: 3030 3720 3131 2e30 3439 3837 342c 372e  007 11.049874,7.
+00009000: 3538 3438 3535 2031 302e 3435 3835 3435  584855 10.458545
+00009010: 2c38 2e34 3531 3537 3033 2043 2039 2e37  ,8.4515703 C 9.7
+00009020: 3533 3339 3937 2c39 2e34 3837 3431 3739  533997,9.4874179
+00009030: 2039 2e34 3037 3734 3131 2c31 302e 3734   9.4077411,10.74
+00009040: 3637 3839 2039 2e34 3331 3339 3539 2c31  6789 9.4313959,1
+00009050: 312e 3939 3533 3437 2043 2039 2e34 3336  1.995347 C 9.436
+00009060: 3637 3432 2c31 332e 3139 3838 3720 392e  6742,13.19887 9.
+00009070: 3736 3931 3330 342c 3134 2e34 3039 3734  7691304,14.40974
+00009080: 3420 3130 2e34 3437 3032 342c 3135 2e34  4 10.447024,15.4
+00009090: 3130 3937 3920 4320 3131 2e30 3134 3231  10979 C 11.01421
+000090a0: 352c 3136 2e32 3632 3435 3720 3131 2e37  5,16.262457 11.7
+000090b0: 3932 3736 322c 3136 2e39 3536 3535 3320  92762,16.956553 
+000090c0: 3132 2e36 3438 3735 2c31 372e 3530 3936  12.64875,17.5096
+000090d0: 3120 7a20 2720 7374 796c 653d 2766 696c  1 z ' style='fil
+000090e0: 6c3a 2024 7a6f 6469 6163 5f63 6f6c 6f72  l: $zodiac_color
+000090f0: 5f36 3b27 202f 3e0d 0a20 2020 2020 2020  _6;' />..       
+00009100: 2020 2020 2020 2020 203c 2f73 796d 626f           </symbo
+00009110: 6c3e 0d0a 2020 2020 2020 2020 2020 2020  l>..            
+00009120: 2020 2020 3c73 796d 626f 6c20 6964 3d27      <symbol id='
+00009130: 7363 6f72 7069 6f27 3e0d 0a20 2020 2020  scorpio'>..     
+00009140: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00009150: 7061 7468 2074 7261 6e73 666f 726d 3d22  path transform="
+00009160: 7363 616c 6528 302e 3829 2220 643d 274d  scale(0.8)" d='M
+00009170: 2032 2e30 3731 3737 352c 3235 2e31 3039   2.071775,25.109
+00009180: 3339 3220 4320 322e 3037 3137 3534 322c  392 C 2.0717542,
+00009190: 3139 2e32 3433 3339 3220 322e 3037 3138  19.243392 2.0718
+000091a0: 3136 362c 3133 2e33 3737 3339 3220 322e  166,13.377392 2.
+000091b0: 3037 3137 3433 322c 372e 3531 3133 3932  0717432,7.511392
+000091c0: 3120 4320 322e 3036 3932 3437 352c 362e  1 C 2.0692475,6.
+000091d0: 3334 3332 3236 3520 312e 3935 3833 3939  3432265 1.958399
+000091e0: 372c 352e 3137 3036 3932 3220 312e 3637  7,5.1706922 1.67
+000091f0: 3731 3632 312c 342e 3033 3532 3632 3620  71621,4.0352626 
+00009200: 4320 312e 3433 3733 3139 362c 332e 3036  C 1.4373196,3.06
+00009210: 3632 3537 3520 312e 3036 3835 3934 2c32  62575 1.068594,2
+00009220: 2e31 3235 3134 3335 2030 2e35 3435 3338  .1251435 0.54538
+00009230: 3034 382c 312e 3237 3336 3937 3120 4320  048,1.2736971 C 
+00009240: 302e 3337 3935 3732 3038 2c31 2e30 3033  0.37957208,1.003
+00009250: 3530 3632 2030 2e31 3938 3636 3435 382c  5062 0.19866458,
+00009260: 302e 3734 3235 3934 2030 2e30 3033 3233  0.742594 0.00323
+00009270: 3933 3736 342c 302e 3439 3330 3635 3120  93764,0.4930651 
+00009280: 4320 302e 3838 3435 3038 3938 2c30 2e34  C 0.88450898,0.4
+00009290: 3933 3036 3531 2031 2e37 3635 3737 3836  930651 1.7657786
+000092a0: 2c30 2e34 3933 3036 3531 2032 2e36 3437  ,0.4930651 2.647
+000092b0: 3034 3833 2c30 2e34 3933 3036 3531 2043  0483,0.4930651 C
+000092c0: 2033 2e32 3334 3035 3333 2c31 2e33 3839   3.2340533,1.389
+000092d0: 3439 3331 2033 2e36 3938 3333 3233 2c32  4931 3.6983323,2
+000092e0: 2e33 3635 3139 3031 2034 2e30 3335 3632  .3651901 4.03562
+000092f0: 3733 2c33 2e33 3832 3334 3234 2043 2034  73,3.3823424 C 4
+00009300: 2e32 3437 3936 3133 2c34 2e30 3231 3033  .2479613,4.02103
+00009310: 3733 2034 2e34 3131 3438 3133 2c34 2e36  73 4.4114813,4.6
+00009320: 3735 3636 3620 342e 3533 3139 3836 332c  75666 4.5319863,
+00009330: 352e 3333 3738 3333 2043 2035 2e30 3438  5.337833 C 5.048
+00009340: 3531 3933 2c34 2e30 3630 3139 3738 2035  5193,4.0601978 5
+00009350: 2e36 3834 3634 3933 2c32 2e38 3236 3833  .6846493,2.82683
+00009360: 3839 2036 2e34 3736 3731 3733 2c31 2e36  89 6.4767173,1.6
+00009370: 3937 3936 3520 4320 362e 3736 3939 3339  97965 C 6.769939
+00009380: 332c 312e 3238 3031 3036 3920 372e 3038  3,1.2801069 7.08
+00009390: 3433 3633 332c 302e 3837 3730 3638 3820  43633,0.8770688 
+000093a0: 372e 3432 3035 3932 332c 302e 3439 3330  7.4205923,0.4930
+000093b0: 3635 3120 4320 382e 3231 3231 3033 332c  651 C 8.2121033,
+000093c0: 302e 3333 3336 3137 3120 392e 3030 3336  0.3336171 9.0036
+000093d0: 3133 332c 302e 3137 3431 3639 2039 2e37  133,0.174169 9.7
+000093e0: 3935 3132 3433 2c30 2e30 3134 3732 3130  951243,0.0147210
+000093f0: 3033 2043 2031 302e 3332 3138 2c30 2e36  03 C 10.3218,0.6
+00009400: 3239 3035 3834 2031 302e 3732 3739 372c  290584 10.72797,
+00009410: 312e 3334 3030 3030 3520 3131 2e30 3337  1.3400005 11.037
+00009420: 3731 342c 322e 3038 3631 3538 3520 4320  714,2.0861585 C 
+00009430: 3131 2e34 3031 3335 382c 322e 3936 3239  11.401358,2.9629
+00009440: 3235 3320 3131 2e36 3338 3033 392c 332e  253 11.638039,3.
+00009450: 3838 3830 3031 3220 3131 2e37 3938 3132  8880012 11.79812
+00009460: 352c 342e 3832 3233 3935 2043 2031 312e  5,4.822395 C 11.
+00009470: 3834 3139 3732 2c35 2e30 3739 3137 3633  841972,5.0791763
+00009480: 2031 312e 3837 3938 3837 2c35 2e33 3336   11.879887,5.336
+00009490: 3936 3538 2031 312e 3931 3236 3139 2c35  9658 11.912619,5
+000094a0: 2e35 3935 3430 3239 2043 2031 322e 3334  .5954029 C 12.34
+000094b0: 3038 3231 2c34 2e33 3630 3233 3938 2031  0821,4.3602398 1
+000094c0: 322e 3935 3035 342c 332e 3139 3239 3637  2.95054,3.192967
+000094d0: 3220 3133 2e36 3734 3534 332c 322e 3130  2 13.674543,2.10
+000094e0: 3639 3030 3220 4320 3134 2e30 3436 3534  69002 C 14.04654
+000094f0: 2c31 2e35 3438 3733 3736 2031 342e 3434  ,1.5487376 14.44
+00009500: 3839 3137 2c31 2e30 3131 3133 3736 2031  8917,1.0111376 1
+00009510: 342e 3837 3436 3634 2c30 2e34 3933 3036  4.874664,0.49306
+00009520: 3531 2043 2031 352e 3638 3234 3935 2c30  51 C 15.682495,0
+00009530: 2e33 3333 3631 3731 2031 362e 3439 3033  .3336171 16.4903
+00009540: 3235 2c30 2e31 3734 3136 3920 3137 2e32  25,0.174169 17.2
+00009550: 3938 3135 362c 302e 3031 3437 3231 3030  98156,0.01472100
+00009560: 3320 4320 3137 2e38 3831 3130 372c 302e  3 C 17.881107,0.
+00009570: 3830 3238 3632 3920 3138 2e33 3436 3437  8028629 18.34647
+00009580: 322c 312e 3637 3833 3335 3720 3138 2e36  2,1.6783357 18.6
+00009590: 3730 3933 2c32 2e36 3034 3032 3734 2043  7093,2.6040274 C
+000095a0: 2031 392e 3032 3735 342c 332e 3631 3633   19.02754,3.6163
+000095b0: 3635 3520 3139 2e32 3136 3233 382c 342e  655 19.216238,4.
+000095c0: 3638 3431 3135 3620 3139 2e32 3636 3336  6841156 19.26636
+000095d0: 392c 352e 3735 3532 3838 3820 4320 3139  9,5.7552888 C 19
+000095e0: 2e32 3830 3034 2c36 2e30 3232 3135 3231  .28004,6.0221521
+000095f0: 2031 392e 3238 3134 3434 2c36 2e32 3839   19.281444,6.289
+00009600: 3337 3733 2031 392e 3238 3130 3132 2c36  3773 19.281012,6
+00009610: 2e35 3536 3532 3339 2043 2031 392e 3238  .5565239 C 19.28
+00009620: 3130 3239 2c31 312e 3632 3730 3831 2031  1029,11.627081 1
+00009630: 392e 3238 3039 3739 2c31 362e 3639 3736  9.280979,16.6976
+00009640: 3339 2031 392e 3238 3130 3338 2c32 312e  39 19.281038,21.
+00009650: 3736 3831 3937 2043 2031 392e 3238 3233  768197 C 19.2823
+00009660: 3737 2c32 322e 3438 3537 3438 2031 392e  77,22.485748 19.
+00009670: 3239 3236 3939 2c32 332e 3230 3336 3339  292699,23.203639
+00009680: 2031 392e 3333 3430 3333 2c32 332e 3932   19.334033,23.92
+00009690: 3031 3235 2043 2031 392e 3335 3432 3937  0125 C 19.354297
+000096a0: 2c32 342e 3234 3936 3333 2031 392e 3337  ,24.249633 19.37
+000096b0: 3838 3331 2c32 342e 3537 3934 3238 2031  8831,24.579428 1
+000096c0: 392e 3432 3838 3236 2c32 342e 3930 3539  9.428826,24.9059
+000096d0: 3433 2043 2031 392e 3434 3434 3931 2c32  43 C 19.444491,2
+000096e0: 352e 3031 3230 3535 2031 392e 3437 3232  5.012055 19.4722
+000096f0: 3738 2c32 352e 3131 3539 3134 2031 392e  78,25.115914 19.
+00009700: 3530 3039 3437 2c32 352e 3231 3931 3220  500947,25.21912 
+00009710: 4320 3139 2e35 3939 3838 342c 3235 2e35  C 19.599884,25.5
+00009720: 3636 3932 3620 3139 2e37 3537 3631 352c  66926 19.757615,
+00009730: 3235 2e38 3938 3431 3820 3139 2e39 3730  25.898418 19.970
+00009740: 3532 2c32 362e 3139 3037 3631 2043 2032  52,26.190761 C 2
+00009750: 302e 3035 3333 3831 2c32 362e 3330 3430  0.053381,26.3040
+00009760: 3032 2032 302e 3134 3230 3639 2c32 362e  02 20.142069,26.
+00009770: 3431 3333 3931 2032 302e 3234 3034 3237  413391 20.240427
+00009780: 2c32 362e 3531 3335 3332 2043 2032 302e  ,26.513532 C 20.
+00009790: 3533 3737 3331 2c32 362e 3831 3337 3338  537731,26.813738
+000097a0: 2032 302e 3930 3637 3931 2c32 372e 3033   20.906791,27.03
+000097b0: 3531 3939 2032 312e 3239 3735 3333 2c32  5199 21.297533,2
+000097c0: 372e 3139 3036 3520 4320 3231 2e37 3833  7.19065 C 21.783
+000097d0: 3732 372c 3237 2e33 3833 3939 3720 3232  727,27.383997 22
+000097e0: 2e33 3032 3132 312c 3237 2e34 3833 3638  .302121,27.48368
+000097f0: 3220 3232 2e38 3231 3234 362c 3237 2e35  2 22.821246,27.5
+00009800: 3334 3236 3220 4320 3233 2e31 3436 3032  34262 C 23.14602
+00009810: 322c 3237 2e35 3636 3030 3920 3233 2e34  2,27.566009 23.4
+00009820: 3732 3437 352c 3237 2e35 3736 3030 3820  72475,27.576008 
+00009830: 3233 2e37 3938 3637 322c 3237 2e35 3734  23.798672,27.574
+00009840: 3730 3420 4320 3234 2e32 3731 3536 312c  704 C 24.271561,
+00009850: 3237 2e35 3734 3730 3420 3234 2e37 3434  27.574704 24.744
+00009860: 3435 322c 3237 2e35 3734 3730 3420 3235  452,27.574704 25
+00009870: 2e32 3137 3334 322c 3237 2e35 3734 3730  .217342,27.57470
+00009880: 3420 4320 3235 2e32 3137 3334 322c 3236  4 C 25.217342,26
+00009890: 2e37 3532 3933 3320 3235 2e32 3137 3334  .752933 25.21734
+000098a0: 322c 3235 2e39 3331 3136 3320 3235 2e32  2,25.931163 25.2
+000098b0: 3137 3334 322c 3235 2e31 3039 3339 3220  17342,25.109392 
+000098c0: 4320 3236 2e35 3134 3736 372c 3236 2e32  C 26.514767,26.2
+000098d0: 3832 3736 3620 3237 2e38 3132 3139 322c  82766 27.812192,
+000098e0: 3237 2e34 3536 3134 2032 392e 3130 3936  27.45614 29.1096
+000098f0: 3137 2c32 382e 3632 3935 3134 2043 2032  17,28.629514 C 2
+00009900: 372e 3831 3231 3932 2c32 392e 3735 3739  7.812192,29.7579
+00009910: 3136 2032 362e 3531 3437 3637 2c33 302e  16 26.514767,30.
+00009920: 3838 3633 3137 2032 352e 3231 3733 3432  886317 25.217342
+00009930: 2c33 322e 3031 3437 3139 2043 2032 352e  ,32.014719 C 25.
+00009940: 3231 3733 3432 2c33 312e 3231 3734 3739  217342,31.217479
+00009950: 2032 352e 3231 3733 3432 2c33 302e 3432   25.217342,30.42
+00009960: 3032 3339 2032 352e 3231 3733 3432 2c32  0239 25.217342,2
+00009970: 392e 3632 3239 3938 2043 2032 342e 3434  9.622998 C 24.44
+00009980: 3938 3339 2c32 392e 3632 3239 3331 2032  9839,29.622931 2
+00009990: 332e 3638 3233 3334 2c32 392e 3632 3331  3.682334,29.6231
+000099a0: 3334 2032 322e 3931 3438 332c 3239 2e36  34 22.91483,29.6
+000099b0: 3232 3839 3520 4320 3232 2e31 3735 3234  22895 C 22.17524
+000099c0: 372c 3239 2e36 3139 3238 3220 3231 2e34  7,29.619282 21.4
+000099d0: 3331 3838 392c 3239 2e35 3531 3335 2032  31889,29.55135 2
+000099e0: 302e 3731 3435 3534 2c32 392e 3336 3437  0.714554,29.3647
+000099f0: 3238 2043 2032 302e 3132 3437 3934 2c32  28 C 20.124794,2
+00009a00: 392e 3231 3130 3833 2031 392e 3535 3234  9.211083 19.5524
+00009a10: 3332 2c32 382e 3937 3230 3933 2031 392e  32,28.972093 19.
+00009a20: 3035 3139 3037 2c32 382e 3632 3036 3736  051907,28.620676
+00009a30: 2043 2031 382e 3638 3735 3531 2c32 382e   C 18.687551,28.
+00009a40: 3336 3632 3537 2031 382e 3336 3535 3433  366257 18.365543
+00009a50: 2c32 382e 3035 3137 3336 2031 382e 3130  ,28.051736 18.10
+00009a60: 3039 3839 2c32 372e 3639 3433 3834 2043  0989,27.694384 C
+00009a70: 2031 372e 3732 3533 3138 2c32 372e 3138   17.725318,27.18
+00009a80: 3934 3636 2031 372e 3436 3031 352c 3236  9466 17.46015,26
+00009a90: 2e36 3039 3435 2031 372e 3237 3237 3134  .60945 17.272714
+00009aa0: 2c32 362e 3031 3033 3438 2043 2031 372e  ,26.010348 C 17.
+00009ab0: 3034 3338 3236 2c32 352e 3237 3632 3636  043826,25.276266
+00009ac0: 2031 362e 3932 3534 3238 2c32 342e 3531   16.925428,24.51
+00009ad0: 3138 2031 362e 3836 3631 3835 2c32 332e  18 16.866185,23.
+00009ae0: 3734 3633 3634 2043 2031 362e 3833 3132  746364 C 16.8312
+00009af0: 3131 2c32 332e 3239 3534 3134 2031 362e  11,23.295414 16.
+00009b00: 3831 3934 3739 2c32 322e 3834 3320 3136  819479,22.843 16
+00009b10: 2e38 3230 3830 312c 3232 2e33 3930 3738  .820801,22.39078
+00009b20: 3520 4320 3136 2e38 3230 3739 2c31 372e  5 C 16.82079,17.
+00009b30: 3437 3335 3033 2031 362e 3832 3038 3233  473503 16.820823
+00009b40: 2c31 322e 3535 3632 3231 2031 362e 3832  ,12.556221 16.82
+00009b50: 3037 3835 2c37 2e36 3338 3933 3832 2043  0785,7.6389382 C
+00009b60: 2031 362e 3831 3839 3936 2c36 2e37 3632   16.818996,6.762
+00009b70: 3231 3932 2031 362e 3737 3735 3933 2c35  2192 16.777593,5
+00009b80: 2e38 3833 3635 3932 2031 362e 3635 3039  .8836592 16.6509
+00009b90: 3737 2c35 2e30 3135 3435 3233 2043 2031  77,5.0154523 C 1
+00009ba0: 362e 3535 3934 372c 342e 3339 3833 3331  6.55947,4.398331
+00009bb0: 3920 3136 2e34 3235 3434 342c 332e 3738  9 16.425444,3.78
+00009bc0: 3434 3132 3720 3136 2e32 3033 3934 332c  44127 16.203943,
+00009bd0: 332e 3230 3031 3033 3120 4320 3136 2e30  3.2001031 C 16.0
+00009be0: 3831 3939 362c 322e 3838 3032 3230 3820  81996,2.8802208 
+00009bf0: 3135 2e39 3332 3633 322c 322e 3536 3936  15.932632,2.5696
+00009c00: 3230 3920 3135 2e37 3433 3639 342c 322e  209 15.743694,2.
+00009c10: 3238 3337 3839 3420 4320 3134 2e38 3135  2837894 C 14.815
+00009c20: 3331 352c 332e 3335 3534 3935 2031 342e  315,3.355495 14.
+00009c30: 3033 3835 3839 2c34 2e35 3536 3331 3138  038589,4.5563118
+00009c40: 2031 332e 3432 3038 3936 2c35 2e38 3332   13.420896,5.832
+00009c50: 3634 3639 2043 2031 322e 3734 3132 3339  6469 C 12.741239
+00009c60: 2c37 2e32 3334 3834 3738 2031 322e 3235  ,7.2348478 12.25
+00009c70: 3032 3234 2c38 2e37 3234 3636 3320 3131  0224,8.724663 11
+00009c80: 2e39 3132 3631 392c 3130 2e32 3434 3938  .912619,10.24498
+00009c90: 3820 4320 3131 2e39 3132 3631 392c 3135  8 C 11.912619,15
+00009ca0: 2e31 3939 3739 2031 312e 3931 3236 3139  .19979 11.912619
+00009cb0: 2c32 302e 3135 3435 3920 3131 2e39 3132  ,20.15459 11.912
+00009cc0: 3631 392c 3235 2e31 3039 3339 3220 4320  619,25.109392 C 
+00009cd0: 3131 2e30 3932 3534 392c 3235 2e31 3039  11.092549,25.109
+00009ce0: 3339 3220 3130 2e32 3732 3437 382c 3235  392 10.272478,25
+00009cf0: 2e31 3039 3339 3220 392e 3435 3234 3038  .109392 9.452408
+00009d00: 332c 3235 2e31 3039 3339 3220 4320 392e  3,25.109392 C 9.
+00009d10: 3435 3233 3937 332c 3139 2e35 3734 3331  4523973,19.57431
+00009d20: 3920 392e 3435 3234 3330 332c 3134 2e30  9 9.4524303,14.0
+00009d30: 3339 3234 3620 392e 3435 3233 3932 332c  39246 9.4523923,
+00009d40: 382e 3530 3431 3733 3320 4320 392e 3435  8.5041733 C 9.45
+00009d50: 3036 3134 332c 372e 3530 3434 3038 3220  06143,7.5044082 
+00009d60: 392e 3431 3330 3134 332c 362e 3530 3332  9.4130143,6.5032
+00009d70: 3131 3820 392e 3239 3536 3639 332c 352e  118 9.2956693,5.
+00009d80: 3530 3938 3239 3620 4320 392e 3231 3437  5098296 C 9.2147
+00009d90: 3532 332c 342e 3833 3832 3237 2039 2e30  523,4.838227 9.0
+00009da0: 3938 3630 3433 2c34 2e31 3638 3536 3835  986043,4.1685685
+00009db0: 2038 2e39 3033 3738 3833 2c33 2e35 3139   8.9037883,3.519
+00009dc0: 3938 3136 2043 2038 2e37 3733 3433 3233  9816 C 8.7734323
+00009dd0: 2c33 2e30 3930 3530 3833 2038 2e36 3038  ,3.0905083 8.608
+00009de0: 3033 3733 2c32 2e36 3638 3633 3720 382e  0373,2.668637 8.
+00009df0: 3337 3533 3031 332c 322e 3238 3337 3839  3753013,2.283789
+00009e00: 3420 4320 372e 3433 3335 3434 332c 332e  4 C 7.4335443,3.
+00009e10: 3334 3433 3739 2036 2e36 3434 3034 3033  344379 6.6440403
+00009e20: 2c34 2e35 3336 3932 3931 2036 2e30 3036  ,4.5369291 6.006
+00009e30: 3438 3033 2c35 2e38 3033 3639 3336 2043  4803,5.8036936 C
+00009e40: 2035 2e33 3831 3534 3833 2c37 2e30 3434   5.3815483,7.044
+00009e50: 3134 3036 2034 2e38 3938 3730 3533 2c38  1406 4.8987053,8
+00009e60: 2e33 3533 3839 3120 342e 3533 3139 3836  .353891 4.531986
+00009e70: 332c 392e 3639 3330 3532 3320 4320 342e  3,9.6930523 C 4.
+00009e80: 3533 3139 3836 332c 3134 2e38 3331 3833  5319863,14.83183
+00009e90: 3320 342e 3533 3139 3836 332c 3139 2e39  3 4.5319863,19.9
+00009ea0: 3730 3631 3220 342e 3533 3139 3836 332c  70612 4.5319863,
+00009eb0: 3235 2e31 3039 3339 3220 4320 332e 3731  25.109392 C 3.71
+00009ec0: 3139 3135 332c 3235 2e31 3039 3339 3220  19153,25.109392 
+00009ed0: 322e 3839 3138 3435 342c 3235 2e31 3039  2.8918454,25.109
+00009ee0: 3339 3220 322e 3037 3137 3735 2c32 352e  392 2.071775,25.
+00009ef0: 3130 3933 3932 207a 2720 7374 796c 653d  109392 z' style=
+00009f00: 2766 696c 6c3a 2024 7a6f 6469 6163 5f63  'fill: $zodiac_c
+00009f10: 6f6c 6f72 5f37 3b27 202f 3e0d 0a20 2020  olor_7;' />..   
+00009f20: 2020 2020 2020 2020 2020 2020 203c 2f73               </s
+00009f30: 796d 626f 6c3e 0d0a 2020 2020 2020 2020  ymbol>..        
+00009f40: 2020 2020 2020 2020 3c73 796d 626f 6c20          <symbol 
+00009f50: 6964 3d27 7361 6769 7474 6172 6975 7327  id='sagittarius'
+00009f60: 3e0d 0a20 2020 2020 2020 2020 2020 2020  >..             
+00009f70: 2020 2020 2020 203c 7061 7468 2074 7261         <path tra
+00009f80: 6e73 666f 726d 3d22 7363 616c 6528 302e  nsform="scale(0.
+00009f90: 3829 2220 643d 274d 2032 392e 3839 3239  8)" d='M 29.8929
+00009fa0: 3432 2c32 2e30 3935 3837 3036 204c 2033  42,2.0958706 L 3
+00009fb0: 322c 3137 2e31 3136 3237 3620 4c20 3238  2,17.116276 L 28
+00009fc0: 2e39 3938 3537 392c 3137 2e35 3837 3038  .998579,17.58708
+00009fd0: 3820 4c20 3237 2e34 3532 3339 332c 362e  8 L 27.452393,6.
+00009fe0: 3633 3639 3233 3520 4c20 3133 2e37 3333  6369235 L 13.733
+00009ff0: 3737 362c 3230 2e34 3131 3935 3720 4c20  776,20.411957 L 
+0000a000: 3230 2e31 3931 3337 392c 3236 2e38 3636  20.191379,26.866
+0000a010: 3633 204c 2031 382e 3033 3838 3435 2c32  63 L 18.038845,2
+0000a020: 392e 3032 3332 3531 204c 2031 312e 3538  9.023251 L 11.58
+0000a030: 3132 3432 2c32 322e 3535 3333 3920 4c20  1242,22.55339 L 
+0000a040: 322e 3039 3139 3031 2c33 312e 3939 3939  2.091901,31.9999
+0000a050: 3935 204c 2031 2e35 652d 3036 2c32 392e  95 L 1.5e-06,29.
+0000a060: 3930 3431 3234 204c 2039 2e34 3734 3138  904124 L 9.47418
+0000a070: 342c 3230 2e34 3432 3333 3220 4c20 332e  4,20.442332 L 3.
+0000a080: 3033 3137 342c 3133 2e39 3732 3437 204c  03174,13.97247 L
+0000a090: 2035 2e31 3533 3935 372c 3131 2e38 3135   5.153957,11.815
+0000a0a0: 3835 204c 2031 312e 3631 3135 362c 3138  85 L 11.61156,18
+0000a0b0: 2e32 3835 3731 3120 4c20 3235 2e33 3630  .285711 L 25.360
+0000a0c0: 3439 332c 342e 3534 3130 3532 3920 4c20  493,4.5410529 L 
+0000a0d0: 3134 2e34 3331 3037 362c 332e 3030 3731  14.431076,3.0071
+0000a0e0: 3138 3620 4c20 3134 2e39 3030 3939 362c  186 L 14.900996,
+0000a0f0: 2d34 2e34 3430 3839 3231 652d 3136 204c  -4.4408921e-16 L
+0000a100: 2032 392e 3839 3239 3432 2c32 2e30 3935   29.892942,2.095
+0000a110: 3837 3036 207a 2027 2073 7479 6c65 3d27  8706 z ' style='
+0000a120: 6669 6c6c 3a20 247a 6f64 6961 635f 636f  fill: $zodiac_co
+0000a130: 6c6f 725f 383b 2720 2f3e 0d0a 2020 2020  lor_8;' />..    
+0000a140: 2020 2020 2020 2020 2020 2020 3c2f 7379              </sy
+0000a150: 6d62 6f6c 3e0d 0a20 2020 2020 2020 2020  mbol>..         
+0000a160: 2020 2020 2020 203c 7379 6d62 6f6c 2069         <symbol i
+0000a170: 643d 2763 6170 7269 636f 726e 273e 0d0a  d='capricorn'>..
+0000a180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a190: 2020 2020 3c70 6174 6820 7472 616e 7366      <path transf
+0000a1a0: 6f72 6d3d 2273 6361 6c65 2830 2e38 2922  orm="scale(0.8)"
+0000a1b0: 2064 3d27 4d20 362e 3130 3933 3535 392c   d='M 6.1093559,
+0000a1c0: 3138 2e39 3034 3737 3420 4320 362e 3130  18.904774 C 6.10
+0000a1d0: 3932 3339 322c 3138 2e35 3839 3535 2036  92392,18.58955 6
+0000a1e0: 2e31 3039 3630 3432 2c31 382e 3237 3433  .1096042,18.2743
+0000a1f0: 3235 2036 2e31 3039 3134 3733 2c31 372e  25 6.1091473,17.
+0000a200: 3935 3931 3033 2043 2036 2e31 3033 3633  959103 C 6.10363
+0000a210: 3839 2c31 372e 3134 3632 3334 2036 2e30  89,17.146234 6.0
+0000a220: 3336 3435 3837 2c31 362e 3333 3530 3635  364587,16.335065
+0000a230: 2035 2e39 3436 3339 3638 2c31 352e 3532   5.9463968,15.52
+0000a240: 3736 3131 2043 2035 2e38 3032 3031 3933  7611 C 5.8020193
+0000a250: 2c31 342e 3235 3436 3432 2035 2e35 3936  ,14.254642 5.596
+0000a260: 3039 3433 2c31 322e 3938 3934 3635 2035  0943,12.989465 5
+0000a270: 2e33 3636 3533 3133 2c31 312e 3732 3933  .3665313,11.7293
+0000a280: 3338 2043 2035 2e32 3235 3836 3034 2c31  38 C 5.2258604,1
+0000a290: 302e 3935 3639 3237 2035 2e30 3730 3434  0.956927 5.07044
+0000a2a0: 2c31 302e 3138 3732 3220 342e 3930 3335  ,10.18722 4.9035
+0000a2b0: 3537 2c39 2e34 3230 3035 3437 2043 2034  57,9.4200547 C 4
+0000a2c0: 2e37 3231 3830 3237 2c38 2e35 3933 3130  .7218027,8.59310
+0000a2d0: 3532 2034 2e35 3236 3233 3839 2c37 2e37  52 4.5262389,7.7
+0000a2e0: 3638 3439 3037 2034 2e32 3835 3333 3336  684907 4.2853336
+0000a2f0: 2c36 2e39 3536 3532 3437 2043 2034 2e31  ,6.9565247 C 4.1
+0000a300: 3533 3230 3336 2c36 2e35 3136 3935 3534  532036,6.5169554
+0000a310: 2034 2e30 3039 3931 3339 2c36 2e30 3739   4.0099139,6.079
+0000a320: 3533 2033 2e38 3235 3133 3334 2c35 2e36  53 3.8251334,5.6
+0000a330: 3538 3838 3536 2043 2033 2e36 3538 3932  588856 C 3.65892
+0000a340: 3334 2c35 2e32 3833 3631 3531 2033 2e34  34,5.2836151 3.4
+0000a350: 3437 3231 3638 2c34 2e39 3236 3935 3239  472168,4.9269529
+0000a360: 2033 2e31 3834 3334 3939 2c34 2e36 3131   3.1843499,4.611
+0000a370: 3038 3838 2043 2032 2e39 3030 3932 3039  0888 C 2.9009209
+0000a380: 2c34 2e32 3730 3039 3239 2032 2e35 3531  ,4.2700929 2.551
+0000a390: 3435 3238 2c33 2e39 3832 3030 3131 2032  4528,3.9820011 2
+0000a3a0: 2e31 3534 3638 3531 2c33 2e37 3832 3336  .1546851,3.78236
+0000a3b0: 3431 2043 2031 2e37 3237 3238 3436 2c33  41 C 1.7272846,3
+0000a3c0: 2e35 3635 3232 3631 2031 2e32 3531 3938  .5652261 1.25198
+0000a3d0: 3437 2c33 2e34 3532 3537 3137 2030 2e37  47,3.4525717 0.7
+0000a3e0: 3734 3938 3437 382c 332e 3432 3230 3438  7498478,3.422048
+0000a3f0: 3620 4320 302e 3538 3730 3136 3737 2c33  6 C 0.58701677,3
+0000a400: 2e34 3038 3937 3036 2030 2e33 3938 3539  .4089706 0.39859
+0000a410: 3637 352c 332e 3431 3239 3732 3820 302e  675,3.4129728 0.
+0000a420: 3231 3033 3431 392c 332e 3431 3232 3935  2103419,3.412295
+0000a430: 2043 2030 2e31 3430 3230 3339 312c 332e   C 0.14020391,3.
+0000a440: 3431 3232 3935 2030 2e30 3730 3036 3436  412295 0.0700646
+0000a450: 3833 2c33 2e34 3132 3239 3520 2d37 2e33  83,3.412295 -7.3
+0000a460: 3330 3237 3765 2d30 352c 332e 3431 3232  30277e-05,3.4122
+0000a470: 3935 2043 202d 372e 3333 3032 3737 652d  95 C -7.330277e-
+0000a480: 3035 2c32 2e37 3239 3533 3335 202d 372e  05,2.7295335 -7.
+0000a490: 3333 3032 3737 652d 3035 2c32 2e30 3436  330277e-05,2.046
+0000a4a0: 3737 3220 2d37 2e33 3330 3237 3765 2d30  772 -7.330277e-0
+0000a4b0: 352c 312e 3336 3430 3130 3620 4320 302e  5,1.3640106 C 0.
+0000a4c0: 3632 3736 3334 3534 2c31 2e33 3634 3033  62763454,1.36403
+0000a4d0: 3137 2031 2e32 3535 3334 3234 2c31 2e33  17 1.2553424,1.3
+0000a4e0: 3633 3936 3936 2031 2e38 3833 3035 3032  639696 1.8830502
+0000a4f0: 2c31 2e33 3634 3034 3136 2043 2032 2e34  ,1.3640416 C 2.4
+0000a500: 3439 3434 342c 312e 3336 3538 3531 3520  49444,1.3658515 
+0000a510: 332e 3032 3130 3939 2c31 2e34 3339 3131  3.021099,1.43911
+0000a520: 3536 2033 2e35 3535 3031 312c 312e 3633  56 3.555011,1.63
+0000a530: 3433 3239 3520 4320 332e 3938 3336 3639  43295 C 3.983669
+0000a540: 342c 312e 3739 3031 3037 3120 342e 3338  4,1.7901071 4.38
+0000a550: 3332 3836 392c 322e 3032 3931 3538 2034  32869,2.029158 4
+0000a560: 2e37 3134 3738 382c 322e 3334 3331 3737  .714788,2.343177
+0000a570: 3420 4320 352e 3036 3932 3535 342c 322e  4 C 5.0692554,2.
+0000a580: 3637 3634 3830 3520 352e 3334 3335 3931  6764805 5.343591
+0000a590: 312c 332e 3038 3834 3836 3120 352e 3534  1,3.0884861 5.54
+0000a5a0: 3432 3334 392c 332e 3533 3031 3633 3220  42349,3.5301632 
+0000a5b0: 4320 352e 3834 3731 3630 382c 342e 3138  C 5.8471608,4.18
+0000a5c0: 3435 3437 3920 362e 3038 3633 3437 342c  45479 6.0863474,
+0000a5d0: 342e 3836 3634 3233 2036 2e32 3939 3537  4.866423 6.29957
+0000a5e0: 3634 2c35 2e35 3534 3632 3035 2043 2036  64,5.5546205 C 6
+0000a5f0: 2e36 3331 3632 3134 2c36 2e36 3335 3035  .6316214,6.63505
+0000a600: 3720 362e 3839 3630 3035 372c 372e 3733  7 6.8960057,7.73
+0000a610: 3530 3636 3420 372e 3133 3138 3332 322c  50664 7.1318322,
+0000a620: 382e 3834 3030 3838 3620 4320 372e 3332  8.8400886 C 7.32
+0000a630: 3737 3433 372c 392e 3736 3231 3930 3220  77437,9.7621902 
+0000a640: 372e 3530 3135 3335 392c 3130 2e36 3838  7.5015359,10.688
+0000a650: 3838 3320 372e 3636 3135 3438 332c 3131  883 7.6615483,11
+0000a660: 2e36 3137 3834 3720 4320 382e 3038 3137  .617847 C 8.0817
+0000a670: 3833 392c 392e 3734 3030 3139 3120 382e  839,9.7400191 8.
+0000a680: 3635 3231 3732 332c 372e 3839 3130 3831  6521723,7.891081
+0000a690: 3220 392e 3433 3635 3035 312c 362e 3133  2 9.4365051,6.13
+0000a6a0: 3139 3739 3720 4320 3130 2e31 3232 3636  19797 C 10.12266
+0000a6b0: 352c 342e 3539 3238 3133 3220 3130 2e39  5,4.5928132 10.9
+0000a6c0: 3736 3733 372c 332e 3132 3338 3233 3320  76737,3.1238233 
+0000a6d0: 3132 2e30 3233 3337 322c 312e 3830 3038  12.023372,1.8008
+0000a6e0: 3733 3620 4320 3132 2e31 3432 3434 322c  736 C 12.142442,
+0000a6f0: 312e 3635 3431 3739 3220 3132 2e32 3538  1.6541792 12.258
+0000a700: 3639 2c31 2e35 3030 3439 3333 2031 322e  69,1.5004933 12.
+0000a710: 3338 3536 3037 2c31 2e33 3632 3937 3238  385607,1.3629728
+0000a720: 2043 2031 332e 3438 3036 3931 2c31 2e31   C 13.480691,1.1
+0000a730: 3532 3238 3338 2031 342e 3537 3537 3737  522838 14.575777
+0000a740: 2c30 2e39 3431 3539 3334 3920 3135 2e36  ,0.94159349 15.6
+0000a750: 3730 3836 312c 302e 3733 3039 3034 3437  70861,0.73090447
+0000a760: 2043 2031 362e 3031 3034 3932 2c31 2e35   C 16.010492,1.5
+0000a770: 3031 3536 3539 2031 362e 3237 3438 3832  015659 16.274882
+0000a780: 2c32 2e33 3033 3135 3839 2031 362e 3530  ,2.3031589 16.50
+0000a790: 3437 3237 2c33 2e31 3132 3633 3937 2043  4727,3.1126397 C
+0000a7a0: 2031 362e 3834 3731 3233 2c34 2e33 3237   16.847123,4.327
+0000a7b0: 3339 3237 2031 372e 3130 3930 3231 2c35  3927 17.109021,5
+0000a7c0: 2e35 3633 3339 3731 2031 372e 3333 3333  .5633971 17.3333
+0000a7d0: 3032 2c36 2e38 3034 3930 3832 2043 2031  02,6.8049082 C 1
+0000a7e0: 372e 3436 3536 3835 2c37 2e35 3339 3231  7.465685,7.53921
+0000a7f0: 3435 2031 372e 3538 3235 3636 2c38 2e32  45 17.582566,8.2
+0000a800: 3736 3233 3036 2031 372e 3639 3035 342c  762306 17.69054,
+0000a810: 392e 3031 3434 3931 3920 4320 3137 2e38  9.0144919 C 17.8
+0000a820: 3431 3031 312c 3130 2e30 3130 3535 3420  41011,10.010554 
+0000a830: 3137 2e39 3931 3438 2c31 312e 3030 3636  17.99148,11.0066
+0000a840: 3135 2031 382e 3134 3139 3531 2c31 322e  15 18.141951,12.
+0000a850: 3030 3236 3736 2043 2031 382e 3233 3632  002676 C 18.2362
+0000a860: 3236 2c31 322e 3638 3139 3832 2031 382e  26,12.681982 18.
+0000a870: 3333 3034 3638 2c31 332e 3336 3133 3439  330468,13.361349
+0000a880: 2031 382e 3431 3330 3531 2c31 342e 3034   18.413051,14.04
+0000a890: 3231 3935 2043 2031 382e 3434 3836 3639  2195 C 18.448669
+0000a8a0: 2c31 342e 3334 3036 3234 2031 382e 3437  ,14.340624 18.47
+0000a8b0: 3930 3639 2c31 342e 3633 3936 3538 2031  9069,14.639658 1
+0000a8c0: 382e 3531 3733 342c 3134 2e39 3337 3737  8.51734,14.93777
+0000a8d0: 3420 4320 3138 2e36 3138 3933 342c 3135  4 C 18.618934,15
+0000a8e0: 2e37 3435 3730 3820 3138 2e37 3431 3936  .745708 18.74196
+0000a8f0: 372c 3136 2e35 3531 3739 3520 3138 2e39  7,16.551795 18.9
+0000a900: 3136 3938 372c 3137 2e33 3437 3338 3120  16987,17.347381 
+0000a910: 4320 3138 2e39 3936 3233 342c 3137 2e37  C 18.996234,17.7
+0000a920: 3034 3532 3220 3139 2e30 3836 3134 312c  04522 19.086141,
+0000a930: 3138 2e30 3539 3631 3320 3139 2e31 3937  18.059613 19.197
+0000a940: 3434 322c 3138 2e34 3038 3232 2043 2031  442,18.40822 C 1
+0000a950: 392e 3635 3435 3634 2c31 372e 3533 3430  9.654564,17.5340
+0000a960: 3134 2032 302e 3230 3330 3731 2c31 362e  14 20.203071,16.
+0000a970: 3730 3132 3735 2032 302e 3838 3037 3036  701275 20.880706
+0000a980: 2c31 352e 3938 3133 3533 2043 2032 312e  ,15.981353 C 21.
+0000a990: 3434 3533 3737 2c31 352e 3338 3037 3731  445377,15.380771
+0000a9a0: 2032 322e 3130 3433 3138 2c31 342e 3836   22.104318,14.86
+0000a9b0: 3335 3037 2032 322e 3834 3233 3136 2c31  3507 22.842316,1
+0000a9c0: 342e 3439 3235 3836 2043 2032 332e 3531  4.492586 C 23.51
+0000a9d0: 3834 3334 2c31 342e 3135 3035 3733 2032  8434,14.150573 2
+0000a9e0: 342e 3235 3730 3535 2c31 332e 3933 3630  4.257055,13.9360
+0000a9f0: 3235 2032 352e 3030 3934 3534 2c31 332e  25 25.009454,13.
+0000aa00: 3835 3033 3034 2043 2032 352e 3536 3639  850304 C 25.5669
+0000aa10: 3839 2c31 332e 3738 3733 3620 3236 2e31  89,13.78736 26.1
+0000aa20: 3332 3231 382c 3133 2e37 3834 3836 3920  32218,13.784869 
+0000aa30: 3236 2e36 3839 3431 2c31 332e 3835 3320  26.68941,13.853 
+0000aa40: 4320 3237 2e33 3730 3631 362c 3133 2e39  C 27.370616,13.9
+0000aa50: 3336 3037 3620 3238 2e30 3338 3837 362c  36076 28.038876,
+0000aa60: 3134 2e31 3333 3120 3238 2e36 3531 3036  14.1331 28.65106
+0000aa70: 312c 3134 2e34 3434 3136 3920 4320 3239  1,14.444169 C 29
+0000aa80: 2e32 3334 3138 372c 3134 2e37 3338 3731  .234187,14.73871
+0000aa90: 3320 3239 2e37 3633 3830 352c 3135 2e31  3 29.763805,15.1
+0000aaa0: 3333 3738 3520 3330 2e32 3237 3530 312c  33785 30.227501,
+0000aab0: 3135 2e35 3932 3834 3720 4320 3330 2e37  15.592847 C 30.7
+0000aac0: 3137 3133 2c31 362e 3037 3135 3137 2033  1713,16.071517 3
+0000aad0: 312e 3133 3338 3035 2c31 362e 3632 3832  1.133805,16.6282
+0000aae0: 3132 2033 312e 3433 3139 342c 3137 2e32  12 31.43194,17.2
+0000aaf0: 3435 3636 3220 4320 3331 2e37 3233 3539  45662 C 31.72359
+0000ab00: 2c31 372e 3834 3536 3833 2033 312e 3930  ,17.845683 31.90
+0000ab10: 3030 3738 2c31 382e 3439 3932 3332 2033  0078,18.499232 3
+0000ab20: 312e 3936 3634 3639 2c31 392e 3136 3233  1.966469,19.1623
+0000ab30: 3938 2043 2033 322e 3031 3536 3132 2c31  98 C 32.015612,1
+0000ab40: 392e 3635 3138 3631 2033 322e 3030 3933  9.651861 32.0093
+0000ab50: 3235 2c32 302e 3134 3633 3538 2033 312e  25,20.146358 31.
+0000ab60: 3935 3736 3034 2c32 302e 3633 3533 3336  957604,20.635336
+0000ab70: 2043 2033 312e 3837 3934 322c 3231 2e33   C 31.87942,21.3
+0000ab80: 3636 3138 3720 3331 2e36 3831 3834 382c  66187 31.681848,
+0000ab90: 3232 2e30 3835 3834 3920 3331 2e33 3539  22.085849 31.359
+0000aba0: 3030 372c 3232 2e37 3436 3938 3820 4320  007,22.746988 C 
+0000abb0: 3331 2e30 3335 3434 322c 3233 2e34 3133  31.035442,23.413
+0000abc0: 3539 3620 3330 2e35 3837 3136 352c 3234  596 30.587165,24
+0000abd0: 2e30 3136 3731 3820 3330 2e30 3537 3635  .016718 30.05765
+0000abe0: 2c32 342e 3533 3339 3937 2043 2032 392e  ,24.533997 C 29.
+0000abf0: 3535 3633 3834 2c32 352e 3032 3538 3933  556384,25.025893
+0000ac00: 2032 382e 3937 3639 3137 2c32 352e 3434   28.976917,25.44
+0000ac10: 3135 3231 2032 382e 3333 3739 3833 2c32  1521 28.337983,2
+0000ac20: 352e 3733 3535 3535 2043 2032 372e 3732  5.735555 C 27.72
+0000ac30: 3034 3331 2c32 362e 3032 3136 3639 2032  0431,26.021669 2
+0000ac40: 372e 3035 3133 3238 2c32 362e 3139 3133  7.051328,26.1913
+0000ac50: 3232 2032 362e 3337 3339 382c 3236 2e32  22 26.37398,26.2
+0000ac60: 3531 3237 3120 4320 3235 2e39 3033 3534  51271 C 25.90354
+0000ac70: 392c 3236 2e32 3933 3334 3920 3235 2e34  9,26.293349 25.4
+0000ac80: 3239 3530 392c 3236 2e32 3834 3235 3920  29509,26.284259 
+0000ac90: 3234 2e39 3539 3335 312c 3236 2e32 3433  24.959351,26.243
+0000aca0: 3233 3320 4320 3234 2e31 3032 3436 342c  233 C 24.102464,
+0000acb0: 3236 2e31 3636 3832 3820 3233 2e32 3537  26.166828 23.257
+0000acc0: 3134 352c 3235 2e39 3535 3232 3720 3232  145,25.955227 22
+0000acd0: 2e34 3638 3435 312c 3235 2e36 3130 3939  .468451,25.61099
+0000ace0: 3120 4320 3231 2e36 3130 3633 322c 3235  1 C 21.610632,25
+0000acf0: 2e32 3338 3632 3120 3230 2e38 3233 3530  .238621 20.82350
+0000ad00: 312c 3234 2e37 3133 3534 3720 3230 2e31  1,24.713547 20.1
+0000ad10: 3236 3036 352c 3234 2e30 3932 3630 3320  26065,24.092603 
+0000ad20: 4320 3139 2e39 3231 3034 342c 3233 2e39  C 19.921044,23.9
+0000ad30: 3130 3336 3920 3139 2e37 3233 3333 362c  10369 19.723336,
+0000ad40: 3233 2e37 3139 3935 3120 3139 2e35 3332  23.719951 19.532
+0000ad50: 3731 362c 3233 2e35 3232 3732 3420 4320  716,23.522724 C 
+0000ad60: 3139 2e31 3131 3834 392c 3234 2e36 3235  19.111849,24.625
+0000ad70: 3639 3220 3138 2e36 3635 3233 372c 3235  692 18.665237,25
+0000ad80: 2e37 3139 3834 3420 3138 2e31 3537 3134  .719844 18.15714
+0000ad90: 2c32 362e 3738 3538 3520 4320 3137 2e38  ,26.78585 C 17.8
+0000ada0: 3430 3431 2c32 372e 3434 3634 3836 2031  4041,27.446486 1
+0000adb0: 372e 3530 3134 3638 2c32 382e 3039 3830  7.501468,28.0980
+0000adc0: 3735 2031 372e 3130 3638 3131 2c32 382e  75 17.106811,28.
+0000add0: 3731 3539 3838 2043 2031 362e 3836 3532  715988 C 16.8652
+0000ade0: 3837 2c32 392e 3039 3038 3735 2031 362e  87,29.090875 16.
+0000adf0: 3630 3339 3834 2c32 392e 3435 3538 3433  603984,29.455843
+0000ae00: 2031 362e 3239 3431 3637 2c32 392e 3737   16.294167,29.77
+0000ae10: 3738 3633 2043 2031 352e 3934 3836 3435  7863 C 15.948645
+0000ae20: 2c33 302e 3133 3735 3332 2031 352e 3532  ,30.137532 15.52
+0000ae30: 3630 3936 2c33 302e 3431 3732 3820 3135  6096,30.41728 15
+0000ae40: 2e30 3734 3132 342c 3330 2e36 3235 3035  .074124,30.62505
+0000ae50: 3320 4320 3134 2e35 3030 3039 312c 3330  3 C 14.500091,30
+0000ae60: 2e38 3839 3039 3520 3133 2e38 3832 3030  .889095 13.88200
+0000ae70: 312c 3331 2e30 3435 3336 2031 332e 3235  1,31.04536 13.25
+0000ae80: 3931 3032 2c33 312e 3134 3130 3433 2043  9102,31.141043 C
+0000ae90: 2031 322e 3631 3833 3234 2c33 312e 3233   12.618324,31.23
+0000aea0: 3838 3320 3131 2e39 3639 3235 352c 3331  883 11.969255,31
+0000aeb0: 2e32 3731 3436 3620 3131 2e33 3231 3536  .271466 11.32156
+0000aec0: 362c 3331 2e32 3638 3936 3320 4320 3130  6,31.268963 C 10
+0000aed0: 2e35 3938 3236 312c 3331 2e32 3638 3936  .598261,31.26896
+0000aee0: 3320 392e 3837 3439 3537 322c 3331 2e32  3 9.8749572,31.2
+0000aef0: 3638 3936 3320 392e 3135 3136 3532 392c  68963 9.1516529,
+0000af00: 3331 2e32 3638 3936 3320 4320 392e 3135  31.268963 C 9.15
+0000af10: 3136 3532 392c 3330 2e35 3737 3932 3520  16529,30.577925 
+0000af20: 392e 3135 3136 3532 392c 3239 2e38 3836  9.1516529,29.886
+0000af30: 3838 3920 392e 3135 3136 3532 392c 3239  889 9.1516529,29
+0000af40: 2e31 3935 3835 3120 4320 392e 3532 3834  .195851 C 9.5284
+0000af50: 3139 372c 3239 2e31 3935 3734 3620 392e  197,29.195746 9.
+0000af60: 3930 3531 3837 372c 3239 2e31 3936 3037  9051877,29.19607
+0000af70: 2031 302e 3238 3139 3534 2c32 392e 3139   10.281954,29.19
+0000af80: 3536 3732 2043 2031 302e 3938 3030 3735  5672 C 10.980075
+0000af90: 2c32 392e 3139 3135 3120 3131 2e36 3830  ,29.19151 11.680
+0000afa0: 3734 362c 3239 2e31 3434 3131 3620 3132  746,29.144116 12
+0000afb0: 2e33 3635 3839 362c 3239 2e30 3034 3833  .365896,29.00483
+0000afc0: 3520 4320 3132 2e38 3739 3231 322c 3238  5 C 12.879212,28
+0000afd0: 2e38 3939 3138 3520 3133 2e33 3836 3431  .899185 13.38641
+0000afe0: 352c 3238 2e37 3430 3535 2031 332e 3834  5,28.74055 13.84
+0000aff0: 3631 3737 2c32 382e 3438 3533 3932 2043  6177,28.485392 C
+0000b000: 2031 342e 3138 3033 3836 2c32 382e 3330   14.180386,28.30
+0000b010: 3030 3937 2031 342e 3438 3634 3734 2c32  0097 14.486474,2
+0000b020: 382e 3035 3934 3520 3134 2e37 3238 3638  8.05945 14.72868
+0000b030: 2c32 372e 3736 3236 3937 2043 2031 342e  ,27.762697 C 14.
+0000b040: 3936 3835 3239 2c32 372e 3437 3031 3720  968529,27.47017 
+0000b050: 3135 2e31 3636 3836 2c32 372e 3134 3633  15.16686,27.1463
+0000b060: 3837 2031 352e 3335 3232 3038 2c32 362e  87 15.352208,26.
+0000b070: 3831 3734 3438 2043 2031 352e 3638 3436  817448 C 15.6846
+0000b080: 3835 2c32 362e 3232 3037 3238 2031 352e  85,26.220728 15.
+0000b090: 3936 3933 3631 2c32 352e 3539 3837 3937  969361,25.598797
+0000b0a0: 2031 362e 3233 3739 3038 2c32 342e 3937   16.237908,24.97
+0000b0b0: 3131 3639 2043 2031 362e 3639 3936 3239  1169 C 16.699629
+0000b0c0: 2c32 332e 3838 3437 3238 2031 372e 3130  ,23.884728 17.10
+0000b0d0: 3735 3133 2c32 322e 3737 3632 3734 2031  7513,22.776274 1
+0000b0e0: 372e 3439 3439 3635 2c32 312e 3636 3134  7.494965,21.6614
+0000b0f0: 3831 2043 2031 372e 3535 3831 312c 3231  81 C 17.55811,21
+0000b100: 2e34 3739 3335 3220 3137 2e36 3230 362c  .479352 17.6206,
+0000b110: 3231 2e32 3936 3939 3520 3137 2e36 3832  21.296995 17.682
+0000b120: 3530 322c 3231 2e31 3134 3433 3820 4320  502,21.114438 C 
+0000b130: 3137 2e33 3832 3230 362c 3230 2e35 3835  17.382206,20.585
+0000b140: 3939 3420 3137 2e31 3030 3433 352c 3230  994 17.100435,20
+0000b150: 2e30 3435 3733 3520 3136 2e38 3637 3435  .045735 16.86745
+0000b160: 2c31 392e 3438 3339 3237 2043 2031 362e  ,19.483927 C 16.
+0000b170: 3732 3734 3438 2c31 392e 3134 3439 3036  727448,19.144906
+0000b180: 2031 362e 3630 3633 3136 2c31 382e 3739   16.606316,18.79
+0000b190: 3639 3737 2031 362e 3532 3731 3337 2c31  6977 16.527137,1
+0000b1a0: 382e 3433 3834 3038 2043 2031 362e 3433  8.438408 C 16.43
+0000b1b0: 3239 3631 2c31 382e 3031 3836 3239 2031  2961,18.018629 1
+0000b1c0: 362e 3336 3236 3035 2c31 372e 3539 3339  6.362605,17.5939
+0000b1d0: 3631 2031 362e 3239 3439 3534 2c31 372e  61 16.294954,17.
+0000b1e0: 3136 3932 3436 2043 2031 362e 3134 3531  169246 C 16.1451
+0000b1f0: 3632 2c31 362e 3231 3131 3032 2031 362e  62,16.211102 16.
+0000b200: 3032 3233 3138 2c31 352e 3234 3920 3135  022318,15.249 15
+0000b210: 2e39 3033 3436 372c 3134 2e32 3836 3631  .903467,14.28661
+0000b220: 3220 4320 3135 2e36 3933 3437 382c 3132  2 C 15.693478,12
+0000b230: 2e37 3035 3938 3620 3135 2e34 3833 3438  .705986 15.48348
+0000b240: 392c 3131 2e31 3235 3336 3120 3135 2e32  9,11.125361 15.2
+0000b250: 3733 352c 392e 3534 3437 3334 3420 4320  735,9.5447344 C 
+0000b260: 3135 2e31 3230 3637 362c 382e 3338 3030  15.120676,8.3800
+0000b270: 3135 3320 3134 2e39 3434 3731 332c 372e  153 14.944713,7.
+0000b280: 3231 3735 3633 2031 342e 3730 3935 352c  217563 14.70955,
+0000b290: 362e 3036 3633 3436 3520 4320 3134 2e35  6.0663465 C 14.5
+0000b2a0: 3635 3539 342c 352e 3336 3935 3834 3720  65594,5.3695847 
+0000b2b0: 3134 2e34 3031 3834 362c 342e 3637 3537  14.401846,4.6757
+0000b2c0: 3035 3420 3134 2e31 3832 3832 2c33 2e39  054 14.18282,3.9
+0000b2d0: 3938 3330 3932 2043 2031 342e 3037 3932  983092 C 14.0792
+0000b2e0: 3334 2c33 2e36 3830 3838 3334 2031 332e  34,3.6808834 13.
+0000b2f0: 3936 3333 3434 2c33 2e33 3636 3833 3535  963344,3.3668355
+0000b300: 2031 332e 3832 3036 3438 2c33 2e30 3634   13.820648,3.064
+0000b310: 3730 3733 2043 2031 332e 3033 3333 3332  7073 C 13.033332
+0000b320: 2c33 2e39 3937 3731 3231 2031 322e 3337  ,3.9977121 12.37
+0000b330: 3036 3835 2c35 2e30 3330 3339 3735 2031  0685,5.0303975 1
+0000b340: 312e 3739 3534 3637 2c36 2e31 3035 3532  1.795467,6.10552
+0000b350: 3039 2043 2031 312e 3133 3039 3032 2c37  09 C 11.130902,7
+0000b360: 2e33 3439 3636 2031 302e 3538 3238 332c  .34966 10.58283,
+0000b370: 382e 3635 3331 3334 3820 3130 2e31 3038  8.6531348 10.108
+0000b380: 3630 362c 392e 3938 3035 3934 3520 4320  606,9.9805945 C 
+0000b390: 392e 3538 3737 3835 352c 3131 2e34 3237  9.5877855,11.427
+0000b3a0: 3930 3620 392e 3135 3834 3635 322c 3132  906 9.1584652,12
+0000b3b0: 2e39 3131 3431 3320 382e 3838 3732 3838  .911413 8.887288
+0000b3c0: 352c 3134 2e34 3236 3630 3320 4320 382e  5,14.426603 C 8.
+0000b3d0: 3639 3830 3536 342c 3135 2e34 3836 3537  6980564,15.48657
+0000b3e0: 3520 382e 3538 3831 3032 382c 3136 2e35  5 8.5881028,16.5
+0000b3f0: 3632 3438 3720 382e 3539 3238 3633 372c  62487 8.5928637,
+0000b400: 3137 2e36 3339 3835 3520 4320 382e 3539  17.639855 C 8.59
+0000b410: 3238 3633 372c 3138 2e30 3631 3439 3520  28637,18.061495 
+0000b420: 382e 3539 3238 3633 372c 3138 2e34 3833  8.5928637,18.483
+0000b430: 3133 3420 382e 3539 3238 3633 372c 3138  134 8.5928637,18
+0000b440: 2e39 3034 3737 3420 4320 372e 3736 3530  .904774 C 7.7650
+0000b450: 3237 332c 3138 2e39 3034 3737 3420 362e  273,18.904774 6.
+0000b460: 3933 3731 3932 322c 3138 2e39 3034 3737  9371922,18.90477
+0000b470: 3420 362e 3130 3933 3535 392c 3138 2e39  4 6.1093559,18.9
+0000b480: 3034 3737 3420 7a20 4d20 3230 2e30 3931  04774 z M 20.091
+0000b490: 3530 352c 3231 2e34 3132 3337 2043 2032  505,21.41237 C 2
+0000b4a0: 302e 3730 3339 3839 2c32 322e 3039 3133  0.703989,22.0913
+0000b4b0: 3033 2032 312e 3337 3632 3136 2c32 322e  03 21.376216,22.
+0000b4c0: 3732 3230 3220 3232 2e31 3330 3836 372c  72202 22.130867,
+0000b4d0: 3233 2e32 3431 3230 3620 4320 3232 2e37  23.241206 C 22.7
+0000b4e0: 3630 3237 362c 3233 2e36 3733 3638 2032  60276,23.67368 2
+0000b4f0: 332e 3435 3131 3536 2c32 342e 3032 3633  3.451156,24.0263
+0000b500: 3035 2032 342e 3138 3938 3735 2c32 342e  05 24.189875,24.
+0000b510: 3232 3831 3739 2043 2032 342e 3835 3138  228179 C 24.8518
+0000b520: 3136 2c32 342e 3431 3034 3036 2032 352e  16,24.410406 25.
+0000b530: 3535 3034 3239 2c32 342e 3436 3436 3431  550429,24.464641
+0000b540: 2032 362e 3233 3134 3037 2c32 342e 3337   26.231407,24.37
+0000b550: 3235 3836 2043 2032 362e 3734 3335 3132  2586 C 26.743512
+0000b560: 2c32 342e 3330 3335 3633 2032 372e 3234  ,24.303563 27.24
+0000b570: 3433 3532 2c32 342e 3134 3234 3439 2032  4352,24.142449 2
+0000b580: 372e 3639 3437 3337 2c32 332e 3838 3830  7.694737,23.8880
+0000b590: 3837 2043 2032 382e 3037 3339 3939 2c32  87 C 28.073999,2
+0000b5a0: 332e 3637 3533 3734 2032 382e 3431 3536  3.675374 28.4156
+0000b5b0: 3539 2c32 332e 3339 3839 3435 2032 382e  59,23.398945 28.
+0000b5c0: 3731 3335 3137 2c32 332e 3038 3238 3537  713517,23.082857
+0000b5d0: 2043 2032 392e 3038 3334 3837 2c32 322e   C 29.083487,22.
+0000b5e0: 3639 3632 3332 2032 392e 3338 3137 3035  696232 29.381705
+0000b5f0: 2c32 322e 3234 3035 3737 2032 392e 3538  ,22.240577 29.58
+0000b600: 3235 3037 2c32 312e 3734 3433 3532 2043  2507,21.744352 C
+0000b610: 2032 392e 3830 3637 3536 2c32 312e 3139   29.806756,21.19
+0000b620: 3435 3034 2032 392e 3931 3138 3934 2c32  4504 29.911894,2
+0000b630: 302e 3630 3037 3637 2032 392e 3932 3436  0.600767 29.9246
+0000b640: 3736 2c32 302e 3030 3834 3820 4320 3239  76,20.00848 C 29
+0000b650: 2e39 3337 3535 332c 3139 2e35 3135 3135  .937553,19.51515
+0000b660: 3620 3239 2e38 3739 3034 362c 3139 2e30  6 29.879046,19.0
+0000b670: 3137 3932 3120 3239 2e37 3239 3435 352c  17921 29.729455,
+0000b680: 3138 2e35 3436 3735 3620 4320 3239 2e35  18.546756 C 29.5
+0000b690: 3736 3730 392c 3138 2e30 3630 3535 3820  76709,18.060558 
+0000b6a0: 3239 2e33 3236 3834 312c 3137 2e36 3036  29.326841,17.606
+0000b6b0: 3339 3520 3239 2e30 3035 3334 2c31 372e  395 29.00534,17.
+0000b6c0: 3231 3134 3120 4320 3238 2e36 3531 3434  21141 C 28.65144
+0000b6d0: 332c 3136 2e37 3736 3531 3320 3238 2e32  3,16.776513 28.2
+0000b6e0: 3139 3438 392c 3136 2e34 3030 3533 3720  19489,16.400537 
+0000b6f0: 3237 2e37 3232 3732 372c 3136 2e31 3337  27.722727,16.137
+0000b700: 3336 3420 4320 3237 2e32 3835 3137 352c  364 C 27.285175,
+0000b710: 3135 2e39 3033 3934 3620 3236 2e38 3030  15.903946 26.800
+0000b720: 3536 332c 3135 2e37 3632 3430 3220 3236  563,15.762402 26
+0000b730: 2e33 3037 3630 322c 3135 2e37 3132 3532  .307602,15.71252
+0000b740: 3820 4320 3235 2e36 3338 3532 392c 3135  8 C 25.638529,15
+0000b750: 2e36 3434 3838 3920 3234 2e39 3532 3537  .644889 24.95257
+0000b760: 362c 3135 2e37 3235 3134 3620 3234 2e33  6,15.725146 24.3
+0000b770: 3232 3838 372c 3135 2e39 3633 3839 3620  22887,15.963896 
+0000b780: 4320 3233 2e37 3331 3738 312c 3136 2e31  C 23.731781,16.1
+0000b790: 3835 3738 3120 3233 2e31 3936 3933 362c  85781 23.196936,
+0000b7a0: 3136 2e35 3431 3432 2032 322e 3733 3533  16.54142 22.7353
+0000b7b0: 382c 3136 2e39 3639 3534 3220 4320 3232  8,16.969542 C 22
+0000b7c0: 2e31 3730 3139 372c 3137 2e34 3933 3337  .170197,17.49337
+0000b7d0: 3620 3231 2e37 3037 3137 362c 3138 2e31  6 21.707176,18.1
+0000b7e0: 3138 3236 3320 3231 2e33 3132 3536 2c31  18263 21.31256,1
+0000b7f0: 382e 3737 3737 2043 2032 302e 3831 3539  8.7777 C 20.8159
+0000b800: 3833 2c31 392e 3631 3038 3337 2032 302e  83,19.610837 20.
+0000b810: 3432 3433 3731 2c32 302e 3530 3236 3837  424371,20.502687
+0000b820: 2032 302e 3039 3135 3035 2c32 312e 3431   20.091505,21.41
+0000b830: 3233 3720 7a20 2720 7374 796c 653d 2766  237 z ' style='f
+0000b840: 696c 6c3a 2024 7a6f 6469 6163 5f63 6f6c  ill: $zodiac_col
+0000b850: 6f72 5f39 3b27 202f 3e0d 0a20 2020 2020  or_9;' />..     
+0000b860: 2020 2020 2020 2020 2020 203c 2f73 796d             </sym
+0000b870: 626f 6c3e 0d0a 2020 2020 2020 2020 2020  bol>..          
+0000b880: 2020 2020 2020 3c73 796d 626f 6c20 6964        <symbol id
+0000b890: 3d27 6171 7561 7269 7573 273e 0d0a 2020  ='aquarius'>..  
+0000b8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b8b0: 2020 3c70 6174 6820 7472 616e 7366 6f72    <path transfor
+0000b8c0: 6d3d 2273 6361 6c65 2830 2e38 2922 2064  m="scale(0.8)" d
+0000b8d0: 3d27 4d20 3265 2d30 362c 3234 2e37 3031  ='M 2e-06,24.701
+0000b8e0: 3635 3720 4c20 392e 3637 3731 312c 3138  657 L 9.67711,18
+0000b8f0: 2e33 3232 3638 3420 4c20 3131 2e37 3937  .322684 L 11.797
+0000b900: 3539 322c 3233 2e32 3634 3134 3220 4c20  592,23.264142 L 
+0000b910: 3139 2e32 3839 3936 312c 3138 2e33 3232  19.289961,18.322
+0000b920: 3638 3420 4c20 3231 2e33 3834 3734 2c32  684 L 21.38474,2
+0000b930: 332e 3236 3431 3432 204c 2032 382e 3838  3.264142 L 28.88
+0000b940: 3939 362c 3138 2e33 3232 3638 3420 4c20  996,18.322684 L 
+0000b950: 3331 2e39 3837 3134 392c 3235 2e36 3030  31.987149,25.600
+0000b960: 3130 3420 4c20 3239 2e39 3832 3333 2c32  104 L 29.98233,2
+0000b970: 362e 3438 3537 3136 204c 2032 372e 3931  6.485716 L 27.91
+0000b980: 3332 3533 2c32 312e 3534 3432 3538 204c  3253,21.544258 L
+0000b990: 2032 302e 3338 3233 332c 3236 2e34 3835   20.38233,26.485
+0000b9a0: 3731 3620 4c20 3138 2e32 3837 3535 312c  716 L 18.287551,
+0000b9b0: 3231 2e35 3434 3235 3820 4c20 3130 2e38  21.544258 L 10.8
+0000b9c0: 3230 3838 352c 3236 2e34 3835 3731 3620  20885,26.485716 
+0000b9d0: 4c20 382e 3731 3332 3534 2c32 312e 3534  L 8.713254,21.54
+0000b9e0: 3432 3538 204c 2031 2e31 3832 3333 312c  4258 L 1.182331,
+0000b9f0: 3236 2e34 3835 3731 3620 4c20 3265 2d30  26.485716 L 2e-0
+0000ba00: 362c 3234 2e37 3031 3635 3720 7a20 4d20  6,24.701657 z M 
+0000ba10: 302e 3031 3238 3533 2c31 312e 3339 3138  0.012853,11.3918
+0000ba20: 3038 204c 2039 2e36 3839 3936 312c 3520  08 L 9.689961,5 
+0000ba30: 4c20 3131 2e38 3130 3434 332c 392e 3934  L 11.810443,9.94
+0000ba40: 3134 3538 204c 2031 392e 3331 3536 3634  1458 L 19.315664
+0000ba50: 2c35 204c 2032 312e 3431 3034 3433 2c39  ,5 L 21.410443,9
+0000ba60: 2e39 3431 3435 3820 4c20 3238 2e39 3032  .941458 L 28.902
+0000ba70: 3831 322c 3520 4c20 3332 2c31 322e 3237  812,5 L 32,12.27
+0000ba80: 3734 3220 4c20 3239 2e39 3935 3138 312c  742 L 29.995181,
+0000ba90: 3133 2e31 3633 3033 3220 4c20 3237 2e39  13.163032 L 27.9
+0000baa0: 3236 3130 352c 382e 3232 3135 3734 204c  26105,8.221574 L
+0000bab0: 2032 302e 3338 3233 332c 3133 2e31 3633   20.38233,13.163
+0000bac0: 3033 3220 4c20 3138 2e32 3837 3535 312c  032 L 18.287551,
+0000bad0: 382e 3232 3135 3734 204c 2031 302e 3832  8.221574 L 10.82
+0000bae0: 3038 3835 2c31 332e 3136 3330 3332 204c  0885,13.163032 L
+0000baf0: 2038 2e37 3338 3935 372c 382e 3232 3135   8.738957,8.2215
+0000bb00: 3734 204c 2031 2e32 3038 3033 342c 3133  74 L 1.208034,13
+0000bb10: 2e31 3633 3033 3220 4c20 302e 3031 3238  .163032 L 0.0128
+0000bb20: 3533 2c31 312e 3339 3138 3038 207a 2027  53,11.391808 z '
+0000bb30: 2073 7479 6c65 3d27 6669 6c6c 3a20 247a   style='fill: $z
+0000bb40: 6f64 6961 635f 636f 6c6f 725f 3130 3b27  odiac_color_10;'
+0000bb50: 202f 3e0d 0a20 2020 2020 2020 2020 2020   />..           
+0000bb60: 2020 2020 203c 2f73 796d 626f 6c3e 0d0a       </symbol>..
+0000bb70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bb80: 3c73 796d 626f 6c20 6964 3d27 7069 7363  <symbol id='pisc
+0000bb90: 6573 273e 0d0a 2020 2020 2020 2020 2020  es'>..          
+0000bba0: 2020 2020 2020 2020 2020 3c70 6174 6820            <path 
+0000bbb0: 7472 616e 7366 6f72 6d3d 2273 6361 6c65  transform="scale
+0000bbc0: 2830 2e38 2922 2064 3d27 4d20 3133 2e32  (0.8)" d='M 13.2
+0000bbd0: 3838 3132 322c 3136 2e34 3933 3539 3320  88122,16.493593 
+0000bbe0: 4320 3133 2e32 3838 3334 312c 3138 2e30  C 13.288341,18.0
+0000bbf0: 3633 3639 3920 3133 2e30 3534 3638 2c31  63699 13.05468,1
+0000bc00: 392e 3632 3833 3632 2031 322e 3635 3939  9.628362 12.6599
+0000bc10: 3235 2c32 312e 3134 3631 3536 2043 2031  25,21.146156 C 1
+0000bc20: 322e 3335 3737 3034 2c32 322e 3330 3732  2.357704,22.3072
+0000bc30: 3434 2031 312e 3936 3332 3133 2c32 332e  44 11.963213,23.
+0000bc40: 3434 3334 3039 2031 312e 3530 3033 372c  443409 11.50037,
+0000bc50: 3234 2e35 3439 3935 3820 4320 3130 2e36  24.549958 C 10.6
+0000bc60: 3836 3138 382c 3236 2e34 3738 3439 3320  86188,26.478493 
+0000bc70: 392e 3636 3631 3735 372c 3238 2e33 3232  9.6661757,28.322
+0000bc80: 3035 3320 382e 3434 3037 3139 372c 3330  053 8.4407197,30
+0000bc90: 2e30 3230 3037 3620 4320 372e 3934 3730  .020076 C 7.9470
+0000bca0: 3935 372c 3330 2e37 3034 3635 2037 2e34  957,30.70465 7.4
+0000bcb0: 3230 3738 3037 2c33 312e 3336 3536 3439  207807,31.365649
+0000bcc0: 2036 2e38 3634 3039 3237 2c33 3220 4320   6.8640927,32 C 
+0000bcd0: 352e 3735 3534 3534 2c33 3220 342e 3634  5.755454,32 4.64
+0000bce0: 3638 3135 332c 3332 2033 2e35 3338 3137  68153,32 3.53817
+0000bcf0: 3636 2c33 3220 4320 352e 3035 3232 3033  66,32 C 5.052203
+0000bd00: 342c 3330 2e34 3034 3035 3520 362e 3430  4,30.404055 6.40
+0000bd10: 3937 3932 372c 3238 2e36 3530 3837 3220  97927,28.650872 
+0000bd20: 372e 3439 3831 3530 372c 3236 2e37 3336  7.4981507,26.736
+0000bd30: 3333 3520 4320 382e 3433 3235 3034 372c  335 C 8.4325047,
+0000bd40: 3235 2e30 3935 3232 3620 392e 3136 3330  25.095226 9.1630
+0000bd50: 3030 372c 3233 2e33 3334 3839 3620 392e  007,23.334896 9.
+0000bd60: 3632 3835 3737 372c 3231 2e35 3033 3537  6285777,21.50357
+0000bd70: 3920 4320 3130 2e30 3436 3233 382c 3139  9 C 10.046238,19
+0000bd80: 2e38 3638 3633 3620 3130 2e32 3531 3637  .868636 10.25167
+0000bd90: 352c 3138 2e31 3830 3731 3120 3130 2e32  5,18.180711 10.2
+0000bda0: 3530 3735 362c 3136 2e34 3933 3539 3320  50756,16.493593 
+0000bdb0: 4320 382e 3038 3931 3633 372c 3136 2e34  C 8.0891637,16.4
+0000bdc0: 3933 3539 3320 352e 3932 3735 3730 372c  93593 5.9275707,
+0000bdd0: 3136 2e34 3933 3539 3320 332e 3736 3539  16.493593 3.7659
+0000bde0: 3739 312c 3136 2e34 3933 3539 3320 4320  791,16.493593 C 
+0000bdf0: 332e 3736 3539 3739 312c 3135 2e37 3334  3.7659791,15.734
+0000be00: 3231 3920 332e 3736 3539 3739 312c 3134  219 3.7659791,14
+0000be10: 2e39 3734 3834 3620 332e 3736 3539 3739  .974846 3.765979
+0000be20: 312c 3134 2e32 3135 3437 3220 4320 352e  1,14.215472 C 5.
+0000be30: 3932 3735 3730 372c 3134 2e32 3135 3437  9275707,14.21547
+0000be40: 3220 382e 3038 3931 3633 372c 3134 2e32  2 8.0891637,14.2
+0000be50: 3135 3437 3220 3130 2e32 3530 3735 362c  15472 10.250756,
+0000be60: 3134 2e32 3135 3437 3220 4320 3130 2e31  14.215472 C 10.1
+0000be70: 3535 3936 322c 3132 2e34 3937 3939 3120  55962,12.497991 
+0000be80: 392e 3831 3234 3836 372c 3130 2e37 3936  9.8124867,10.796
+0000be90: 3437 2039 2e32 3534 3634 3837 2c39 2e31  47 9.2546487,9.1
+0000bea0: 3730 3034 3320 4320 382e 3631 3035 3436  70043 C 8.610546
+0000beb0: 372c 372e 3238 3634 2037 2e36 3836 3231  7,7.2864 7.68621
+0000bec0: 3037 2c35 2e35 3035 3639 3120 362e 3538  07,5.505691 6.58
+0000bed0: 3330 3636 372c 332e 3835 3132 3534 2043  30667,3.851254 C
+0000bee0: 2035 2e36 3734 3330 3331 2c32 2e34 3837   5.6743031,2.487
+0000bef0: 3930 3820 342e 3634 3531 3235 2c31 2e32  908 4.645125,1.2
+0000bf00: 3037 3039 3839 2033 2e35 3338 3137 3636  070989 3.5381766
+0000bf10: 2c33 652d 3037 2043 2034 2e35 3836 3036  ,3e-07 C 4.58606
+0000bf20: 382c 3365 2d30 3720 352e 3633 3339 3539  8,3e-07 5.633959
+0000bf30: 332c 3365 2d30 3720 362e 3638 3138 3530  3,3e-07 6.681850
+0000bf40: 372c 3365 2d30 3720 4320 382e 3135 3939  7,3e-07 C 8.1599
+0000bf50: 3339 372c 312e 3537 3538 3437 3620 392e  397,1.5758476 9.
+0000bf60: 3436 3235 3835 372c 332e 3332 3136 3520  4625857,3.32165 
+0000bf70: 3130 2e35 3034 3333 352c 352e 3231 3632  10.504335,5.2162
+0000bf80: 3331 2043 2031 312e 3436 3030 3434 2c36  31 C 11.460044,6
+0000bf90: 2e39 3530 3234 3820 3132 2e31 3933 3035  .950248 12.19305
+0000bfa0: 362c 382e 3830 3639 3139 2031 322e 3637  6,8.806919 12.67
+0000bfb0: 3637 3238 2c31 302e 3732 3639 3835 2043  6728,10.726985 C
+0000bfc0: 2031 322e 3936 3631 3731 2c31 312e 3837   12.966171,11.87
+0000bfd0: 3236 3435 2031 332e 3136 3833 3634 2c31  2645 13.168364,1
+0000bfe0: 332e 3034 3030 3036 2031 332e 3238 3831  3.040006 13.2881
+0000bff0: 3232 2c31 342e 3231 3534 3732 2043 2031  22,14.215472 C 1
+0000c000: 352e 3338 3339 3035 2c31 342e 3231 3534  5.383905,14.2154
+0000c010: 3732 2031 372e 3437 3936 3838 2c31 342e  72 17.479688,14.
+0000c020: 3231 3534 3732 2031 392e 3537 3534 372c  215472 19.57547,
+0000c030: 3134 2e32 3135 3437 3220 4320 3139 2e37  14.215472 C 19.7
+0000c040: 3836 3838 322c 3132 2e31 3837 3735 3820  86882,12.187758 
+0000c050: 3230 2e32 3435 3838 342c 3130 2e31 3834  20.245884,10.184
+0000c060: 3133 2032 302e 3936 3332 3439 2c38 2e32  13 20.963249,8.2
+0000c070: 3735 3034 3120 4320 3231 2e36 3730 3432  75041 C 21.67042
+0000c080: 392c 362e 3338 3637 3732 2032 322e 3632  9,6.386772 22.62
+0000c090: 3836 3535 2c34 2e35 3934 3834 3920 3233  8655,4.594849 23
+0000c0a0: 2e37 3836 3533 332c 322e 3934 3439 3136  .786533,2.944916
+0000c0b0: 2043 2032 342e 3531 3334 3135 2c31 2e39   C 24.513415,1.9
+0000c0c0: 3037 3832 3239 2032 352e 3331 3735 3838  078229 25.317588
+0000c0d0: 2c30 2e39 3235 3536 3837 2032 362e 3138  ,0.9255687 26.18
+0000c0e0: 3137 3432 2c33 652d 3037 2043 2032 372e  1742,3e-07 C 27.
+0000c0f0: 3232 3936 3333 2c33 652d 3037 2032 382e  229633,3e-07 28.
+0000c100: 3237 3735 3235 2c33 652d 3037 2032 392e  277525,3e-07 29.
+0000c110: 3332 3534 3136 2c33 652d 3037 2043 2032  325416,3e-07 C 2
+0000c120: 372e 3835 3436 3138 2c31 2e36 3034 3038  7.854618,1.60408
+0000c130: 3837 2032 362e 3531 3838 3439 2c33 2e33  87 26.518849,3.3
+0000c140: 3430 3034 3720 3235 2e34 3234 3932 312c  40047 25.424921,
+0000c150: 352e 3232 3430 3136 2043 2032 342e 3437  5.224016 C 24.47
+0000c160: 3034 3538 2c36 2e38 3637 3033 2032 332e  0458,6.86703 23.
+0000c170: 3730 3439 3935 2c38 2e36 3235 3439 3820  704995,8.625498 
+0000c180: 3233 2e32 3135 3137 352c 3130 2e34 3633  23.215175,10.463
+0000c190: 3336 3420 4320 3232 2e38 3837 3534 372c  364 C 22.887547,
+0000c1a0: 3131 2e36 3839 3233 3220 3232 2e36 3833  11.689232 22.683
+0000c1b0: 3238 312c 3132 2e39 3438 3339 3220 3232  281,12.948392 22
+0000c1c0: 2e36 3132 3833 372c 3134 2e32 3135 3437  .612837,14.21547
+0000c1d0: 3220 4320 3234 2e37 3734 3432 382c 3134  2 C 24.774428,14
+0000c1e0: 2e32 3135 3437 3220 3236 2e39 3336 3032  .215472 26.93602
+0000c1f0: 322c 3134 2e32 3135 3437 3220 3239 2e30  2,14.215472 29.0
+0000c200: 3937 3631 342c 3134 2e32 3135 3437 3220  97614,14.215472 
+0000c210: 4320 3239 2e30 3937 3631 342c 3134 2e39  C 29.097614,14.9
+0000c220: 3734 3834 3620 3239 2e30 3937 3631 342c  74846 29.097614,
+0000c230: 3135 2e37 3334 3231 3920 3239 2e30 3937  15.734219 29.097
+0000c240: 3631 342c 3136 2e34 3933 3539 3320 4320  614,16.493593 C 
+0000c250: 3236 2e39 3336 3032 322c 3136 2e34 3933  26.936022,16.493
+0000c260: 3539 3320 3234 2e37 3734 3432 382c 3136  593 24.774428,16
+0000c270: 2e34 3933 3539 3320 3232 2e36 3132 3833  .493593 22.61283
+0000c280: 372c 3136 2e34 3933 3539 3320 4320 3232  7,16.493593 C 22
+0000c290: 2e36 3131 3539 312c 3138 2e33 3130 3031  .611591,18.31001
+0000c2a0: 3320 3232 2e38 3530 3534 342c 3230 2e31  3 22.850544,20.1
+0000c2b0: 3237 3334 3720 3233 2e33 3334 3435 342c  27347 23.334454,
+0000c2c0: 3231 2e38 3738 3532 3420 4320 3233 2e38  21.878524 C 23.8
+0000c2d0: 3337 3332 322c 3233 2e37 3037 3239 3320  37322,23.707293 
+0000c2e0: 3234 2e36 3034 3336 392c 3235 2e34 3539  24.604369,25.459
+0000c2f0: 3439 3420 3235 2e35 3730 3639 342c 3237  494 25.570694,27
+0000c300: 2e30 3930 3130 3520 4320 3236 2e36 3232  .090105 C 26.622
+0000c310: 3732 372c 3238 2e38 3637 3736 3520 3237  727,28.867765 27
+0000c320: 2e39 3035 3038 332c 3330 2e35 3032 3732  .905083,30.50272
+0000c330: 3320 3239 2e33 3235 3431 362c 3332 2043  3 29.325416,32 C
+0000c340: 2032 382e 3232 3138 3339 2c33 3220 3237   28.221839,32 27
+0000c350: 2e31 3138 3236 342c 3332 2032 362e 3031  .118264,32 26.01
+0000c360: 3436 3837 2c33 3220 4320 3234 2e36 3934  4687,32 C 24.694
+0000c370: 3433 352c 3330 2e35 3038 3337 3720 3233  435,30.508377 23
+0000c380: 2e35 3439 3139 372c 3238 2e38 3633 3331  .549197,28.86331
+0000c390: 3520 3232 2e35 3937 3331 332c 3237 2e31  5 22.597313,27.1
+0000c3a0: 3133 3832 3120 4320 3232 2e31 3034 3238  13821 C 22.10428
+0000c3b0: 2c32 362e 3230 3737 3938 2032 312e 3636  ,26.207798 21.66
+0000c3c0: 3035 3333 2c32 352e 3237 3439 3120 3231  0533,25.27491 21
+0000c3d0: 2e32 3638 3236 352c 3234 2e33 3230 3933  .268265,24.32093
+0000c3e0: 3520 4320 3230 2e36 3233 3633 342c 3232  5 C 20.623634,22
+0000c3f0: 2e37 3337 3733 3920 3230 2e31 3135 3631  .737739 20.11561
+0000c400: 332c 3231 2e30 3933 3732 3920 3139 2e38  3,21.093729 19.8
+0000c410: 3238 3932 322c 3139 2e34 3036 3732 3120  28922,19.406721 
+0000c420: 4320 3139 2e36 3635 3538 352c 3138 2e34  C 19.665585,18.4
+0000c430: 3434 3736 3820 3139 2e35 3735 3430 322c  44768 19.575402,
+0000c440: 3137 2e34 3639 3630 3320 3139 2e35 3735  17.469603 19.575
+0000c450: 3437 2c31 362e 3439 3335 3933 2043 2031  47,16.493593 C 1
+0000c460: 372e 3437 3936 3838 2c31 362e 3439 3335  7.479688,16.4935
+0000c470: 3933 2031 352e 3338 3339 3035 2c31 362e  93 15.383905,16.
+0000c480: 3439 3335 3933 2031 332e 3238 3831 3232  493593 13.288122
+0000c490: 2c31 362e 3439 3335 3933 207a 2027 2073  ,16.493593 z ' s
+0000c4a0: 7479 6c65 3d27 6669 6c6c 3a20 247a 6f64  tyle='fill: $zod
+0000c4b0: 6961 635f 636f 6c6f 725f 3131 3b27 202f  iac_color_11;' /
+0000c4c0: 3e0d 0a20 2020 2020 2020 2020 2020 2020  >..             
+0000c4d0: 2020 203c 2f73 796d 626f 6c3e 2020 2020     </symbol>    
+0000c4e0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+0000c4f0: 2020 2020 2020 2020 2020 2020 2020 3c21                <!
+0000c500: 2d2d 2041 7370 6563 7473 2031 3278 3132  -- Aspects 12x12
+0000c510: 202d 2d3e 0d0a 2020 2020 2020 2020 2020   -->..          
+0000c520: 2020 2020 2020 3c73 796d 626f 6c20 6964        <symbol id
+0000c530: 3d27 6f72 6230 273e 0d0a 2020 2020 2020  ='orb0'>..      
+0000c540: 2020 2020 2020 2020 2020 2020 2020 3c70                <p
+0000c550: 6174 6820 643d 274d 2036 2e30 3639 3735  ath d='M 6.06975
+0000c560: 3339 2c37 2e33 3233 3438 3532 2043 2036  39,7.3234852 C 6
+0000c570: 2e30 3639 3735 3339 2c38 2e37 3335 3438  .0697539,8.73548
+0000c580: 3832 2034 2e39 3137 3336 3531 2c39 2e38  82 4.9173651,9.8
+0000c590: 3830 3134 3432 2033 2e34 3935 3832 3134  801442 3.4958214
+0000c5a0: 2c39 2e38 3830 3134 3432 2043 2032 2e30  ,9.8801442 C 2.0
+0000c5b0: 3734 3237 3735 2c39 2e38 3830 3134 3432  742775,9.8801442
+0000c5c0: 2030 2e39 3231 3838 3835 372c 382e 3733   0.92188857,8.73
+0000c5d0: 3534 3838 3220 302e 3932 3138 3838 3537  54882 0.92188857
+0000c5e0: 2c37 2e33 3233 3438 3532 2043 2030 2e39  ,7.3234852 C 0.9
+0000c5f0: 3231 3838 3835 372c 352e 3931 3134 3832  2188857,5.911482
+0000c600: 3220 322e 3037 3432 3737 352c 342e 3736  2 2.0742775,4.76
+0000c610: 3638 3237 3220 332e 3439 3538 3231 342c  68272 3.4958214,
+0000c620: 342e 3736 3638 3237 3220 4320 342e 3931  4.7668272 C 4.91
+0000c630: 3733 3635 312c 342e 3736 3638 3237 3220  73651,4.7668272 
+0000c640: 362e 3036 3937 3533 392c 352e 3931 3134  6.0697539,5.9114
+0000c650: 3832 3220 362e 3036 3937 3533 392c 372e  822 6.0697539,7.
+0000c660: 3332 3334 3835 3220 4c20 362e 3036 3937  3234852 L 6.0697
+0000c670: 3533 392c 372e 3332 3334 3835 3220 7a20  539,7.3234852 z 
+0000c680: 4d20 352e 3632 3532 3630 392c 352e 3231  M 5.6252609,5.21
+0000c690: 3133 3230 3220 4320 3130 2e30 3730 3139  13202 C 10.07019
+0000c6a0: 2c30 2e37 3636 3339 3031 3820 3130 2e30  ,0.76639018 10.0
+0000c6b0: 3730 3139 2c30 2e37 3636 3339 3031 3820  7019,0.76639018 
+0000c6c0: 3130 2e30 3730 3139 2c30 2e37 3636 3339  10.07019,0.76639
+0000c6d0: 3031 3827 2073 7479 6c65 3d27 6f70 6163  018' style='opac
+0000c6e0: 6974 793a 313b 6669 6c6c 3a6e 6f6e 653b  ity:1;fill:none;
+0000c6f0: 6669 6c6c 2d6f 7061 6369 7479 3a31 3b66  fill-opacity:1;f
+0000c700: 696c 6c2d 7275 6c65 3a6e 6f6e 7a65 726f  ill-rule:nonzero
+0000c710: 3b73 7472 6f6b 653a 2024 6f72 625f 636f  ;stroke: $orb_co
+0000c720: 6c6f 725f 303b 7374 726f 6b65 2d77 6964  lor_0;stroke-wid
+0000c730: 7468 3a31 2e34 3736 3333 3036 343b 7374  th:1.47633064;st
+0000c740: 726f 6b65 2d6c 696e 6563 6170 3a62 7574  roke-linecap:but
+0000c750: 743b 7374 726f 6b65 2d6c 696e 656a 6f69  t;stroke-linejoi
+0000c760: 6e3a 6d69 7465 723b 7374 726f 6b65 2d6d  n:miter;stroke-m
+0000c770: 6974 6572 6c69 6d69 743a 343b 7374 726f  iterlimit:4;stro
+0000c780: 6b65 2d64 6173 6861 7272 6179 3a6e 6f6e  ke-dasharray:non
+0000c790: 653b 7374 726f 6b65 2d6f 7061 6369 7479  e;stroke-opacity
+0000c7a0: 3a31 2720 2f3e 0d0a 2020 2020 2020 2020  :1' />..        
+0000c7b0: 2020 2020 2020 2020 3c2f 7379 6d62 6f6c          </symbol
+0000c7c0: 3e0d 0a20 2020 2020 2020 2020 2020 2020  >..             
+0000c7d0: 2020 203c 7379 6d62 6f6c 2069 643d 276f     <symbol id='o
+0000c7e0: 7262 3330 273e 0d0a 2020 2020 2020 2020  rb30'>..        
+0000c7f0: 2020 2020 2020 2020 2020 2020 3c70 6174              <pat
+0000c800: 6820 643d 274d 2030 2e38 3136 3735 3135  h d='M 0.8167515
+0000c810: 342c 362e 3133 3432 3339 3820 4320 3131  4,6.1342398 C 11
+0000c820: 2e33 3436 3631 352c 362e 3136 3230 3134  .346615,6.162014
+0000c830: 3820 3131 2e33 3436 3631 352c 362e 3136  8 11.346615,6.16
+0000c840: 3230 3134 3820 3131 2e33 3436 3631 352c  20148 11.346615,
+0000c850: 362e 3136 3230 3134 3820 4d20 3130 2e36  6.1620148 M 10.6
+0000c860: 3132 3138 342c 302e 3735 3939 3537 3733  12184,0.75995773
+0000c870: 2043 2035 2e37 3133 3834 3739 2c35 2e39   C 5.7138479,5.9
+0000c880: 3033 3231 3038 2035 2e37 3133 3834 3739  032108 5.7138479
+0000c890: 2c35 2e39 3033 3231 3038 2035 2e37 3133  ,5.9032108 5.713
+0000c8a0: 3834 3739 2c35 2e39 3033 3231 3038 204d  8479,5.9032108 M
+0000c8b0: 2031 2e33 3035 3334 3531 2c30 2e37 3539   1.3053451,0.759
+0000c8c0: 3935 3737 3320 4320 352e 3838 3037 3138  95773 C 5.880718
+0000c8d0: 392c 362e 3139 3235 3136 3820 352e 3838  9,6.1925168 5.88
+0000c8e0: 3037 3138 392c 362e 3139 3235 3136 3820  07189,6.1925168 
+0000c8f0: 352e 3838 3037 3138 392c 362e 3139 3235  5.8807189,6.1925
+0000c900: 3136 3827 2073 7479 6c65 3d27 6f70 6163  168' style='opac
+0000c910: 6974 793a 313b 6669 6c6c 3a6e 6f6e 653b  ity:1;fill:none;
+0000c920: 6669 6c6c 2d6f 7061 6369 7479 3a31 3b66  fill-opacity:1;f
+0000c930: 696c 6c2d 7275 6c65 3a6e 6f6e 7a65 726f  ill-rule:nonzero
+0000c940: 3b73 7472 6f6b 653a 2024 6f72 625f 636f  ;stroke: $orb_co
+0000c950: 6c6f 725f 3330 3b73 7472 6f6b 652d 7769  lor_30;stroke-wi
+0000c960: 6474 683a 312e 3437 3633 3330 3634 3b73  dth:1.47633064;s
+0000c970: 7472 6f6b 652d 6c69 6e65 6361 703a 6275  troke-linecap:bu
+0000c980: 7474 3b73 7472 6f6b 652d 6c69 6e65 6a6f  tt;stroke-linejo
+0000c990: 696e 3a6d 6974 6572 3b73 7472 6f6b 652d  in:miter;stroke-
+0000c9a0: 6d69 7465 726c 696d 6974 3a34 3b73 7472  miterlimit:4;str
+0000c9b0: 6f6b 652d 6461 7368 6172 7261 793a 6e6f  oke-dasharray:no
+0000c9c0: 6e65 3b73 7472 6f6b 652d 6f70 6163 6974  ne;stroke-opacit
+0000c9d0: 793a 3127 202f 3e0d 0a20 2020 2020 2020  y:1' />..       
+0000c9e0: 2020 2020 2020 2020 203c 2f73 796d 626f           </symbo
+0000c9f0: 6c3e 0d0a 2020 2020 2020 2020 2020 2020  l>..            
+0000ca00: 2020 2020 3c73 796d 626f 6c20 6964 3d27      <symbol id='
+0000ca10: 6f72 6234 3527 3e0d 0a20 2020 2020 2020  orb45'>..       
+0000ca20: 2020 2020 2020 2020 2020 2020 203c 7061               <pa
+0000ca30: 7468 2064 3d27 4d20 392e 3831 3030 3137  th d='M 9.810017
+0000ca40: 382c 392e 3539 3231 3936 3620 4320 362e  8,9.5921966 C 6.
+0000ca50: 3936 3430 3635 382c 392e 3539 3231 3935  9640658,9.592195
+0000ca60: 3620 342e 3131 3831 3132 352c 392e 3539  6 4.1181125,9.59
+0000ca70: 3231 3936 3620 312e 3237 3231 362c 392e  21966 1.27216,9.
+0000ca80: 3539 3231 3936 3620 4320 322e 3639 3531  5921966 C 2.6951
+0000ca90: 3336 322c 362e 3734 3632 3434 3120 342e  362,6.7462441 4.
+0000caa0: 3131 3831 3132 352c 332e 3930 3032 3930  1181125,3.900290
+0000cab0: 3520 352e 3534 3130 3838 382c 312e 3035  5 5.5410888,1.05
+0000cac0: 3433 3337 3927 2073 7479 6c65 3d27 6f70  43379' style='op
+0000cad0: 6163 6974 793a 313b 6669 6c6c 3a6e 6f6e  acity:1;fill:non
+0000cae0: 653b 6669 6c6c 2d6f 7061 6369 7479 3a31  e;fill-opacity:1
+0000caf0: 3b66 696c 6c2d 7275 6c65 3a6e 6f6e 7a65  ;fill-rule:nonze
+0000cb00: 726f 3b73 7472 6f6b 653a 2024 6f72 625f  ro;stroke: $orb_
+0000cb10: 636f 6c6f 725f 3435 3b73 7472 6f6b 652d  color_45;stroke-
+0000cb20: 7769 6474 683a 312e 3437 3633 3330 3634  width:1.47633064
+0000cb30: 3b73 7472 6f6b 652d 6c69 6e65 6361 703a  ;stroke-linecap:
+0000cb40: 6275 7474 3b73 7472 6f6b 652d 6c69 6e65  butt;stroke-line
+0000cb50: 6a6f 696e 3a6d 6974 6572 3b73 7472 6f6b  join:miter;strok
+0000cb60: 652d 6d69 7465 726c 696d 6974 3a34 3b73  e-miterlimit:4;s
+0000cb70: 7472 6f6b 652d 6461 7368 6172 7261 793a  troke-dasharray:
+0000cb80: 6e6f 6e65 3b73 7472 6f6b 652d 6f70 6163  none;stroke-opac
+0000cb90: 6974 793a 3127 202f 3e0d 0a20 2020 2020  ity:1' />..     
+0000cba0: 2020 2020 2020 2020 2020 203c 2f73 796d             </sym
+0000cbb0: 626f 6c3e 0d0a 2020 2020 2020 2020 2020  bol>..          
+0000cbc0: 2020 2020 2020 3c73 796d 626f 6c20 6964        <symbol id
+0000cbd0: 3d27 6f72 6236 3027 3e0d 0a20 2020 2020  ='orb60'>..     
+0000cbe0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+0000cbf0: 7061 7468 2064 3d27 4d20 302e 3838 3138  path d='M 0.8818
+0000cc00: 3234 3431 2c30 2e37 3138 3134 3736 3520  2441,0.71814765 
+0000cc10: 4320 332e 3338 3036 3837 322c 332e 3231  C 3.3806872,3.21
+0000cc20: 3736 3030 3720 352e 3837 3935 3530 322c  76007 5.8795502,
+0000cc30: 352e 3731 3730 3532 3720 382e 3337 3834  5.7170527 8.3784
+0000cc40: 3133 322c 382e 3231 3635 3035 3720 4d20  132,8.2165057 M 
+0000cc50: 382e 3631 3139 3336 322c 342e 3430 3336  8.6119362,4.4036
+0000cc60: 3535 3720 4320 352e 3936 3430 3434 322c  557 C 5.9640442,
+0000cc70: 342e 3430 3336 3535 3720 332e 3331 3631  4.4036557 3.3161
+0000cc80: 3533 342c 342e 3430 3336 3535 3720 302e  534,4.4036557 0.
+0000cc90: 3636 3832 3632 3231 2c34 2e34 3033 3635  66826221,4.40365
+0000cca0: 3537 204d 2030 2e38 3439 3235 3738 312c  57 M 0.84925781,
+0000ccb0: 382e 3139 3434 3937 3720 4320 332e 3337  8.1944977 C 3.37
+0000ccc0: 3634 3835 322c 352e 3732 3234 3333 3720  64852,5.7224337 
+0000ccd0: 352e 3930 3337 3133 322c 332e 3235 3033  5.9037132,3.2503
+0000cce0: 3730 3720 382e 3433 3039 3430 322c 302e  707 8.4309402,0.
+0000ccf0: 3737 3833 3037 3635 2720 7374 796c 653d  77830765' style=
+0000cd00: 276f 7061 6369 7479 3a31 3b66 696c 6c3a  'opacity:1;fill:
+0000cd10: 6e6f 6e65 3b66 696c 6c2d 6f70 6163 6974  none;fill-opacit
+0000cd20: 793a 313b 6669 6c6c 2d72 756c 653a 6e6f  y:1;fill-rule:no
+0000cd30: 6e7a 6572 6f3b 7374 726f 6b65 3a20 246f  nzero;stroke: $o
+0000cd40: 7262 5f63 6f6c 6f72 5f36 303b 7374 726f  rb_color_60;stro
+0000cd50: 6b65 2d77 6964 7468 3a31 2e34 3736 3333  ke-width:1.47633
+0000cd60: 3036 343b 7374 726f 6b65 2d6c 696e 6563  064;stroke-linec
+0000cd70: 6170 3a62 7574 743b 7374 726f 6b65 2d6c  ap:butt;stroke-l
+0000cd80: 696e 656a 6f69 6e3a 6d69 7465 723b 7374  inejoin:miter;st
+0000cd90: 726f 6b65 2d6d 6974 6572 6c69 6d69 743a  roke-miterlimit:
+0000cda0: 343b 7374 726f 6b65 2d64 6173 6861 7272  4;stroke-dasharr
+0000cdb0: 6179 3a6e 6f6e 653b 7374 726f 6b65 2d6f  ay:none;stroke-o
+0000cdc0: 7061 6369 7479 3a31 2720 2f3e 0d0a 2020  pacity:1' />..  
+0000cdd0: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+0000cde0: 7379 6d62 6f6c 3e0d 0a20 2020 2020 2020  symbol>..       
+0000cdf0: 2020 2020 2020 2020 203c 7379 6d62 6f6c           <symbol
+0000ce00: 2069 643d 276f 7262 3732 273e 0d0a 2020   id='orb72'>..  
+0000ce10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ce20: 2020 3c70 6174 6820 643d 274d 2038 2e39    <path d='M 8.9
+0000ce30: 3136 3530 3434 2c35 2e36 3431 3734 3338  165044,5.6417438
+0000ce40: 2043 2038 2e39 3136 3530 3434 2c37 2e39   C 8.9165044,7.9
+0000ce50: 3638 3736 3633 2037 2e32 3734 3238 3434  687663 7.2742844
+0000ce60: 2c39 2e38 3535 3138 3933 2035 2e32 3438  ,9.8551893 5.248
+0000ce70: 3530 3334 2c39 2e38 3535 3138 3933 2043  5034,9.8551893 C
+0000ce80: 2033 2e32 3232 3732 3234 2c39 2e38 3535   3.2227224,9.855
+0000ce90: 3138 3933 2031 2e35 3830 3530 3237 2c37  1893 1.5805027,7
+0000cea0: 2e39 3638 3736 3633 2031 2e35 3830 3530  .9687663 1.58050
+0000ceb0: 3237 2c35 2e36 3431 3734 3338 2043 2031  27,5.6417438 C 1
+0000cec0: 2e35 3830 3530 3237 2c33 2e33 3134 3732  .5805027,3.31472
+0000ced0: 3038 2033 2e32 3232 3732 3234 2c31 2e34  08 3.2227224,1.4
+0000cee0: 3238 3239 3637 2035 2e32 3438 3530 3334  282967 5.2485034
+0000cef0: 2c31 2e34 3238 3239 3637 2043 2037 2e32  ,1.4282967 C 7.2
+0000cf00: 3734 3238 3434 2c31 2e34 3238 3239 3637  742844,1.4282967
+0000cf10: 2038 2e39 3136 3530 3434 2c33 2e33 3134   8.9165044,3.314
+0000cf20: 3732 3038 2038 2e39 3136 3530 3434 2c35  7208 8.9165044,5
+0000cf30: 2e36 3431 3734 3338 204c 2038 2e39 3136  .6417438 L 8.916
+0000cf40: 3530 3434 2c35 2e36 3431 3734 3338 207a  5044,5.6417438 z
+0000cf50: 204d 2035 2e34 3730 3236 3334 2c36 2e37   M 5.4702634,6.7
+0000cf60: 3436 3333 3538 2043 2039 2e30 3531 3138  463358 C 9.05118
+0000cf70: 3034 2c31 302e 3131 3932 3238 2039 2e30  04,10.119228 9.0
+0000cf80: 3531 3138 3034 2c31 302e 3131 3932 3238  511804,10.119228
+0000cf90: 2039 2e30 3531 3138 3034 2c31 302e 3131   9.0511804,10.11
+0000cfa0: 3932 3238 2720 7374 796c 653d 276f 7061  9228' style='opa
+0000cfb0: 6369 7479 3a31 3b66 696c 6c3a 6e6f 6e65  city:1;fill:none
+0000cfc0: 3b66 696c 6c2d 6f70 6163 6974 793a 313b  ;fill-opacity:1;
+0000cfd0: 6669 6c6c 2d72 756c 653a 6e6f 6e7a 6572  fill-rule:nonzer
+0000cfe0: 6f3b 7374 726f 6b65 3a20 246f 7262 5f63  o;stroke: $orb_c
+0000cff0: 6f6c 6f72 5f37 323b 7374 726f 6b65 2d77  olor_72;stroke-w
+0000d000: 6964 7468 3a31 2e34 3736 3333 3036 343b  idth:1.47633064;
+0000d010: 7374 726f 6b65 2d6c 696e 6563 6170 3a62  stroke-linecap:b
+0000d020: 7574 743b 7374 726f 6b65 2d6c 696e 656a  utt;stroke-linej
+0000d030: 6f69 6e3a 6d69 7465 723b 7374 726f 6b65  oin:miter;stroke
+0000d040: 2d6d 6974 6572 6c69 6d69 743a 343b 7374  -miterlimit:4;st
+0000d050: 726f 6b65 2d64 6173 6861 7272 6179 3a6e  roke-dasharray:n
+0000d060: 6f6e 653b 7374 726f 6b65 2d6f 7061 6369  one;stroke-opaci
+0000d070: 7479 3a31 2720 2f3e 0d0a 2020 2020 2020  ty:1' />..      
+0000d080: 2020 2020 2020 2020 2020 3c2f 7379 6d62            </symb
+0000d090: 6f6c 3e0d 0a20 2020 2020 2020 2020 2020  ol>..           
+0000d0a0: 2020 2020 203c 7379 6d62 6f6c 2069 643d       <symbol id=
+0000d0b0: 276f 7262 3930 273e 0d0a 2020 2020 2020  'orb90'>..      
+0000d0c0: 2020 2020 2020 2020 2020 2020 2020 3c72                <r
+0000d0d0: 6563 7420 6865 6967 6874 3d27 382e 3038  ect height='8.08
+0000d0e0: 3631 3935 2720 7769 6474 683d 2738 2e37  6195' width='8.7
+0000d0f0: 3135 3831 3336 2720 783d 2731 2e31 3833  158136' x='1.183
+0000d100: 3138 3236 2720 793d 2731 2e31 3839 3235  1826' y='1.18925
+0000d110: 3435 2720 7374 796c 653d 276f 7061 6369  45' style='opaci
+0000d120: 7479 3a31 3b66 696c 6c3a 6e6f 6e65 3b66  ty:1;fill:none;f
+0000d130: 696c 6c2d 6f70 6163 6974 793a 313b 6669  ill-opacity:1;fi
+0000d140: 6c6c 2d72 756c 653a 6e6f 6e7a 6572 6f3b  ll-rule:nonzero;
+0000d150: 7374 726f 6b65 3a20 246f 7262 5f63 6f6c  stroke: $orb_col
+0000d160: 6f72 5f39 303b 7374 726f 6b65 2d77 6964  or_90;stroke-wid
+0000d170: 7468 3a31 2e32 3530 3339 3531 383b 7374  th:1.25039518;st
+0000d180: 726f 6b65 2d6c 696e 6563 6170 3a62 7574  roke-linecap:but
+0000d190: 743b 7374 726f 6b65 2d6c 696e 656a 6f69  t;stroke-linejoi
+0000d1a0: 6e3a 6d69 7465 723b 7374 726f 6b65 2d6d  n:miter;stroke-m
+0000d1b0: 6974 6572 6c69 6d69 743a 343b 7374 726f  iterlimit:4;stro
+0000d1c0: 6b65 2d64 6173 6861 7272 6179 3a6e 6f6e  ke-dasharray:non
+0000d1d0: 653b 7374 726f 6b65 2d6f 7061 6369 7479  e;stroke-opacity
+0000d1e0: 3a31 2720 2f3e 0d0a 2020 2020 2020 2020  :1' />..        
+0000d1f0: 2020 2020 2020 2020 3c2f 7379 6d62 6f6c          </symbol
+0000d200: 3e0d 0a20 2020 2020 2020 2020 2020 2020  >..             
+0000d210: 2020 203c 7379 6d62 6f6c 2069 643d 276f     <symbol id='o
+0000d220: 7262 3132 3027 3e0d 0a20 2020 2020 2020  rb120'>..       
+0000d230: 2020 2020 2020 2020 2020 2020 203c 7061               <pa
+0000d240: 7468 2064 3d27 4d20 312e 3137 3535 3031  th d='M 1.175501
+0000d250: 312c 392e 3439 3739 3733 2043 2039 2e30  1,9.497973 C 9.0
+0000d260: 3935 3738 3639 2c39 2e34 3937 3937 3320  957869,9.497973 
+0000d270: 392e 3039 3537 3836 392c 392e 3439 3739  9.0957869,9.4979
+0000d280: 3733 2039 2e30 3935 3738 3639 2c39 2e34  73 9.0957869,9.4
+0000d290: 3937 3937 3320 4c20 352e 3133 3536 3433  97973 L 5.135643
+0000d2a0: 382c 312e 3436 3339 3036 3320 4320 352e  8,1.4639063 C 5.
+0000d2b0: 3133 3536 3433 382c 312e 3436 3339 3036  1356438,1.463906
+0000d2c0: 3320 352e 3133 3536 3433 382c 312e 3436  3 5.1356438,1.46
+0000d2d0: 3339 3036 3320 312e 3137 3535 3031 312c  39063 1.1755011,
+0000d2e0: 392e 3439 3739 3733 207a 2720 7374 796c  9.497973 z' styl
+0000d2f0: 653d 2766 696c 6c3a 6e6f 6e65 3b66 696c  e='fill:none;fil
+0000d300: 6c2d 7275 6c65 3a65 7665 6e6f 6464 3b73  l-rule:evenodd;s
+0000d310: 7472 6f6b 653a 2024 6f72 625f 636f 6c6f  troke: $orb_colo
+0000d320: 725f 3132 303b 7374 726f 6b65 2d77 6964  r_120;stroke-wid
+0000d330: 7468 3a31 2e31 3936 3534 3632 3b73 7472  th:1.1965462;str
+0000d340: 6f6b 652d 6c69 6e65 6361 703a 6275 7474  oke-linecap:butt
+0000d350: 3b73 7472 6f6b 652d 6c69 6e65 6a6f 696e  ;stroke-linejoin
+0000d360: 3a6d 6974 6572 3b73 7472 6f6b 652d 6d69  :miter;stroke-mi
+0000d370: 7465 726c 696d 6974 3a34 3b73 7472 6f6b  terlimit:4;strok
+0000d380: 652d 6461 7368 6172 7261 793a 6e6f 6e65  e-dasharray:none
+0000d390: 3b73 7472 6f6b 652d 6f70 6163 6974 793a  ;stroke-opacity:
+0000d3a0: 3127 202f 3e0d 0a20 2020 2020 2020 2020  1' />..         
+0000d3b0: 2020 2020 2020 203c 2f73 796d 626f 6c3e         </symbol>
+0000d3c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000d3d0: 2020 3c73 796d 626f 6c20 6964 3d27 6f72    <symbol id='or
+0000d3e0: 6231 3335 273e 0d0a 2020 2020 2020 2020  b135'>..        
+0000d3f0: 2020 2020 2020 2020 2020 2020 3c70 6174              <pat
+0000d400: 6820 643d 274d 2032 2e32 3338 3835 3832  h d='M 2.2388582
+0000d410: 2c31 2e37 3135 3639 3934 204c 2039 2e32  ,1.7156994 L 9.2
+0000d420: 3933 3831 3534 2c31 2e37 3135 3639 3934  938154,1.7156994
+0000d430: 204c 2039 2e32 3933 3831 3534 2c37 2e37   L 9.2938154,7.7
+0000d440: 3831 3138 3237 204c 2032 2e32 3338 3835  811827 L 2.23885
+0000d450: 3832 2c37 2e37 3831 3138 3237 204c 2032  82,7.7811827 L 2
+0000d460: 2e32 3338 3835 3832 2c31 2e37 3135 3639  .2388582,1.71569
+0000d470: 3934 207a 204d 2036 2e38 3436 3131 3034  94 z M 6.8461104
+0000d480: 2c35 2e35 3733 3432 3637 2043 2036 2e38  ,5.5734267 C 6.8
+0000d490: 3436 3131 3034 2c35 2e35 3733 3432 3637  461104,5.5734267
+0000d4a0: 2036 2e38 3436 3131 3034 2c35 2e35 3733   6.8461104,5.573
+0000d4b0: 3432 3637 2033 2e32 3436 3836 3532 2c31  4267 3.2468652,1
+0000d4c0: 302e 3337 3234 3220 4320 382e 3034 3538  0.37242 C 8.0458
+0000d4d0: 3538 342c 3130 2e33 3732 3432 2038 2e30  584,10.37242 8.0
+0000d4e0: 3435 3835 3834 2c31 302e 3337 3234 3220  458584,10.37242 
+0000d4f0: 382e 3034 3538 3538 342c 3130 2e33 3732  8.0458584,10.372
+0000d500: 3432 2720 7374 796c 653d 2766 696c 6c3a  42' style='fill:
+0000d510: 6e6f 6e65 3b66 696c 6c2d 7275 6c65 3a65  none;fill-rule:e
+0000d520: 7665 6e6f 6464 3b73 7472 6f6b 653a 2024  venodd;stroke: $
+0000d530: 6f72 625f 636f 6c6f 725f 3133 353b 7374  orb_color_135;st
+0000d540: 726f 6b65 2d77 6964 7468 3a31 2e31 3936  roke-width:1.196
+0000d550: 3534 3632 3b73 7472 6f6b 652d 6c69 6e65  5462;stroke-line
+0000d560: 6361 703a 6275 7474 3b73 7472 6f6b 652d  cap:butt;stroke-
+0000d570: 6c69 6e65 6a6f 696e 3a6d 6974 6572 3b73  linejoin:miter;s
+0000d580: 7472 6f6b 652d 6d69 7465 726c 696d 6974  troke-miterlimit
+0000d590: 3a34 3b73 7472 6f6b 652d 6461 7368 6172  :4;stroke-dashar
+0000d5a0: 7261 793a 6e6f 6e65 3b73 7472 6f6b 652d  ray:none;stroke-
+0000d5b0: 6f70 6163 6974 793a 3127 202f 3e0d 0a20  opacity:1' />.. 
+0000d5c0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+0000d5d0: 2f73 796d 626f 6c3e 0d0a 2020 2020 2020  /symbol>..      
+0000d5e0: 2020 2020 2020 2020 2020 3c73 796d 626f            <symbo
+0000d5f0: 6c20 6964 3d27 6f72 6231 3434 273e 0d0a  l id='orb144'>..
+0000d600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d610: 2020 2020 3c70 6174 6820 643d 274d 2031      <path d='M 1
+0000d620: 2e34 3234 3531 3639 2c31 2e32 3936 3835  .4245169,1.29685
+0000d630: 3938 2043 2031 2e34 3234 3531 3639 2c39  98 C 1.4245169,9
+0000d640: 2e36 3736 3331 3239 2031 2e34 3234 3531  .6763129 1.42451
+0000d650: 3639 2c39 2e36 3736 3331 3239 2031 2e34  69,9.6763129 1.4
+0000d660: 3234 3531 3639 2c39 2e36 3736 3331 3239  245169,9.6763129
+0000d670: 204d 2031 2e39 3230 3833 3331 2c35 2e33   M 1.9208331,5.3
+0000d680: 3836 3832 3739 2043 2032 2e37 3732 3238  868279 C 2.77228
+0000d690: 3836 2c35 2e33 3335 3234 3339 2033 2e35  86,5.3352439 3.5
+0000d6a0: 3534 3135 3533 2c35 2e36 3836 3431 3239  541553,5.6864129
+0000d6b0: 2033 2e39 3336 3532 3337 2c36 2e32 3932   3.9365237,6.292
+0000d6c0: 3135 3639 2043 2034 2e33 3138 3839 322c  1569 C 4.318892,
+0000d6d0: 362e 3839 3739 3030 3920 342e 3233 3531  6.8979009 4.2351
+0000d6e0: 3631 342c 372e 3635 3237 3132 3920 332e  614,7.6527129 3.
+0000d6f0: 3732 3036 3632 322c 382e 3233 3830 3938  7206622,8.238098
+0000d700: 3920 4320 332e 3230 3631 3633 322c 382e  9 C 3.2061632,8.
+0000d710: 3832 3334 3834 3920 322e 3335 3035 3130  8234849 2.350510
+0000d720: 312c 392e 3133 3734 3832 3920 312e 3531  1,9.1374829 1.51
+0000d730: 3437 3437 312c 392e 3034 3736 3031 3920  47471,9.0476019 
+0000d740: 4d20 392e 3835 3238 3633 392c 352e 3538  M 9.8528639,5.58
+0000d750: 3531 3234 3920 4320 392e 3835 3330 3434  51249 C 9.853044
+0000d760: 392c 372e 3437 3933 3431 3920 382e 3836  9,7.4793419 8.86
+0000d770: 3439 3639 392c 392e 3031 3530 3537 3920  49699,9.0150579 
+0000d780: 372e 3634 3630 3533 392c 392e 3031 3530  7.6460539,9.0150
+0000d790: 3537 3920 4320 362e 3432 3731 3338 392c  579 C 6.4271389,
+0000d7a0: 392e 3031 3530 3537 3920 352e 3433 3930  9.0150579 5.4390
+0000d7b0: 3632 392c 372e 3437 3933 3431 3920 352e  629,7.4793419 5.
+0000d7c0: 3433 3932 3434 392c 352e 3538 3531 3234  4392449,5.585124
+0000d7d0: 3920 4320 352e 3433 3930 3632 392c 332e  9 C 5.4390629,3.
+0000d7e0: 3639 3039 3038 3820 362e 3432 3731 3338  6909088 6.427138
+0000d7f0: 392c 322e 3135 3531 3932 3820 372e 3634  9,2.1551928 7.64
+0000d800: 3630 3533 392c 322e 3135 3531 3932 3820  60539,2.1551928 
+0000d810: 4320 382e 3836 3439 3639 392c 322e 3135  C 8.8649699,2.15
+0000d820: 3531 3932 3820 392e 3835 3330 3434 392c  51928 9.8530449,
+0000d830: 332e 3639 3039 3038 3820 392e 3835 3238  3.6909088 9.8528
+0000d840: 3633 392c 352e 3538 3531 3234 3920 7a20  639,5.5851249 z 
+0000d850: 4d20 382e 3235 3830 3434 392c 372e 3236  M 8.2580449,7.26
+0000d860: 3237 3935 3920 4320 3130 2e31 3938 3235  27959 C 10.19825
+0000d870: 362c 392e 3938 3033 3637 3920 3130 2e31  6,9.9803679 10.1
+0000d880: 3938 3235 362c 392e 3938 3033 3637 3920  98256,9.9803679 
+0000d890: 3130 2e31 3938 3235 362c 392e 3938 3033  10.198256,9.9803
+0000d8a0: 3637 3927 2073 7479 6c65 3d27 6f70 6163  679' style='opac
+0000d8b0: 6974 793a 313b 6669 6c6c 3a6e 6f6e 653b  ity:1;fill:none;
+0000d8c0: 6669 6c6c 2d6f 7061 6369 7479 3a31 3b66  fill-opacity:1;f
+0000d8d0: 696c 6c2d 7275 6c65 3a6e 6f6e 7a65 726f  ill-rule:nonzero
+0000d8e0: 3b73 7472 6f6b 653a 2024 6f72 625f 636f  ;stroke: $orb_co
+0000d8f0: 6c6f 725f 3134 343b 7374 726f 6b65 2d77  lor_144;stroke-w
+0000d900: 6964 7468 3a31 2e34 3736 3333 3036 343b  idth:1.47633064;
+0000d910: 7374 726f 6b65 2d6c 696e 6563 6170 3a62  stroke-linecap:b
+0000d920: 7574 743b 7374 726f 6b65 2d6c 696e 656a  utt;stroke-linej
+0000d930: 6f69 6e3a 6d69 7465 723b 7374 726f 6b65  oin:miter;stroke
+0000d940: 2d6d 6974 6572 6c69 6d69 743a 343b 7374  -miterlimit:4;st
+0000d950: 726f 6b65 2d64 6173 6861 7272 6179 3a6e  roke-dasharray:n
+0000d960: 6f6e 653b 7374 726f 6b65 2d6f 7061 6369  one;stroke-opaci
+0000d970: 7479 3a31 2720 2f3e 0d0a 2020 2020 2020  ty:1' />..      
+0000d980: 2020 2020 2020 2020 2020 3c2f 7379 6d62            </symb
+0000d990: 6f6c 3e0d 0a20 2020 2020 2020 2020 2020  ol>..           
+0000d9a0: 2020 2020 203c 7379 6d62 6f6c 2069 643d       <symbol id=
+0000d9b0: 276f 7262 3135 3027 3e0d 0a20 2020 2020  'orb150'>..     
+0000d9c0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+0000d9d0: 7061 7468 2064 3d27 4d20 312e 3137 3731  path d='M 1.1771
+0000d9e0: 3437 362c 332e 3833 3635 3532 3220 4320  476,3.8365522 C 
+0000d9f0: 342e 3638 3731 3032 2c33 2e38 3237 3239  4.687102,3.82729
+0000da00: 3336 2038 2e31 3937 3035 3632 2c33 2e38  36 8.1970562,3.8
+0000da10: 3138 3033 3533 2031 312e 3730 3730 3131  180353 11.707011
+0000da20: 2c33 2e38 3038 3737 3637 204d 2031 302e  ,3.8087767 M 10.
+0000da30: 3937 3235 3739 2c39 2e32 3130 3833 3431  972579,9.2108341
+0000da40: 2043 2039 2e33 3339 3830 3032 2c37 2e34   C 9.3398002,7.4
+0000da50: 3936 3431 3631 2037 2e37 3037 3032 3232  964161 7.7070222
+0000da60: 2c35 2e37 3831 3939 3839 2036 2e30 3734  ,5.7819989 6.074
+0000da70: 3234 3334 2c34 2e30 3637 3538 3133 204d  2434,4.0675813 M
+0000da80: 2031 2e36 3635 3734 312c 392e 3231 3038   1.665741,9.2108
+0000da90: 3334 3120 4320 332e 3139 3038 3635 362c  341 C 3.1908656,
+0000daa0: 372e 3339 3939 3831 3120 342e 3731 3539  7.3999811 4.7159
+0000dab0: 3930 342c 352e 3538 3931 3237 3920 362e  904,5.5891279 6.
+0000dac0: 3234 3131 3135 2c33 2e37 3738 3237 3438  241115,3.7782748
+0000dad0: 2720 7374 796c 653d 276f 7061 6369 7479  ' style='opacity
+0000dae0: 3a31 3b66 696c 6c3a 6e6f 6e65 3b66 696c  :1;fill:none;fil
+0000daf0: 6c2d 6f70 6163 6974 793a 313b 6669 6c6c  l-opacity:1;fill
+0000db00: 2d72 756c 653a 6e6f 6e7a 6572 6f3b 7374  -rule:nonzero;st
+0000db10: 726f 6b65 3a20 246f 7262 5f63 6f6c 6f72  roke: $orb_color
+0000db20: 5f31 3530 3b73 7472 6f6b 652d 7769 6474  _150;stroke-widt
+0000db30: 683a 312e 3437 3633 3330 3634 3b73 7472  h:1.47633064;str
+0000db40: 6f6b 652d 6c69 6e65 6361 703a 6275 7474  oke-linecap:butt
+0000db50: 3b73 7472 6f6b 652d 6c69 6e65 6a6f 696e  ;stroke-linejoin
+0000db60: 3a6d 6974 6572 3b73 7472 6f6b 652d 6d69  :miter;stroke-mi
+0000db70: 7465 726c 696d 6974 3a34 3b73 7472 6f6b  terlimit:4;strok
+0000db80: 652d 6461 7368 6172 7261 793a 6e6f 6e65  e-dasharray:none
+0000db90: 3b73 7472 6f6b 652d 6f70 6163 6974 793a  ;stroke-opacity:
+0000dba0: 3127 202f 3e0d 0a20 2020 2020 2020 2020  1' />..         
+0000dbb0: 2020 2020 2020 203c 2f73 796d 626f 6c3e         </symbol>
+0000dbc0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000dbd0: 2020 3c73 796d 626f 6c20 6964 3d27 6f72    <symbol id='or
+0000dbe0: 6231 3830 273e 0d0a 2020 2020 2020 2020  b180'>..        
+0000dbf0: 2020 2020 2020 2020 2020 2020 3c70 6174              <pat
+0000dc00: 6820 643d 274d 2035 2e32 3436 3431 3337  h d='M 5.2464137
+0000dc10: 2c39 2e31 3032 3431 3134 2043 2035 2e32  ,9.1024114 C 5.2
+0000dc20: 3630 3736 3637 2c31 302e 3032 3331 3320  607667,10.02313 
+0000dc30: 342e 3634 3234 3034 372c 3130 2e39 3131  4.6424047,10.911
+0000dc40: 3735 3620 332e 3737 3637 3636 372c 3131  756 3.7767667,11
+0000dc50: 2e32 3233 3733 3520 4320 332e 3030 3433  .223735 C 3.0043
+0000dc60: 3030 372c 3131 2e35 3134 3532 3220 322e  007,11.514522 2.
+0000dc70: 3037 3536 3930 372c 3131 2e33 3435 3731  0756907,11.34571
+0000dc80: 3320 312e 3436 3738 3136 372c 3130 2e37  3 1.4678167,10.7
+0000dc90: 3832 3838 3620 4320 302e 3837 3036 3238  82886 C 0.870628
+0000dca0: 3637 2c31 302e 3234 3734 3620 302e 3539  67,10.24746 0.59
+0000dcb0: 3037 3530 3637 2c39 2e33 3831 3830 3932  075067,9.3818092
+0000dcc0: 2030 2e37 3737 3037 3536 372c 382e 3539   0.77707567,8.59
+0000dcd0: 3935 3631 3420 4320 302e 3935 3837 3238  95614 C 0.958728
+0000dce0: 3637 2c37 2e37 3932 3038 3433 2031 2e36  67,7.7920843 1.6
+0000dcf0: 3132 3535 3537 2c37 2e31 3037 3434 3334  125557,7.1074434
+0000dd00: 2032 2e34 3139 3431 3537 2c36 2e39 3039   2.4194157,6.909
+0000dd10: 3932 3035 2043 2033 2e31 3930 3036 3237  9205 C 3.1900627
+0000dd20: 2c36 2e37 3130 3638 2034 2e30 3632 3133  ,6.71068 4.06213
+0000dd30: 3137 2c36 2e39 3435 3439 3636 2034 2e36  17,6.9454966 4.6
+0000dd40: 3130 3038 3737 2c37 2e35 3238 3130 3538  100877,7.5281058
+0000dd50: 2043 2035 2e30 3132 3935 3537 2c37 2e39   C 5.0129557,7.9
+0000dd60: 3435 3335 3136 2035 2e32 3531 3739 3437  453516 5.2517947
+0000dd70: 2c38 2e35 3231 3031 3934 2035 2e32 3436  ,8.5210194 5.246
+0000dd80: 3431 3337 2c39 2e31 3032 3431 3134 207a  4137,9.1024114 z
+0000dd90: 204d 2031 312e 3234 3634 3134 2c33 2e31   M 11.246414,3.1
+0000dda0: 3032 3431 3239 2043 2031 312e 3236 3037  024129 C 11.2607
+0000ddb0: 3635 2c34 2e30 3233 3133 3137 2031 302e  65,4.0231317 10.
+0000ddc0: 3634 3234 3034 2c34 2e39 3131 3735 3734  642404,4.9117574
+0000ddd0: 2039 2e37 3736 3736 3537 2c35 2e32 3233   9.7767657,5.223
+0000dde0: 3733 3631 2043 2039 2e30 3034 3239 3937  7361 C 9.0042997
+0000ddf0: 2c35 2e35 3134 3532 3338 2038 2e30 3735  ,5.5145238 8.075
+0000de00: 3638 3937 2c35 2e33 3435 3731 3335 2037  6897,5.3457135 7
+0000de10: 2e34 3637 3831 3437 2c34 2e37 3832 3838  .4678147,4.78288
+0000de20: 3733 2043 2036 2e38 3730 3632 3737 2c34  73 C 6.8706277,4
+0000de30: 2e32 3437 3436 3133 2036 2e35 3930 3734  .2474613 6.59074
+0000de40: 3937 2c33 2e33 3831 3831 2036 2e37 3737  97,3.38181 6.777
+0000de50: 3037 3437 2c32 2e35 3939 3536 3234 2043  0747,2.5995624 C
+0000de60: 2036 2e39 3538 3732 3637 2c31 2e37 3932   6.9587267,1.792
+0000de70: 3038 3533 2037 2e36 3132 3535 3437 2c31  0853 7.6125547,1
+0000de80: 2e31 3037 3434 3435 2038 2e34 3139 3431  .1074445 8.41941
+0000de90: 3437 2c30 2e39 3039 3932 3135 2043 2039  47,0.9099215 C 9
+0000dea0: 2e31 3930 3036 3137 2c30 2e37 3130 3638  .1900617,0.71068
+0000deb0: 3132 2031 302e 3036 3231 332c 302e 3934  12 10.06213,0.94
+0000dec0: 3534 3938 3220 3130 2e36 3130 3038 372c  54982 10.610087,
+0000ded0: 312e 3532 3831 3037 3320 4320 3131 2e30  1.5281073 C 11.0
+0000dee0: 3132 3935 352c 312e 3934 3533 3532 3920  12955,1.9453529 
+0000def0: 3131 2e32 3531 3739 342c 322e 3532 3130  11.251794,2.5210
+0000df00: 3230 3620 3131 2e32 3436 3431 342c 332e  206 11.246414,3.
+0000df10: 3130 3234 3132 3920 7a20 4d20 342e 3530  1024129 z M 4.50
+0000df20: 3832 3439 372c 372e 3537 3837 3433 2043  82497,7.578743 C
+0000df30: 2035 2e35 3334 3835 3337 2c36 2e35 3934   5.5348537,6.594
+0000df40: 3532 3236 2036 2e35 3631 3435 3737 2c35  5226 6.5614577,5
+0000df50: 2e36 3130 3330 3232 2037 2e35 3838 3036  .6103022 7.58806
+0000df60: 3137 2c34 2e36 3236 3038 3138 2720 7374  17,4.6260818' st
+0000df70: 796c 653d 276f 7061 6369 7479 3a31 3b66  yle='opacity:1;f
+0000df80: 696c 6c3a 6e6f 6e65 3b66 696c 6c2d 6f70  ill:none;fill-op
+0000df90: 6163 6974 793a 313b 6669 6c6c 2d72 756c  acity:1;fill-rul
+0000dfa0: 653a 6e6f 6e7a 6572 6f3b 7374 726f 6b65  e:nonzero;stroke
+0000dfb0: 3a20 246f 7262 5f63 6f6c 6f72 5f31 3830  : $orb_color_180
+0000dfc0: 3b73 7472 6f6b 652d 7769 6474 683a 312e  ;stroke-width:1.
+0000dfd0: 3437 3633 3330 3634 3b73 7472 6f6b 652d  47633064;stroke-
+0000dfe0: 6c69 6e65 6361 703a 6275 7474 3b73 7472  linecap:butt;str
+0000dff0: 6f6b 652d 6c69 6e65 6a6f 696e 3a6d 6974  oke-linejoin:mit
+0000e000: 6572 3b73 7472 6f6b 652d 6d69 7465 726c  er;stroke-miterl
+0000e010: 696d 6974 3a34 3b73 7472 6f6b 652d 6461  imit:4;stroke-da
+0000e020: 7368 6172 7261 793a 6e6f 6e65 3b73 7472  sharray:none;str
+0000e030: 6f6b 652d 6f70 6163 6974 793a 3127 202f  oke-opacity:1' /
+0000e040: 3e0d 0a20 2020 2020 2020 2020 2020 2020  >..             
+0000e050: 2020 203c 2f73 796d 626f 6c3e 2020 2020     </symbol>    
+0000e060: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+0000e070: 2020 2020 2020 2020 2020 2020 2020 3c21                <!
+0000e080: 2d2d 2072 6574 726f 6772 6164 6520 7379  -- retrograde sy
+0000e090: 6d62 6f6c 2028 3132 7831 3229 202d 2d3e  mbol (12x12) -->
+0000e0a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000e0b0: 2020 3c73 796d 626f 6c20 6964 3d27 7265    <symbol id='re
+0000e0c0: 7472 6f67 7261 6465 273e 0d0a 2020 2020  trograde'>..    
+0000e0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e0e0: 3c70 6174 6820 643d 274d 2035 2e31 3639  <path d='M 5.169
+0000e0f0: 3530 3839 2c30 2e30 3635 3134 3330 3720  5089,0.06514307 
+0000e100: 4320 332e 3735 3937 3938 392c 302e 3231  C 3.7597989,0.21
+0000e110: 3539 3732 3037 2032 2e33 3331 3733 3439  597207 2.3317349
+0000e120: 2c30 2e33 3331 3439 3030 3720 302e 3931  ,0.33149007 0.91
+0000e130: 3335 3831 3931 2c30 2e32 3335 3133 3130  358191,0.2351310
+0000e140: 3720 4320 312e 3534 3930 3332 392c 302e  7 C 1.5490329,0.
+0000e150: 3831 3930 3232 3037 2031 2e34 3032 3438  81902207 1.40248
+0000e160: 3439 2c31 2e37 3130 3030 3131 2031 2e34  49,1.7100011 1.4
+0000e170: 3232 3833 3739 2c32 2e34 3730 3034 3331  228379,2.4700431
+0000e180: 2043 2031 2e34 3137 3431 3539 2c35 2e32   C 1.4174159,5.2
+0000e190: 3137 3434 3831 2031 2e34 3333 3737 3039  174481 1.4337709
+0000e1a0: 2c37 2e39 3635 3237 3331 2031 2e34 3134  ,7.9652731 1.414
+0000e1b0: 3530 3139 2c31 302e 3731 3234 3131 2043  5019,10.712411 C
+0000e1c0: 2031 2e35 3134 3934 3039 2c31 312e 3137   1.5149409,11.17
+0000e1d0: 3038 3438 2030 2e39 3637 3939 3739 312c  0848 0.96799791,
+0000e1e0: 3131 2e38 3334 3437 3120 302e 3930 3238  11.834471 0.9028
+0000e1f0: 3436 3931 2c31 312e 3936 3433 3032 2043  4691,11.964302 C
+0000e200: 2031 2e39 3937 3638 3839 2c31 312e 3936   1.9976889,11.96
+0000e210: 3433 3032 2033 2e30 3932 3532 3939 2c31  4302 3.0925299,1
+0000e220: 312e 3936 3433 3032 2034 2e31 3837 3337  1.964302 4.18737
+0000e230: 3139 2c31 312e 3936 3433 3032 2043 2033  19,11.964302 C 3
+0000e240: 2e36 3031 3834 3339 2c31 312e 3537 3739  .6018439,11.5779
+0000e250: 3735 2033 2e36 3531 3039 3239 2c31 302e  75 3.6510929,10.
+0000e260: 3832 3030 3334 2033 2e36 3431 3733 3939  820034 3.6417399
+0000e270: 2c31 302e 3231 3938 3338 2043 2033 2e36  ,10.219838 C 3.6
+0000e280: 3431 3733 3939 2c38 2e38 3937 3436 3031  417399,8.8974601
+0000e290: 2033 2e36 3431 3733 3939 2c37 2e35 3735   3.6417399,7.575
+0000e2a0: 3038 3331 2033 2e36 3431 3733 3939 2c36  0831 3.6417399,6
+0000e2b0: 2e32 3532 3730 3531 2043 2034 2e35 3032  .2527051 C 4.502
+0000e2c0: 3632 3539 2c37 2e33 3937 3239 3131 2035  6259,7.3972911 5
+0000e2d0: 2e33 3633 3531 3039 2c38 2e35 3431 3837  .3635109,8.54187
+0000e2e0: 3731 2036 2e32 3234 3339 3539 2c39 2e36  71 6.2243959,9.6
+0000e2f0: 3836 3436 3331 2043 2035 2e36 3033 3036  864631 C 5.60306
+0000e300: 3939 2c31 302e 3031 3330 3439 2035 2e30  99,10.013049 5.0
+0000e310: 3732 3134 3339 2c31 302e 3439 3733 3534  721439,10.497354
+0000e320: 2034 2e33 3639 3234 3839 2c31 302e 3637   4.3692489,10.67
+0000e330: 3233 3933 2043 2034 2e35 3735 3337 3639  2393 C 4.5753769
+0000e340: 2c31 302e 3935 3537 3036 2034 2e37 3831  ,10.955706 4.781
+0000e350: 3530 3339 2c31 312e 3233 3930 3220 342e  5039,11.23902 4.
+0000e360: 3938 3736 3331 392c 3131 2e35 3232 3333  9876319,11.52233
+0000e370: 3320 4320 352e 3439 3339 3231 392c 3131  3 C 5.4939219,11
+0000e380: 2e30 3138 3033 3620 362e 3134 3236 3338  .018036 6.142638
+0000e390: 392c 3130 2e36 3732 3231 3820 362e 3733  9,10.672218 6.73
+0000e3a0: 3336 3532 392c 3130 2e32 3634 3432 3120  36529,10.264421 
+0000e3b0: 4320 372e 3338 3937 3033 392c 3131 2e32  C 7.3897039,11.2
+0000e3c0: 3136 3931 3220 382e 3436 3937 3437 392c  16912 8.4697479,
+0000e3d0: 3132 2e30 3438 3339 3220 392e 3734 3139  12.048392 9.7419
+0000e3e0: 3339 392c 3132 2e30 3131 3537 3920 4320  399,12.011579 C 
+0000e3f0: 3130 2e31 3433 3630 332c 3132 2e30 3032  10.143603,12.002
+0000e400: 3139 3920 3131 2e30 3637 3639 312c 3131  199 11.067691,11
+0000e410: 2e38 3835 3832 3420 3131 2e30 3633 3737  .885824 11.06377
+0000e420: 352c 3131 2e36 3736 3037 3520 4320 392e  5,11.676075 C 9.
+0000e430: 3930 3034 3936 392c 3131 2e31 3238 3035  9004969,11.12805
+0000e440: 3420 392e 3030 3138 3834 392c 3130 2e31  4 9.0018849,10.1
+0000e450: 3739 3038 3520 382e 3430 3639 3232 392c  79085 8.4069229,
+0000e460: 392e 3130 3835 3034 3120 4320 382e 3936  9.1085041 C 8.96
+0000e470: 3730 3433 392c 382e 3637 3536 3634 3120  70439,8.6756641 
+0000e480: 392e 3530 3536 3238 392c 382e 3138 3730  9.5056289,8.1870
+0000e490: 3035 3120 3130 2e31 3737 3338 322c 372e  051 10.177382,7.
+0000e4a0: 3930 3836 3733 3120 4320 3130 2e34 3139  9086731 C 10.419
+0000e4b0: 3838 312c 372e 3836 3631 3530 3120 3130  881,7.8661501 10
+0000e4c0: 2e30 3331 3636 382c 372e 3537 3633 3537  .031668,7.576357
+0000e4d0: 3120 392e 3938 3135 3033 392c 372e 3431  1 9.9815039,7.41
+0000e4e0: 3930 3935 3120 4320 392e 3738 3936 3038  90951 C 9.789608
+0000e4f0: 392c 362e 3930 3632 3933 3120 392e 3632  9,6.9062931 9.62
+0000e500: 3134 3337 392c 372e 3436 3934 3636 3120  14379,7.4694661 
+0000e510: 392e 3239 3530 3833 392c 372e 3632 3339  9.2950839,7.6239
+0000e520: 3435 3120 4320 382e 3834 3533 3938 392c  451 C 8.8453989,
+0000e530: 372e 3839 3237 3638 3120 382e 3330 3738  7.8927681 8.3078
+0000e540: 3833 392c 382e 3336 3436 3031 3120 372e  839,8.3646011 7.
+0000e550: 3836 3134 3435 392c 382e 3434 3534 3335  8614459,8.445435
+0000e560: 3120 4320 372e 3235 3531 3336 392c 372e  1 C 7.2551369,7.
+0000e570: 3538 3938 3637 3120 362e 3634 3838 3237  5898671 6.648827
+0000e580: 392c 362e 3733 3432 3939 3120 362e 3034  9,6.7342991 6.04
+0000e590: 3235 3139 392c 352e 3837 3837 3332 3120  25199,5.8787321 
+0000e5a0: 4320 372e 3234 3531 3933 392c 352e 3631  C 7.2451939,5.61
+0000e5b0: 3734 3335 3120 382e 3538 3237 3833 392c  74351 8.5827839,
+0000e5c0: 352e 3038 3533 3839 3120 392e 3037 3034  5.0853891 9.0704
+0000e5d0: 3430 392c 332e 3933 3638 3938 3120 4320  409,3.9368981 C 
+0000e5e0: 392e 3430 3633 3133 392c 332e 3131 3230  9.4063139,3.1120
+0000e5f0: 3231 3120 392e 3236 3337 3333 392c 322e  211 9.2637339,2.
+0000e600: 3136 3637 3933 3120 382e 3931 3037 3838  1667931 8.910788
+0000e610: 392c 312e 3337 3334 3730 3120 4320 382e  9,1.3734701 C 8.
+0000e620: 3136 3834 3836 392c 302e 3431 3039 3131  1684869,0.410911
+0000e630: 3037 2036 2e38 3639 3230 3439 2c2d 302e  07 6.8692049,-0.
+0000e640: 3037 3234 3531 3933 3120 352e 3631 3939  072451931 5.6199
+0000e650: 3732 392c 302e 3032 3531 3036 3037 2043  729,0.02510607 C
+0000e660: 2035 2e34 3639 3332 3739 2c30 2e30 3332   5.4693279,0.032
+0000e670: 3837 3230 3720 352e 3331 3930 3531 392c  87207 5.3190519,
+0000e680: 302e 3034 3635 3130 3037 2035 2e31 3639  0.04651007 5.169
+0000e690: 3530 3839 2c30 2e30 3635 3134 3330 3720  5089,0.06514307 
+0000e6a0: 4c20 352e 3136 3935 3038 392c 302e 3036  L 5.1695089,0.06
+0000e6b0: 3531 3433 3037 207a 204d 2034 2e30 3035  514307 z M 4.005
+0000e6c0: 3439 3439 2c30 2e39 3833 3037 3830 3620  4949,0.98307806 
+0000e6d0: 4320 342e 3932 3734 3230 392c 302e 3837  C 4.9274209,0.87
+0000e6e0: 3531 3630 3037 2036 2e30 3735 3238 3339  516007 6.0752839
+0000e6f0: 2c30 2e39 3536 3539 3430 3620 362e 3631  ,0.95659406 6.61
+0000e700: 3139 3436 392c 312e 3737 3639 3832 3120  19469,1.7769821 
+0000e710: 4320 372e 3139 3935 3438 392c 322e 3734  C 7.1995489,2.74
+0000e720: 3336 3233 3120 362e 3937 3731 3737 392c  36231 6.9771779,
+0000e730: 342e 3032 3737 3234 3120 362e 3233 3838  4.0277241 6.2388
+0000e740: 3835 392c 342e 3836 3934 3030 3120 4320  859,4.8694001 C 
+0000e750: 352e 3630 3533 3238 392c 352e 3535 3439  5.6053289,5.5549
+0000e760: 3033 3120 342e 3535 3231 3035 392c 352e  031 4.5521059,5.
+0000e770: 3637 3830 3737 3120 332e 3634 3137 3339  6780771 3.641739
+0000e780: 392c 352e 3537 3237 3533 3120 4320 332e  9,5.5727531 C 3.
+0000e790: 3634 3137 3339 392c 342e 3036 3535 3237  6417399,4.065527
+0000e7a0: 3120 332e 3634 3137 3339 392c 322e 3535  1 3.6417399,2.55
+0000e7b0: 3833 3030 3120 332e 3634 3137 3339 392c  83001 3.6417399,
+0000e7c0: 312e 3035 3130 3733 3120 4320 332e 3736  1.0510731 C 3.76
+0000e7d0: 3239 3931 392c 312e 3032 3834 3038 3120  29919,1.0284081 
+0000e7e0: 332e 3838 3432 3432 392c 312e 3030 3537  3.8842429,1.0057
+0000e7f0: 3433 3120 342e 3030 3534 3934 392c 302e  431 4.0054949,0.
+0000e800: 3938 3330 3738 3036 207a 2720 7374 796c  98307806 z' styl
+0000e810: 653d 2766 696c 6c3a 2470 6170 6572 5f63  e='fill:$paper_c
+0000e820: 6f6c 6f72 5f30 3b27 202f 3e0d 0a20 2020  olor_0;' />..   
+0000e830: 2020 2020 2020 2020 2020 2020 203c 2f73               </s
+0000e840: 796d 626f 6c3e 0d0a 2020 2020 2020 2020  ymbol>..        
+0000e850: 2020 2020 2020 2020 3c67 2074 7261 6e73          <g trans
+0000e860: 666f 726d 3d27 7472 616e 736c 6174 6528  form='translate(
+0000e870: 3530 2c35 3029 273e 0d0a 2020 2020 2020  50,50)'>..      
+0000e880: 2020 2020 2020 2020 2020 2020 2020 3c67                <g
+0000e890: 2074 7261 6e73 666f 726d 3d27 7472 616e   transform='tran
+0000e8a0: 736c 6174 6528 2463 6972 636c 6558 2c24  slate($circleX,$
+0000e8b0: 6369 7263 6c65 5929 273e 2020 2020 2020  circleY)'>      
+0000e8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e8d0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+0000e8e0: 2020 2020 2020 2020 2020 2020 3c21 2d2d              <!--
+0000e8f0: 205a 6f64 6961 6320 2d2d 3e0d 0a20 2020   Zodiac -->..   
+0000e900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e910: 2020 2020 2024 6d61 6b65 5a6f 6469 6163       $makeZodiac
+0000e920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e930: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+0000e940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e950: 2020 3c21 2d2d 2046 6972 7374 2043 6972    <!-- First Cir
+0000e960: 636c 6520 2d2d 3e0d 0a20 2020 2020 2020  cle -->..       
+0000e970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e980: 203c 6369 7263 6c65 2024 6331 2073 7479   <circle $c1 sty
+0000e990: 6c65 3d27 2463 3173 7479 6c65 2720 2f3e  le='$c1style' />
+0000e9a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000e9b0: 2020 2020 2020 2020 2020 3c21 2d2d 2053            <!-- S
+0000e9c0: 6563 6f6e 6420 4369 7263 6c65 202d 2d3e  econd Circle -->
+0000e9d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000e9e0: 2020 2020 2020 2020 2020 3c63 6972 636c            <circl
+0000e9f0: 6520 2463 3220 7374 796c 653d 2724 6332  e $c2 style='$c2
+0000ea00: 7374 796c 6527 202f 3e0d 0a20 2020 2020  style' />..     
 0000ea10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ea20: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-0000ea30: 2020 2020 2020 2020 2020 2020 3c21 2d2d              <!--
-0000ea40: 205a 6f64 6961 6320 2d2d 3e0d 0a20 2020   Zodiac -->..   
-0000ea50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ea60: 2020 2020 2024 6d61 6b65 5a6f 6469 6163       $makeZodiac
-0000ea70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ea80: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-0000ea90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eaa0: 2020 3c21 2d2d 2046 6972 7374 2043 6972    <!-- First Cir
-0000eab0: 636c 6520 2d2d 3e0d 0a20 2020 2020 2020  cle -->..       
-0000eac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ead0: 203c 6369 7263 6c65 2024 6331 2073 7479   <circle $c1 sty
-0000eae0: 6c65 3d27 2463 3173 7479 6c65 2720 2f3e  le='$c1style' />
-0000eaf0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000eb00: 2020 2020 2020 2020 2020 3c21 2d2d 2053            <!-- S
-0000eb10: 6563 6f6e 6420 4369 7263 6c65 202d 2d3e  econd Circle -->
-0000eb20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000eb30: 2020 2020 2020 2020 2020 3c63 6972 636c            <circl
-0000eb40: 6520 2463 3220 7374 796c 653d 2724 6332  e $c2 style='$c2
-0000eb50: 7374 796c 6527 202f 3e0d 0a20 2020 2020  style' />..     
-0000eb60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eb70: 2020 203c 212d 2d20 5468 6972 6420 4369     <!-- Third Ci
-0000eb80: 7263 6c65 202d 2d3e 0d0a 2020 2020 2020  rcle -->..      
+0000ea20: 2020 203c 212d 2d20 5468 6972 6420 4369     <!-- Third Ci
+0000ea30: 7263 6c65 202d 2d3e 0d0a 2020 2020 2020  rcle -->..      
+0000ea40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ea50: 2020 3c63 6972 636c 6520 2463 3320 7374    <circle $c3 st
+0000ea60: 796c 653d 2724 6333 7374 796c 6527 202f  yle='$c3style' /
+0000ea70: 3e0d 0a20 2020 2020 2020 2020 2020 2020  >..             
+0000ea80: 2020 2020 2020 2020 2020 203c 212d 2d20             <!-- 
+0000ea90: 5472 616e 7369 7452 696e 6720 2d2d 3e24  TransitRing -->$
+0000eaa0: 7472 616e 7369 7452 696e 6720 2020 2020  transitRing     
+0000eab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eac0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+0000ead0: 2020 2020 2020 2020 2020 2020 203c 212d               <!-
+0000eae0: 2d20 486f 7573 6573 202d 2d3e 246d 616b  - Houses -->$mak
+0000eaf0: 6548 6f75 7365 730d 0a20 2020 2020 2020  eHouses..       
+0000eb00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eb10: 203c 212d 2d20 4178 6973 202d 2d3e 246d   <!-- Axis -->$m
+0000eb20: 616b 6541 7869 7320 2020 2020 2020 2020  akeAxis         
+0000eb30: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+0000eb40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000eb50: 2020 2020 2020 2020 203c 212d 2d20 506c           <!-- Pl
+0000eb60: 616e 6574 7320 2d2d 3e24 6d61 6b65 506c  anets -->$makePl
+0000eb70: 616e 6574 7320 2020 2020 2020 2020 2020  anets           
+0000eb80: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
 0000eb90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eba0: 2020 3c63 6972 636c 6520 2463 3320 7374    <circle $c3 st
-0000ebb0: 796c 653d 2724 6333 7374 796c 6527 202f  yle='$c3style' /
-0000ebc0: 3e0d 0a20 2020 2020 2020 2020 2020 2020  >..             
-0000ebd0: 2020 2020 2020 2020 2020 203c 212d 2d20             <!-- 
-0000ebe0: 5472 616e 7369 7452 696e 6720 2d2d 3e24  TransitRing -->$
-0000ebf0: 7472 616e 7369 7452 696e 6720 2020 2020  transitRing     
-0000ec00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ec10: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+0000eba0: 2020 2020 2020 203c 212d 2d20 4173 7065         <!-- Aspe
+0000ebb0: 6374 7320 2d2d 3e24 6d61 6b65 4173 7065  cts -->$makeAspe
+0000ebc0: 6374 7320 2020 2020 2020 2020 2020 2020  cts             
+0000ebd0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+0000ebe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ebf0: 203c 2f67 3e0d 0a20 2020 2020 2020 2020   </g>..         
+0000ec00: 2020 2020 2020 203c 2f67 3e20 2020 2020         </g>     
+0000ec10: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
 0000ec20: 2020 2020 2020 2020 2020 2020 203c 212d               <!-
-0000ec30: 2d20 4465 6772 6565 2052 696e 6720 2d2d  - Degree Ring --
-0000ec40: 3e24 6465 6772 6565 5269 6e67 2020 2020  >$degreeRing    
-0000ec50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ec60: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-0000ec70: 2020 2020 2020 2020 2020 2020 2020 3c21                <!
-0000ec80: 2d2d 2048 6f75 7365 7320 2d2d 3e24 6d61  -- Houses -->$ma
-0000ec90: 6b65 486f 7573 6573 0d0a 2020 2020 2020  keHouses..      
-0000eca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ecb0: 2020 3c21 2d2d 2041 7869 7320 2d2d 3e24    <!-- Axis -->$
-0000ecc0: 6d61 6b65 4178 6973 2020 2020 2020 2020  makeAxis        
-0000ecd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ece0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000ecf0: 2020 2020 2020 2020 2020 3c21 2d2d 2050            <!-- P
-0000ed00: 6c61 6e65 7473 202d 2d3e 246d 616b 6550  lanets -->$makeP
-0000ed10: 6c61 6e65 7473 2020 2020 2020 2020 2020  lanets          
-0000ed20: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-0000ed30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ed40: 2020 2020 2020 2020 3c21 2d2d 2041 7370          <!-- Asp
-0000ed50: 6563 7473 202d 2d3e 246d 616b 6541 7370  ects -->$makeAsp
-0000ed60: 6563 7473 2020 2020 2020 2020 2020 2020  ects            
-0000ed70: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-0000ed80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ed90: 2020 3c2f 673e 0d0a 2020 2020 2020 2020    </g>..        
-0000eda0: 2020 2020 2020 2020 3c2f 673e 2020 2020          </g>    
-0000edb0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-0000edc0: 2020 2020 2020 2020 2020 2020 2020 3c21                <!
-0000edd0: 2d2d 2074 6573 7469 6e67 2070 7269 6e74  -- testing print
-0000ede0: 6572 202d 2d3e 0d0a 2020 2020 2020 2020  er -->..        
-0000edf0: 2020 2020 2020 2020 3c21 2d2d 203c 7265          <!-- <re
-0000ee00: 6374 2078 3d27 3027 2079 3d27 3027 2077  ct x='0' y='0' w
-0000ee10: 6964 7468 3d27 3737 322e 3227 2068 6569  idth='772.2' hei
-0000ee20: 6768 743d 2735 3436 2e30 2720 7374 796c  ght='546.0' styl
-0000ee30: 653d 2766 696c 6c3a 2024 7061 7065 725f  e='fill: $paper_
-0000ee40: 636f 6c6f 725f 313b 2073 7472 6f6b 652d  color_1; stroke-
-0000ee50: 7769 6474 683a 2031 7078 3b20 7374 726f  width: 1px; stro
-0000ee60: 6b65 3a72 6564 3b27 202f 3e3c 6c69 6e65  ke:red;' /><line
-0000ee70: 2078 313d 2730 2720 7931 3d27 3027 2078   x1='0' y1='0' x
-0000ee80: 323d 2737 3732 2e32 2720 7932 3d27 3534  2='772.2' y2='54
-0000ee90: 362e 3027 2073 7479 6c65 3d27 6669 6c6c  6.0' style='fill
-0000eea0: 3a6e 6f6e 653b 2073 7472 6f6b 652d 7769  :none; stroke-wi
-0000eeb0: 6474 683a 2031 7078 3b20 7374 726f 6b65  dth: 1px; stroke
-0000eec0: 3a72 6564 3b27 202f 3e3c 6c69 6e65 2078  :red;' /><line x
-0000eed0: 313d 2737 3732 2e32 2720 7931 3d27 3027  1='772.2' y1='0'
-0000eee0: 2078 323d 2730 2720 7932 3d27 3534 362e   x2='0' y2='546.
-0000eef0: 3027 2073 7479 6c65 3d27 6669 6c6c 3a6e  0' style='fill:n
-0000ef00: 6f6e 653b 2073 7472 6f6b 652d 7769 6474  one; stroke-widt
-0000ef10: 683a 2031 7078 3b20 7374 726f 6b65 3a72  h: 1px; stroke:r
-0000ef20: 6564 3b27 202f 3e2d 2d3e 0d0a 2020 2020  ed;' />-->..    
-0000ef30: 2020 2020 2020 2020 3c2f 673e 0d0a 2020          </g>..  
-0000ef40: 2020 2020 2020 3c2f 673e 0d0a 2020 2020        </g>..    
-0000ef50: 3c2f 673e 2020 2020 0d0a 2020 2020 3c21  </g>    ..    <!
-0000ef60: 2d2d 2074 6573 7469 6e67 2070 7269 6e74  -- testing print
-0000ef70: 6572 3c72 6563 7420 783d 2730 2720 793d  er<rect x='0' y=
-0000ef80: 2730 2720 7769 6474 683d 2724 7376 6757  '0' width='$svgW
-0000ef90: 6964 7468 2720 6865 6967 6874 3d27 2473  idth' height='$s
-0000efa0: 7667 4865 6967 6874 2720 7374 796c 653d  vgHeight' style=
-0000efb0: 2766 696c 6c3a 6e6f 6e65 3b20 7374 726f  'fill:none; stro
-0000efc0: 6b65 2d77 6964 7468 3a20 3170 783b 2073  ke-width: 1px; s
-0000efd0: 7472 6f6b 653a 626c 7565 3b27 202f 3e3c  troke:blue;' /><
-0000efe0: 6c69 6e65 2078 313d 2730 2720 7931 3d27  line x1='0' y1='
-0000eff0: 3027 2078 323d 2724 7376 6757 6964 7468  0' x2='$svgWidth
-0000f000: 2720 7932 3d27 2473 7667 4865 6967 6874  ' y2='$svgHeight
-0000f010: 2720 7374 796c 653d 2766 696c 6c3a 6e6f  ' style='fill:no
-0000f020: 6e65 3b20 7374 726f 6b65 2d77 6964 7468  ne; stroke-width
-0000f030: 3a20 3170 783b 2073 7472 6f6b 653a 626c  : 1px; stroke:bl
-0000f040: 7565 3b27 202f 3e3c 6c69 6e65 2078 313d  ue;' /><line x1=
-0000f050: 2724 7376 6757 6964 7468 2720 7931 3d27  '$svgWidth' y1='
-0000f060: 3027 2078 323d 2730 2720 7932 3d27 2473  0' x2='0' y2='$s
-0000f070: 7667 4865 6967 6874 2720 7374 796c 653d  vgHeight' style=
-0000f080: 2766 696c 6c3a 6e6f 6e65 3b20 7374 726f  'fill:none; stro
-0000f090: 6b65 2d77 6964 7468 3a20 3170 783b 2073  ke-width: 1px; s
-0000f0a0: 7472 6f6b 653a 626c 7565 3b27 202f 3e2d  troke:blue;' />-
-0000f0b0: 2d3e 3c2f 7376 673e                      -></svg>
+0000ec30: 2d20 7465 7374 696e 6720 7072 696e 7465  - testing printe
+0000ec40: 7220 2d2d 3e0d 0a20 2020 2020 2020 2020  r -->..         
+0000ec50: 2020 2020 2020 203c 212d 2d20 3c72 6563         <!-- <rec
+0000ec60: 7420 783d 2730 2720 793d 2730 2720 7769  t x='0' y='0' wi
+0000ec70: 6474 683d 2737 3732 2e32 2720 6865 6967  dth='772.2' heig
+0000ec80: 6874 3d27 3534 362e 3027 2073 7479 6c65  ht='546.0' style
+0000ec90: 3d27 6669 6c6c 3a20 2470 6170 6572 5f63  ='fill: $paper_c
+0000eca0: 6f6c 6f72 5f31 3b20 7374 726f 6b65 2d77  olor_1; stroke-w
+0000ecb0: 6964 7468 3a20 3170 783b 2073 7472 6f6b  idth: 1px; strok
+0000ecc0: 653a 7265 643b 2720 2f3e 3c6c 696e 6520  e:red;' /><line 
+0000ecd0: 7831 3d27 3027 2079 313d 2730 2720 7832  x1='0' y1='0' x2
+0000ece0: 3d27 3737 322e 3227 2079 323d 2735 3436  ='772.2' y2='546
+0000ecf0: 2e30 2720 7374 796c 653d 2766 696c 6c3a  .0' style='fill:
+0000ed00: 6e6f 6e65 3b20 7374 726f 6b65 2d77 6964  none; stroke-wid
+0000ed10: 7468 3a20 3170 783b 2073 7472 6f6b 653a  th: 1px; stroke:
+0000ed20: 7265 643b 2720 2f3e 3c6c 696e 6520 7831  red;' /><line x1
+0000ed30: 3d27 3737 322e 3227 2079 313d 2730 2720  ='772.2' y1='0' 
+0000ed40: 7832 3d27 3027 2079 323d 2735 3436 2e30  x2='0' y2='546.0
+0000ed50: 2720 7374 796c 653d 2766 696c 6c3a 6e6f  ' style='fill:no
+0000ed60: 6e65 3b20 7374 726f 6b65 2d77 6964 7468  ne; stroke-width
+0000ed70: 3a20 3170 783b 2073 7472 6f6b 653a 7265  : 1px; stroke:re
+0000ed80: 643b 2720 2f3e 2d2d 3e0d 0a20 2020 2020  d;' />-->..     
+0000ed90: 2020 2020 2020 203c 2f67 3e0d 0a20 2020         </g>..   
+0000eda0: 2020 2020 203c 2f67 3e0d 0a20 2020 203c       </g>..    <
+0000edb0: 2f67 3e20 2020 200d 0a20 2020 203c 212d  /g>    ..    <!-
+0000edc0: 2d20 7465 7374 696e 6720 7072 696e 7465  - testing printe
+0000edd0: 723c 7265 6374 2078 3d27 3027 2079 3d27  r<rect x='0' y='
+0000ede0: 3027 2077 6964 7468 3d27 2473 7667 5769  0' width='$svgWi
+0000edf0: 6474 6827 2068 6569 6768 743d 2724 7376  dth' height='$sv
+0000ee00: 6748 6569 6768 7427 2073 7479 6c65 3d27  gHeight' style='
+0000ee10: 6669 6c6c 3a6e 6f6e 653b 2073 7472 6f6b  fill:none; strok
+0000ee20: 652d 7769 6474 683a 2031 7078 3b20 7374  e-width: 1px; st
+0000ee30: 726f 6b65 3a62 6c75 653b 2720 2f3e 3c6c  roke:blue;' /><l
+0000ee40: 696e 6520 7831 3d27 3027 2079 313d 2730  ine x1='0' y1='0
+0000ee50: 2720 7832 3d27 2473 7667 5769 6474 6827  ' x2='$svgWidth'
+0000ee60: 2079 323d 2724 7376 6748 6569 6768 7427   y2='$svgHeight'
+0000ee70: 2073 7479 6c65 3d27 6669 6c6c 3a6e 6f6e   style='fill:non
+0000ee80: 653b 2073 7472 6f6b 652d 7769 6474 683a  e; stroke-width:
+0000ee90: 2031 7078 3b20 7374 726f 6b65 3a62 6c75   1px; stroke:blu
+0000eea0: 653b 2720 2f3e 3c6c 696e 6520 7831 3d27  e;' /><line x1='
+0000eeb0: 2473 7667 5769 6474 6827 2079 313d 2730  $svgWidth' y1='0
+0000eec0: 2720 7832 3d27 3027 2079 323d 2724 7376  ' x2='0' y2='$sv
+0000eed0: 6748 6569 6768 7427 2073 7479 6c65 3d27  gHeight' style='
+0000eee0: 6669 6c6c 3a6e 6f6e 653b 2073 7472 6f6b  fill:none; strok
+0000eef0: 652d 7769 6474 683a 2031 7078 3b20 7374  e-width: 1px; st
+0000ef00: 726f 6b65 3a62 6c75 653b 2720 2f3e 2d2d  roke:blue;' />--
+0000ef10: 3e3c 2f73 7667 3e                        ></svg>
```

### Comparing `py_astrolab-0.2.0/py_astrolab/charts/wonderful_mistake.py` & `py_astrolab-0.2.1/py_astrolab/charts/wonderful_mistake.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.2.0/py_astrolab/fetch_geonames.py` & `py_astrolab-0.2.1/py_astrolab/fetch_geonames.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.2.0/py_astrolab/kr.config.json` & `py_astrolab-0.2.1/py_astrolab/kr.config.json`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.2.0/py_astrolab/main.py` & `py_astrolab-0.2.1/py_astrolab/main.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.2.0/py_astrolab/print_all_data.py` & `py_astrolab-0.2.1/py_astrolab/print_all_data.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.2.0/py_astrolab/relationship_score.py` & `py_astrolab-0.2.1/py_astrolab/relationship_score.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.2.0/py_astrolab/report.py` & `py_astrolab-0.2.1/py_astrolab/report.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.2.0/py_astrolab/types.py` & `py_astrolab-0.2.1/py_astrolab/types.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.2.0/py_astrolab/utilities.py` & `py_astrolab-0.2.1/py_astrolab/utilities.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.2.0/pyproject.toml` & `py_astrolab-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-astrolab"
-version = "0.2.0"
+version = "0.2.1"
 description = "A Python interface on Swiss Ephemeris to perform astrological calculations"
 authors = ["Giacomo Battaglia <battaglia.giacomo@yahoo.it>", "Arcangelo Massari <arcangelomas@gmail.com>"]
 license = "GNU General Public License (GPL)"
 readme = "README.md"
 packages = [{include = "py_astrolab"}]
 
 [tool.poetry.dependencies]
```

### Comparing `py_astrolab-0.2.0/PKG-INFO` & `py_astrolab-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-astrolab
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Python interface on Swiss Ephemeris to perform astrological calculations
 License: GNU General Public License (GPL)
 Author: Giacomo Battaglia
 Author-email: battaglia.giacomo@yahoo.it
 Requires-Python: >=3.9,<3.10
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

