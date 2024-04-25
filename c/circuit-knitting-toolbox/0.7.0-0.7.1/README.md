# Comparing `tmp/circuit_knitting_toolbox-0.7.0.tar.gz` & `tmp/circuit_knitting_toolbox-0.7.1.tar.gz`

## Comparing `circuit_knitting_toolbox-0.7.0.tar` & `circuit_knitting_toolbox-0.7.1.tar`

### file list

```diff
@@ -1,181 +1,184 @@
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/.dockerignore
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/.git-blame-ignore-revs
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/.mergify.yml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/.mypy.ini
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/.ruff.toml
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/CITATION.bib
--rw-r--r--   0        0        0     6153 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/CONTRIBUTING.md
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/Dockerfile
--rw-r--r--   0        0        0     6407 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/INSTALL.rst
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/SECURITY.md
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/compose.yaml
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/setup.py
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/tox.ini
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/.github/dependabot.yml
--rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/.github/workflows/README.md
--rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/.github/workflows/citation.yml
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/.github/workflows/coverage.yml
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/.github/workflows/docker.yml
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/.github/workflows/docs.yml
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/.github/workflows/lint.yml
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/.github/workflows/release.yml
--rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/.github/workflows/test_development_versions.yml
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/.github/workflows/test_latest_versions.yml
--rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/.github/workflows/test_minimum_versions.yml
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/circuit_knitting/__init__.py
--rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/circuit_knitting/cutting/__init__.py
--rw-r--r--   0        0        0     6040 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/circuit_knitting/cutting/automated_cut_finding.py
--rw-r--r--   0        0        0    10276 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/circuit_knitting/cutting/cutting_decomposition.py
--rw-r--r--   0        0        0    16980 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/circuit_knitting/cutting/cutting_experiments.py
--rw-r--r--   0        0        0     9505 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/circuit_knitting/cutting/cutting_reconstruction.py
--rw-r--r--   0        0        0     6690 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/circuit_knitting/cutting/wire_cutting_transforms.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/circuit_knitting/cutting/cut_finding/__init__.py
--rw-r--r--   0        0        0    15497 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/circuit_knitting/cutting/cut_finding/best_first_search.py
--rw-r--r--   0        0        0     6327 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/circuit_knitting/cutting/cut_finding/cco_utils.py
--rw-r--r--   0        0        0    19543 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/circuit_knitting/cutting/cut_finding/circuit_interface.py
--rw-r--r--   0        0        0    13653 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/circuit_knitting/cutting/cut_finding/cut_optimization.py
--rw-r--r--   0        0        0    14952 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/circuit_knitting/cutting/cut_finding/cutting_actions.py
--rw-r--r--   0        0        0    19661 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/circuit_knitting/cutting/cut_finding/disjoint_subcircuits_state.py
--rw-r--r--   0        0        0     7314 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/circuit_knitting/cutting/cut_finding/lo_cuts_optimizer.py
--rw-r--r--   0        0        0     5120 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/circuit_knitting/cutting/cut_finding/optimization_settings.py
--rw-r--r--   0        0        0     7810 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/circuit_knitting/cutting/cut_finding/search_space_generator.py
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/circuit_knitting/cutting/cutqc/__init__.py
--rw-r--r--   0        0        0    20995 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/circuit_knitting/cutting/cutqc/dynamic_definition.py
--rw-r--r--   0        0        0    21451 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/circuit_knitting/cutting/cutqc/mip_model.py
--rw-r--r--   0        0        0    40187 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/circuit_knitting/cutting/cutqc/wire_cutting.py
--rw-r--r--   0        0        0    16502 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/circuit_knitting/cutting/cutqc/wire_cutting_evaluation.py
--rw-r--r--   0        0        0    20311 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/circuit_knitting/cutting/cutqc/wire_cutting_post_processing.py
--rw-r--r--   0        0        0     6114 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/circuit_knitting/cutting/cutqc/wire_cutting_verification.py
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/circuit_knitting/cutting/instructions/__init__.py
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/circuit_knitting/cutting/instructions/cut_wire.py
--rw-r--r--   0        0        0     3045 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/circuit_knitting/cutting/instructions/move.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/circuit_knitting/cutting/qpd/__init__.py
--rw-r--r--   0        0        0     9642 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/circuit_knitting/cutting/qpd/decompose.py
--rw-r--r--   0        0        0    19038 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/circuit_knitting/cutting/qpd/decompositions.py
--rw-r--r--   0        0        0     4850 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/circuit_knitting/cutting/qpd/qpd_basis.py
--rw-r--r--   0        0        0    18063 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/circuit_knitting/cutting/qpd/weights.py
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/circuit_knitting/cutting/qpd/instructions/__init__.py
--rw-r--r--   0        0        0     6957 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/circuit_knitting/cutting/qpd/instructions/qpd_gate.py
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/circuit_knitting/cutting/qpd/instructions/qpd_measure.py
--rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/circuit_knitting/utils/__init__.py
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/circuit_knitting/utils/bitwise.py
--rw-r--r--   0        0        0     4552 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/circuit_knitting/utils/conversion.py
--rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/circuit_knitting/utils/iteration.py
--rw-r--r--   0        0        0     8566 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/circuit_knitting/utils/metrics.py
--rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/circuit_knitting/utils/observable_grouping.py
--rw-r--r--   0        0        0     7600 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/circuit_knitting/utils/simulation.py
--rw-r--r--   0        0        0    10432 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/circuit_knitting/utils/transforms.py
--rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/circuit_knitting/utils/transpiler_passes.py
--rw-r--r--   0        0        0     4292 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/docs/conf.py
--rw-r--r--   0        0        0     2386 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/docs/index.rst
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/docs/install.rst
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/docs/release-notes.rst
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/docs/_templates/autosummary/class_no_inherited_members.rst
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/docs/apidocs/circuit_cutting.rst
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/docs/apidocs/index.rst
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/docs/apidocs/utils.rst
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/docs/circuit_cutting/cutqc/README.rst
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/docs/circuit_cutting/cutqc/index.rst
--rw-r--r--   0        0        0   163408 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/docs/circuit_cutting/cutqc/tutorials/tutorial_1_automatic_cut_finding.ipynb
--rw-r--r--   0        0        0   261527 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/docs/circuit_cutting/cutqc/tutorials/tutorial_2_manual_cutting.ipynb
--rw-r--r--   0        0        0    24570 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/docs/circuit_cutting/explanation/index.rst
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/docs/circuit_cutting/how-tos/README.rst
--rw-r--r--   0        0        0     3530 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/docs/circuit_cutting/how-tos/how_to_generate_exact_quasi_dists_from_sampler.ipynb
--rw-r--r--   0        0        0    54615 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/docs/circuit_cutting/how-tos/how_to_generate_exact_sampling_coefficients.ipynb
--rw-r--r--   0        0        0   193545 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/docs/circuit_cutting/how-tos/how_to_specify_cut_wires.ipynb
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/docs/circuit_cutting/how-tos/index.rst
--rw-r--r--   0        0        0    63032 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/docs/circuit_cutting/tutorials/01_gate_cutting_to_reduce_circuit_width.ipynb
--rw-r--r--   0        0        0   188807 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/docs/circuit_cutting/tutorials/02_gate_cutting_to_reduce_circuit_depth.ipynb
--rw-r--r--   0        0        0   147948 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/docs/circuit_cutting/tutorials/03_wire_cutting_via_move_instruction.ipynb
--rw-r--r--   0        0        0   199049 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/docs/circuit_cutting/tutorials/04_automatic_cut_finding.ipynb
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/docs/circuit_cutting/tutorials/README.rst
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/docs/circuit_cutting/tutorials/index.rst
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/releasenotes/config.yaml
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/releasenotes/notes/0.1/dep-versions-383f4a21044cf599.yaml
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/releasenotes/notes/0.1/deprecate-py37-5ef642682641aeb8.yaml
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/releasenotes/notes/0.1/migrate-to-qiskit-nature-0.5.0-96e90cd48f36d731.yaml
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/releasenotes/notes/0.1/optional-cplex-f578dabd9d1a83f8.yaml
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/releasenotes/notes/0.2/cutqc-package-98dc0e9a3f81ff16.yaml
--rw-r--r--   0        0        0     3648 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/releasenotes/notes/0.2/gate-cutting-workflow-ebbedbdb1313b258.yaml
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/releasenotes/notes/0.2/remove-py37-0ca8b41847e64d43.yaml
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/releasenotes/notes/0.3/additional-gates-f4ed6c0e8dc3a9be.yaml
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/releasenotes/notes/0.3/automatic-partition-labels-f90428f66ec5543a.yaml
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/releasenotes/notes/0.3/batch-by-sampler-c4ae836df9997b1d.yaml
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/releasenotes/notes/0.3/cutqc-dynamic-definition-78f8bdfe82c9f839.yaml
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/releasenotes/notes/0.3/deprecate-decompose-gates-318e0393be733b52.yaml
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/releasenotes/notes/0.3/dx-qpd-inst-bug-fe9c50dad716b848.yaml
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/releasenotes/notes/0.3/ef-results-bug-5aa84ca5611dd827.yaml
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/releasenotes/notes/0.3/explicit-numpy-dependency-fdd89846b37a8d4c.yaml
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/releasenotes/notes/0.3/fixed-hartree-fock-447c33a956ffea84.yaml
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/releasenotes/notes/0.3/generate-qpd-weights-mixture-79c1c420105c8564.yaml
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/releasenotes/notes/0.3/prepare-0.3-d9049766293a3be7.yaml
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/releasenotes/notes/0.3/qpd_basis_from_instruction-6f46489c395ba20b.yaml
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/releasenotes/notes/0.3/remove-opflow-177bb07ba0e68002.yaml
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/releasenotes/notes/0.3/rename-top-level-import-bad074e7a8f348c9.yaml
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/releasenotes/notes/0.3/two-qubit-wire-cutting-27aff379403ea226.yaml
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/releasenotes/notes/0.3/update-qpdgate-labels-612e7d355ae1c1a3.yaml
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/releasenotes/notes/0.4/generate-experiments-2ac773442132c78d.yaml
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/releasenotes/notes/0.4/prepare-0.4-4781e468fe35315c.yaml
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/releasenotes/notes/0.4/qiskit-metapackage-e755916a18b4c62c.yaml
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/releasenotes/notes/0.4/refactor-evaluate-05fe26e94ff68166.yaml
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/releasenotes/notes/0.4/refactor-reconstruct-45e00c3df1bdd4ff.yaml
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/releasenotes/notes/0.5/deprecate-execute_experiments-b96e39653546dcc1.yaml
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/releasenotes/notes/0.5/prepare-0.5-1057fa4d83bf26dc.yaml
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/releasenotes/notes/0.5/qiskit-algorithms-ec3fe782619bab45.yaml
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/releasenotes/notes/0.5/qiskit-nature-pinned-c359e3933bfef993.yaml
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/releasenotes/notes/0.5/register_order_swapped-5b07fb661c6250f9.yaml
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/releasenotes/notes/0.5/remove-wire-cutting-ad0e7ab8af699561.yaml
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/releasenotes/notes/0.6/qiskit-0.45-required-5eec7abe45b88ecc.yaml
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/releasenotes/notes/0.6/qpdgate-serialization-710ce2fc6ab898e0.yaml
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/releasenotes/notes/0.6/remove-QPDBasis-from-gate-7c2d232e7de8dbc3.yaml
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/releasenotes/notes/0.6/remove-ckt-path-2386dc156b1ed9ca.yaml
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/releasenotes/notes/0.6/remove-decompose-gates-d4f78df2f77cc031.yaml
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/releasenotes/notes/0.6/remove-execute-experiments-32bd1bdd1cd1f5d5.yaml
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/releasenotes/notes/0.6/remove-forging-340dc643092a747a.yaml
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/releasenotes/notes/0.6/remove-generate-qpd-samples-63b160fd9280b0a9.yaml
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/releasenotes/notes/0.6/remove-qpdbasis-from-gate-5c66c0b2211012f0.yaml
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/releasenotes/notes/0.6/remove-redundant-resets-1893a61a341e6ce8.yaml
--rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/releasenotes/notes/0.7/automatic-cut-finding-696556915e347138.yaml
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/releasenotes/notes/0.7/bump-dependency-versions-d5dc3b10ba842f2d.yaml
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/releasenotes/notes/0.7/cutting-samplerv2-603b0c631a3330df.yaml
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/releasenotes/notes/0.7/deprecate-cutqc-7541c514bd96fb05.yaml
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/releasenotes/notes/0.7/prepare-0.7.0-48b344ae77523c34.yaml
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/releasenotes/notes/0.7/qpd_py_gone-854d6fd5d070f844.yaml
--rw-r--r--   0        0        0     3681 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/test/README.md
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/test/__init__.py
--rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/test/conftest.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/test/cutting/__init__.py
--rw-r--r--   0        0        0     5177 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/test/cutting/test_cutqc.py
--rw-r--r--   0        0        0    12136 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/test/cutting/test_cutting_decomposition.py
--rw-r--r--   0        0        0     9847 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/test/cutting/test_cutting_experiments.py
--rw-r--r--   0        0        0     5192 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/test/cutting/test_cutting_reconstruction.py
--rw-r--r--   0        0        0     6943 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/test/cutting/test_cutting_roundtrip.py
--rw-r--r--   0        0        0     7438 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/test/cutting/test_cutting_workflows.py
--rw-r--r--   0        0        0     3523 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/test/cutting/test_find_cuts.py
--rw-r--r--   0        0        0    11314 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/test/cutting/test_wire_cutting_transforms.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/test/cutting/cut_finding/__init__.py
--rw-r--r--   0        0        0     5122 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/test/cutting/cut_finding/test_best_first_search.py
--rw-r--r--   0        0        0     5334 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/test/cutting/cut_finding/test_cco_utils.py
--rw-r--r--   0        0        0     7120 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/test/cutting/cut_finding/test_circuit_interfaces.py
--rw-r--r--   0        0        0    12686 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/test/cutting/cut_finding/test_cut_finder_results.py
--rw-r--r--   0        0        0     5637 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/test/cutting/cut_finding/test_cutting_actions.py
--rw-r--r--   0        0        0     7773 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/test/cutting/cut_finding/test_disjoint_subcircuits_state.py
--rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/test/cutting/cut_finding/test_optimization_settings.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/test/cutting/qpd/__init__.py
--rw-r--r--   0        0        0    21023 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/test/cutting/qpd/test_qpd.py
--rw-r--r--   0        0        0     7465 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/test/cutting/qpd/test_qpd_basis.py
--rw-r--r--   0        0        0     3968 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/test/cutting/qpd/instructions/test_qpd_gate.py
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/test/cutting/qpd/instructions/test_qpd_measure.py
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/test/qasm_circuits/circuit_find_cuts_test.qasm
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/test/utils/test_iteration.py
--rw-r--r--   0        0        0     4218 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/test/utils/test_observable_grouping.py
--rw-r--r--   0        0        0     4428 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/test/utils/test_simulation.py
--rw-r--r--   0        0        0    16770 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/test/utils/test_transforms.py
--rw-r--r--   0        0        0     4107 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/test/utils/test_transpiler_passes.py
--rwxr-xr-x   0        0        0     4645 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/tools/extremal-python-dependencies.py
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/.gitignore
--rw-r--r--   0        0        0    11416 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/LICENSE.txt
--rw-r--r--   0        0        0     6058 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/README.md
--rw-r--r--   0        0        0     3593 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/pyproject.toml
--rw-r--r--   0        0        0    23343 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/.dockerignore
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/.git-blame-ignore-revs
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/.mergify.yml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/.mypy.ini
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/.ruff.toml
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/CITATION.bib
+-rw-r--r--   0        0        0     6153 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/Dockerfile
+-rw-r--r--   0        0        0     6407 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/INSTALL.rst
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/SECURITY.md
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/compose.yaml
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/setup.py
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/tox.ini
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/.github/dependabot.yml
+-rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/.github/workflows/README.md
+-rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/.github/workflows/citation.yml
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/.github/workflows/docker.yml
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/.github/workflows/lint.yml
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/.github/workflows/test_development_versions.yml
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/.github/workflows/test_latest_versions.yml
+-rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/.github/workflows/test_minimum_versions.yml
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/circuit_knitting/__init__.py
+-rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/circuit_knitting/cutting/__init__.py
+-rw-r--r--   0        0        0     6040 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/circuit_knitting/cutting/automated_cut_finding.py
+-rw-r--r--   0        0        0    10276 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/circuit_knitting/cutting/cutting_decomposition.py
+-rw-r--r--   0        0        0    18939 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/circuit_knitting/cutting/cutting_experiments.py
+-rw-r--r--   0        0        0     9505 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/circuit_knitting/cutting/cutting_reconstruction.py
+-rw-r--r--   0        0        0     6690 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/circuit_knitting/cutting/wire_cutting_transforms.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/circuit_knitting/cutting/cut_finding/__init__.py
+-rw-r--r--   0        0        0    15497 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/circuit_knitting/cutting/cut_finding/best_first_search.py
+-rw-r--r--   0        0        0     6327 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/circuit_knitting/cutting/cut_finding/cco_utils.py
+-rw-r--r--   0        0        0    19543 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/circuit_knitting/cutting/cut_finding/circuit_interface.py
+-rw-r--r--   0        0        0    13653 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/circuit_knitting/cutting/cut_finding/cut_optimization.py
+-rw-r--r--   0        0        0    14952 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/circuit_knitting/cutting/cut_finding/cutting_actions.py
+-rw-r--r--   0        0        0    19661 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/circuit_knitting/cutting/cut_finding/disjoint_subcircuits_state.py
+-rw-r--r--   0        0        0     7314 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/circuit_knitting/cutting/cut_finding/lo_cuts_optimizer.py
+-rw-r--r--   0        0        0     5120 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/circuit_knitting/cutting/cut_finding/optimization_settings.py
+-rw-r--r--   0        0        0     7810 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/circuit_knitting/cutting/cut_finding/search_space_generator.py
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/circuit_knitting/cutting/cutqc/__init__.py
+-rw-r--r--   0        0        0    20995 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/circuit_knitting/cutting/cutqc/dynamic_definition.py
+-rw-r--r--   0        0        0    21451 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/circuit_knitting/cutting/cutqc/mip_model.py
+-rw-r--r--   0        0        0    40187 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/circuit_knitting/cutting/cutqc/wire_cutting.py
+-rw-r--r--   0        0        0    16502 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/circuit_knitting/cutting/cutqc/wire_cutting_evaluation.py
+-rw-r--r--   0        0        0    20311 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/circuit_knitting/cutting/cutqc/wire_cutting_post_processing.py
+-rw-r--r--   0        0        0     6114 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/circuit_knitting/cutting/cutqc/wire_cutting_verification.py
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/circuit_knitting/cutting/instructions/__init__.py
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/circuit_knitting/cutting/instructions/cut_wire.py
+-rw-r--r--   0        0        0     3045 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/circuit_knitting/cutting/instructions/move.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/circuit_knitting/cutting/qpd/__init__.py
+-rw-r--r--   0        0        0     9647 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/circuit_knitting/cutting/qpd/decompose.py
+-rw-r--r--   0        0        0    19038 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/circuit_knitting/cutting/qpd/decompositions.py
+-rw-r--r--   0        0        0     4850 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/circuit_knitting/cutting/qpd/qpd_basis.py
+-rw-r--r--   0        0        0    18063 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/circuit_knitting/cutting/qpd/weights.py
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/circuit_knitting/cutting/qpd/instructions/__init__.py
+-rw-r--r--   0        0        0     6957 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/circuit_knitting/cutting/qpd/instructions/qpd_gate.py
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/circuit_knitting/cutting/qpd/instructions/qpd_measure.py
+-rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/circuit_knitting/utils/__init__.py
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/circuit_knitting/utils/bitwise.py
+-rw-r--r--   0        0        0     4552 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/circuit_knitting/utils/conversion.py
+-rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/circuit_knitting/utils/iteration.py
+-rw-r--r--   0        0        0     8566 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/circuit_knitting/utils/metrics.py
+-rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/circuit_knitting/utils/observable_grouping.py
+-rw-r--r--   0        0        0     7600 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/circuit_knitting/utils/simulation.py
+-rw-r--r--   0        0        0    10432 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/circuit_knitting/utils/transforms.py
+-rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/circuit_knitting/utils/transpiler_passes.py
+-rw-r--r--   0        0        0     4292 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/docs/conf.py
+-rw-r--r--   0        0        0     2386 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/docs/index.rst
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/docs/install.rst
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/docs/release-notes.rst
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/docs/_templates/autosummary/class_no_inherited_members.rst
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/docs/apidocs/circuit_cutting.rst
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/docs/apidocs/index.rst
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/docs/apidocs/utils.rst
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/docs/circuit_cutting/cutqc/README.rst
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/docs/circuit_cutting/cutqc/index.rst
+-rw-r--r--   0        0        0   163408 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/docs/circuit_cutting/cutqc/tutorials/tutorial_1_automatic_cut_finding.ipynb
+-rw-r--r--   0        0        0   261527 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/docs/circuit_cutting/cutqc/tutorials/tutorial_2_manual_cutting.ipynb
+-rw-r--r--   0        0        0    24570 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/docs/circuit_cutting/explanation/index.rst
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/docs/circuit_cutting/how-tos/README.rst
+-rw-r--r--   0        0        0     3530 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/docs/circuit_cutting/how-tos/how_to_generate_exact_quasi_dists_from_sampler.ipynb
+-rw-r--r--   0        0        0    54615 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/docs/circuit_cutting/how-tos/how_to_generate_exact_sampling_coefficients.ipynb
+-rw-r--r--   0        0        0   193545 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/docs/circuit_cutting/how-tos/how_to_specify_cut_wires.ipynb
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/docs/circuit_cutting/how-tos/index.rst
+-rw-r--r--   0        0        0    63032 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/docs/circuit_cutting/tutorials/01_gate_cutting_to_reduce_circuit_width.ipynb
+-rw-r--r--   0        0        0   188807 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/docs/circuit_cutting/tutorials/02_gate_cutting_to_reduce_circuit_depth.ipynb
+-rw-r--r--   0        0        0   147948 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/docs/circuit_cutting/tutorials/03_wire_cutting_via_move_instruction.ipynb
+-rw-r--r--   0        0        0   199049 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/docs/circuit_cutting/tutorials/04_automatic_cut_finding.ipynb
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/docs/circuit_cutting/tutorials/README.rst
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/docs/circuit_cutting/tutorials/index.rst
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/releasenotes/config.yaml
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/releasenotes/notes/0.1/dep-versions-383f4a21044cf599.yaml
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/releasenotes/notes/0.1/deprecate-py37-5ef642682641aeb8.yaml
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/releasenotes/notes/0.1/migrate-to-qiskit-nature-0.5.0-96e90cd48f36d731.yaml
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/releasenotes/notes/0.1/optional-cplex-f578dabd9d1a83f8.yaml
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/releasenotes/notes/0.2/cutqc-package-98dc0e9a3f81ff16.yaml
+-rw-r--r--   0        0        0     3648 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/releasenotes/notes/0.2/gate-cutting-workflow-ebbedbdb1313b258.yaml
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/releasenotes/notes/0.2/remove-py37-0ca8b41847e64d43.yaml
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/releasenotes/notes/0.3/additional-gates-f4ed6c0e8dc3a9be.yaml
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/releasenotes/notes/0.3/automatic-partition-labels-f90428f66ec5543a.yaml
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/releasenotes/notes/0.3/batch-by-sampler-c4ae836df9997b1d.yaml
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/releasenotes/notes/0.3/cutqc-dynamic-definition-78f8bdfe82c9f839.yaml
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/releasenotes/notes/0.3/deprecate-decompose-gates-318e0393be733b52.yaml
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/releasenotes/notes/0.3/dx-qpd-inst-bug-fe9c50dad716b848.yaml
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/releasenotes/notes/0.3/ef-results-bug-5aa84ca5611dd827.yaml
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/releasenotes/notes/0.3/explicit-numpy-dependency-fdd89846b37a8d4c.yaml
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/releasenotes/notes/0.3/fixed-hartree-fock-447c33a956ffea84.yaml
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/releasenotes/notes/0.3/generate-qpd-weights-mixture-79c1c420105c8564.yaml
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/releasenotes/notes/0.3/prepare-0.3-d9049766293a3be7.yaml
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/releasenotes/notes/0.3/qpd_basis_from_instruction-6f46489c395ba20b.yaml
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/releasenotes/notes/0.3/remove-opflow-177bb07ba0e68002.yaml
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/releasenotes/notes/0.3/rename-top-level-import-bad074e7a8f348c9.yaml
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/releasenotes/notes/0.3/two-qubit-wire-cutting-27aff379403ea226.yaml
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/releasenotes/notes/0.3/update-qpdgate-labels-612e7d355ae1c1a3.yaml
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/releasenotes/notes/0.4/generate-experiments-2ac773442132c78d.yaml
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/releasenotes/notes/0.4/prepare-0.4-4781e468fe35315c.yaml
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/releasenotes/notes/0.4/qiskit-metapackage-e755916a18b4c62c.yaml
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/releasenotes/notes/0.4/refactor-evaluate-05fe26e94ff68166.yaml
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/releasenotes/notes/0.4/refactor-reconstruct-45e00c3df1bdd4ff.yaml
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/releasenotes/notes/0.5/deprecate-execute_experiments-b96e39653546dcc1.yaml
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/releasenotes/notes/0.5/prepare-0.5-1057fa4d83bf26dc.yaml
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/releasenotes/notes/0.5/qiskit-algorithms-ec3fe782619bab45.yaml
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/releasenotes/notes/0.5/qiskit-nature-pinned-c359e3933bfef993.yaml
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/releasenotes/notes/0.5/register_order_swapped-5b07fb661c6250f9.yaml
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/releasenotes/notes/0.5/remove-wire-cutting-ad0e7ab8af699561.yaml
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/releasenotes/notes/0.6/qiskit-0.45-required-5eec7abe45b88ecc.yaml
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/releasenotes/notes/0.6/qpdgate-serialization-710ce2fc6ab898e0.yaml
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/releasenotes/notes/0.6/remove-QPDBasis-from-gate-7c2d232e7de8dbc3.yaml
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/releasenotes/notes/0.6/remove-ckt-path-2386dc156b1ed9ca.yaml
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/releasenotes/notes/0.6/remove-decompose-gates-d4f78df2f77cc031.yaml
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/releasenotes/notes/0.6/remove-execute-experiments-32bd1bdd1cd1f5d5.yaml
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/releasenotes/notes/0.6/remove-forging-340dc643092a747a.yaml
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/releasenotes/notes/0.6/remove-generate-qpd-samples-63b160fd9280b0a9.yaml
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/releasenotes/notes/0.6/remove-qpdbasis-from-gate-5c66c0b2211012f0.yaml
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/releasenotes/notes/0.6/remove-redundant-resets-1893a61a341e6ce8.yaml
+-rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/releasenotes/notes/0.7/automatic-cut-finding-696556915e347138.yaml
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/releasenotes/notes/0.7/bump-dependency-versions-d5dc3b10ba842f2d.yaml
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/releasenotes/notes/0.7/cutting-samplerv2-603b0c631a3330df.yaml
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/releasenotes/notes/0.7/deprecate-cutqc-7541c514bd96fb05.yaml
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/releasenotes/notes/0.7/nonzero-register-size-e112e34417ff79b9.yaml
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/releasenotes/notes/0.7/prepare-0.7.0-48b344ae77523c34.yaml
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/releasenotes/notes/0.7/prepare-0.7.1-a18412f0e07ece06.yaml
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/releasenotes/notes/0.7/qpd_py_gone-854d6fd5d070f844.yaml
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/releasenotes/notes/0.7/subexperiment-gen-speedup-41a4e8679353d1d9.yaml
+-rw-r--r--   0        0        0     3681 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/test/README.md
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/test/__init__.py
+-rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/test/conftest.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/test/cutting/__init__.py
+-rw-r--r--   0        0        0     5177 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/test/cutting/test_cutqc.py
+-rw-r--r--   0        0        0    12136 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/test/cutting/test_cutting_decomposition.py
+-rw-r--r--   0        0        0    13254 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/test/cutting/test_cutting_experiments.py
+-rw-r--r--   0        0        0     5192 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/test/cutting/test_cutting_reconstruction.py
+-rw-r--r--   0        0        0     6943 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/test/cutting/test_cutting_roundtrip.py
+-rw-r--r--   0        0        0     7438 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/test/cutting/test_cutting_workflows.py
+-rw-r--r--   0        0        0     3523 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/test/cutting/test_find_cuts.py
+-rw-r--r--   0        0        0    11314 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/test/cutting/test_wire_cutting_transforms.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/test/cutting/cut_finding/__init__.py
+-rw-r--r--   0        0        0     5122 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/test/cutting/cut_finding/test_best_first_search.py
+-rw-r--r--   0        0        0     5334 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/test/cutting/cut_finding/test_cco_utils.py
+-rw-r--r--   0        0        0     7120 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/test/cutting/cut_finding/test_circuit_interfaces.py
+-rw-r--r--   0        0        0    12686 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/test/cutting/cut_finding/test_cut_finder_results.py
+-rw-r--r--   0        0        0     5637 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/test/cutting/cut_finding/test_cutting_actions.py
+-rw-r--r--   0        0        0     7773 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/test/cutting/cut_finding/test_disjoint_subcircuits_state.py
+-rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/test/cutting/cut_finding/test_optimization_settings.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/test/cutting/qpd/__init__.py
+-rw-r--r--   0        0        0    21023 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/test/cutting/qpd/test_qpd.py
+-rw-r--r--   0        0        0     7465 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/test/cutting/qpd/test_qpd_basis.py
+-rw-r--r--   0        0        0     3968 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/test/cutting/qpd/instructions/test_qpd_gate.py
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/test/cutting/qpd/instructions/test_qpd_measure.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/test/qasm_circuits/circuit_find_cuts_test.qasm
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/test/utils/test_iteration.py
+-rw-r--r--   0        0        0     4218 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/test/utils/test_observable_grouping.py
+-rw-r--r--   0        0        0     4428 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/test/utils/test_simulation.py
+-rw-r--r--   0        0        0    16770 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/test/utils/test_transforms.py
+-rw-r--r--   0        0        0     4107 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/test/utils/test_transpiler_passes.py
+-rwxr-xr-x   0        0        0     4645 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/tools/extremal-python-dependencies.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/.gitignore
+-rw-r--r--   0        0        0    11416 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/LICENSE.txt
+-rw-r--r--   0        0        0     6058 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/README.md
+-rw-r--r--   0        0        0     3593 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0    23343 2020-02-02 00:00:00.000000 circuit_knitting_toolbox-0.7.1/PKG-INFO
```

