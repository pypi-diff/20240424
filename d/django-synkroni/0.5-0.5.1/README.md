# Comparing `tmp/django-synkroni-0.5.tar.gz` & `tmp/django_synkroni-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-synkroni-0.5.tar", last modified: Mon Jun 12 06:25:01 2023, max compression
+gzip compressed data, was "django_synkroni-0.5.1.tar", last modified: Wed Apr 24 17:59:46 2024, max compression
```

## Comparing `django-synkroni-0.5.tar` & `django_synkroni-0.5.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-12 06:25:01.249438 django-synkroni-0.5/
--rw-r--r--   0 aha        (501) staff       (20)       75 2021-09-06 06:31:51.000000 django-synkroni-0.5/MANIFEST.in
--rw-r--r--   0 aha        (501) staff       (20)      240 2023-06-12 06:25:01.249285 django-synkroni-0.5/PKG-INFO
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-12 06:25:01.246614 django-synkroni-0.5/django_synkroni.egg-info/
--rw-r--r--   0 aha        (501) staff       (20)      240 2023-06-12 06:25:01.000000 django-synkroni-0.5/django_synkroni.egg-info/PKG-INFO
--rw-r--r--   0 aha        (501) staff       (20)      592 2023-06-12 06:25:01.000000 django-synkroni-0.5/django_synkroni.egg-info/SOURCES.txt
--rw-r--r--   0 aha        (501) staff       (20)        1 2023-06-12 06:25:01.000000 django-synkroni-0.5/django_synkroni.egg-info/dependency_links.txt
--rw-r--r--   0 aha        (501) staff       (20)       47 2023-06-12 06:25:01.000000 django-synkroni-0.5/django_synkroni.egg-info/entry_points.txt
--rw-r--r--   0 aha        (501) staff       (20)     6944 2023-06-12 06:25:01.000000 django-synkroni-0.5/django_synkroni.egg-info/historia.json
--rw-r--r--   0 aha        (501) staff       (20)        1 2021-09-06 06:32:14.000000 django-synkroni-0.5/django_synkroni.egg-info/not-zip-safe
--rw-r--r--   0 aha        (501) staff       (20)       34 2023-06-12 06:25:01.000000 django-synkroni-0.5/django_synkroni.egg-info/requires.txt
--rw-r--r--   0 aha        (501) staff       (20)        9 2023-06-12 06:25:01.000000 django-synkroni-0.5/django_synkroni.egg-info/top_level.txt
--rw-r--r--   0 aha        (501) staff       (20)       80 2023-06-12 06:21:01.000000 django-synkroni-0.5/pyproject.toml
--rw-r--r--   0 aha        (501) staff       (20)       38 2023-06-12 06:25:01.249481 django-synkroni-0.5/setup.cfg
--rw-r--r--   0 aha        (501) staff       (20)      576 2023-06-12 06:20:49.000000 django-synkroni-0.5/setup.py
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-12 06:25:01.248422 django-synkroni-0.5/synkroni/
--rw-r--r--   0 aha        (501) staff       (20)      107 2021-04-07 18:03:12.000000 django-synkroni-0.5/synkroni/__init__.py
--rw-r--r--   0 aha        (501) staff       (20)      683 2021-09-20 10:38:01.000000 django-synkroni-0.5/synkroni/json.py
--rw-r--r--   0 aha        (501) staff       (20)      261 2021-09-20 10:38:01.000000 django-synkroni-0.5/synkroni/komennot.py
--rw-r--r--   0 aha        (501) staff       (20)      159 2021-04-08 18:06:03.000000 django-synkroni-0.5/synkroni/mallit.py
--rw-r--r--   0 aha        (501) staff       (20)       22 2021-04-08 17:56:03.000000 django-synkroni-0.5/synkroni/models.py
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-12 06:25:01.244742 django-synkroni-0.5/synkroni/static/
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-12 06:25:01.244793 django-synkroni-0.5/synkroni/static/synkroni/
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-12 06:25:01.248713 django-synkroni-0.5/synkroni/static/synkroni/js/
--rw-r--r--   0 aha        (501) staff       (20)     9447 2022-09-27 07:22:03.000000 django-synkroni-0.5/synkroni/static/synkroni/js/synkroni.js
--rw-r--r--   0 aha        (501) staff       (20)     2688 2022-11-18 14:29:51.000000 django-synkroni-0.5/synkroni/synkroni.py
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-12 06:25:01.244918 django-synkroni-0.5/synkroni/templates/
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-12 06:25:01.249089 django-synkroni-0.5/synkroni/templates/synkroni/
--rw-r--r--   0 aha        (501) staff       (20)      859 2022-05-04 12:06:11.000000 django-synkroni-0.5/synkroni/templates/synkroni/synkroni.html
--rw-r--r--   0 aha        (501) staff       (20)     2080 2023-06-08 12:38:34.000000 django-synkroni-0.5/synkroni/toiminnot.py
--rw-r--r--   0 aha        (501) staff       (20)     5565 2022-11-18 14:29:51.000000 django-synkroni-0.5/synkroni/websocket.py
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2024-04-24 17:59:46.456380 django_synkroni-0.5.1/
+-rw-r--r--   0 aha        (501) staff       (20)       75 2021-09-06 06:31:51.000000 django_synkroni-0.5.1/MANIFEST.in
+-rw-r--r--   0 aha        (501) staff       (20)      306 2024-04-24 17:59:46.455994 django_synkroni-0.5.1/PKG-INFO
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2024-04-24 17:59:46.455698 django_synkroni-0.5.1/django_synkroni.egg-info/
+-rw-r--r--   0 aha        (501) staff       (20)      306 2024-04-24 17:59:46.000000 django_synkroni-0.5.1/django_synkroni.egg-info/PKG-INFO
+-rw-r--r--   0 aha        (501) staff       (20)      592 2024-04-24 17:59:46.000000 django_synkroni-0.5.1/django_synkroni.egg-info/SOURCES.txt
+-rw-r--r--   0 aha        (501) staff       (20)        1 2024-04-24 17:59:46.000000 django_synkroni-0.5.1/django_synkroni.egg-info/dependency_links.txt
+-rw-r--r--   0 aha        (501) staff       (20)       47 2024-04-24 17:59:46.000000 django_synkroni-0.5.1/django_synkroni.egg-info/entry_points.txt
+-rw-r--r--   0 aha        (501) staff       (20)     7124 2024-04-24 17:59:46.000000 django_synkroni-0.5.1/django_synkroni.egg-info/historia.json
+-rw-r--r--   0 aha        (501) staff       (20)        1 2021-09-06 06:32:14.000000 django_synkroni-0.5.1/django_synkroni.egg-info/not-zip-safe
+-rw-r--r--   0 aha        (501) staff       (20)       34 2024-04-24 17:59:46.000000 django_synkroni-0.5.1/django_synkroni.egg-info/requires.txt
+-rw-r--r--   0 aha        (501) staff       (20)        9 2024-04-24 17:59:46.000000 django_synkroni-0.5.1/django_synkroni.egg-info/top_level.txt
+-rw-r--r--   0 aha        (501) staff       (20)       80 2023-06-12 06:21:01.000000 django_synkroni-0.5.1/pyproject.toml
+-rw-r--r--   0 aha        (501) staff       (20)       38 2024-04-24 17:59:46.456516 django_synkroni-0.5.1/setup.cfg
+-rw-r--r--   0 aha        (501) staff       (20)      576 2023-06-12 06:20:49.000000 django_synkroni-0.5.1/setup.py
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2024-04-24 17:59:46.454069 django_synkroni-0.5.1/synkroni/
+-rw-r--r--   0 aha        (501) staff       (20)      107 2021-04-07 18:03:12.000000 django_synkroni-0.5.1/synkroni/__init__.py
+-rw-r--r--   0 aha        (501) staff       (20)      683 2021-09-20 10:38:01.000000 django_synkroni-0.5.1/synkroni/json.py
+-rw-r--r--   0 aha        (501) staff       (20)      261 2021-09-20 10:38:01.000000 django_synkroni-0.5.1/synkroni/komennot.py
+-rw-r--r--   0 aha        (501) staff       (20)      159 2021-04-08 18:06:03.000000 django_synkroni-0.5.1/synkroni/mallit.py
+-rw-r--r--   0 aha        (501) staff       (20)       22 2021-04-08 17:56:03.000000 django_synkroni-0.5.1/synkroni/models.py
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2024-04-24 17:59:46.449283 django_synkroni-0.5.1/synkroni/static/
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2024-04-24 17:59:46.449346 django_synkroni-0.5.1/synkroni/static/synkroni/
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2024-04-24 17:59:46.454596 django_synkroni-0.5.1/synkroni/static/synkroni/js/
+-rw-r--r--   0 aha        (501) staff       (20)    11452 2023-08-25 08:44:45.000000 django_synkroni-0.5.1/synkroni/static/synkroni/js/synkroni.js
+-rw-r--r--   0 aha        (501) staff       (20)     2688 2022-11-18 14:29:51.000000 django_synkroni-0.5.1/synkroni/synkroni.py
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2024-04-24 17:59:46.449490 django_synkroni-0.5.1/synkroni/templates/
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2024-04-24 17:59:46.455298 django_synkroni-0.5.1/synkroni/templates/synkroni/
+-rw-r--r--   0 aha        (501) staff       (20)      859 2022-05-04 12:06:11.000000 django_synkroni-0.5.1/synkroni/templates/synkroni/synkroni.html
+-rw-r--r--   0 aha        (501) staff       (20)     2080 2023-11-08 17:08:31.000000 django_synkroni-0.5.1/synkroni/toiminnot.py
+-rw-r--r--   0 aha        (501) staff       (20)     5402 2024-04-24 17:46:43.000000 django_synkroni-0.5.1/synkroni/websocket.py
```

### Comparing `django-synkroni-0.5/django_synkroni.egg-info/SOURCES.txt` & `django_synkroni-0.5.1/django_synkroni.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-synkroni-0.5/django_synkroni.egg-info/historia.json` & `django_synkroni-0.5.1/django_synkroni.egg-info/historia.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {'insert': "[(0, OrderedDict([('revisio', '33d7654e04257bda9e567162abc77c96616afe27'), ('versio', "*

 * *           "'0.5.1'), ('kuvaus', 'Vältetään toimintojen nostamien poikkeusten nielaiseminen')]))]"}*

