# Comparing `tmp/Products.PortalTransforms-4.0.2.tar.gz` & `tmp/products_portaltransforms-4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Products.PortalTransforms-4.0.2.tar", last modified: Mon Jan 22 20:04:46 2024, max compression
+gzip compressed data, was "products_portaltransforms-4.0.3.tar", last modified: Thu Apr 25 19:36:35 2024, max compression
```

## Comparing `Products.PortalTransforms-4.0.2.tar` & `products_portaltransforms-4.0.3.tar`

### file list

```diff
@@ -1,162 +1,162 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-01-22 20:04:46.261197 Products.PortalTransforms-4.0.2/
--rw-r--r--   0 maurits    (501) staff       (20)     1342 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/.editorconfig
--rw-r--r--   0 maurits    (501) staff       (20)      540 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/.flake8
--rw-r--r--   0 maurits    (501) staff       (20)      663 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/.gitignore
--rw-r--r--   0 maurits    (501) staff       (20)      590 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/.meta.toml
--rw-r--r--   0 maurits    (501) staff       (20)     1940 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/.pre-commit-config.yaml
--rw-r--r--   0 maurits    (501) staff       (20)    22724 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      170 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    25343 2024-01-22 20:04:46.260399 Products.PortalTransforms-4.0.2/PKG-INFO
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-01-22 20:04:46.210378 Products.PortalTransforms-4.0.2/Products/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-01-22 20:04:46.218226 Products.PortalTransforms-4.0.2/Products/PortalTransforms/
--rw-r--r--   0 maurits    (501) staff       (20)    11462 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/Transform.py
--rw-r--r--   0 maurits    (501) staff       (20)    25608 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/TransformEngine.py
--rw-r--r--   0 maurits    (501) staff       (20)       82 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/TransformTool.py
--rw-r--r--   0 maurits    (501) staff       (20)      742 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1970 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/cache.py
--rw-r--r--   0 maurits    (501) staff       (20)     7401 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/chain.py
--rw-r--r--   0 maurits    (501) staff       (20)      649 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1862 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/data.py
--rw-r--r--   0 maurits    (501) staff       (20)     3684 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/interfaces.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-01-22 20:04:46.220077 Products.PortalTransforms-4.0.2/Products/PortalTransforms/libtransforms/
--rw-r--r--   0 maurits    (501) staff       (20)       88 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/libtransforms/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     2711 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/libtransforms/commandtransform.py
--rw-r--r--   0 maurits    (501) staff       (20)      987 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/libtransforms/piltransform.py
--rw-r--r--   0 maurits    (501) staff       (20)      795 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/libtransforms/retransform.py
--rw-r--r--   0 maurits    (501) staff       (20)     3019 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/libtransforms/utils.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-01-22 20:04:46.203971 Products.PortalTransforms-4.0.2/Products/PortalTransforms/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-01-22 20:04:46.221809 Products.PortalTransforms-4.0.2/Products/PortalTransforms/profiles/default/
--rw-r--r--   0 maurits    (501) staff       (20)      255 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/profiles/default/componentregistry.xml
--rw-r--r--   0 maurits    (501) staff       (20)      391 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/profiles/default/import_steps.xml
--rw-r--r--   0 maurits    (501) staff       (20)       87 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/profiles/default/metadata.xml
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/profiles/default/portal-transforms-various.txt
--rw-r--r--   0 maurits    (501) staff       (20)      187 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/profiles/default/toolset.xml
--rw-r--r--   0 maurits    (501) staff       (20)     2483 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/setuphandlers.py
--rw-r--r--   0 maurits    (501) staff       (20)      986 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/testing.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-01-22 20:04:46.225127 Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      368 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/base.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-01-22 20:04:46.232132 Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/input/
--rw-r--r--   0 maurits    (501) staff       (20)   106910 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/input/demo1.pdf
--rw-r--r--   0 maurits    (501) staff       (20)      226 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/input/input.textile
--rw-r--r--   0 maurits    (501) staff       (20)     1710 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/input/logo.bmp
--rw-r--r--   0 maurits    (501) staff       (20)     1317 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/input/logo.gif
--rw-r--r--   0 maurits    (501) staff       (20)      801 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/input/logo.jpg
--rw-r--r--   0 maurits    (501) staff       (20)     1773 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/input/logo.png
--rw-r--r--   0 maurits    (501) staff       (20)      101 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/input/markdown.txt
--rw-r--r--   0 maurits    (501) staff       (20)     7278 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/input/org-news.xml
--rw-r--r--   0 maurits    (501) staff       (20)       73 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/input/rest1.rst
--rw-r--r--   0 maurits    (501) staff       (20)      152 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/input/rest2.rst
--rw-r--r--   0 maurits    (501) staff       (20)      338 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/input/rest3.rst
--rw-r--r--   0 maurits    (501) staff       (20)     1505 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/input/rss2html.xslt
--rw-r--r--   0 maurits    (501) staff       (20)     7680 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/input/test.doc
--rw-r--r--   0 maurits    (501) staff       (20)       25 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/input/test_invalid_tags.html
--rw-r--r--   0 maurits    (501) staff       (20)     9729 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/input/test_js.doc
--rw-r--r--   0 maurits    (501) staff       (20)       29 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/input/test_js_on.html
--rw-r--r--   0 maurits    (501) staff       (20)       37 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/input/test_js_uri.html
--rw-r--r--   0 maurits    (501) staff       (20)     3224 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/input/test_lynx.html
--rw-r--r--   0 maurits    (501) staff       (20)      147 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/input/test_python.py
--rw-r--r--   0 maurits    (501) staff       (20)      956 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/input/test_safehtml.html
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-01-22 20:04:46.239754 Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/output/
--rw-r--r--   0 maurits    (501) staff       (20)    22253 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/output/demo1.html
--rw-r--r--   0 maurits    (501) staff       (20)    22253 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/output/demo1.html.nofilename
--rw-r--r--   0 maurits    (501) staff       (20)     1710 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/output/logo.bmp
--rw-r--r--   0 maurits    (501) staff       (20)     1422 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/output/logo.gif
--rw-r--r--   0 maurits    (501) staff       (20)      805 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/output/logo.jpg
--rw-r--r--   0 maurits    (501) staff       (20)     3086 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/output/logo.pcx
--rw-r--r--   0 maurits    (501) staff       (20)     1773 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/output/logo.png
--rw-r--r--   0 maurits    (501) staff       (20)     1669 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/output/logo.ppm
--rw-r--r--   0 maurits    (501) staff       (20)     1796 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/output/logo.tiff
--rw-r--r--   0 maurits    (501) staff       (20)      161 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/output/markdown.html
--rw-r--r--   0 maurits    (501) staff       (20)     3025 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/output/org-news.html
--rw-r--r--   0 maurits    (501) staff       (20)       92 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/output/rest1.html
--rw-r--r--   0 maurits    (501) staff       (20)      112 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/output/rest1.out
--rw-r--r--   0 maurits    (501) staff       (20)       73 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/output/rest1.rst
--rw-r--r--   0 maurits    (501) staff       (20)      244 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/output/rest2.out
--rw-r--r--   0 maurits    (501) staff       (20)      482 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/output/rest3.out
--rw-r--r--   0 maurits    (501) staff       (20)     1511 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/output/test_html_to_text.txt
--rw-r--r--   0 maurits    (501) staff       (20)     2053 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/output/test_lynx.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1308 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/output/test_python.out
--rw-r--r--   0 maurits    (501) staff       (20)      531 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/output/test_safe.html
--rw-r--r--   0 maurits    (501) staff       (20)      266 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/output/test_word.html
--rw-r--r--   0 maurits    (501) staff       (20)      367 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/output/textile.html
--rw-r--r--   0 maurits    (501) staff       (20)      275 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/test_doctests.py
--rw-r--r--   0 maurits    (501) staff       (20)    10342 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/test_engine.py
--rw-r--r--   0 maurits    (501) staff       (20)     3916 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/test_graph.py
--rw-r--r--   0 maurits    (501) staff       (20)     5807 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/test_intelligenttext.py
--rw-r--r--   0 maurits    (501) staff       (20)       37 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/test_js_uri.html
--rw-r--r--   0 maurits    (501) staff       (20)    24689 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/test_transforms.py
--rw-r--r--   0 maurits    (501) staff       (20)     9628 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/test_xss.py
--rw-r--r--   0 maurits    (501) staff       (20)     1948 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/utils.py
--rw-r--r--   0 maurits    (501) staff       (20)      339 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/tool.gif
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-01-22 20:04:46.252143 Products.PortalTransforms-4.0.2/Products/PortalTransforms/transforms/
--rw-r--r--   0 maurits    (501) staff       (20)     2805 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/transforms/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      820 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/transforms/broken.py
--rw-r--r--   0 maurits    (501) staff       (20)      998 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/transforms/html_body.py
--rw-r--r--   0 maurits    (501) staff       (20)     1102 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/transforms/html_to_text.py
--rw-r--r--   0 maurits    (501) staff       (20)     1263 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/transforms/html_to_web_intelligent_plain_text.py
--rw-r--r--   0 maurits    (501) staff       (20)     1087 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/transforms/identity.py
--rw-r--r--   0 maurits    (501) staff       (20)      265 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/transforms/image_to_bmp.py
--rw-r--r--   0 maurits    (501) staff       (20)      260 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/transforms/image_to_gif.py
--rw-r--r--   0 maurits    (501) staff       (20)      440 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/transforms/image_to_html.py
--rw-r--r--   0 maurits    (501) staff       (20)      265 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/transforms/image_to_jpeg.py
--rw-r--r--   0 maurits    (501) staff       (20)      260 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/transforms/image_to_pcx.py
--rw-r--r--   0 maurits    (501) staff       (20)      260 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/transforms/image_to_png.py
--rw-r--r--   0 maurits    (501) staff       (20)      274 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/transforms/image_to_ppm.py
--rw-r--r--   0 maurits    (501) staff       (20)      265 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/transforms/image_to_tiff.py
--rw-r--r--   0 maurits    (501) staff       (20)      497 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/transforms/lynx_dump.py
--rw-r--r--   0 maurits    (501) staff       (20)     1537 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/transforms/markdown_to_html.py
--rw-r--r--   0 maurits    (501) staff       (20)     2584 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/transforms/office_com.py
--rw-r--r--   0 maurits    (501) staff       (20)     2029 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/transforms/office_uno.py
--rw-r--r--   0 maurits    (501) staff       (20)     1449 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/transforms/office_wvware.py
--rw-r--r--   0 maurits    (501) staff       (20)     2280 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/transforms/pdf_to_html.py
--rw-r--r--   0 maurits    (501) staff       (20)      517 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/transforms/pdf_to_text.py
--rw-r--r--   0 maurits    (501) staff       (20)     4728 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/transforms/python.py
--rw-r--r--   0 maurits    (501) staff       (20)     4886 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/transforms/rest.py
--rw-r--r--   0 maurits    (501) staff       (20)     1764 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/transforms/rtf_to_html.py
--rw-r--r--   0 maurits    (501) staff       (20)     1652 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/transforms/rtf_to_xml.py
--rw-r--r--   0 maurits    (501) staff       (20)     6402 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/transforms/safe_html.py
--rw-r--r--   0 maurits    (501) staff       (20)      596 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/transforms/st.py
--rw-r--r--   0 maurits    (501) staff       (20)     1008 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/transforms/text_pre_to_html.py
--rw-r--r--   0 maurits    (501) staff       (20)     1221 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/transforms/text_to_html.py
--rw-r--r--   0 maurits    (501) staff       (20)      941 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/transforms/textile_to_html.py
--rw-r--r--   0 maurits    (501) staff       (20)     1289 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/transforms/web_intelligent_plain_text_to_html.py
--rw-r--r--   0 maurits    (501) staff       (20)     1510 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/transforms/word_to_html.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-01-22 20:04:46.253174 Products.PortalTransforms-4.0.2/Products/PortalTransforms/unsafe_transforms/
--rw-r--r--   0 maurits    (501) staff       (20)     3014 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/unsafe_transforms/build_transforms.py
--rw-r--r--   0 maurits    (501) staff       (20)     3591 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/unsafe_transforms/command.py
--rw-r--r--   0 maurits    (501) staff       (20)     6213 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/unsafe_transforms/xml.py
--rw-r--r--   0 maurits    (501) staff       (20)      556 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/utils.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-01-22 20:04:46.256273 Products.PortalTransforms-4.0.2/Products/PortalTransforms/www/
--rw-r--r--   0 maurits    (501) staff       (20)     1191 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/www/addTransform.zpt
--rw-r--r--   0 maurits    (501) staff       (20)     1183 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/www/addTransformsChain.zpt
--rw-r--r--   0 maurits    (501) staff       (20)     2868 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/www/configureTransform.zpt
--rw-r--r--   0 maurits    (501) staff       (20)     2273 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/www/editTransformationPolicy.zpt
--rw-r--r--   0 maurits    (501) staff       (20)     2788 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/www/editTransformsChain.zpt
--rw-r--r--   0 maurits    (501) staff       (20)      634 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/www/reloadAllTransforms.zpt
--rw-r--r--   0 maurits    (501) staff       (20)      505 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/www/reloadTransform.zpt
--rw-r--r--   0 maurits    (501) staff       (20)     1082 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/www/setCacheTime.zpt
--rw-r--r--   0 maurits    (501) staff       (20)     2103 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/PortalTransforms/www/tr_widgets.zpt
--rw-r--r--   0 maurits    (501) staff       (20)      245 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/Products/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-01-22 20:04:46.259497 Products.PortalTransforms-4.0.2/Products.PortalTransforms.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    25343 2024-01-22 20:04:46.000000 Products.PortalTransforms-4.0.2/Products.PortalTransforms.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     6662 2024-01-22 20:04:46.000000 Products.PortalTransforms-4.0.2/Products.PortalTransforms.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2024-01-22 20:04:46.000000 Products.PortalTransforms-4.0.2/Products.PortalTransforms.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)        9 2024-01-22 20:04:46.000000 Products.PortalTransforms-4.0.2/Products.PortalTransforms.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2024-01-22 20:04:46.000000 Products.PortalTransforms-4.0.2/Products.PortalTransforms.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      289 2024-01-22 20:04:46.000000 Products.PortalTransforms-4.0.2/Products.PortalTransforms.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        9 2024-01-22 20:04:46.000000 Products.PortalTransforms-4.0.2/Products.PortalTransforms.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1049 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-01-22 20:04:46.259118 Products.PortalTransforms-4.0.2/docs/
--rw-r--r--   0 maurits    (501) staff       (20)     8682 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/docs/ChangeLog
--rw-r--r--   0 maurits    (501) staff       (20)     1600 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/docs/LICENSE.txt
--rw-r--r--   0 maurits    (501) staff       (20)      273 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/docs/TODO
--rw-r--r--   0 maurits    (501) staff       (20)     7166 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/docs/dev_manual.rst
--rw-r--r--   0 maurits    (501) staff       (20)      271 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/docs/makefile
--rw-r--r--   0 maurits    (501) staff       (20)     3972 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/docs/uno_setup.rst
--rw-r--r--   0 maurits    (501) staff       (20)     6613 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/docs/user_manual.rst
--rw-r--r--   0 maurits    (501) staff       (20)     4340 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)       38 2024-01-22 20:04:46.261274 Products.PortalTransforms-4.0.2/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     2031 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/setup.py
--rw-r--r--   0 maurits    (501) staff       (20)     4632 2024-01-22 20:04:45.000000 Products.PortalTransforms-4.0.2/tox.ini
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:36:35.177333 products_portaltransforms-4.0.3/
+-rw-r--r--   0 maurits    (501) staff       (20)     1342 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/.editorconfig
+-rw-r--r--   0 maurits    (501) staff       (20)      540 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/.flake8
+-rw-r--r--   0 maurits    (501) staff       (20)      663 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/.gitignore
+-rw-r--r--   0 maurits    (501) staff       (20)      590 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/.meta.toml
+-rw-r--r--   0 maurits    (501) staff       (20)     1939 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/.pre-commit-config.yaml
+-rw-r--r--   0 maurits    (501) staff       (20)    22956 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      170 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    25606 2024-04-25 19:36:35.176838 products_portaltransforms-4.0.3/PKG-INFO
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:36:35.126979 products_portaltransforms-4.0.3/Products/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:36:35.135471 products_portaltransforms-4.0.3/Products/PortalTransforms/
+-rw-r--r--   0 maurits    (501) staff       (20)    11462 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/Transform.py
+-rw-r--r--   0 maurits    (501) staff       (20)    25608 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/TransformEngine.py
+-rw-r--r--   0 maurits    (501) staff       (20)       82 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/TransformTool.py
+-rw-r--r--   0 maurits    (501) staff       (20)      742 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1971 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/cache.py
+-rw-r--r--   0 maurits    (501) staff       (20)     7401 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/chain.py
+-rw-r--r--   0 maurits    (501) staff       (20)      649 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     1862 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/data.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3684 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/interfaces.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:36:35.137627 products_portaltransforms-4.0.3/Products/PortalTransforms/libtransforms/
+-rw-r--r--   0 maurits    (501) staff       (20)       88 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/libtransforms/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2711 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/libtransforms/commandtransform.py
+-rw-r--r--   0 maurits    (501) staff       (20)      987 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/libtransforms/piltransform.py
+-rw-r--r--   0 maurits    (501) staff       (20)      795 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/libtransforms/retransform.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3019 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/libtransforms/utils.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:36:35.119601 products_portaltransforms-4.0.3/Products/PortalTransforms/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:36:35.139618 products_portaltransforms-4.0.3/Products/PortalTransforms/profiles/default/
+-rw-r--r--   0 maurits    (501) staff       (20)      255 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/profiles/default/componentregistry.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      391 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/profiles/default/import_steps.xml
+-rw-r--r--   0 maurits    (501) staff       (20)       87 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/profiles/default/metadata.xml
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/profiles/default/portal-transforms-various.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      187 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/profiles/default/toolset.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     2484 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/setuphandlers.py
+-rw-r--r--   0 maurits    (501) staff       (20)      986 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/testing.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:36:35.144006 products_portaltransforms-4.0.3/Products/PortalTransforms/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      368 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/tests/base.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:36:35.151605 products_portaltransforms-4.0.3/Products/PortalTransforms/tests/input/
+-rw-r--r--   0 maurits    (501) staff       (20)   106910 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/tests/input/demo1.pdf
+-rw-r--r--   0 maurits    (501) staff       (20)      226 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/tests/input/input.textile
+-rw-r--r--   0 maurits    (501) staff       (20)     1710 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/tests/input/logo.bmp
+-rw-r--r--   0 maurits    (501) staff       (20)     1317 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/tests/input/logo.gif
+-rw-r--r--   0 maurits    (501) staff       (20)      801 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/tests/input/logo.jpg
+-rw-r--r--   0 maurits    (501) staff       (20)     1773 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/tests/input/logo.png
+-rw-r--r--   0 maurits    (501) staff       (20)      101 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/tests/input/markdown.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     7278 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/tests/input/org-news.xml
+-rw-r--r--   0 maurits    (501) staff       (20)       73 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/tests/input/rest1.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      152 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/tests/input/rest2.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      338 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/tests/input/rest3.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     1505 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/tests/input/rss2html.xslt
+-rw-r--r--   0 maurits    (501) staff       (20)     7680 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/tests/input/test.doc
+-rw-r--r--   0 maurits    (501) staff       (20)       25 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/tests/input/test_invalid_tags.html
+-rw-r--r--   0 maurits    (501) staff       (20)     9729 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/tests/input/test_js.doc
+-rw-r--r--   0 maurits    (501) staff       (20)       29 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/tests/input/test_js_on.html
+-rw-r--r--   0 maurits    (501) staff       (20)       37 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/tests/input/test_js_uri.html
+-rw-r--r--   0 maurits    (501) staff       (20)     3224 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/tests/input/test_lynx.html
+-rw-r--r--   0 maurits    (501) staff       (20)      147 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/tests/input/test_python.py
+-rw-r--r--   0 maurits    (501) staff       (20)      956 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/tests/input/test_safehtml.html
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:36:35.159160 products_portaltransforms-4.0.3/Products/PortalTransforms/tests/output/
+-rw-r--r--   0 maurits    (501) staff       (20)    22253 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/tests/output/demo1.html
+-rw-r--r--   0 maurits    (501) staff       (20)    22253 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/tests/output/demo1.html.nofilename
+-rw-r--r--   0 maurits    (501) staff       (20)     1710 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/tests/output/logo.bmp
+-rw-r--r--   0 maurits    (501) staff       (20)     1422 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/tests/output/logo.gif
+-rw-r--r--   0 maurits    (501) staff       (20)      805 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/tests/output/logo.jpg
+-rw-r--r--   0 maurits    (501) staff       (20)     3086 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/tests/output/logo.pcx
+-rw-r--r--   0 maurits    (501) staff       (20)     1773 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/tests/output/logo.png
+-rw-r--r--   0 maurits    (501) staff       (20)     1669 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/tests/output/logo.ppm
+-rw-r--r--   0 maurits    (501) staff       (20)     1796 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/tests/output/logo.tiff
+-rw-r--r--   0 maurits    (501) staff       (20)      161 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/tests/output/markdown.html
+-rw-r--r--   0 maurits    (501) staff       (20)     3025 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/tests/output/org-news.html
+-rw-r--r--   0 maurits    (501) staff       (20)       92 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/tests/output/rest1.html
+-rw-r--r--   0 maurits    (501) staff       (20)      112 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/tests/output/rest1.out
+-rw-r--r--   0 maurits    (501) staff       (20)       73 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/tests/output/rest1.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      244 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/tests/output/rest2.out
+-rw-r--r--   0 maurits    (501) staff       (20)      482 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/tests/output/rest3.out
+-rw-r--r--   0 maurits    (501) staff       (20)     1511 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/tests/output/test_html_to_text.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     2053 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/tests/output/test_lynx.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1308 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/tests/output/test_python.out
+-rw-r--r--   0 maurits    (501) staff       (20)      531 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/tests/output/test_safe.html
+-rw-r--r--   0 maurits    (501) staff       (20)      266 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/tests/output/test_word.html
+-rw-r--r--   0 maurits    (501) staff       (20)      367 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/tests/output/textile.html
+-rw-r--r--   0 maurits    (501) staff       (20)      275 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/tests/test_doctests.py
+-rw-r--r--   0 maurits    (501) staff       (20)    10342 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/tests/test_engine.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3916 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/tests/test_graph.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5807 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/tests/test_intelligenttext.py
+-rw-r--r--   0 maurits    (501) staff       (20)       37 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/tests/test_js_uri.html
+-rw-r--r--   0 maurits    (501) staff       (20)    24689 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/tests/test_transforms.py
+-rw-r--r--   0 maurits    (501) staff       (20)     9997 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/tests/test_xss.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1948 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/tests/utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)      339 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/tool.gif
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:36:35.169303 products_portaltransforms-4.0.3/Products/PortalTransforms/transforms/
+-rw-r--r--   0 maurits    (501) staff       (20)     2805 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/transforms/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      820 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/transforms/broken.py
+-rw-r--r--   0 maurits    (501) staff       (20)      998 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/transforms/html_body.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1102 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/transforms/html_to_text.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1263 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/transforms/html_to_web_intelligent_plain_text.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1087 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/transforms/identity.py
+-rw-r--r--   0 maurits    (501) staff       (20)      265 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/transforms/image_to_bmp.py
+-rw-r--r--   0 maurits    (501) staff       (20)      260 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/transforms/image_to_gif.py
+-rw-r--r--   0 maurits    (501) staff       (20)      440 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/transforms/image_to_html.py
+-rw-r--r--   0 maurits    (501) staff       (20)      265 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/transforms/image_to_jpeg.py
+-rw-r--r--   0 maurits    (501) staff       (20)      260 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/transforms/image_to_pcx.py
+-rw-r--r--   0 maurits    (501) staff       (20)      260 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/transforms/image_to_png.py
+-rw-r--r--   0 maurits    (501) staff       (20)      274 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/transforms/image_to_ppm.py
+-rw-r--r--   0 maurits    (501) staff       (20)      265 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/transforms/image_to_tiff.py
+-rw-r--r--   0 maurits    (501) staff       (20)      498 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/transforms/lynx_dump.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1537 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/transforms/markdown_to_html.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2584 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/transforms/office_com.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2029 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/transforms/office_uno.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1449 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/transforms/office_wvware.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2281 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/transforms/pdf_to_html.py
+-rw-r--r--   0 maurits    (501) staff       (20)      517 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/transforms/pdf_to_text.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4728 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/transforms/python.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4886 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/transforms/rest.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1764 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/transforms/rtf_to_html.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1653 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/transforms/rtf_to_xml.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6402 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/transforms/safe_html.py
+-rw-r--r--   0 maurits    (501) staff       (20)      596 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/transforms/st.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1008 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/transforms/text_pre_to_html.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1221 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/transforms/text_to_html.py
+-rw-r--r--   0 maurits    (501) staff       (20)      941 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/transforms/textile_to_html.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1289 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/transforms/web_intelligent_plain_text_to_html.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1510 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/transforms/word_to_html.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:36:35.170261 products_portaltransforms-4.0.3/Products/PortalTransforms/unsafe_transforms/
+-rw-r--r--   0 maurits    (501) staff       (20)     3015 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/unsafe_transforms/build_transforms.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3591 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/unsafe_transforms/command.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6213 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/unsafe_transforms/xml.py
+-rw-r--r--   0 maurits    (501) staff       (20)      557 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/utils.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:36:35.173232 products_portaltransforms-4.0.3/Products/PortalTransforms/www/
+-rw-r--r--   0 maurits    (501) staff       (20)     1191 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/www/addTransform.zpt
+-rw-r--r--   0 maurits    (501) staff       (20)     1183 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/www/addTransformsChain.zpt
+-rw-r--r--   0 maurits    (501) staff       (20)     2868 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/www/configureTransform.zpt
+-rw-r--r--   0 maurits    (501) staff       (20)     2273 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/www/editTransformationPolicy.zpt
+-rw-r--r--   0 maurits    (501) staff       (20)     2788 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/www/editTransformsChain.zpt
+-rw-r--r--   0 maurits    (501) staff       (20)      634 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/www/reloadAllTransforms.zpt
+-rw-r--r--   0 maurits    (501) staff       (20)      505 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/www/reloadTransform.zpt
+-rw-r--r--   0 maurits    (501) staff       (20)     1082 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/www/setCacheTime.zpt
+-rw-r--r--   0 maurits    (501) staff       (20)     2103 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/PortalTransforms/www/tr_widgets.zpt
+-rw-r--r--   0 maurits    (501) staff       (20)      245 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/Products/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:36:35.175944 products_portaltransforms-4.0.3/Products.PortalTransforms.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    25606 2024-04-25 19:36:35.000000 products_portaltransforms-4.0.3/Products.PortalTransforms.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     6662 2024-04-25 19:36:35.000000 products_portaltransforms-4.0.3/Products.PortalTransforms.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2024-04-25 19:36:35.000000 products_portaltransforms-4.0.3/Products.PortalTransforms.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        9 2024-04-25 19:36:35.000000 products_portaltransforms-4.0.3/Products.PortalTransforms.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2024-04-25 19:36:35.000000 products_portaltransforms-4.0.3/Products.PortalTransforms.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      305 2024-04-25 19:36:35.000000 products_portaltransforms-4.0.3/Products.PortalTransforms.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        9 2024-04-25 19:36:35.000000 products_portaltransforms-4.0.3/Products.PortalTransforms.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1049 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:36:35.175502 products_portaltransforms-4.0.3/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)     8682 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/docs/ChangeLog
+-rw-r--r--   0 maurits    (501) staff       (20)     1600 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/docs/LICENSE.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      273 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/docs/TODO
+-rw-r--r--   0 maurits    (501) staff       (20)     7166 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/docs/dev_manual.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      271 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/docs/makefile
+-rw-r--r--   0 maurits    (501) staff       (20)     3972 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/docs/uno_setup.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     6613 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/docs/user_manual.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     4340 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)       38 2024-04-25 19:36:35.177446 products_portaltransforms-4.0.3/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     2058 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/setup.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4632 2024-04-25 19:36:34.000000 products_portaltransforms-4.0.3/tox.ini
```

### Comparing `Products.PortalTransforms-4.0.2/.editorconfig` & `products_portaltransforms-4.0.3/.editorconfig`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/.flake8` & `products_portaltransforms-4.0.3/.flake8`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/.gitignore` & `products_portaltransforms-4.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/.meta.toml` & `products_portaltransforms-4.0.3/.meta.toml`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/.pre-commit-config.yaml` & `products_portaltransforms-4.0.3/.pre-commit-config.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 # See the inline comments on how to expand/tweak this configuration file
 ci:
     autofix_prs: false
     autoupdate_schedule: monthly
 
 repos:
 -   repo: https://github.com/asottile/pyupgrade
-    rev: v3.15.0
+    rev: v3.15.2
     hooks:
     -   id: pyupgrade
         args: [--py38-plus]
 -   repo: https://github.com/pycqa/isort
     rev: 5.13.2
     hooks:
     -   id: isort
 -   repo: https://github.com/psf/black
-    rev: 23.12.1
+    rev: 24.3.0
     hooks:
     -   id: black
 -   repo: https://github.com/collective/zpretty
     rev: 3.1.0
     hooks:
     -   id: zpretty
         exclude: tests/.*.html
@@ -29,15 +29,15 @@
 # Add extra configuration options in .meta.toml:
 #  [pre_commit]
 #  zpretty_extra_lines = """
 #  _your own configuration lines_
 #  """
 ##
 -   repo: https://github.com/PyCQA/flake8
-    rev: 6.1.0
+    rev: 7.0.0
     hooks:
     -   id: flake8
 
 ##
 # Add extra configuration options in .meta.toml:
 #  [pre_commit]
 #  flake8_extra_lines = """
```

