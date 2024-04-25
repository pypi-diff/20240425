# Comparing `tmp/mat3ra_made-2024.4.25.post0.tar.gz` & `tmp/mat3ra-made-2024.4.8.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mat3ra_made-2024.4.25.post0.tar", last modified: Thu Apr 25 03:31:59 2024, max compression
+gzip compressed data, was "mat3ra-made-2024.4.8.post0.tar", last modified: Mon Apr  8 11:38:12 2024, max compression
```

## Comparing `mat3ra_made-2024.4.25.post0.tar` & `mat3ra-made-2024.4.8.post0.tar`

### file list

```diff
@@ -1,161 +1,154 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:31:59.593110 mat3ra_made-2024.4.25.post0/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/.babelrc
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/.eslintrc.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:31:59.569110 mat3ra_made-2024.4.25.post0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:31:59.577110 mat3ra_made-2024.4.25.post0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/.github/workflows/cicd.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:31:59.577110 mat3ra_made-2024.4.25.post0/.husky/
--rwxr-xr-x   0 runner    (1001) docker     (127)      351 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/.husky/post-checkout
--rwxr-xr-x   0 runner    (1001) docker     (127)      347 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/.husky/post-commit
--rwxr-xr-x   0 runner    (1001) docker     (127)      345 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/.husky/post-merge
--rwxr-xr-x   0 runner    (1001) docker     (127)       89 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/.husky/pre-commit
--rwxr-xr-x   0 runner    (1001) docker     (127)      341 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/.husky/pre-push
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/.mocharc.json
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/.prettierignore
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/.prettierrc
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    10278 2024-04-25 03:31:59.593110 mat3ra_made-2024.4.25.post0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   373142 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/package.json
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 03:31:59.593110 mat3ra_made-2024.4.25.post0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:31:59.569110 mat3ra_made-2024.4.25.post0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:31:59.577110 mat3ra_made-2024.4.25.post0/src/js/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:31:59.577110 mat3ra_made-2024.4.25.post0/src/js/abstract/
--rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/src/js/abstract/array_with_ids.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/src/js/abstract/scalar_with_id.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:31:59.577110 mat3ra_made-2024.4.25.post0/src/js/basis/
--rw-r--r--   0 runner    (1001) docker     (127)    21777 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/src/js/basis/basis.ts
--rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/src/js/basis/constrained_basis.ts
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/src/js/basis/types.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:31:59.577110 mat3ra_made-2024.4.25.post0/src/js/cell/
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/src/js/cell/cell.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/src/js/cell/conventional_cell.ts
--rw-r--r--   0 runner    (1001) docker     (127)     6064 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/src/js/cell/primitive_cell.ts
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/src/js/constants.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:31:59.577110 mat3ra_made-2024.4.25.post0/src/js/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/src/js/constraints/constraints.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:31:59.577110 mat3ra_made-2024.4.25.post0/src/js/lattice/
--rw-r--r--   0 runner    (1001) docker     (127)     7334 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/src/js/lattice/lattice.ts
--rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/src/js/lattice/lattice_bravais.ts
--rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/src/js/lattice/lattice_vectors.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:31:59.581110 mat3ra_made-2024.4.25.post0/src/js/lattice/reciprocal/
--rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/src/js/lattice/reciprocal/lattice_reciprocal.js
--rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/src/js/lattice/reciprocal/paths.js
--rw-r--r--   0 runner    (1001) docker     (127)    24706 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/src/js/lattice/reciprocal/symmetry_points.ts
--rw-r--r--   0 runner    (1001) docker     (127)     3515 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/src/js/lattice/types.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/src/js/lattice/unit_cell.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/src/js/made.js
--rw-r--r--   0 runner    (1001) docker     (127)    13731 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/src/js/material.ts
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/src/js/math.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:31:59.581110 mat3ra_made-2024.4.25.post0/src/js/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/src/js/parsers/cif.js
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/src/js/parsers/errors.js
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/src/js/parsers/espresso.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/src/js/parsers/native_format_parsers.js
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/src/js/parsers/parsers.js
--rw-r--r--   0 runner    (1001) docker     (127)     7160 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/src/js/parsers/poscar.ts
--rw-r--r--   0 runner    (1001) docker     (127)     6505 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/src/js/parsers/xyz.ts
--rw-r--r--   0 runner    (1001) docker     (127)     7540 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/src/js/parsers/xyz_combinatorial_basis.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:31:59.581110 mat3ra_made-2024.4.25.post0/src/js/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/src/js/tools/basis.js
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/src/js/tools/cell.js
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/src/js/tools/index.js
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/src/js/tools/material.js
--rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/src/js/tools/supercell.ts
--rw-r--r--   0 runner    (1001) docker     (127)     6274 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/src/js/tools/surface.js
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/src/js/types.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:31:59.581110 mat3ra_made-2024.4.25.post0/src/py/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/src/py/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:31:59.581110 mat3ra_made-2024.4.25.post0/src/py/mat3ra/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/src/py/mat3ra/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:31:59.581110 mat3ra_made-2024.4.25.post0/src/py/mat3ra/made/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/src/py/mat3ra/made/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/src/py/mat3ra/made/material.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:31:59.585110 mat3ra_made-2024.4.25.post0/src/py/mat3ra/made/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/src/py/mat3ra/made/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/src/py/mat3ra/made/tools/analyze.py
--rw-r--r--   0 runner    (1001) docker     (127)     4791 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/src/py/mat3ra/made/tools/calculate.py
--rw-r--r--   0 runner    (1001) docker     (127)     6435 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/src/py/mat3ra/made/tools/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/src/py/mat3ra/made/tools/modify.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/src/py/mat3ra/made/tools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:31:59.593110 mat3ra_made-2024.4.25.post0/src/py/mat3ra_made.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10278 2024-04-25 03:31:59.000000 mat3ra_made-2024.4.25.post0/src/py/mat3ra_made.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-04-25 03:31:59.000000 mat3ra_made-2024.4.25.post0/src/py/mat3ra_made.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 03:31:59.000000 mat3ra_made-2024.4.25.post0/src/py/mat3ra_made.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-25 03:31:59.000000 mat3ra_made-2024.4.25.post0/src/py/mat3ra_made.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-25 03:31:59.000000 mat3ra_made-2024.4.25.post0/src/py/mat3ra_made.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:31:59.585110 mat3ra_made-2024.4.25.post0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/tests/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:31:59.589110 mat3ra_made-2024.4.25.post0/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/tests/fixtures/AsGe-basis.json
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/tests/fixtures/C2H4-translated.json
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/tests/fixtures/C2H4.json
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/tests/fixtures/FeLiSi-basis.json
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/tests/fixtures/FeO.json
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/tests/fixtures/Ge2-basis.json
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/tests/fixtures/Graphene.json
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/tests/fixtures/Graphene.poscar
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/tests/fixtures/H2+H-final.json
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/tests/fixtures/H2+H-image.json
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/tests/fixtures/H2+H-initial.json
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/tests/fixtures/H2O.poscar
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/tests/fixtures/LiFeSi-basis.json
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/tests/fixtures/Na.json
--rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/tests/fixtures/Na4Cl4-cartesian.json
--rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/tests/fixtures/Na4Cl4.json
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/tests/fixtures/Na4Cl4.poscar
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/tests/fixtures/Ni-hex.json
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/tests/fixtures/Ni-hex.poscar
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/tests/fixtures/OSi-basis.json
--rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/tests/fixtures/Si-hex.json
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/tests/fixtures/Si-hex.poscar
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/tests/fixtures/Si-pwscf.in
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/tests/fixtures/Si-slab.json
--rw-r--r--   0 runner    (1001) docker     (127)     3244 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/tests/fixtures/Si-supercell.json
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/tests/fixtures/Si.json
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/tests/fixtures/Si2-basis-repeated.json
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/tests/fixtures/Si2-basis.json
--rw-r--r--   0 runner    (1001) docker     (127)    11190 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/tests/fixtures/Zr1H23Zr1H1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/tests/fixtures/Zr1H23Zr1H1.poscar
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/tests/fixtures/atomic-constraints.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:31:59.589110 mat3ra_made-2024.4.25.post0/tests/js/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:31:59.589110 mat3ra_made-2024.4.25.post0/tests/js/basis/
--rw-r--r--   0 runner    (1001) docker     (127)     6941 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/tests/js/basis/basis.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:31:59.589110 mat3ra_made-2024.4.25.post0/tests/js/cell/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/tests/js/cell/cell.js
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/tests/js/cell/primitive_cell.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:31:59.589110 mat3ra_made-2024.4.25.post0/tests/js/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/tests/js/constraints/constraints.js
--rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/tests/js/enums.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:31:59.589110 mat3ra_made-2024.4.25.post0/tests/js/lattice/
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/tests/js/lattice/lattice.js
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/tests/js/lattice/lattice_bravais.js
--rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/tests/js/lattice/lattice_reciprocal.js
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/tests/js/lattice/lattice_vectors.js
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/tests/js/material.test.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:31:59.589110 mat3ra_made-2024.4.25.post0/tests/js/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/tests/js/parsers/espresso.js
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/tests/js/parsers/native_formats.js
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/tests/js/parsers/poscar.js
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/tests/js/parsers/xyz.js
--rw-r--r--   0 runner    (1001) docker     (127)     5006 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/tests/js/parsers/xyz_combinatorial_basis.js
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/tests/js/setup.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:31:59.593110 mat3ra_made-2024.4.25.post0/tests/js/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/tests/js/tools/basis.js
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/tests/js/tools/supercell.js
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/tests/js/tools/surface.js
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/tests/js/utils.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:31:59.573110 mat3ra_made-2024.4.25.post0/tests/py/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:31:59.593110 mat3ra_made-2024.4.25.post0/tests/py/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/tests/py/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/tests/py/unit/test_material.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/tests/py/unit/test_tools_analyze.py
--rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/tests/py/unit/test_tools_calculate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/tests/py/unit/test_tools_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/tests/py/unit/test_tools_modify.py
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/tsconfig-transpile.json
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-25 03:31:43.000000 mat3ra_made-2024.4.25.post0/tsconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:38:12.534860 mat3ra-made-2024.4.8.post0/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/.babelrc
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/.eslintrc.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:38:12.506861 mat3ra-made-2024.4.8.post0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:38:12.514860 mat3ra-made-2024.4.8.post0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/.github/workflows/cicd.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:38:12.514860 mat3ra-made-2024.4.8.post0/.husky/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      351 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/.husky/post-checkout
+-rwxr-xr-x   0 runner    (1001) docker     (127)      347 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/.husky/post-commit
+-rwxr-xr-x   0 runner    (1001) docker     (127)      345 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/.husky/post-merge
+-rwxr-xr-x   0 runner    (1001) docker     (127)       89 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/.husky/pre-commit
+-rwxr-xr-x   0 runner    (1001) docker     (127)      341 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/.husky/pre-push
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/.mocharc.json
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/.prettierignore
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/.prettierrc
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9905 2024-04-08 11:38:12.534860 mat3ra-made-2024.4.8.post0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7950 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   373142 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 11:38:12.534860 mat3ra-made-2024.4.8.post0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:38:12.506861 mat3ra-made-2024.4.8.post0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:38:12.514860 mat3ra-made-2024.4.8.post0/src/js/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:38:12.514860 mat3ra-made-2024.4.8.post0/src/js/abstract/
+-rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/src/js/abstract/array_with_ids.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/src/js/abstract/scalar_with_id.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:38:12.514860 mat3ra-made-2024.4.8.post0/src/js/basis/
+-rw-r--r--   0 runner    (1001) docker     (127)    21777 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/src/js/basis/basis.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/src/js/basis/constrained_basis.ts
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/src/js/basis/types.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:38:12.518860 mat3ra-made-2024.4.8.post0/src/js/cell/
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/src/js/cell/cell.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/src/js/cell/conventional_cell.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     6064 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/src/js/cell/primitive_cell.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/src/js/constants.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:38:12.518860 mat3ra-made-2024.4.8.post0/src/js/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/src/js/constraints/constraints.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:38:12.518860 mat3ra-made-2024.4.8.post0/src/js/lattice/
+-rw-r--r--   0 runner    (1001) docker     (127)     7334 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/src/js/lattice/lattice.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/src/js/lattice/lattice_bravais.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/src/js/lattice/lattice_vectors.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:38:12.518860 mat3ra-made-2024.4.8.post0/src/js/lattice/reciprocal/
+-rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/src/js/lattice/reciprocal/lattice_reciprocal.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/src/js/lattice/reciprocal/paths.js
+-rw-r--r--   0 runner    (1001) docker     (127)    24706 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/src/js/lattice/reciprocal/symmetry_points.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     3515 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/src/js/lattice/types.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/src/js/lattice/unit_cell.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/src/js/made.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13731 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/src/js/material.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/src/js/math.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:38:12.518860 mat3ra-made-2024.4.8.post0/src/js/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/src/js/parsers/cif.js
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/src/js/parsers/errors.js
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/src/js/parsers/espresso.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/src/js/parsers/native_format_parsers.js
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/src/js/parsers/parsers.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7160 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/src/js/parsers/poscar.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     6505 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/src/js/parsers/xyz.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     7540 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/src/js/parsers/xyz_combinatorial_basis.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:38:12.522861 mat3ra-made-2024.4.8.post0/src/js/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/src/js/tools/basis.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/src/js/tools/cell.js
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/src/js/tools/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/src/js/tools/material.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/src/js/tools/supercell.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     6274 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/src/js/tools/surface.js
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/src/js/types.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:38:12.522861 mat3ra-made-2024.4.8.post0/src/py/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/src/py/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:38:12.522861 mat3ra-made-2024.4.8.post0/src/py/mat3ra/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/src/py/mat3ra/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:38:12.522861 mat3ra-made-2024.4.8.post0/src/py/mat3ra/made/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/src/py/mat3ra/made/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/src/py/mat3ra/made/material.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:38:12.522861 mat3ra-made-2024.4.8.post0/src/py/mat3ra/made/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/src/py/mat3ra/made/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/src/py/mat3ra/made/tools/material.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:38:12.534860 mat3ra-made-2024.4.8.post0/src/py/mat3ra_made.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9905 2024-04-08 11:38:12.000000 mat3ra-made-2024.4.8.post0/src/py/mat3ra_made.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3326 2024-04-08 11:38:12.000000 mat3ra-made-2024.4.8.post0/src/py/mat3ra_made.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 11:38:12.000000 mat3ra-made-2024.4.8.post0/src/py/mat3ra_made.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-08 11:38:12.000000 mat3ra-made-2024.4.8.post0/src/py/mat3ra_made.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-08 11:38:12.000000 mat3ra-made-2024.4.8.post0/src/py/mat3ra_made.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:38:12.522861 mat3ra-made-2024.4.8.post0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/tests/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:38:12.530861 mat3ra-made-2024.4.8.post0/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/tests/fixtures/AsGe-basis.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/tests/fixtures/C2H4-translated.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/tests/fixtures/C2H4.json
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/tests/fixtures/FeLiSi-basis.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/tests/fixtures/FeO.json
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/tests/fixtures/Ge2-basis.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/tests/fixtures/Graphene.json
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/tests/fixtures/Graphene.poscar
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/tests/fixtures/H2+H-final.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/tests/fixtures/H2+H-image.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/tests/fixtures/H2+H-initial.json
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/tests/fixtures/H2O.poscar
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/tests/fixtures/LiFeSi-basis.json
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/tests/fixtures/Na.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/tests/fixtures/Na4Cl4-cartesian.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/tests/fixtures/Na4Cl4.json
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/tests/fixtures/Na4Cl4.poscar
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/tests/fixtures/Ni-hex.json
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/tests/fixtures/Ni-hex.poscar
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/tests/fixtures/OSi-basis.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/tests/fixtures/Si-hex.json
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/tests/fixtures/Si-hex.poscar
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/tests/fixtures/Si-pwscf.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/tests/fixtures/Si-slab.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3244 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/tests/fixtures/Si-supercell.json
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/tests/fixtures/Si.json
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/tests/fixtures/Si2-basis-repeated.json
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/tests/fixtures/Si2-basis.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11190 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/tests/fixtures/Zr1H23Zr1H1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/tests/fixtures/Zr1H23Zr1H1.poscar
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/tests/fixtures/atomic-constraints.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:38:12.530861 mat3ra-made-2024.4.8.post0/tests/js/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:38:12.530861 mat3ra-made-2024.4.8.post0/tests/js/basis/
+-rw-r--r--   0 runner    (1001) docker     (127)     6941 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/tests/js/basis/basis.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:38:12.530861 mat3ra-made-2024.4.8.post0/tests/js/cell/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/tests/js/cell/cell.js
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/tests/js/cell/primitive_cell.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:38:12.530861 mat3ra-made-2024.4.8.post0/tests/js/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/tests/js/constraints/constraints.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/tests/js/enums.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:38:12.530861 mat3ra-made-2024.4.8.post0/tests/js/lattice/
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/tests/js/lattice/lattice.js
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/tests/js/lattice/lattice_bravais.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/tests/js/lattice/lattice_reciprocal.js
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/tests/js/lattice/lattice_vectors.js
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/tests/js/material.test.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:38:12.530861 mat3ra-made-2024.4.8.post0/tests/js/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/tests/js/parsers/espresso.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/tests/js/parsers/native_formats.js
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/tests/js/parsers/poscar.js
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/tests/js/parsers/xyz.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5006 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/tests/js/parsers/xyz_combinatorial_basis.js
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/tests/js/setup.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:38:12.530861 mat3ra-made-2024.4.8.post0/tests/js/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/tests/js/tools/basis.js
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/tests/js/tools/supercell.js
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/tests/js/tools/surface.js
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/tests/js/utils.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:38:12.510861 mat3ra-made-2024.4.8.post0/tests/py/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:38:12.534860 mat3ra-made-2024.4.8.post0/tests/py/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/tests/py/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/tests/py/unit/test_material.py
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/tests/py/unit/test_tools_material.py
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/tsconfig-transpile.json
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-08 11:37:56.000000 mat3ra-made-2024.4.8.post0/tsconfig.json
```

### Comparing `mat3ra_made-2024.4.25.post0/.github/workflows/cicd.yml` & `mat3ra-made-2024.4.8.post0/.github/workflows/cicd.yml`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.4.25.post0/.gitignore` & `mat3ra-made-2024.4.8.post0/.gitignore`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.4.25.post0/.pre-commit-config.yaml` & `mat3ra-made-2024.4.8.post0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.4.25.post0/LICENSE.md` & `mat3ra-made-2024.4.8.post0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.4.25.post0/PKG-INFO` & `mat3ra-made-2024.4.8.post0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mat3ra-made
-Version: 2024.4.25.post0
+Version: 2024.4.8.post0
 Summary: MAterials DEfinitions and/or MAterials DEsign library.
 Author-email: "Exabyte Inc." <info@mat3ra.com>
 License: # LICENSE
         
         Copyright 2019 Exabyte Inc.
         
         Licensed under the Apache License, Version 2.0 (the "License");