```diff
@@ -1,9 +1,14 @@
 [
     {
+        "kuvaus": "V\u00e4ltet\u00e4\u00e4n toimintojen nostamien poikkeusten nielaiseminen",
+        "revisio": "33d7654e04257bda9e567162abc77c96616afe27",
+        "versio": "0.5.1"
+    },
+    {
         "kuvaus": "Muutettu `toiminnot.muuttaa_tietoja` asynkroniseksi kontekstink\u00e4sittelij\u00e4ksi",
         "revisio": "058f3de1f888379881e82044d569970a3c884381",
         "versio": "0.5"
     },
     {
         "kuvaus": "P\u00e4ivitetty versiointij\u00e4rjestelm\u00e4",
         "revisio": "a3c6dfc33ea6c98b28f8b5a3929e27e70055e3c0",
```

### Comparing `django-synkroni-0.5/setup.py` & `django_synkroni-0.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `django-synkroni-0.5/synkroni/json.py` & `django_synkroni-0.5.1/synkroni/json.py`

 * *Files identical despite different names*

### Comparing `django-synkroni-0.5/synkroni/static/synkroni/js/synkroni.js` & `django_synkroni-0.5.1/synkroni/static/synkroni/js/synkroni.js`

 * *Files 21% similar despite different names*

#### js-beautify {}

