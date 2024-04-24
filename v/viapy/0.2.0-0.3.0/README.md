# Comparing `tmp/viapy-0.2.0.tar.gz` & `tmp/viapy-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/viapy-0.2.0.tar", last modified: Thu Mar 26 16:03:57 2020, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `viapy-0.2.0.tar` & `viapy-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,30 @@
-drwxr-xr-x   0 rkoeser  (2011409658) admin       (80)        0 2020-03-26 16:03:57.000000 viapy-0.2.0/
--rw-r--r--   0 rkoeser  (2011409658) admin       (80)     5738 2020-03-26 16:03:57.000000 viapy-0.2.0/PKG-INFO
-drwxr-xr-x   0 rkoeser  (2011409658) admin       (80)        0 2020-03-26 16:03:57.000000 viapy-0.2.0/viapy/
--rw-r--r--   0 rkoeser  (2011409658) admin       (80)      259 2020-03-26 16:03:21.000000 viapy-0.2.0/viapy/__init__.py
--rw-r--r--   0 rkoeser  (2011409658) admin       (80)      730 2020-03-26 16:02:33.000000 viapy-0.2.0/viapy/widgets.py
--rw-r--r--   0 rkoeser  (2011409658) admin       (80)     6355 2017-10-12 21:22:34.000000 viapy-0.2.0/viapy/api.py
--rw-r--r--   0 rkoeser  (2011409658) admin       (80)      461 2020-03-26 16:02:33.000000 viapy-0.2.0/viapy/urls.py
--rw-r--r--   0 rkoeser  (2011409658) admin       (80)      253 2017-10-12 21:22:34.000000 viapy-0.2.0/viapy/test_urls.py
--rw-r--r--   0 rkoeser  (2011409658) admin       (80)     2476 2017-10-12 21:22:34.000000 viapy-0.2.0/viapy/views.py
--rw-r--r--   0 rkoeser  (2011409658) admin       (80)     1960 2020-03-26 16:02:33.000000 viapy-0.2.0/setup.py
-drwxr-xr-x   0 rkoeser  (2011409658) admin       (80)        0 2020-03-26 16:03:57.000000 viapy-0.2.0/viapy.egg-info/
--rw-r--r--   0 rkoeser  (2011409658) admin       (80)     5738 2020-03-26 16:03:57.000000 viapy-0.2.0/viapy.egg-info/PKG-INFO
--rw-r--r--   0 rkoeser  (2011409658) admin       (80)      269 2020-03-26 16:03:57.000000 viapy-0.2.0/viapy.egg-info/SOURCES.txt
--rw-r--r--   0 rkoeser  (2011409658) admin       (80)      224 2020-03-26 16:03:57.000000 viapy-0.2.0/viapy.egg-info/requires.txt
--rw-r--r--   0 rkoeser  (2011409658) admin       (80)        6 2020-03-26 16:03:57.000000 viapy-0.2.0/viapy.egg-info/top_level.txt
--rw-r--r--   0 rkoeser  (2011409658) admin       (80)        1 2020-03-26 16:03:57.000000 viapy-0.2.0/viapy.egg-info/dependency_links.txt
--rw-r--r--   0 rkoeser  (2011409658) admin       (80)      121 2020-03-26 16:03:57.000000 viapy-0.2.0/setup.cfg
--rw-r--r--   0 rkoeser  (2011409658) admin       (80)     3596 2020-03-26 16:02:33.000000 viapy-0.2.0/README.rst
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 viapy-0.3.0/CHANGELOG.rst
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 viapy-0.3.0/doc-requirements.txt
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 viapy-0.3.0/requirements.lock
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 viapy-0.3.0/setup.cfg
+-rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 viapy-0.3.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 viapy-0.3.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 viapy-0.3.0/.github/workflows/unit_tests.yml
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 viapy-0.3.0/sphinx-docs/Makefile
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 viapy-0.3.0/sphinx-docs/changelog.rst
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 viapy-0.3.0/sphinx-docs/codedocs.rst
+-rw-r--r--   0        0        0     6003 2020-02-02 00:00:00.000000 viapy-0.3.0/sphinx-docs/conf.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 viapy-0.3.0/sphinx-docs/docsettings.py
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 viapy-0.3.0/sphinx-docs/index.rst
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 viapy-0.3.0/sphinx-docs/make.bat
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 viapy-0.3.0/sphinx-docs/_templates/sidebar_footer.html
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 viapy-0.3.0/viapy/__init__.py
+-rw-r--r--   0        0        0     6653 2020-02-02 00:00:00.000000 viapy-0.3.0/viapy/api.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 viapy-0.3.0/viapy/test_urls.py
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 viapy-0.3.0/viapy/urls.py
+-rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 viapy-0.3.0/viapy/views.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 viapy-0.3.0/viapy/widgets.py
+-rw-r--r--   0        0        0     6813 2020-02-02 00:00:00.000000 viapy-0.3.0/viapy/tests/test_api.py
+-rw-r--r--   0        0        0     5365 2020-02-02 00:00:00.000000 viapy-0.3.0/viapy/tests/test_django.py
+-rw-r--r--   0        0        0   110994 2020-02-02 00:00:00.000000 viapy-0.3.0/viapy/tests/fixtures/102333412_rdf.xml
+-rw-r--r--   0        0        0    16978 2020-02-02 00:00:00.000000 viapy-0.3.0/viapy/tests/fixtures/sru_search.json
+-rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 viapy-0.3.0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 viapy-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3644 2020-02-02 00:00:00.000000 viapy-0.3.0/README.rst
+-rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 viapy-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6107 2020-02-02 00:00:00.000000 viapy-0.3.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `viapy-0.2.0/viapy/widgets.py` & `viapy-0.3.0/viapy/widgets.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from dal import autocomplete
 from django.utils.safestring import mark_safe
 
 
 class ViafWidget(autocomplete.Select2):
-    '''Custom autocomplete select widget that displays VIAF id as a link.
-    Extends :class:`dal.autocomplete.Select2`.'''
+    """Custom autocomplete select widget that displays VIAF id as a link.
+    Extends :class:`dal.autocomplete.Select2`."""
 
     def render(self, name, value, renderer=None, attrs=None):
         # select2 filters based on existing choices (non-existent here),
         # so when a value is set, add it to the list of choices
         if value:
             self.choices = [(value, value)]
         widget = super(ViafWidget, self).render(name, value, attrs)
         return mark_safe(
-            '%s<p><br /><a id="viaf_uri" target="_blank" href="%s">%s</a></p>' % \
-            (widget, value or '', value or ''))
-
-
+            '%s<p><br /><a id="viaf_uri" target="_blank" href="%s">%s</a></p>'
+            % (widget, value or "", value or "")
+        )
```

