# Comparing `tmp/caustics-0.7.0.tar.gz` & `tmp/caustics-0.8.0.tar.gz`

## Comparing `caustics-0.7.0.tar` & `caustics-0.8.0.tar`

### file list

```diff
@@ -1,108 +1,117 @@
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 caustics-0.7.0/.codespell-whitelist
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 caustics-0.7.0/.git_archival.txt
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 caustics-0.7.0/.gitattributes
--rw-r--r--   0        0        0     2249 2020-02-02 00:00:00.000000 caustics-0.7.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 caustics-0.7.0/.readthedocs.yml
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 caustics-0.7.0/noxfile.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 caustics-0.7.0/requirements.txt
--rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 caustics-0.7.0/.devcontainer/Dockerfile
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 caustics-0.7.0/.devcontainer/cpu/devcontainer.json
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 caustics-0.7.0/.devcontainer/scripts/postBuild.sh
--rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 caustics-0.7.0/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 caustics-0.7.0/.github/dependabot.yml
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 caustics-0.7.0/.github/matchers/pylint.json
--rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 caustics-0.7.0/.github/workflows/cd.yml
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 caustics-0.7.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 caustics-0.7.0/docs/Makefile
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 caustics-0.7.0/docs/requirements.txt
--rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 caustics-0.7.0/docs/source/_config.yml
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 caustics-0.7.0/docs/source/_toc.yml
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 caustics-0.7.0/docs/source/citation.rst
--rw-r--r--   0        0        0     4205 2020-02-02 00:00:00.000000 caustics-0.7.0/docs/source/contributing.rst
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 caustics-0.7.0/docs/source/getting_started.rst
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 caustics-0.7.0/docs/source/illustrative_examples.rst
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 caustics-0.7.0/docs/source/install.rst
--rw-r--r--   0        0        0     2351 2020-02-02 00:00:00.000000 caustics-0.7.0/docs/source/intro.md
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 caustics-0.7.0/docs/source/license.rst
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 caustics-0.7.0/docs/source/modules.rst
--rw-r--r--   0        0        0    13274 2020-02-02 00:00:00.000000 caustics-0.7.0/docs/source/tutorials/BasicIntroduction.ipynb
--rw-r--r--   0        0        0     4567 2020-02-02 00:00:00.000000 caustics-0.7.0/docs/source/tutorials/InvertLensEquation.ipynb
--rw-r--r--   0        0        0    15296 2020-02-02 00:00:00.000000 caustics-0.7.0/docs/source/tutorials/LensZoo.ipynb
--rw-r--r--   0        0        0     8310 2020-02-02 00:00:00.000000 caustics-0.7.0/docs/source/tutorials/MultiplaneDemo.ipynb
--rw-r--r--   0        0        0     8373 2020-02-02 00:00:00.000000 caustics-0.7.0/docs/source/tutorials/Parameters.ipynb
--rw-r--r--   0        0        0     6956 2020-02-02 00:00:00.000000 caustics-0.7.0/docs/source/tutorials/Playground.ipynb
--rw-r--r--   0        0        0     8410 2020-02-02 00:00:00.000000 caustics-0.7.0/docs/source/tutorials/Simulators.ipynb
--rw-r--r--   0        0        0     5958 2020-02-02 00:00:00.000000 caustics-0.7.0/docs/source/tutorials/VisualizeCaustics.ipynb
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 caustics-0.7.0/docs/source/tutorials/index.md
--rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 caustics-0.7.0/media/caustics_favicon.ico
--rw-r--r--   0        0        0   551338 2020-02-02 00:00:00.000000 caustics-0.7.0/media/caustics_logo.png
--rw-r--r--   0        0        0   527747 2020-02-02 00:00:00.000000 caustics-0.7.0/media/caustics_logo_white.png
--rw-r--r--   0        0        0    52708 2020-02-02 00:00:00.000000 caustics-0.7.0/media/minimal_example.png
--rw-r--r--   0        0        0   608466 2020-02-02 00:00:00.000000 caustics-0.7.0/media/minisim_jacobian.png
--rw-r--r--   0        0        0   304348 2020-02-02 00:00:00.000000 caustics-0.7.0/media/minisim_vmap.png
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 caustics-0.7.0/src/caustics/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 caustics-0.7.0/src/caustics/_version.py
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 caustics-0.7.0/src/caustics/constants.py
--rw-r--r--   0        0        0    12439 2020-02-02 00:00:00.000000 caustics-0.7.0/src/caustics/cosmology.py
--rw-r--r--   0        0        0     5948 2020-02-02 00:00:00.000000 caustics-0.7.0/src/caustics/namespace_dict.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 caustics-0.7.0/src/caustics/packed.py
--rw-r--r--   0        0        0     2864 2020-02-02 00:00:00.000000 caustics-0.7.0/src/caustics/parameter.py
--rw-r--r--   0        0        0    21804 2020-02-02 00:00:00.000000 caustics-0.7.0/src/caustics/parametrized.py
--rw-r--r--   0        0        0     6104 2020-02-02 00:00:00.000000 caustics-0.7.0/src/caustics/tests.py
--rw-r--r--   0        0        0    19525 2020-02-02 00:00:00.000000 caustics-0.7.0/src/caustics/utils.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 caustics-0.7.0/src/caustics/data/__init__.py
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 caustics-0.7.0/src/caustics/data/hdf5dataset.py
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 caustics-0.7.0/src/caustics/data/illustris_kappa.py
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 caustics-0.7.0/src/caustics/data/probes.py
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 caustics-0.7.0/src/caustics/lenses/__init__.py
--rw-r--r--   0        0        0    32985 2020-02-02 00:00:00.000000 caustics-0.7.0/src/caustics/lenses/base.py
--rw-r--r--   0        0        0     8960 2020-02-02 00:00:00.000000 caustics-0.7.0/src/caustics/lenses/epl.py
--rw-r--r--   0        0        0     4928 2020-02-02 00:00:00.000000 caustics-0.7.0/src/caustics/lenses/external_shear.py
--rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 caustics-0.7.0/src/caustics/lenses/mass_sheet.py
--rw-r--r--   0        0        0    11338 2020-02-02 00:00:00.000000 caustics-0.7.0/src/caustics/lenses/multiplane.py
--rw-r--r--   0        0        0    15419 2020-02-02 00:00:00.000000 caustics-0.7.0/src/caustics/lenses/nfw.py
--rw-r--r--   0        0        0    17069 2020-02-02 00:00:00.000000 caustics-0.7.0/src/caustics/lenses/pixelated_convergence.py
--rw-r--r--   0        0        0     4964 2020-02-02 00:00:00.000000 caustics-0.7.0/src/caustics/lenses/point.py
--rw-r--r--   0        0        0    10628 2020-02-02 00:00:00.000000 caustics-0.7.0/src/caustics/lenses/pseudo_jaffe.py
--rw-r--r--   0        0        0     5713 2020-02-02 00:00:00.000000 caustics-0.7.0/src/caustics/lenses/sie.py
--rw-r--r--   0        0        0     3958 2020-02-02 00:00:00.000000 caustics-0.7.0/src/caustics/lenses/singleplane.py
--rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 caustics-0.7.0/src/caustics/lenses/sis.py
--rw-r--r--   0        0        0    18317 2020-02-02 00:00:00.000000 caustics-0.7.0/src/caustics/lenses/tnfw.py
--rw-r--r--   0        0        0     2639 2020-02-02 00:00:00.000000 caustics-0.7.0/src/caustics/lenses/utils.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 caustics-0.7.0/src/caustics/light/__init__.py
--rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 caustics-0.7.0/src/caustics/light/base.py
--rw-r--r--   0        0        0     4211 2020-02-02 00:00:00.000000 caustics-0.7.0/src/caustics/light/pixelated.py
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 caustics-0.7.0/src/caustics/light/probes.py
--rw-r--r--   0        0        0     5425 2020-02-02 00:00:00.000000 caustics-0.7.0/src/caustics/light/sersic.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 caustics-0.7.0/src/caustics/sims/__init__.py
--rw-r--r--   0        0        0    10369 2020-02-02 00:00:00.000000 caustics-0.7.0/src/caustics/sims/lens_source.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 caustics-0.7.0/src/caustics/sims/simulator.py
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 caustics-0.7.0/tests/test_base.py
--rw-r--r--   0        0        0     2545 2020-02-02 00:00:00.000000 caustics-0.7.0/tests/test_batching.py
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 caustics-0.7.0/tests/test_cosmology.py
--rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 caustics-0.7.0/tests/test_epl.py
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 caustics-0.7.0/tests/test_external_shear.py
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 caustics-0.7.0/tests/test_interpolate_image.py
--rw-r--r--   0        0        0     3840 2020-02-02 00:00:00.000000 caustics-0.7.0/tests/test_jacobian_lens_equation.py
--rw-r--r--   0        0        0     4729 2020-02-02 00:00:00.000000 caustics-0.7.0/tests/test_kappa_grid.py
--rw-r--r--   0        0        0     6806 2020-02-02 00:00:00.000000 caustics-0.7.0/tests/test_lens_potential.py
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 caustics-0.7.0/tests/test_masssheet.py
--rw-r--r--   0        0        0     5040 2020-02-02 00:00:00.000000 caustics-0.7.0/tests/test_multiplane.py
--rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 caustics-0.7.0/tests/test_namespace_dict.py
--rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 caustics-0.7.0/tests/test_nfw.py
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 caustics-0.7.0/tests/test_parameter.py
--rw-r--r--   0        0        0     8008 2020-02-02 00:00:00.000000 caustics-0.7.0/tests/test_parametrized.py
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 caustics-0.7.0/tests/test_pixel_grid.py
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 caustics-0.7.0/tests/test_point.py
--rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 caustics-0.7.0/tests/test_pseudo_jaffe.py
--rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 caustics-0.7.0/tests/test_sersic.py
--rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 caustics-0.7.0/tests/test_sie.py
--rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 caustics-0.7.0/tests/test_simulator.py
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 caustics-0.7.0/tests/test_sis.py
--rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 caustics-0.7.0/tests/test_tnfw.py
--rw-r--r--   0        0        0     7610 2020-02-02 00:00:00.000000 caustics-0.7.0/tests/utils.py
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 caustics-0.7.0/.gitignore
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 caustics-0.7.0/LICENSE
--rw-r--r--   0        0        0     4777 2020-02-02 00:00:00.000000 caustics-0.7.0/README.md
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 caustics-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     7405 2020-02-02 00:00:00.000000 caustics-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 caustics-0.8.0/.codespell-whitelist
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 caustics-0.8.0/.git_archival.txt
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 caustics-0.8.0/.gitattributes
+-rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 caustics-0.8.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 caustics-0.8.0/.readthedocs.yml
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 caustics-0.8.0/noxfile.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 caustics-0.8.0/requirements.txt
+-rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 caustics-0.8.0/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 caustics-0.8.0/.devcontainer/cpu/devcontainer.json
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 caustics-0.8.0/.devcontainer/scripts/postBuild.sh
+-rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 caustics-0.8.0/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 caustics-0.8.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 caustics-0.8.0/.github/matchers/pylint.json
+-rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 caustics-0.8.0/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 caustics-0.8.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 caustics-0.8.0/docs/Makefile
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 caustics-0.8.0/docs/requirements.txt
+-rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 caustics-0.8.0/docs/source/_config.yml
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 caustics-0.8.0/docs/source/_toc.yml
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 caustics-0.8.0/docs/source/citation.rst
+-rw-r--r--   0        0        0     5963 2020-02-02 00:00:00.000000 caustics-0.8.0/docs/source/contributing.rst
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 caustics-0.8.0/docs/source/getting_started.rst
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 caustics-0.8.0/docs/source/illustrative_examples.rst
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 caustics-0.8.0/docs/source/install.rst
+-rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 caustics-0.8.0/docs/source/intro.md
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 caustics-0.8.0/docs/source/license.rst
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 caustics-0.8.0/docs/source/modules.rst
+-rw-r--r--   0        0        0    13240 2020-02-02 00:00:00.000000 caustics-0.8.0/docs/source/tutorials/BasicIntroduction.ipynb
+-rw-r--r--   0        0        0     4480 2020-02-02 00:00:00.000000 caustics-0.8.0/docs/source/tutorials/InvertLensEquation.ipynb
+-rw-r--r--   0        0        0    15030 2020-02-02 00:00:00.000000 caustics-0.8.0/docs/source/tutorials/LensZoo.ipynb
+-rw-r--r--   0        0        0     8067 2020-02-02 00:00:00.000000 caustics-0.8.0/docs/source/tutorials/MultiplaneDemo.ipynb
+-rw-r--r--   0        0        0     7921 2020-02-02 00:00:00.000000 caustics-0.8.0/docs/source/tutorials/Parameters.ipynb
+-rw-r--r--   0        0        0     6870 2020-02-02 00:00:00.000000 caustics-0.8.0/docs/source/tutorials/Playground.ipynb
+-rw-r--r--   0        0        0     8240 2020-02-02 00:00:00.000000 caustics-0.8.0/docs/source/tutorials/Simulators.ipynb
+-rw-r--r--   0        0        0     5857 2020-02-02 00:00:00.000000 caustics-0.8.0/docs/source/tutorials/VisualizeCaustics.ipynb
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 caustics-0.8.0/docs/source/tutorials/index.md
+-rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 caustics-0.8.0/media/caustics_favicon.ico
+-rw-r--r--   0        0        0   551338 2020-02-02 00:00:00.000000 caustics-0.8.0/media/caustics_logo.png
+-rw-r--r--   0        0        0   527747 2020-02-02 00:00:00.000000 caustics-0.8.0/media/caustics_logo_white.png
+-rw-r--r--   0        0        0    52708 2020-02-02 00:00:00.000000 caustics-0.8.0/media/minimal_example.png
+-rw-r--r--   0        0        0   608466 2020-02-02 00:00:00.000000 caustics-0.8.0/media/minisim_jacobian.png
+-rw-r--r--   0        0        0   304348 2020-02-02 00:00:00.000000 caustics-0.8.0/media/minisim_vmap.png
+-rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 caustics-0.8.0/src/caustics/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 caustics-0.8.0/src/caustics/_version.py
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 caustics-0.8.0/src/caustics/constants.py
+-rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 caustics-0.8.0/src/caustics/io.py
+-rw-r--r--   0        0        0     5948 2020-02-02 00:00:00.000000 caustics-0.8.0/src/caustics/namespace_dict.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 caustics-0.8.0/src/caustics/packed.py
+-rw-r--r--   0        0        0     2904 2020-02-02 00:00:00.000000 caustics-0.8.0/src/caustics/parameter.py
+-rw-r--r--   0        0        0    21872 2020-02-02 00:00:00.000000 caustics-0.8.0/src/caustics/parametrized.py
+-rw-r--r--   0        0        0     6104 2020-02-02 00:00:00.000000 caustics-0.8.0/src/caustics/tests.py
+-rw-r--r--   0        0        0    19559 2020-02-02 00:00:00.000000 caustics-0.8.0/src/caustics/utils.py
+-rw-r--r--   0        0        0     5794 2020-02-02 00:00:00.000000 caustics-0.8.0/src/caustics/cosmology/FlatLambdaCDM.py
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 caustics-0.8.0/src/caustics/cosmology/__init__.py
+-rw-r--r--   0        0        0     7002 2020-02-02 00:00:00.000000 caustics-0.8.0/src/caustics/cosmology/base.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 caustics-0.8.0/src/caustics/data/__init__.py
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 caustics-0.8.0/src/caustics/data/hdf5dataset.py
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 caustics-0.8.0/src/caustics/data/illustris_kappa.py
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 caustics-0.8.0/src/caustics/data/probes.py
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 caustics-0.8.0/src/caustics/lenses/__init__.py
+-rw-r--r--   0        0        0    33108 2020-02-02 00:00:00.000000 caustics-0.8.0/src/caustics/lenses/base.py
+-rw-r--r--   0        0        0     9241 2020-02-02 00:00:00.000000 caustics-0.8.0/src/caustics/lenses/epl.py
+-rw-r--r--   0        0        0     5088 2020-02-02 00:00:00.000000 caustics-0.8.0/src/caustics/lenses/external_shear.py
+-rw-r--r--   0        0        0     3613 2020-02-02 00:00:00.000000 caustics-0.8.0/src/caustics/lenses/mass_sheet.py
+-rw-r--r--   0        0        0    11324 2020-02-02 00:00:00.000000 caustics-0.8.0/src/caustics/lenses/multiplane.py
+-rw-r--r--   0        0        0    15778 2020-02-02 00:00:00.000000 caustics-0.8.0/src/caustics/lenses/nfw.py
+-rw-r--r--   0        0        0    17234 2020-02-02 00:00:00.000000 caustics-0.8.0/src/caustics/lenses/pixelated_convergence.py
+-rw-r--r--   0        0        0     5132 2020-02-02 00:00:00.000000 caustics-0.8.0/src/caustics/lenses/point.py
+-rw-r--r--   0        0        0    10976 2020-02-02 00:00:00.000000 caustics-0.8.0/src/caustics/lenses/pseudo_jaffe.py
+-rw-r--r--   0        0        0     5952 2020-02-02 00:00:00.000000 caustics-0.8.0/src/caustics/lenses/sie.py
+-rw-r--r--   0        0        0     4001 2020-02-02 00:00:00.000000 caustics-0.8.0/src/caustics/lenses/singleplane.py
+-rw-r--r--   0        0        0     4528 2020-02-02 00:00:00.000000 caustics-0.8.0/src/caustics/lenses/sis.py
+-rw-r--r--   0        0        0    18856 2020-02-02 00:00:00.000000 caustics-0.8.0/src/caustics/lenses/tnfw.py
+-rw-r--r--   0        0        0     2639 2020-02-02 00:00:00.000000 caustics-0.8.0/src/caustics/lenses/utils.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 caustics-0.8.0/src/caustics/light/__init__.py
+-rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 caustics-0.8.0/src/caustics/light/base.py
+-rw-r--r--   0        0        0     4301 2020-02-02 00:00:00.000000 caustics-0.8.0/src/caustics/light/pixelated.py
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 caustics-0.8.0/src/caustics/light/probes.py
+-rw-r--r--   0        0        0     5554 2020-02-02 00:00:00.000000 caustics-0.8.0/src/caustics/light/sersic.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 caustics-0.8.0/src/caustics/sims/__init__.py
+-rw-r--r--   0        0        0    10369 2020-02-02 00:00:00.000000 caustics-0.8.0/src/caustics/sims/lens_source.py
+-rw-r--r--   0        0        0     2930 2020-02-02 00:00:00.000000 caustics-0.8.0/src/caustics/sims/simulator.py
+-rw-r--r--   0        0        0     8985 2020-02-02 00:00:00.000000 caustics-0.8.0/src/caustics/sims/state_dict.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 caustics-0.8.0/tests/conftest.py
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 caustics-0.8.0/tests/test_base.py
+-rw-r--r--   0        0        0     2545 2020-02-02 00:00:00.000000 caustics-0.8.0/tests/test_batching.py
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 caustics-0.8.0/tests/test_cosmology.py
+-rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 caustics-0.8.0/tests/test_epl.py
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 caustics-0.8.0/tests/test_external_shear.py
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 caustics-0.8.0/tests/test_interpolate_image.py
+-rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 caustics-0.8.0/tests/test_io.py
+-rw-r--r--   0        0        0     3840 2020-02-02 00:00:00.000000 caustics-0.8.0/tests/test_jacobian_lens_equation.py
+-rw-r--r--   0        0        0     4729 2020-02-02 00:00:00.000000 caustics-0.8.0/tests/test_kappa_grid.py
+-rw-r--r--   0        0        0     6806 2020-02-02 00:00:00.000000 caustics-0.8.0/tests/test_lens_potential.py
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 caustics-0.8.0/tests/test_masssheet.py
+-rw-r--r--   0        0        0     5040 2020-02-02 00:00:00.000000 caustics-0.8.0/tests/test_multiplane.py
+-rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 caustics-0.8.0/tests/test_namespace_dict.py
+-rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 caustics-0.8.0/tests/test_nfw.py
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 caustics-0.8.0/tests/test_parameter.py
+-rw-r--r--   0        0        0     8008 2020-02-02 00:00:00.000000 caustics-0.8.0/tests/test_parametrized.py
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 caustics-0.8.0/tests/test_pixel_grid.py
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 caustics-0.8.0/tests/test_point.py
+-rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 caustics-0.8.0/tests/test_pseudo_jaffe.py
+-rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 caustics-0.8.0/tests/test_sersic.py
+-rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 caustics-0.8.0/tests/test_sie.py
+-rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 caustics-0.8.0/tests/test_simulator_runs.py
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 caustics-0.8.0/tests/test_sis.py
+-rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 caustics-0.8.0/tests/test_tnfw.py
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 caustics-0.8.0/tests/sims/conftest.py
+-rw-r--r--   0        0        0     2875 2020-02-02 00:00:00.000000 caustics-0.8.0/tests/sims/test_simulator.py
+-rw-r--r--   0        0        0     6980 2020-02-02 00:00:00.000000 caustics-0.8.0/tests/sims/test_state_dict.py
+-rw-r--r--   0        0        0     7640 2020-02-02 00:00:00.000000 caustics-0.8.0/tests/utils/__init__.py
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 caustics-0.8.0/.gitignore
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 caustics-0.8.0/LICENSE
+-rw-r--r--   0        0        0     4743 2020-02-02 00:00:00.000000 caustics-0.8.0/README.md
+-rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 caustics-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     7588 2020-02-02 00:00:00.000000 caustics-0.8.0/PKG-INFO
```

