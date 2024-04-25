# Comparing `tmp/ipydatagrid-1.3.0.tar.gz` & `tmp/ipydatagrid-1.3.1.tar.gz`

## Comparing `ipydatagrid-1.3.0.tar` & `ipydatagrid-1.3.1.tar`

### file list

```diff
@@ -1,97 +1,97 @@
--rw-r--r--   0        0        0     7548 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/RELEASE.md
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/babel.config.js
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid.json
--rw-r--r--   0        0        0     5321 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/package.json
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/tsconfig.json
--rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/webpack.config.js
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/webpack.lab.config.js
--rw-r--r--   0        0        0   403706 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/yarn.lock
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/__init__.py
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/_frontend.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/_version.py
--rw-r--r--   0        0        0     7812 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/cellrenderer.py
--rw-r--r--   0        0        0    34516 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/datagrid.py
--rw-r--r--   0        0        0     5437 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/package.json
--rw-r--r--   0        0        0    17303 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/109.bdd9793b392cc2fe87da.js
--rw-r--r--   0        0        0     4982 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/142.025e64e0cbb8aa528385.js
--rw-r--r--   0        0        0    26563 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/143.171db67c9b56d395ae64.js
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/14ad542071f6e259fbe2.png
--rw-r--r--   0        0        0     9449 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/271.c6d995708c863e1b27ed.js
--rw-r--r--   0        0        0     7708 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/296.d2eeaa2e543e597ac586.js
--rw-r--r--   0        0        0    32396 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/351.372e5eec3c9010a57cf3.js
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/3546b939aba74f121f34.png
--rw-r--r--   0        0        0     2801 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/400.95b73fc6eb3f120b823f.js
--rw-r--r--   0        0        0    17303 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/41.1846c3ba970651a706b6.js
--rw-r--r--   0        0        0    17304 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/433.75ed253aaa8060b28c81.js
--rw-r--r--   0        0        0    17304 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/455.25b625d30041b5a1671c.js
--rw-r--r--   0        0        0     4293 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/456.afd75d5e116998d22e56.js
--rw-r--r--   0        0        0     4982 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/462.68e4d74f02bf2411528e.js
--rw-r--r--   0        0        0    12212 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/48.732e43cec274cf5b8cf5.js
--rw-r--r--   0        0        0     5161 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/481.911a23288443c8041987.js
--rw-r--r--   0        0        0    17304 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/513.73d1ca46ed758871d49a.js
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/568.2b5bb2c0c4fdfa06786c.js
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/5b5469a81198fb5e6aa1.png
--rw-r--r--   0        0        0    11919 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/642.730227a42292c5f89120.js
--rw-r--r--   0        0        0    17304 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/643.a265dd26cb50ebd06923.js
--rw-r--r--   0        0        0   136897 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/679.e174128fe156c1cd0d10.js
--rw-r--r--   0        0        0    12508 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/683.efe59705c1680a8f8b3a.js
--rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/700.7f792a9e7380bfde28dc.js
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/733684aa1ae47c885305.png
--rw-r--r--   0        0        0   292706 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/762.42901b906691b1301214.js
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/762.42901b906691b1301214.js.LICENSE.txt
--rw-r--r--   0        0        0    20610 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/781.ef3f9c2a235c4a40bdc0.js
--rw-r--r--   0        0        0   105436 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/787.f307b1ca46997f4a9051.js
--rw-r--r--   0        0        0    22076 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/794.d7c23e15137c8752365e.js
--rw-r--r--   0        0        0    10377 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/811.a135ebc21be585e6d76d.js
--rw-r--r--   0        0        0     5901 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/823.18e09aad57c7797df987.js
--rw-r--r--   0        0        0    26563 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/917.b972bc5b41fae8990bff.js
--rw-r--r--   0        0        0    35000 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/939.04c5876588e4898127e3.js
--rw-r--r--   0        0        0    11847 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/941.23c8b1f0eb18afd531e9.js
--rw-r--r--   0        0        0     5901 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/990.e35c256305f259cdaeb9.js
--rw-r--r--   0        0        0    13315 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/remoteEntry.e416f171876299bb6885.js
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/style.js
--rw-r--r--   0        0        0    40475 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/nbextension/extension.js
--rw-r--r--   0        0        0  2612931 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/nbextension/index.js
--rw-r--r--   0        0        0     2167 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/nbextension/index.js.LICENSE.txt
--rw-r--r--   0        0        0    16722 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/js/cellrenderer.ts
--rw-r--r--   0        0        0    24043 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/js/datagrid.ts
--rw-r--r--   0        0        0     3560 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/js/datasource.ts
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/js/extension.ts
--rw-r--r--   0        0        0    31969 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/js/feathergrid.ts
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/js/index.ts
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/js/keyhandler.ts
--rw-r--r--   0        0        0     4832 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/js/mousehandler.ts
--rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/js/plugin.ts
--rw-r--r--   0        0        0     9492 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/js/utils.ts
--rw-r--r--   0        0        0     4151 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/js/vegaexpr.ts
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/js/version.ts
--rw-r--r--   0        0        0     6282 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/js/core/barrenderer.ts
--rw-r--r--   0        0        0    45377 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/js/core/filterMenu.ts
--rw-r--r--   0        0        0     7329 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/js/core/gridContextMenu.ts
--rw-r--r--   0        0        0    15136 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/js/core/headerRenderer.ts
--rw-r--r--   0        0        0     8567 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/js/core/htmlRenderer.ts
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/js/core/transform.ts
--rw-r--r--   0        0        0    11413 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/js/core/transformExecutors.ts
--rw-r--r--   0        0        0     6994 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/js/core/transformStateManager.ts
--rw-r--r--   0        0        0     4899 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/js/core/valueRenderer.ts
--rw-r--r--   0        0        0     7540 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/js/core/view.ts
--rw-r--r--   0        0        0    19073 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/js/core/viewbasedjsonmodel.ts
--rw-r--r--   0        0        0  1526055 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/static/ipydatagrid_1.gif
--rw-r--r--   0        0        0  1526560 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/static/ipydatagrid_2.gif
--rw-r--r--   0        0        0  2696451 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/static/ipydatagrid_3.gif
--rw-r--r--   0        0        0   203865 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/static/ipydatagrid_4.gif
--rw-r--r--   0        0        0    52546 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/static/ipydatagrid_5.gif
--rw-r--r--   0        0        0     4544 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/style/feathergrid.css
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/style/jupyter-widget.css
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/style/icons/arrow-down-short-dark.svg
--rwxr-xr-x   0        0        0      416 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/style/icons/arrow-down-short.svg
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/style/icons/arrow-up-short-dark.svg
--rwxr-xr-x   0        0        0      400 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/style/icons/arrow-up-short.svg
--rwxr-xr-x   0        0        0      349 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/style/icons/filter-dark.svg
--rwxr-xr-x   0        0        0      349 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/style/icons/filter.svg
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/.gitignore
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/LICENSE.txt
--rw-r--r--   0        0        0     4897 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/README.md
--rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     6036 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     7548 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/RELEASE.md
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/babel.config.js
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid.json
+-rw-r--r--   0        0        0     5321 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/package.json
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/tsconfig.json
+-rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/webpack.config.js
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/webpack.lab.config.js
+-rw-r--r--   0        0        0   403706 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/yarn.lock
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/__init__.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/_frontend.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/_version.py
+-rw-r--r--   0        0        0     7812 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/cellrenderer.py
+-rw-r--r--   0        0        0    34516 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/datagrid.py
+-rw-r--r--   0        0        0     5437 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/package.json
+-rw-r--r--   0        0        0    17303 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/109.bdd9793b392cc2fe87da.js
+-rw-r--r--   0        0        0     4982 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/142.025e64e0cbb8aa528385.js
+-rw-r--r--   0        0        0    26563 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/143.171db67c9b56d395ae64.js
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/14ad542071f6e259fbe2.png
+-rw-r--r--   0        0        0     9449 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/271.c6d995708c863e1b27ed.js
+-rw-r--r--   0        0        0     7708 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/296.d2eeaa2e543e597ac586.js
+-rw-r--r--   0        0        0    32396 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/351.372e5eec3c9010a57cf3.js
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/3546b939aba74f121f34.png
+-rw-r--r--   0        0        0     2801 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/400.95b73fc6eb3f120b823f.js
+-rw-r--r--   0        0        0    17303 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/41.1846c3ba970651a706b6.js
+-rw-r--r--   0        0        0    17304 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/433.75ed253aaa8060b28c81.js
+-rw-r--r--   0        0        0    17304 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/455.25b625d30041b5a1671c.js
+-rw-r--r--   0        0        0     4293 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/456.afd75d5e116998d22e56.js
+-rw-r--r--   0        0        0     4982 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/462.68e4d74f02bf2411528e.js
+-rw-r--r--   0        0        0    12212 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/48.732e43cec274cf5b8cf5.js
+-rw-r--r--   0        0        0     5161 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/481.911a23288443c8041987.js
+-rw-r--r--   0        0        0    17304 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/513.73d1ca46ed758871d49a.js
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/568.2b5bb2c0c4fdfa06786c.js
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/5b5469a81198fb5e6aa1.png
+-rw-r--r--   0        0        0    11919 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/642.730227a42292c5f89120.js
+-rw-r--r--   0        0        0    17304 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/643.a265dd26cb50ebd06923.js
+-rw-r--r--   0        0        0   136897 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/679.e174128fe156c1cd0d10.js
+-rw-r--r--   0        0        0    12508 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/683.efe59705c1680a8f8b3a.js
+-rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/700.7f792a9e7380bfde28dc.js
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/733684aa1ae47c885305.png
+-rw-r--r--   0        0        0   292706 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/762.42901b906691b1301214.js
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/762.42901b906691b1301214.js.LICENSE.txt
+-rw-r--r--   0        0        0    20610 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/781.ef3f9c2a235c4a40bdc0.js
+-rw-r--r--   0        0        0   105961 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/787.47c1e167bb24294e1e7e.js
+-rw-r--r--   0        0        0    22076 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/794.d7c23e15137c8752365e.js
+-rw-r--r--   0        0        0    10377 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/811.a135ebc21be585e6d76d.js
+-rw-r--r--   0        0        0     5901 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/823.18e09aad57c7797df987.js
+-rw-r--r--   0        0        0    26563 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/917.b972bc5b41fae8990bff.js
+-rw-r--r--   0        0        0    35000 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/939.04c5876588e4898127e3.js
+-rw-r--r--   0        0        0    11847 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/941.23c8b1f0eb18afd531e9.js
+-rw-r--r--   0        0        0     5901 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/990.e35c256305f259cdaeb9.js
+-rw-r--r--   0        0        0    13315 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/remoteEntry.6d509d1468636d15eab8.js
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/style.js
+-rw-r--r--   0        0        0    40475 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/nbextension/extension.js
+-rw-r--r--   0        0        0  2613456 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/nbextension/index.js
+-rw-r--r--   0        0        0     2167 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/nbextension/index.js.LICENSE.txt
+-rw-r--r--   0        0        0    16722 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/js/cellrenderer.ts
+-rw-r--r--   0        0        0    25051 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/js/datagrid.ts
+-rw-r--r--   0        0        0     3560 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/js/datasource.ts
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/js/extension.ts
+-rw-r--r--   0        0        0    31969 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/js/feathergrid.ts
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/js/index.ts
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/js/keyhandler.ts
+-rw-r--r--   0        0        0     4832 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/js/mousehandler.ts
+-rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/js/plugin.ts
+-rw-r--r--   0        0        0     9492 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/js/utils.ts
+-rw-r--r--   0        0        0     4151 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/js/vegaexpr.ts
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/js/version.ts
+-rw-r--r--   0        0        0     6282 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/js/core/barrenderer.ts
+-rw-r--r--   0        0        0    45377 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/js/core/filterMenu.ts
+-rw-r--r--   0        0        0     7846 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/js/core/gridContextMenu.ts
+-rw-r--r--   0        0        0    15136 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/js/core/headerRenderer.ts
+-rw-r--r--   0        0        0     8567 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/js/core/htmlRenderer.ts
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/js/core/transform.ts
+-rw-r--r--   0        0        0    11413 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/js/core/transformExecutors.ts
+-rw-r--r--   0        0        0     6994 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/js/core/transformStateManager.ts
+-rw-r--r--   0        0        0     4899 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/js/core/valueRenderer.ts
+-rw-r--r--   0        0        0     7540 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/js/core/view.ts
+-rw-r--r--   0        0        0    19073 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/js/core/viewbasedjsonmodel.ts
+-rw-r--r--   0        0        0  1526055 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/static/ipydatagrid_1.gif
+-rw-r--r--   0        0        0  1526560 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/static/ipydatagrid_2.gif
+-rw-r--r--   0        0        0  2696451 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/static/ipydatagrid_3.gif
+-rw-r--r--   0        0        0   203865 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/static/ipydatagrid_4.gif
+-rw-r--r--   0        0        0    52546 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/static/ipydatagrid_5.gif
+-rw-r--r--   0        0        0     4544 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/style/feathergrid.css
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/style/jupyter-widget.css
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/style/icons/arrow-down-short-dark.svg
+-rwxr-xr-x   0        0        0      416 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/style/icons/arrow-down-short.svg
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/style/icons/arrow-up-short-dark.svg
+-rwxr-xr-x   0        0        0      400 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/style/icons/arrow-up-short.svg
+-rwxr-xr-x   0        0        0      349 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/style/icons/filter-dark.svg
+-rwxr-xr-x   0        0        0      349 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/style/icons/filter.svg
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/.gitignore
+-rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/LICENSE.txt
+-rw-r--r--   0        0        0     4897 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/README.md
+-rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     6036 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/PKG-INFO
```