### Comparing `circuit_knitting_toolbox-0.7.0/.dockerignore` & `circuit_knitting_toolbox-0.7.1/.dockerignore`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/CITATION.bib` & `circuit_knitting_toolbox-0.7.1/CITATION.bib`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/CODE_OF_CONDUCT.md` & `circuit_knitting_toolbox-0.7.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/CONTRIBUTING.md` & `circuit_knitting_toolbox-0.7.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/Dockerfile` & `circuit_knitting_toolbox-0.7.1/Dockerfile`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/INSTALL.rst` & `circuit_knitting_toolbox-0.7.1/INSTALL.rst`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/SECURITY.md` & `circuit_knitting_toolbox-0.7.1/SECURITY.md`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/compose.yaml` & `circuit_knitting_toolbox-0.7.1/compose.yaml`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/tox.ini` & `circuit_knitting_toolbox-0.7.1/tox.ini`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/.github/workflows/README.md` & `circuit_knitting_toolbox-0.7.1/.github/workflows/README.md`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/.github/workflows/citation.yml` & `circuit_knitting_toolbox-0.7.1/.github/workflows/citation.yml`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/.github/workflows/coverage.yml` & `circuit_knitting_toolbox-0.7.1/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/.github/workflows/docker.yml` & `circuit_knitting_toolbox-0.7.1/.github/workflows/docker.yml`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/.github/workflows/docs.yml` & `circuit_knitting_toolbox-0.7.1/.github/workflows/docs.yml`

 * *Files 1% similar despite different names*

