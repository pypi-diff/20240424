# Comparing `tmp/collective.blog-1.0.0a9.tar.gz` & `tmp/collective.blog-1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collective.blog-1.0.0a9.tar", last modified: Wed Mar 27 18:11:28 2024, max compression
+gzip compressed data, was "dist/collective.blog-1.0a1.tar", last modified: Sun Feb 14 18:26:35 2016, max compression
```

## Comparing `collective.blog-1.0.0a9.tar` & `collective.blog-1.0a1.tar`

### file list

```diff
@@ -1,157 +1,91 @@
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-03-27 18:11:28.858569 collective.blog-1.0.0a9/
--rw-r--r--   0 davisagli   (501) staff       (20)     1363 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/.editorconfig
--rw-r--r--   0 davisagli   (501) staff       (20)     2387 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/CHANGES.md
--rw-r--r--   0 davisagli   (501) staff       (20)      137 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/CONTRIBUTORS.md
--rw-r--r--   0 davisagli   (501) staff       (20)    18092 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/LICENSE.GPL
--rw-r--r--   0 davisagli   (501) staff       (20)      659 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/LICENSE.md
--rw-r--r--   0 davisagli   (501) staff       (20)      328 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/MANIFEST.in
--rw-r--r--   0 davisagli   (501) staff       (20)     8672 2024-03-27 18:11:28.858231 collective.blog-1.0.0a9/PKG-INFO
--rw-r--r--   0 davisagli   (501) staff       (20)     4461 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/README.md
--rw-r--r--   0 davisagli   (501) staff       (20)       61 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/constraints.txt
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-03-27 18:11:28.840958 collective.blog-1.0.0a9/docs/
--rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/docs/.gitkeep
--rw-r--r--   0 davisagli   (501) staff       (20)    28415 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/docs/dlr.svg
--rw-r--r--   0 davisagli   (501) staff       (20)     9029 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/docs/fz-juelich.svg
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-03-27 18:11:28.841261 collective.blog-1.0.0a9/news/
--rw-r--r--   0 davisagli   (501) staff       (20)      308 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/news/.changelog_template.jinja
--rw-r--r--   0 davisagli   (501) staff       (20)        1 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/news/.gitkeep
--rw-r--r--   0 davisagli   (501) staff       (20)     4641 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/pyproject.toml
--rw-r--r--   0 davisagli   (501) staff       (20)       32 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/requirements.txt
--rw-r--r--   0 davisagli   (501) staff       (20)       38 2024-03-27 18:11:28.858615 collective.blog-1.0.0a9/setup.cfg
--rw-r--r--   0 davisagli   (501) staff       (20)     2308 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/setup.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-03-27 18:11:28.835956 collective.blog-1.0.0a9/src/
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-03-27 18:11:28.841395 collective.blog-1.0.0a9/src/collective/
--rw-r--r--   0 davisagli   (501) staff       (20)       56 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective/__init__.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-03-27 18:11:28.843925 collective.blog-1.0.0a9/src/collective/blog/
--rw-r--r--   0 davisagli   (501) staff       (20)      195 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective/blog/__init__.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-03-27 18:11:28.844541 collective.blog-1.0.0a9/src/collective/blog/behaviors/
--rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective/blog/behaviors/__init__.py
--rw-r--r--   0 davisagli   (501) staff       (20)      146 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective/blog/behaviors/blog.py
--rw-r--r--   0 davisagli   (501) staff       (20)      541 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective/blog/behaviors/configure.zcml
--rw-r--r--   0 davisagli   (501) staff       (20)      810 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective/blog/behaviors/tags.py
--rw-r--r--   0 davisagli   (501) staff       (20)      691 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective/blog/configure.zcml
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-03-27 18:11:28.845550 collective.blog-1.0.0a9/src/collective/blog/content/
--rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective/blog/content/__init__.py
--rw-r--r--   0 davisagli   (501) staff       (20)      408 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective/blog/content/author.py
--rw-r--r--   0 davisagli   (501) staff       (20)      229 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective/blog/content/blog.py
--rw-r--r--   0 davisagli   (501) staff       (20)     2422 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective/blog/content/post.py
--rw-r--r--   0 davisagli   (501) staff       (20)      414 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective/blog/content/tag.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-03-27 18:11:28.846036 collective.blog-1.0.0a9/src/collective/blog/controlpanel/
--rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective/blog/controlpanel/__init__.py
--rw-r--r--   0 davisagli   (501) staff       (20)      348 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective/blog/controlpanel/configure.zcml
--rw-r--r--   0 davisagli   (501) staff       (20)      546 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective/blog/controlpanel/controlpanel.py
--rw-r--r--   0 davisagli   (501) staff       (20)      186 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective/blog/dependencies.zcml
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-03-27 18:11:28.846801 collective.blog-1.0.0a9/src/collective/blog/indexers/
--rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective/blog/indexers/__init__.py
--rw-r--r--   0 davisagli   (501) staff       (20)      247 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective/blog/indexers/author.py
--rw-r--r--   0 davisagli   (501) staff       (20)      507 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective/blog/indexers/configure.zcml
--rw-r--r--   0 davisagli   (501) staff       (20)      531 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective/blog/indexers/post.py
--rw-r--r--   0 davisagli   (501) staff       (20)      420 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective/blog/indexers/tag.py
--rw-r--r--   0 davisagli   (501) staff       (20)      950 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective/blog/interfaces.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-03-27 18:11:28.847260 collective.blog-1.0.0a9/src/collective/blog/locales/
--rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective/blog/locales/__init__.py
--rw-r--r--   0 davisagli   (501) staff       (20)     5241 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective/blog/locales/collective.blog.pot
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-03-27 18:11:28.836596 collective.blog-1.0.0a9/src/collective/blog/locales/de/
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-03-27 18:11:28.847407 collective.blog-1.0.0a9/src/collective/blog/locales/de/LC_MESSAGES/
--rw-r--r--   0 davisagli   (501) staff       (20)     5217 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective/blog/locales/de/LC_MESSAGES/collective.blog.po
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-03-27 18:11:28.836741 collective.blog-1.0.0a9/src/collective/blog/locales/en/
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-03-27 18:11:28.847559 collective.blog-1.0.0a9/src/collective/blog/locales/en/LC_MESSAGES/
--rw-r--r--   0 davisagli   (501) staff       (20)     5132 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective/blog/locales/en/LC_MESSAGES/collective.blog.po
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-03-27 18:11:28.836884 collective.blog-1.0.0a9/src/collective/blog/locales/es/
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-03-27 18:11:28.847722 collective.blog-1.0.0a9/src/collective/blog/locales/es/LC_MESSAGES/
--rw-r--r--   0 davisagli   (501) staff       (20)     5123 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective/blog/locales/es/LC_MESSAGES/collective.blog.po
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-03-27 18:11:28.837034 collective.blog-1.0.0a9/src/collective/blog/locales/pt_BR/
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-03-27 18:11:28.847889 collective.blog-1.0.0a9/src/collective/blog/locales/pt_BR/LC_MESSAGES/
--rw-r--r--   0 davisagli   (501) staff       (20)     5756 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective/blog/locales/pt_BR/LC_MESSAGES/collective.blog.po
--rw-r--r--   0 davisagli   (501) staff       (20)     2487 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective/blog/locales/update.py
--rw-r--r--   0 davisagli   (501) staff       (20)      670 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective/blog/permissions.zcml
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-03-27 18:11:28.837433 collective.blog-1.0.0a9/src/collective/blog/profiles/
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-03-27 18:11:28.849298 collective.blog-1.0.0a9/src/collective/blog/profiles/default/
--rw-r--r--   0 davisagli   (501) staff       (20)      157 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective/blog/profiles/default/browserlayer.xml
--rw-r--r--   0 davisagli   (501) staff       (20)      860 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective/blog/profiles/default/catalog.xml
--rw-r--r--   0 davisagli   (501) staff       (20)      422 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective/blog/profiles/default/controlpanel.xml
--rw-r--r--   0 davisagli   (501) staff       (20)      624 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective/blog/profiles/default/diff_tool.xml
--rw-r--r--   0 davisagli   (501) staff       (20)      189 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective/blog/profiles/default/metadata.xml
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-03-27 18:11:28.849897 collective.blog-1.0.0a9/src/collective/blog/profiles/default/registry/
--rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective/blog/profiles/default/registry/.gitkeep
--rw-r--r--   0 davisagli   (501) staff       (20)      752 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective/blog/profiles/default/registry/Products.CMFPlone.interfaces.controlpanel.INavigationSchema.xml
--rw-r--r--   0 davisagli   (501) staff       (20)      292 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective/blog/profiles/default/registry/collective.blog.interfaces.IBlogSettings.xml
--rw-r--r--   0 davisagli   (501) staff       (20)     1538 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective/blog/profiles/default/registry/plone.app.querystring.interfaces.IQueryField.xml
--rw-r--r--   0 davisagli   (501) staff       (20)      592 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective/blog/profiles/default/repositorytool.xml
--rw-r--r--   0 davisagli   (501) staff       (20)      625 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective/blog/profiles/default/rolemap.xml
--rw-r--r--   0 davisagli   (501) staff       (20)      109 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective/blog/profiles/default/theme.xml
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-03-27 18:11:28.850686 collective.blog-1.0.0a9/src/collective/blog/profiles/default/types/
--rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective/blog/profiles/default/types/.gitkeep
--rw-r--r--   0 davisagli   (501) staff       (20)     2797 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective/blog/profiles/default/types/Author.xml
--rw-r--r--   0 davisagli   (501) staff       (20)     2994 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective/blog/profiles/default/types/BlogFolder.xml
--rw-r--r--   0 davisagli   (501) staff       (20)     2782 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective/blog/profiles/default/types/BlogTag.xml
--rw-r--r--   0 davisagli   (501) staff       (20)     3019 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective/blog/profiles/default/types/Post.xml
--rw-r--r--   0 davisagli   (501) staff       (20)      467 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective/blog/profiles/default/types.xml
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-03-27 18:11:28.850848 collective.blog-1.0.0a9/src/collective/blog/profiles/uninstall/
--rw-r--r--   0 davisagli   (501) staff       (20)      118 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective/blog/profiles/uninstall/browserlayer.xml
--rw-r--r--   0 davisagli   (501) staff       (20)      845 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective/blog/profiles.zcml
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-03-27 18:11:28.851935 collective.blog-1.0.0a9/src/collective/blog/serializers/
--rw-r--r--   0 davisagli   (501) staff       (20)      681 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective/blog/serializers/__init__.py
--rw-r--r--   0 davisagli   (501) staff       (20)      417 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective/blog/serializers/author.py
--rw-r--r--   0 davisagli   (501) staff       (20)      407 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective/blog/serializers/blog.py
--rw-r--r--   0 davisagli   (501) staff       (20)      526 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective/blog/serializers/configure.zcml
--rw-r--r--   0 davisagli   (501) staff       (20)      407 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective/blog/serializers/post.py
--rw-r--r--   0 davisagli   (501) staff       (20)      330 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective/blog/serializers/summary.py
--rw-r--r--   0 davisagli   (501) staff       (20)      455 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective/blog/serializers/vocab.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-03-27 18:11:28.852233 collective.blog-1.0.0a9/src/collective/blog/services/
--rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective/blog/services/__init__.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-03-27 18:11:28.852707 collective.blog-1.0.0a9/src/collective/blog/services/authors/
--rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective/blog/services/authors/__init__.py
--rw-r--r--   0 davisagli   (501) staff       (20)      558 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective/blog/services/authors/configure.zcml
--rw-r--r--   0 davisagli   (501) staff       (20)     2097 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective/blog/services/authors/get.py
--rw-r--r--   0 davisagli   (501) staff       (20)      100 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective/blog/services/configure.zcml
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-03-27 18:11:28.852881 collective.blog-1.0.0a9/src/collective/blog/setuphandlers/
--rw-r--r--   0 davisagli   (501) staff       (20)      335 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective/blog/setuphandlers/__init__.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-03-27 18:11:28.853374 collective.blog-1.0.0a9/src/collective/blog/subscribers/
--rw-r--r--   0 davisagli   (501) staff       (20)        2 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective/blog/subscribers/__init__.py
--rw-r--r--   0 davisagli   (501) staff       (20)     4447 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective/blog/subscribers/blog.py
--rw-r--r--   0 davisagli   (501) staff       (20)      241 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective/blog/subscribers/configure.zcml
--rw-r--r--   0 davisagli   (501) staff       (20)     1530 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective/blog/testing.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-03-27 18:11:28.853991 collective.blog-1.0.0a9/src/collective/blog/upgrades/
--rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective/blog/upgrades/__init__.py
--rw-r--r--   0 davisagli   (501) staff       (20)     2281 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective/blog/upgrades/configure.zcml
--rw-r--r--   0 davisagli   (501) staff       (20)     1396 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective/blog/upgrades/v1002.py
--rw-r--r--   0 davisagli   (501) staff       (20)      521 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective/blog/upgrades/v1003.py
--rw-r--r--   0 davisagli   (501) staff       (20)      502 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective/blog/utils.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-03-27 18:11:28.854594 collective.blog-1.0.0a9/src/collective/blog/vocabularies/
--rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective/blog/vocabularies/__init__.py
--rw-r--r--   0 davisagli   (501) staff       (20)      775 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective/blog/vocabularies/authors.py
--rw-r--r--   0 davisagli   (501) staff       (20)      264 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective/blog/vocabularies/configure.zcml
--rw-r--r--   0 davisagli   (501) staff       (20)     1022 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective/blog/vocabularies/tags.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-03-27 18:11:28.857484 collective.blog-1.0.0a9/src/collective.blog.egg-info/
--rw-r--r--   0 davisagli   (501) staff       (20)     8672 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective.blog.egg-info/PKG-INFO
--rw-r--r--   0 davisagli   (501) staff       (20)     4655 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective.blog.egg-info/SOURCES.txt
--rw-r--r--   0 davisagli   (501) staff       (20)        1 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective.blog.egg-info/dependency_links.txt
--rw-r--r--   0 davisagli   (501) staff       (20)      120 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective.blog.egg-info/entry_points.txt
--rw-r--r--   0 davisagli   (501) staff       (20)       11 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective.blog.egg-info/namespace_packages.txt
--rw-r--r--   0 davisagli   (501) staff       (20)        1 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective.blog.egg-info/not-zip-safe
--rw-r--r--   0 davisagli   (501) staff       (20)      175 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective.blog.egg-info/requires.txt
--rw-r--r--   0 davisagli   (501) staff       (20)       11 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/src/collective.blog.egg-info/top_level.txt
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-03-27 18:11:28.854751 collective.blog-1.0.0a9/tests/
--rw-r--r--   0 davisagli   (501) staff       (20)     7329 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/tests/conftest.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-03-27 18:11:28.855357 collective.blog-1.0.0a9/tests/content/
--rw-r--r--   0 davisagli   (501) staff       (20)     2902 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/tests/content/test_author.py
--rw-r--r--   0 davisagli   (501) staff       (20)     5202 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/tests/content/test_blog.py
--rw-r--r--   0 davisagli   (501) staff       (20)     3376 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/tests/content/test_post.py
--rw-r--r--   0 davisagli   (501) staff       (20)     2854 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/tests/content/test_tag.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-03-27 18:11:28.855686 collective.blog-1.0.0a9/tests/controlpanel/
--rw-r--r--   0 davisagli   (501) staff       (20)      193 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/tests/controlpanel/conftest.py
--rw-r--r--   0 davisagli   (501) staff       (20)     2507 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/tests/controlpanel/test_controlpanel.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-03-27 18:11:28.855995 collective.blog-1.0.0a9/tests/restapi/
--rw-r--r--   0 davisagli   (501) staff       (20)     1957 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/tests/restapi/conftest.py
--rw-r--r--   0 davisagli   (501) staff       (20)     1849 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/tests/restapi/test_service_authors.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-03-27 18:11:28.856536 collective.blog-1.0.0a9/tests/setup/
--rw-r--r--   0 davisagli   (501) staff       (20)      631 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/tests/setup/test_setup_install.py
--rw-r--r--   0 davisagli   (501) staff       (20)      677 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/tests/setup/test_setup_navigation.py
--rw-r--r--   0 davisagli   (501) staff       (20)      614 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/tests/setup/test_setup_uninstall.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-03-27 18:11:28.856860 collective.blog-1.0.0a9/tests/setup/upgrades/
--rw-r--r--   0 davisagli   (501) staff       (20)      641 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/tests/setup/upgrades/conftest.py
--rw-r--r--   0 davisagli   (501) staff       (20)     3330 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/tests/setup/upgrades/test_upgrades_to_v1002.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-03-27 18:11:28.857216 collective.blog-1.0.0a9/tests/vocabularies/
--rw-r--r--   0 davisagli   (501) staff       (20)     1242 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/tests/vocabularies/test_vocab_authors.py
--rw-r--r--   0 davisagli   (501) staff       (20)     1181 2024-03-27 18:11:28.000000 collective.blog-1.0.0a9/tests/vocabularies/test_vocab_tags.py
+drwxrwxr-x   0 pcdummy   (1000) pcdummy   (1000)        0 2016-02-14 18:26:35.000000 collective.blog-1.0a1/
+drwxrwxr-x   0 pcdummy   (1000) pcdummy   (1000)        0 2016-02-14 18:26:35.000000 collective.blog-1.0a1/docs/
+-rw-rw-r--   0 pcdummy   (1000) pcdummy   (1000)    18092 2016-02-14 18:26:34.000000 collective.blog-1.0a1/docs/LICENSE.GPL
+-rw-rw-r--   0 pcdummy   (1000) pcdummy   (1000)      657 2016-02-14 18:26:34.000000 collective.blog-1.0a1/docs/LICENSE.rst
+-rw-rw-r--   0 pcdummy   (1000) pcdummy   (1000)       78 2016-02-14 18:26:34.000000 collective.blog-1.0a1/docs/index.rst
+drwxrwxr-x   0 pcdummy   (1000) pcdummy   (1000)        0 2016-02-14 18:26:35.000000 collective.blog-1.0a1/src/
+drwxrwxr-x   0 pcdummy   (1000) pcdummy   (1000)        0 2016-02-14 18:26:35.000000 collective.blog-1.0a1/src/collective/
+drwxrwxr-x   0 pcdummy   (1000) pcdummy   (1000)        0 2016-02-14 18:26:35.000000 collective.blog-1.0a1/src/collective/blog/
+drwxrwxr-x   0 pcdummy   (1000) pcdummy   (1000)        0 2016-02-14 18:26:35.000000 collective.blog-1.0a1/src/collective/blog/browser/
+drwxrwxr-x   0 pcdummy   (1000) pcdummy   (1000)        0 2016-02-14 18:26:35.000000 collective.blog-1.0a1/src/collective/blog/browser/static/
+drwxrwxr-x   0 pcdummy   (1000) pcdummy   (1000)        0 2016-02-14 18:26:35.000000 collective.blog-1.0a1/src/collective/blog/browser/static/less/
+-rw-rw-r--   0 pcdummy   (1000) pcdummy   (1000)      259 2016-02-14 18:26:34.000000 collective.blog-1.0a1/src/collective/blog/browser/static/less/blog.less
+-rw-rw-r--   0 pcdummy   (1000) pcdummy   (1000)        0 2016-02-14 18:26:34.000000 collective.blog-1.0a1/src/collective/blog/browser/static/.gitkeep
+-rw-rw-r--   0 pcdummy   (1000) pcdummy   (1000)        0 2016-02-14 18:26:34.000000 collective.blog-1.0a1/src/collective/blog/browser/__init__.py
+-rw-rw-r--   0 pcdummy   (1000) pcdummy   (1000)     3663 2016-02-14 18:26:34.000000 collective.blog-1.0a1/src/collective/blog/browser/blog_entry.pt
+-rw-rw-r--   0 pcdummy   (1000) pcdummy   (1000)      709 2016-02-14 18:26:34.000000 collective.blog-1.0a1/src/collective/blog/browser/blog_entry.py
+-rw-rw-r--   0 pcdummy   (1000) pcdummy   (1000)     6467 2016-02-14 18:26:34.000000 collective.blog-1.0a1/src/collective/blog/browser/blog_listing.pt
+-rw-rw-r--   0 pcdummy   (1000) pcdummy   (1000)     6255 2016-02-14 18:26:34.000000 collective.blog-1.0a1/src/collective/blog/browser/blog_listing.py
+-rw-rw-r--   0 pcdummy   (1000) pcdummy   (1000)      771 2016-02-14 18:26:34.000000 collective.blog-1.0a1/src/collective/blog/browser/configure.zcml
+drwxrwxr-x   0 pcdummy   (1000) pcdummy   (1000)        0 2016-02-14 18:26:35.000000 collective.blog-1.0a1/src/collective/blog/content/
+-rw-rw-r--   0 pcdummy   (1000) pcdummy   (1000)        0 2016-02-14 18:26:34.000000 collective.blog-1.0a1/src/collective/blog/content/__init__.py
+-rw-rw-r--   0 pcdummy   (1000) pcdummy   (1000)     4853 2016-02-14 18:26:34.000000 collective.blog-1.0a1/src/collective/blog/content/blog_entry.py
+-rw-rw-r--   0 pcdummy   (1000) pcdummy   (1000)     1308 2016-02-14 18:26:34.000000 collective.blog-1.0a1/src/collective/blog/content/configure.zcml
+drwxrwxr-x   0 pcdummy   (1000) pcdummy   (1000)        0 2016-02-14 18:26:35.000000 collective.blog-1.0a1/src/collective/blog/locales/
+-rw-rw-r--   0 pcdummy   (1000) pcdummy   (1000)        0 2016-02-14 18:26:34.000000 collective.blog-1.0a1/src/collective/blog/locales/collective.blog.pot
+-rwxrwxr-x   0 pcdummy   (1000) pcdummy   (1000)      482 2016-02-14 18:26:34.000000 collective.blog-1.0a1/src/collective/blog/locales/update.sh
+drwxrwxr-x   0 pcdummy   (1000) pcdummy   (1000)        0 2016-02-14 18:26:35.000000 collective.blog-1.0a1/src/collective/blog/portlets/
+-rw-rw-r--   0 pcdummy   (1000) pcdummy   (1000)        0 2016-02-14 18:26:34.000000 collective.blog-1.0a1/src/collective/blog/portlets/__init__.py
+-rw-rw-r--   0 pcdummy   (1000) pcdummy   (1000)      559 2016-02-14 18:26:34.000000 collective.blog-1.0a1/src/collective/blog/portlets/configure.zcml
+-rw-rw-r--   0 pcdummy   (1000) pcdummy   (1000)      760 2016-02-14 18:26:34.000000 collective.blog-1.0a1/src/collective/blog/portlets/tags.pt
+-rw-rw-r--   0 pcdummy   (1000) pcdummy   (1000)     7580 2016-02-14 18:26:34.000000 collective.blog-1.0a1/src/collective/blog/portlets/tags.py
+drwxrwxr-x   0 pcdummy   (1000) pcdummy   (1000)        0 2016-02-14 18:26:35.000000 collective.blog-1.0a1/src/collective/blog/profiles/
+drwxrwxr-x   0 pcdummy   (1000) pcdummy   (1000)        0 2016-02-14 18:26:35.000000 collective.blog-1.0a1/src/collective/blog/profiles/default/
+drwxrwxr-x   0 pcdummy   (1000) pcdummy   (1000)        0 2016-02-14 18:26:35.000000 collective.blog-1.0a1/src/collective/blog/profiles/default/types/
+-rw-rw-r--   0 pcdummy   (1000) pcdummy   (1000)      169 2016-02-14 18:26:34.000000 collective.blog-1.0a1/src/collective/blog/profiles/default/types/Collection.xml
+-rw-rw-r--   0 pcdummy   (1000) pcdummy   (1000)      165 2016-02-14 18:26:34.000000 collective.blog-1.0a1/src/collective/blog/profiles/default/types/Folder.xml
+-rw-rw-r--   0 pcdummy   (1000) pcdummy   (1000)      169 2016-02-14 18:26:34.000000 collective.blog-1.0a1/src/collective/blog/profiles/default/types/Plone_Site.xml
+-rw-rw-r--   0 pcdummy   (1000) pcdummy   (1000)     2834 2016-02-14 18:26:34.000000 collective.blog-1.0a1/src/collective/blog/profiles/default/types/collective.blog.blogentry.xml
+-rw-rw-r--   0 pcdummy   (1000) pcdummy   (1000)      154 2016-02-14 18:26:34.000000 collective.blog-1.0a1/src/collective/blog/profiles/default/browserlayer.xml
+-rw-rw-r--   0 pcdummy   (1000) pcdummy   (1000)      239 2016-02-14 18:26:34.000000 collective.blog-1.0a1/src/collective/blog/profiles/default/catalog.xml
+-rw-rw-r--   0 pcdummy   (1000) pcdummy   (1000)        0 2016-02-14 18:26:34.000000 collective.blog-1.0a1/src/collective/blog/profiles/default/collectiveblog_default.txt
+-rw-rw-r--   0 pcdummy   (1000) pcdummy   (1000)      171 2016-02-14 18:26:34.000000 collective.blog-1.0a1/src/collective/blog/profiles/default/metadata.xml
+-rw-rw-r--   0 pcdummy   (1000) pcdummy   (1000)      209 2016-02-14 18:26:34.000000 collective.blog-1.0a1/src/collective/blog/profiles/default/portlets.xml
+-rw-rw-r--   0 pcdummy   (1000) pcdummy   (1000)      832 2016-02-14 18:26:34.000000 collective.blog-1.0a1/src/collective/blog/profiles/default/registry.xml
+-rw-rw-r--   0 pcdummy   (1000) pcdummy   (1000)      309 2016-02-14 18:26:34.000000 collective.blog-1.0a1/src/collective/blog/profiles/default/types.xml
+drwxrwxr-x   0 pcdummy   (1000) pcdummy   (1000)        0 2016-02-14 18:26:35.000000 collective.blog-1.0a1/src/collective/blog/profiles/uninstall/
+drwxrwxr-x   0 pcdummy   (1000) pcdummy   (1000)        0 2016-02-14 18:26:35.000000 collective.blog-1.0a1/src/collective/blog/profiles/uninstall/types/
+-rw-rw-r--   0 pcdummy   (1000) pcdummy   (1000)      183 2016-02-14 18:26:34.000000 collective.blog-1.0a1/src/collective/blog/profiles/uninstall/types/Collection.xml
+-rw-rw-r--   0 pcdummy   (1000) pcdummy   (1000)      178 2016-02-14 18:26:34.000000 collective.blog-1.0a1/src/collective/blog/profiles/uninstall/types/Folder.xml
+-rw-rw-r--   0 pcdummy   (1000) pcdummy   (1000)      182 2016-02-14 18:26:34.000000 collective.blog-1.0a1/src/collective/blog/profiles/uninstall/types/Plone_Site.xml
+-rw-rw-r--   0 pcdummy   (1000) pcdummy   (1000)      107 2016-02-14 18:26:34.000000 collective.blog-1.0a1/src/collective/blog/profiles/uninstall/browserlayer.xml
+-rw-rw-r--   0 pcdummy   (1000) pcdummy   (1000)      135 2016-02-14 18:26:34.000000 collective.blog-1.0a1/src/collective/blog/profiles/uninstall/catalog.xml
+-rw-rw-r--   0 pcdummy   (1000) pcdummy   (1000)        0 2016-02-14 18:26:34.000000 collective.blog-1.0a1/src/collective/blog/profiles/uninstall/collectiveblog_uninstall.txt
+-rw-rw-r--   0 pcdummy   (1000) pcdummy   (1000)      133 2016-02-14 18:26:34.000000 collective.blog-1.0a1/src/collective/blog/profiles/uninstall/portlets.xml
+-rw-rw-r--   0 pcdummy   (1000) pcdummy   (1000)      269 2016-02-14 18:26:34.000000 collective.blog-1.0a1/src/collective/blog/profiles/uninstall/registry.xml
+-rw-rw-r--   0 pcdummy   (1000) pcdummy   (1000)      175 2016-02-14 18:26:34.000000 collective.blog-1.0a1/src/collective/blog/profiles/uninstall/types.xml
+drwxrwxr-x   0 pcdummy   (1000) pcdummy   (1000)        0 2016-02-14 18:26:35.000000 collective.blog-1.0a1/src/collective/blog/tests/
+drwxrwxr-x   0 pcdummy   (1000) pcdummy   (1000)        0 2016-02-14 18:26:35.000000 collective.blog-1.0a1/src/collective/blog/tests/robot/
+-rw-rw-r--   0 pcdummy   (1000) pcdummy   (1000)     2655 2016-02-14 18:26:34.000000 collective.blog-1.0a1/src/collective/blog/tests/robot/test_blogentry.robot
+-rw-rw-r--   0 pcdummy   (1000) pcdummy   (1000)     1991 2016-02-14 18:26:34.000000 collective.blog-1.0a1/src/collective/blog/tests/robot/test_example.robot
+-rw-rw-r--   0 pcdummy   (1000) pcdummy   (1000)        0 2016-02-14 18:26:34.000000 collective.blog-1.0a1/src/collective/blog/tests/__init__.py
+-rw-rw-r--   0 pcdummy   (1000) pcdummy   (1000)     1442 2016-02-14 18:26:34.000000 collective.blog-1.0a1/src/collective/blog/tests/test_blogentry.py
+-rw-rw-r--   0 pcdummy   (1000) pcdummy   (1000)      874 2016-02-14 18:26:34.000000 collective.blog-1.0a1/src/collective/blog/tests/test_robot.py
+-rw-rw-r--   0 pcdummy   (1000) pcdummy   (1000)     1757 2016-02-14 18:26:34.000000 collective.blog-1.0a1/src/collective/blog/tests/test_setup.py
+drwxrwxr-x   0 pcdummy   (1000) pcdummy   (1000)        0 2016-02-14 18:26:35.000000 collective.blog-1.0a1/src/collective/blog/viewlets/
+-rw-rw-r--   0 pcdummy   (1000) pcdummy   (1000)        0 2016-02-14 18:26:34.000000 collective.blog-1.0a1/src/collective/blog/viewlets/__init__.py
+-rw-rw-r--   0 pcdummy   (1000) pcdummy   (1000)     1326 2016-02-14 18:26:34.000000 collective.blog-1.0a1/src/collective/blog/viewlets/blog_byline.pt
+-rw-rw-r--   0 pcdummy   (1000) pcdummy   (1000)     1106 2016-02-14 18:26:34.000000 collective.blog-1.0a1/src/collective/blog/viewlets/blog_byline.py
+-rw-rw-r--   0 pcdummy   (1000) pcdummy   (1000)      513 2016-02-14 18:26:34.000000 collective.blog-1.0a1/src/collective/blog/viewlets/configure.zcml
+-rw-rw-r--   0 pcdummy   (1000) pcdummy   (1000)      132 2016-02-14 18:26:34.000000 collective.blog-1.0a1/src/collective/blog/__init__.py
+-rw-rw-r--   0 pcdummy   (1000) pcdummy   (1000)     1622 2016-02-14 18:26:34.000000 collective.blog-1.0a1/src/collective/blog/configure.zcml
+-rw-rw-r--   0 pcdummy   (1000) pcdummy   (1000)     1054 2016-02-14 18:26:34.000000 collective.blog-1.0a1/src/collective/blog/interfaces.py
+-rw-rw-r--   0 pcdummy   (1000) pcdummy   (1000)     2576 2016-02-14 18:26:34.000000 collective.blog-1.0a1/src/collective/blog/setuphandlers.py
+-rw-rw-r--   0 pcdummy   (1000) pcdummy   (1000)     1285 2016-02-14 18:26:34.000000 collective.blog-1.0a1/src/collective/blog/testing.py
+-rw-rw-r--   0 pcdummy   (1000) pcdummy   (1000)       80 2016-02-14 18:26:34.000000 collective.blog-1.0a1/src/collective/__init__.py
+drwxrwxr-x   0 pcdummy   (1000) pcdummy   (1000)        0 2016-02-14 18:26:35.000000 collective.blog-1.0a1/src/collective.blog.egg-info/
+-rw-rw-r--   0 pcdummy   (1000) pcdummy   (1000)     5437 2016-02-14 18:26:35.000000 collective.blog-1.0a1/src/collective.blog.egg-info/PKG-INFO
+-rw-rw-r--   0 pcdummy   (1000) pcdummy   (1000)     2938 2016-02-14 18:26:35.000000 collective.blog-1.0a1/src/collective.blog.egg-info/SOURCES.txt
+-rw-rw-r--   0 pcdummy   (1000) pcdummy   (1000)        1 2016-02-14 18:26:35.000000 collective.blog-1.0a1/src/collective.blog.egg-info/dependency_links.txt
+-rw-rw-r--   0 pcdummy   (1000) pcdummy   (1000)       53 2016-02-14 18:26:35.000000 collective.blog-1.0a1/src/collective.blog.egg-info/entry_points.txt
+-rw-rw-r--   0 pcdummy   (1000) pcdummy   (1000)       11 2016-02-14 18:26:35.000000 collective.blog-1.0a1/src/collective.blog.egg-info/namespace_packages.txt
+-rw-rw-r--   0 pcdummy   (1000) pcdummy   (1000)        1 2016-02-14 18:26:35.000000 collective.blog-1.0a1/src/collective.blog.egg-info/not-zip-safe
+-rw-rw-r--   0 pcdummy   (1000) pcdummy   (1000)      122 2016-02-14 18:26:35.000000 collective.blog-1.0a1/src/collective.blog.egg-info/requires.txt
+-rw-rw-r--   0 pcdummy   (1000) pcdummy   (1000)       11 2016-02-14 18:26:35.000000 collective.blog-1.0a1/src/collective.blog.egg-info/top_level.txt
+-rw-rw-r--   0 pcdummy   (1000) pcdummy   (1000)       92 2016-02-14 18:26:34.000000 collective.blog-1.0a1/CHANGES.rst
+-rw-rw-r--   0 pcdummy   (1000) pcdummy   (1000)       31 2016-02-14 18:26:34.000000 collective.blog-1.0a1/CONTRIBUTORS.rst
+-rw-rw-r--   0 pcdummy   (1000) pcdummy   (1000)       88 2016-02-14 18:26:34.000000 collective.blog-1.0a1/MANIFEST.in
+-rw-rw-r--   0 pcdummy   (1000) pcdummy   (1000)     3413 2016-02-14 18:26:34.000000 collective.blog-1.0a1/README.rst
+-rw-rw-r--   0 pcdummy   (1000) pcdummy   (1000)     1631 2016-02-14 18:26:34.000000 collective.blog-1.0a1/setup.py
+-rw-rw-r--   0 pcdummy   (1000) pcdummy   (1000)     5437 2016-02-14 18:26:35.000000 collective.blog-1.0a1/PKG-INFO
+-rw-rw-r--   0 pcdummy   (1000) pcdummy   (1000)      161 2016-02-14 18:26:35.000000 collective.blog-1.0a1/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `collective.blog-1.0.0a9/LICENSE.GPL` & `collective.blog-1.0a1/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `collective.blog-1.0.0a9/src/collective/blog/interfaces.py` & `collective.blog-1.0a1/src/collective/blog/interfaces.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,31 +1,40 @@
+# -*- coding: utf-8 -*-
 """Module where all interfaces, events and exceptions live."""