### Comparing `ipydatagrid-1.3.0/RELEASE.md` & `ipydatagrid-1.3.1/RELEASE.md`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.0/package.json` & `ipydatagrid-1.3.1/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9705882352941176%*

 * *Differences: {"'version'": "'1.3.1'"}*

```diff
@@ -166,9 +166,9 @@
         "test": "jest --verbose",
         "watch": "npm-run-all -p watch:lib watch:labextension watch:nbextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:lib": "tsc -w",
         "watch:nbextension": "webpack --watch"
     },
     "types": "./lib/index.d.ts",
-    "version": "1.3.0"
+    "version": "1.3.1"
 }
```

### Comparing `ipydatagrid-1.3.0/tsconfig.json` & `ipydatagrid-1.3.1/tsconfig.json`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.0/webpack.config.js` & `ipydatagrid-1.3.1/webpack.config.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.0/yarn.lock` & `ipydatagrid-1.3.1/yarn.lock`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.0/ipydatagrid/__init__.py` & `ipydatagrid-1.3.1/ipydatagrid/__init__.py`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.0/ipydatagrid/cellrenderer.py` & `ipydatagrid-1.3.1/ipydatagrid/cellrenderer.py`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.0/ipydatagrid/datagrid.py` & `ipydatagrid-1.3.1/ipydatagrid/datagrid.py`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.0/ipydatagrid/labextension/package.json` & `ipydatagrid-1.3.1/ipydatagrid/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9698529411764706%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.6d509d1468636d15eab8.js'}}",*

 * * "'version'": "'1.3.1'"}*

```diff
@@ -82,15 +82,15 @@
         "dist/*.png",
         "style/**/*.*"
     ],
     "homepage": "https://github.com/Bloomberg/ipydatagrid",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.e416f171876299bb6885.js"
+            "load": "static/remoteEntry.6d509d1468636d15eab8.js"
         },
         "extension": "lib/plugin",
         "outputDir": "./ipydatagrid/labextension",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
                 "singleton": true
@@ -170,9 +170,9 @@
         "test": "jest --verbose",
         "watch": "npm-run-all -p watch:lib watch:labextension watch:nbextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:lib": "tsc -w",
         "watch:nbextension": "webpack --watch"
     },
     "types": "./lib/index.d.ts",
-    "version": "1.3.0"
+    "version": "1.3.1"
 }
```