### Comparing `Products.PortalTransforms-4.0.2/CHANGES.rst` & `products_portaltransforms-4.0.3/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,26 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.0.3 (2024-04-25)
+------------------
+
+Bug fixes:
+
+
+- Use ``Cleaner`` from new package ``lxml_html_clean``.
+  This was factored out from ``lxml`` in version 5.2.0.
+  See https://lxml-html-clean.readthedocs.io/
+  [maurits] (#3938)
+
+
 4.0.2 (2024-01-22)
 ------------------
 
 Internal:
 
 
 - Update configuration files.
```

### Comparing `Products.PortalTransforms-4.0.2/PKG-INFO` & `products_portaltransforms-4.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Products.PortalTransforms
-Version: 4.0.2
+Version: 4.0.3
 Summary: MIME based content transformations
 Home-page: https://pypi.org/project/Products.PortalTransforms
 Author: Benjamin Saller
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL
 Keywords: Zope Plone Transform
 Classifier: Development Status :: 5 - Production/Stable
@@ -24,14 +24,15 @@
 Description-Content-Type: text/x-rst
 Requires-Dist: docutils
 Requires-Dist: DocumentTemplate
 Requires-Dist: Persistence
 Requires-Dist: Products.GenericSetup
 Requires-Dist: setuptools
 Requires-Dist: lxml
+Requires-Dist: lxml_html_clean
 Requires-Dist: persistent
 Requires-Dist: plone.base
 Requires-Dist: plone.registry
 Requires-Dist: plone.intelligenttext
 Requires-Dist: zope.structuredtext
 Requires-Dist: Pillow>=3.1.0
 Requires-Dist: Products.CMFCore
@@ -86,14 +87,26 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.0.3 (2024-04-25)
+------------------
+
+Bug fixes:
+
+
+- Use ``Cleaner`` from new package ``lxml_html_clean``.
+  This was factored out from ``lxml`` in version 5.2.0.
+  See https://lxml-html-clean.readthedocs.io/
+  [maurits] (#3938)
+
+
 4.0.2 (2024-01-22)
 ------------------
 
 Internal:
 
 
 - Update configuration files.
```

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/Transform.py` & `products_portaltransforms-4.0.3/Products/PortalTransforms/Transform.py`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/TransformEngine.py` & `products_portaltransforms-4.0.3/Products/PortalTransforms/TransformEngine.py`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/__init__.py` & `products_portaltransforms-4.0.3/Products/PortalTransforms/__init__.py`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/cache.py` & `products_portaltransforms-4.0.3/Products/PortalTransforms/cache.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Cache
 """
+
 from Acquisition import aq_base
 from time import time
 
 
 _marker = object()
```

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/chain.py` & `products_portaltransforms-4.0.3/Products/PortalTransforms/chain.py`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/configure.zcml` & `products_portaltransforms-4.0.3/Products/PortalTransforms/configure.zcml`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/data.py` & `products_portaltransforms-4.0.3/Products/PortalTransforms/data.py`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/interfaces.py` & `products_portaltransforms-4.0.3/Products/PortalTransforms/interfaces.py`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/libtransforms/commandtransform.py` & `products_portaltransforms-4.0.3/Products/PortalTransforms/libtransforms/commandtransform.py`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/libtransforms/piltransform.py` & `products_portaltransforms-4.0.3/Products/PortalTransforms/libtransforms/piltransform.py`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/libtransforms/retransform.py` & `products_portaltransforms-4.0.3/Products/PortalTransforms/libtransforms/retransform.py`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/libtransforms/utils.py` & `products_portaltransforms-4.0.3/Products/PortalTransforms/libtransforms/utils.py`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/setuphandlers.py` & `products_portaltransforms-4.0.3/Products/PortalTransforms/setuphandlers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 PortalTransforms setup handlers.
 """
+
 from io import StringIO as NativeStringIO
 from Products.CMFCore.utils import getToolByName
 
 
 def correctMapping(out, portal):
     pt = getToolByName(portal, "portal_transforms")
     pt_ids = pt.objectIds()
```

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/testing.py` & `products_portaltransforms-4.0.3/Products/PortalTransforms/testing.py`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/input/demo1.pdf` & `products_portaltransforms-4.0.3/Products/PortalTransforms/tests/input/demo1.pdf`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/input/logo.bmp` & `products_portaltransforms-4.0.3/Products/PortalTransforms/tests/input/logo.bmp`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/input/logo.gif` & `products_portaltransforms-4.0.3/Products/PortalTransforms/tests/input/logo.gif`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/input/logo.jpg` & `products_portaltransforms-4.0.3/Products/PortalTransforms/tests/input/logo.jpg`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/input/logo.png` & `products_portaltransforms-4.0.3/Products/PortalTransforms/tests/input/logo.png`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/input/org-news.xml` & `products_portaltransforms-4.0.3/Products/PortalTransforms/tests/input/org-news.xml`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/input/rss2html.xslt` & `products_portaltransforms-4.0.3/Products/PortalTransforms/tests/input/rss2html.xslt`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/input/test.doc` & `products_portaltransforms-4.0.3/Products/PortalTransforms/tests/input/test.doc`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/input/test_js.doc` & `products_portaltransforms-4.0.3/Products/PortalTransforms/tests/input/test_js.doc`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/input/test_lynx.html` & `products_portaltransforms-4.0.3/Products/PortalTransforms/tests/input/test_lynx.html`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/input/test_safehtml.html` & `products_portaltransforms-4.0.3/Products/PortalTransforms/tests/input/test_safehtml.html`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/output/demo1.html` & `products_portaltransforms-4.0.3/Products/PortalTransforms/tests/output/demo1.html`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/output/demo1.html.nofilename` & `products_portaltransforms-4.0.3/Products/PortalTransforms/tests/output/demo1.html.nofilename`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/output/logo.bmp` & `products_portaltransforms-4.0.3/Products/PortalTransforms/tests/output/logo.bmp`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/output/logo.gif` & `products_portaltransforms-4.0.3/Products/PortalTransforms/tests/output/logo.gif`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/output/logo.jpg` & `products_portaltransforms-4.0.3/Products/PortalTransforms/tests/output/logo.jpg`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/output/logo.pcx` & `products_portaltransforms-4.0.3/Products/PortalTransforms/tests/output/logo.pcx`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/output/logo.png` & `products_portaltransforms-4.0.3/Products/PortalTransforms/tests/output/logo.png`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/output/logo.tiff` & `products_portaltransforms-4.0.3/Products/PortalTransforms/tests/output/logo.tiff`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/output/org-news.html` & `products_portaltransforms-4.0.3/Products/PortalTransforms/tests/output/org-news.html`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/output/test_html_to_text.txt` & `products_portaltransforms-4.0.3/Products/PortalTransforms/tests/output/test_html_to_text.txt`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/output/test_lynx.txt` & `products_portaltransforms-4.0.3/Products/PortalTransforms/tests/output/test_lynx.txt`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/output/test_python.out` & `products_portaltransforms-4.0.3/Products/PortalTransforms/tests/output/test_python.out`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/output/test_safe.html` & `products_portaltransforms-4.0.3/Products/PortalTransforms/tests/output/test_safe.html`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/test_engine.py` & `products_portaltransforms-4.0.3/Products/PortalTransforms/tests/test_engine.py`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/test_graph.py` & `products_portaltransforms-4.0.3/Products/PortalTransforms/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/test_intelligenttext.py` & `products_portaltransforms-4.0.3/Products/PortalTransforms/tests/test_intelligenttext.py`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/test_transforms.py` & `products_portaltransforms-4.0.3/Products/PortalTransforms/tests/test_transforms.py`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/test_xss.py` & `products_portaltransforms-4.0.3/Products/PortalTransforms/tests/test_xss.py`

 * *Files 2% similar despite different names*

```diff
@@ -247,13 +247,18 @@
         self.doTest(data_in, data_out)
 
     def test_38(self):
         data_in = (
             """<p><a href="http://T\\foo\\20111015\\bar.msg">FOO</a></p>"""  # noqa
         )
         data_out = """<p><a href="http://T%5Cfoo%5C20111015%5Cbar.msg">FOO</a></p>"""
-        self.doTest(data_in, data_out)
+        # When we were still using lxml.xml, converting data_in gave data_in as anwer.
+        # Then we switched to lxml.html, which caused the backslashes to be converted
+        # into '%5C'.  And now when we upgrade from lxml 4 to 5, data_in is again
+        # unchanged after converting.  So let's accept both.
+        result = self.doConvert(data_in)
+        self.assertIn(result, (data_in, data_out))
 
     def test_39(self):
         data_in = """<a href="&#42;&Ascr;\xa9"></a>"""
         data_out = '<a href="*&amp;Ascr;%C2%A9"></a>'
         self.doTest(data_in, data_out)
```

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/tests/utils.py` & `products_portaltransforms-4.0.3/Products/PortalTransforms/tests/utils.py`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/transforms/__init__.py` & `products_portaltransforms-4.0.3/Products/PortalTransforms/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/transforms/broken.py` & `products_portaltransforms-4.0.3/Products/PortalTransforms/transforms/broken.py`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/transforms/html_body.py` & `products_portaltransforms-4.0.3/Products/PortalTransforms/transforms/html_body.py`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/transforms/html_to_text.py` & `products_portaltransforms-4.0.3/Products/PortalTransforms/transforms/html_to_text.py`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/transforms/html_to_web_intelligent_plain_text.py` & `products_portaltransforms-4.0.3/Products/PortalTransforms/transforms/html_to_web_intelligent_plain_text.py`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/transforms/identity.py` & `products_portaltransforms-4.0.3/Products/PortalTransforms/transforms/identity.py`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/transforms/markdown_to_html.py` & `products_portaltransforms-4.0.3/Products/PortalTransforms/transforms/markdown_to_html.py`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/transforms/office_com.py` & `products_portaltransforms-4.0.3/Products/PortalTransforms/transforms/office_com.py`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/transforms/office_uno.py` & `products_portaltransforms-4.0.3/Products/PortalTransforms/transforms/office_uno.py`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/transforms/office_wvware.py` & `products_portaltransforms-4.0.3/Products/PortalTransforms/transforms/office_wvware.py`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/transforms/pdf_to_html.py` & `products_portaltransforms-4.0.3/Products/PortalTransforms/transforms/pdf_to_html.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Uses the http://sf.net/projects/pdftohtml bin to do its handy work
 
 """
+
 from Products.PortalTransforms.interfaces import ITransform
 from Products.PortalTransforms.libtransforms.commandtransform import commandtransform
 from Products.PortalTransforms.libtransforms.utils import bodyfinder
 from Products.PortalTransforms.libtransforms.utils import sansext
 from zope.interface import implementer
 
 import os
```

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/transforms/pdf_to_text.py` & `products_portaltransforms-4.0.3/Products/PortalTransforms/transforms/pdf_to_text.py`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/transforms/python.py` & `products_portaltransforms-4.0.3/Products/PortalTransforms/transforms/python.py`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/transforms/rest.py` & `products_portaltransforms-4.0.3/Products/PortalTransforms/transforms/rest.py`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/transforms/rtf_to_html.py` & `products_portaltransforms-4.0.3/Products/PortalTransforms/transforms/rtf_to_html.py`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/transforms/rtf_to_xml.py` & `products_portaltransforms-4.0.3/Products/PortalTransforms/transforms/rtf_to_xml.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Uses the http://sf.net/projects/rtf2xml bin to do its handy work
 
 """
+
 from Products.PortalTransforms.interfaces import ITransform
 from Products.PortalTransforms.libtransforms.commandtransform import commandtransform
 from Products.PortalTransforms.libtransforms.utils import sansext
 from zope.interface import implementer
 
 import subprocess
```

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/transforms/safe_html.py` & `products_portaltransforms-4.0.3/Products/PortalTransforms/transforms/safe_html.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from html.entities import html5 as html5entities
 from lxml import etree
 from lxml import html
-from lxml.html.clean import Cleaner
+from lxml_html_clean import Cleaner
 from plone.base.interfaces import IFilterSchema
 from plone.base.utils import safe_bytes
 from plone.registry.interfaces import IRegistry
 from Products.PortalTransforms.interfaces import ITransform
 from Products.PortalTransforms.libtransforms.utils import bodyfinder
 from zope.component import getUtility
 from zope.interface import implementer
```

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/transforms/st.py` & `products_portaltransforms-4.0.3/Products/PortalTransforms/transforms/st.py`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/transforms/text_pre_to_html.py` & `products_portaltransforms-4.0.3/Products/PortalTransforms/transforms/text_pre_to_html.py`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/transforms/text_to_html.py` & `products_portaltransforms-4.0.3/Products/PortalTransforms/transforms/text_to_html.py`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/transforms/textile_to_html.py` & `products_portaltransforms-4.0.3/Products/PortalTransforms/transforms/textile_to_html.py`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/transforms/web_intelligent_plain_text_to_html.py` & `products_portaltransforms-4.0.3/Products/PortalTransforms/transforms/web_intelligent_plain_text_to_html.py`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/transforms/word_to_html.py` & `products_portaltransforms-4.0.3/Products/PortalTransforms/transforms/word_to_html.py`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/unsafe_transforms/build_transforms.py` & `products_portaltransforms-4.0.3/Products/PortalTransforms/unsafe_transforms/build_transforms.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """try to build some useful transformations with the command and xml
 transforms and the available binaries
 """
+
 from command import ExternalCommandTransform
 from Products.PortalTransforms.libtransforms.utils import bin_search
 from Products.PortalTransforms.libtransforms.utils import MissingBinary
 
 
 COMMAND_CONFIGS = (
     (
```

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/unsafe_transforms/command.py` & `products_portaltransforms-4.0.3/Products/PortalTransforms/unsafe_transforms/command.py`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/unsafe_transforms/xml.py` & `products_portaltransforms-4.0.3/Products/PortalTransforms/unsafe_transforms/xml.py`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/utils.py` & `products_portaltransforms-4.0.3/Products/PortalTransforms/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """some common utilities
 """
+
 # directory where template for the ZMI are located
 import logging
 import os.path
 
 
 class TransformException(Exception):
     pass
```

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/www/addTransform.zpt` & `products_portaltransforms-4.0.3/Products/PortalTransforms/www/addTransform.zpt`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/www/addTransformsChain.zpt` & `products_portaltransforms-4.0.3/Products/PortalTransforms/www/addTransformsChain.zpt`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/www/configureTransform.zpt` & `products_portaltransforms-4.0.3/Products/PortalTransforms/www/configureTransform.zpt`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/www/editTransformationPolicy.zpt` & `products_portaltransforms-4.0.3/Products/PortalTransforms/www/editTransformationPolicy.zpt`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/www/editTransformsChain.zpt` & `products_portaltransforms-4.0.3/Products/PortalTransforms/www/editTransformsChain.zpt`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/www/reloadAllTransforms.zpt` & `products_portaltransforms-4.0.3/Products/PortalTransforms/www/reloadAllTransforms.zpt`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/www/setCacheTime.zpt` & `products_portaltransforms-4.0.3/Products/PortalTransforms/www/setCacheTime.zpt`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/Products/PortalTransforms/www/tr_widgets.zpt` & `products_portaltransforms-4.0.3/Products/PortalTransforms/www/tr_widgets.zpt`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/Products.PortalTransforms.egg-info/PKG-INFO` & `products_portaltransforms-4.0.3/Products.PortalTransforms.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Products.PortalTransforms
-Version: 4.0.2
+Version: 4.0.3
 Summary: MIME based content transformations
 Home-page: https://pypi.org/project/Products.PortalTransforms
 Author: Benjamin Saller
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL
 Keywords: Zope Plone Transform
 Classifier: Development Status :: 5 - Production/Stable
@@ -24,14 +24,15 @@
 Description-Content-Type: text/x-rst
 Requires-Dist: docutils
 Requires-Dist: DocumentTemplate
 Requires-Dist: Persistence
 Requires-Dist: Products.GenericSetup
 Requires-Dist: setuptools
 Requires-Dist: lxml
+Requires-Dist: lxml_html_clean
 Requires-Dist: persistent
 Requires-Dist: plone.base
 Requires-Dist: plone.registry
 Requires-Dist: plone.intelligenttext
 Requires-Dist: zope.structuredtext
 Requires-Dist: Pillow>=3.1.0
 Requires-Dist: Products.CMFCore
@@ -86,14 +87,26 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.0.3 (2024-04-25)
+------------------
+
+Bug fixes:
+
+
+- Use ``Cleaner`` from new package ``lxml_html_clean``.
+  This was factored out from ``lxml`` in version 5.2.0.
+  See https://lxml-html-clean.readthedocs.io/
+  [maurits] (#3938)
+
+
 4.0.2 (2024-01-22)
 ------------------
 
 Internal:
 
 
 - Update configuration files.
```

### Comparing `Products.PortalTransforms-4.0.2/Products.PortalTransforms.egg-info/SOURCES.txt` & `products_portaltransforms-4.0.3/Products.PortalTransforms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/README.rst` & `products_portaltransforms-4.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/docs/ChangeLog` & `products_portaltransforms-4.0.3/docs/ChangeLog`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/docs/LICENSE.txt` & `products_portaltransforms-4.0.3/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/docs/dev_manual.rst` & `products_portaltransforms-4.0.3/docs/dev_manual.rst`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/docs/uno_setup.rst` & `products_portaltransforms-4.0.3/docs/uno_setup.rst`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/docs/user_manual.rst` & `products_portaltransforms-4.0.3/docs/user_manual.rst`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/pyproject.toml` & `products_portaltransforms-4.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Products.PortalTransforms-4.0.2/setup.py` & `products_portaltransforms-4.0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pathlib import Path
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "4.0.2"
+version = "4.0.3"
 
 long_description = (
     f"{Path('README.rst').read_text()}\n{Path('CHANGES.rst').read_text()}"
 )
 
 setup(
     name="Products.PortalTransforms",
@@ -51,14 +51,15 @@
     install_requires=[
         "docutils",
         "DocumentTemplate",
         "Persistence",
         "Products.GenericSetup",
         "setuptools",
         "lxml",
+        "lxml_html_clean",
         "persistent",
         "plone.base",
         "plone.registry",
         "plone.intelligenttext",
         "zope.structuredtext",
         "Pillow>=3.1.0",
         "Products.CMFCore",
```

### Comparing `Products.PortalTransforms-4.0.2/tox.ini` & `products_portaltransforms-4.0.3/tox.ini`

 * *Files identical despite different names*