### Comparing `viapy-0.2.0/viapy/api.py` & `viapy-0.3.0/viapy/api.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import rdflib
 from rdflib.namespace import Namespace
 
 
 logger = logging.getLogger(__name__)
 
 
-SCHEMA_NS = Namespace('http://schema.org/')
+SCHEMA_NS = Namespace("http://schema.org/")
 
 
 class ViafAPI(object):
     """Wrapper for VIAF API.
 
     https://platform.worldcat.org/api-explorer/apis/VIAF
     """
@@ -29,176 +29,191 @@
 
     @classmethod
     def uri_from_id(cls, viaf_id):
         """Generate a canonical VIAF URI for the specified id"""
         return "%s/%s" % (cls.uri_base, viaf_id)
 
     def suggest(self, term):
-        '''Query autosuggest API.  Returns a list of results, or an
-        empty list if no suggestions are found or if something went wrong'''
+        """Query autosuggest API.  Returns a list of results, or an
+        empty list if no suggestions are found or if something went wrong"""
 
         #  'viaf/AutoSuggest?query=[searchTerms]&callback[optionalCallbackName]
-        autosuggest_url = '%s/AutoSuggest' % self.api_base
-        response = requests.get(autosuggest_url,
-                                params={'query': term},
-                                headers={'accept': 'application/json'})
-        logger.debug('autosuggest \'%s\': %s %s, %0.2f',
-                     term, response.status_code, response.reason,
-                     response.elapsed.total_seconds())
+        autosuggest_url = "%s/AutoSuggest" % self.api_base
+        response = requests.get(
+            autosuggest_url,
+            params={"query": term},
+            headers={"accept": "application/json"},
+        )
+        logger.debug(
+            "autosuggest '%s': %s %s, %0.2f",
+            term,
+            response.status_code,
+            response.reason,
+            response.elapsed.total_seconds(),
+        )
 
         if response.status_code == requests.codes.ok:
-            return response.json().get('result', None) or []
+            return response.json().get("result", None) or []
 
         # if there was an http error, raise it
         response.raise_for_status()
 
         return []
 
     def search(self, query):