### Comparing `caustics-0.7.0/.pre-commit-config.yaml` & `caustics-0.8.0/.pre-commit-config.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 exclude: |
   (?x)^(
-    tests/utils.py
+    tests/utils/
   )
 
 ci:
   autoupdate_commit_msg: "chore: update pre-commit hooks"
   autofix_commit_msg: "style: pre-commit fixes"
 
 repos:
   - repo: https://github.com/psf/black
-    rev: "23.12.1"
+    rev: "24.1.1"
     hooks:
       - id: black-jupyter
 
   - repo: https://github.com/asottile/blacken-docs
     rev: "1.16.0"
     hooks:
       - id: blacken-docs
@@ -46,37 +46,36 @@
     rev: "v4.0.0-alpha.8"
     hooks:
       - id: prettier
         types_or: [yaml, markdown, html, css, scss, javascript, json]
         args: [--prose-wrap=always]
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: "v0.1.9"
+    rev: "v0.2.1"
     hooks:
       - id: ruff
         args: ["--fix", "--show-fixes"]
 
-  # 2023-12-11: Not use mypy for now.
-  # - repo: https://github.com/pre-commit/mirrors-mypy
-  #   rev: "v1.8.0"
-  #   hooks:
-  #     - id: mypy
-  #       files: src|tests
-  #       args: []
-  #       additional_dependencies:
-  #         - pytest
+  - repo: https://github.com/pre-commit/mirrors-mypy
+    rev: "v1.8.0"
+    hooks:
+      - id: mypy
+        files: src
+        args: ["--ignore-missing-imports"]
+        additional_dependencies:
+          - pytest
 
   - repo: https://github.com/codespell-project/codespell
     rev: "v2.2.6"
     hooks:
       - id: codespell
         args: ["--write-changes", "--ignore-words", ".codespell-whitelist"]
 
   - repo: https://github.com/kynan/nbstripout
-    rev: 0.6.1
+    rev: 0.7.1
     hooks:
       - id: nbstripout
         args: [--extra-keys=metadata.kernelspec metadata.language_info.version]
 
   - repo: local
     hooks:
       - id: disallow-caps
```

### Comparing `caustics-0.7.0/.readthedocs.yml` & `caustics-0.8.0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `caustics-0.7.0/noxfile.py` & `caustics-0.8.0/noxfile.py`

 * *Files identical despite different names*

### Comparing `caustics-0.7.0/.devcontainer/Dockerfile` & `caustics-0.8.0/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `caustics-0.7.0/.devcontainer/cpu/devcontainer.json` & `caustics-0.8.0/.devcontainer/cpu/devcontainer.json`

 * *Files 16% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 // README at: https://github.com/devcontainers/templates/tree/main/src/anaconda
 {
   "name": "Caustics - CPU",
   "build": {
     "context": "../..",
     "dockerfile": "../Dockerfile",
     "args": {
-      "CLANG_VERSION": ""
-    }
+      "CLANG_VERSION": "",
+    },
   },
 
   // Use 'forwardPorts' to make a list of ports inside the container available locally.
   // "forwardPorts": [],
 
   // Use 'postCreateCommand' to run commands after the container is created.
   "postCreateCommand": "bash .devcontainer/scripts/postBuild.sh",
@@ -22,15 +22,15 @@
   "customizations": {
     "vscode": {
       "extensions": [
         "ms-toolsai.jupyter",
         "ms-python.python",
         "ms-vsliveshare.vsliveshare",
         "DavidAnson.vscode-markdownlint",
-        "GitHub.copilot"
-      ]
-    }
-  }
+        "GitHub.copilot",
+      ],
+    },
+  },
 
   // Uncomment to connect as root instead. More info: https://aka.ms/dev-containers-non-root.
   // "remoteUser": "root"
 }
```

### Comparing `caustics-0.7.0/.github/CONTRIBUTING.md` & `caustics-0.8.0/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `caustics-0.7.0/.github/matchers/pylint.json` & `caustics-0.8.0/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `caustics-0.7.0/.github/workflows/cd.yml` & `caustics-0.8.0/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `caustics-0.7.0/.github/workflows/ci.yml` & `caustics-0.8.0/.github/workflows/ci.yml`

 * *Files 1% similar despite different names*

```diff
@@ -67,8 +67,8 @@
           pip show ${{ env.PROJECT_NAME }}
 
       - name: Test with pytest
         run: |
           pytest -vvv --cov=${{ env.PROJECT_NAME }} --cov-report=xml --cov-report=term tests/
 
       - name: Upload coverage reports to Codecov with GitHub Action
-        uses: codecov/codecov-action@v3
+        uses: codecov/codecov-action@v4
```

### Comparing `caustics-0.7.0/docs/Makefile` & `caustics-0.8.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `caustics-0.7.0/docs/source/_config.yml` & `caustics-0.8.0/docs/source/_config.yml`

 * *Files identical despite different names*

### Comparing `caustics-0.7.0/docs/source/_toc.yml` & `caustics-0.8.0/docs/source/_toc.yml`

 * *Files identical despite different names*

### Comparing `caustics-0.7.0/docs/source/contributing.rst` & `caustics-0.8.0/docs/source/contributing.rst`

 * *Files 27% similar despite different names*

```diff
@@ -57,8 +57,35 @@
 5. Click **Create Pull Request**.
 
 Finalizing a Pull Request
 -------------------------
 
 Once the PR is submitted, we will look through it and request any changes necessary before merging it into the main branch. You can make those changes just like any other edits on your fork. Then when you push them, they will be joined in to the PR automatically and any unit tests will run again.
 
+Black Formatting Exceptions for Equations
+-----------------------------------------
+
+In the **caustics** project, we utilize the Black code formatter to ensure consistent and readable code. However, there are instances where the automatic formatting performed by Black may not align with the desired formatting for equations within the code.
+
+To address this, we have introduced the use of ``#fmt: skip`` tags to exempt specific code blocks or lines from Black formatting. This is particularly useful when dealing with equations that have a specific format or layout that should not be altered by the code formatter.
+
+How to Use ``#fmt: skip`` for Equations
+---------------------------------------
+
+To exempt a specific section of code, such as an equation, from Black formatting, simply add a comment with the ``#fmt: skip`` tag at the end of the line containing the code block. For example:
+
+.. code-block:: python
+
+    psi = (q**2 * (x**2 + self.s**2) + y**2).sqrt()  # fmt: skip
+
+In the above example, the line with the ``#fmt: skip`` comment informs Black to skip formatting for the following line containing the equation. This allows developers to maintain control over the formatting of equations while still benefiting from the automatic formatting provided by Black for the rest of the codebase.
+
+Best Practices for Black Formatting Exceptions
+----------------------------------------------
+
+- Use ``#fmt: skip`` sparingly and only for sections where manual formatting is essential.
+- Clearly document the reason for using ``#fmt: skip`` to provide context for future developers.
+
+By incorporating ``#fmt: skip`` tags for equations, we strike a balance between automated code formatting and the need for manual control over certain code elements.
+
+
 Once the PR has been merged, you may delete your fork if you aren't using it any more, or take on a new issue, it's up to you!
```

### Comparing `caustics-0.7.0/docs/source/getting_started.rst` & `caustics-0.8.0/docs/source/getting_started.rst`

 * *Files identical despite different names*

### Comparing `caustics-0.7.0/docs/source/install.rst` & `caustics-0.8.0/docs/source/install.rst`

 * *Files identical despite different names*

### Comparing `caustics-0.7.0/docs/source/intro.md` & `caustics-0.8.0/docs/source/intro.md`

 * *Files 7% similar despite different names*

```diff
@@ -23,27 +23,27 @@
 ## Minimal Example
 
 ```python
 import matplotlib.pyplot as plt
 import caustics
 import torch
 
-cosmology = caustics.cosmology.FlatLambdaCDM()
-sie = caustics.lenses.SIE(cosmology=cosmology, name="lens")
-src = caustics.light.Sersic(name="source")
-lnslt = caustics.light.Sersic(name="lenslight")
+cosmology = caustics.FlatLambdaCDM()
+sie = caustics.SIE(cosmology=cosmology, name="lens")
+src = caustics.Sersic(name="source")
+lnslt = caustics.Sersic(name="lenslight")
 
 x = torch.tensor([
 #   z_s  z_l   x0   y0   q    phi     b    x0   y0   q     phi    n    Re
     1.5, 0.5, -0.2, 0.0, 0.4, 1.5708, 1.7, 0.0, 0.0, 0.5, -0.985, 1.3, 1.0,
 #   Ie    x0   y0   q    phi  n   Re   Ie
     5.0, -0.2, 0.0, 0.8, 0.0, 1., 1.0, 10.0
 ])  # fmt: skip
 