### Comparing `ipydatagrid-1.3.0/ipydatagrid/labextension/static/109.bdd9793b392cc2fe87da.js` & `ipydatagrid-1.3.1/ipydatagrid/labextension/static/109.bdd9793b392cc2fe87da.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.0/ipydatagrid/labextension/static/142.025e64e0cbb8aa528385.js` & `ipydatagrid-1.3.1/ipydatagrid/labextension/static/142.025e64e0cbb8aa528385.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.0/ipydatagrid/labextension/static/143.171db67c9b56d395ae64.js` & `ipydatagrid-1.3.1/ipydatagrid/labextension/static/143.171db67c9b56d395ae64.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.0/ipydatagrid/labextension/static/271.c6d995708c863e1b27ed.js` & `ipydatagrid-1.3.1/ipydatagrid/labextension/static/271.c6d995708c863e1b27ed.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.0/ipydatagrid/labextension/static/296.d2eeaa2e543e597ac586.js` & `ipydatagrid-1.3.1/ipydatagrid/labextension/static/296.d2eeaa2e543e597ac586.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.0/ipydatagrid/labextension/static/351.372e5eec3c9010a57cf3.js` & `ipydatagrid-1.3.1/ipydatagrid/labextension/static/351.372e5eec3c9010a57cf3.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.0/ipydatagrid/labextension/static/400.95b73fc6eb3f120b823f.js` & `ipydatagrid-1.3.1/ipydatagrid/labextension/static/400.95b73fc6eb3f120b823f.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.0/ipydatagrid/labextension/static/41.1846c3ba970651a706b6.js` & `ipydatagrid-1.3.1/ipydatagrid/labextension/static/41.1846c3ba970651a706b6.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.0/ipydatagrid/labextension/static/433.75ed253aaa8060b28c81.js` & `ipydatagrid-1.3.1/ipydatagrid/labextension/static/433.75ed253aaa8060b28c81.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.0/ipydatagrid/labextension/static/455.25b625d30041b5a1671c.js` & `ipydatagrid-1.3.1/ipydatagrid/labextension/static/455.25b625d30041b5a1671c.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.0/ipydatagrid/labextension/static/456.afd75d5e116998d22e56.js` & `ipydatagrid-1.3.1/ipydatagrid/labextension/static/456.afd75d5e116998d22e56.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.0/ipydatagrid/labextension/static/462.68e4d74f02bf2411528e.js` & `ipydatagrid-1.3.1/ipydatagrid/labextension/static/462.68e4d74f02bf2411528e.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.0/ipydatagrid/labextension/static/48.732e43cec274cf5b8cf5.js` & `ipydatagrid-1.3.1/ipydatagrid/labextension/static/48.732e43cec274cf5b8cf5.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.0/ipydatagrid/labextension/static/481.911a23288443c8041987.js` & `ipydatagrid-1.3.1/ipydatagrid/labextension/static/481.911a23288443c8041987.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.0/ipydatagrid/labextension/static/513.73d1ca46ed758871d49a.js` & `ipydatagrid-1.3.1/ipydatagrid/labextension/static/513.73d1ca46ed758871d49a.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.0/ipydatagrid/labextension/static/568.2b5bb2c0c4fdfa06786c.js` & `ipydatagrid-1.3.1/ipydatagrid/labextension/static/568.2b5bb2c0c4fdfa06786c.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.0/ipydatagrid/labextension/static/642.730227a42292c5f89120.js` & `ipydatagrid-1.3.1/ipydatagrid/labextension/static/642.730227a42292c5f89120.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.0/ipydatagrid/labextension/static/643.a265dd26cb50ebd06923.js` & `ipydatagrid-1.3.1/ipydatagrid/labextension/static/643.a265dd26cb50ebd06923.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.0/ipydatagrid/labextension/static/679.e174128fe156c1cd0d10.js` & `ipydatagrid-1.3.1/ipydatagrid/labextension/static/679.e174128fe156c1cd0d10.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.0/ipydatagrid/labextension/static/683.efe59705c1680a8f8b3a.js` & `ipydatagrid-1.3.1/ipydatagrid/labextension/static/683.efe59705c1680a8f8b3a.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.0/ipydatagrid/labextension/static/700.7f792a9e7380bfde28dc.js` & `ipydatagrid-1.3.1/ipydatagrid/labextension/static/700.7f792a9e7380bfde28dc.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.0/ipydatagrid/labextension/static/762.42901b906691b1301214.js` & `ipydatagrid-1.3.1/ipydatagrid/labextension/static/762.42901b906691b1301214.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.0/ipydatagrid/labextension/static/781.ef3f9c2a235c4a40bdc0.js` & `ipydatagrid-1.3.1/ipydatagrid/labextension/static/781.ef3f9c2a235c4a40bdc0.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.0/ipydatagrid/labextension/static/787.f307b1ca46997f4a9051.js` & `ipydatagrid-1.3.1/ipydatagrid/labextension/static/787.47c1e167bb24294e1e7e.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1214,15 +1214,17 @@
                                 command: a.CommandID.RevertGrid,
                                 args: i
                             });
                             break;
                         default:
                             throw "unreachable"
                     }