```diff
@@ -178,14 +178,46 @@
                     this.yhteys.send(
                         `{"n": ${osat.length - i - 1}, "o": "${osa}"}`
                     );
                 }.bind(this))
             }
         },
 
+        _poimiMuuttuneetSolmut: function(p) {
+            // Poimi kaikki JSON-paikkauksen muuttamat solmut.
+            // Huomaa, että kukin muutettu polku esitetään vinoviivalla
+            // alkavana, vinoviivoin erotettuna merkkijonona.
+            // Ensimmäinen alkio on aina tyhjä, viimeinen on muuttunut tieto.
+            // Poimitaan kunkin polun kaikki alkiot näiden väliltä.
+            // Poistetaan kaksoiskappaleet luettelosta.
+            let muuttuneetSolmut = p.map(function(muutos) {
+                return muutos.path.split("/").slice(1, -1);
+            });
+
+            // Järjestä muutokset ensin polun pituuden mukaan, sitten aakkosittain.
+            muuttuneetSolmut.sort(function(s1, s2) {
+                return s1.length - s2.length || (s1 < s2 ? -1 : s1 > s2 ? 1 : 0);
+            });
+
+            // Suodata pois muihin muutoksiin sisältyvät, sisemmät muutokset.
+            // Palauta tulokset tavuviivoin erotettuina merkkijonoina.
+            return muuttuneetSolmut.reduce(function(muutokset, s2) {
+                for (let muutos of muutokset)
+                    if (muutos.reduce(function(tulos, alkio, i) {
+                            return tulos && alkio === s2[i];
+                        }))
+                        // Jokin aiempi muutospolku sisälsi s2:n: ei lisätä mitään.
+                        return muutokset;
+                // Mikään aiempi muutos ei sisältänyt s2:ta: lisätään se listalle.
+                return muutokset.concat([s2]);
+            }, []).map(function(muutos) {
+                return muutos.join("-");
+            });
+        },
+
         _lahtevaMuutos: function(p) {
             jsonpatch.apply(this.__vietavaData, JSON.parse(JSON.stringify(p)));
             if (this.yhteys?.readyState === 1) {
                 this._lahetaData(p);
             } else {
                 // Jätä sanoma jonoon, mikäli yhteyttä ei ole.
                 this.lahetysjono.push(p);
@@ -195,28 +227,47 @@
             this.tarkkailija?.pause?.();
             jsonpatch.apply(document.data, p);
             jsonpatch.apply(this.__vietavaData, JSON.parse(JSON.stringify(p)));
             this._tulkitseVierasavaimet(document.data);
             this.tarkkailija?.resume?.();
             document.dispatchEvent(
                 new Event("data-paivitetty")
+                // new CustomEvent(
+                //   "data-paivitetty",
+                //   {detail: this._poimiMuuttuneetSolmut(p)}
+                // )
             );
         },
 
-        _tulkitseVierasavaimet: function(data) {
+        _tulkitseVierasavaimet: function(data, solmu) {
+            solmu = solmu ?? [];
             for (let [avain, arvo] of Object.entries(data)) {
                 if (Array.isArray(arvo))
-                    for (let rivi of arvo)
-                        this._tulkitseVierasavaimet(rivi);
+                    for (let [indeksi, rivi] of arvo.entries())
+                        this._tulkitseVierasavaimet(
+                            rivi,
+                            solmu.concat([avain, indeksi])
+                        );
                 else if (typeof arvo !== 'object' || arvo === null)
                 ;
                 else if (arvo.hasOwnProperty("__vierasavain__")) {
                     let [
                         vierasavain, vierasavain_id
                     ] = arvo.__vierasavain__;
+                    document.dispatchEvent(
+                        new CustomEvent(
+                            "data-vierasavain", {
+                                detail: {
+                                    lahde: solmu.concat([avain]),
+                                    kohde: vierasavain,
+                                    avain: vierasavain_id,
+                                }
+                            }
+                        )
+                    );
                     Object.defineProperty(
                         data,
                         avain, {
                             get: function() {
                                 // Poimitaan vierasavain ensisijaisesti
                                 // `this`-olion tiedoista.
                                 // Mikäli tätä ei ole, käytetään
@@ -235,15 +286,18 @@
                             enumerable: arvo.hasOwnProperty(
                                 vierasavain_id
                             ),
                             configurable: true
                         }
                     );
                 } else
-                    this._tulkitseVierasavaimet(arvo);
+                    this._tulkitseVierasavaimet(
+                        arvo,
+                        solmu.concat([avain])
+                    );
             }
         },
 
         toiminto: function(data) {
             data.toiminto_id = ++this.toiminto_id;
             return new Promise(function(vastaus, virhe) {
                 this.toimintojono[data.toiminto_id] = {
```

