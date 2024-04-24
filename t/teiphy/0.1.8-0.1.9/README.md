# Comparing `tmp/teiphy-0.1.8.tar.gz` & `tmp/teiphy-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teiphy-0.1.8.tar", max compression
+gzip compressed data, was "teiphy-0.1.9.tar", max compression
```

## Comparing `teiphy-0.1.8.tar` & `teiphy-0.1.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1070 2023-12-23 02:52:33.594553 teiphy-0.1.8/LICENSE
--rw-r--r--   0        0        0     6698 2023-12-23 02:52:33.594553 teiphy-0.1.8/README.rst
--rw-r--r--   0        0        0     1578 2023-12-23 02:52:33.598553 teiphy-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      195 2023-12-23 02:52:33.598553 teiphy-0.1.8/teiphy/__init__.py
--rw-r--r--   0        0        0   121138 2023-12-23 02:52:33.598553 teiphy-0.1.8/teiphy/collation.py
--rw-r--r--   0        0        0      134 2023-12-23 02:52:33.598553 teiphy-0.1.8/teiphy/common.py
--rw-r--r--   0        0        0     1085 2023-12-23 02:52:33.598553 teiphy-0.1.8/teiphy/format.py
--rw-r--r--   0        0        0     7047 2023-12-23 02:52:33.598553 teiphy-0.1.8/teiphy/main.py
--rw-r--r--   0        0        0    12734 2023-12-23 02:52:33.598553 teiphy-0.1.8/teiphy/reading.py
--rw-r--r--   0        0        0    18746 2023-12-23 02:52:33.598553 teiphy-0.1.8/teiphy/templates/beast_template.xml
--rw-r--r--   0        0        0     7939 2023-12-23 02:52:33.598553 teiphy-0.1.8/teiphy/variation_unit.py
--rw-r--r--   0        0        0     3034 2023-12-23 02:52:33.598553 teiphy-0.1.8/teiphy/witness.py
--rw-r--r--   0        0        0     8006 1970-01-01 00:00:00.000000 teiphy-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-03-08 04:49:44.857281 teiphy-0.1.9/LICENSE
+-rw-r--r--   0        0        0     6698 2024-03-08 04:49:44.857281 teiphy-0.1.9/README.rst
+-rw-r--r--   0        0        0     1578 2024-03-08 04:49:44.861281 teiphy-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      195 2024-03-08 04:49:44.861281 teiphy-0.1.9/teiphy/__init__.py
+-rw-r--r--   0        0        0   121138 2024-03-08 04:49:44.861281 teiphy-0.1.9/teiphy/collation.py
+-rw-r--r--   0        0        0      134 2024-03-08 04:49:44.861281 teiphy-0.1.9/teiphy/common.py
+-rw-r--r--   0        0        0     1085 2024-03-08 04:49:44.861281 teiphy-0.1.9/teiphy/format.py
+-rw-r--r--   0        0        0     7047 2024-03-08 04:49:44.861281 teiphy-0.1.9/teiphy/main.py
+-rw-r--r--   0        0        0    12734 2024-03-08 04:49:44.861281 teiphy-0.1.9/teiphy/reading.py
+-rw-r--r--   0        0        0    19623 2024-03-08 04:49:44.861281 teiphy-0.1.9/teiphy/templates/beast_template.xml
+-rw-r--r--   0        0        0     7939 2024-03-08 04:49:44.861281 teiphy-0.1.9/teiphy/variation_unit.py
+-rw-r--r--   0        0        0     3034 2024-03-08 04:49:44.861281 teiphy-0.1.9/teiphy/witness.py
+-rw-r--r--   0        0        0     8006 1970-01-01 00:00:00.000000 teiphy-0.1.9/PKG-INFO
```

### Comparing `teiphy-0.1.8/LICENSE` & `teiphy-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `teiphy-0.1.8/README.rst` & `teiphy-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `teiphy-0.1.8/pyproject.toml` & `teiphy-0.1.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "teiphy"
-version = "0.1.8"
+version = "0.1.9"
 description = "Converts TEI XML collations to NEXUS and other formats"
 authors = ["Joey McCollum and Robert Turnbull"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/jjmccollum/teiphy"
 repository = "https://github.com/jjmccollum/teiphy"
 documentation = "https://jjmccollum.github.io/teiphy/"
@@ -19,15 +19,15 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 
 
 [tool.poetry.dependencies]
 python = "^3.8"
-lxml = "^4.9.1"
+lxml = "^4.9.3"
 numpy = "^1.23.2"
 pandas = "^1.4.4"
 openpyxl = "^3.0.10"
 typer = "^0.6.1"
 rich = "^12.5.1"
 python-slugify = "^6.1.2"
 Jinja2 = "^3.1.2"
```

### Comparing `teiphy-0.1.8/teiphy/collation.py` & `teiphy-0.1.9/teiphy/collation.py`

 * *Files identical despite different names*

### Comparing `teiphy-0.1.8/teiphy/format.py` & `teiphy-0.1.9/teiphy/format.py`

 * *Files identical despite different names*

### Comparing `teiphy-0.1.8/teiphy/main.py` & `teiphy-0.1.9/teiphy/main.py`

 * *Files identical despite different names*

### Comparing `teiphy-0.1.8/teiphy/reading.py` & `teiphy-0.1.9/teiphy/reading.py`

 * *Files identical despite different names*

### Comparing `teiphy-0.1.8/teiphy/templates/beast_template.xml` & `teiphy-0.1.9/teiphy/templates/beast_template.xml`

 * *Files 4% similar despite different names*

#### Comparing `teiphy-0.1.8/teiphy/templates/beast_template.xml` & `teiphy-0.1.9/teiphy/templates/beast_template.xml`

```diff
@@ -16,16 +16,20 @@
     <trait spec="TraitSet" traitname="date" units="year" value="{{ date_map }}">
       <taxa spec="TaxonSet" id="taxa" alignment="@alignment"/>
     </trait>
     <taxonset spec="TaxonSet" idref="taxa"/>
   </tree>
   <birthDeathSkylineModel spec="bdsky.evolution.speciation.BirthDeathSkylineModel" id="birthDeath" tree="@tree">
     {%- if origin_span[1] %}
-    <origin spec="parameter.RealParameter" id="origin" lower="{{ origin_span[0] }}" upper="{{ origin_span[1] }}" value="{{ origin_span[1] }}"/>
+        {%- if origin_span[1] == origin_span[0] %}
+    <origin spec="parameter.RealParameter" id="origin" lower="{{ origin_span[0] }}" upper="{{ origin_span[1] }}" value="{{ origin_span[1] }}" estimate="false"/>
     {%- else %}
+    <origin spec="parameter.RealParameter" id="origin" lower="{{ origin_span[0] }}" upper="{{ origin_span[1] }}" value="{{ origin_span[1] }}"/>
+    {%- endif %}
+        {%- else %}
     <origin spec="parameter.RealParameter" id="origin" lower="{{ origin_span[0] }}" upper="Infinity" value="1.0"/>
     {%- endif %}
     <reproductiveNumber spec="parameter.RealParameter" id="reproductiveNumber" lower="0.0" upper="Infinity" value="2.0"/>
     <becomeUninfectiousRate spec="parameter.RealParameter" id="becomeUninfectiousRate" lower="0.0" upper="Infinity" value="1.0"/>
     <samplingProportion spec="parameter.RealParameter" id="samplingProportion" lower="0.0" upper="1.0" value="0.01"/>
   </birthDeathSkylineModel>
   {%- if clock_model == &quot;strict&quot; %}
@@ -70,21 +74,25 @@
     </state>
     <distribution spec="CompoundDistribution" id="posterior">
       <distribution spec="CompoundDistribution" id="prior">
         <!-- Priors for the Birth-Death Skyline model -->
         <distribution spec="CompoundDistribution" id="bdLikelihood">
           <distribution idref="birthDeath"/>
         </distribution>
+        {%- if origin_span[1] %}
+                {%- if origin_span[1] != origin_span[0] %}
         <distribution spec="Prior" id="originPrior" x="@origin">
-          {%- if origin_span[1] %}
           <distr spec="beast.base.inference.distribution.Uniform" lower="{{ origin_span[0] }}" upper="{{ origin_span[1] }}"/>
-          {%- else %}
+        </distribution>
+        {%- endif %}
+                {%- else %}
+        <distribution spec="Prior" id="originPrior" x="@origin">
           <distr spec="LogNormalDistributionModel" M="0.0" S="1.0" offset="{{ origin_span[0] }}"/>
-          {%- endif %}
         </distribution>
+        {%- endif %}
         <distribution spec="Prior" id="samplingProportionPrior" x="@samplingProportion">
           <distr spec="Beta" alpha="1.0" beta="1.0" offset="0.0"/>
         </distribution>
         <distribution spec="Prior" id="reproductiveNumberPrior" x="@reproductiveNumber">
           <distr spec="LogNormalDistributionModel" M="0.0" S="1.0"/>
         </distribution>
         <distribution spec="Prior" id="becomeUninfectiousRatePrior" x="@becomeUninfectiousRate">
@@ -176,15 +184,21 @@
     <operator spec="ScaleOperator" id="bdskySerialTreeScaler" scaleFactor="0.5" tree="@tree" weight="3.0"/>
     <operator spec="ScaleOperator" id="bdskySerialTreeRootScaler" rootOnly="true" scaleFactor="0.5" tree="@tree" weight="3.0"/>
     <operator spec="beast.base.evolution.operator.Uniform" id="bdskySerialUniformOperator" tree="@tree" weight="30.0"/>
     <operator spec="SubtreeSlide" id="bdskySerialSubtreeSlide" tree="@tree" weight="15.0"/>
     <operator spec="Exchange" id="bdskySerialNarrow" tree="@tree" weight="0.0"/>
     <operator spec="Exchange" id="bdskySerialWide" isNarrow="false" tree="@tree" weight="3.0"/>
     <operator spec="WilsonBalding" id="bdskySerialWilsonBalding" tree="@tree" weight="3.0"/>
+    {%- if origin_span[1] %}
+        {%- if origin_span[1] != origin_span[0] %}
+    <operator spec="ScaleOperator" id="originScaler" parameter="@origin" weight="10.0"/>
+    {%- endif %}
+        {%- else %}
     <operator spec="ScaleOperator" id="originScaler" parameter="@origin" weight="10.0"/>
+    {%- endif %}
     <operator spec="ScaleOperator" id="becomeUninfectiousRateScaler" parameter="@becomeUninfectiousRate" weight="2.0"/>
     <operator spec="ScaleOperator" id="reproductiveNumberScaler" parameter="@reproductiveNumber" weight="10.0"/>
     <operator spec="ScaleOperator" id="samplingProportionScaler" parameter="@samplingProportion" weight="10.0"/>
     <operator spec="UpDownOperator" id="updownBD" scaleFactor="0.75" weight="2.0">
       <up idref="reproductiveNumber"/>
       <down idref="becomeUninfectiousRate"/>
     </operator>
@@ -227,15 +241,21 @@
         {%- endfor %}
     <logger spec="Logger" id="tracelog" fileName="beast.log" logEvery="1000" model="@posterior" sanitiseHeaders="true" sort="smart">
       <log idref="posterior"/>
       <log idref="likelihood"/>
       <log idref="prior"/>
       <log spec="TreeHeightLogger" id="treeHeight" tree="@tree"/>
       <log idref="birthDeath"/>
+      {%- if origin_span[1] %}
+            {%- if origin_span[1] != origin_span[0] %}
       <log idref="origin"/>
+      {%- endif %}
+            {%- else %}
+      <log idref="origin"/>
+      {%- endif %}
       <log idref="becomeUninfectiousRate"/>
       <log idref="reproductiveNumber"/>
       <log idref="samplingProportion"/>
       <log spec="RateStatistic" id="rate" branchratemodel="@clock" tree="@tree"/>
       {%- if clock_model == &quot;strict&quot; %}
       <log idref="clock.mean"/>
       {%- elif clock_model == &quot;uncorrelated&quot; %}
```

### Comparing `teiphy-0.1.8/teiphy/variation_unit.py` & `teiphy-0.1.9/teiphy/variation_unit.py`

 * *Files identical despite different names*

### Comparing `teiphy-0.1.8/teiphy/witness.py` & `teiphy-0.1.9/teiphy/witness.py`

 * *Files identical despite different names*

### Comparing `teiphy-0.1.8/PKG-INFO` & `teiphy-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teiphy
-Version: 0.1.8
+Version: 0.1.9
 Summary: Converts TEI XML collations to NEXUS and other formats
 Home-page: https://github.com/jjmccollum/teiphy
 License: MIT
 Keywords: Python,phylogenetics,text encoding,TEI,NEXUS
 Author: Joey McCollum and Robert Turnbull
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Science/Research
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
-Requires-Dist: lxml (>=4.9.1,<5.0.0)
+Requires-Dist: lxml (>=4.9.3,<5.0.0)
 Requires-Dist: numpy (>=1.23.2,<2.0.0)
 Requires-Dist: openpyxl (>=3.0.10,<4.0.0)
 Requires-Dist: pandas (>=1.4.4,<2.0.0)
 Requires-Dist: python-slugify (>=6.1.2,<7.0.0)
 Requires-Dist: rich (>=12.5.1,<13.0.0)
 Requires-Dist: typer (>=0.6.1,<0.7.0)
 Project-URL: Documentation, https://jjmccollum.github.io/teiphy/
```