-                    this._menu.open(t.x, t.y)
+                    this._menu.open(t.x, t.y);
+                    const n = document.body.firstElementChild;
+                    this._menu.node.parentElement == document.body && n != this._menu.node && (r.Widget.detach(this._menu), r.Widget.attach(this._menu, document.body, n))
                 }
             }
             t.FeatherGridContextMenu = a,
                 function(e) {
                     let t;
                     ! function(e) {
                         e.SortAscending = "sort:Asc", e.SortDescending = "sort:Desc", e.SortClear = "sort:Clear", e.OpenFilterByConditionDialog = "filterCondition:openDialog", e.OpenFilterByValueDialog = "filterValue:openDialog", e.RevertGrid = "grid:reset", e.ClearThisFilter = "filter:clearCurrentColumn", e.ClearFiltersInAllColumns = "filter:clearAllColumns", e.CopyToClipboard = "copyToClipboard", e.CopySelectionToClipboard = "copySelectionToClipboard", e.SaveSelectionAsCsv = "saveSelectionAsCsv", e.SaveAllAsCsv = "saveAllAsCsv", e.ClearSelection = "clearSelection"
@@ -2262,15 +2264,26 @@
                 },
                 header_renderer: {
                     deserialize: c.unpack_models
                 },
                 _data: {
                     deserialize: function(e, t) {
                         const i = {};
-                        for (const r of Object.keys(e.data)) "raw" == e.data[r].type ? i[r] = b(e.data[r].value) : i[r] = u.array_or_json_serializer.deserialize(e.data[r], t);
+                        if (Array.isArray(e.data)) {
+                            if (0 === e.data.length) return new f.DataSource(i, e.fields, e.schema, !0);
+                            const t = b(e.data);
+                            for (const e of Object.keys(t[0])) {
+                                const r = new Array(t.length);
+                                let n = 0;
+                                for (const i of t) r[n++] = i[e];
+                                i[e] = r
+                            }
+                            return new f.DataSource(i, e.fields, e.schema, !0)
+                        }
+                        for (const r of Object.keys(e.data)) i[r] = [], Array.isArray(e.data[r]) ? i[r] = e.data[r] : "raw" == e.data[r].type ? i[r] = b(e.data[r].value) : 0 !== e.data[r].value.length && (i[r] = u.array_or_json_serializer.deserialize(e.data[r], t));
                         return new f.DataSource(i, e.fields, e.schema, !0)
                     },
                     serialize: function(e, t) {
                         const i = {};
                         for (const r of Object.keys(e.data)) i[r] = u.array_or_json_serializer.serialize(e.data[r], t);
                         return {
                             data: i,
@@ -3465,11 +3478,11 @@
         7888: e => {
             e.exports = "data:image/svg+xml,%3csvg class='bi bi-filter' width='1em' height='1em' viewBox='0 0 20 20' fill='white' xmlns='http://www.w3.org/2000/svg'%3e %3cpath fill-rule='evenodd' d='M7.5 13a.5.5 0 01.5-.5h4a.5.5 0 010 1H8a.5.5 0 01-.5-.5zm-2-3a.5.5 0 01.5-.5h8a.5.5 0 010 1H6a.5.5 0 01-.5-.5zm-2-3a.5.5 0 01.5-.5h12a.5.5 0 010 1H4a.5.5 0 01-.5-.5z' clip-rule='evenodd'/%3e %3c/svg%3e"
         },
         7509: e => {
             e.exports = "data:image/svg+xml,%3csvg class='bi bi-filter' width='1em' height='1em' viewBox='0 0 20 20' fill='black' xmlns='http://www.w3.org/2000/svg'%3e %3cpath fill-rule='evenodd' d='M7.5 13a.5.5 0 01.5-.5h4a.5.5 0 010 1H8a.5.5 0 01-.5-.5zm-2-3a.5.5 0 01.5-.5h8a.5.5 0 010 1H6a.5.5 0 01-.5-.5zm-2-3a.5.5 0 01.5-.5h12a.5.5 0 010 1H4a.5.5 0 01-.5-.5z' clip-rule='evenodd'/%3e %3c/svg%3e"
         },
         4147: e => {
-            e.exports = JSON.parse('{"name":"ipydatagrid","version":"1.3.0","description":"Fast Datagrid widget for the Jupyter Notebook and JupyterLab","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","lib/**/*.js.map","lib/**/*.ts","dist/*.js","dist/*.js.map","dist/*.png","style/**/*.*"],"homepage":"https://github.com/Bloomberg/ipydatagrid","bugs":{"url":"https://github.com/Bloomberg/ipydatagrid/issues"},"license":"BSD-3-Clause","author":{"name":"Bloomberg","email":""},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/Bloomberg/ipydatagrid"},"scripts":{"build":"jlpm run build:lib && jlpm run build:nbextension && jlpm run build:labextension","build:dev":"jlpm run build:lib && jlpm run build:nbextension && jlpm run build:labextension:dev","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack --mode=production --no-devtool","build:widget-examples":"cd widget-examples/basic && webpack --mode=production","build:all":"jlpm run build:labextension && jlpm run build:nbextension && jlpm run build:widget-examples","clean":"rimraf dist && jlpm run clean:lib && jlpm run clean:labextension && jlpm run clean:nbextension","clean:lib":"rimraf lib","clean:labextension":"rimraf ipydatagrid/labextension","clean:nbextension":"rimraf ipydatagrid/nbextension/index.*","lint":"eslint \'js/**/*.{js,ts}\' --quiet --fix","prepack":"jlpm run build:labextension && jlpm run build:nbextension","test":"jest --verbose","watch":"npm-run-all -p watch:lib watch:labextension watch:nbextension","watch:lib":"tsc -w","watch:nbextension":"webpack --watch","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^2 || ^3 || ^4 || ^6","@jupyterlab/apputils":"^3 || ^4","@lumino/algorithm":"^1 || ^2","@lumino/application":"^1 || ^2","@lumino/commands":"^1 || ^2","@lumino/coreutils":"^1 || ^2","@lumino/datagrid":"^1 || ^2","@lumino/default-theme":"^1 || ^2","@lumino/domutils":"^1 || ^2","@lumino/messaging":"^1 || ^2","@lumino/signaling":"^1 || ^2","@lumino/virtualdom":"^1 || ^2","@lumino/widgets":"^1 || ^2","bqplot":"^0.5","core-js-pure":"^3.30.2","d3-array":"^2.2.0","d3-color":"^3.1.0","d3-format":"^1.3.2","d3-scale":"^3.0.0","d3-time-format":"^2.1.3","jest-environment-jsdom":"^28.1.3","moment":"^2.24.0","underscore":"^1.13.6","vega-expression":"^2.6.0","vega-format":"^1.1.1","vega-functions":"^5.3.0"},"devDependencies":{"@babel/cli":"^7.6.3","@babel/core":"^7.6.3","@babel/preset-env":"^7.6.3","@babel/preset-typescript":"^7.6.0","@jupyterlab/builder":"^4.0.5","@types/jest":"^27.4.1","@types/node":"^10.11.6","@types/underscore":"^1.11.4","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.5.0","@typescript-eslint/parser":"^3.5.0","acorn":"^6.2.0","babel-jest":"^28.1.3","babel-plugin-transform-es2015-modules-commonjs":"^6.26.2","css-loader":"^6.8.1","eslint":"^7.3.1","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","fs-extra":"^7.0.0","jest":"^28.1.3","jest-raw-loader":"^1.0.1","lint-staged":"^10.2.11","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","raw-loader":"^4.0.2","rimraf":"^2.6.2","source-map-loader":"^0.2.4","style-loader":"^3.3.3","svg-url-loader":"~3.0.3","ts-jest":"^28.0.8","ts-loader":"^6.0.4","typescript":"~4.2.4","url-loader":"^4.1.0","webpack":"^5.88.2","webpack-cli":"^4.4.0"},"jupyterlab":{"extension":"lib/plugin","webpackConfig":"webpack.lab.config.js","outputDir":"./ipydatagrid/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true},"bqplot":{"bundled":false,"singleton":true},"@lumino/algorithm":{"bundled":false,"singleton":true},"@lumino/commands":{"bundled":false,"singleton":true},"@lumino/coreutils":{"bundled":false,"singleton":true},"@lumino/datagrid":{"bundled":false,"singleton":true},"@lumino/default-theme":{"bundled":false,"singleton":true},"@lumino/domutils":{"bundled":false,"singleton":true},"@lumino/messaging":{"bundled":false,"singleton":true},"@lumino/virtualdom":{"bundled":false,"singleton":true},"@lumino/widgets":{"bundled":false,"singleton":true}}},"packageManager":"yarn@3.7.0"}')
+            e.exports = JSON.parse('{"name":"ipydatagrid","version":"1.3.1","description":"Fast Datagrid widget for the Jupyter Notebook and JupyterLab","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","lib/**/*.js.map","lib/**/*.ts","dist/*.js","dist/*.js.map","dist/*.png","style/**/*.*"],"homepage":"https://github.com/Bloomberg/ipydatagrid","bugs":{"url":"https://github.com/Bloomberg/ipydatagrid/issues"},"license":"BSD-3-Clause","author":{"name":"Bloomberg","email":""},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/Bloomberg/ipydatagrid"},"scripts":{"build":"jlpm run build:lib && jlpm run build:nbextension && jlpm run build:labextension","build:dev":"jlpm run build:lib && jlpm run build:nbextension && jlpm run build:labextension:dev","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack --mode=production --no-devtool","build:widget-examples":"cd widget-examples/basic && webpack --mode=production","build:all":"jlpm run build:labextension && jlpm run build:nbextension && jlpm run build:widget-examples","clean":"rimraf dist && jlpm run clean:lib && jlpm run clean:labextension && jlpm run clean:nbextension","clean:lib":"rimraf lib","clean:labextension":"rimraf ipydatagrid/labextension","clean:nbextension":"rimraf ipydatagrid/nbextension/index.*","lint":"eslint \'js/**/*.{js,ts}\' --quiet --fix","prepack":"jlpm run build:labextension && jlpm run build:nbextension","test":"jest --verbose","watch":"npm-run-all -p watch:lib watch:labextension watch:nbextension","watch:lib":"tsc -w","watch:nbextension":"webpack --watch","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^2 || ^3 || ^4 || ^6","@jupyterlab/apputils":"^3 || ^4","@lumino/algorithm":"^1 || ^2","@lumino/application":"^1 || ^2","@lumino/commands":"^1 || ^2","@lumino/coreutils":"^1 || ^2","@lumino/datagrid":"^1 || ^2","@lumino/default-theme":"^1 || ^2","@lumino/domutils":"^1 || ^2","@lumino/messaging":"^1 || ^2","@lumino/signaling":"^1 || ^2","@lumino/virtualdom":"^1 || ^2","@lumino/widgets":"^1 || ^2","bqplot":"^0.5","core-js-pure":"^3.30.2","d3-array":"^2.2.0","d3-color":"^3.1.0","d3-format":"^1.3.2","d3-scale":"^3.0.0","d3-time-format":"^2.1.3","jest-environment-jsdom":"^28.1.3","moment":"^2.24.0","underscore":"^1.13.6","vega-expression":"^2.6.0","vega-format":"^1.1.1","vega-functions":"^5.3.0"},"devDependencies":{"@babel/cli":"^7.6.3","@babel/core":"^7.6.3","@babel/preset-env":"^7.6.3","@babel/preset-typescript":"^7.6.0","@jupyterlab/builder":"^4.0.5","@types/jest":"^27.4.1","@types/node":"^10.11.6","@types/underscore":"^1.11.4","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.5.0","@typescript-eslint/parser":"^3.5.0","acorn":"^6.2.0","babel-jest":"^28.1.3","babel-plugin-transform-es2015-modules-commonjs":"^6.26.2","css-loader":"^6.8.1","eslint":"^7.3.1","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","fs-extra":"^7.0.0","jest":"^28.1.3","jest-raw-loader":"^1.0.1","lint-staged":"^10.2.11","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","raw-loader":"^4.0.2","rimraf":"^2.6.2","source-map-loader":"^0.2.4","style-loader":"^3.3.3","svg-url-loader":"~3.0.3","ts-jest":"^28.0.8","ts-loader":"^6.0.4","typescript":"~4.2.4","url-loader":"^4.1.0","webpack":"^5.88.2","webpack-cli":"^4.4.0"},"jupyterlab":{"extension":"lib/plugin","webpackConfig":"webpack.lab.config.js","outputDir":"./ipydatagrid/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true},"bqplot":{"bundled":false,"singleton":true},"@lumino/algorithm":{"bundled":false,"singleton":true},"@lumino/commands":{"bundled":false,"singleton":true},"@lumino/coreutils":{"bundled":false,"singleton":true},"@lumino/datagrid":{"bundled":false,"singleton":true},"@lumino/default-theme":{"bundled":false,"singleton":true},"@lumino/domutils":{"bundled":false,"singleton":true},"@lumino/messaging":{"bundled":false,"singleton":true},"@lumino/virtualdom":{"bundled":false,"singleton":true},"@lumino/widgets":{"bundled":false,"singleton":true}}},"packageManager":"yarn@3.7.0"}')
         }
     }
 ]);
```

### Comparing `ipydatagrid-1.3.0/ipydatagrid/labextension/static/794.d7c23e15137c8752365e.js` & `ipydatagrid-1.3.1/ipydatagrid/labextension/static/794.d7c23e15137c8752365e.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.0/ipydatagrid/labextension/static/811.a135ebc21be585e6d76d.js` & `ipydatagrid-1.3.1/ipydatagrid/labextension/static/811.a135ebc21be585e6d76d.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.0/ipydatagrid/labextension/static/823.18e09aad57c7797df987.js` & `ipydatagrid-1.3.1/ipydatagrid/labextension/static/823.18e09aad57c7797df987.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.0/ipydatagrid/labextension/static/917.b972bc5b41fae8990bff.js` & `ipydatagrid-1.3.1/ipydatagrid/labextension/static/917.b972bc5b41fae8990bff.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.0/ipydatagrid/labextension/static/939.04c5876588e4898127e3.js` & `ipydatagrid-1.3.1/ipydatagrid/labextension/static/939.04c5876588e4898127e3.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.0/ipydatagrid/labextension/static/941.23c8b1f0eb18afd531e9.js` & `ipydatagrid-1.3.1/ipydatagrid/labextension/static/941.23c8b1f0eb18afd531e9.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.0/ipydatagrid/labextension/static/990.e35c256305f259cdaeb9.js` & `ipydatagrid-1.3.1/ipydatagrid/labextension/static/990.e35c256305f259cdaeb9.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.0/ipydatagrid/labextension/static/remoteEntry.e416f171876299bb6885.js` & `ipydatagrid-1.3.1/ipydatagrid/labextension/static/remoteEntry.6d509d1468636d15eab8.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -71,15 +71,15 @@
         643: "a265dd26cb50ebd06923",
         679: "e174128fe156c1cd0d10",
         683: "efe59705c1680a8f8b3a",
         689: "3cdb49d94599b1683563",
         700: "7f792a9e7380bfde28dc",
         762: "42901b906691b1301214",
         781: "ef3f9c2a235c4a40bdc0",
-        787: "f307b1ca46997f4a9051",
+        787: "47c1e167bb24294e1e7e",
         794: "d7c23e15137c8752365e",
         811: "a135ebc21be585e6d76d",
         823: "18e09aad57c7797df987",
         917: "b972bc5b41fae8990bff",
         939: "04c5876588e4898127e3",
         941: "23c8b1f0eb18afd531e9",
         990: "e35c256305f259cdaeb9"
@@ -108,15 +108,15 @@
         643: "a265dd26cb50ebd06923",
         679: "e174128fe156c1cd0d10",
         683: "efe59705c1680a8f8b3a",
         689: "3cdb49d94599b1683563",
         700: "7f792a9e7380bfde28dc",
         762: "42901b906691b1301214",
         781: "ef3f9c2a235c4a40bdc0",
-        787: "f307b1ca46997f4a9051",
+        787: "47c1e167bb24294e1e7e",
         794: "d7c23e15137c8752365e",
         811: "a135ebc21be585e6d76d",
         823: "18e09aad57c7797df987",
         917: "b972bc5b41fae8990bff",
         939: "04c5876588e4898127e3",
         941: "23c8b1f0eb18afd531e9",
         990: "e35c256305f259cdaeb9"
@@ -175,15 +175,15 @@
                         (!f || !f.loaded && (!r != !f.eager ? r : o > f.from)) && (d[a] = {
                             get: t,
                             from: o,
                             eager: !!r
                         })
                     },
                     i = [];