-        '''Query VIAF seach interface.  Returns a list of :class:`SRUItem`
+        """Query VIAF seach interface.  Returns a list of :class:`SRUItem`
         :param query: CQL query in viaf syntax (e.g., ``cql.any all "term"``)
-        '''
-        search_url = '%s/search' % self.api_base
+        """
+        search_url = "%s/search" % self.api_base
         params = {
-            'query': query,
-            'httpAccept': 'application/json',
-            'maximumRecords': 50,   # TODO: configurable ?
+            "query": query,
+            "httpAccept": "application/json",
+            "maximumRecords": 50,  # TODO: configurable ?
             # sort by number of holdings (default sort on web search)
             # - so better known names show up first
-            'sortKeys': 'holdingscount'
+            "sortKeys": "holdingscount",
         }
 
         response = requests.get(search_url, params=params)
-        logger.debug('search \'%s\': %s %s, %0.2f',
-                     params['query'], response.status_code, response.reason,
-                     response.elapsed.total_seconds())
+        logger.debug(
+            "search '%s': %s %s, %0.2f",
+            params["query"],
+            response.status_code,
+            response.reason,
+            response.elapsed.total_seconds(),
+        )
         if response.status_code == requests.codes.ok:
             data = SRUResult(response.json())
             if data.total_results:
                 return data.records
 
         # if response was not ok, raise the error
         response.raise_for_status()
 
     def _find_type(self, fltr, value):
         return self.search('%s all "%s"' % (fltr, value))
 
     def find_person(self, name):
-        '''Search VIAF for local.personalNames'''
-        return self._find_type('local.personalNames', name)
+        """Search VIAF for local.personalNames"""
+        return self._find_type("local.personalNames", name)
 
     def find_corporate(self, name):
-        '''Search VIAF for local.corporateNames'''
-        return self._find_type('local.corporateNames', name)
+        """Search VIAF for local.corporateNames"""
+        return self._find_type("local.corporateNames", name)
 
     def find_place(self, name):
-        '''Search VIAF for local.geographicNames'''
-        return self._find_type('local.geographicNames', name)
+        """Search VIAF for local.geographicNames"""
+        return self._find_type("local.geographicNames", name)
 
 
 class ViafEntity(object):
-    '''Object for working with a single VIAF entity.
+    """Object for working with a single VIAF entity.
 
     :param viaf_id: viaf identifier (either integer or uri)