@@ -23,78 +23,53 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Software Development
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: numpy
+Requires-Dist: pymatgen
+Requires-Dist: ase
 Requires-Dist: mat3ra-esse
 Requires-Dist: mat3ra-code
-Provides-Extra: tools
-Requires-Dist: pymatgen; extra == "tools"
-Requires-Dist: ase; extra == "tools"
-Provides-Extra: dev
-Requires-Dist: pre-commit; extra == "dev"
-Requires-Dist: black; extra == "dev"
-Requires-Dist: ruff; extra == "dev"
-Requires-Dist: isort; extra == "dev"
-Requires-Dist: mypy; extra == "dev"
-Requires-Dist: pip-tools; extra == "dev"
 Provides-Extra: tests
 Requires-Dist: coverage[toml]>=5.3; extra == "tests"
+Requires-Dist: pre-commit; extra == "tests"
+Requires-Dist: black; extra == "tests"
+Requires-Dist: ruff; extra == "tests"
+Requires-Dist: isort; extra == "tests"
+Requires-Dist: mypy; extra == "tests"
+Requires-Dist: pip-tools; extra == "tests"
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: pytest-cov; extra == "tests"
-Requires-Dist: gradio; extra == "tests"
 Requires-Dist: pydantic; extra == "tests"
-Requires-Dist: mat3ra-made[tools]; extra == "tests"
+Requires-Dist: gradio; extra == "tests"
+Provides-Extra: tools
+Requires-Dist: pymatgen; extra == "tools"
+Requires-Dist: ase; extra == "tools"
 Provides-Extra: all
 Requires-Dist: mat3ra-made[tests]; extra == "all"