-                return "default" === t && (f("d3-array", "3.2.4", (() => P.e(433).then((() => () => P(3433))))), f("d3-array", "3.2.4", (() => P.e(455).then((() => () => P(2455))))), f("d3-array", "3.2.4", (() => P.e(513).then((() => () => P(5513))))), f("d3-array", "3.2.4", (() => P.e(643).then((() => () => P(8643))))), f("d3-array", "3.2.4", (() => P.e(41).then((() => () => P(8041))))), f("d3-array", "3.2.4", (() => P.e(109).then((() => () => P(109))))), f("d3-color", "3.1.0", (() => P.e(811).then((() => () => P(4811))))), f("d3-format", "1.4.5", (() => P.e(481).then((() => () => P(8481))))), f("d3-format", "3.1.0", (() => P.e(142).then((() => () => P(2142))))), f("d3-format", "3.1.0", (() => P.e(462).then((() => () => P(7271))))), f("d3-scale", "4.0.2", (() => Promise.all([P.e(781), P.e(622), P.e(112), P.e(456)]).then((() => () => P(2781))))), f("d3-time-format", "2.3.0", (() => P.e(48).then((() => () => P(4048))))), f("d3-time-format", "4.1.0", (() => P.e(941).then((() => () => P(6941))))), f("d3-time-format", "4.1.0", (() => P.e(683).then((() => () => P(271))))), f("ipydatagrid", "1.3.0", (() => Promise.all([P.e(939), P.e(268), P.e(787), P.e(568)]).then((() => () => P(1568))))), f("moment", "2.29.4", (() => Promise.all([P.e(762), P.e(700)]).then((() => () => P(381))))), f("underscore", "1.13.6", (() => P.e(794).then((() => () => P(7794))))), f("vega-expression", "2.7.0", (() => P.e(351).then((() => () => P(6351))))), f("vega-expression", "5.1.0", (() => Promise.all([P.e(143), P.e(823)]).then((() => () => P(8143))))), f("vega-expression", "5.1.0", (() => Promise.all([P.e(917), P.e(990)]).then((() => () => P(9917))))), f("vega-format", "1.1.1", (() => Promise.all([P.e(642), P.e(689), P.e(400)]).then((() => () => P(7400))))), f("vega-functions", "5.14.0", (() => Promise.all([P.e(642), P.e(679), P.e(268), P.e(622), P.e(689), P.e(159)]).then((() => () => P(679)))))), e[t] = i.length ? Promise.all(i).then((() => e[t] = 1)) : 1
+                return "default" === t && (f("d3-array", "3.2.4", (() => P.e(433).then((() => () => P(3433))))), f("d3-array", "3.2.4", (() => P.e(455).then((() => () => P(2455))))), f("d3-array", "3.2.4", (() => P.e(513).then((() => () => P(5513))))), f("d3-array", "3.2.4", (() => P.e(643).then((() => () => P(8643))))), f("d3-array", "3.2.4", (() => P.e(41).then((() => () => P(8041))))), f("d3-array", "3.2.4", (() => P.e(109).then((() => () => P(109))))), f("d3-color", "3.1.0", (() => P.e(811).then((() => () => P(4811))))), f("d3-format", "1.4.5", (() => P.e(481).then((() => () => P(8481))))), f("d3-format", "3.1.0", (() => P.e(142).then((() => () => P(2142))))), f("d3-format", "3.1.0", (() => P.e(462).then((() => () => P(7271))))), f("d3-scale", "4.0.2", (() => Promise.all([P.e(781), P.e(622), P.e(112), P.e(456)]).then((() => () => P(2781))))), f("d3-time-format", "2.3.0", (() => P.e(48).then((() => () => P(4048))))), f("d3-time-format", "4.1.0", (() => P.e(941).then((() => () => P(6941))))), f("d3-time-format", "4.1.0", (() => P.e(683).then((() => () => P(271))))), f("ipydatagrid", "1.3.1", (() => Promise.all([P.e(939), P.e(268), P.e(787), P.e(568)]).then((() => () => P(1568))))), f("moment", "2.29.4", (() => Promise.all([P.e(762), P.e(700)]).then((() => () => P(381))))), f("underscore", "1.13.6", (() => P.e(794).then((() => () => P(7794))))), f("vega-expression", "2.7.0", (() => P.e(351).then((() => () => P(6351))))), f("vega-expression", "5.1.0", (() => Promise.all([P.e(143), P.e(823)]).then((() => () => P(8143))))), f("vega-expression", "5.1.0", (() => Promise.all([P.e(917), P.e(990)]).then((() => () => P(9917))))), f("vega-format", "1.1.1", (() => Promise.all([P.e(642), P.e(689), P.e(400)]).then((() => () => P(7400))))), f("vega-functions", "5.14.0", (() => Promise.all([P.e(642), P.e(679), P.e(268), P.e(622), P.e(689), P.e(159)]).then((() => () => P(679)))))), e[t] = i.length ? Promise.all(i).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         P.g.importScripts && (e = P.g.location + "");
         var a = P.g.document;
         if (!e && a && (a.currentScript && (e = a.currentScript.src), !e)) {
```

### Comparing `ipydatagrid-1.3.0/ipydatagrid/labextension/static/third-party-licenses.json` & `ipydatagrid-1.3.1/ipydatagrid/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.0/ipydatagrid/nbextension/index.js` & `ipydatagrid-1.3.1/ipydatagrid/nbextension/index.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -89125,15 +89125,17 @@
                                     command: s.CommandID.RevertGrid,
                                     args: n
                                 });
                                 break;
                             default:
                                 throw "unreachable"
                         }