-    '''
+    """
+
     def __init__(self, viaf_id):
         try:
             int(viaf_id)
             self.uri = ViafAPI.uri_from_id(viaf_id)
         except ValueError:
             # NOTE: do we need to canonicalize the URI in any way to
             # ensure RDF queries work properly?
             self.uri = viaf_id
 
     @property
     def uriref(self):
-        '''VIAF URI reference as instance of :class:`rdflib.URIRef`'''
+        """VIAF URI reference as instance of :class:`rdflib.URIRef`"""
         return rdflib.URIRef(self.uri)
 
     @cached_property
     def rdf(self):
-        '''VIAF data for this entity as :class:`rdflib.Graph`'''
+        """VIAF data for this entity as :class:`rdflib.Graph`"""
         start = time.time()
         graph = rdflib.Graph()
         graph.parse(self.uri)
-        logger.debug('Loaded VIAF RDF %s: %0.2f sec',
-                     self.uri, time.time() - start)
+        logger.debug("Loaded VIAF RDF %s: %0.2f sec", self.uri, time.time() - start)
         return graph
 
     # person-specific properties
 
     @property
     def birthdate(self):
-        '''schema birthdate as :class:`rdflib.Literal`'''
+        """schema birthdate as :class:`rdflib.Literal`"""
         return self.rdf.value(self.uriref, SCHEMA_NS.birthDate)
 
     @property
     def deathdate(self):
-        '''schema deathdate as :class:`rdflib.Literal`'''
+        """schema deathdate as :class:`rdflib.Literal`"""
         return self.rdf.value(self.uriref, SCHEMA_NS.deathDate)
 
     @property
     def birthyear(self):
-        '''birth year'''
+        """birth year"""
         if self.birthdate:
             return self.year_from_isodate(str(self.birthdate))
 
     @property
     def deathyear(self):
-        '''death year'''
+        """death year"""
         if self.deathdate:
             return self.year_from_isodate(str(self.deathdate))
 
     # utility method for date parsing
     @classmethod
     def year_from_isodate(cls, date):
-        '''Return just the year portion of an ISO8601 date.  Expects
-        a string, returns an integer'''
-        return int(date.split('-')[0])
+        """Return just the year portion of an ISO8601 date.  Expects
+        a string, returns an integer. Supports negative dates."""
+        negative = False
+        # if the date starts with a dash, strip off before trying to split
+        if date.startswith("-"):
+            date = date[1:]
+            negative = True
+        value = int(date.split("-")[0])
+        if negative:
+            return -value
+        return value
 
 
 class SRUResult(object):
-    '''SRU search result object, for use with :meth:`ViafAPI.search`.'''
+    """SRU search result object, for use with :meth:`ViafAPI.search`."""
 
     def __init__(self, data):
-        self._data = data.get('searchRetrieveResponse', {})
+        self._data = data.get("searchRetrieveResponse", {})
 
     @cached_property
     def total_results(self):
-        '''number of records matching the query'''
-        return int(self._data.get('numberOfRecords', 0))
+        """number of records matching the query"""
+        return int(self._data.get("numberOfRecords", 0))
 
     @cached_property
     def records(self):
-        '''list of results as :class:`SRUItem`.'''
-        return [SRUItem(d['record']) for d in self._data.get('records', [])]
+        """list of results as :class:`SRUItem`."""
+        return [SRUItem(d["record"]) for d in self._data.get("records", [])]
 
 
 class SRUItem(AttrMap):
-    '''Single item returned by a SRU search, for use with
-    :meth:`ViafAPI.search` and :class:`SRUResult`.'''
+    """Single item returned by a SRU search, for use with
+    :meth:`ViafAPI.search` and :class:`SRUResult`."""
 
     @property
     def uri(self):
-        '''VIAF URI for this result'''
-        return self.recordData.Document['@about']
+        """VIAF URI for this result"""
+        return self.recordData.Document["@about"]
 
     @property
     def viaf_id(self):
-        '''VIAF numeric identifier'''
+        """VIAF numeric identifier"""
         return self.recordData.viafID
 
-
     @property
     def nametype(self):
-        '''type of name (personal, corporate, title, etc)'''
+        """type of name (personal, corporate, title, etc)"""
         return self.recordData.nameType
 
     @property
     def label(self):
-        '''first main heading for this item'''
+        """first main heading for this item"""
         try:
             return self.recordData.mainHeadings.data[0].text
         except KeyError:
             return self.recordData.mainHeadings.data.text
-
-
```

### Comparing `viapy-0.2.0/viapy/views.py` & `viapy-0.3.0/viapy/views.py`

 * *Files identical despite different names*

### Comparing `viapy-0.2.0/setup.py` & `viapy-0.3.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,56 +1,59 @@
-import os
-from setuptools import find_packages, setup
+[build-system]
+requires = ["hatchling"]
+build-backend = "hatchling.build"
+
+[project]
+name = "viapy"
+description = "Python module for interacting with VIAF data & APIs"
+authors = [
+  {name = "Center for Digital Humanities at Princeton", email = "cdh@princeton.edu"},
+]
+requires-python = ">=3.9"
+readme = "README.rst"
+license = {text = "Apache-2"}
+classifiers = [
+    "Environment :: Web Environment",
+    "Framework :: Django",
+    "Framework :: Django :: 3.2",
+    "Framework :: Django :: 4.0",
+    "Framework :: Django :: 4.1",
+    "Framework :: Django :: 4.2",
+    "Framework :: Django :: 5.0",
+    "Intended Audience :: Developers",
+    "License :: OSI Approved :: Apache Software License",
+    "Operating System :: OS Independent",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
+    "Topic :: Internet :: WWW/HTTP",
+    "Topic :: Software Development :: Libraries :: Python Modules",
+]
+dynamic = ["version"]
+dependencies = [
+  "requests", "rdflib", "cached_property", "attrdict3"
+]
+
+[project.urls]
+#Documentation = "https://readthedocs.org"
+Repository = "https://github.com/Princeton-CDH/viapy"
+Changelog = "https://github.com/Princeton-CDH/viapy/blob/main/CHANGELOG.rst"
+
+[tool.hatch.version]
+path = "viapy/__init__.py"
+
+[project.optional-dependencies]
+test = [
+  "pytest",
+  "pytest-cov"
+]
+django = ["django>=3.2", "django-autocomplete-light"]
+django_test = ["pytest-django", "viapy[django]"]
+docs = ["sphinx"]
+test_all = ["viapy[test]", "viapy[django_test]"]
+dev = ["pre-commit", "viapy[django]", "viapy[test_all]", "viapy[docs]"]
 
-from viapy import __version__
-
-with open(os.path.join(os.path.dirname(__file__), 'README.rst')) as readme:
-    README = readme.read()
-
-# allow setup.py to be run from any path
-os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
-
-REQUIREMENTS = ['requests', 'rdflib', 'cached_property', 'attrdict']
-TEST_REQUIREMENTS = ['pytest', 'pytest-cov']
-DJANGO_REQS = ['django>=1.11,<3.1', 'django-autocomplete-light']
-DJANGO_TEST_REQS = ['pytest-django']
-
-
-setup(
-    name='viapy',
-    version=__version__,
-    packages=find_packages(),
-    include_package_data=True,
-    license='Apache License, Version 2.0',
-    description='Python module for interacting with VIAF data & APIs',
-    long_description=README,
-    url='https://github.com/Princeton-CDH/viapy',
-    install_requires=REQUIREMENTS,
-    setup_requires=['pytest-runner'],
-    tests_require=TEST_REQUIREMENTS,
-    extras_require={
-        'django': DJANGO_REQS,
-        'test': TEST_REQUIREMENTS,
-        'test_all': TEST_REQUIREMENTS + DJANGO_REQS + DJANGO_TEST_REQS,
-        'docs': ['sphinx']
-    },
-    author='CDH @ Princeton',
-    author_email='digitalhumanities@princeton.edu',
-    classifiers=[
-        'Environment :: Web Environment',
-        'Framework :: Django',
-        'Framework :: Django :: 1.11',
-        'Framework :: Django :: 2.0',
-        'Framework :: Django :: 2.1',
-        'Framework :: Django :: 2.2',
-        'Framework :: Django :: 3.0',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: Apache Software License',
-        'Operating System :: OS Independent',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
-        'Topic :: Internet :: WWW/HTTP',
-        'Topic :: Software Development :: Libraries :: Python Modules',
-    ],
-)
+[tool.pytest.ini_options]
+DJANGO_SETTINGS_MODULE = "testsettings"
```

### Comparing `viapy-0.2.0/README.rst` & `viapy-0.3.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 Authority File) data and APIs.
 
 .. _VIAF: http://viaf.org
 
 **viapy** provides optional Django integration; this currently includes a
 django-autocomplete-light lookup view and a VIAF url widget.
 
-.. image:: https://travis-ci.org/Princeton-CDH/viapy.svg
-    :target: https://travis-ci.org/Princeton-CDH/viapy
+.. image:: https://github.com/Princeton-CDH/viapy/actions/workflows/unit_tests.yml/badge.svg
+    :target: https://github.com/Princeton-CDH/viapy/actions/workflows/unit_tests.yml
     :alt: Build status
 
 .. image:: https://codecov.io/gh/Princeton-CDH/viapy/branch/master/graph/badge.svg
     :target: https://codecov.io/gh/Princeton-CDH/viapy/branch/master
     :alt: Code coverage
 
 .. image:: https://requires.io/github/Princeton-CDH/viapy/requirements.svg
@@ -61,37 +61,36 @@
     )
 
 
 Include the viapy urls at the desired base url with the namespace::
 
     urlpatterns = [
         ...
-        url(r'^viaf/', include('viapy.urls', namespace='viaf')),
+        path(r'viaf/', include('viapy.urls', namespace='viaf')),
         ...
     ]
 
 
 Development instructions
 ------------------------
 
 This git repository uses `git flow`_ branching conventions.
 
 .. _git flow: https://github.com/nvie/gitflow
 
 Initial setup and installation:
 
-- Recommended: create and activate a python 3.5 virtualenv::
+- Recommended: create and activate a python 3.11 virtualenv::
 
-    virtualenv viapy -p python3.5
+    python3 -m venv viapy
     source viapy/bin/activate
 
-- pip install the package with its python dependencies::
+- pip install the package with all development and test dependencies::
 
-    pip install -e .
-    pip install -e ".[django]""
+    pip install -e ".[dev]""
 
 
 Unit Testing
 ^^^^^^^^^^^^
 
 Unit tests are set up to be run with `py.test <http://doc.pytest.org/>`_
 
@@ -111,15 +110,15 @@
 
 Documentation
 ^^^^^^^^^^^^^
 
 Documentation is generated using `sphinx <http://www.sphinx-doc.org/>`_.
 To generate documentation, first install development requirements::
 
-    pip install -e ".[docs]"
+    pip install -e ".[dev]"
 
 Then build the documentation using the customized make file in the `docs`
 directory::
 
     cd sphinx-docs
     make html
 
@@ -129,11 +128,11 @@
 
 
 License
 -------
 
 **viapy** is distributed under the Apache 2.0 License.
 
-©2017 Trustees of Princeton University.  Permission granted via
+©2024 Trustees of Princeton University.  Permission granted via
 Princeton Docket #18-3449-1 for distribution online under a standard Open Source
 license.  Ownership rights transferred to Rebecca Koeser provided software
 is distributed online via open source.
```