-from collective.blog import _
+
 from zope import schema
 from zope.interface import Interface
 from zope.publisher.interfaces.browser import IDefaultBrowserLayer
 
+from . import _
+
 
-class IBrowserLayer(IDefaultBrowserLayer):
+class ICollectiveBlogLayer(IDefaultBrowserLayer):
     """Marker interface that defines a browser layer."""
 
 
 class IBlogSettings(Interface):
-    enable_authors_folder = schema.Bool(
-        title=_("Authors container inside the Blog"),
-        description=_(
-            "help_enable_authors_folder",
-            default="Should we create the Authors container inside the Blog?",
-        ),
-        required=False,
-        default=True,
-    )
-
-    enable_tags_folder = schema.Bool(
-        title=_("Tags container inside the Blog"),
-        description=_(
-            "help_enable_tags_folder",
-            default="Should we create the Tags container inside the Blog?",
-        ),
-        required=False,
-        default=True,
-    )
+    """ Marker Interface for Registry Settings of this
+    Addon.
+    """
+
+    show_lead_image = schema.Bool(
+        title=_(u"Show lead image in blog entries"),
+        default=False)
+
+    batch_size = schema.Int(
+        title=_(u"Number of blog entries to show on "
+                u"batch (prev/next) navigations"),
+        default=10)
+
+    show_folder_title = schema.Bool(
+        title=_(u"Show the folders title on blog listings"),
+        default=False)
+
+    allow_anonymous_view_about = schema.Bool(
+        title=_(u"Allow anonymous users to see the about line"),
+        default=False)
+
+
+class IBlogEntryView(Interface):
+    """Marker Interface for BlogView
+    """
```