-                        this._menu.open(t.x, t.y)
+                        this._menu.open(t.x, t.y);
+                        const r = document.body.firstElementChild;
+                        this._menu.node.parentElement == document.body && r != this._menu.node && (i.Widget.detach(this._menu), i.Widget.attach(this._menu, document.body, r))
                     }
                 }
                 t.FeatherGridContextMenu = s,
                     function(e) {
                         let t;
                         ! function(e) {
                             e.SortAscending = "sort:Asc", e.SortDescending = "sort:Desc", e.SortClear = "sort:Clear", e.OpenFilterByConditionDialog = "filterCondition:openDialog", e.OpenFilterByValueDialog = "filterValue:openDialog", e.RevertGrid = "grid:reset", e.ClearThisFilter = "filter:clearCurrentColumn", e.ClearFiltersInAllColumns = "filter:clearAllColumns", e.CopyToClipboard = "copyToClipboard", e.CopySelectionToClipboard = "copySelectionToClipboard", e.SaveSelectionAsCsv = "saveSelectionAsCsv", e.SaveAllAsCsv = "saveAllAsCsv", e.ClearSelection = "clearSelection"
@@ -90181,15 +90183,26 @@
                     },
                     header_renderer: {
                         deserialize: h.unpack_models
                     },
                     _data: {
                         deserialize: function(e, t) {
                             const n = {};
-                            for (const i of Object.keys(e.data)) "raw" == e.data[i].type ? n[i] = y(e.data[i].value) : n[i] = d.array_or_json_serializer.deserialize(e.data[i], t);
+                            if (Array.isArray(e.data)) {
+                                if (0 === e.data.length) return new g.DataSource(n, e.fields, e.schema, !0);
+                                const t = y(e.data);
+                                for (const e of Object.keys(t[0])) {
+                                    const i = new Array(t.length);
+                                    let r = 0;
+                                    for (const n of t) i[r++] = n[e];
+                                    n[e] = i
+                                }
+                                return new g.DataSource(n, e.fields, e.schema, !0)
+                            }
+                            for (const i of Object.keys(e.data)) n[i] = [], Array.isArray(e.data[i]) ? n[i] = e.data[i] : "raw" == e.data[i].type ? n[i] = y(e.data[i].value) : 0 !== e.data[i].value.length && (n[i] = d.array_or_json_serializer.deserialize(e.data[i], t));
                             return new g.DataSource(n, e.fields, e.schema, !0)
                         },
                         serialize: function(e, t) {
                             const n = {};
                             for (const i of Object.keys(e.data)) n[i] = d.array_or_json_serializer.serialize(e.data[i], t);
                             return {
                                 data: n,
@@ -93254,15 +93267,15 @@
                 "use strict";
                 e.exports = {
                     version: "0.5.43"
                 }
             },
             4147: e => {
                 "use strict";
-                e.exports = JSON.parse('{"name":"ipydatagrid","version":"1.3.0","description":"Fast Datagrid widget for the Jupyter Notebook and JupyterLab","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","lib/**/*.js.map","lib/**/*.ts","dist/*.js","dist/*.js.map","dist/*.png","style/**/*.*"],"homepage":"https://github.com/Bloomberg/ipydatagrid","bugs":{"url":"https://github.com/Bloomberg/ipydatagrid/issues"},"license":"BSD-3-Clause","author":{"name":"Bloomberg","email":""},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/Bloomberg/ipydatagrid"},"scripts":{"build":"jlpm run build:lib && jlpm run build:nbextension && jlpm run build:labextension","build:dev":"jlpm run build:lib && jlpm run build:nbextension && jlpm run build:labextension:dev","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack --mode=production --no-devtool","build:widget-examples":"cd widget-examples/basic && webpack --mode=production","build:all":"jlpm run build:labextension && jlpm run build:nbextension && jlpm run build:widget-examples","clean":"rimraf dist && jlpm run clean:lib && jlpm run clean:labextension && jlpm run clean:nbextension","clean:lib":"rimraf lib","clean:labextension":"rimraf ipydatagrid/labextension","clean:nbextension":"rimraf ipydatagrid/nbextension/index.*","lint":"eslint \'js/**/*.{js,ts}\' --quiet --fix","prepack":"jlpm run build:labextension && jlpm run build:nbextension","test":"jest --verbose","watch":"npm-run-all -p watch:lib watch:labextension watch:nbextension","watch:lib":"tsc -w","watch:nbextension":"webpack --watch","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^2 || ^3 || ^4 || ^6","@jupyterlab/apputils":"^3 || ^4","@lumino/algorithm":"^1 || ^2","@lumino/application":"^1 || ^2","@lumino/commands":"^1 || ^2","@lumino/coreutils":"^1 || ^2","@lumino/datagrid":"^1 || ^2","@lumino/default-theme":"^1 || ^2","@lumino/domutils":"^1 || ^2","@lumino/messaging":"^1 || ^2","@lumino/signaling":"^1 || ^2","@lumino/virtualdom":"^1 || ^2","@lumino/widgets":"^1 || ^2","bqplot":"^0.5","core-js-pure":"^3.30.2","d3-array":"^2.2.0","d3-color":"^3.1.0","d3-format":"^1.3.2","d3-scale":"^3.0.0","d3-time-format":"^2.1.3","jest-environment-jsdom":"^28.1.3","moment":"^2.24.0","underscore":"^1.13.6","vega-expression":"^2.6.0","vega-format":"^1.1.1","vega-functions":"^5.3.0"},"devDependencies":{"@babel/cli":"^7.6.3","@babel/core":"^7.6.3","@babel/preset-env":"^7.6.3","@babel/preset-typescript":"^7.6.0","@jupyterlab/builder":"^4.0.5","@types/jest":"^27.4.1","@types/node":"^10.11.6","@types/underscore":"^1.11.4","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.5.0","@typescript-eslint/parser":"^3.5.0","acorn":"^6.2.0","babel-jest":"^28.1.3","babel-plugin-transform-es2015-modules-commonjs":"^6.26.2","css-loader":"^6.8.1","eslint":"^7.3.1","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","fs-extra":"^7.0.0","jest":"^28.1.3","jest-raw-loader":"^1.0.1","lint-staged":"^10.2.11","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","raw-loader":"^4.0.2","rimraf":"^2.6.2","source-map-loader":"^0.2.4","style-loader":"^3.3.3","svg-url-loader":"~3.0.3","ts-jest":"^28.0.8","ts-loader":"^6.0.4","typescript":"~4.2.4","url-loader":"^4.1.0","webpack":"^5.88.2","webpack-cli":"^4.4.0"},"jupyterlab":{"extension":"lib/plugin","webpackConfig":"webpack.lab.config.js","outputDir":"./ipydatagrid/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true},"bqplot":{"bundled":false,"singleton":true},"@lumino/algorithm":{"bundled":false,"singleton":true},"@lumino/commands":{"bundled":false,"singleton":true},"@lumino/coreutils":{"bundled":false,"singleton":true},"@lumino/datagrid":{"bundled":false,"singleton":true},"@lumino/default-theme":{"bundled":false,"singleton":true},"@lumino/domutils":{"bundled":false,"singleton":true},"@lumino/messaging":{"bundled":false,"singleton":true},"@lumino/virtualdom":{"bundled":false,"singleton":true},"@lumino/widgets":{"bundled":false,"singleton":true}}},"packageManager":"yarn@3.7.0"}')
+                e.exports = JSON.parse('{"name":"ipydatagrid","version":"1.3.1","description":"Fast Datagrid widget for the Jupyter Notebook and JupyterLab","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","lib/**/*.js.map","lib/**/*.ts","dist/*.js","dist/*.js.map","dist/*.png","style/**/*.*"],"homepage":"https://github.com/Bloomberg/ipydatagrid","bugs":{"url":"https://github.com/Bloomberg/ipydatagrid/issues"},"license":"BSD-3-Clause","author":{"name":"Bloomberg","email":""},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/Bloomberg/ipydatagrid"},"scripts":{"build":"jlpm run build:lib && jlpm run build:nbextension && jlpm run build:labextension","build:dev":"jlpm run build:lib && jlpm run build:nbextension && jlpm run build:labextension:dev","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack --mode=production --no-devtool","build:widget-examples":"cd widget-examples/basic && webpack --mode=production","build:all":"jlpm run build:labextension && jlpm run build:nbextension && jlpm run build:widget-examples","clean":"rimraf dist && jlpm run clean:lib && jlpm run clean:labextension && jlpm run clean:nbextension","clean:lib":"rimraf lib","clean:labextension":"rimraf ipydatagrid/labextension","clean:nbextension":"rimraf ipydatagrid/nbextension/index.*","lint":"eslint \'js/**/*.{js,ts}\' --quiet --fix","prepack":"jlpm run build:labextension && jlpm run build:nbextension","test":"jest --verbose","watch":"npm-run-all -p watch:lib watch:labextension watch:nbextension","watch:lib":"tsc -w","watch:nbextension":"webpack --watch","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^2 || ^3 || ^4 || ^6","@jupyterlab/apputils":"^3 || ^4","@lumino/algorithm":"^1 || ^2","@lumino/application":"^1 || ^2","@lumino/commands":"^1 || ^2","@lumino/coreutils":"^1 || ^2","@lumino/datagrid":"^1 || ^2","@lumino/default-theme":"^1 || ^2","@lumino/domutils":"^1 || ^2","@lumino/messaging":"^1 || ^2","@lumino/signaling":"^1 || ^2","@lumino/virtualdom":"^1 || ^2","@lumino/widgets":"^1 || ^2","bqplot":"^0.5","core-js-pure":"^3.30.2","d3-array":"^2.2.0","d3-color":"^3.1.0","d3-format":"^1.3.2","d3-scale":"^3.0.0","d3-time-format":"^2.1.3","jest-environment-jsdom":"^28.1.3","moment":"^2.24.0","underscore":"^1.13.6","vega-expression":"^2.6.0","vega-format":"^1.1.1","vega-functions":"^5.3.0"},"devDependencies":{"@babel/cli":"^7.6.3","@babel/core":"^7.6.3","@babel/preset-env":"^7.6.3","@babel/preset-typescript":"^7.6.0","@jupyterlab/builder":"^4.0.5","@types/jest":"^27.4.1","@types/node":"^10.11.6","@types/underscore":"^1.11.4","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.5.0","@typescript-eslint/parser":"^3.5.0","acorn":"^6.2.0","babel-jest":"^28.1.3","babel-plugin-transform-es2015-modules-commonjs":"^6.26.2","css-loader":"^6.8.1","eslint":"^7.3.1","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","fs-extra":"^7.0.0","jest":"^28.1.3","jest-raw-loader":"^1.0.1","lint-staged":"^10.2.11","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","raw-loader":"^4.0.2","rimraf":"^2.6.2","source-map-loader":"^0.2.4","style-loader":"^3.3.3","svg-url-loader":"~3.0.3","ts-jest":"^28.0.8","ts-loader":"^6.0.4","typescript":"~4.2.4","url-loader":"^4.1.0","webpack":"^5.88.2","webpack-cli":"^4.4.0"},"jupyterlab":{"extension":"lib/plugin","webpackConfig":"webpack.lab.config.js","outputDir":"./ipydatagrid/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true},"bqplot":{"bundled":false,"singleton":true},"@lumino/algorithm":{"bundled":false,"singleton":true},"@lumino/commands":{"bundled":false,"singleton":true},"@lumino/coreutils":{"bundled":false,"singleton":true},"@lumino/datagrid":{"bundled":false,"singleton":true},"@lumino/default-theme":{"bundled":false,"singleton":true},"@lumino/domutils":{"bundled":false,"singleton":true},"@lumino/messaging":{"bundled":false,"singleton":true},"@lumino/virtualdom":{"bundled":false,"singleton":true},"@lumino/widgets":{"bundled":false,"singleton":true}}},"packageManager":"yarn@3.7.0"}')
             }
         },
         n = {};
 
     function i(e) {
         var r = n[e];
         if (void 0 !== r) return r.exports;
```

### Comparing `ipydatagrid-1.3.0/ipydatagrid/nbextension/index.js.LICENSE.txt` & `ipydatagrid-1.3.1/ipydatagrid/nbextension/index.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.0/js/cellrenderer.ts` & `ipydatagrid-1.3.1/js/cellrenderer.ts`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.0/js/datagrid.ts` & `ipydatagrid-1.3.1/js/datagrid.ts`

 * *Files 2% similar despite different names*

```diff
@@ -79,22 +79,55 @@
     );
   }
   return { data: serialized_data, fields: data.fields, schema: data.schema };
 }
 
 function deserialize_data(data: any, manager: any): DataSource {
   const deserialized_data: any = {};
+
+  // Backward compatibility for when data.data was an array of rows
+  // (should be removed in ipydatagrid 2.x?)
+  if (Array.isArray(data.data)) {
+    if (data.data.length === 0) {
+      return new DataSource(deserialized_data, data.fields, data.schema, true);
+    }
+
+    const unpacked = unpack_raw_data(data.data);
+    // Turn array of rows (old approach) into a dictionary of columns as arrays (new approach)
+    for (const column of Object.keys(unpacked[0])) {
+      const columnData = new Array(unpacked.length);
+      let rowIdx = 0;
+
+      for (const row of unpacked) {
+        columnData[rowIdx++] = row[column];
+      }
+
+      deserialized_data[column] = columnData;
+    }
+
+    return new DataSource(deserialized_data, data.fields, data.schema, true);
+  }
+
   for (const column of Object.keys(data.data)) {
+    deserialized_data[column] = [];
+
+    if (Array.isArray(data.data[column])) {
+      deserialized_data[column] = data.data[column];
+      continue;
+    }
+
     if (data.data[column].type == 'raw') {
       deserialized_data[column] = unpack_raw_data(data.data[column].value);
     } else {
-      deserialized_data[column] = array_or_json_serializer.deserialize(
-        data.data[column],
-        manager,
-      );
+      if (data.data[column].value.length !== 0) {
+        deserialized_data[column] = array_or_json_serializer.deserialize(
+          data.data[column],
+          manager,
+        );
+      }
     }
   }
   return new DataSource(deserialized_data, data.fields, data.schema, true);
 }
 
 export class DataGridModel extends DOMWidgetModel {
   defaults() {
@@ -454,15 +487,18 @@
     this.el.classList.add('datagrid-container');
     window.addEventListener('resize', this.manageResizeEvent);
     this.once('remove', () => {
       window.removeEventListener('resize', this.manageResizeEvent);
     });
 
     const grid_style = this.model.get('grid_style');
-    if (this.model.get('horizontal_stripes') || this.model.get('vertical_stripes')) {
+    if (
+      this.model.get('horizontal_stripes') ||
+      this.model.get('vertical_stripes')
+    ) {
       const index = this.model.get('horizontal_stripes')
         ? 'rowBackgroundColor'
         : 'columnBackgroundColor';
       grid_style[index] = (index: number): string => {
         return index % 2 === 0
           ? Theme.getBackgroundColor(1)
           : Theme.getBackgroundColor(2);
```

### Comparing `ipydatagrid-1.3.0/js/datasource.ts` & `ipydatagrid-1.3.1/js/datasource.ts`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.0/js/extension.ts` & `ipydatagrid-1.3.1/js/extension.ts`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.0/js/feathergrid.ts` & `ipydatagrid-1.3.1/js/feathergrid.ts`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.0/js/keyhandler.ts` & `ipydatagrid-1.3.1/js/keyhandler.ts`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.0/js/mousehandler.ts` & `ipydatagrid-1.3.1/js/mousehandler.ts`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.0/js/plugin.ts` & `ipydatagrid-1.3.1/js/plugin.ts`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.0/js/utils.ts` & `ipydatagrid-1.3.1/js/utils.ts`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.0/js/vegaexpr.ts` & `ipydatagrid-1.3.1/js/vegaexpr.ts`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.0/js/core/barrenderer.ts` & `ipydatagrid-1.3.1/js/core/barrenderer.ts`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.0/js/core/filterMenu.ts` & `ipydatagrid-1.3.1/js/core/filterMenu.ts`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.0/js/core/gridContextMenu.ts` & `ipydatagrid-1.3.1/js/core/gridContextMenu.ts`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import { DataGrid } from '@lumino/datagrid';
 
 import { DataModel } from '@lumino/datagrid';
 
 import { CommandRegistry } from '@lumino/commands';
 
-import { Menu } from '@lumino/widgets';
+import { Menu, Widget } from '@lumino/widgets';
 
 /**
  * An object which provides context menus for the data grid.
  *
  * #### Notes
  * This item creates one Menu widget, then changes it's items based on
  * the `cellClick` signal from `DataGrid`.
@@ -203,14 +203,23 @@
         break;
       default:
         throw 'unreachable';
     }
 
     // Open context menu at location of the click event
     this._menu.open(hit.x, hit.y);
+
+    // Issue 422: menu should be first child of document.body not last child to work on all of
+    // Jupyter Lab, Notebook < 7, NbClassic and Voila. Until this is available in lumino/widgets,
+    // detach and reattach the menu here.
+    const bodyFirstChild = document.body.firstElementChild;
+    if (this._menu.node.parentElement == document.body && bodyFirstChild != this._menu.node) {
+      Widget.detach(this._menu);
+      Widget.attach(this._menu, document.body, bodyFirstChild as HTMLElement);
+    }
   }
 }
 
 /**
  * The namespace for the `IPyDataGridContextMenu` class statics.
  */
 export namespace FeatherGridContextMenu {
```

### Comparing `ipydatagrid-1.3.0/js/core/headerRenderer.ts` & `ipydatagrid-1.3.1/js/core/headerRenderer.ts`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.0/js/core/htmlRenderer.ts` & `ipydatagrid-1.3.1/js/core/htmlRenderer.ts`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.0/js/core/transform.ts` & `ipydatagrid-1.3.1/js/core/transform.ts`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.0/js/core/transformExecutors.ts` & `ipydatagrid-1.3.1/js/core/transformExecutors.ts`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.0/js/core/transformStateManager.ts` & `ipydatagrid-1.3.1/js/core/transformStateManager.ts`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.0/js/core/valueRenderer.ts` & `ipydatagrid-1.3.1/js/core/valueRenderer.ts`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.0/js/core/view.ts` & `ipydatagrid-1.3.1/js/core/view.ts`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.0/js/core/viewbasedjsonmodel.ts` & `ipydatagrid-1.3.1/js/core/viewbasedjsonmodel.ts`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.0/static/ipydatagrid_1.gif` & `ipydatagrid-1.3.1/static/ipydatagrid_1.gif`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.0/static/ipydatagrid_2.gif` & `ipydatagrid-1.3.1/static/ipydatagrid_2.gif`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.0/static/ipydatagrid_3.gif` & `ipydatagrid-1.3.1/static/ipydatagrid_3.gif`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.0/static/ipydatagrid_4.gif` & `ipydatagrid-1.3.1/static/ipydatagrid_4.gif`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.0/static/ipydatagrid_5.gif` & `ipydatagrid-1.3.1/static/ipydatagrid_5.gif`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.0/style/feathergrid.css` & `ipydatagrid-1.3.1/style/feathergrid.css`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.0/.gitignore` & `ipydatagrid-1.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.0/LICENSE.txt` & `ipydatagrid-1.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.0/README.md` & `ipydatagrid-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.0/pyproject.toml` & `ipydatagrid-1.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 requires = [
   "hatchling>=1.18",
   "jupyterlab>=4.0.5",
 ]
 
 [project]
 name = "ipydatagrid"
-version = "1.3.0"
+version = "1.3.1"
 description = "Fast Datagrid widget for the Jupyter Notebook and JupyterLab"
 readme = "README.md"
 keywords = [
   "IPython",
   "Jupyter",
   "Widgets",
 ]
@@ -115,15 +115,15 @@
 [tool.tbump]
 field = [
     { name = "channel", default = "" },
     { name = "release", default = "" },
 ]
 
 [tool.tbump.version]
-current = "1.3.0"
+current = "1.3.1"
 regex = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)((?P<channel>a|b|rc|.dev)(?P<release>\\d+))?"
 
 [tool.tbump.git]
 message_template = "Bump to {new_version}"
 tag_template = "v{new_version}"
 
 [[tool.tbump.file]]
```

### Comparing `ipydatagrid-1.3.0/PKG-INFO` & `ipydatagrid-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ipydatagrid
-Version: 1.3.0
+Version: 1.3.1
 Summary: Fast Datagrid widget for the Jupyter Notebook and JupyterLab
 Project-URL: Homepage, https://github.com/bloomberg/ipydatagrid
 Author: Bloomberg
 License-File: LICENSE.txt
 Keywords: IPython,Jupyter,Widgets
 Classifier: Framework :: Jupyter
 Classifier: Intended Audience :: Developers
```