```diff
@@ -47,11 +47,11 @@
         if: always()
         uses: actions/upload-artifact@v4
         with:
           name: ckt_html_docs
           path: ./artifact
       - name: Deploy docs
         if: ${{ github.ref == 'refs/heads/stable/0.7' }}
-        uses: peaceiris/actions-gh-pages@v3
+        uses: peaceiris/actions-gh-pages@v4
         with:
           github_token: ${{ secrets.GITHUB_TOKEN }}
           publish_dir: ./docs/_build/html/
```

### Comparing `circuit_knitting_toolbox-0.7.0/.github/workflows/lint.yml` & `circuit_knitting_toolbox-0.7.1/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/.github/workflows/release.yml` & `circuit_knitting_toolbox-0.7.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/.github/workflows/test_development_versions.yml` & `circuit_knitting_toolbox-0.7.1/.github/workflows/test_development_versions.yml`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/.github/workflows/test_latest_versions.yml` & `circuit_knitting_toolbox-0.7.1/.github/workflows/test_latest_versions.yml`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     timeout-minutes: 30
     strategy:
       max-parallel: 4
       matrix:
         os: [ubuntu-latest]
         python-version: ["3.9", "3.12"]
         include:
-          - os: macos-latest
+          - os: macos-13
             python-version: "3.8"
           - os: windows-latest
             python-version: "3.10"
     steps:
       - uses: actions/checkout@v4
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v5
```

### Comparing `circuit_knitting_toolbox-0.7.0/.github/workflows/test_minimum_versions.yml` & `circuit_knitting_toolbox-0.7.1/.github/workflows/test_minimum_versions.yml`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/circuit_knitting/__init__.py` & `circuit_knitting_toolbox-0.7.1/circuit_knitting/__init__.py`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/circuit_knitting/cutting/__init__.py` & `circuit_knitting_toolbox-0.7.1/circuit_knitting/cutting/__init__.py`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/circuit_knitting/cutting/automated_cut_finding.py` & `circuit_knitting_toolbox-0.7.1/circuit_knitting/cutting/automated_cut_finding.py`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/circuit_knitting/cutting/cutting_decomposition.py` & `circuit_knitting_toolbox-0.7.1/circuit_knitting/cutting/cutting_decomposition.py`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/circuit_knitting/cutting/cutting_experiments.py` & `circuit_knitting_toolbox-0.7.1/circuit_knitting/cutting/cutting_experiments.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,20 +15,16 @@
 
 from collections import defaultdict
 from collections.abc import Sequence, Hashable
 
 import numpy as np
 from qiskit.circuit import QuantumCircuit, ClassicalRegister
 from qiskit.quantum_info import PauliList
-from qiskit.transpiler import PassManager
-from qiskit.transpiler.passes import RemoveResetInZeroState, DAGFixedPoint
-from qiskit.passmanager.flow_controllers import DoWhileController
 
 from ..utils.iteration import strict_zip
-from ..utils.transpiler_passes import RemoveFinalReset, ConsolidateResets
 from ..utils.observable_grouping import ObservableCollection, CommutingObservableGroup
 from .qpd import (
     WeightType,
     QPDBasis,
     SingleQubitQPDGate,
     TwoQubitQPDGate,
     generate_qpd_weights,
@@ -58,20 +54,14 @@
 
     In both cases, the subexperiment lists are ordered as follows:
 
         :math:`[sample_{0}observable_{0}, \ldots, sample_{0}observable_{N-1}, sample_{1}observable_{0}, \ldots, sample_{M-1}observable_{N-1}]`
 
     The coefficients will always be returned as a 1D array -- one coefficient for each unique sample.
 
-    Note that this function also runs some transpiler passes on each generated
-    circuit, namely :class:`~qiskit.transpiler.passes.RemoveResetInZeroState`,
-    :class:`.RemoveFinalReset`, and :class:`.ConsolidateResets`, in order to
-    remove unnecessary :class:`~qiskit.circuit.library.Reset`\ s from the
-    circuit that are added by the subexperiment decompositions for cut wires.
-
     Args:
         circuits: The circuit(s) to partition and separate
         observables: The observable(s) to evaluate for each unique sample
         num_samples: The number of samples to draw from the quasi-probability distribution. If set
             to infinity, the weights will be generated rigorously rather than by sampling from
             the distribution.
     Returns:
@@ -168,28 +158,19 @@
 
     # Remove initial and final resets from the subexperiments.  This will
     # enable the `Move` operation to work on backends that don't support
     # `Reset`, as long as qubits are not re-used.  See
     # https://github.com/Qiskit-Extensions/circuit-knitting-toolbox/issues/452.
     # While we are at it, we also consolidate each run of multiple resets
     # (which can arise when re-using qubits) into a single reset.
-    pass_manager = PassManager()
-    passes = [
-        RemoveResetInZeroState(),
-        RemoveFinalReset(),
-        ConsolidateResets(),
-        DAGFixedPoint(),
-    ]
-    pass_manager.append(
-        DoWhileController(
-            passes, do_while=lambda property_set: not property_set["dag_fixed_point"]
-        )
-    )
-    for label, subexperiments in subexperiments_dict.items():
-        subexperiments_dict[label] = pass_manager.run(subexperiments)
+    for subexperiments in subexperiments_dict.values():
+        for circ in subexperiments:
+            _remove_resets_in_zero_state(circ)
+            _remove_final_resets(circ)
+            _consolidate_resets(circ)
 
     # If the input was a single quantum circuit, return the subexperiments as a list
     subexperiments_out: list[QuantumCircuit] | dict[Hashable, list[QuantumCircuit]] = (
         dict(subexperiments_dict)
     )
     assert isinstance(subexperiments_out, dict)
     if isinstance(circuits, QuantumCircuit):
@@ -385,7 +366,94 @@
     # If the circuit has no measurements, the Sampler will fail.  So, we
     # measure one qubit as a temporary workaround to
     # https://github.com/Qiskit-Extensions/circuit-knitting-toolbox/issues/422
     pauli_indices = cog.pauli_indices
     if not pauli_indices:
         pauli_indices = [0]
     return pauli_indices
+
+
+def _consolidate_resets(
+    circuit: QuantumCircuit, inplace: bool = True
+) -> QuantumCircuit:
+    """Consolidate redundant resets into a single reset."""
+    if not inplace:  # pragma: no cover
+        circuit = circuit.copy()
+
+    # Keep up with whether the previous instruction on a given qubit was a reset
+    resets = [False] * circuit.num_qubits
+
+    # Remove resets which are immediately following other resets
+    remove_ids = []
+    for i, inst in enumerate(circuit.data):
+        qargs = [circuit.find_bit(q).index for q in inst.qubits]
+        if inst.operation.name == "reset":
+            if resets[qargs[0]]:
+                remove_ids.append(i)
+            else:
+                resets[qargs[0]] = True
+        else:
+            for q in qargs:
+                resets[q] = False
+
+    for i in sorted(remove_ids, reverse=True):
+        del circuit.data[i]
+
+    return circuit
+
+
+def _remove_resets_in_zero_state(
+    circuit: QuantumCircuit, inplace: bool = True
+) -> QuantumCircuit:
+    """Remove resets if they are the first instruction on a qubit."""
+    if not inplace:  # pragma: no cover
+        circuit = circuit.copy()
+
+    # Keep up with which qubits have at least one non-reset instruction
+    active_qubits: set[int] = set()
+    remove_ids = []
+    for i, inst in enumerate(circuit.data):
+        qargs = [circuit.find_bit(q).index for q in inst.qubits]
+        if inst.operation.name == "reset":
+            if qargs[0] not in active_qubits:
+                remove_ids.append(i)
+        else:
+            for q in qargs:
+                active_qubits.add(q)
+            # Early terminate once all qubits have become active
+            if len(active_qubits) == circuit.num_qubits:
+                break
+
+    for i in sorted(remove_ids, reverse=True):
+        del circuit.data[i]
+
+    return circuit
+
+
+def _remove_final_resets(
+    circuit: QuantumCircuit, inplace: bool = True
+) -> QuantumCircuit:
+    """Remove resets if they are the final instruction on a qubit."""
+    if not inplace:  # pragma: no cover
+        circuit = circuit.copy()
+
+    # Keep up with whether we are at the end of a qubit
+    # We iterate in reverse, so all qubits begin in the "end" state
+    qubit_ended = set(range(circuit.num_qubits))
+    remove_ids = []
+    num_inst = len(circuit.data)
+    for i, inst in enumerate(reversed(circuit.data)):
+        qargs = [circuit.find_bit(q).index for q in inst.qubits]
+        if inst.operation.name == "reset":
+            if qargs[0] in qubit_ended:
+                remove_ids.append(num_inst - 1 - i)
+        else:
+            for q in qargs:
+                qubit_ended.discard(q)
+            # Early terminate once all qubits have been touched
+            if not qubit_ended:
+                break
+
+    for i in sorted(remove_ids, reverse=True):
+        del circuit.data[i]
+
+    return circuit
```