-Requires-Dist: mat3ra-made[dev]; extra == "all"
+Requires-Dist: mat3ra-made[tools]; extra == "all"
 
 [![npm version](https://badge.fury.io/js/%40mat3ra%2Fmade.svg)](https://badge.fury.io/js/%40mat3ra%2Fmade)
 [![License: Apache](https://img.shields.io/badge/License-Apache-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0)
 
 # Made
 
 Made is a library for **MA**terials **DE**sign in JavaScript/TypeScript and Python. It allows for the creation and manipulation of material structures from atoms up on the web. The library is aimed to be used for the development of web applications, both on the client (web browser) and server (eg. Node.js) side.
 
-## 1. Overview
-
-The package provides a software environment for interacting with Materials-related data structures from ESSE Data Convention [[1]](#links) for use on the web.
-
-## 2. Installation
-
-### 2.1. JavaScript/TypeScript
-
-From NPM for use within a software project:
-
-```bash
-npm install @mat3ra/made
-
-```
-
-### 2.2. Python
+The library was originally designed as part of and presently powers materials design capabilities of the [Exabyte.io](https://exabyte.io) platform. For example, [this page](https://platform.exabyte.io/demo/materials/n3HSzCmyoctgJFGGE) representing a crystal of Silicon online uses Made.js.
 
-From PyPI for use within a software project:
+Exabyte.io believe in a collaborative future of materials design on the web.
 
-```bash
-pip install mat3ra-made
-```
+## Functionality
 
-When willing to use the optional `tools` module, install the package with the following command:
-
-```bash
-pip install "mat3ra-made[tools]"
-```
-
-
-## 3. Functionality
-
-As below
+As below:
 
+- the package provides a software environment for interacting with Materials-related data structures from ESSE Data Convention [[1]](#links) and is written in ECMAScript 2015 for use on the web
 - High-level classes for the representation of the [Material](src/material.js) and the corresponding structural information, ie:
     - [Basis](src/basis/basis.js),
     - [Lattice](src/lattice/lattice.js),
     - [ReciprocalLattice](src/lattice/reciprocal/lattice_reciprocal.js),
     - [Cell](src/cell/cell.js),
     - [AtomicConstraints](src/constraints/constraints.js)
     - and others to be added.
@@ -105,82 +80,98 @@
     - and others to be added.
 - structural generation and analysis tools:
     - [supercell](src/tools/supercell.js)
     - [surfaces](src/tools/surface.js)
     - [combinatorial sets](src/parsers/xyz_combinatorial_basis.js)
     - [interpolated sets for chemical reactions](src/tools/basis.js)
 
+The package is written in a modular way easy to extend. Contributions can be in the form of additional tools or modules you develop, or feature requests and [bug/issue reports](https://help.github.com/articles/creating-an-issue/).
+
+## Installation
+
+From NPM for use within a software project:
+
+```bash
+npm install @mat3ra/made
 
-## 4. Contribution
+```
+
+From source to contribute to development:
+
+```bash
+git clone git@github.com:Exabyte-io/made
+```
+
+## Contribution
 
 This repository is an [open-source](LICENSE.md) work-in-progress and we welcome contributions.
 
+### Why contribute?
+
 We regularly deploy the latest code containing all accepted contributions online as part of the [Mat3ra.com](https://mat3ra.com) platform, so contributors will see their code in action there.
 
+### Adding new functionality
+
 We suggest forking this repository and introducing the adjustments there to be considered for merging into this repository as explained in more details [here](https://gist.github.com/Chaser324/ce0505fbed06b947d962), for example.
 
-### 4.1. Source code conventions
+### Source code conventions
 
-Object-oriented design patterns encapsulate key concepts following the conventions below.
+Made.js is written in EcmaScript 6th edition [[2]](#links) with the application of object-oriented design patterns encapsulating key concepts following the conventions below.
 
 1. Classes follow the Exabyte Data Convention and data structures defined in ESSE [[1]](#links)
 
 2. Only materials-related code is considered. Properties related to [simulation model](https://docs.exabyte.io/models/overview/) parameters (eg. type of approximation, numerical parameters) shall go elsewhere.
 
 3. `tools` directory contains helper functions that act on one or more classes and include an external parameter. Functions that use class data without any external parameters should be implemented inside the class. For example, `basis.clone()` is implemented in `Basis`, but basis repetition is implemented as a tool in the correspondingly named function ([tools/basis.js#repeat](src/tools/basis.js)) because the repetion requires a parameter external to basis - number of repetitions in 3 spatial dimensions.
 
-4. [Deprecated, use mat3ra-parsers or @mat3ra/parsers] `parsers` directory contains the parsers to- and from- ESSE format mentioned in 1. All functionality related to external data conversion is contained in this directory.
+4. `parsers` directory contains the parsers to- and from- ESSE format mentioned in 1. All functionality related to external data conversion is contained in this directory.
 
 
-### 4.2. TODO list
+### TODO list
 
-[Outdated] Desirable features for implementation:
+Desirable features for implementation:
 
 - identify primitive / conventional structures
 - support for molecular geometries
 - support for polymer geometries
 - radial correlation function calculation
 - generation of complex atomic shapes:
     - fullerene
     - nanotube
     - nanowire
     - nano-cluster
     - a combination of the above
     - arbitrary atomic arrangement
 
-## 5. Development
-
-### 5.1. JavaScript/TypeScript
-
-#### 5.1.1. Tests
+## Tests
 
 Made tests are written based on Mocha [6](#links) testing framework and can be executed as follows.
 
 ```bash
 git pull
 git lfs pull
 ```
 to get the latest test fixtures from LFS, and then:
 
 ```bash
 npm install
 npm test
 ```
 
-#### 5.1.2. Important Notes
+### Tests Important Notes
 
 1. Keep the tests directory structure similar to the main codebase directory structure. Every JS module in the main codebase should have a corresponding module in tests directory which implements the tests for provided functionality.
 
 2. Add tests fixtures into [fixtures](./tests/fixtures) directory. The fixtures are automatically stored on Git LFS [7](#links).
 
 3. If the fixtures are going to be used inside multiple cases, read and export them inside [enums](./tests/enums.js) to avoid code duplicates.
 
 4. [Tests setup module](./tests/setup.js) can be used to implement the hooks that are used to prepare the tests environment.
 
-#### 5.1.3. Using Linter
+## Using Linter
 
 Linter setup will prevent committing files that don't adhere to the code standard. It will
 attempt to fix what it can automatically prior to the commit in order to reduce diff noise. This can lead to "unexpected" behavior where a
 file that is staged for commit is not identical to the file that actually gets committed. This happens
 in the `lint-staged` directive of the `package.json` file (by using a `husky` pre-commit hook). For example,
 if you add extra whitespace to a file, stage it, and try to commit it, you will see the following:
 
@@ -206,52 +197,21 @@
 ```bash
 npm run lint:fix
 ```
 
 In which case, you may need to then add the linter edits to your staging, which in the example above, puts the
 file back to identical with the base branch, resulting in no staged changes whatsoever.
 
-#### 5.1.4. Configuring WebStorm for use with Linter
+## Configuring WebStorm for use with Linter
 
 In order for the WebStorm IDE to take full advantage of the linting configuration, it can be configured in the project:
 
 - `Preferences -> Languages & Frameworks -> JavaScript -> Code Quality Tools -> ESLint`
 - Check `Automatic ESLint configuration` which should infer all the configurations from the project directory
 
-### 5.2. Python
-
-#### 5.2.1. Tests
-
-Python 3.8+ is required to run the tests. We recommend using PyEnv to manage Python versions. Tests are written based on PyTest and can be executed as follows.
-
-```bash
-virtualenv .venv
-source .venv/bin/activate
-pip install ".[tests]"
-pytest tests/py
-```
-
-#### 5.2.2. Important Notes
-
-Conventions:
-
-- The "tools" module has external dependencies on "pymatgen" and "ase" packages and so is meant as optional. When implementing new functionality, the use of ASE is recommended over pymatgen for compatibility purposes.
-
-### 5.3. Known Issues
-
-#### 5.3.1. JavaScript/TypeScript
-
-To be added.
-
-#### 5.3.2. Python
-
-As below:
-
-- Python 3.8 tests are failing on Apple Silicon due to https://github.com/materialsproject/pymatgen/issues/3521
-
 ## Links
 
 1. [Exabyte Source of Schemas and Examples (ESSE), Github Repository](https://github.com/exabyte-io/exabyte-esse)
 2. [ECMAScript 2015 Language Specifications](https://www.ecma-international.org/ecma-262/6.0/)
 3. [POSCAR file format, official website](https://cms.mpi.univie.ac.at/vasp/guide/node59.html)
 4. [XYZ file format, Wikipedia](https://en.wikipedia.org/wiki/XYZ_file_format)
 5. [Quantum ESPRESSO, Official Website](https://www.quantum-espresso.org/)
```

### Comparing `mat3ra_made-2024.4.25.post0/README.md` & `mat3ra-made-2024.4.8.post0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,48 +1,23 @@
 [![npm version](https://badge.fury.io/js/%40mat3ra%2Fmade.svg)](https://badge.fury.io/js/%40mat3ra%2Fmade)
 [![License: Apache](https://img.shields.io/badge/License-Apache-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0)
 
 # Made
 
 Made is a library for **MA**terials **DE**sign in JavaScript/TypeScript and Python. It allows for the creation and manipulation of material structures from atoms up on the web. The library is aimed to be used for the development of web applications, both on the client (web browser) and server (eg. Node.js) side.
 
-## 1. Overview
+The library was originally designed as part of and presently powers materials design capabilities of the [Exabyte.io](https://exabyte.io) platform. For example, [this page](https://platform.exabyte.io/demo/materials/n3HSzCmyoctgJFGGE) representing a crystal of Silicon online uses Made.js.
 
-The package provides a software environment for interacting with Materials-related data structures from ESSE Data Convention [[1]](#links) for use on the web.
+Exabyte.io believe in a collaborative future of materials design on the web.
 
-## 2. Installation
+## Functionality
 
-### 2.1. JavaScript/TypeScript
-
-From NPM for use within a software project:
-
-```bash
-npm install @mat3ra/made
-
-```
-
-### 2.2. Python
-
-From PyPI for use within a software project:
-
-```bash
-pip install mat3ra-made
-```
-
-When willing to use the optional `tools` module, install the package with the following command:
-
-```bash
-pip install "mat3ra-made[tools]"
-```
-
-
-## 3. Functionality
-
-As below
+As below:
 
+- the package provides a software environment for interacting with Materials-related data structures from ESSE Data Convention [[1]](#links) and is written in ECMAScript 2015 for use on the web
 - High-level classes for the representation of the [Material](src/material.js) and the corresponding structural information, ie:
     - [Basis](src/basis/basis.js),
     - [Lattice](src/lattice/lattice.js),
     - [ReciprocalLattice](src/lattice/reciprocal/lattice_reciprocal.js),
     - [Cell](src/cell/cell.js),
     - [AtomicConstraints](src/constraints/constraints.js)
     - and others to be added.
@@ -53,82 +28,98 @@
     - and others to be added.
 - structural generation and analysis tools:
     - [supercell](src/tools/supercell.js)
     - [surfaces](src/tools/surface.js)
     - [combinatorial sets](src/parsers/xyz_combinatorial_basis.js)
     - [interpolated sets for chemical reactions](src/tools/basis.js)
 
+The package is written in a modular way easy to extend. Contributions can be in the form of additional tools or modules you develop, or feature requests and [bug/issue reports](https://help.github.com/articles/creating-an-issue/).
+
+## Installation
+
+From NPM for use within a software project:
+
+```bash
+npm install @mat3ra/made
+
+```
 
-## 4. Contribution
+From source to contribute to development:
+
+```bash
+git clone git@github.com:Exabyte-io/made
+```
+
+## Contribution
 
 This repository is an [open-source](LICENSE.md) work-in-progress and we welcome contributions.
 
+### Why contribute?
+
 We regularly deploy the latest code containing all accepted contributions online as part of the [Mat3ra.com](https://mat3ra.com) platform, so contributors will see their code in action there.
 
+### Adding new functionality
+
 We suggest forking this repository and introducing the adjustments there to be considered for merging into this repository as explained in more details [here](https://gist.github.com/Chaser324/ce0505fbed06b947d962), for example.
 
-### 4.1. Source code conventions
+### Source code conventions
 
-Object-oriented design patterns encapsulate key concepts following the conventions below.
+Made.js is written in EcmaScript 6th edition [[2]](#links) with the application of object-oriented design patterns encapsulating key concepts following the conventions below.
 
 1. Classes follow the Exabyte Data Convention and data structures defined in ESSE [[1]](#links)
 
 2. Only materials-related code is considered. Properties related to [simulation model](https://docs.exabyte.io/models/overview/) parameters (eg. type of approximation, numerical parameters) shall go elsewhere.
 
 3. `tools` directory contains helper functions that act on one or more classes and include an external parameter. Functions that use class data without any external parameters should be implemented inside the class. For example, `basis.clone()` is implemented in `Basis`, but basis repetition is implemented as a tool in the correspondingly named function ([tools/basis.js#repeat](src/tools/basis.js)) because the repetion requires a parameter external to basis - number of repetitions in 3 spatial dimensions.
 
-4. [Deprecated, use mat3ra-parsers or @mat3ra/parsers] `parsers` directory contains the parsers to- and from- ESSE format mentioned in 1. All functionality related to external data conversion is contained in this directory.
+4. `parsers` directory contains the parsers to- and from- ESSE format mentioned in 1. All functionality related to external data conversion is contained in this directory.
 
 
-### 4.2. TODO list
+### TODO list
 
-[Outdated] Desirable features for implementation:
+Desirable features for implementation:
 
 - identify primitive / conventional structures
 - support for molecular geometries
 - support for polymer geometries
 - radial correlation function calculation
 - generation of complex atomic shapes:
     - fullerene
     - nanotube
     - nanowire
     - nano-cluster
     - a combination of the above
     - arbitrary atomic arrangement
 
-## 5. Development
-
-### 5.1. JavaScript/TypeScript
-
-#### 5.1.1. Tests
+## Tests
 
 Made tests are written based on Mocha [6](#links) testing framework and can be executed as follows.
 
 ```bash
 git pull
 git lfs pull
 ```
 to get the latest test fixtures from LFS, and then:
 
 ```bash
 npm install
 npm test
 ```
 
-#### 5.1.2. Important Notes
+### Tests Important Notes
 
 1. Keep the tests directory structure similar to the main codebase directory structure. Every JS module in the main codebase should have a corresponding module in tests directory which implements the tests for provided functionality.
 
 2. Add tests fixtures into [fixtures](./tests/fixtures) directory. The fixtures are automatically stored on Git LFS [7](#links).
 
 3. If the fixtures are going to be used inside multiple cases, read and export them inside [enums](./tests/enums.js) to avoid code duplicates.
 
 4. [Tests setup module](./tests/setup.js) can be used to implement the hooks that are used to prepare the tests environment.
 
-#### 5.1.3. Using Linter
+## Using Linter
 
 Linter setup will prevent committing files that don't adhere to the code standard. It will
 attempt to fix what it can automatically prior to the commit in order to reduce diff noise. This can lead to "unexpected" behavior where a
 file that is staged for commit is not identical to the file that actually gets committed. This happens
 in the `lint-staged` directive of the `package.json` file (by using a `husky` pre-commit hook). For example,
 if you add extra whitespace to a file, stage it, and try to commit it, you will see the following:
 
@@ -154,52 +145,21 @@
 ```bash
 npm run lint:fix
 ```
 
 In which case, you may need to then add the linter edits to your staging, which in the example above, puts the
 file back to identical with the base branch, resulting in no staged changes whatsoever.
 
-#### 5.1.4. Configuring WebStorm for use with Linter
+## Configuring WebStorm for use with Linter
 
 In order for the WebStorm IDE to take full advantage of the linting configuration, it can be configured in the project:
 
 - `Preferences -> Languages & Frameworks -> JavaScript -> Code Quality Tools -> ESLint`
 - Check `Automatic ESLint configuration` which should infer all the configurations from the project directory
 
-### 5.2. Python
-
-#### 5.2.1. Tests
-
-Python 3.8+ is required to run the tests. We recommend using PyEnv to manage Python versions. Tests are written based on PyTest and can be executed as follows.
-
-```bash
-virtualenv .venv
-source .venv/bin/activate
-pip install ".[tests]"
-pytest tests/py
-```
-
-#### 5.2.2. Important Notes
-
-Conventions:
-
-- The "tools" module has external dependencies on "pymatgen" and "ase" packages and so is meant as optional. When implementing new functionality, the use of ASE is recommended over pymatgen for compatibility purposes.
-
-### 5.3. Known Issues
-
-#### 5.3.1. JavaScript/TypeScript
-
-To be added.
-
-#### 5.3.2. Python
-
-As below:
-
-- Python 3.8 tests are failing on Apple Silicon due to https://github.com/materialsproject/pymatgen/issues/3521
-
 ## Links
 
 1. [Exabyte Source of Schemas and Examples (ESSE), Github Repository](https://github.com/exabyte-io/exabyte-esse)
 2. [ECMAScript 2015 Language Specifications](https://www.ecma-international.org/ecma-262/6.0/)
 3. [POSCAR file format, official website](https://cms.mpi.univie.ac.at/vasp/guide/node59.html)
 4. [XYZ file format, Wikipedia](https://en.wikipedia.org/wiki/XYZ_file_format)
 5. [Quantum ESPRESSO, Official Website](https://www.quantum-espresso.org/)
```

### Comparing `mat3ra_made-2024.4.25.post0/package-lock.json` & `mat3ra-made-2024.4.8.post0/package-lock.json`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.4.25.post0/package.json` & `mat3ra-made-2024.4.8.post0/package.json`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.4.25.post0/pyproject.toml` & `mat3ra-made-2024.4.8.post0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -13,44 +13,42 @@
     "Programming Language :: Python :: 3",
     "Development Status :: 3 - Alpha",
     "Topic :: Software Development",
 ]
 dependencies = [
     # add requirements here
     "numpy",
+    "pymatgen",
+    "ase",
     "mat3ra-esse",
     "mat3ra-code",
 ]
 
 [project.optional-dependencies]
-# tracking separately the deps required to use the tools module
-tools = [
-    "pymatgen",
-    "ase",
-]
-dev = [
+tests = [
+    "coverage[toml]>=5.3",
     "pre-commit",
     "black",
     "ruff",
     "isort",
     "mypy",
     "pip-tools",
-]
-tests = [
-    "coverage[toml]>=5.3",
     "pytest",
     "pytest-cov",
-    # B/c of https://github.com/binary-husky/gpt_academic/issues/1237
-    "gradio",
     "pydantic",
-    "mat3ra-made[tools]",
+    "gradio",
+]
+# required to use the tools module
+tools = [
+    "pymatgen",
+    "ase",
 ]
 all = [
     "mat3ra-made[tests]",
-    "mat3ra-made[dev]",
+    "mat3ra-made[tools]",
 ]
 
 # Entrypoint scripts can be defined here, see examples below.
 [project.scripts]
 # my-script = "my_package.my_module:my_function"
```

### Comparing `mat3ra_made-2024.4.25.post0/src/js/abstract/array_with_ids.ts` & `mat3ra-made-2024.4.8.post0/src/js/abstract/array_with_ids.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.4.25.post0/src/js/abstract/scalar_with_id.ts` & `mat3ra-made-2024.4.8.post0/src/js/abstract/scalar_with_id.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.4.25.post0/src/js/basis/basis.ts` & `mat3ra-made-2024.4.8.post0/src/js/basis/basis.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.4.25.post0/src/js/basis/constrained_basis.ts` & `mat3ra-made-2024.4.8.post0/src/js/basis/constrained_basis.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.4.25.post0/src/js/cell/cell.ts` & `mat3ra-made-2024.4.8.post0/src/js/cell/cell.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.4.25.post0/src/js/cell/conventional_cell.ts` & `mat3ra-made-2024.4.8.post0/src/js/cell/conventional_cell.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.4.25.post0/src/js/cell/primitive_cell.ts` & `mat3ra-made-2024.4.8.post0/src/js/cell/primitive_cell.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.4.25.post0/src/js/constraints/constraints.ts` & `mat3ra-made-2024.4.8.post0/src/js/constraints/constraints.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.4.25.post0/src/js/lattice/lattice.ts` & `mat3ra-made-2024.4.8.post0/src/js/lattice/lattice.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.4.25.post0/src/js/lattice/lattice_bravais.ts` & `mat3ra-made-2024.4.8.post0/src/js/lattice/lattice_bravais.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.4.25.post0/src/js/lattice/lattice_vectors.ts` & `mat3ra-made-2024.4.8.post0/src/js/lattice/lattice_vectors.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.4.25.post0/src/js/lattice/reciprocal/lattice_reciprocal.js` & `mat3ra-made-2024.4.8.post0/src/js/lattice/reciprocal/lattice_reciprocal.js`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.4.25.post0/src/js/lattice/reciprocal/paths.js` & `mat3ra-made-2024.4.8.post0/src/js/lattice/reciprocal/paths.js`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.4.25.post0/src/js/lattice/reciprocal/symmetry_points.ts` & `mat3ra-made-2024.4.8.post0/src/js/lattice/reciprocal/symmetry_points.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.4.25.post0/src/js/lattice/types.ts` & `mat3ra-made-2024.4.8.post0/src/js/lattice/types.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.4.25.post0/src/js/lattice/unit_cell.ts` & `mat3ra-made-2024.4.8.post0/src/js/lattice/unit_cell.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.4.25.post0/src/js/made.js` & `mat3ra-made-2024.4.8.post0/src/js/made.js`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.4.25.post0/src/js/material.ts` & `mat3ra-made-2024.4.8.post0/src/js/material.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.4.25.post0/src/js/parsers/espresso.ts` & `mat3ra-made-2024.4.8.post0/src/js/parsers/espresso.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.4.25.post0/src/js/parsers/native_format_parsers.js` & `mat3ra-made-2024.4.8.post0/src/js/parsers/native_format_parsers.js`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.4.25.post0/src/js/parsers/poscar.ts` & `mat3ra-made-2024.4.8.post0/src/js/parsers/poscar.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.4.25.post0/src/js/parsers/xyz.ts` & `mat3ra-made-2024.4.8.post0/src/js/parsers/xyz.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.4.25.post0/src/js/parsers/xyz_combinatorial_basis.js` & `mat3ra-made-2024.4.8.post0/src/js/parsers/xyz_combinatorial_basis.js`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.4.25.post0/src/js/tools/basis.js` & `mat3ra-made-2024.4.8.post0/src/js/tools/basis.js`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.4.25.post0/src/js/tools/cell.js` & `mat3ra-made-2024.4.8.post0/src/js/tools/cell.js`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.4.25.post0/src/js/tools/material.js` & `mat3ra-made-2024.4.8.post0/src/js/tools/material.js`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.4.25.post0/src/js/tools/supercell.ts` & `mat3ra-made-2024.4.8.post0/src/js/tools/supercell.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.4.25.post0/src/js/tools/surface.js` & `mat3ra-made-2024.4.8.post0/src/js/tools/surface.js`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.4.25.post0/src/py/mat3ra/made/material.py` & `mat3ra-made-2024.4.8.post0/src/py/mat3ra/made/material.py`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.4.25.post0/src/py/mat3ra_made.egg-info/PKG-INFO` & `mat3ra-made-2024.4.8.post0/src/py/mat3ra_made.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mat3ra-made
-Version: 2024.4.25.post0
+Version: 2024.4.8.post0
 Summary: MAterials DEfinitions and/or MAterials DEsign library.
 Author-email: "Exabyte Inc." <info@mat3ra.com>
 License: # LICENSE
         
         Copyright 2019 Exabyte Inc.
         
         Licensed under the Apache License, Version 2.0 (the "License");
@@ -23,78 +23,53 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Software Development
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: numpy
+Requires-Dist: pymatgen
+Requires-Dist: ase
 Requires-Dist: mat3ra-esse
 Requires-Dist: mat3ra-code
-Provides-Extra: tools
-Requires-Dist: pymatgen; extra == "tools"
-Requires-Dist: ase; extra == "tools"
-Provides-Extra: dev
-Requires-Dist: pre-commit; extra == "dev"
-Requires-Dist: black; extra == "dev"
-Requires-Dist: ruff; extra == "dev"
-Requires-Dist: isort; extra == "dev"
-Requires-Dist: mypy; extra == "dev"
-Requires-Dist: pip-tools; extra == "dev"
 Provides-Extra: tests
 Requires-Dist: coverage[toml]>=5.3; extra == "tests"
+Requires-Dist: pre-commit; extra == "tests"
+Requires-Dist: black; extra == "tests"
+Requires-Dist: ruff; extra == "tests"
+Requires-Dist: isort; extra == "tests"
+Requires-Dist: mypy; extra == "tests"
+Requires-Dist: pip-tools; extra == "tests"
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: pytest-cov; extra == "tests"
-Requires-Dist: gradio; extra == "tests"
 Requires-Dist: pydantic; extra == "tests"
-Requires-Dist: mat3ra-made[tools]; extra == "tests"
+Requires-Dist: gradio; extra == "tests"
+Provides-Extra: tools
+Requires-Dist: pymatgen; extra == "tools"
+Requires-Dist: ase; extra == "tools"
 Provides-Extra: all
 Requires-Dist: mat3ra-made[tests]; extra == "all"
-Requires-Dist: mat3ra-made[dev]; extra == "all"
+Requires-Dist: mat3ra-made[tools]; extra == "all"
 
 [![npm version](https://badge.fury.io/js/%40mat3ra%2Fmade.svg)](https://badge.fury.io/js/%40mat3ra%2Fmade)
 [![License: Apache](https://img.shields.io/badge/License-Apache-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0)
 
 # Made
 
 Made is a library for **MA**terials **DE**sign in JavaScript/TypeScript and Python. It allows for the creation and manipulation of material structures from atoms up on the web. The library is aimed to be used for the development of web applications, both on the client (web browser) and server (eg. Node.js) side.
 
-## 1. Overview
-
-The package provides a software environment for interacting with Materials-related data structures from ESSE Data Convention [[1]](#links) for use on the web.
-
-## 2. Installation
-
-### 2.1. JavaScript/TypeScript
-
-From NPM for use within a software project:
-
-```bash
-npm install @mat3ra/made
-
-```
-
-### 2.2. Python
+The library was originally designed as part of and presently powers materials design capabilities of the [Exabyte.io](https://exabyte.io) platform. For example, [this page](https://platform.exabyte.io/demo/materials/n3HSzCmyoctgJFGGE) representing a crystal of Silicon online uses Made.js.
 
-From PyPI for use within a software project:
+Exabyte.io believe in a collaborative future of materials design on the web.
 
-```bash
-pip install mat3ra-made
-```
+## Functionality
 
-When willing to use the optional `tools` module, install the package with the following command:
-
-```bash
-pip install "mat3ra-made[tools]"
-```
-
-
-## 3. Functionality
-
-As below
+As below:
 
+- the package provides a software environment for interacting with Materials-related data structures from ESSE Data Convention [[1]](#links) and is written in ECMAScript 2015 for use on the web
 - High-level classes for the representation of the [Material](src/material.js) and the corresponding structural information, ie:
     - [Basis](src/basis/basis.js),
     - [Lattice](src/lattice/lattice.js),
     - [ReciprocalLattice](src/lattice/reciprocal/lattice_reciprocal.js),
     - [Cell](src/cell/cell.js),
     - [AtomicConstraints](src/constraints/constraints.js)
     - and others to be added.
@@ -105,82 +80,98 @@
     - and others to be added.
 - structural generation and analysis tools:
     - [supercell](src/tools/supercell.js)
     - [surfaces](src/tools/surface.js)
     - [combinatorial sets](src/parsers/xyz_combinatorial_basis.js)
     - [interpolated sets for chemical reactions](src/tools/basis.js)
 
+The package is written in a modular way easy to extend. Contributions can be in the form of additional tools or modules you develop, or feature requests and [bug/issue reports](https://help.github.com/articles/creating-an-issue/).
+
+## Installation
+
+From NPM for use within a software project:
+
+```bash
+npm install @mat3ra/made
 
-## 4. Contribution
+```
+
+From source to contribute to development:
+
+```bash
+git clone git@github.com:Exabyte-io/made
+```
+
+## Contribution
 
 This repository is an [open-source](LICENSE.md) work-in-progress and we welcome contributions.
 
+### Why contribute?
+
 We regularly deploy the latest code containing all accepted contributions online as part of the [Mat3ra.com](https://mat3ra.com) platform, so contributors will see their code in action there.
 
+### Adding new functionality
+
 We suggest forking this repository and introducing the adjustments there to be considered for merging into this repository as explained in more details [here](https://gist.github.com/Chaser324/ce0505fbed06b947d962), for example.
 
-### 4.1. Source code conventions
+### Source code conventions
 
-Object-oriented design patterns encapsulate key concepts following the conventions below.
+Made.js is written in EcmaScript 6th edition [[2]](#links) with the application of object-oriented design patterns encapsulating key concepts following the conventions below.
 
 1. Classes follow the Exabyte Data Convention and data structures defined in ESSE [[1]](#links)
 
 2. Only materials-related code is considered. Properties related to [simulation model](https://docs.exabyte.io/models/overview/) parameters (eg. type of approximation, numerical parameters) shall go elsewhere.
 
 3. `tools` directory contains helper functions that act on one or more classes and include an external parameter. Functions that use class data without any external parameters should be implemented inside the class. For example, `basis.clone()` is implemented in `Basis`, but basis repetition is implemented as a tool in the correspondingly named function ([tools/basis.js#repeat](src/tools/basis.js)) because the repetion requires a parameter external to basis - number of repetitions in 3 spatial dimensions.
 
-4. [Deprecated, use mat3ra-parsers or @mat3ra/parsers] `parsers` directory contains the parsers to- and from- ESSE format mentioned in 1. All functionality related to external data conversion is contained in this directory.
+4. `parsers` directory contains the parsers to- and from- ESSE format mentioned in 1. All functionality related to external data conversion is contained in this directory.
 
 
-### 4.2. TODO list
+### TODO list
 
-[Outdated] Desirable features for implementation:
+Desirable features for implementation:
 
 - identify primitive / conventional structures
 - support for molecular geometries
 - support for polymer geometries
 - radial correlation function calculation
 - generation of complex atomic shapes:
     - fullerene
     - nanotube
     - nanowire
     - nano-cluster
     - a combination of the above
     - arbitrary atomic arrangement
 
-## 5. Development
-
-### 5.1. JavaScript/TypeScript
-
-#### 5.1.1. Tests
+## Tests
 
 Made tests are written based on Mocha [6](#links) testing framework and can be executed as follows.
 
 ```bash
 git pull
 git lfs pull
 ```
 to get the latest test fixtures from LFS, and then:
 
 ```bash
 npm install
 npm test
 ```
 
-#### 5.1.2. Important Notes
+### Tests Important Notes
 
 1. Keep the tests directory structure similar to the main codebase directory structure. Every JS module in the main codebase should have a corresponding module in tests directory which implements the tests for provided functionality.
 
 2. Add tests fixtures into [fixtures](./tests/fixtures) directory. The fixtures are automatically stored on Git LFS [7](#links).
 
 3. If the fixtures are going to be used inside multiple cases, read and export them inside [enums](./tests/enums.js) to avoid code duplicates.
 
 4. [Tests setup module](./tests/setup.js) can be used to implement the hooks that are used to prepare the tests environment.
 
-#### 5.1.3. Using Linter
+## Using Linter
 
 Linter setup will prevent committing files that don't adhere to the code standard. It will
 attempt to fix what it can automatically prior to the commit in order to reduce diff noise. This can lead to "unexpected" behavior where a
 file that is staged for commit is not identical to the file that actually gets committed. This happens
 in the `lint-staged` directive of the `package.json` file (by using a `husky` pre-commit hook). For example,
 if you add extra whitespace to a file, stage it, and try to commit it, you will see the following:
 
@@ -206,52 +197,21 @@
 ```bash
 npm run lint:fix
 ```
 
 In which case, you may need to then add the linter edits to your staging, which in the example above, puts the
 file back to identical with the base branch, resulting in no staged changes whatsoever.
 
-#### 5.1.4. Configuring WebStorm for use with Linter
+## Configuring WebStorm for use with Linter
 
 In order for the WebStorm IDE to take full advantage of the linting configuration, it can be configured in the project:
 
 - `Preferences -> Languages & Frameworks -> JavaScript -> Code Quality Tools -> ESLint`
 - Check `Automatic ESLint configuration` which should infer all the configurations from the project directory
 
-### 5.2. Python
-
-#### 5.2.1. Tests
-
-Python 3.8+ is required to run the tests. We recommend using PyEnv to manage Python versions. Tests are written based on PyTest and can be executed as follows.
-
-```bash
-virtualenv .venv
-source .venv/bin/activate
-pip install ".[tests]"
-pytest tests/py
-```
-
-#### 5.2.2. Important Notes
-
-Conventions:
-
-- The "tools" module has external dependencies on "pymatgen" and "ase" packages and so is meant as optional. When implementing new functionality, the use of ASE is recommended over pymatgen for compatibility purposes.
-
-### 5.3. Known Issues
-
-#### 5.3.1. JavaScript/TypeScript
-
-To be added.
-
-#### 5.3.2. Python
-
-As below:
-
-- Python 3.8 tests are failing on Apple Silicon due to https://github.com/materialsproject/pymatgen/issues/3521
-
 ## Links
 
 1. [Exabyte Source of Schemas and Examples (ESSE), Github Repository](https://github.com/exabyte-io/exabyte-esse)
 2. [ECMAScript 2015 Language Specifications](https://www.ecma-international.org/ecma-262/6.0/)
 3. [POSCAR file format, official website](https://cms.mpi.univie.ac.at/vasp/guide/node59.html)
 4. [XYZ file format, Wikipedia](https://en.wikipedia.org/wiki/XYZ_file_format)
 5. [Quantum ESPRESSO, Official Website](https://www.quantum-espresso.org/)
```

### Comparing `mat3ra_made-2024.4.25.post0/src/py/mat3ra_made.egg-info/SOURCES.txt` & `mat3ra-made-2024.4.8.post0/src/py/mat3ra_made.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -55,19 +55,15 @@
 src/js/tools/supercell.ts
 src/js/tools/surface.js
 src/py/__init__.py
 src/py/mat3ra/__init__.py
 src/py/mat3ra/made/__init__.py
 src/py/mat3ra/made/material.py
 src/py/mat3ra/made/tools/__init__.py
-src/py/mat3ra/made/tools/analyze.py
-src/py/mat3ra/made/tools/calculate.py
-src/py/mat3ra/made/tools/convert.py
-src/py/mat3ra/made/tools/modify.py
-src/py/mat3ra/made/tools/utils.py
+src/py/mat3ra/made/tools/material.py
 src/py/mat3ra_made.egg-info/PKG-INFO
 src/py/mat3ra_made.egg-info/SOURCES.txt
 src/py/mat3ra_made.egg-info/dependency_links.txt
 src/py/mat3ra_made.egg-info/requires.txt
 src/py/mat3ra_made.egg-info/top_level.txt
 tests/.gitattributes
 tests/fixtures/AsGe-basis.json
@@ -119,11 +115,8 @@
 tests/js/parsers/xyz.js
 tests/js/parsers/xyz_combinatorial_basis.js
 tests/js/tools/basis.js
 tests/js/tools/supercell.js
 tests/js/tools/surface.js
 tests/py/unit/__init__.py
 tests/py/unit/test_material.py
-tests/py/unit/test_tools_analyze.py
-tests/py/unit/test_tools_calculate.py
-tests/py/unit/test_tools_convert.py
-tests/py/unit/test_tools_modify.py
+tests/py/unit/test_tools_material.py
```

### Comparing `mat3ra_made-2024.4.25.post0/tests/fixtures/C2H4-translated.json` & `mat3ra-made-2024.4.8.post0/tests/fixtures/C2H4-translated.json`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.4.25.post0/tests/fixtures/C2H4.json` & `mat3ra-made-2024.4.8.post0/tests/fixtures/C2H4.json`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.4.25.post0/tests/fixtures/FeO.json` & `mat3ra-made-2024.4.8.post0/tests/fixtures/FeO.json`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.4.25.post0/tests/fixtures/Graphene.json` & `mat3ra-made-2024.4.8.post0/tests/fixtures/Graphene.json`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.4.25.post0/tests/fixtures/H2+H-final.json` & `mat3ra-made-2024.4.8.post0/tests/fixtures/H2+H-final.json`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.4.25.post0/tests/fixtures/H2+H-image.json` & `mat3ra-made-2024.4.8.post0/tests/fixtures/H2+H-image.json`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.4.25.post0/tests/fixtures/H2+H-initial.json` & `mat3ra-made-2024.4.8.post0/tests/fixtures/H2+H-initial.json`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.4.25.post0/tests/fixtures/Na.json` & `mat3ra-made-2024.4.8.post0/tests/fixtures/Na.json`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.4.25.post0/tests/fixtures/Na4Cl4-cartesian.json` & `mat3ra-made-2024.4.8.post0/tests/fixtures/Na4Cl4-cartesian.json`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.4.25.post0/tests/fixtures/Na4Cl4.json` & `mat3ra-made-2024.4.8.post0/tests/fixtures/Na4Cl4.json`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.4.25.post0/tests/fixtures/Na4Cl4.poscar` & `mat3ra-made-2024.4.8.post0/tests/fixtures/Na4Cl4.poscar`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.4.25.post0/tests/fixtures/Ni-hex.json` & `mat3ra-made-2024.4.8.post0/tests/fixtures/Ni-hex.json`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.4.25.post0/tests/fixtures/Si-hex.json` & `mat3ra-made-2024.4.8.post0/tests/fixtures/Si-hex.json`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.4.25.post0/tests/fixtures/Si-slab.json` & `mat3ra-made-2024.4.8.post0/tests/fixtures/Si-slab.json`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.4.25.post0/tests/fixtures/Si-supercell.json` & `mat3ra-made-2024.4.8.post0/tests/fixtures/Si-supercell.json`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.4.25.post0/tests/fixtures/Si.json` & `mat3ra-made-2024.4.8.post0/tests/fixtures/Si.json`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.4.25.post0/tests/fixtures/Si2-basis-repeated.json` & `mat3ra-made-2024.4.8.post0/tests/fixtures/Si2-basis-repeated.json`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.4.25.post0/tests/fixtures/Zr1H23Zr1H1.json` & `mat3ra-made-2024.4.8.post0/tests/fixtures/Zr1H23Zr1H1.json`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.4.25.post0/tests/fixtures/Zr1H23Zr1H1.poscar` & `mat3ra-made-2024.4.8.post0/tests/fixtures/Zr1H23Zr1H1.poscar`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.4.25.post0/tests/js/basis/basis.js` & `mat3ra-made-2024.4.8.post0/tests/js/basis/basis.js`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.4.25.post0/tests/js/cell/cell.js` & `mat3ra-made-2024.4.8.post0/tests/js/cell/cell.js`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.4.25.post0/tests/js/cell/primitive_cell.js` & `mat3ra-made-2024.4.8.post0/tests/js/cell/primitive_cell.js`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.4.25.post0/tests/js/constraints/constraints.js` & `mat3ra-made-2024.4.8.post0/tests/js/constraints/constraints.js`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.4.25.post0/tests/js/enums.js` & `mat3ra-made-2024.4.8.post0/tests/js/enums.js`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.4.25.post0/tests/js/lattice/lattice.js` & `mat3ra-made-2024.4.8.post0/tests/js/lattice/lattice.js`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.4.25.post0/tests/js/lattice/lattice_bravais.js` & `mat3ra-made-2024.4.8.post0/tests/js/lattice/lattice_bravais.js`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.4.25.post0/tests/js/lattice/lattice_reciprocal.js` & `mat3ra-made-2024.4.8.post0/tests/js/lattice/lattice_reciprocal.js`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.4.25.post0/tests/js/parsers/native_formats.js` & `mat3ra-made-2024.4.8.post0/tests/js/parsers/native_formats.js`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.4.25.post0/tests/js/parsers/poscar.js` & `mat3ra-made-2024.4.8.post0/tests/js/parsers/poscar.js`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.4.25.post0/tests/js/parsers/xyz.js` & `mat3ra-made-2024.4.8.post0/tests/js/parsers/xyz.js`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.4.25.post0/tests/js/parsers/xyz_combinatorial_basis.js` & `mat3ra-made-2024.4.8.post0/tests/js/parsers/xyz_combinatorial_basis.js`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.4.25.post0/tests/js/tools/basis.js` & `mat3ra-made-2024.4.8.post0/tests/js/tools/basis.js`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.4.25.post0/tests/js/tools/supercell.js` & `mat3ra-made-2024.4.8.post0/tests/js/tools/supercell.js`

 * *Files identical despite different names*