-minisim = caustics.sims.Lens_Source(
+minisim = caustics.Lens_Source(
     lens=sie, source=src, lens_light=lnslt, pixelscale=0.05, pixels_x=100
 )
 plt.imshow(minisim(x, quad_level=3), origin="lower")
 plt.show()
 ```
 
 ![Caustics lensed image](../../media/minimal_example.png)
```

### Comparing `caustics-0.7.0/docs/source/license.rst` & `caustics-0.8.0/docs/source/license.rst`

 * *Files identical despite different names*

### Comparing `caustics-0.7.0/docs/source/tutorials/BasicIntroduction.ipynb` & `caustics-0.8.0/docs/source/tutorials/BasicIntroduction.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.99775%*

 * *Differences: {"'cells'": "{4: {'source': ['cosmology = caustics.FlatLambdaCDM()']}, 6: {'source': ['sie = "*

 * *            'caustics.SIE(cosmology=cosmology, name="lens")\']}, 8: {\'source\': [\'src = '*

 * *            'caustics.Sersic(name="source")\']}, 10: {\'source\': [\'lnslt = '*

 * *            'caustics.Sersic(name="lenslight")\']}, 12: {\'source\': {insert: [(0, \'minisim = '*

 * *            "caustics.Lens_Source(\\n')], delete: [0]}}}"}*

```diff
@@ -40,15 +40,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "cosmology = caustics.cosmology.FlatLambdaCDM()"
+                "cosmology = caustics.FlatLambdaCDM()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Lens Mass Distribution\n",
@@ -58,15 +58,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "sie = caustics.lenses.SIE(cosmology=cosmology, name=\"lens\")"
+                "sie = caustics.SIE(cosmology=cosmology, name=\"lens\")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Sersic Source Light Distribution\n",
@@ -76,15 +76,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "src = caustics.light.Sersic(name=\"source\")"
+                "src = caustics.Sersic(name=\"source\")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Sersic Lens Light Distribution\n",
@@ -94,15 +94,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "lnslt = caustics.light.Sersic(name=\"lenslight\")"
+                "lnslt = caustics.Sersic(name=\"lenslight\")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Lens Source Simulator\n",
@@ -112,15 +112,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "minisim = caustics.sims.Lens_Source(\n",
+                "minisim = caustics.Lens_Source(\n",
                 "    lens=sie, source=src, lens_light=lnslt, pixelscale=0.05, pixels_x=100\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
```

### Comparing `caustics-0.7.0/docs/source/tutorials/InvertLensEquation.ipynb` & `caustics-0.8.0/docs/source/tutorials/InvertLensEquation.ipynb`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9884758141762452%*

 * *Differences: {"'cells'": "{0: {'id': '0'}, 1: {'id': '1'}, 2: {'id': '2', 'source': {insert: [(2, 'cosmology = "*

 * *            'caustics.FlatLambdaCDM(name="cosmo")\\n\'), (16, \'lens = caustics.SIE(\\n\')], '*

 * *            "delete: [16, 2]}}, 3: {'id': '3'}, 4: {'id': '4'}, 5: {'id': '5'}}"}*

```diff
@@ -1,23 +1,23 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
-            "id": "b7d08f1d",
+            "id": "0",
             "metadata": {},
             "source": [
                 "# Inverting the Lens Equation\n",
                 "\n",
                 "The lens equation $\\vec{\\beta} = \\vec{\\theta} - \\vec{\\alpha}(\\vec{\\theta})$ allows us to find a point in the source plane given a point in the image plane. However, sometimes we know a point in the source plane and would like to see where it ends up in the image plane. This is not easy to do since a point in the source plane may map to multiple locations in the image plane. There is no closed form function to invert the lens equation, in large part because the deflection angle $\\vec{\\alpha}$ depends on the position in the image plane $\\vec{\\theta}$. To invert the lens equation, we will need to rely on optimization and a little luck to find all the images for a given source plane point. Below we will demonstrate how this is done in caustic!"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "4027aaf9",
+            "id": "1",
             "metadata": {},
             "outputs": [],
             "source": [
                 "%load_ext autoreload\n",
                 "%autoreload 2\n",
                 "\n",
                 "from functools import partial\n",
@@ -32,35 +32,35 @@
                 "\n",
                 "import caustics"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "2118e1c1",
+            "id": "2",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# initialization stuff for an SIE lens\n",
                 "\n",
-                "cosmology = caustics.cosmology.FlatLambdaCDM(name=\"cosmo\")\n",
+                "cosmology = caustics.FlatLambdaCDM(name=\"cosmo\")\n",
                 "cosmology.to(dtype=torch.float32)\n",
                 "n_pix = 100\n",
                 "res = 0.05\n",
                 "upsample_factor = 1\n",
                 "fov = res * n_pix\n",
                 "thx, thy = caustics.utils.get_meshgrid(\n",
                 "    res / upsample_factor,\n",
                 "    upsample_factor * n_pix,\n",
                 "    upsample_factor * n_pix,\n",
                 "    dtype=torch.float32,\n",
                 ")\n",
                 "z_l = torch.tensor(0.5, dtype=torch.float32)\n",
                 "z_s = torch.tensor(1.5, dtype=torch.float32)\n",
-                "lens = caustics.lenses.SIE(\n",
+                "lens = caustics.SIE(\n",
                 "    cosmology=cosmology,\n",
                 "    name=\"sie\",\n",
                 "    z_l=z_l,\n",
                 "    x0=0.0,\n",
                 "    y0=0.0,\n",
                 "    q=0.4,\n",
                 "    phi=np.pi / 5,\n",
@@ -68,15 +68,15 @@
                 "    s=1e-3,\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "98e46aa1",
+            "id": "3",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Point in the source plane\n",
                 "sp_x = torch.tensor(0.2)\n",
                 "sp_y = torch.tensor(0.2)\n",
                 "\n",
@@ -86,15 +86,15 @@
                 "# Raytrace to check\n",
                 "bx, by = lens.raytrace(x, y, z_s)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "eb73147c",
+            "id": "4",
             "metadata": {},
             "outputs": [],
             "source": [
                 "fig, ax = plt.subplots()\n",
                 "\n",
                 "A = lens.jacobian_lens_equation(thx, thy, z_s)\n",
                 "detA = torch.linalg.det(A)\n",
@@ -118,15 +118,15 @@
                 "plt.legend()\n",
                 "plt.show()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "e9f2d09f-6327-4d01-8d62-baa749ffc621",
+            "id": "5",
             "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
         "language_info": {
```

### Comparing `caustics-0.7.0/docs/source/tutorials/LensZoo.ipynb` & `caustics-0.8.0/docs/source/tutorials/LensZoo.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.986534031235899%*

 * *Differences: {"'cells'": "{0: {'id': '0'}, 1: {'id': '1'}, 2: {'id': '2', 'source': {insert: [(0, 'cosmology = "*

 * *            "caustics.FlatLambdaCDM()\\n'), (3, 'base_sersic = caustics.Sersic(\\n')], delete: [3, "*

 * *            "0]}}, 3: {'id': '3'}, 4: {'id': '4', 'source': {insert: [(0, 'lens = "*

 * *            "caustics.Point(\\n'), (6, 'sim = caustics.Lens_Source(\\n')], delete: [6, 0]}}, 5: "*

 * *            "{'id': '5'}, 6: {'id': '6', 'source': {insert: [(0, 'lens = caustics.SIS(\\n'), (6, "*

 * *            "'sim = caustics.L […]*

```diff
@@ -1,23 +1,23 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
-            "id": "e4054d16",
+            "id": "0",
             "metadata": {},
             "source": [
                 "# A Menagerie of Lenses\n",
                 "\n",
                 "Here we have a quick visual demo of every type of lens in caustic. This is a good way to pick out what you need and quickly copy paste. For all of these lenses we have placed a Sersic source with the same parameters as the background, that way you can visualize the differences between them."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "beeb58fa",
+            "id": "1",
             "metadata": {},
             "outputs": [],
             "source": [
                 "%load_ext autoreload\n",
                 "%autoreload 2\n",
                 "\n",
                 "import torch\n",
@@ -30,22 +30,22 @@
                 "\n",
                 "import caustics"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "72cbde6d",
+            "id": "2",
             "metadata": {},
             "outputs": [],
             "source": [
-                "cosmology = caustics.cosmology.FlatLambdaCDM()\n",
+                "cosmology = caustics.FlatLambdaCDM()\n",
                 "cosmology.to(dtype=torch.float32)\n",
                 "z_s = torch.tensor(1.0)\n",
-                "base_sersic = caustics.light.Sersic(\n",
+                "base_sersic = caustics.Sersic(\n",
                 "    x0=0.1,\n",
                 "    y0=0.1,\n",
                 "    q=0.6,\n",
                 "    phi=np.pi / 3,\n",
                 "    n=2.0,\n",
                 "    Re=1.0,\n",
                 "    Ie=1.0,\n",
@@ -66,36 +66,36 @@
                 "plt.gca().axis(\"off\")\n",
                 "plt.title(\"Base Sersic\")\n",
                 "plt.show()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "aa183e3d",
+            "id": "3",
             "metadata": {},
             "source": [
                 "## Point (Point)\n",
                 "\n",
                 "The simplest lens, an infinitely small point of mass (did someone say black holes?)."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "4b4b2faa",
+            "id": "4",
             "metadata": {},
             "outputs": [],
             "source": [
-                "lens = caustics.lenses.Point(\n",
+                "lens = caustics.Point(\n",
                 "    cosmology=cosmology,\n",
                 "    x0=0.0,\n",
                 "    y0=0.0,\n",
                 "    th_ein=1.0,\n",
                 ")\n",
-                "sim = caustics.sims.Lens_Source(\n",
+                "sim = caustics.Lens_Source(\n",
                 "    lens=lens,\n",
                 "    source=base_sersic,\n",
                 "    pixelscale=res,\n",
                 "    pixels_x=n_pix,\n",
                 "    z_s=z_s,\n",
                 "    upsample_factor=2,\n",
                 ")\n",
@@ -107,36 +107,36 @@
                 "axarr[1].axis(\"off\")\n",
                 "axarr[1].set_title(\"Lensed Sersic\")\n",
                 "plt.show()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "2ca96b29",
+            "id": "5",
             "metadata": {},
             "source": [
                 "## Singular Isothermal Sphere (SIS)\n",
                 "\n",
                 "An SIS is a mass distribution represented by a constant temperature velocity dispersion of masses. Alternatively, a constant temperature gas in a spherical gravitational potential."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "6d563d58",
+            "id": "6",
             "metadata": {},
             "outputs": [],
             "source": [
-                "lens = caustics.lenses.SIS(\n",
+                "lens = caustics.SIS(\n",
                 "    cosmology=cosmology,\n",
                 "    x0=0.0,\n",
                 "    y0=0.0,\n",
                 "    th_ein=1.0,\n",
                 ")\n",
-                "sim = caustics.sims.Lens_Source(\n",
+                "sim = caustics.Lens_Source(\n",
                 "    lens=lens,\n",
                 "    source=base_sersic,\n",
                 "    pixelscale=res,\n",
                 "    pixels_x=n_pix,\n",
                 "    z_s=z_s,\n",
                 "    upsample_factor=2,\n",
                 ")\n",
@@ -151,38 +151,38 @@
                 "axarr[1].axis(\"off\")\n",
                 "axarr[1].set_title(\"Lensed Sersic\")\n",
                 "plt.show()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "e09f874d",
+            "id": "7",
             "metadata": {},
             "source": [
                 "## Singular Isothermal Ellipsoid (SIE)\n",
                 "\n",
                 "The SIE is just like the SIS except it has been compressed along one axis."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "63c78c9a",
+            "id": "8",
             "metadata": {},
             "outputs": [],
             "source": [
-                "lens = caustics.lenses.SIE(\n",
+                "lens = caustics.SIE(\n",
                 "    cosmology=cosmology,\n",
                 "    x0=0.0,\n",
                 "    y0=0.0,\n",
                 "    q=0.6,\n",
                 "    phi=np.pi / 2,\n",
                 "    b=1.0,\n",
                 ")\n",
-                "sim = caustics.sims.Lens_Source(\n",
+                "sim = caustics.Lens_Source(\n",
                 "    lens=lens,\n",
                 "    source=base_sersic,\n",
                 "    pixelscale=res,\n",
                 "    pixels_x=n_pix,\n",
                 "    z_s=z_s,\n",
                 "    upsample_factor=2,\n",
                 ")\n",
@@ -197,39 +197,39 @@
                 "axarr[1].axis(\"off\")\n",
                 "axarr[1].set_title(\"Lensed Sersic\")\n",
                 "plt.show()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "794060c3",
+            "id": "9",
             "metadata": {},
             "source": [
                 "## Elliptical Power Law (EPL)\n",
                 "\n",
                 "This is a power law mass distribution with an elliptical isodensity contour."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "557bad9f",
+            "id": "10",
             "metadata": {},
             "outputs": [],
             "source": [
-                "lens = caustics.lenses.EPL(\n",
+                "lens = caustics.EPL(\n",
                 "    cosmology=cosmology,\n",
                 "    x0=0.0,\n",
                 "    y0=0.0,\n",
                 "    q=0.6,\n",
                 "    phi=np.pi / 2,\n",
                 "    b=1.0,\n",
                 "    t=0.5,\n",
                 ")\n",
-                "sim = caustics.sims.Lens_Source(\n",
+                "sim = caustics.Lens_Source(\n",
                 "    lens=lens,\n",
                 "    source=base_sersic,\n",
                 "    pixelscale=res,\n",
                 "    pixels_x=n_pix,\n",
                 "    z_s=z_s,\n",
                 "    upsample_factor=2,\n",
                 ")\n",
@@ -244,39 +244,39 @@
                 "axarr[1].axis(\"off\")\n",
                 "axarr[1].set_title(\"Lensed Sersic\")\n",
                 "plt.show()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "1aa4a0b4",
+            "id": "11",
             "metadata": {},
             "source": [
                 "## Navarro Frenk White profile (NFW)\n",
                 "\n",
                 "The NFW profile is a classic mass profile that approximates the mass distribution of halos in large dark matter simulations.\n",
                 "\n",
                 "$$\\rho(r) = \\frac{\\rho_0}{\\frac{r}{r_s}\\left(1 + \\frac{r}{r_s}\\right)^2}$$"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "bb209aba",
+            "id": "12",
             "metadata": {},
             "outputs": [],
             "source": [
-                "lens = caustics.lenses.NFW(\n",
+                "lens = caustics.NFW(\n",
                 "    cosmology=cosmology,\n",
                 "    x0=0.0,\n",
                 "    y0=0.0,\n",
                 "    m=1e13,\n",
                 "    c=20.0,\n",
                 ")\n",
-                "sim = caustics.sims.Lens_Source(\n",
+                "sim = caustics.Lens_Source(\n",
                 "    lens=lens,\n",
                 "    source=base_sersic,\n",
                 "    pixelscale=res,\n",
                 "    pixels_x=n_pix,\n",
                 "    z_s=z_s,\n",
                 "    upsample_factor=2,\n",
                 ")\n",
@@ -291,42 +291,42 @@
                 "axarr[1].axis(\"off\")\n",
                 "axarr[1].set_title(\"Lensed Sersic\")\n",
                 "plt.show()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "d96d3992",
+            "id": "13",
             "metadata": {},
             "source": [
                 "## Truncated NFW profile (TNFW)\n",
                 "\n",
                 "The TNFW profile is a slight modification to the classic NFW mass profile that approximates the mass distribution of halos in large dark matter simulations. The new density profile is defined as:\n",
                 "\n",
                 "$$\\rho_{\\rm tnfw}(r) =  \\rho_{\\rm nfw}(r)\\frac{\\tau^2}{\\tau^2 + \\frac{r^2}{r_s^2}}$$\n",
                 "\n",
                 "where $\\tau = \\frac{r_t}{r_s}$ is the ratio of the truncation radius to the scale radius. Note that the truncation happens smoothly so there are no sharp boundaries. In the TNFW profile, the mass quantity now actually corresponds the to the total mass since it is no longer divergent. This often means the mass values are larger."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "dd5805a5",
+            "id": "14",
             "metadata": {},
             "outputs": [],
             "source": [
-                "lens = caustics.lenses.TNFW(\n",
+                "lens = caustics.TNFW(\n",
                 "    cosmology=cosmology,\n",
                 "    x0=0.0,\n",
                 "    y0=0.0,\n",
                 "    mass=1e12,\n",
                 "    scale_radius=1.0,\n",
                 "    tau=3.0,\n",
                 ")\n",
-                "sim = caustics.sims.Lens_Source(\n",
+                "sim = caustics.Lens_Source(\n",
                 "    lens=lens,\n",
                 "    source=base_sersic,\n",
                 "    pixelscale=res,\n",
                 "    pixels_x=n_pix,\n",
                 "    z_s=z_s,\n",
                 "    upsample_factor=2,\n",
                 ")\n",
@@ -341,42 +341,42 @@
                 "axarr[1].axis(\"off\")\n",
                 "axarr[1].set_title(\"Lensed Sersic\")\n",
                 "plt.show()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "f6f19942",
+            "id": "15",
             "metadata": {},
             "source": [
                 "## Pseudo Jaffe (PseudoJaffe)\n",
                 "\n",
                 "The Pseudo Jaffe closely approximates an isothermal mass distribution except that it is easier to compute and has finite mass.\n",
                 "\n",
                 "$$ \\rho(r) = \\frac{\\rho_0}{\\left(1 + \\frac{r^2}{r_c^2}\\right)\\left(1 + \\frac{r^2}{r_s^2}\\right)} $$\n",
                 "\n",
                 "where $\\rho_0$ is the central density limit, $r_c$ is the core radius, $r_s$ is the scale radius."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "0c8985d8",
+            "id": "16",
             "metadata": {},
             "outputs": [],
             "source": [
-                "lens = caustics.lenses.PseudoJaffe(\n",
+                "lens = caustics.PseudoJaffe(\n",
                 "    cosmology=cosmology,\n",
                 "    x0=0.0,\n",
                 "    y0=0.0,\n",
                 "    mass=1e13,\n",
                 "    core_radius=5e-1,\n",
                 "    scale_radius=15.0,\n",
                 ")\n",
-                "sim = caustics.sims.Lens_Source(\n",
+                "sim = caustics.Lens_Source(\n",
                 "    lens=lens,\n",
                 "    source=base_sersic,\n",
                 "    pixelscale=res,\n",
                 "    pixels_x=n_pix,\n",
                 "    z_s=z_s,\n",
                 "    upsample_factor=2,\n",
                 ")\n",
@@ -391,37 +391,37 @@
                 "axarr[1].axis(\"off\")\n",
                 "axarr[1].set_title(\"Lensed Sersic\")\n",
                 "plt.show()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "b232c8b0",
+            "id": "17",
             "metadata": {},
             "source": [
                 "## External Shear (ExternalShear)\n",
                 "\n",
                 "It is often necessary to embed a lens in an external shear field to account for the fact that the lensing mass is not the only mass in the universe."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "e1d7b927",
+            "id": "18",
             "metadata": {},
             "outputs": [],
             "source": [
-                "lens = caustics.lenses.ExternalShear(\n",
+                "lens = caustics.ExternalShear(\n",
                 "    cosmology=cosmology,\n",
                 "    x0=0.0,\n",
                 "    y0=0.0,\n",
                 "    gamma_1=1.0,\n",
                 "    gamma_2=-1.0,\n",
                 ")\n",
-                "sim = caustics.sims.Lens_Source(\n",
+                "sim = caustics.Lens_Source(\n",
                 "    lens=lens,\n",
                 "    source=base_sersic,\n",
                 "    pixelscale=res,\n",
                 "    pixels_x=n_pix,\n",
                 "    z_s=z_s,\n",
                 "    upsample_factor=2,\n",
                 ")\n",
@@ -434,36 +434,36 @@
                 "axarr[1].axis(\"off\")\n",
                 "axarr[1].set_title(\"Lensed Sersic\")\n",
                 "plt.show()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "688d0796",
+            "id": "19",
             "metadata": {},
             "source": [
                 "## Mass Sheet (MassSheet)\n",
                 "\n",
                 "This is a simple case of an external shear field which represents an infinite constant surface density sheet."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "cdfba784",
+            "id": "20",
             "metadata": {},
             "outputs": [],
             "source": [
-                "lens = caustics.lenses.MassSheet(\n",
+                "lens = caustics.MassSheet(\n",
                 "    cosmology=cosmology,\n",
                 "    x0=0.0,\n",
                 "    y0=0.0,\n",
                 "    surface_density=1.5,\n",
                 ")\n",
-                "sim = caustics.sims.Lens_Source(\n",
+                "sim = caustics.Lens_Source(\n",
                 "    lens=lens,\n",
                 "    source=base_sersic,\n",
                 "    pixelscale=res,\n",
                 "    pixels_x=n_pix,\n",
                 "    z_s=z_s,\n",
                 "    upsample_factor=2,\n",
                 ")\n",
@@ -479,15 +479,15 @@
                 "axarr[1].set_title(\"Lensed Sersic\")\n",
                 "plt.show()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "d6c44b6c",
+            "id": "21",
             "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
         "language_info": {
```

### Comparing `caustics-0.7.0/docs/source/tutorials/MultiplaneDemo.ipynb` & `caustics-0.8.0/docs/source/tutorials/MultiplaneDemo.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9876244212962964%*

 * *Differences: {"'cells'": "{0: {'id': '0'}, 1: {'id': '1'}, 2: {'id': '2', 'source': {insert: [(1, 'cosmology = "*

 * *            'caustics.FlatLambdaCDM(name="cosmo")\\n\')], delete: [1]}}, 3: {\'id\': \'3\', '*

 * *            "'source': {insert: [(11, '            caustics.SIE(\\n'), (23, '        "*

 * *            'caustics.SinglePlane(\\n\'), (28, \'lens = caustics.Multiplane(name="multiplane", '*

 * *            "cosmology=cosmology, lenses=planes)')], delete: [28, 23, 11]}}, 4: {'id': '4'}, 5: "*

 * *            "{'id': '5'}, 6: {'id':  […]*

```diff
@@ -1,25 +1,25 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
-            "id": "2a324070-a163-4b79-8e77-819da73083f3",
+            "id": "0",
             "metadata": {},
             "source": [
                 "# Multiplane Lensing\n",
                 "\n",
                 "The universe is three dimensional and filled with stuff. A light ray traveling to our telescope may encounter more than a single massive object on its way to our telescopes. This is handled by a multiplane lensing framework. Multiplane lensing involves tracing the path of a ray backwards from our telescope through each individual plane (which is treated similarly to typical single plane lensing, though extra factors account for the ray physically moving in 3D space) getting perturbed at each step until it finally lands on the source we'd like to image. For more mathematical details see [Petkova et al. 2014](https://doi.org/10.1093/mnras/stu1860) for the formalism we use internally.\n",
                 "\n",
                 "The main concept to keep in mind is that a lot of quantities we are used to working with, such as \"reduced deflection angles\" don't really exist in multiplane lensing since these are normalized by the redshift of the source and lens, however there is no single \"lens redshift\" for multiplane! Instead we define everything with respect to results from full raytracing, once the raytracing is done we can define effective quantities (like effective reduced deflection angle) which behave similarly in intuition but are not quite the same in detail."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "45b6a8b4",
+            "id": "1",
             "metadata": {},
             "outputs": [],
             "source": [
                 "%load_ext autoreload\n",
                 "%autoreload 2\n",
                 "\n",
                 "import torch\n",
@@ -31,20 +31,20 @@
                 "\n",
                 "import caustics"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "ab43e042",
+            "id": "2",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# initialization stuff for lenses\n",
-                "cosmology = caustics.cosmology.FlatLambdaCDM(name=\"cosmo\")\n",
+                "cosmology = caustics.FlatLambdaCDM(name=\"cosmo\")\n",
                 "cosmology.to(dtype=torch.float32)\n",
                 "n_pix = 100\n",
                 "res = 0.5\n",
                 "upsample_factor = 2\n",
                 "fov = res * n_pix\n",
                 "thx, thy = caustics.utils.get_meshgrid(\n",
                 "    res / upsample_factor,\n",
@@ -54,61 +54,61 @@
                 ")\n",
                 "z_s = torch.tensor(1.5, dtype=torch.float32)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "ea49d25d",
+            "id": "3",
             "metadata": {},
             "outputs": [],
             "source": [
                 "N_planes = 10\n",
                 "N_lenses = 2  # per plane\n",
                 "\n",
                 "z_plane = np.linspace(0.1, 1.0, N_planes)\n",
                 "planes = []\n",
                 "\n",
                 "for p, z_p in enumerate(z_plane):\n",
                 "    lenses = []\n",
                 "\n",
                 "    for _ in range(N_lenses):\n",
                 "        lenses.append(\n",
-                "            caustics.lenses.SIE(\n",
+                "            caustics.SIE(\n",
                 "                cosmology=cosmology,\n",
                 "                z_l=z_p,\n",
                 "                x0=np.random.uniform(-fov / 4.0, fov / 4.0),\n",
                 "                y0=np.random.uniform(-fov / 4.0, fov / 4.0),\n",
                 "                q=np.random.uniform(0.3, 0.7),\n",
                 "                phi=np.random.uniform(0, np.pi),\n",
                 "                b=np.random.uniform(0.1, 1.5),\n",
                 "            )\n",
                 "        )\n",
                 "\n",
                 "    planes.append(\n",
-                "        caustics.lenses.SinglePlane(\n",
+                "        caustics.SinglePlane(\n",
                 "            z_l=z_p, cosmology=cosmology, lenses=lenses, name=f\"plane_{p}\"\n",
                 "        )\n",
                 "    )\n",
                 "\n",
-                "lens = caustics.lenses.Multiplane(name=\"multiplane\", cosmology=cosmology, lenses=planes)"
+                "lens = caustics.Multiplane(name=\"multiplane\", cosmology=cosmology, lenses=planes)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "4aa429c8",
+            "id": "4",
             "metadata": {},
             "source": [
                 "## Effective Reduced Deflection Angles"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "f2e0a341",
+            "id": "5",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Effective reduced deflection angles for the multiplane lens system\n",
                 "ax, ay = lens.effective_reduced_deflection_angle(thx, thy, z_s)\n",
                 "\n",
                 "# Plot\n",
@@ -124,24 +124,24 @@
                 "axarr[1].set_title(\"Deflection angle Y\")\n",
                 "plt.colorbar(im)\n",
                 "plt.show()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "c7ad98c6",
+            "id": "6",
             "metadata": {},
             "source": [
                 "## Critical Lines"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "b2e23c3e",
+            "id": "7",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Compute critical curves using effective difflection angle\n",
                 "A = lens.jacobian_lens_equation(thx, thy, z_s)\n",
                 "\n",
                 "# Here we compute detA at every point\n",
@@ -158,15 +158,15 @@
                 "plt.title(\"Critical curves\")\n",
                 "plt.show()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "7cd1f948",
+            "id": "8",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# For completeness, here are the caustics!\n",
                 "paths = CS.allsegs[0]\n",
                 "\n",
                 "for path in paths:\n",
@@ -185,77 +185,77 @@
                 "# plt.ylim([-fov/2,fov/2])\n",
                 "plt.title(\"Caustics\")\n",
                 "plt.show()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "94144e25",
+            "id": "9",
             "metadata": {},
             "source": [
                 "## Effective Convergence"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "d8a84fde",
+            "id": "10",
             "metadata": {},
             "outputs": [],
             "source": [
                 "C = lens.effective_convergence_div(thx, thy, z_s)\n",
                 "\n",
                 "plt.imshow(np.log10(C.detach().cpu().numpy()), origin=\"lower\")\n",
                 "plt.colorbar()\n",
                 "plt.title(\"Effective Convergence (log)\")\n",
                 "plt.show()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "708338df",
+            "id": "11",
             "metadata": {},
             "outputs": [],
             "source": [
                 "Curl = lens.effective_convergence_curl(thx, thy, z_s)\n",
                 "\n",
                 "plt.imshow(Curl.detach().cpu().numpy(), origin=\"lower\")\n",
                 "plt.colorbar()\n",
                 "plt.title(\"Curl\")\n",
                 "plt.show()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "d6933714-dbce-4e5a-a92a-cd1a7b4df54e",
+            "id": "12",
             "metadata": {},
             "source": [
                 "## Time Delay"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "9a4c6c28-2dd4-4f96-a4d4-9e5d44f3aa77",
+            "id": "13",
             "metadata": {},
             "outputs": [],
             "source": [
                 "TD = lens.time_delay(thx, thy, z_s)\n",
                 "\n",
                 "plt.imshow(TD.detach().cpu().numpy(), origin=\"lower\")\n",
                 "plt.colorbar()\n",
                 "plt.title(\"Time Delay (seconds)\")\n",
                 "plt.show()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "28cbf540-c3f4-4cfc-8fb8-d7dad1eee028",
+            "id": "14",
             "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
         "language_info": {
```

### Comparing `caustics-0.7.0/docs/source/tutorials/Parameters.ipynb` & `caustics-0.8.0/docs/source/tutorials/Parameters.ipynb`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9874338624338624%*

 * *Differences: {"'cells'": "{0: {'id': '0'}, 1: {'id': '1'}, 2: {'id': '2'}, 3: {'id': '3', 'source': {insert: "*

 * *            '[(1, \'cosmo = caustics.FlatLambdaCDM(name="cosmo", h0=None, Om0=None)\\n\'), (4, '*

 * *            "'lens = caustics.SIE(cosmology=cosmo, q=0.4, b=1.0)\\n'), (7, 'source = "*

 * *            'caustics.Sersic(name="source", n=2.0, Re=1.0, Ie=1.0)\\n\'), (10, \'lens_light = '*

 * *            'caustics.Sersic(name="lenslight", x0=0.0, phi=1.3, Re=1.0)\\n\'), (13, \'sim = '*

 * *            "caustics.Lens_Source(\\n')] […]*

```diff
@@ -1,25 +1,25 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
-            "id": "6527560d-1978-4187-8b40-50867258cb62",
+            "id": "0",
             "metadata": {},
             "source": [
                 "# Parameters\n",
                 "\n",
                 "This notebook will walk you through the various ways to interact with parameters in caustics. For each lens and light model there are certain parameters which are given special priority as these parameters are the ones that would be sampled in a simulator. This allows for taking the machinery of caustics and converting it into a function which can use all the power of pytorch, or other sampling/optimization frameworks. \n",
                 "\n",
                 "Throughout the tutorial, keep in mind that parameters are stored in a directed acyclic graph (DAG). This gives a unique way to access each parameter"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "36b860f4-5675-48a3-a867-f4e1ddaf47ce",
+            "id": "1",
             "metadata": {},
             "outputs": [],
             "source": [
                 "%load_ext autoreload\n",
                 "%autoreload 2\n",
                 "\n",
                 "import torch\n",
@@ -29,93 +29,93 @@
                 "import numpy as np\n",
                 "\n",
                 "import caustics"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "15337194-64a3-4048-9564-1ff1295bf283",
+            "id": "2",
             "metadata": {},
             "source": [
                 "## Setting static/dynamic parameters\n",
                 "\n",
                 "Let's see how we can set static and dynamic parameters. In caustics, a dynamic parameter is one which will be involved in sampling and must be provided on evaluation of a function. A static parameter has a fixed value and so \"disappears\" from the graph so that you don't need to worry about it anymore."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "c9ae5563-6e55-4af3-a20a-cacfd257a2e8",
+            "id": "3",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Flat cosmology with all dynamic parameters\n",
-                "cosmo = caustics.cosmology.FlatLambdaCDM(name=\"cosmo\", h0=None, Om0=None)\n",
+                "cosmo = caustics.FlatLambdaCDM(name=\"cosmo\", h0=None, Om0=None)\n",
                 "\n",
                 "# SIE lens with q and b as static parameters\n",
-                "lens = caustics.lenses.SIE(cosmology=cosmo, q=0.4, b=1.0)\n",
+                "lens = caustics.SIE(cosmology=cosmo, q=0.4, b=1.0)\n",
                 "\n",
                 "# Sersic with all dynamic parameters except the sersic index, effective radius, and effective brightness\n",
-                "source = caustics.light.Sersic(name=\"source\", n=2.0, Re=1.0, Ie=1.0)\n",
+                "source = caustics.Sersic(name=\"source\", n=2.0, Re=1.0, Ie=1.0)\n",
                 "\n",
                 "# Sersic with all dynamic parameters except the x position, position angle, and effective radius\n",
-                "lens_light = caustics.light.Sersic(name=\"lenslight\", x0=0.0, phi=1.3, Re=1.0)\n",
+                "lens_light = caustics.Sersic(name=\"lenslight\", x0=0.0, phi=1.3, Re=1.0)\n",
                 "\n",
                 "# A simulator which captures all these parameters into a single DAG\n",
-                "sim = caustics.sims.Lens_Source(\n",
+                "sim = caustics.Lens_Source(\n",
                 "    lens=lens, source=source, lens_light=lens_light, pixelscale=0.05, pixels_x=100\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "28dea7af-b5fe-468a-bdbf-66fceba75945",
+            "id": "4",
             "metadata": {},
             "source": [
                 "We can have the simulator print a graph of the DAG from it's perspective. Note that the white boxes are dynamic parameters while the grey boxes are static parameters"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "0041971d-0f17-4ee4-9b6a-81bea8c51369",
+            "id": "5",
             "metadata": {},
             "outputs": [],
             "source": [
                 "sim.get_graph(True, True)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "298aa458-e518-424d-af9d-1ce45d55e4f4",
+            "id": "6",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Accessing a parameter and giving it a value will turn it into a static parameter\n",
                 "sim.SIE.phi = 0.4\n",
                 "sim.get_graph(True, True)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "08e6a094-5630-45cd-ab6b-1dbd89b3ebad",
+            "id": "7",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Accessing a parameter and setting it to None will turn it into a dynamic parameter\n",
                 "sim.lenslight.x0 = None\n",
                 "sim.get_graph(True, True)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "3f6bbccd-ae91-444f-a8ac-ec31b1562d78",
+            "id": "8",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# This also gives us the order of parameters for a vector that can be an input to the sim function\n",
                 "x_tens = torch.tensor(\n",
                 "    [\n",
                 "        1.5,  # z_s\n",
@@ -173,26 +173,26 @@
                 "axarr[1].imshow(res_dict, origin=\"lower\")\n",
                 "axarr[1].set_title(\"Simulator from dictionary\")\n",
                 "plt.show()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "f3a1a9db-d825-47e8-96f1-c556f1dbe32c",
+            "id": "9",
             "metadata": {},
             "source": [
                 "## Manual Inputs\n",
                 "\n",
                 "We have now seen the standard `pack` method of passing dynamic parameters to a caustics function/simulator. This is very powerful at scale, but can be tedious to enter by hand while prototyping and doing tests. Now lets see a more manual way to pass parameters to a function. For this lets try getting the exact position of each of the 4 images of the background source."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "5b77bf0e-49dd-424c-8268-cb654297a896",
+            "id": "10",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# First find the position of each of the images\n",
                 "x, y = lens.forward_raytrace(\n",
                 "    torch.tensor(0.0),  # First three arguments are regular function arguments\n",
                 "    torch.tensor(0.0),\n",
@@ -217,15 +217,15 @@
                 "ax.scatter(x.detach().cpu().numpy(), y.detach().cpu().numpy(), color=\"r\")\n",
                 "plt.show()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "064832a0-e59b-4e91-8438-edf1aeff471a",
+            "id": "11",
             "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
         "language_info": {
```

### Comparing `caustics-0.7.0/docs/source/tutorials/Playground.ipynb` & `caustics-0.8.0/docs/source/tutorials/Playground.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9885998480998002%*

 * *Differences: {"'cells'": "{0: {'id': '0'}, 1: {'id': '1'}, 2: {'id': '2', 'source': {insert: [(12, 'cosmology = "*

 * *            'caustics.FlatLambdaCDM(name="cosmo")\\n\')], delete: [12]}}, 3: {\'id\': \'3\', '*

 * *            "'source': {insert: [(4, '    lens = caustics.SIE(\\n')], delete: [4]}}, 4: {'id': "*

 * *            "'4'}, 5: {'id': '5', 'source': {insert: [(15, '    lens = caustics.SIE(\\n'), (24, "*

 * *            "'    source = caustics.Sersic(\\n')], delete: [24, 15]}}, 6: {'id': '6'}, 7: {'id': "*

 * *            "'7'}}"}*

```diff
@@ -1,23 +1,23 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
-            "id": "1fafae89",
+            "id": "0",
             "metadata": {},
             "source": [
                 "# Lensing playground\n",
                 "\n",
                 "This is just a fun notebook where you can interactively change lensing parameters. It is a great way to build some intuition around lensing and make some cool pictures!"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "c0d85608",
+            "id": "1",
             "metadata": {},
             "outputs": [],
             "source": [
                 "%load_ext autoreload\n",
                 "%autoreload 2\n",
                 "\n",
                 "import torch\n",
@@ -29,15 +29,15 @@
                 "\n",
                 "import caustics"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "b1ac7bf7",
+            "id": "2",
             "metadata": {},
             "outputs": [],
             "source": [
                 "n_pix = 100\n",
                 "res = 0.05\n",
                 "upsample_factor = 2\n",
                 "fov = res * n_pix\n",
@@ -45,30 +45,30 @@
                 "    res / upsample_factor,\n",
                 "    upsample_factor * n_pix,\n",
                 "    upsample_factor * n_pix,\n",
                 "    dtype=torch.float32,\n",
                 ")\n",
                 "z_l = torch.tensor(0.5, dtype=torch.float32)\n",
                 "z_s = torch.tensor(1.5, dtype=torch.float32)\n",
-                "cosmology = caustics.cosmology.FlatLambdaCDM(name=\"cosmo\")\n",
+                "cosmology = caustics.FlatLambdaCDM(name=\"cosmo\")\n",
                 "cosmology.to(dtype=torch.float32)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "964a76a6",
+            "id": "3",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# SIE lens model, kappa map, alpha map, magnification, time delay, caustics\n",
                 "\n",
                 "\n",
                 "def plot_lens_metrics(thx0, thy0, q, phi, b):\n",
-                "    lens = caustics.lenses.SIE(\n",
+                "    lens = caustics.SIE(\n",
                 "        cosmology=cosmology,\n",
                 "        z_l=z_l,\n",
                 "        x0=thx0,\n",
                 "        y0=thy0,\n",
                 "        q=q,\n",
                 "        phi=phi,\n",
                 "        b=b,\n",
@@ -103,15 +103,15 @@
                 "    axarr[1][2].set_title(\"deflection angle y\")\n",
                 "    plt.show()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "3b04c973",
+            "id": "4",
             "metadata": {},
             "outputs": [],
             "source": [
                 "p = interact(\n",
                 "    plot_lens_metrics,\n",
                 "    thx0=(-2.5, 2.5, 0.1),\n",
                 "    thy0=(-2.5, 2.5, 0.1),\n",
@@ -120,15 +120,15 @@
                 "    b=(0.1, 2.0, 0.1),\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "dce1edef",
+            "id": "5",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Sersic source, demo lensed source\n",
                 "def plot_lens_distortion(\n",
                 "    x0_lens,\n",
                 "    y0_lens,\n",
@@ -139,24 +139,24 @@
                 "    y0_src,\n",
                 "    q_src,\n",
                 "    phi_src,\n",
                 "    n_src,\n",
                 "    Re_src,\n",
                 "    Ie_src,\n",
                 "):\n",
-                "    lens = caustics.lenses.SIE(\n",
+                "    lens = caustics.SIE(\n",
                 "        cosmology,\n",
                 "        z_l,\n",
                 "        x0=x0_lens,\n",
                 "        y0=y0_lens,\n",
                 "        q=q_lens,\n",
                 "        phi=phi_lens,\n",
                 "        b=b_lens,\n",
                 "    )\n",
-                "    source = caustics.light.Sersic(\n",
+                "    source = caustics.Sersic(\n",
                 "        x0=x0_src,\n",
                 "        y0=y0_src,\n",
                 "        q=q_src,\n",
                 "        phi=phi_src,\n",
                 "        n=n_src,\n",
                 "        Re=Re_src,\n",
                 "        Ie=Ie_src,\n",
@@ -180,15 +180,15 @@
                 "    axarr[2].set_title(\"Sersic lensed\")\n",
                 "    plt.show()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "c03161b9",
+            "id": "6",
             "metadata": {},
             "outputs": [],
             "source": [
                 "p = interact(\n",
                 "    plot_lens_distortion,\n",
                 "    x0_lens=(-2.5, 2.5, 0.1),\n",
                 "    y0_lens=(-2.5, 2.5, 0.1),\n",
@@ -204,15 +204,15 @@
                 "    Ie_src=(0.1, 2.0, 0.1),\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "35336e43",
+            "id": "7",
             "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
         "language_info": {
```

### Comparing `caustics-0.7.0/docs/source/tutorials/Simulators.ipynb` & `caustics-0.8.0/docs/source/tutorials/Simulators.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9877716789259128%*

 * *Differences: {"'cells'": "{0: {'id': '0'}, 1: {'id': '1'}, 2: {'id': '2', 'source': {insert: [(13, 'cosmology = "*

 * *            'caustics.FlatLambdaCDM(name="cosmo")\\n\')], delete: [13]}}, 3: {\'id\': \'3\', '*

 * *            "'source': {insert: [(3, 'class Simple_Sim(caustics.Simulator):\\n')], delete: [3]}}, "*

 * *            "4: {'id': '4', 'source': {insert: [(0, 'sie = caustics.SIE(cosmology, "*

 * *            'name="sie")\\n\'), (1, \'src = caustics.Sersic(name="src")\\n\')], delete: [1, 0]}}, '*

 * *            "5: {'id': '5'}, 6: […]*

```diff
@@ -1,23 +1,23 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
-            "id": "f3ed209f",
+            "id": "0",
             "metadata": {},
             "source": [
                 "# Now you're thinking with Simulators\n",
                 "\n",
                 "At least, you will by the end of the tutorial."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "89275b65",
+            "id": "1",
             "metadata": {},
             "outputs": [],
             "source": [
                 "%load_ext autoreload\n",
                 "%autoreload 2\n",
                 "\n",
                 "import torch\n",
@@ -28,15 +28,15 @@
                 "\n",
                 "import caustics"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "88a9200a",
+            "id": "2",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Specify the image/cosmology parameters\n",
                 "n_pix = 100\n",
                 "res = 0.05\n",
                 "upsample_factor = 2\n",
@@ -45,29 +45,29 @@
                 "    res / upsample_factor,\n",
                 "    upsample_factor * n_pix,\n",
                 "    upsample_factor * n_pix,\n",
                 "    dtype=torch.float32,\n",
                 ")\n",
                 "z_l = torch.tensor(0.5, dtype=torch.float32)\n",
                 "z_s = torch.tensor(1.5, dtype=torch.float32)\n",
-                "cosmology = caustics.cosmology.FlatLambdaCDM(name=\"cosmo\")\n",
+                "cosmology = caustics.FlatLambdaCDM(name=\"cosmo\")\n",
                 "cosmology.to(dtype=torch.float32)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "1665abeb",
+            "id": "3",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# demo simulator with sersic source, SIE lens. then sample some examples. demo the model graph\n",
                 "\n",
                 "\n",
-                "class Simple_Sim(caustics.sims.Simulator):\n",
+                "class Simple_Sim(caustics.Simulator):\n",
                 "    def __init__(\n",
                 "        self,\n",
                 "        lens,\n",
                 "        src,\n",
                 "        z_s=None,\n",
                 "        name: str = \"sim\",\n",
                 "    ):\n",
@@ -91,30 +91,30 @@
                 "        # We return the sampled brightness at each pixel location\n",
                 "        return avg_pool2d(mu_fine.squeeze()[None, None], upsample_factor)[0, 0]"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "0babaead",
+            "id": "4",
             "metadata": {},
             "outputs": [],
             "source": [
-                "sie = caustics.lenses.SIE(cosmology, name=\"sie\")\n",
-                "src = caustics.light.Sersic(name=\"src\")\n",
+                "sie = caustics.SIE(cosmology, name=\"sie\")\n",
+                "src = caustics.Sersic(name=\"src\")\n",
                 "\n",
                 "sim = Simple_Sim(sie, src, torch.tensor(0.8))\n",
                 "\n",
                 "sim.get_graph(True, True)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "e672be73",
+            "id": "5",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Reading the x_keys above we can input the parameters that we would like the simulator to evaluate\n",
                 "x = torch.tensor(\n",
                 "    [\n",
                 "        z_l.item(),  # sie z_l\n",
@@ -134,36 +134,36 @@
                 ")\n",
                 "plt.imshow(sim(x), origin=\"lower\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "fe16052c",
+            "id": "6",
             "metadata": {},
             "outputs": [],
             "source": [
-                "sie = caustics.lenses.SIE(cosmology, name=\"sie\")\n",
+                "sie = caustics.SIE(cosmology, name=\"sie\")\n",
                 "hdu = fits.open(\n",
                 "    \"https://www.legacysurvey.org/viewer/fits-cutout?ra=36.3684&dec=-25.6389&size=250&layer=ls-dr9&pixscale=0.262&bands=r\"\n",
                 ")\n",
                 "image_data = np.array(hdu[0].data, dtype=np.float64)\n",
-                "src = caustics.light.Pixelated(\n",
+                "src = caustics.Pixelated(\n",
                 "    name=\"ESO479_G1\", image=torch.tensor(image_data, dtype=torch.float32)\n",
                 ")\n",
                 "\n",
                 "sim2 = Simple_Sim(sie, src, torch.tensor(0.8))\n",
                 "\n",
                 "sim2.get_graph(True, True)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "b9921f68",
+            "id": "7",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# x can also be a dict\n",
                 "x = torch.tensor(\n",
                 "    [\n",
                 "        z_l.item(),  # sie z_l\n",
@@ -183,51 +183,51 @@
                 "axarr[1].imshow(sim2(x), origin=\"lower\")\n",
                 "axarr[1].set_title(\"Lensed image\")\n",
                 "plt.show()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "e16ca698",
+            "id": "8",
             "metadata": {},
             "source": [
                 "## Setting static/dynamic parameters\n",
                 "\n",
                 "So far we have assumed that all parameters for the source and lens are being modelled. However, it is often the case that a parameter can/must be fixed for a given science case. It is very easy to do this in Caustic, simply pass the fixed value when constructing the lens/source objects.\n",
                 "\n",
                 "Below we have fixed some parameters in our simulator by providing them when constructing the objects. In the graph they now appear as greyed boxes. In fact we can see now that the cosmology object `FlatLambdaCDM` had fixed parameters all along. This is because there are natural default parameters for such a cosmology. It is possible, of course, to make a different cosmology object which has alternate values, or which leaves some values as free parameters.\n",
                 "\n",
                 "In general, to set a parameter as dynamic (must be passed to the simulator) just set it to `None`, to fix a parameter give it a value."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "91d3cf26",
+            "id": "9",
             "metadata": {},
             "outputs": [],
             "source": [
-                "sief = caustics.lenses.SIE(\n",
+                "sief = caustics.SIE(\n",
                 "    name=\"sie\",\n",
                 "    cosmology=cosmology,\n",
                 "    z_l=torch.tensor(0.5),\n",
                 "    x0=torch.tensor(0.0),\n",
                 "    y0=torch.tensor(0.0),\n",
                 ")\n",
-                "srcf = caustics.light.Sersic(name=\"src\", n=torch.tensor(2.0))\n",
+                "srcf = caustics.Sersic(name=\"src\", n=torch.tensor(2.0))\n",
                 "\n",
                 "simf = Simple_Sim(sief, srcf, z_s=torch.tensor(0.8))\n",
                 "\n",
                 "simf.get_graph(True, True)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "6b029159",
+            "id": "10",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Reading the x_keys above we can input the parameters that we would like the simulator to evaluate\n",
                 "x = torch.tensor(\n",
                 "    [\n",
                 "        0.4,  # sie q\n",
@@ -243,23 +243,23 @@
                 ")\n",
                 "plt.imshow(simf(x), origin=\"lower\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "6e244b74",
+            "id": "11",
             "metadata": {},
             "outputs": [],
             "source": []
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "fb6619ec-9057-4daa-916b-9384b74a5e29",
+            "id": "12",
             "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
         "language_info": {
```

### Comparing `caustics-0.7.0/docs/source/tutorials/VisualizeCaustics.ipynb` & `caustics-0.8.0/docs/source/tutorials/VisualizeCaustics.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9874565972222222%*

 * *Differences: {"'cells'": "{0: {'id': '0'}, 1: {'id': '1'}, 2: {'id': '2', 'source': {insert: [(2, 'cosmology = "*

 * *            'caustics.FlatLambdaCDM(name="cosmo")\\n\'), (4, \'sie = caustics.SIE(cosmology, '*

 * *            'name="sie")\\n\')], delete: [4, 2]}}, 3: {\'id\': \'3\'}, 4: {\'id\': \'4\'}, 5: '*

 * *            "{'id': '5'}, 6: {'id': '6'}, 7: {'id': '7'}}"}*

```diff
@@ -1,25 +1,25 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
-            "id": "3bb2cd70-e98d-4e8d-b195-64d7e5de6e13",
+            "id": "0",
             "metadata": {},
             "source": [
                 "# Visualize Caustics\n",
                 "\n",
                 "Here we will demonstrate how to collect caustic lines using caustic! Since caustic (the code) uses autodiff and can get exact derivatives, it is actually very accurate at computing caustics. \n",
                 "\n",
                 "Conceptually a caustic occurs where the magnification of a lens diverges to infinity. A convenient way to measure the magnification in the image plane is by taking the determinant ($det$) of the jacobian of the lens equation ($A$), its reciprocal is the magnification. This means that anywhere that $det(A) = 0$ is a critical line in the image plane (magnification goes to infinity). If we take this line and raytrace it back to the source plane we can see the caustics which define boundaries for lensing phenomena."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "f716feef",
+            "id": "1",
             "metadata": {},
             "outputs": [],
             "source": [
                 "%load_ext autoreload\n",
                 "%autoreload 2\n",
                 "\n",
                 "import torch\n",
@@ -32,23 +32,23 @@
                 "\n",
                 "import caustics"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "bdede2df",
+            "id": "2",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# initialization stuff for an SIE lens\n",
                 "\n",
-                "cosmology = caustics.cosmology.FlatLambdaCDM(name=\"cosmo\")\n",
+                "cosmology = caustics.FlatLambdaCDM(name=\"cosmo\")\n",
                 "cosmology.to(dtype=torch.float32)\n",
-                "sie = caustics.lenses.SIE(cosmology, name=\"sie\")\n",
+                "sie = caustics.SIE(cosmology, name=\"sie\")\n",
                 "n_pix = 100\n",
                 "res = 0.05\n",
                 "upsample_factor = 2\n",
                 "fov = res * n_pix\n",
                 "thx, thy = caustics.utils.get_meshgrid(\n",
                 "    res / upsample_factor,\n",
                 "    upsample_factor * n_pix,\n",
@@ -68,26 +68,26 @@
                 "    ]\n",
                 ")\n",
                 "packparams = sie.pack(x)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "38dd09e3",
+            "id": "3",
             "metadata": {},
             "source": [
                 "## Critical Lines\n",
                 "\n",
                 "Before we can see the caustics, we need to find the critical lines. The critical lines are the locus of points in the lens plane (the plane of the mass causing the lensing) at which the magnification of the source becomes theoretically infinite for a point source. In simpler terms, it is where the lensing effect becomes so strong that it can create highly magnified and distorted images of the source. The shape and size of the critical curve depend on the distribution of mass in the lensing object. These lines can be found using the Jacobian of the lensing deflection, specifically $A = \\mathbb{I} - J$. When ${\\rm det}(A) = 0$, that point is on the critical line. Interestingly, $\\frac{1}{{\\rm det}(A)}$ is the magnification, which is why ${\\rm det}(A) = 0$ defines the points of infinite magnification."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "487b3030",
+            "id": "4",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Conveniently caustic has a function to compute the jacobian of the lens equation\n",
                 "A = sie.jacobian_lens_equation(thx, thy, z_s, packparams)\n",
                 "# Note that if this is too slow you can set `method = \"finitediff\"` to run a faster version. You will also need to provide `pixelscale` then\n",
                 "\n",
@@ -102,26 +102,26 @@
                 "CS = plt.contour(thx, thy, detA, levels=[0.0], colors=\"b\")\n",
                 "\n",
                 "plt.show()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "3b099cfd",
+            "id": "5",
             "metadata": {},
             "source": [
                 "## Caustics\n",
                 "\n",
                 "Critical lines show us where the magnification approaches infinity, they are important structures in understanding a lensing system. These lines are also very useful when mapped into the source plane. When the critical lines are raytraced back to the source plane they are called caustics (see what we did there?). In the source plane these lines deliniate when a source will be multiply imaged. "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "0c1f1177",
+            "id": "6",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Get the path from the matplotlib contour plot of the critical line\n",
                 "paths = CS.allsegs[0]\n",
                 "\n",
                 "for path in paths:\n",
@@ -135,15 +135,15 @@
                 "    plt.plot(y1, y2)\n",
                 "plt.show()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "1e77da2e",
+            "id": "7",
             "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
         "language_info": {
```

### Comparing `caustics-0.7.0/media/caustics_favicon.ico` & `caustics-0.8.0/media/caustics_favicon.ico`

 * *Files identical despite different names*

### Comparing `caustics-0.7.0/media/caustics_logo.png` & `caustics-0.8.0/media/caustics_logo.png`

 * *Files identical despite different names*

### Comparing `caustics-0.7.0/media/caustics_logo_white.png` & `caustics-0.8.0/media/caustics_logo_white.png`

 * *Files identical despite different names*

### Comparing `caustics-0.7.0/media/minimal_example.png` & `caustics-0.8.0/media/minimal_example.png`

 * *Files identical despite different names*

### Comparing `caustics-0.7.0/media/minisim_jacobian.png` & `caustics-0.8.0/media/minisim_jacobian.png`

 * *Files identical despite different names*

### Comparing `caustics-0.7.0/media/minisim_vmap.png` & `caustics-0.8.0/media/minisim_vmap.png`

 * *Files identical despite different names*

### Comparing `caustics-0.7.0/src/caustics/constants.py` & `caustics-0.8.0/src/caustics/constants.py`

 * *Files identical despite different names*

### Comparing `caustics-0.7.0/src/caustics/namespace_dict.py` & `caustics-0.8.0/src/caustics/namespace_dict.py`

 * *Files identical despite different names*

### Comparing `caustics-0.7.0/src/caustics/parameter.py` & `caustics-0.8.0/src/caustics/parameter.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# mypy: disable-error-code="union-attr"
 from typing import Optional, Union
 
 import torch
 from torch import Tensor
 
 __all__ = ("Parameter",)
```

### Comparing `caustics-0.7.0/src/caustics/parametrized.py` & `caustics-0.8.0/src/caustics/parametrized.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# mypy: disable-error-code="var-annotated,index,type-arg"
 from collections import OrderedDict
 from math import prod
 from typing import Optional, Union
 import functools
 import inspect
 
 import torch
@@ -55,15 +56,15 @@
         Size of dynamic parameters.
     n_dynamic: int
         Number of dynamic parameters.
     n_static: int
         Number of static parameters.
     """
 
-    def __init__(self, name: str = None):
+    def __init__(self, name: Optional[str] = None):
         if name is None:
             name = self._default_name()
         check_valid_name(name)
         if not isinstance(name, str):
             raise ValueError(f"name must be a string (received {name})")
         self._name = name
         self._parents: OrderedDict[str, Parametrized] = NamespaceDict()
```

### Comparing `caustics-0.7.0/src/caustics/tests.py` & `caustics-0.8.0/src/caustics/tests.py`

 * *Files identical despite different names*

### Comparing `caustics-0.7.0/src/caustics/utils.py` & `caustics-0.8.0/src/caustics/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# mypy: disable-error-code="misc"
 from math import pi
 from typing import Callable, Optional, Tuple, Union
 from functools import partial, lru_cache
 
 import torch
 from torch import Tensor
 from torch.func import jacfwd
```

### Comparing `caustics-0.7.0/src/caustics/data/hdf5dataset.py` & `caustics-0.8.0/src/caustics/data/hdf5dataset.py`

 * *Files identical despite different names*

### Comparing `caustics-0.7.0/src/caustics/data/illustris_kappa.py` & `caustics-0.8.0/src/caustics/data/illustris_kappa.py`

 * *Files identical despite different names*

### Comparing `caustics-0.7.0/src/caustics/data/probes.py` & `caustics-0.8.0/src/caustics/data/probes.py`

 * *Files identical despite different names*

### Comparing `caustics-0.7.0/src/caustics/lenses/__init__.py` & `caustics-0.8.0/src/caustics/lenses/__init__.py`

 * *Files identical despite different names*

### Comparing `caustics-0.7.0/src/caustics/lenses/base.py` & `caustics-0.8.0/src/caustics/lenses/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# mypy: disable-error-code="call-overload"
 from abc import abstractmethod
 from typing import Optional, Union
 from functools import partial
 import warnings
 
 import torch
 from torch import Tensor
@@ -17,15 +18,15 @@
 
 
 class Lens(Parametrized):
     """
     Base class for all lenses
     """
 
-    def __init__(self, cosmology: Cosmology, name: str = None):
+    def __init__(self, cosmology: Cosmology, name: Optional[str] = None):
         """
         Initializes a new instance of the Lens class.
 
         Parameters
         ----------
         name: string
             The name of the lens model.
@@ -95,17 +96,15 @@
             Dynamic parameter container for the lens model. Defaults to None.
 
         Returns
         -------
         Tensor
             Gravitational magnification at the given coordinates.
         """
-        return get_magnification(
-            partial(self.raytrace, params=params), x, y, z_s, **kwargs
-        )
+        return get_magnification(partial(self.raytrace, params=params), x, y, z_s)
 
     @unpack
     def forward_raytrace(
         self,
         bx: Tensor,
         by: Tensor,
         z_s: Tensor,
@@ -513,15 +512,15 @@
         Return the jacobian of the lensing equation at specified points.
         This equates to a (2,2) matrix at each (x,y) point.
         """
         # Build Jacobian
         J = self._jacobian_effective_deflection_angle_finitediff(
             x, y, z_s, pixelscale, params, **kwargs
         )
-        return torch.eye(2) - J
+        return torch.eye(2).to(J.device) - J
 
     @unpack
     def _jacobian_lens_equation_autograd(
         self,
         x: Tensor,
         y: Tensor,
         z_s: Tensor,
@@ -533,15 +532,15 @@
         Return the jacobian of the lensing equation at specified points.
         This equates to a (2,2) matrix at each (x,y) point.
         """
         # Build Jacobian
         J = self._jacobian_effective_deflection_angle_autograd(
             x, y, z_s, params, **kwargs
         )
-        return torch.eye(2) - J.detach()
+        return torch.eye(2).to(J.device) - J.detach()
 
     @unpack
     def effective_convergence_div(
         self,
         x: Tensor,
         y: Tensor,
         z_s: Tensor,
@@ -605,28 +604,28 @@
 
     """
 
     def __init__(
         self,
         cosmology: Cosmology,
         z_l: Optional[Union[Tensor, float]] = None,
-        name: str = None,
+        name: Optional[str] = None,
     ):
         super().__init__(cosmology=cosmology, name=name)
         self.add_param("z_l", z_l)
 
     @unpack
     def reduced_deflection_angle(
         self,
         x: Tensor,
         y: Tensor,
         z_s: Tensor,
         *args,
         params: Optional["Packed"] = None,
-        z_l: Tensor = None,
+        z_l: Optional[Tensor] = None,
         **kwargs,
     ) -> tuple[Tensor, Tensor]:
         """
         Computes the reduced deflection angle of the lens at given coordinates [arcsec].
 
         Parameters
         ----------
@@ -658,15 +657,15 @@
     def physical_deflection_angle(
         self,
         x: Tensor,
         y: Tensor,
         z_s: Tensor,
         *args,
         params: Optional["Packed"] = None,
-        z_l: Tensor = None,
+        z_l: Optional[Tensor] = None,
         **kwargs,
     ) -> tuple[Tensor, Tensor]:
         """
         Computes the physical deflection angle immediately after passing through this lens's plane.
 
         Parameters
         ----------
@@ -762,15 +761,15 @@
     def surface_density(
         self,
         x: Tensor,
         y: Tensor,
         z_s: Tensor,
         *args,
         params: Optional["Packed"] = None,
-        z_l: Tensor = None,
+        z_l: Optional[Tensor] = None,
         **kwargs,
     ) -> Tensor:
         """
         Computes the surface mass density of the lens at given coordinates.
 
         Parameters
         ----------
@@ -840,15 +839,15 @@
     def time_delay(
         self,
         x: Tensor,
         y: Tensor,
         z_s: Tensor,
         *args,
         params: Optional["Packed"] = None,
-        z_l: Tensor = None,
+        z_l: Optional[Tensor] = None,
         shapiro_time_delay: bool = True,
         geometric_time_delay: bool = True,
         **kwargs,
     ) -> Tensor:
         """
         Computes the gravitational time delay for light passing through the lens at given coordinates.
 
@@ -1013,15 +1012,15 @@
         Return the jacobian of the lensing equation at specified points.
         This equates to a (2,2) matrix at each (x,y) point.
         """
         # Build Jacobian
         J = self._jacobian_deflection_angle_finitediff(
             x, y, z_s, pixelscale, params, **kwargs
         )
-        return torch.eye(2) - J
+        return torch.eye(2).to(J.device) - J
 
     @unpack
     def _jacobian_lens_equation_autograd(
         self,
         x: Tensor,
         y: Tensor,
         z_s: Tensor,
@@ -1031,8 +1030,8 @@
     ) -> tuple[tuple[Tensor, Tensor], tuple[Tensor, Tensor]]:
         """
         Return the jacobian of the lensing equation at specified points.
         This equates to a (2,2) matrix at each (x,y) point.
         """
         # Build Jacobian
         J = self._jacobian_deflection_angle_autograd(x, y, z_s, params, **kwargs)
-        return torch.eye(2) - J.detach()
+        return torch.eye(2).to(J.device) - J.detach()
```

### Comparing `caustics-0.7.0/src/caustics/lenses/epl.py` & `caustics-0.8.0/src/caustics/lenses/epl.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# mypy: disable-error-code="operator"
 from typing import Optional, Union
 
 import torch
 from torch import Tensor
 
 from ..cosmology import Cosmology
 from ..utils import derotate, translate_rotate
@@ -76,15 +77,15 @@
         y0: Optional[Union[Tensor, float]] = None,
         q: Optional[Union[Tensor, float]] = None,
         phi: Optional[Union[Tensor, float]] = None,
         b: Optional[Union[Tensor, float]] = None,
         t: Optional[Union[Tensor, float]] = None,
         s: float = 0.0,
         n_iter: int = 18,
-        name: str = None,
+        name: Optional[str] = None,
     ):
         """
         Initialize an EPL lens model.
 
         Parameters
         -----------
         name: string
@@ -133,21 +134,21 @@
     def reduced_deflection_angle(
         self,
         x: Tensor,
         y: Tensor,
         z_s: Tensor,
         *args,
         params: Optional["Packed"] = None,
-        z_l: Tensor = None,
-        x0: Tensor = None,
-        y0: Tensor = None,
-        q: Tensor = None,
-        phi: Tensor = None,
-        b: Tensor = None,
-        t: Tensor = None,
+        z_l: Optional[Tensor] = None,
+        x0: Optional[Tensor] = None,
+        y0: Optional[Tensor] = None,
+        q: Optional[Tensor] = None,
+        phi: Optional[Tensor] = None,
+        b: Optional[Tensor] = None,
+        t: Optional[Tensor] = None,
         **kwargs,
     ) -> tuple[Tensor, Tensor]:
         """
         Compute the reduced deflection angles of the lens.
 
         Parameters
         ----------
@@ -216,21 +217,21 @@
     def potential(
         self,
         x: Tensor,
         y: Tensor,
         z_s: Tensor,
         *args,
         params: Optional["Packed"] = None,
-        z_l: Tensor = None,
-        x0: Tensor = None,
-        y0: Tensor = None,
-        q: Tensor = None,
-        phi: Tensor = None,
-        b: Tensor = None,
-        t: Tensor = None,
+        z_l: Optional[Tensor] = None,
+        x0: Optional[Tensor] = None,
+        y0: Optional[Tensor] = None,
+        q: Optional[Tensor] = None,
+        phi: Optional[Tensor] = None,
+        b: Optional[Tensor] = None,
+        t: Optional[Tensor] = None,
         **kwargs,
     ):
         """
         Compute the lensing potential of the lens.
 
         Parameters
         ----------
@@ -247,33 +248,33 @@
         -------
         Tensor
             The lensing potential.
         """
         ax, ay = self.reduced_deflection_angle(x, y, z_s, params)
         ax, ay = derotate(ax, ay, -phi)
         x, y = translate_rotate(x, y, x0, y0, phi)
-        return (x * ax + y * ay) / (2 - t)
+        return (x * ax + y * ay) / (2 - t)  # fmt: skip
 
     @unpack
     def convergence(
         self,
         x: Tensor,
         y: Tensor,
         z_s: Tensor,
         *args,
         params: Optional["Packed"] = None,
-        z_l: Tensor = None,
-        x0: Tensor = None,
-        y0: Tensor = None,
-        q: Tensor = None,
-        phi: Tensor = None,
-        b: Tensor = None,
-        t: Tensor = None,
+        z_l: Optional[Tensor] = None,
+        x0: Optional[Tensor] = None,
+        y0: Optional[Tensor] = None,
+        q: Optional[Tensor] = None,
+        phi: Optional[Tensor] = None,
+        b: Optional[Tensor] = None,
+        t: Optional[Tensor] = None,
         **kwargs,
-    ):
+    ) -> Tensor:
         """
         Compute the convergence of the lens, which describes the local density of the lens.
 
         Parameters
         ----------
         x: Tensor
             X coordinates in the lens plane.
```

### Comparing `caustics-0.7.0/src/caustics/lenses/external_shear.py` & `caustics-0.8.0/src/caustics/lenses/external_shear.py`

 * *Files 20% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         cosmology: Cosmology,
         z_l: Optional[Union[Tensor, float]] = None,
         x0: Optional[Union[Tensor, float]] = None,
         y0: Optional[Union[Tensor, float]] = None,
         gamma_1: Optional[Union[Tensor, float]] = None,
         gamma_2: Optional[Union[Tensor, float]] = None,
         s: float = 0.0,
-        name: str = None,
+        name: Optional[str] = None,
     ):
         super().__init__(cosmology, z_l, name=name)
 
         self.add_param("x0", x0)
         self.add_param("y0", y0)
         self.add_param("gamma_1", gamma_1)
         self.add_param("gamma_2", gamma_2)
@@ -64,19 +64,19 @@
     def reduced_deflection_angle(
         self,
         x: Tensor,
         y: Tensor,
         z_s: Tensor,
         *args,
         params: Optional["Packed"] = None,
-        z_l: Tensor = None,
-        x0: Tensor = None,
-        y0: Tensor = None,
-        gamma_1: Tensor = None,
-        gamma_2: Tensor = None,
+        z_l: Optional[Tensor] = None,
+        x0: Optional[Tensor] = None,
+        y0: Optional[Tensor] = None,
+        gamma_1: Optional[Tensor] = None,
+        gamma_2: Optional[Tensor] = None,
         **kwargs,
     ) -> tuple[Tensor, Tensor]:
         """
         Calculates the reduced deflection angle.
 
         Parameters
         ----------
@@ -109,19 +109,19 @@
     def potential(
         self,
         x: Tensor,
         y: Tensor,
         z_s: Tensor,
         *args,
         params: Optional["Packed"] = None,
-        z_l: Tensor = None,
-        x0: Tensor = None,
-        y0: Tensor = None,
-        gamma_1: Tensor = None,
-        gamma_2: Tensor = None,
+        z_l: Optional[Tensor] = None,
+        x0: Optional[Tensor] = None,
+        y0: Optional[Tensor] = None,
+        gamma_1: Optional[Tensor] = None,
+        gamma_2: Optional[Tensor] = None,
         **kwargs,
     ) -> Tensor:
         """
         Calculates the lensing potential.
 
         Parameters
         ----------
@@ -147,19 +147,19 @@
     def convergence(
         self,
         x: Tensor,
         y: Tensor,
         z_s: Tensor,
         *args,
         params: Optional["Packed"] = None,
-        z_l: Tensor = None,
-        x0: Tensor = None,
-        y0: Tensor = None,
-        gamma_1: Tensor = None,
-        gamma_2: Tensor = None,
+        z_l: Optional[Tensor] = None,
+        x0: Optional[Tensor] = None,
+        y0: Optional[Tensor] = None,
+        gamma_1: Optional[Tensor] = None,
+        gamma_2: Optional[Tensor] = None,
         **kwargs,
     ) -> Tensor:
         """
         The convergence is undefined for an external shear.
 
         Parameters
         ----------
```

### Comparing `caustics-0.7.0/src/caustics/lenses/mass_sheet.py` & `caustics-0.8.0/src/caustics/lenses/sis.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,130 +1,174 @@
+# mypy: disable-error-code="operator"
 from typing import Optional, Union
 
-import torch
 from torch import Tensor
 
 from ..cosmology import Cosmology
 from ..utils import translate_rotate
 from .base import ThinLens
 from ..parametrized import unpack
 from ..packed import Packed
 
-__all__ = ("MassSheet",)
+__all__ = ("SIS",)
 
 
-class MassSheet(ThinLens):
+class SIS(ThinLens):
     """
-    Represents an external shear effect in a gravitational lensing system.
+    A class representing the Singular Isothermal Sphere (SIS) model.
+    This model inherits from the base `ThinLens` class.
 
     Attributes
     ----------
-    name: string
-        Identifier for the lens instance.
+    name: str
+        The name of the SIS lens.
     cosmology: Cosmology
-        The cosmological model used for lensing calculations.
+        An instance of the Cosmology class.
     z_l: Optional[Union[Tensor, float]]
-        The redshift of the lens.
-    x0, y0: Optional[Union[Tensor, float]]
-        Coordinates of the shear center in the lens plane.
-    gamma_1, gamma_2: Optional[Union[Tensor, float]]
-        Shear components.
-
-    Notes
-    ------
-    The shear components gamma_1 and gamma_2 represent an external shear, a gravitational
-    distortion that can be caused by nearby structures outside of the main lens galaxy.
+        The lens redshift.
+    x0: Optional[Union[Tensor, float]]
+        The x-coordinate of the lens center.
+    y0: Optional[Union[Tensor, float]]
+        The y-coordinate of the lens center.
+        th_ein (Optional[Union[Tensor, float]]): The Einstein radius of the lens.
+    s: float
+        A smoothing factor, default is 0.0.
     """
 
     _null_params = {
         "x0": 0.0,
         "y0": 0.0,
-        "surface_density": 0.1,
+        "th_ein": 1.0,
     }
 
     def __init__(
         self,
         cosmology: Cosmology,
         z_l: Optional[Union[Tensor, float]] = None,
         x0: Optional[Union[Tensor, float]] = None,
         y0: Optional[Union[Tensor, float]] = None,
-        surface_density: Optional[Union[Tensor, float]] = None,
-        name: str = None,
+        th_ein: Optional[Union[Tensor, float]] = None,
+        s: float = 0.0,
+        name: Optional[str] = None,
     ):
+        """
+        Initialize the SIS lens model.
+        """
         super().__init__(cosmology, z_l, name=name)
 
         self.add_param("x0", x0)
         self.add_param("y0", y0)
-        self.add_param("surface_density", surface_density)
+        self.add_param("th_ein", th_ein)
+        self.s = s
 
     @unpack
     def reduced_deflection_angle(
         self,
         x: Tensor,
         y: Tensor,
         z_s: Tensor,
         *args,
         params: Optional["Packed"] = None,
-        z_l: Tensor = None,
-        x0: Tensor = None,
-        y0: Tensor = None,
-        surface_density: Tensor = None,
+        z_l: Optional[Tensor] = None,
+        x0: Optional[Tensor] = None,
+        y0: Optional[Tensor] = None,
+        th_ein: Optional[Tensor] = None,
         **kwargs,
     ) -> tuple[Tensor, Tensor]:
         """
-        Calculates the reduced deflection angle.
+        Calculate the deflection angle of the SIS lens.
 
         Parameters
         ----------
         x: Tensor
-            x-coordinates in the lens plane.
+            The x-coordinate of the lens.
         y: Tensor
-            y-coordinates in the lens plane.
+            The y-coordinate of the lens.
         z_s: Tensor
-            Redshifts of the sources.
+            The source redshift.
         params: (Packed, optional)
             Dynamic parameter container.
 
         Returns
         -------
-        tuple[Tensor, Tensor]
-            The reduced deflection angles in the x and y directions.
+        Tuple[Tensor, Tensor]
+            The deflection angle in the x and y directions.
         """
         x, y = translate_rotate(x, y, x0, y0)
-        # Meneghetti eq 3.84
-        ax = x * surface_density
-        ay = y * surface_density
+        R = (x**2 + y**2).sqrt() + self.s
+        ax = th_ein * x / R
+        ay = th_ein * y / R
         return ax, ay
 
     @unpack
     def potential(
         self,
         x: Tensor,
         y: Tensor,
         z_s: Tensor,
         *args,
         params: Optional["Packed"] = None,
-        z_l: Tensor = None,
-        x0: Tensor = None,
-        y0: Tensor = None,
-        surface_density: Tensor = None,
+        z_l: Optional[Tensor] = None,
+        x0: Optional[Tensor] = None,
+        y0: Optional[Tensor] = None,
+        th_ein: Optional[Tensor] = None,
         **kwargs,
     ) -> Tensor:
-        # Meneghetti eq 3.81
-        return surface_density * 0.5 * (x**2 + y**2)  # fmt: skip
+        """
+        Compute the lensing potential of the SIS lens.
+
+        Parameters
+        ----------
+        x: Tensor
+            The x-coordinate of the lens.
+        y: Tensor
+            The y-coordinate of the lens.
+        z_s: Tensor
+            The source redshift.
+        params: (Packed, optional)
+            Dynamic parameter container.
+
+        Returns
+        -------
+        Tensor
+            The lensing potential.
+        """
+        x, y = translate_rotate(x, y, x0, y0)
+        th = (x**2 + y**2).sqrt() + self.s
+        return th_ein * th
 
     @unpack
     def convergence(
         self,
         x: Tensor,
         y: Tensor,
         z_s: Tensor,
         *args,
         params: Optional["Packed"] = None,
-        z_l: Tensor = None,
-        x0: Tensor = None,
-        y0: Tensor = None,
-        surface_density: Tensor = None,
+        z_l: Optional[Tensor] = None,
+        x0: Optional[Tensor] = None,
+        y0: Optional[Tensor] = None,
+        th_ein: Optional[Tensor] = None,
         **kwargs,
     ) -> Tensor:
-        # Essentially by definition
-        return surface_density * torch.ones_like(x)
+        """
+        Calculate the projected mass density of the SIS lens.
+
+        Parameters
+        ----------
+        x: Tensor
+            The x-coordinate of the lens.
+        y: Tensor
+            The y-coordinate of the lens.
+        z_s: Tensor
+            The source redshift.
+        params: (Packed, optional)
+            Dynamic parameter container.
+
+        Returns
+        -------
+        Tensor
+            The projected mass density.
+        """
+        x, y = translate_rotate(x, y, x0, y0)
+        th = (x**2 + y**2).sqrt() + self.s
+        return 0.5 * th_ein / th
```

### Comparing `caustics-0.7.0/src/caustics/lenses/multiplane.py` & `caustics-0.8.0/src/caustics/lenses/multiplane.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,17 @@
         Name of the lens.
     cosmology: Cosmology
         Cosmological parameters used for calculations.
     lenses: list[ThinLens]
         List of thin lenses.
     """
 
-    def __init__(self, cosmology: Cosmology, lenses: list[ThinLens], name: str = None):
+    def __init__(
+        self, cosmology: Cosmology, lenses: list[ThinLens], name: Optional[str] = None
+    ):
         super().__init__(cosmology, name=name)
         self.lenses = lenses
         for lens in lenses:
             self.add_parametrized(lens)
 
     @unpack
     def get_z_ls(
@@ -114,17 +116,15 @@
             if shapiro_time_delay:
                 beta_ij = D * D_s / (D_next * D_is)
                 potential = self.lenses[i].potential(
                     X * rad_to_arcsec / D_l, Y * rad_to_arcsec / D_l, z_s, params
                 )
                 TD += (-tau_ij * beta_ij * arcsec_to_rad**2) * potential
             if geometric_time_delay:
-                TD += (tau_ij * arcsec_to_rad**2 * 0.5) * (
-                    alpha_x**2 + alpha_y**2
-                )
+                TD += (tau_ij * arcsec_to_rad**2 * 0.5) * (alpha_x**2 + alpha_y**2)
 
             # Propagate rays to next plane (basically eq 18)
             X = X + D * theta_x * arcsec_to_rad
             Y = Y + D * theta_y * arcsec_to_rad
 
         # Convert from physical position to angular position on the source plane
         D_end = self.cosmology.transverse_comoving_distance(z_s, params)
```

### Comparing `caustics-0.7.0/src/caustics/lenses/nfw.py` & `caustics-0.8.0/src/caustics/lenses/nfw.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# mypy: disable-error-code="operator,union-attr"
 from math import pi
 from typing import Optional, Union
 
 import torch
 from torch import Tensor
 
 from ..constants import G_over_c2, arcsec_to_rad, rad_to_arcsec
@@ -78,15 +79,15 @@
         z_l: Optional[Union[Tensor, float]] = None,
         x0: Optional[Union[Tensor, float]] = None,
         y0: Optional[Union[Tensor, float]] = None,
         m: Optional[Union[Tensor, float]] = None,
         c: Optional[Union[Tensor, float]] = None,
         s: float = 0.0,
         use_case="batchable",
-        name: str = None,
+        name: Optional[str] = None,
     ):
         """
         Initialize an instance of the NFW lens class.
 
         Parameters
         ----------
         name: str
@@ -129,19 +130,19 @@
             raise ValueError("use case should be one of: batchable, differentiable")
 
     @unpack
     def get_scale_radius(
         self,
         *args,
         params: Optional["Packed"] = None,
-        z_l: Tensor = None,
-        x0: Tensor = None,
-        y0: Tensor = None,
-        m: Tensor = None,
-        c: Tensor = None,
+        z_l: Optional[Tensor] = None,
+        x0: Optional[Tensor] = None,
+        y0: Optional[Tensor] = None,
+        m: Optional[Tensor] = None,
+        c: Optional[Tensor] = None,
         **kwargs,
     ) -> Tensor:
         """
         Calculate the scale radius of the lens.
 
         Parameters
         ----------
@@ -164,19 +165,19 @@
         return 1 / c * r_delta
 
     @unpack
     def get_scale_density(
         self,
         *args,
         params: Optional["Packed"] = None,
-        z_l: Tensor = None,
-        x0: Tensor = None,
-        y0: Tensor = None,
-        m: Tensor = None,
-        c: Tensor = None,
+        z_l: Optional[Tensor] = None,
+        x0: Optional[Tensor] = None,
+        y0: Optional[Tensor] = None,
+        m: Optional[Tensor] = None,
+        c: Optional[Tensor] = None,
         **kwargs,
     ) -> Tensor:
         """
         Calculate the scale density of the lens.
 
         Parameters
         ----------
@@ -197,19 +198,19 @@
 
     @unpack
     def get_convergence_s(
         self,
         z_s,
         *args,
         params: Optional["Packed"] = None,
-        z_l: Tensor = None,
-        x0: Tensor = None,
-        y0: Tensor = None,
-        m: Tensor = None,
-        c: Tensor = None,
+        z_l: Optional[Tensor] = None,
+        x0: Optional[Tensor] = None,
+        y0: Optional[Tensor] = None,
+        m: Optional[Tensor] = None,
+        c: Optional[Tensor] = None,
         **kwargs,
     ) -> Tensor:
         """
         Calculate the dimensionless surface mass density of the lens.
 
         Parameters
         ----------
@@ -384,19 +385,19 @@
     def reduced_deflection_angle(
         self,
         x: Tensor,
         y: Tensor,
         z_s: Tensor,
         *args,
         params: Optional["Packed"] = None,
-        z_l: Tensor = None,
-        x0: Tensor = None,
-        y0: Tensor = None,
-        m: Tensor = None,
-        c: Tensor = None,
+        z_l: Optional[Tensor] = None,
+        x0: Optional[Tensor] = None,
+        y0: Optional[Tensor] = None,
+        m: Optional[Tensor] = None,
+        c: Optional[Tensor] = None,
         **kwargs,
     ) -> tuple[Tensor, Tensor]:
         """
         Compute the reduced deflection angle.
 
         Parameters
         ----------
@@ -433,19 +434,19 @@
     def convergence(
         self,
         x: Tensor,
         y: Tensor,
         z_s: Tensor,
         *args,
         params: Optional["Packed"] = None,
-        z_l: Tensor = None,
-        x0: Tensor = None,
-        y0: Tensor = None,
-        m: Tensor = None,
-        c: Tensor = None,
+        z_l: Optional[Tensor] = None,
+        x0: Optional[Tensor] = None,
+        y0: Optional[Tensor] = None,
+        m: Optional[Tensor] = None,
+        c: Optional[Tensor] = None,
         **kwargs,
     ) -> Tensor:
         """
         Compute the convergence (dimensionless surface mass density).
 
         Parameters
         ----------
@@ -476,19 +477,19 @@
     def potential(
         self,
         x: Tensor,
         y: Tensor,
         z_s: Tensor,
         *args,
         params: Optional["Packed"] = None,
-        z_l: Tensor = None,
-        x0: Tensor = None,
-        y0: Tensor = None,
-        m: Tensor = None,
-        c: Tensor = None,
+        z_l: Optional[Tensor] = None,
+        x0: Optional[Tensor] = None,
+        y0: Optional[Tensor] = None,
+        m: Optional[Tensor] = None,
+        c: Optional[Tensor] = None,
         **kwargs,
     ) -> Tensor:
         """
         Compute the lensing potential.
 
         Parameters
         ----------
```

### Comparing `caustics-0.7.0/src/caustics/lenses/pixelated_convergence.py` & `caustics-0.8.0/src/caustics/lenses/pixelated_convergence.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# mypy: disable-error-code="index"
 from math import pi
 from typing import Optional
 
 import torch
 import torch.nn.functional as F
 from scipy.fft import next_fast_len
 from torch import Tensor
@@ -32,15 +33,15 @@
         x0: Optional[Tensor] = torch.tensor(0.0),
         y0: Optional[Tensor] = torch.tensor(0.0),
         convergence_map: Optional[Tensor] = None,
         shape: Optional[tuple[int, ...]] = None,
         convolution_mode: str = "fft",
         use_next_fast_len: bool = True,
         padding: str = "zero",
-        name: str = None,
+        name: Optional[str] = None,
     ):
         """Strong lensing with user provided kappa map
 
         PixelatedConvergence is a class for strong gravitational lensing with a
         user-provided kappa map. It inherits from the ThinLens class.
         This class enables the computation of deflection angles and
         lensing potential by applying the user-provided kappa map to a
@@ -256,18 +257,18 @@
     def reduced_deflection_angle(
         self,
         x: Tensor,
         y: Tensor,
         z_s: Tensor,
         *args,
         params: Optional["Packed"] = None,
-        z_l: Tensor = None,
-        x0: Tensor = None,
-        y0: Tensor = None,
-        convergence_map: Tensor = None,
+        z_l: Optional[Tensor] = None,
+        x0: Optional[Tensor] = None,
+        y0: Optional[Tensor] = None,
+        convergence_map: Optional[Tensor] = None,
         **kwargs,
     ) -> tuple[Tensor, Tensor]:
         """
         Compute the deflection angles at the specified positions using the given convergence map.
 
         Parameters
         ----------
@@ -363,18 +364,18 @@
     def potential(
         self,
         x: Tensor,
         y: Tensor,
         z_s: Tensor,
         *args,
         params: Optional["Packed"] = None,
-        z_l: Tensor = None,
-        x0: Tensor = None,
-        y0: Tensor = None,
-        convergence_map: Tensor = None,
+        z_l: Optional[Tensor] = None,
+        x0: Optional[Tensor] = None,
+        y0: Optional[Tensor] = None,
+        convergence_map: Optional[Tensor] = None,
         **kwargs,
     ) -> Tensor:
         """
         Compute the lensing potential at the specified positions using the given convergence map.
 
         Parameters
         ----------
@@ -449,18 +450,18 @@
     def convergence(
         self,
         x: Tensor,
         y: Tensor,
         z_s: Tensor,
         *args,
         params: Optional["Packed"] = None,
-        z_l: Tensor = None,
-        x0: Tensor = None,
-        y0: Tensor = None,
-        convergence_map: Tensor = None,
+        z_l: Optional[Tensor] = None,
+        x0: Optional[Tensor] = None,
+        y0: Optional[Tensor] = None,
+        convergence_map: Optional[Tensor] = None,
         **kwargs,
     ) -> Tensor:
         """
         Compute the convergence at the specified positions. This method is not implemented.
 
         Parameters
         ----------
```

### Comparing `caustics-0.7.0/src/caustics/lenses/point.py` & `caustics-0.8.0/src/caustics/lenses/point.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# mypy: disable-error-code="operator"
 from typing import Optional, Union
 
 import torch
 from torch import Tensor
 
 from ..cosmology import Cosmology
 from ..utils import translate_rotate
@@ -44,15 +45,15 @@
         self,
         cosmology: Cosmology,
         z_l: Optional[Union[Tensor, float]] = None,
         x0: Optional[Union[Tensor, float]] = None,
         y0: Optional[Union[Tensor, float]] = None,
         th_ein: Optional[Union[Tensor, float]] = None,
         s: float = 0.0,
-        name: str = None,
+        name: Optional[str] = None,
     ):
         """
         Initialize the Point class.
 
         Parameters
         ----------
         name: string
@@ -81,18 +82,18 @@
     def reduced_deflection_angle(
         self,
         x: Tensor,
         y: Tensor,
         z_s: Tensor,
         *args,
         params: Optional["Packed"] = None,
-        z_l: Tensor = None,
-        x0: Tensor = None,
-        y0: Tensor = None,
-        th_ein: Tensor = None,
+        z_l: Optional[Tensor] = None,
+        x0: Optional[Tensor] = None,
+        y0: Optional[Tensor] = None,
+        th_ein: Optional[Tensor] = None,
         **kwargs,
     ) -> tuple[Tensor, Tensor]:
         """
         Compute the deflection angles.
 
         Parameters
         ----------
@@ -120,18 +121,18 @@
     def potential(
         self,
         x: Tensor,
         y: Tensor,
         z_s: Tensor,
         *args,
         params: Optional["Packed"] = None,
-        z_l: Tensor = None,
-        x0: Tensor = None,
-        y0: Tensor = None,
-        th_ein: Tensor = None,
+        z_l: Optional[Tensor] = None,
+        x0: Optional[Tensor] = None,
+        y0: Optional[Tensor] = None,
+        th_ein: Optional[Tensor] = None,
         **kwargs,
     ) -> Tensor:
         """
         Compute the lensing potential.
 
         Parameters
         ----------
@@ -157,18 +158,18 @@
     def convergence(
         self,
         x: Tensor,
         y: Tensor,
         z_s: Tensor,
         *args,
         params: Optional["Packed"] = None,
-        z_l: Tensor = None,
-        x0: Tensor = None,
-        y0: Tensor = None,
-        th_ein: Tensor = None,
+        z_l: Optional[Tensor] = None,
+        x0: Optional[Tensor] = None,
+        y0: Optional[Tensor] = None,
+        th_ein: Optional[Tensor] = None,
         **kwargs,
     ) -> Tensor:
         """
         Compute the convergence (dimensionless surface mass density).
 
         Parameters
         ----------
```

### Comparing `caustics-0.7.0/src/caustics/lenses/pseudo_jaffe.py` & `caustics-0.8.0/src/caustics/lenses/pseudo_jaffe.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# mypy: disable-error-code="operator"
 from math import pi
 from typing import Optional, Union
 
 import torch
 from torch import Tensor
 
 from ..cosmology import Cosmology
@@ -56,15 +57,15 @@
         z_l: Optional[Union[Tensor, float]] = None,
         x0: Optional[Union[Tensor, float]] = None,
         y0: Optional[Union[Tensor, float]] = None,
         mass: Optional[Union[Tensor, float]] = None,
         core_radius: Optional[Union[Tensor, float]] = None,
         scale_radius: Optional[Union[Tensor, float]] = None,
         s: float = 0.0,
-        name: str = None,
+        name: Optional[str] = None,
     ):
         """
         Initialize the PseudoJaffe class.
 
         Parameters
         ----------
         name: string
@@ -97,39 +98,39 @@
 
     @unpack
     def get_convergence_0(
         self,
         z_s,
         *args,
         params: Optional["Packed"] = None,
-        z_l: Tensor = None,
-        x0: Tensor = None,
-        y0: Tensor = None,
-        mass: Tensor = None,
-        core_radius: Tensor = None,
-        scale_radius: Tensor = None,
+        z_l: Optional[Tensor] = None,
+        x0: Optional[Tensor] = None,
+        y0: Optional[Tensor] = None,
+        mass: Optional[Tensor] = None,
+        core_radius: Optional[Tensor] = None,
+        scale_radius: Optional[Tensor] = None,
         **kwargs,
     ):
         d_l = self.cosmology.angular_diameter_distance(z_l, params)
         sigma_crit = self.cosmology.critical_surface_density(z_l, z_s, params)
         return mass / (2 * torch.pi * sigma_crit * core_radius * scale_radius * (d_l * arcsec_to_rad) ** 2)  # fmt: skip
 
     @unpack
     def mass_enclosed_2d(
         self,
         theta,
         z_s,
         *args,
         params: Optional["Packed"] = None,
-        z_l: Tensor = None,
-        x0: Tensor = None,
-        y0: Tensor = None,
-        mass: Tensor = None,
-        core_radius: Tensor = None,
-        scale_radius: Tensor = None,
+        z_l: Optional[Tensor] = None,
+        x0: Optional[Tensor] = None,
+        y0: Optional[Tensor] = None,
+        mass: Optional[Tensor] = None,
+        core_radius: Optional[Tensor] = None,
+        scale_radius: Optional[Tensor] = None,
         **kwargs,
     ):
         """
         Calculate the mass enclosed within a two-dimensional radius. Using equation A10 from `Eliasdottir et al 2007 <https://arxiv.org/abs/0710.5636>`_.
 
         Parameters
         ----------
@@ -195,20 +196,20 @@
     def reduced_deflection_angle(
         self,
         x: Tensor,
         y: Tensor,
         z_s: Tensor,
         *args,
         params: Optional["Packed"] = None,
-        z_l: Tensor = None,
-        x0: Tensor = None,
-        y0: Tensor = None,
-        mass: Tensor = None,
-        core_radius: Tensor = None,
-        scale_radius: Tensor = None,
+        z_l: Optional[Tensor] = None,
+        x0: Optional[Tensor] = None,
+        y0: Optional[Tensor] = None,
+        mass: Optional[Tensor] = None,
+        core_radius: Optional[Tensor] = None,
+        scale_radius: Optional[Tensor] = None,
         **kwargs,
     ) -> tuple[Tensor, Tensor]:
         """Calculate the deflection angle.
 
         Parameters
         ----------
         x: Tensor
@@ -237,20 +238,20 @@
     def potential(
         self,
         x: Tensor,
         y: Tensor,
         z_s: Tensor,
         *args,
         params: Optional["Packed"] = None,
-        z_l: Tensor = None,
-        x0: Tensor = None,
-        y0: Tensor = None,
-        mass: Tensor = None,
-        core_radius: Tensor = None,
-        scale_radius: Tensor = None,
+        z_l: Optional[Tensor] = None,
+        x0: Optional[Tensor] = None,
+        y0: Optional[Tensor] = None,
+        mass: Optional[Tensor] = None,
+        core_radius: Optional[Tensor] = None,
+        scale_radius: Optional[Tensor] = None,
         **kwargs,
     ) -> Tensor:
         """
         Compute the lensing potential. This calculation is based on equation A18 from `Eliasdottir et al 2007 <https://arxiv.org/abs/0710.5636>`_.
 
         Parameters
         --------
@@ -294,20 +295,20 @@
     def convergence(
         self,
         x: Tensor,
         y: Tensor,
         z_s: Tensor,
         *args,
         params: Optional["Packed"] = None,
-        z_l: Tensor = None,
-        x0: Tensor = None,
-        y0: Tensor = None,
-        mass: Tensor = None,
-        core_radius: Tensor = None,
-        scale_radius: Tensor = None,
+        z_l: Optional[Tensor] = None,
+        x0: Optional[Tensor] = None,
+        y0: Optional[Tensor] = None,
+        mass: Optional[Tensor] = None,
+        core_radius: Optional[Tensor] = None,
+        scale_radius: Optional[Tensor] = None,
         **kwargs,
     ) -> Tensor:
         """
         Calculate the projected mass density, based on equation A6.
 
         Parameters
         -----------
```

### Comparing `caustics-0.7.0/src/caustics/lenses/singleplane.py` & `caustics-0.8.0/src/caustics/lenses/singleplane.py`

 * *Files 17% similar despite different names*

```diff
@@ -23,15 +23,19 @@
     cosmology: Cosmology
         An instance of the Cosmology class.
     lenses: List[ThinLens]
         A list of ThinLens objects that are being combined into a single lensing plane.
     """
 
     def __init__(
-        self, cosmology: Cosmology, lenses: list[ThinLens], name: str = None, **kwargs
+        self,
+        cosmology: Cosmology,
+        lenses: list[ThinLens],
+        name: Optional[str] = None,
+        **kwargs,
     ):
         """
         Initialize the SinglePlane lens model.
         """
         super().__init__(cosmology, name=name, **kwargs)
         self.lenses = lenses
         for lens in lenses:
```

### Comparing `caustics-0.7.0/src/caustics/lenses/sis.py` & `caustics-0.8.0/src/caustics/lenses/sie.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,123 +1,161 @@
+# mypy: disable-error-code="operator,union-attr"
 from typing import Optional, Union
 
 from torch import Tensor
 
 from ..cosmology import Cosmology
-from ..utils import translate_rotate
+from ..utils import derotate, translate_rotate
 from .base import ThinLens
 from ..parametrized import unpack
 from ..packed import Packed
 
-__all__ = ("SIS",)
+__all__ = ("SIE",)
 
 
-class SIS(ThinLens):
+class SIE(ThinLens):
     """
-    A class representing the Singular Isothermal Sphere (SIS) model.
-    This model inherits from the base `ThinLens` class.
+    A class representing a Singular Isothermal Ellipsoid (SIE) strong gravitational lens model.
+    This model is based on Keeton 2001, which can be found at https://arxiv.org/abs/astro-ph/0102341.
 
     Attributes
     ----------
     name: str
-        The name of the SIS lens.
+        The name of the lens.
     cosmology: Cosmology
         An instance of the Cosmology class.
     z_l: Optional[Union[Tensor, float]]
-        The lens redshift.
+        The redshift of the lens.
     x0: Optional[Union[Tensor, float]]
         The x-coordinate of the lens center.
     y0: Optional[Union[Tensor, float]]
         The y-coordinate of the lens center.
-        th_ein (Optional[Union[Tensor, float]]): The Einstein radius of the lens.
+    q: Optional[Union[Tensor, float]]
+        The axis ratio of the lens.
+    phi: Optional[Union[Tensor, float]]
+        The orientation angle of the lens (position angle).
+    b: Optional[Union[Tensor, float]]
+        The Einstein radius of the lens.
     s: float
-        A smoothing factor, default is 0.0.
+        The core radius of the lens (defaults to 0.0).
     """
 
     _null_params = {
         "x0": 0.0,
         "y0": 0.0,
-        "th_ein": 1.0,
+        "q": 0.5,
+        "phi": 0.0,
+        "b": 1.0,
     }
 
     def __init__(
         self,
         cosmology: Cosmology,
         z_l: Optional[Union[Tensor, float]] = None,
         x0: Optional[Union[Tensor, float]] = None,
         y0: Optional[Union[Tensor, float]] = None,
-        th_ein: Optional[Union[Tensor, float]] = None,
+        q: Optional[Union[Tensor, float]] = None,  # TODO change to true axis ratio
+        phi: Optional[Union[Tensor, float]] = None,
+        b: Optional[Union[Tensor, float]] = None,
         s: float = 0.0,
-        name: str = None,
+        name: Optional[str] = None,
     ):
         """
-        Initialize the SIS lens model.
+        Initialize the SIE lens model.
         """
         super().__init__(cosmology, z_l, name=name)
 
         self.add_param("x0", x0)
         self.add_param("y0", y0)
-        self.add_param("th_ein", th_ein)
+        self.add_param("q", q)
+        self.add_param("phi", phi)
+        self.add_param("b", b)
         self.s = s
 
+    def _get_potential(self, x, y, q):
+        """
+        Compute the radial coordinate in the lens plane.
+
+        Parameters
+        ----------
+        x: Tensor
+            The x-coordinate in the lens plane.
+        y: Tensor
+            The y-coordinate in the lens plane.
+        q: Tensor
+            The axis ratio of the lens.
+
+        Returns
+        --------
+        Tensor
+            The radial coordinate in the lens plane.
+        """
+        return (q**2 * (x**2 + self.s**2) + y**2).sqrt()  # fmt: skip
+
     @unpack
     def reduced_deflection_angle(
         self,
         x: Tensor,
         y: Tensor,
         z_s: Tensor,
         *args,
         params: Optional["Packed"] = None,
-        z_l: Tensor = None,
-        x0: Tensor = None,
-        y0: Tensor = None,
-        th_ein: Tensor = None,
+        z_l: Optional[Tensor] = None,
+        x0: Optional[Tensor] = None,
+        y0: Optional[Tensor] = None,
+        q: Optional[Tensor] = None,
+        phi: Optional[Tensor] = None,
+        b: Optional[Tensor] = None,
         **kwargs,
     ) -> tuple[Tensor, Tensor]:
         """
-        Calculate the deflection angle of the SIS lens.
+        Calculate the physical deflection angle.
 
         Parameters
         ----------
         x: Tensor
             The x-coordinate of the lens.
         y: Tensor
             The y-coordinate of the lens.
         z_s: Tensor
             The source redshift.
         params: (Packed, optional)
             Dynamic parameter container.
 
         Returns
-        -------
+        --------
         Tuple[Tensor, Tensor]
             The deflection angle in the x and y directions.
         """
-        x, y = translate_rotate(x, y, x0, y0)
-        R = (x**2 + y**2).sqrt() + self.s
-        ax = th_ein * x / R
-        ay = th_ein * y / R
-        return ax, ay
+        x, y = translate_rotate(x, y, x0, y0, phi)
+        psi = self._get_potential(x, y, q)
+        f = (1 - q**2).sqrt()
+        ax = b * q.sqrt() / f * (f * x / (psi + self.s)).atan()  # fmt: skip
+        ay = b * q.sqrt() / f * (f * y / (psi + q**2 * self.s)).atanh()  # fmt: skip
+
+        return derotate(ax, ay, phi)
 
     @unpack
     def potential(
         self,
         x: Tensor,
         y: Tensor,
         z_s: Tensor,
         *args,
         params: Optional["Packed"] = None,
-        z_l: Tensor = None,
-        x0: Tensor = None,
-        y0: Tensor = None,
-        th_ein: Tensor = None,
+        x0: Optional[Tensor] = None,
+        z_l: Optional[Tensor] = None,
+        y0: Optional[Tensor] = None,
+        q: Optional[Tensor] = None,
+        phi: Optional[Tensor] = None,
+        b: Optional[Tensor] = None,
         **kwargs,
     ) -> Tensor:
         """
-        Compute the lensing potential of the SIS lens.
+        Compute the lensing potential.
 
         Parameters
         ----------
         x: Tensor
             The x-coordinate of the lens.
         y: Tensor
             The y-coordinate of the lens.
@@ -127,34 +165,37 @@
             Dynamic parameter container.
 
         Returns
         -------
         Tensor
             The lensing potential.
         """
-        x, y = translate_rotate(x, y, x0, y0)
-        th = (x**2 + y**2).sqrt() + self.s
-        return th_ein * th
+        ax, ay = self.reduced_deflection_angle(x, y, z_s, params)
+        ax, ay = derotate(ax, ay, -phi)
+        x, y = translate_rotate(x, y, x0, y0, phi)
+        return x * ax + y * ay
 
     @unpack
     def convergence(
         self,
         x: Tensor,
         y: Tensor,
         z_s: Tensor,
         *args,
         params: Optional["Packed"] = None,
-        z_l: Tensor = None,
-        x0: Tensor = None,
-        y0: Tensor = None,
-        th_ein: Tensor = None,
+        z_l: Optional[Tensor] = None,
+        x0: Optional[Tensor] = None,
+        y0: Optional[Tensor] = None,
+        q: Optional[Tensor] = None,
+        phi: Optional[Tensor] = None,
+        b: Optional[Tensor] = None,
         **kwargs,
     ) -> Tensor:
         """
-        Calculate the projected mass density of the SIS lens.
+        Calculate the projected mass density.
 
         Parameters
         ----------
         x: Tensor
             The x-coordinate of the lens.
         y: Tensor
             The y-coordinate of the lens.
@@ -162,12 +203,12 @@
             The source redshift.
         params: (Packed, optional)
             Dynamic parameter container.
 
         Returns
         -------
         Tensor
-            The projected mass density.
+            The projected mass.
         """
-        x, y = translate_rotate(x, y, x0, y0)
-        th = (x**2 + y**2).sqrt() + self.s
-        return 0.5 * th_ein / th
+        x, y = translate_rotate(x, y, x0, y0, phi)
+        psi = self._get_potential(x, y, q)
+        return 0.5 * q.sqrt() * b / psi
```

### Comparing `caustics-0.7.0/src/caustics/lenses/tnfw.py` & `caustics-0.8.0/src/caustics/lenses/tnfw.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# mypy: disable-error-code="operator,union-attr"
 from math import pi
 from typing import Optional, Union
 
 import torch
 from torch import Tensor
 
 from ..constants import G_over_c2, arcsec_to_rad, rad_to_arcsec
@@ -91,15 +92,15 @@
         y0: Optional[Union[Tensor, float]] = None,
         mass: Optional[Union[Tensor, float]] = None,
         scale_radius: Optional[Union[Tensor, float]] = None,
         tau: Optional[Union[Tensor, float]] = None,
         s: float = 0.0,
         interpret_m_total_mass: bool = True,
         use_case="batchable",
-        name: str = None,
+        name: Optional[str] = None,
     ):
         """
         Initialize an instance of the TNFW lens class.
 
         """
         super().__init__(cosmology, z_l, name=name)
 
@@ -146,20 +147,20 @@
         return (x / (tau + (tau**2 + x**2).sqrt())).log()  # fmt: skip
 
     @unpack
     def get_concentration(
         self,
         *args,
         params: Optional[Packed] = None,
-        z_l: Tensor = None,
-        x0: Tensor = None,
-        y0: Tensor = None,
-        mass: Tensor = None,
-        scale_radius: Tensor = None,
-        tau: Tensor = None,
+        z_l: Optional[Tensor] = None,
+        x0: Optional[Tensor] = None,
+        y0: Optional[Tensor] = None,
+        mass: Optional[Tensor] = None,
+        scale_radius: Optional[Tensor] = None,
+        tau: Optional[Tensor] = None,
         **kwargs,
     ) -> Tensor:
         """
         Calculate the scale radius of the lens.
         This is the same formula used for the classic NFW profile.
 
         Parameters
@@ -190,20 +191,20 @@
         return r_delta / (scale_radius * d_l * arcsec_to_rad)  # fmt: skip
 
     @unpack
     def get_truncation_radius(
         self,
         *args,
         params: Optional[Packed] = None,
-        z_l: Tensor = None,
-        x0: Tensor = None,
-        y0: Tensor = None,
-        mass: Tensor = None,
-        scale_radius: Tensor = None,
-        tau: Tensor = None,
+        z_l: Optional[Tensor] = None,
+        x0: Optional[Tensor] = None,
+        y0: Optional[Tensor] = None,
+        mass: Optional[Tensor] = None,
+        scale_radius: Optional[Tensor] = None,
+        tau: Optional[Tensor] = None,
         **kwargs,
     ) -> Tensor:
         """
         Calculate the truncation radius of the TNFW lens.
 
         Parameters
         ----------
@@ -230,20 +231,20 @@
         return tau * scale_radius
 
     @unpack
     def get_M0(
         self,
         *args,
         params: Optional[Packed] = None,
-        z_l: Tensor = None,
-        x0: Tensor = None,
-        y0: Tensor = None,
-        mass: Tensor = None,
-        scale_radius: Tensor = None,
-        tau: Tensor = None,
+        z_l: Optional[Tensor] = None,
+        x0: Optional[Tensor] = None,
+        y0: Optional[Tensor] = None,
+        mass: Optional[Tensor] = None,
+        scale_radius: Optional[Tensor] = None,
+        tau: Optional[Tensor] = None,
         **kwargs,
     ) -> Tensor:
         """
         Calculate the reference mass.
         This is an abstract reference mass used internally
         in the equations from Baltz et al. 2009.
 
@@ -276,20 +277,20 @@
             return 4 * torch.pi * (scale_radius * d_l * arcsec_to_rad) ** 3 * self.get_scale_density(params)  # fmt: skip
 
     @unpack
     def get_scale_density(
         self,
         *args,
         params: Optional[Packed] = None,
-        z_l: Tensor = None,
-        x0: Tensor = None,
-        y0: Tensor = None,
-        mass: Tensor = None,
-        scale_radius: Tensor = None,
-        tau: Tensor = None,
+        z_l: Optional[Tensor] = None,
+        x0: Optional[Tensor] = None,
+        y0: Optional[Tensor] = None,
+        mass: Optional[Tensor] = None,
+        scale_radius: Optional[Tensor] = None,
+        tau: Optional[Tensor] = None,
         **kwargs,
     ) -> Tensor:
         """
         Calculate the scale density of the lens.
 
         Parameters
         ----------
@@ -320,20 +321,20 @@
     def convergence(
         self,
         x: Tensor,
         y: Tensor,
         z_s: Tensor,
         *args,
         params: Optional[Packed] = None,
-        z_l: Tensor = None,
-        x0: Tensor = None,
-        y0: Tensor = None,
-        mass: Tensor = None,
-        scale_radius: Tensor = None,
-        tau: Tensor = None,
+        z_l: Optional[Tensor] = None,
+        x0: Optional[Tensor] = None,
+        y0: Optional[Tensor] = None,
+        mass: Optional[Tensor] = None,
+        scale_radius: Optional[Tensor] = None,
+        tau: Optional[Tensor] = None,
         **kwargs,
     ) -> Tensor:
         """
         TNFW convergence as given in Baltz et al. 2009.
         This is unitless since it is Sigma(x) / Sigma_crit.
 
         Parameters
@@ -380,20 +381,20 @@
     @unpack
     def mass_enclosed_2d(
         self,
         r: Tensor,
         z_s: Tensor,
         *args,
         params: Optional[Packed] = None,
-        z_l: Tensor = None,
-        x0: Tensor = None,
-        y0: Tensor = None,
-        mass: Tensor = None,
-        scale_radius: Tensor = None,
-        tau: Tensor = None,
+        z_l: Optional[Tensor] = None,
+        x0: Optional[Tensor] = None,
+        y0: Optional[Tensor] = None,
+        mass: Optional[Tensor] = None,
+        scale_radius: Optional[Tensor] = None,
+        tau: Optional[Tensor] = None,
         **kwargs,
     ) -> Tensor:
         """
         Total projected mass (Msol) within a radius r (arcsec).
 
         Parameters
         -----------
@@ -433,20 +434,20 @@
     def physical_deflection_angle(
         self,
         x: Tensor,
         y: Tensor,
         z_s: Tensor,
         *args,
         params: Optional[Packed] = None,
-        z_l: Tensor = None,
-        x0: Tensor = None,
-        y0: Tensor = None,
-        mass: Tensor = None,
-        scale_radius: Tensor = None,
-        tau: Tensor = None,
+        z_l: Optional[Tensor] = None,
+        x0: Optional[Tensor] = None,
+        y0: Optional[Tensor] = None,
+        mass: Optional[Tensor] = None,
+        scale_radius: Optional[Tensor] = None,
+        tau: Optional[Tensor] = None,
         **kwargs,
     ) -> tuple[Tensor, Tensor]:
         """Compute the physical deflection angle (arcsec) for this lens at
         the requested position. Note that the NFW/TNFW profile is more
         naturally represented as a physical deflection angle, this is
         easily internally converted to a reduced deflection angle.
 
@@ -489,20 +490,20 @@
     def potential(
         self,
         x: Tensor,
         y: Tensor,
         z_s: Tensor,
         *args,
         params: Optional[Packed] = None,
-        z_l: Tensor = None,
-        x0: Tensor = None,
-        y0: Tensor = None,
-        mass: Tensor = None,
-        scale_radius: Tensor = None,
-        tau: Tensor = None,
+        z_l: Optional[Tensor] = None,
+        x0: Optional[Tensor] = None,
+        y0: Optional[Tensor] = None,
+        mass: Optional[Tensor] = None,
+        scale_radius: Optional[Tensor] = None,
+        tau: Optional[Tensor] = None,
         **kwargs,
     ) -> Tensor:
         """
         Compute the lensing potential.
         Note that this is not a unitless potential!
         This is the potential as given in Baltz et al. 2009.
```

### Comparing `caustics-0.7.0/src/caustics/lenses/utils.py` & `caustics-0.8.0/src/caustics/lenses/utils.py`

 * *Files identical despite different names*

### Comparing `caustics-0.7.0/src/caustics/light/base.py` & `caustics-0.8.0/src/caustics/light/base.py`

 * *Files identical despite different names*

### Comparing `caustics-0.7.0/src/caustics/light/pixelated.py` & `caustics-0.8.0/src/caustics/light/pixelated.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# mypy: disable-error-code="union-attr"
 from typing import Optional, Union
 
 from torch import Tensor
 
 from ..utils import interp2d
 from .base import Source
 from ..parametrized import unpack
@@ -38,15 +39,15 @@
     def __init__(
         self,
         image: Optional[Tensor] = None,
         x0: Optional[Union[Tensor, float]] = None,
         y0: Optional[Union[Tensor, float]] = None,
         pixelscale: Optional[Union[Tensor, float]] = None,
         shape: Optional[tuple[int, ...]] = None,
-        name: str = None,
+        name: Optional[str] = None,
     ):
         """
         Constructs the `Pixelated` object with the given parameters.
 
         Parameters
         ----------
         name : str
@@ -79,18 +80,18 @@
     @unpack
     def brightness(
         self,
         x,
         y,
         *args,
         params: Optional["Packed"] = None,
-        x0: Tensor = None,
-        y0: Tensor = None,
-        image: Tensor = None,
-        pixelscale: Tensor = None,
+        x0: Optional[Tensor] = None,
+        y0: Optional[Tensor] = None,
+        image: Optional[Tensor] = None,
+        pixelscale: Optional[Tensor] = None,
         **kwargs,
     ):
         """
         Implements the `brightness` method for `Pixelated`.
         The brightness at a given point is determined
         by interpolating values from the source image.
```

### Comparing `caustics-0.7.0/src/caustics/light/probes.py` & `caustics-0.8.0/src/caustics/light/probes.py`

 * *Files identical despite different names*

### Comparing `caustics-0.7.0/src/caustics/light/sersic.py` & `caustics-0.8.0/src/caustics/light/sersic.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# mypy: disable-error-code="operator,union-attr"
 from typing import Optional, Union
 
 from torch import Tensor
 
 from ..utils import to_elliptical, translate_rotate
 from .base import Source
 from ..parametrized import unpack
@@ -49,15 +50,15 @@
         q: Optional[Union[Tensor, float]] = None,
         phi: Optional[Union[Tensor, float]] = None,
         n: Optional[Union[Tensor, float]] = None,
         Re: Optional[Union[Tensor, float]] = None,
         Ie: Optional[Union[Tensor, float]] = None,
         s: float = 0.0,
         use_lenstronomy_k=False,
-        name: str = None,
+        name: Optional[str] = None,
     ):
         """
         Constructs the `Sersic` object with the given parameters.
 
         Parameters
         ----------
         name: str
@@ -96,21 +97,21 @@
     @unpack
     def brightness(
         self,
         x,
         y,
         *args,
         params: Optional["Packed"] = None,
-        x0: Tensor = None,
-        y0: Tensor = None,
-        q: Tensor = None,
-        phi: Tensor = None,
-        n: Tensor = None,
-        Re: Tensor = None,
-        Ie: Tensor = None,
+        x0: Optional[Tensor] = None,
+        y0: Optional[Tensor] = None,
+        q: Optional[Tensor] = None,
+        phi: Optional[Tensor] = None,
+        n: Optional[Tensor] = None,
+        Re: Optional[Tensor] = None,
+        Ie: Optional[Tensor] = None,
         **kwargs,
     ):
         """
         Implements the `brightness` method for `Sersic`. The brightness at a given point is
         determined by the Sersic profile formula.
 
         Parameters
```

### Comparing `caustics-0.7.0/src/caustics/sims/lens_source.py` & `caustics-0.8.0/src/caustics/sims/lens_source.py`

 * *Files identical despite different names*

### Comparing `caustics-0.7.0/tests/test_base.py` & `caustics-0.8.0/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `caustics-0.7.0/tests/test_batching.py` & `caustics-0.8.0/tests/test_batching.py`

 * *Files identical despite different names*

### Comparing `caustics-0.7.0/tests/test_cosmology.py` & `caustics-0.8.0/tests/test_cosmology.py`

 * *Files identical despite different names*

### Comparing `caustics-0.7.0/tests/test_epl.py` & `caustics-0.8.0/tests/test_epl.py`

 * *Files identical despite different names*

### Comparing `caustics-0.7.0/tests/test_external_shear.py` & `caustics-0.8.0/tests/test_external_shear.py`

 * *Files identical despite different names*

### Comparing `caustics-0.7.0/tests/test_interpolate_image.py` & `caustics-0.8.0/tests/test_interpolate_image.py`

 * *Files identical despite different names*

### Comparing `caustics-0.7.0/tests/test_jacobian_lens_equation.py` & `caustics-0.8.0/tests/test_jacobian_lens_equation.py`

 * *Files identical despite different names*

### Comparing `caustics-0.7.0/tests/test_kappa_grid.py` & `caustics-0.8.0/tests/test_kappa_grid.py`

 * *Files identical despite different names*

### Comparing `caustics-0.7.0/tests/test_lens_potential.py` & `caustics-0.8.0/tests/test_lens_potential.py`

 * *Files identical despite different names*

### Comparing `caustics-0.7.0/tests/test_masssheet.py` & `caustics-0.8.0/tests/test_masssheet.py`

 * *Files identical despite different names*

### Comparing `caustics-0.7.0/tests/test_multiplane.py` & `caustics-0.8.0/tests/test_multiplane.py`

 * *Files identical despite different names*

### Comparing `caustics-0.7.0/tests/test_namespace_dict.py` & `caustics-0.8.0/tests/test_namespace_dict.py`

 * *Files identical despite different names*

### Comparing `caustics-0.7.0/tests/test_nfw.py` & `caustics-0.8.0/tests/test_nfw.py`

 * *Files identical despite different names*

### Comparing `caustics-0.7.0/tests/test_parameter.py` & `caustics-0.8.0/tests/test_parameter.py`

 * *Files identical despite different names*

### Comparing `caustics-0.7.0/tests/test_parametrized.py` & `caustics-0.8.0/tests/test_parametrized.py`

 * *Files identical despite different names*

### Comparing `caustics-0.7.0/tests/test_pixel_grid.py` & `caustics-0.8.0/tests/test_pixel_grid.py`

 * *Files identical despite different names*

### Comparing `caustics-0.7.0/tests/test_point.py` & `caustics-0.8.0/tests/test_point.py`

 * *Files identical despite different names*

### Comparing `caustics-0.7.0/tests/test_pseudo_jaffe.py` & `caustics-0.8.0/tests/test_pseudo_jaffe.py`

 * *Files identical despite different names*

### Comparing `caustics-0.7.0/tests/test_sersic.py` & `caustics-0.8.0/tests/test_sersic.py`

 * *Files identical despite different names*

### Comparing `caustics-0.7.0/tests/test_sie.py` & `caustics-0.8.0/tests/test_sie.py`

 * *Files identical despite different names*

### Comparing `caustics-0.7.0/tests/test_simulator.py` & `caustics-0.8.0/tests/test_simulator_runs.py`

 * *Files identical despite different names*

### Comparing `caustics-0.7.0/tests/test_sis.py` & `caustics-0.8.0/tests/test_sis.py`

 * *Files identical despite different names*

### Comparing `caustics-0.7.0/tests/test_tnfw.py` & `caustics-0.8.0/tests/test_tnfw.py`

 * *Files identical despite different names*

### Comparing `caustics-0.7.0/tests/utils.py` & `caustics-0.8.0/tests/utils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+"""
+Utilities for testing
+"""
 from typing import Any, Dict, List, Union
 
 import torch
 import numpy as np
 from astropy.cosmology import FlatLambdaCDM as FlatLambdaCDM_AP
 from lenstronomy.Data.pixel_grid import PixelGrid
 from lenstronomy.LensModel.lens_model import LensModel
```

### Comparing `caustics-0.7.0/.gitignore` & `caustics-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `caustics-0.7.0/LICENSE` & `caustics-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `caustics-0.7.0/README.md` & `caustics-0.8.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -28,27 +28,27 @@
 ## Minimal Example
 
 ```python
 import matplotlib.pyplot as plt
 import caustics
 import torch
 
-cosmology = caustics.cosmology.FlatLambdaCDM()
-sie = caustics.lenses.SIE(cosmology=cosmology, name="lens")
-src = caustics.light.Sersic(name="source")
-lnslt = caustics.light.Sersic(name="lenslight")
+cosmology = caustics.FlatLambdaCDM()
+sie = caustics.SIE(cosmology=cosmology, name="lens")
+src = caustics.Sersic(name="source")
+lnslt = caustics.Sersic(name="lenslight")
 
 x = torch.tensor([
 #   z_s  z_l   x0   y0   q    phi     b    x0   y0   q     phi    n    Re
     1.5, 0.5, -0.2, 0.0, 0.4, 1.5708, 1.7, 0.0, 0.0, 0.5, -0.985, 1.3, 1.0,
 #   Ie    x0   y0   q    phi  n   Re   Ie
     5.0, -0.2, 0.0, 0.8, 0.0, 1., 1.0, 10.0
 ])  # fmt: skip
 
-minisim = caustics.sims.Lens_Source(
+minisim = caustics.Lens_Source(
     lens=sie, source=src, lens_light=lnslt, pixelscale=0.05, pixels_x=100
 )
 plt.imshow(minisim(x, quad_level=3), origin="lower")
 plt.axis("off")
 plt.show()
 ```
```

### Comparing `caustics-0.7.0/pyproject.toml` & `caustics-0.8.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -39,15 +39,18 @@
 Homepage = "https://mila.quebec/en/"
 Documentation = "https://caustics.readthedocs.io/en/latest/"
 Repository = "https://github.com/Ciela-Institute/caustics"
 Issues = "https://github.com/Ciela-Institute/caustics/issues"
 
 [project.optional-dependencies]
 dev = [
-    "lenstronomy==1.11.1"
+    "lenstronomy==1.11.1",
+    "pytest>=8.0,<9",
+    "pytest-cov>=4.1,<5",
+    "pre-commit>=3.6,<4"
 ]
 
 [tool.hatch.metadata.hooks.requirements_txt]
 files = ["requirements.txt"]
 
 [tool.hatch.version]
 source = "vcs"
@@ -57,7 +60,10 @@
 
 [tool.hatch.version.raw-options]
 local_scheme = "no-local-version"
 
 [tool.ruff]
 # Same as Black.
 line-length = 100
+
+[tool.pytest.ini_options]
+norecursedirs = "tests/utils"
```

### Comparing `caustics-0.7.0/PKG-INFO` & `caustics-0.8.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caustics
-Version: 0.7.0
+Version: 0.8.0
 Summary: The lensing pipeline of the future: GPU-accelerated, automatically-differentiable, highly modular. Currently under heavy development: expect interface changes and some imprecise/untested calculations.
 Project-URL: Homepage, https://mila.quebec/en/
 Project-URL: Documentation, https://caustics.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/Ciela-Institute/caustics
 Project-URL: Issues, https://github.com/Ciela-Institute/caustics/issues
 Author-email: Connor Stone <connor.stone@mila.quebec>, Alexandre Adam <alexandre.adam@mila.quebec>, UW SSEC <ssec@uw.edu>
 License: MIT License
@@ -36,19 +36,24 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Requires-Dist: astropy<6.0.0,>=5.2.1
 Requires-Dist: graphviz==0.20.1
 Requires-Dist: h5py>=3.8.0
 Requires-Dist: levmarq-torch==0.0.1
+Requires-Dist: numba<0.59.0,>=0.58.1
 Requires-Dist: numpy>=1.23.5
+Requires-Dist: safetensors>=0.4.1
 Requires-Dist: scipy>=1.8.0
 Requires-Dist: torch>=2.0.0
 Provides-Extra: dev
 Requires-Dist: lenstronomy==1.11.1; extra == 'dev'
+Requires-Dist: pre-commit<4,>=3.6; extra == 'dev'
+Requires-Dist: pytest-cov<5,>=4.1; extra == 'dev'
+Requires-Dist: pytest<9,>=8.0; extra == 'dev'
 Description-Content-Type: text/markdown
 
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="https://github.com/Ciela-Institute/caustics/blob/main/media/caustics_logo.png?raw=true">
   <source media="(prefers-color-scheme: light)" srcset="https://github.com/Ciela-Institute/caustics/blob/main/media/caustics_logo_white.png?raw=true">
   <img alt="caustics logo" src="media/caustics_logo.png" width="70%">
 </picture>
@@ -77,27 +82,27 @@
 ## Minimal Example
 
 ```python
 import matplotlib.pyplot as plt
 import caustics
 import torch
 
-cosmology = caustics.cosmology.FlatLambdaCDM()
-sie = caustics.lenses.SIE(cosmology=cosmology, name="lens")
-src = caustics.light.Sersic(name="source")
-lnslt = caustics.light.Sersic(name="lenslight")
+cosmology = caustics.FlatLambdaCDM()
+sie = caustics.SIE(cosmology=cosmology, name="lens")
+src = caustics.Sersic(name="source")
+lnslt = caustics.Sersic(name="lenslight")
 
 x = torch.tensor([
 #   z_s  z_l   x0   y0   q    phi     b    x0   y0   q     phi    n    Re
     1.5, 0.5, -0.2, 0.0, 0.4, 1.5708, 1.7, 0.0, 0.0, 0.5, -0.985, 1.3, 1.0,
 #   Ie    x0   y0   q    phi  n   Re   Ie
     5.0, -0.2, 0.0, 0.8, 0.0, 1., 1.0, 10.0
 ])  # fmt: skip
 
-minisim = caustics.sims.Lens_Source(
+minisim = caustics.Lens_Source(
     lens=sie, source=src, lens_light=lnslt, pixelscale=0.05, pixels_x=100
 )
 plt.imshow(minisim(x, quad_level=3), origin="lower")
 plt.axis("off")
 plt.show()
 ```
```