### Comparing `circuit_knitting_toolbox-0.7.0/circuit_knitting/cutting/cutting_reconstruction.py` & `circuit_knitting_toolbox-0.7.1/circuit_knitting/cutting/cutting_reconstruction.py`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/circuit_knitting/cutting/wire_cutting_transforms.py` & `circuit_knitting_toolbox-0.7.1/circuit_knitting/cutting/wire_cutting_transforms.py`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/circuit_knitting/cutting/cut_finding/best_first_search.py` & `circuit_knitting_toolbox-0.7.1/circuit_knitting/cutting/cut_finding/best_first_search.py`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/circuit_knitting/cutting/cut_finding/cco_utils.py` & `circuit_knitting_toolbox-0.7.1/circuit_knitting/cutting/cut_finding/cco_utils.py`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/circuit_knitting/cutting/cut_finding/circuit_interface.py` & `circuit_knitting_toolbox-0.7.1/circuit_knitting/cutting/cut_finding/circuit_interface.py`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/circuit_knitting/cutting/cut_finding/cut_optimization.py` & `circuit_knitting_toolbox-0.7.1/circuit_knitting/cutting/cut_finding/cut_optimization.py`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/circuit_knitting/cutting/cut_finding/cutting_actions.py` & `circuit_knitting_toolbox-0.7.1/circuit_knitting/cutting/cut_finding/cutting_actions.py`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/circuit_knitting/cutting/cut_finding/disjoint_subcircuits_state.py` & `circuit_knitting_toolbox-0.7.1/circuit_knitting/cutting/cut_finding/disjoint_subcircuits_state.py`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/circuit_knitting/cutting/cut_finding/lo_cuts_optimizer.py` & `circuit_knitting_toolbox-0.7.1/circuit_knitting/cutting/cut_finding/lo_cuts_optimizer.py`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/circuit_knitting/cutting/cut_finding/optimization_settings.py` & `circuit_knitting_toolbox-0.7.1/circuit_knitting/cutting/cut_finding/optimization_settings.py`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/circuit_knitting/cutting/cut_finding/search_space_generator.py` & `circuit_knitting_toolbox-0.7.1/circuit_knitting/cutting/cut_finding/search_space_generator.py`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/circuit_knitting/cutting/cutqc/__init__.py` & `circuit_knitting_toolbox-0.7.1/circuit_knitting/cutting/cutqc/__init__.py`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/circuit_knitting/cutting/cutqc/dynamic_definition.py` & `circuit_knitting_toolbox-0.7.1/circuit_knitting/cutting/cutqc/dynamic_definition.py`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/circuit_knitting/cutting/cutqc/mip_model.py` & `circuit_knitting_toolbox-0.7.1/circuit_knitting/cutting/cutqc/mip_model.py`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/circuit_knitting/cutting/cutqc/wire_cutting.py` & `circuit_knitting_toolbox-0.7.1/circuit_knitting/cutting/cutqc/wire_cutting.py`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/circuit_knitting/cutting/cutqc/wire_cutting_evaluation.py` & `circuit_knitting_toolbox-0.7.1/circuit_knitting/cutting/cutqc/wire_cutting_evaluation.py`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/circuit_knitting/cutting/cutqc/wire_cutting_post_processing.py` & `circuit_knitting_toolbox-0.7.1/circuit_knitting/cutting/cutqc/wire_cutting_post_processing.py`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/circuit_knitting/cutting/cutqc/wire_cutting_verification.py` & `circuit_knitting_toolbox-0.7.1/circuit_knitting/cutting/cutqc/wire_cutting_verification.py`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/circuit_knitting/cutting/instructions/__init__.py` & `circuit_knitting_toolbox-0.7.1/circuit_knitting/cutting/instructions/__init__.py`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/circuit_knitting/cutting/instructions/cut_wire.py` & `circuit_knitting_toolbox-0.7.1/circuit_knitting/cutting/instructions/cut_wire.py`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/circuit_knitting/cutting/instructions/move.py` & `circuit_knitting_toolbox-0.7.1/circuit_knitting/cutting/instructions/move.py`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/circuit_knitting/cutting/qpd/__init__.py` & `circuit_knitting_toolbox-0.7.1/circuit_knitting/cutting/qpd/__init__.py`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/circuit_knitting/cutting/qpd/decompose.py` & `circuit_knitting_toolbox-0.7.1/circuit_knitting/cutting/qpd/decompose.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,18 +141,18 @@
     # here because it refers to old indices, before the decomposition.
     qpd_measure_ids = [
         i
         for i, instruction in enumerate(circuit.data)
         if instruction.operation.name.lower() == "qpd_measure"
     ]
 