### Comparing `django-synkroni-0.5/synkroni/synkroni.py` & `django_synkroni-0.5.1/synkroni/synkroni.py`

 * *Files identical despite different names*

### Comparing `django-synkroni-0.5/synkroni/templates/synkroni/synkroni.html` & `django_synkroni-0.5.1/synkroni/templates/synkroni/synkroni.html`

 * *Files identical despite different names*

### Comparing `django-synkroni-0.5/synkroni/toiminnot.py` & `django_synkroni-0.5.1/synkroni/toiminnot.py`

 * *Files identical despite different names*

### Comparing `django-synkroni-0.5/synkroni/websocket.py` & `django_synkroni-0.5.1/synkroni/websocket.py`

 * *Files 6% similar despite different names*

```diff
@@ -111,24 +111,19 @@
     # async def kasittele_toiminto
 
   async def kasittele_saapuva_sanoma(self, request, sanoma):
     ''' Käsittele selaimelta saapuva sanoma. '''
     if 'toiminto_id' in sanoma:
       # Komento: suorita taustalla.
       # Useat peräkkäin saapuvat toiminnot ajetaan samanaikaisesti.
-      toiminto = asyncio.ensure_future(
-        self.kasittele_toiminto(request, **sanoma)
+      self.toimintojono.add(
+        asyncio.create_task(
+          self.kasittele_toiminto(request, **sanoma)
+        )
       )
-      self.toimintojono.add(toiminto)
-      @toiminto.add_done_callback
-      def done(task):
-        try:
-          task.result()
-        except BaseException:
-          traceback.print_exc()
 
     else:
       # Json-paikkaus: toteuta tässä.
       # Huomaa, että paikkaukset on toteutettava peräkkäin
       # saapumisjärjestyksessä, ei samanaikaisesti.
       sanoma = sanoma if isinstance(sanoma, list) else [sanoma]
       # pylint: disable=no-value-for-parameter
```