-    # Create a classical register for the qpd measurement results.  This is
-    # partly for convenience, partly to work around
-    # https://github.com/Qiskit/qiskit-aer/issues/1660.
-    reg = ClassicalRegister(len(qpd_measure_ids), name="qpd_measurements")
+    # Create a classical register for the qpd measurement results.
+    # We force at least one classical bit as a workaround to
+    # https://github.com/openqasm/qe-qasm/issues/37.
+    reg = ClassicalRegister(max(1, len(qpd_measure_ids)), name="qpd_measurements")
     circuit.add_register(reg)
 
     # Place the measurement instructions
     for idx, i in enumerate(qpd_measure_ids):
         gate = circuit.data[i]
         inst = CircuitInstruction(
             operation=Measure(), qubits=[gate.qubits], clbits=[reg[idx]]
```

### Comparing `circuit_knitting_toolbox-0.7.0/circuit_knitting/cutting/qpd/decompositions.py` & `circuit_knitting_toolbox-0.7.1/circuit_knitting/cutting/qpd/decompositions.py`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/circuit_knitting/cutting/qpd/qpd_basis.py` & `circuit_knitting_toolbox-0.7.1/circuit_knitting/cutting/qpd/qpd_basis.py`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/circuit_knitting/cutting/qpd/weights.py` & `circuit_knitting_toolbox-0.7.1/circuit_knitting/cutting/qpd/weights.py`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/circuit_knitting/cutting/qpd/instructions/__init__.py` & `circuit_knitting_toolbox-0.7.1/circuit_knitting/cutting/qpd/instructions/__init__.py`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/circuit_knitting/cutting/qpd/instructions/qpd_gate.py` & `circuit_knitting_toolbox-0.7.1/circuit_knitting/cutting/qpd/instructions/qpd_gate.py`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/circuit_knitting/cutting/qpd/instructions/qpd_measure.py` & `circuit_knitting_toolbox-0.7.1/circuit_knitting/cutting/qpd/instructions/qpd_measure.py`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/circuit_knitting/utils/__init__.py` & `circuit_knitting_toolbox-0.7.1/circuit_knitting/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/circuit_knitting/utils/bitwise.py` & `circuit_knitting_toolbox-0.7.1/circuit_knitting/utils/bitwise.py`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/circuit_knitting/utils/conversion.py` & `circuit_knitting_toolbox-0.7.1/circuit_knitting/utils/conversion.py`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/circuit_knitting/utils/iteration.py` & `circuit_knitting_toolbox-0.7.1/circuit_knitting/utils/iteration.py`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/circuit_knitting/utils/metrics.py` & `circuit_knitting_toolbox-0.7.1/circuit_knitting/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/circuit_knitting/utils/observable_grouping.py` & `circuit_knitting_toolbox-0.7.1/circuit_knitting/utils/observable_grouping.py`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/circuit_knitting/utils/simulation.py` & `circuit_knitting_toolbox-0.7.1/circuit_knitting/utils/simulation.py`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/circuit_knitting/utils/transforms.py` & `circuit_knitting_toolbox-0.7.1/circuit_knitting/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/circuit_knitting/utils/transpiler_passes.py` & `circuit_knitting_toolbox-0.7.1/circuit_knitting/utils/transpiler_passes.py`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/docs/conf.py` & `circuit_knitting_toolbox-0.7.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/docs/index.rst` & `circuit_knitting_toolbox-0.7.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/docs/_templates/autosummary/class_no_inherited_members.rst` & `circuit_knitting_toolbox-0.7.1/docs/_templates/autosummary/class_no_inherited_members.rst`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/docs/circuit_cutting/cutqc/index.rst` & `circuit_knitting_toolbox-0.7.1/docs/circuit_cutting/cutqc/index.rst`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/docs/circuit_cutting/cutqc/tutorials/tutorial_1_automatic_cut_finding.ipynb` & `circuit_knitting_toolbox-0.7.1/docs/circuit_cutting/cutqc/tutorials/tutorial_1_automatic_cut_finding.ipynb`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/docs/circuit_cutting/cutqc/tutorials/tutorial_2_manual_cutting.ipynb` & `circuit_knitting_toolbox-0.7.1/docs/circuit_cutting/cutqc/tutorials/tutorial_2_manual_cutting.ipynb`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/docs/circuit_cutting/explanation/index.rst` & `circuit_knitting_toolbox-0.7.1/docs/circuit_cutting/explanation/index.rst`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/docs/circuit_cutting/how-tos/README.rst` & `circuit_knitting_toolbox-0.7.1/docs/circuit_cutting/how-tos/README.rst`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/docs/circuit_cutting/how-tos/how_to_generate_exact_quasi_dists_from_sampler.ipynb` & `circuit_knitting_toolbox-0.7.1/docs/circuit_cutting/how-tos/how_to_generate_exact_quasi_dists_from_sampler.ipynb`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/docs/circuit_cutting/how-tos/how_to_generate_exact_sampling_coefficients.ipynb` & `circuit_knitting_toolbox-0.7.1/docs/circuit_cutting/how-tos/how_to_generate_exact_sampling_coefficients.ipynb`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/docs/circuit_cutting/how-tos/how_to_specify_cut_wires.ipynb` & `circuit_knitting_toolbox-0.7.1/docs/circuit_cutting/how-tos/how_to_specify_cut_wires.ipynb`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/docs/circuit_cutting/tutorials/01_gate_cutting_to_reduce_circuit_width.ipynb` & `circuit_knitting_toolbox-0.7.1/docs/circuit_cutting/tutorials/01_gate_cutting_to_reduce_circuit_width.ipynb`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/docs/circuit_cutting/tutorials/02_gate_cutting_to_reduce_circuit_depth.ipynb` & `circuit_knitting_toolbox-0.7.1/docs/circuit_cutting/tutorials/02_gate_cutting_to_reduce_circuit_depth.ipynb`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/docs/circuit_cutting/tutorials/03_wire_cutting_via_move_instruction.ipynb` & `circuit_knitting_toolbox-0.7.1/docs/circuit_cutting/tutorials/03_wire_cutting_via_move_instruction.ipynb`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/docs/circuit_cutting/tutorials/04_automatic_cut_finding.ipynb` & `circuit_knitting_toolbox-0.7.1/docs/circuit_cutting/tutorials/04_automatic_cut_finding.ipynb`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/releasenotes/notes/0.1/migrate-to-qiskit-nature-0.5.0-96e90cd48f36d731.yaml` & `circuit_knitting_toolbox-0.7.1/releasenotes/notes/0.1/migrate-to-qiskit-nature-0.5.0-96e90cd48f36d731.yaml`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/releasenotes/notes/0.2/gate-cutting-workflow-ebbedbdb1313b258.yaml` & `circuit_knitting_toolbox-0.7.1/releasenotes/notes/0.2/gate-cutting-workflow-ebbedbdb1313b258.yaml`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/releasenotes/notes/0.3/additional-gates-f4ed6c0e8dc3a9be.yaml` & `circuit_knitting_toolbox-0.7.1/releasenotes/notes/0.3/additional-gates-f4ed6c0e8dc3a9be.yaml`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/releasenotes/notes/0.3/automatic-partition-labels-f90428f66ec5543a.yaml` & `circuit_knitting_toolbox-0.7.1/releasenotes/notes/0.3/automatic-partition-labels-f90428f66ec5543a.yaml`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/releasenotes/notes/0.3/generate-qpd-weights-mixture-79c1c420105c8564.yaml` & `circuit_knitting_toolbox-0.7.1/releasenotes/notes/0.3/generate-qpd-weights-mixture-79c1c420105c8564.yaml`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/releasenotes/notes/0.3/prepare-0.3-d9049766293a3be7.yaml` & `circuit_knitting_toolbox-0.7.1/releasenotes/notes/0.3/prepare-0.3-d9049766293a3be7.yaml`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/releasenotes/notes/0.3/rename-top-level-import-bad074e7a8f348c9.yaml` & `circuit_knitting_toolbox-0.7.1/releasenotes/notes/0.3/rename-top-level-import-bad074e7a8f348c9.yaml`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/releasenotes/notes/0.4/generate-experiments-2ac773442132c78d.yaml` & `circuit_knitting_toolbox-0.7.1/releasenotes/notes/0.4/generate-experiments-2ac773442132c78d.yaml`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/releasenotes/notes/0.4/refactor-evaluate-05fe26e94ff68166.yaml` & `circuit_knitting_toolbox-0.7.1/releasenotes/notes/0.4/refactor-evaluate-05fe26e94ff68166.yaml`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/releasenotes/notes/0.4/refactor-reconstruct-45e00c3df1bdd4ff.yaml` & `circuit_knitting_toolbox-0.7.1/releasenotes/notes/0.4/refactor-reconstruct-45e00c3df1bdd4ff.yaml`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/releasenotes/notes/0.6/remove-redundant-resets-1893a61a341e6ce8.yaml` & `circuit_knitting_toolbox-0.7.1/releasenotes/notes/0.6/remove-redundant-resets-1893a61a341e6ce8.yaml`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/releasenotes/notes/0.7/automatic-cut-finding-696556915e347138.yaml` & `circuit_knitting_toolbox-0.7.1/releasenotes/notes/0.7/automatic-cut-finding-696556915e347138.yaml`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/releasenotes/notes/0.7/deprecate-cutqc-7541c514bd96fb05.yaml` & `circuit_knitting_toolbox-0.7.1/releasenotes/notes/0.7/deprecate-cutqc-7541c514bd96fb05.yaml`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/releasenotes/notes/0.7/prepare-0.7.0-48b344ae77523c34.yaml` & `circuit_knitting_toolbox-0.7.1/releasenotes/notes/0.7/prepare-0.7.0-48b344ae77523c34.yaml`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/test/README.md` & `circuit_knitting_toolbox-0.7.1/test/README.md`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/test/conftest.py` & `circuit_knitting_toolbox-0.7.1/test/conftest.py`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/test/cutting/test_cutqc.py` & `circuit_knitting_toolbox-0.7.1/test/cutting/test_cutqc.py`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/test/cutting/test_cutting_decomposition.py` & `circuit_knitting_toolbox-0.7.1/test/cutting/test_cutting_decomposition.py`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/test/cutting/test_cutting_reconstruction.py` & `circuit_knitting_toolbox-0.7.1/test/cutting/test_cutting_reconstruction.py`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/test/cutting/test_cutting_roundtrip.py` & `circuit_knitting_toolbox-0.7.1/test/cutting/test_cutting_roundtrip.py`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/test/cutting/test_cutting_workflows.py` & `circuit_knitting_toolbox-0.7.1/test/cutting/test_cutting_workflows.py`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/test/cutting/test_find_cuts.py` & `circuit_knitting_toolbox-0.7.1/test/cutting/test_find_cuts.py`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/test/cutting/test_wire_cutting_transforms.py` & `circuit_knitting_toolbox-0.7.1/test/cutting/test_wire_cutting_transforms.py`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/test/cutting/cut_finding/test_best_first_search.py` & `circuit_knitting_toolbox-0.7.1/test/cutting/cut_finding/test_best_first_search.py`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/test/cutting/cut_finding/test_cco_utils.py` & `circuit_knitting_toolbox-0.7.1/test/cutting/cut_finding/test_cco_utils.py`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/test/cutting/cut_finding/test_circuit_interfaces.py` & `circuit_knitting_toolbox-0.7.1/test/cutting/cut_finding/test_circuit_interfaces.py`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/test/cutting/cut_finding/test_cut_finder_results.py` & `circuit_knitting_toolbox-0.7.1/test/cutting/cut_finding/test_cut_finder_results.py`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/test/cutting/cut_finding/test_cutting_actions.py` & `circuit_knitting_toolbox-0.7.1/test/cutting/cut_finding/test_cutting_actions.py`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/test/cutting/cut_finding/test_disjoint_subcircuits_state.py` & `circuit_knitting_toolbox-0.7.1/test/cutting/cut_finding/test_disjoint_subcircuits_state.py`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/test/cutting/cut_finding/test_optimization_settings.py` & `circuit_knitting_toolbox-0.7.1/test/cutting/cut_finding/test_optimization_settings.py`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/test/cutting/qpd/test_qpd.py` & `circuit_knitting_toolbox-0.7.1/test/cutting/qpd/test_qpd.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,32 +144,32 @@
             assert sum(w for w, t in samples.values()) == pytest.approx(1)
             assert all(t == WeightType.EXACT for w, t in samples.values())
 
     def test_decompose_qpd_instructions(self):
         with self.subTest("Empty circuit"):
             circ = QuantumCircuit()
             new_circ = decompose_qpd_instructions(QuantumCircuit(), [])
-            circ.add_register(ClassicalRegister(0, name="qpd_measurements"))
+            circ.add_register(ClassicalRegister(1, name="qpd_measurements"))
             self.assertEqual(circ, new_circ)
         with self.subTest("No QPD circuit"):
             circ = QuantumCircuit(2, 1)
             circ.h(0)
             circ.cx(0, 1)
             circ.measure(1, 0)
             new_circ = decompose_qpd_instructions(circ, [])
-            circ.add_register(ClassicalRegister(0, name="qpd_measurements"))
+            circ.add_register(ClassicalRegister(1, name="qpd_measurements"))
             self.assertEqual(circ, new_circ)
         with self.subTest("Single QPD gate"):
             circ = QuantumCircuit(2)
             circ_compare = circ.copy()
             qpd_basis = QPDBasis.from_instruction(RXXGate(np.pi / 3))
             qpd_gate = TwoQubitQPDGate(qpd_basis)
             circ.data.append(CircuitInstruction(qpd_gate, qubits=[0, 1]))
             decomp_circ = decompose_qpd_instructions(circ, [[0]], map_ids=[0])
-            circ_compare.add_register(ClassicalRegister(0, name="qpd_measurements"))
+            circ_compare.add_register(ClassicalRegister(1, name="qpd_measurements"))
             self.assertEqual(decomp_circ, circ_compare)
         with self.subTest("Incorrect map index size"):
             with pytest.raises(ValueError) as e_info:
                 decomp_circ = decompose_qpd_instructions(
                     self.qpd_circuit, [[9], [20]], map_ids=[0]
                 )
             assert (
```

### Comparing `circuit_knitting_toolbox-0.7.0/test/cutting/qpd/test_qpd_basis.py` & `circuit_knitting_toolbox-0.7.1/test/cutting/qpd/test_qpd_basis.py`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/test/cutting/qpd/instructions/test_qpd_gate.py` & `circuit_knitting_toolbox-0.7.1/test/cutting/qpd/instructions/test_qpd_gate.py`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/test/cutting/qpd/instructions/test_qpd_measure.py` & `circuit_knitting_toolbox-0.7.1/test/cutting/qpd/instructions/test_qpd_measure.py`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/test/qasm_circuits/circuit_find_cuts_test.qasm` & `circuit_knitting_toolbox-0.7.1/test/qasm_circuits/circuit_find_cuts_test.qasm`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/test/utils/test_iteration.py` & `circuit_knitting_toolbox-0.7.1/test/utils/test_iteration.py`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/test/utils/test_observable_grouping.py` & `circuit_knitting_toolbox-0.7.1/test/utils/test_observable_grouping.py`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/test/utils/test_simulation.py` & `circuit_knitting_toolbox-0.7.1/test/utils/test_simulation.py`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/test/utils/test_transforms.py` & `circuit_knitting_toolbox-0.7.1/test/utils/test_transforms.py`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/test/utils/test_transpiler_passes.py` & `circuit_knitting_toolbox-0.7.1/test/utils/test_transpiler_passes.py`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/tools/extremal-python-dependencies.py` & `circuit_knitting_toolbox-0.7.1/tools/extremal-python-dependencies.py`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/.gitignore` & `circuit_knitting_toolbox-0.7.1/.gitignore`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/LICENSE.txt` & `circuit_knitting_toolbox-0.7.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/README.md` & `circuit_knitting_toolbox-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.7.0/pyproject.toml` & `circuit_knitting_toolbox-0.7.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "circuit-knitting-toolbox"
-version = "0.7.0"
+version = "0.7.1"
 description = "A software prototype for a circuit knitting toolbox which connects user applications with runtime primitives"
 readme = "README.md"
 license = {file = "LICENSE.txt"}
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
```

### Comparing `circuit_knitting_toolbox-0.7.0/PKG-INFO` & `circuit_knitting_toolbox-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: circuit-knitting-toolbox
-Version: 0.7.0
+Version: 0.7.1
 Summary: A software prototype for a circuit knitting toolbox which connects user applications with runtime primitives
 Project-URL: Documentation, https://qiskit-extensions.github.io/circuit-knitting-toolbox/
 Project-URL: Repository, https://github.com/Qiskit-Extensions/circuit-knitting-toolbox
 License:                     Copyright 2022 IBM and its contributors
         
                                          Apache License
                                    Version 2.0, January 2004
```

