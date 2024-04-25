# Comparing `tmp/oaklib-0.6.3.tar.gz` & `tmp/oaklib-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oaklib-0.6.3.tar", max compression
+gzip compressed data, was "oaklib-0.6.4.tar", max compression
```

## Comparing `oaklib-0.6.3.tar` & `oaklib-0.6.4.tar`

### file list

```diff
@@ -1,316 +1,316 @@
--rw-r--r--   0        0        0    11357 2024-04-16 00:05:41.065160 oaklib-0.6.3/LICENSE
--rw-r--r--   0        0        0     7258 2024-04-16 00:05:41.065160 oaklib-0.6.3/README.md
--rw-r--r--   0        0        0     3500 2024-04-16 00:06:13.765343 oaklib-0.6.3/pyproject.toml
--rw-r--r--   0        0        0      272 2024-04-16 00:05:41.229161 oaklib-0.6.3/src/oaklib/__init__.py
--rw-r--r--   0        0        0   232022 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/cli.py
--rw-r--r--   0        0        0       64 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/conf/__init__.py
--rw-r--r--   0        0        0      372 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/conf/go-human-input-spec.yaml
--rw-r--r--   0        0        0      162 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/conf/go-pombase-input-spec.yaml
--rw-r--r--   0        0        0      109 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/conf/hpoa-g2p-input-spec.yaml
--rw-r--r--   0        0        0      106 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/conf/hpoa-input-spec.yaml
--rw-r--r--   0        0        0     1903 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/conf/lexmatch-rules-oboinowl-default.yaml
--rw-r--r--   0        0        0     1011 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/conf/mondo-g2d-input-spec.yaml
--rw-r--r--   0        0        0      109 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/conf/mondo-gencc-input-spec.yaml
--rw-r--r--   0        0        0      529 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/conf/mondo-hpoa-g2d-input-spec.yaml
--rw-r--r--   0        0        0      118 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/conf/mondo-medgen-g2d-input-spec.yaml
--rw-r--r--   0        0        0     4730 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/conf/obograph-style.json
--rw-r--r--   0        0        0      256 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/conf/omo-to-skos.sssom.tsv
--rw-r--r--   0        0        0      131 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/conf/value-set-expander.conf.yaml
--rw-r--r--   0        0        0      149 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/constants.py
--rw-r--r--   0        0        0        0 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/converters/__init__.py
--rw-r--r--   0        0        0     1461 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/converters/data_model_converter.py
--rw-r--r--   0        0        0     2547 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/converters/logical_definition_flattener.py
--rw-r--r--   0        0        0     2446 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/converters/obo_graph_to_cx_converter.py
--rw-r--r--   0        0        0    12105 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/converters/obo_graph_to_fhir_converter.py
--rw-r--r--   0        0        0     7719 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/converters/obo_graph_to_obo_format_converter.py
--rw-r--r--   0        0        0     6100 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/converters/obo_graph_to_rdf_owl_converter.py
--rw-r--r--   0        0        0       60 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/datamodels/__init__.py
--rw-r--r--   0        0        0     4034 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/datamodels/association.owl.ttl
--rw-r--r--   0        0        0    38339 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/datamodels/association.py
--rw-r--r--   0        0        0    13058 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/datamodels/association.yaml
--rw-r--r--   0        0        0     6165 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/datamodels/class_enrichment.owl.ttl
--rw-r--r--   0        0        0    13288 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/datamodels/class_enrichment.py
--rw-r--r--   0        0        0     3262 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/datamodels/class_enrichment.yaml
--rw-r--r--   0        0        0    19083 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/datamodels/cross_ontology_diff.owl.ttl
--rw-r--r--   0        0        0    24250 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/datamodels/cross_ontology_diff.py
--rw-r--r--   0        0        0    10687 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/datamodels/cross_ontology_diff.yaml
--rw-r--r--   0        0        0    29418 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/datamodels/cx.py
--rw-r--r--   0        0        0     6314 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/datamodels/cx.yaml
--rw-r--r--   0        0        0    15826 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/datamodels/fhir.owl.ttl
--rw-r--r--   0        0        0    35746 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/datamodels/fhir.py
--rw-r--r--   0        0        0     5064 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/datamodels/fhir.yaml
--rw-r--r--   0        0        0    14566 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/datamodels/input_specification.py
--rw-r--r--   0        0        0     3560 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/datamodels/input_specification.yaml
--rw-r--r--   0        0        0    15776 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/datamodels/item_list.py
--rw-r--r--   0        0        0     6339 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/datamodels/item_list.yaml
--rw-r--r--   0        0        0     8984 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/datamodels/lexical_index.owl.ttl
--rw-r--r--   0        0        0    17296 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/datamodels/lexical_index.py
--rw-r--r--   0        0        0     6429 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/datamodels/lexical_index.schema.json
--rw-r--r--   0        0        0     4016 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/datamodels/lexical_index.yaml
--rw-r--r--   0        0        0    26474 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/datamodels/mapping_cluster_datamodel.py
--rw-r--r--   0        0        0     7317 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/datamodels/mapping_cluster_datamodel.yaml
--rw-r--r--   0        0        0   226115 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/mapping_rules_datamodel.owl.ttl
--rw-r--r--   0        0        0    30133 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/mapping_rules_datamodel.py
--rw-r--r--   0        0        0    12889 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/mapping_rules_datamodel.schema.json
--rw-r--r--   0        0        0     3634 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/mapping_rules_datamodel.yaml
--rw-r--r--   0        0        0    25354 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/obograph.owl.ttl
--rw-r--r--   0        0        0    51109 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/obograph.py
--rw-r--r--   0        0        0    22375 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/obograph.schema.json
--rw-r--r--   0        0        0    19600 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/obograph.yaml
--rw-r--r--   0        0        0    59793 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/ontology_metadata.owl.ttl
--rw-r--r--   0        0        0   116914 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/ontology_metadata.py
--rw-r--r--   0        0        0    95288 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/ontology_metadata.schema.json
--rw-r--r--   0        0        0    31452 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/ontology_metadata.yaml
--rw-r--r--   0        0        0    14759 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/oxo.owl.ttl
--rw-r--r--   0        0        0    21914 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/oxo.py
--rw-r--r--   0        0        0     4392 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/oxo.yaml
--rw-r--r--   0        0        0     3348 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/search.py
--rw-r--r--   0        0        0    16948 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/search_datamodel.owl.ttl
--rw-r--r--   0        0        0    25157 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/search_datamodel.py
--rw-r--r--   0        0        0     6684 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/search_datamodel.yaml
--rw-r--r--   0        0        0      287 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/settings.py
--rw-r--r--   0        0        0    12826 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/similarity.owl.ttl
--rw-r--r--   0        0        0    22645 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/similarity.py
--rw-r--r--   0        0        0     5690 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/similarity.yaml
--rw-r--r--   0        0        0    31217 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/summary_statistics_datamodel.owl.ttl
--rw-r--r--   0        0        0    50743 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/summary_statistics_datamodel.py
--rw-r--r--   0        0        0    21176 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/summary_statistics_datamodel.schema.json
--rw-r--r--   0        0        0    16246 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/summary_statistics_datamodel.yaml
--rw-r--r--   0        0        0    23481 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/synonymizer_datamodel.py
--rw-r--r--   0        0        0     2476 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/synonymizer_datamodel.yaml
--rw-r--r--   0        0        0     9909 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/taxon_constraints.owl.ttl
--rw-r--r--   0        0        0    18432 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/taxon_constraints.py
--rw-r--r--   0        0        0     5880 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/taxon_constraints.yaml
--rw-r--r--   0        0        0    11599 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/text_annotator.owl.ttl
--rw-r--r--   0        0        0    21645 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/text_annotator.py
--rw-r--r--   0        0        0     2464 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/text_annotator.schema.json
--rw-r--r--   0        0        0     4996 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/text_annotator.yaml
--rw-r--r--   0        0        0    13670 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/validation_datamodel.owl.ttl
--rw-r--r--   0        0        0    33912 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/validation_datamodel.py
--rw-r--r--   0        0        0    10783 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/validation_datamodel.schema.json
--rw-r--r--   0        0        0     9005 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/validation_datamodel.yaml
--rw-r--r--   0        0        0     6640 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/datamodels/value_set_configuration.owl.ttl
--rw-r--r--   0        0        0     8458 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/datamodels/value_set_configuration.py
--rw-r--r--   0        0        0     2276 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/datamodels/value_set_configuration.yaml
--rw-r--r--   0        0        0     6595 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/datamodels/vocabulary.py
--rw-r--r--   0        0        0     6452 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/__init__.py
--rw-r--r--   0        0        0        0 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/aggregator/__init__.py
--rw-r--r--   0        0        0     6377 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/aggregator/aggregator_implementation.py
--rw-r--r--   0        0        0        0 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/agrkb/__init__.py
--rw-r--r--   0        0        0     8848 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/agrkb/agrkb_implementation.py
--rw-r--r--   0        0        0        0 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/amigo/__init__.py
--rw-r--r--   0        0        0    16195 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/amigo/amigo_implementation.py
--rw-r--r--   0        0        0        0 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/cx/__init__.py
--rw-r--r--   0        0        0     1985 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/cx/cx_implementation.py
--rw-r--r--   0        0        0        0 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/eutils/__init__.py
--rw-r--r--   0        0        0     2180 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/eutils/eutils_implementation.py
--rw-r--r--   0        0        0     1055 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/eutils/pubmed_implementation.py
--rw-r--r--   0        0        0        0 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/fhir/__init__.py
--rw-r--r--   0        0        0        0 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/funowl/__init__.py
--rw-r--r--   0        0        0     8473 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/funowl/funowl_implementation.py
--rw-r--r--   0        0        0     3565 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/gilda.py
--rw-r--r--   0        0        0        0 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/kgx/__init__.py
--rw-r--r--   0        0        0    30523 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/kgx/kgx_implementation.py
--rw-r--r--   0        0        0    28777 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/llm_implementation.py
--rw-r--r--   0        0        0        0 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/monarch/__init__.py
--rw-r--r--   0        0        0     7034 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/monarch/monarch_implementation.py
--rw-r--r--   0        0        0        0 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/ncbi/__init__.py
--rw-r--r--   0        0        0     7034 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/ncbi/ncbi_gene_implementation.py
--rw-r--r--   0        0        0        0 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/neo4j/__init__.py
--rw-r--r--   0        0        0        0 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/obograph/__init__.py
--rw-r--r--   0        0        0    17122 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/obograph/obograph_implementation.py
--rw-r--r--   0        0        0      267 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/ols/__init__.py
--rw-r--r--   0        0        0      132 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/ols/constants.py
--rw-r--r--   0        0        0     8071 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/ols/ols_implementation.py
--rw-r--r--   0        0        0      686 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/ols/oxo_utils.py
--rw-r--r--   0        0        0        0 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/ontobee/__init__.py
--rw-r--r--   0        0        0     2641 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/ontobee/ontobee_implementation.py
--rw-r--r--   0        0        0        0 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/ontoportal/__init__.py
--rw-r--r--   0        0        0      382 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/ontoportal/agroportal_implementation.py
--rw-r--r--   0        0        0     1250 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/ontoportal/bioportal_implementation.py
--rw-r--r--   0        0        0      378 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/ontoportal/ecoportal_implementation.py
--rw-r--r--   0        0        0      378 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/ontoportal/matportal_implementation.py
--rw-r--r--   0        0        0    13670 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/ontoportal/ontoportal_implementation_base.py
--rw-r--r--   0        0        0        0 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/owlery/__init__.py
--rw-r--r--   0        0        0      427 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/owlery/owlery_implementation.py
--rw-r--r--   0        0        0        0 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/pantherdb/__init__.py
--rw-r--r--   0        0        0    12625 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/pantherdb/pantherdb_implementation.py
--rw-r--r--   0        0        0        0 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/pronto/__init__.py
--rw-r--r--   0        0        0    37863 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/pronto/pronto_implementation.py
--rw-r--r--   0        0        0        0 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/robot/__init__.py
--rw-r--r--   0        0        0        0 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/scigraph/__init__.py
--rw-r--r--   0        0        0        0 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/semsimian/__init__.py
--rw-r--r--   0        0        0      247 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/semsimian/profiler.py
--rw-r--r--   0        0        0    11605 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/semsimian/semsimian_implementation.py
--rw-r--r--   0        0        0        0 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/simpleobo/__init__.py
--rw-r--r--   0        0        0    46328 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/simpleobo/simple_obo_implementation.py
--rw-r--r--   0        0        0    23081 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/simpleobo/simple_obo_parser.py
--rw-r--r--   0        0        0        0 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/skos/__init__.py
--rw-r--r--   0        0        0        0 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/solor/__init__.py
--rw-r--r--   0        0        0        0 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/solr/__init__.py
--rw-r--r--   0        0        0       96 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/implementations/sparql/__init__.py
--rw-r--r--   0        0        0    38067 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/implementations/sparql/abstract_sparql_implementation.py
--rw-r--r--   0        0        0      885 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/implementations/sparql/lov_implementation.py
--rw-r--r--   0        0        0     1721 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/implementations/sparql/oak_metamodel_implementation.py
--rw-r--r--   0        0        0     2658 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/implementations/sparql/sparql_implementation.py
--rw-r--r--   0        0        0     2325 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/implementations/sparql/sparql_query.py
--rw-r--r--   0        0        0       96 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/implementations/sqldb/__init__.py
--rw-r--r--   0        0        0   115796 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/implementations/sqldb/sql_implementation.py
--rw-r--r--   0        0        0     1903 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/implementations/sqldb/sqlite_utils.py
--rw-r--r--   0        0        0        0 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/implementations/tabular/__init__.py
--rw-r--r--   0        0        0    19432 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/implementations/tabular/robot_template_implementation.py
--rw-r--r--   0        0        0     3279 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/implementations/tabular/tabular_implementation.py
--rw-r--r--   0        0        0        0 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/implementations/tccm/__init__.py
--rw-r--r--   0        0        0        0 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/implementations/translator/__init__.py
--rw-r--r--   0        0        0     5442 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/implementations/translator/translator_implementation.py
--rw-r--r--   0        0        0      108 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/implementations/ubergraph/__init__.py
--rw-r--r--   0        0        0    20090 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/implementations/ubergraph/ubergraph_implementation.py
--rw-r--r--   0        0        0        0 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/implementations/umls/__init__.py
--rw-r--r--   0        0        0        0 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/implementations/uniprot/__init__.py
--rw-r--r--   0        0        0    14740 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/implementations/uniprot/uniprot_implementation.py
--rw-r--r--   0        0        0       96 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/implementations/wikidata/__init__.py
--rw-r--r--   0        0        0    17267 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/implementations/wikidata/wikidata_implementation.py
--rw-r--r--   0        0        0        0 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/indexes/__init__.py
--rw-r--r--   0        0        0     3089 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/indexes/edge_index.py
--rw-r--r--   0        0        0        0 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/inference/__init__.py
--rw-r--r--   0        0        0      748 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/inference/owl_reasoner.py
--rw-r--r--   0        0        0      105 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/inference/reasoner.py
--rw-r--r--   0        0        0     6960 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/inference/relation_graph_reasoner.py
--rw-r--r--   0        0        0      913 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/interfaces/__init__.py
--rw-r--r--   0        0        0    28686 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/interfaces/association_provider_interface.py
--rw-r--r--   0        0        0    55465 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/interfaces/basic_ontology_interface.py
--rw-r--r--   0        0        0     9243 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/interfaces/class_enrichment_calculation_interface.py
--rw-r--r--   0        0        0    21219 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/interfaces/differ_interface.py
--rw-r--r--   0        0        0     3222 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/interfaces/dumper_interface.py
--rw-r--r--   0        0        0      788 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/interfaces/embedding_provider_interface.py
--rw-r--r--   0        0        0    13680 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/interfaces/mapping_provider_interface.py
--rw-r--r--   0        0        0     3262 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/interfaces/merge_interface.py
--rw-r--r--   0        0        0     3103 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/interfaces/metadata_interface.py
--rw-r--r--   0        0        0    22954 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/interfaces/obograph_interface.py
--rw-r--r--   0        0        0     1003 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/interfaces/obolegacy_interface.py
--rw-r--r--   0        0        0      786 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/interfaces/ontology_generator_interface.py
--rw-r--r--   0        0        0      784 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/interfaces/ontology_interface.py
--rw-r--r--   0        0        0    13645 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/interfaces/owl_interface.py
--rw-r--r--   0        0        0     8606 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/interfaces/patcher_interface.py
--rw-r--r--   0        0        0     1955 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/interfaces/rdf_interface.py
--rw-r--r--   0        0        0     2287 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/interfaces/relation_graph_interface.py
--rw-r--r--   0        0        0     3759 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/interfaces/search_interface.py
--rw-r--r--   0        0        0    16173 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/interfaces/semsim_interface.py
--rw-r--r--   0        0        0     1063 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/interfaces/skos_interface.py
--rw-r--r--   0        0        0     2113 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/interfaces/subsetter_interface.py
--rw-r--r--   0        0        0    10140 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/interfaces/summary_statistics_interface.py
--rw-r--r--   0        0        0    18295 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/interfaces/taxon_constraint_interface.py
--rw-r--r--   0        0        0    10076 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/interfaces/text_annotator_interface.py
--rw-r--r--   0        0        0    12915 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/interfaces/validator_interface.py
--rw-r--r--   0        0        0        0 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/io/__init__.py
--rw-r--r--   0        0        0     2091 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/io/heatmap_writer.py
--rw-r--r--   0        0        0     1698 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/io/html_writer.py
--rw-r--r--   0        0        0     1565 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/io/obograph_writer.py
--rw-r--r--   0        0        0     3444 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/io/rollup_report_writer.py
--rw-r--r--   0        0        0      739 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/io/streaming_axiom_writer.py
--rw-r--r--   0        0        0     9012 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/io/streaming_csv_writer.py
--rw-r--r--   0        0        0     1284 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/io/streaming_fhir_writer.py
--rw-r--r--   0        0        0     2524 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/io/streaming_info_writer.py
--rw-r--r--   0        0        0      785 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/io/streaming_json_lines_writer.py
--rw-r--r--   0        0        0     1806 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/io/streaming_json_writer.py
--rw-r--r--   0        0        0      741 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/io/streaming_kgcl_writer.py
--rw-r--r--   0        0        0     2672 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/io/streaming_markdown_writer.py
--rw-r--r--   0        0        0     1152 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/io/streaming_nl_writer.py
--rw-r--r--   0        0        0     1117 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/io/streaming_obo_json_writer.py
--rw-r--r--   0        0        0     3485 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/io/streaming_obo_writer.py
--rw-r--r--   0        0        0     1270 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/io/streaming_owl_functional_writer.py
--rw-r--r--   0        0        0     2244 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/io/streaming_rdf_writer.py
--rw-r--r--   0        0        0     5126 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/io/streaming_writer.py
--rw-r--r--   0        0        0     1318 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/io/streaming_yaml_writer.py
--rw-r--r--   0        0        0      113 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/mappers/__init__.py
--rw-r--r--   0        0        0     3956 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/mappers/base_mapper.py
--rw-r--r--   0        0        0     1979 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/mappers/ontology_metadata_mapper.py
--rw-r--r--   0        0        0     2363 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/parsers/__init__.py
--rw-r--r--   0        0        0     1525 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/parsers/association_parser.py
--rw-r--r--   0        0        0      522 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/parsers/association_parser_factory.py
--rw-r--r--   0        0        0     4732 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/parsers/boomer_parser.py
--rw-r--r--   0        0        0     2148 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/parsers/gaf_association_parser.py
--rw-r--r--   0        0        0     2101 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/parsers/gencc_association_parser.py
--rw-r--r--   0        0        0     1131 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/parsers/hpoa_association_parser.py
--rw-r--r--   0        0        0     1673 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/parsers/hpoa_g2d_association_parser.py
--rw-r--r--   0        0        0      603 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/parsers/hpoa_g2p_association_parser.py
--rw-r--r--   0        0        0      654 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/parsers/kgx_association_parser.py
--rw-r--r--   0        0        0     1672 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/parsers/mim2gene_association_parser.py
--rw-r--r--   0        0        0      526 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/parsers/pairwise_association_parser.py
--rw-r--r--   0        0        0     1433 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/parsers/parser_base.py
--rw-r--r--   0        0        0      708 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/parsers/phaf_association_parser.py
--rw-r--r--   0        0        0     8681 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/parsers/xaf_association_parser.py
--rw-r--r--   0        0        0     2210 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/resource.py
--rw-r--r--   0        0        0    15958 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/selector.py
--rw-r--r--   0        0        0        0 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/transformers/__init__.py
--rw-r--r--   0        0        0      589 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/transformers/chained_ontology_transformer.py
--rw-r--r--   0        0        0     2757 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/transformers/edge_filter_transformer.py
--rw-r--r--   0        0        0     1257 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/transformers/graph_transformer.py
--rw-r--r--   0        0        0     1804 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/transformers/node_filter_transformer.py
--rw-r--r--   0        0        0      470 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/transformers/ontology_transformer.py
--rw-r--r--   0        0        0     6353 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/transformers/sep_transformer.py
--rw-r--r--   0        0        0     1768 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/transformers/transformers_factory.py
--rw-r--r--   0        0        0      177 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/types.py
--rw-r--r--   0        0        0        0 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/utilities/__init__.py
--rw-r--r--   0        0        0     1613 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/utilities/apikey_manager.py
--rw-r--r--   0        0        0        0 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/utilities/associations/__init__.py
--rw-r--r--   0        0        0    13441 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/utilities/associations/association_differ.py
--rw-r--r--   0        0        0     3427 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/utilities/associations/association_index.py
--rw-r--r--   0        0        0        0 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/utilities/axioms/__init__.py
--rw-r--r--   0        0        0     7694 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/utilities/axioms/disjointness_axiom_analyzer.py
--rw-r--r--   0        0        0     4093 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/utilities/axioms/logical_definition_analyzer.py
--rw-r--r--   0        0        0     8829 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/utilities/axioms/logical_definition_summarizer.py
--rw-r--r--   0        0        0     2436 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/utilities/axioms/logical_definition_utilities.py
--rw-r--r--   0        0        0     1540 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/utilities/basic_utils.py
--rw-r--r--   0        0        0     1356 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/utilities/format_utilities.py
--rw-r--r--   0        0        0        0 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/utilities/graph/__init__.py
--rw-r--r--   0        0        0     2491 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/utilities/graph/networkx_bridge.py
--rw-r--r--   0        0        0     2857 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/utilities/graph/relationship_walker.py
--rw-r--r--   0        0        0      993 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/utilities/identifier_utils.py
--rw-r--r--   0        0        0      999 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/utilities/iterator_utils.py
--rw-r--r--   0        0        0     1015 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/utilities/keyval_cache.py
--rw-r--r--   0        0        0     3425 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/utilities/kgcl_utilities.py
--rw-r--r--   0        0        0      850 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/utilities/label_utilities.py
--rw-r--r--   0        0        0        0 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/utilities/lexical/__init__.py
--rw-r--r--   0        0        0    19249 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/utilities/lexical/lexical_indexer.py
--rw-r--r--   0        0        0    10235 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/utilities/lexical/patternizer.py
--rw-r--r--   0        0        0     6881 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/utilities/lexical/synonymizer.py
--rw-r--r--   0        0        0        0 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/utilities/mapping/__init__.py
--rw-r--r--   0        0        0    14422 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/utilities/mapping/boomer_utils.py
--rw-r--r--   0        0        0    15527 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/utilities/mapping/cross_ontology_diffs.py
--rw-r--r--   0        0        0      751 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/utilities/mapping/mapping_propagator.py
--rw-r--r--   0        0        0    10929 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/utilities/mapping/mapping_validation.py
--rw-r--r--   0        0        0     2558 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/utilities/mapping/sssom_utils.py
--rw-r--r--   0        0        0      690 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/utilities/ner_utilities.py
--rw-r--r--   0        0        0        0 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/utilities/nlp/__init__.py
--rw-r--r--   0        0        0     3358 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/utilities/nlp/natual_language_generation.py
--rw-r--r--   0        0        0      136 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/utilities/oboformat_utils.py
--rw-r--r--   0        0        0    30409 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/utilities/obograph_utils.py
--rw-r--r--   0        0        0     2275 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/utilities/ontology_builder.py
--rw-r--r--   0        0        0        0 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/utilities/publication_utils/__init__.py
--rw-r--r--   0        0        0     5283 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/utilities/publication_utils/doi_wrapper.py
--rw-r--r--   0        0        0      924 2024-04-16 00:05:41.253161 oaklib-0.6.3/src/oaklib/utilities/publication_utils/pubdb_wrapper.py
--rw-r--r--   0        0        0     6575 2024-04-16 00:05:41.253161 oaklib-0.6.3/src/oaklib/utilities/publication_utils/pubmed_wrapper.py
--rw-r--r--   0        0        0      380 2024-04-16 00:05:41.253161 oaklib-0.6.3/src/oaklib/utilities/rate_limiter.py
--rw-r--r--   0        0        0        0 2024-04-16 00:05:41.253161 oaklib-0.6.3/src/oaklib/utilities/reasoning/__init__.py
--rw-r--r--   0        0        0      569 2024-04-16 00:05:41.253161 oaklib-0.6.3/src/oaklib/utilities/reasoning/relation_graph.py
--rw-r--r--   0        0        0        0 2024-04-16 00:05:41.253161 oaklib-0.6.3/src/oaklib/utilities/semsim/__init__.py
--rw-r--r--   0        0        0     2545 2024-04-16 00:05:41.253161 oaklib-0.6.3/src/oaklib/utilities/semsim/similarity_utils.py
--rw-r--r--   0        0        0        0 2024-04-16 00:05:41.253161 oaklib-0.6.3/src/oaklib/utilities/stats/__init__.py
--rw-r--r--   0        0        0     1511 2024-04-16 00:05:41.253161 oaklib-0.6.3/src/oaklib/utilities/stats/hypergeometric.py
--rw-r--r--   0        0        0        0 2024-04-16 00:05:41.253161 oaklib-0.6.3/src/oaklib/utilities/subsets/__init__.py
--rw-r--r--   0        0        0     2819 2024-04-16 00:05:41.253161 oaklib-0.6.3/src/oaklib/utilities/subsets/slimmer_utils.py
--rw-r--r--   0        0        0     4701 2024-04-16 00:05:41.253161 oaklib-0.6.3/src/oaklib/utilities/subsets/subset_analysis.py
--rw-r--r--   0        0        0    12015 2024-04-16 00:05:41.253161 oaklib-0.6.3/src/oaklib/utilities/subsets/value_set_expander.py
--rw-r--r--   0        0        0    18045 2024-04-16 00:05:41.253161 oaklib-0.6.3/src/oaklib/utilities/table_filler.py
--rw-r--r--   0        0        0        0 2024-04-16 00:05:41.253161 oaklib-0.6.3/src/oaklib/utilities/taxon/__init__.py
--rw-r--r--   0        0        0     1743 2024-04-16 00:05:41.253161 oaklib-0.6.3/src/oaklib/utilities/taxon/taxon_constraint_utils.py
--rw-r--r--   0        0        0        0 2024-04-16 00:05:41.253161 oaklib-0.6.3/src/oaklib/utilities/validation/__init__.py
--rw-r--r--   0        0        0    11118 2024-04-16 00:05:41.253161 oaklib-0.6.3/src/oaklib/utilities/validation/definition_ontology_rule.py
--rw-r--r--   0        0        0     7492 2024-04-16 00:05:41.253161 oaklib-0.6.3/src/oaklib/utilities/validation/disjointness_rule.py
--rw-r--r--   0        0        0     1729 2024-04-16 00:05:41.253161 oaklib-0.6.3/src/oaklib/utilities/validation/lint_utils.py
--rw-r--r--   0        0        0     1402 2024-04-16 00:05:41.253161 oaklib-0.6.3/src/oaklib/utilities/validation/ontology_rule.py
--rw-r--r--   0        0        0     1275 2024-04-16 00:05:41.253161 oaklib-0.6.3/src/oaklib/utilities/validation/rule_runner.py
--rw-r--r--   0        0        0      122 2024-04-16 00:05:41.253161 oaklib-0.6.3/src/oaklib/utilities/writers/__init__.py
--rw-r--r--   0        0        0    16522 2024-04-16 00:05:41.253161 oaklib-0.6.3/src/oaklib/utilities/writers/change_handler.py
--rw-r--r--   0        0        0     9171 1970-01-01 00:00:00.000000 oaklib-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-25 00:55:39.708864 oaklib-0.6.4/LICENSE
+-rw-r--r--   0        0        0     7258 2024-04-25 00:55:39.708864 oaklib-0.6.4/README.md
+-rw-r--r--   0        0        0     3500 2024-04-25 00:56:12.428821 oaklib-0.6.4/pyproject.toml
+-rw-r--r--   0        0        0      272 2024-04-25 00:55:39.876864 oaklib-0.6.4/src/oaklib/__init__.py
+-rw-r--r--   0        0        0   231404 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/cli.py
+-rw-r--r--   0        0        0       64 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/conf/__init__.py
+-rw-r--r--   0        0        0      372 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/conf/go-human-input-spec.yaml
+-rw-r--r--   0        0        0      162 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/conf/go-pombase-input-spec.yaml
+-rw-r--r--   0        0        0      109 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/conf/hpoa-g2p-input-spec.yaml
+-rw-r--r--   0        0        0      106 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/conf/hpoa-input-spec.yaml
+-rw-r--r--   0        0        0     1903 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/conf/lexmatch-rules-oboinowl-default.yaml
+-rw-r--r--   0        0        0     1011 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/conf/mondo-g2d-input-spec.yaml
+-rw-r--r--   0        0        0      109 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/conf/mondo-gencc-input-spec.yaml
+-rw-r--r--   0        0        0      529 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/conf/mondo-hpoa-g2d-input-spec.yaml
+-rw-r--r--   0        0        0      118 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/conf/mondo-medgen-g2d-input-spec.yaml
+-rw-r--r--   0        0        0     4730 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/conf/obograph-style.json
+-rw-r--r--   0        0        0      256 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/conf/omo-to-skos.sssom.tsv
+-rw-r--r--   0        0        0      131 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/conf/value-set-expander.conf.yaml
+-rw-r--r--   0        0        0      149 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/constants.py
+-rw-r--r--   0        0        0        0 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/converters/__init__.py
+-rw-r--r--   0        0        0     1461 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/converters/data_model_converter.py
+-rw-r--r--   0        0        0     2547 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/converters/logical_definition_flattener.py
+-rw-r--r--   0        0        0     2446 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/converters/obo_graph_to_cx_converter.py
+-rw-r--r--   0        0        0    12105 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/converters/obo_graph_to_fhir_converter.py
+-rw-r--r--   0        0        0     7719 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/converters/obo_graph_to_obo_format_converter.py
+-rw-r--r--   0        0        0     6100 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/converters/obo_graph_to_rdf_owl_converter.py
+-rw-r--r--   0        0        0       60 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/datamodels/__init__.py
+-rw-r--r--   0        0        0     4034 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/datamodels/association.owl.ttl
+-rw-r--r--   0        0        0    38339 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/datamodels/association.py
+-rw-r--r--   0        0        0    13058 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/datamodels/association.yaml
+-rw-r--r--   0        0        0     6165 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/datamodels/class_enrichment.owl.ttl
+-rw-r--r--   0        0        0    13288 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/datamodels/class_enrichment.py
+-rw-r--r--   0        0        0     3262 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/datamodels/class_enrichment.yaml
+-rw-r--r--   0        0        0    19083 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/datamodels/cross_ontology_diff.owl.ttl
+-rw-r--r--   0        0        0    24250 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/datamodels/cross_ontology_diff.py
+-rw-r--r--   0        0        0    10687 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/datamodels/cross_ontology_diff.yaml
+-rw-r--r--   0        0        0    29418 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/datamodels/cx.py
+-rw-r--r--   0        0        0     6314 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/datamodels/cx.yaml
+-rw-r--r--   0        0        0    15826 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/datamodels/fhir.owl.ttl
+-rw-r--r--   0        0        0    35746 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/datamodels/fhir.py
+-rw-r--r--   0        0        0     5064 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/datamodels/fhir.yaml
+-rw-r--r--   0        0        0    14566 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/datamodels/input_specification.py
+-rw-r--r--   0        0        0     3560 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/datamodels/input_specification.yaml
+-rw-r--r--   0        0        0    15776 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/datamodels/item_list.py
+-rw-r--r--   0        0        0     6339 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/datamodels/item_list.yaml
+-rw-r--r--   0        0        0     8984 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/datamodels/lexical_index.owl.ttl
+-rw-r--r--   0        0        0    17296 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/datamodels/lexical_index.py
+-rw-r--r--   0        0        0     6429 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/datamodels/lexical_index.schema.json
+-rw-r--r--   0        0        0     4016 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/datamodels/lexical_index.yaml
+-rw-r--r--   0        0        0    26474 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/datamodels/mapping_cluster_datamodel.py
+-rw-r--r--   0        0        0     7317 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/datamodels/mapping_cluster_datamodel.yaml
+-rw-r--r--   0        0        0   226115 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/datamodels/mapping_rules_datamodel.owl.ttl
+-rw-r--r--   0        0        0    30133 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/datamodels/mapping_rules_datamodel.py
+-rw-r--r--   0        0        0    12889 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/datamodels/mapping_rules_datamodel.schema.json
+-rw-r--r--   0        0        0     3634 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/datamodels/mapping_rules_datamodel.yaml
+-rw-r--r--   0        0        0    25354 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/datamodels/obograph.owl.ttl
+-rw-r--r--   0        0        0    51109 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/datamodels/obograph.py
+-rw-r--r--   0        0        0    22375 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/datamodels/obograph.schema.json
+-rw-r--r--   0        0        0    19600 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/datamodels/obograph.yaml
+-rw-r--r--   0        0        0    59793 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/datamodels/ontology_metadata.owl.ttl
+-rw-r--r--   0        0        0   116914 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/datamodels/ontology_metadata.py
+-rw-r--r--   0        0        0    95288 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/datamodels/ontology_metadata.schema.json
+-rw-r--r--   0        0        0    31452 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/datamodels/ontology_metadata.yaml
+-rw-r--r--   0        0        0    14759 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/datamodels/oxo.owl.ttl
+-rw-r--r--   0        0        0    21914 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/datamodels/oxo.py
+-rw-r--r--   0        0        0     4392 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/datamodels/oxo.yaml
+-rw-r--r--   0        0        0     3348 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/datamodels/search.py
+-rw-r--r--   0        0        0    16948 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/datamodels/search_datamodel.owl.ttl
+-rw-r--r--   0        0        0    25157 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/datamodels/search_datamodel.py
+-rw-r--r--   0        0        0     6684 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/datamodels/search_datamodel.yaml
+-rw-r--r--   0        0        0      287 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/datamodels/settings.py
+-rw-r--r--   0        0        0    12826 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/datamodels/similarity.owl.ttl
+-rw-r--r--   0        0        0    22645 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/datamodels/similarity.py
+-rw-r--r--   0        0        0     5690 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/datamodels/similarity.yaml
+-rw-r--r--   0        0        0    31217 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/datamodels/summary_statistics_datamodel.owl.ttl
+-rw-r--r--   0        0        0    50743 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/datamodels/summary_statistics_datamodel.py
+-rw-r--r--   0        0        0    21176 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/datamodels/summary_statistics_datamodel.schema.json
+-rw-r--r--   0        0        0    16246 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/datamodels/summary_statistics_datamodel.yaml
+-rw-r--r--   0        0        0    23481 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/datamodels/synonymizer_datamodel.py
+-rw-r--r--   0        0        0     2476 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/datamodels/synonymizer_datamodel.yaml
+-rw-r--r--   0        0        0     9909 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/datamodels/taxon_constraints.owl.ttl
+-rw-r--r--   0        0        0    18432 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/datamodels/taxon_constraints.py
+-rw-r--r--   0        0        0     5880 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/datamodels/taxon_constraints.yaml
+-rw-r--r--   0        0        0    11599 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/datamodels/text_annotator.owl.ttl
+-rw-r--r--   0        0        0    21645 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/datamodels/text_annotator.py
+-rw-r--r--   0        0        0     2464 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/datamodels/text_annotator.schema.json
+-rw-r--r--   0        0        0     4996 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/datamodels/text_annotator.yaml
+-rw-r--r--   0        0        0    13670 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/datamodels/validation_datamodel.owl.ttl
+-rw-r--r--   0        0        0    33912 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/datamodels/validation_datamodel.py
+-rw-r--r--   0        0        0    10783 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/datamodels/validation_datamodel.schema.json
+-rw-r--r--   0        0        0     9005 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/datamodels/validation_datamodel.yaml
+-rw-r--r--   0        0        0     6640 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/datamodels/value_set_configuration.owl.ttl
+-rw-r--r--   0        0        0     8458 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/datamodels/value_set_configuration.py
+-rw-r--r--   0        0        0     2276 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/datamodels/value_set_configuration.yaml
+-rw-r--r--   0        0        0     6595 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/datamodels/vocabulary.py
+-rw-r--r--   0        0        0     6452 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/implementations/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/implementations/aggregator/__init__.py
+-rw-r--r--   0        0        0     6377 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/implementations/aggregator/aggregator_implementation.py
+-rw-r--r--   0        0        0        0 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/implementations/agrkb/__init__.py
+-rw-r--r--   0        0        0     8848 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/implementations/agrkb/agrkb_implementation.py
+-rw-r--r--   0        0        0        0 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/implementations/amigo/__init__.py
+-rw-r--r--   0        0        0    16195 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/implementations/amigo/amigo_implementation.py
+-rw-r--r--   0        0        0        0 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/implementations/cx/__init__.py
+-rw-r--r--   0        0        0     1985 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/implementations/cx/cx_implementation.py
+-rw-r--r--   0        0        0        0 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/eutils/__init__.py
+-rw-r--r--   0        0        0     2180 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/eutils/eutils_implementation.py
+-rw-r--r--   0        0        0     1055 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/eutils/pubmed_implementation.py
+-rw-r--r--   0        0        0        0 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/fhir/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/funowl/__init__.py
+-rw-r--r--   0        0        0     8473 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/funowl/funowl_implementation.py
+-rw-r--r--   0        0        0     3565 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/gilda.py
+-rw-r--r--   0        0        0        0 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/kgx/__init__.py
+-rw-r--r--   0        0        0    30523 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/kgx/kgx_implementation.py
+-rw-r--r--   0        0        0    28777 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/llm_implementation.py
+-rw-r--r--   0        0        0        0 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/monarch/__init__.py
+-rw-r--r--   0        0        0     7034 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/monarch/monarch_implementation.py
+-rw-r--r--   0        0        0        0 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/ncbi/__init__.py
+-rw-r--r--   0        0        0     7034 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/ncbi/ncbi_gene_implementation.py
+-rw-r--r--   0        0        0        0 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/neo4j/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/obograph/__init__.py
+-rw-r--r--   0        0        0    17122 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/obograph/obograph_implementation.py
+-rw-r--r--   0        0        0      267 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/ols/__init__.py
+-rw-r--r--   0        0        0      132 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/ols/constants.py
+-rw-r--r--   0        0        0     8071 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/ols/ols_implementation.py
+-rw-r--r--   0        0        0      686 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/ols/oxo_utils.py
+-rw-r--r--   0        0        0        0 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/ontobee/__init__.py
+-rw-r--r--   0        0        0     2641 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/ontobee/ontobee_implementation.py
+-rw-r--r--   0        0        0        0 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/ontoportal/__init__.py
+-rw-r--r--   0        0        0      382 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/ontoportal/agroportal_implementation.py
+-rw-r--r--   0        0        0     1250 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/ontoportal/bioportal_implementation.py
+-rw-r--r--   0        0        0      378 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/ontoportal/ecoportal_implementation.py
+-rw-r--r--   0        0        0      378 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/ontoportal/matportal_implementation.py
+-rw-r--r--   0        0        0    13670 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/ontoportal/ontoportal_implementation_base.py
+-rw-r--r--   0        0        0        0 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/owlery/__init__.py
+-rw-r--r--   0        0        0      427 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/owlery/owlery_implementation.py
+-rw-r--r--   0        0        0        0 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/pantherdb/__init__.py
+-rw-r--r--   0        0        0    12625 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/pantherdb/pantherdb_implementation.py
+-rw-r--r--   0        0        0        0 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/pronto/__init__.py
+-rw-r--r--   0        0        0    37863 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/pronto/pronto_implementation.py
+-rw-r--r--   0        0        0        0 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/robot/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/scigraph/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/semsimian/__init__.py
+-rw-r--r--   0        0        0      247 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/semsimian/profiler.py
+-rw-r--r--   0        0        0    11605 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/semsimian/semsimian_implementation.py
+-rw-r--r--   0        0        0        0 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/simpleobo/__init__.py
+-rw-r--r--   0        0        0    46328 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/simpleobo/simple_obo_implementation.py
+-rw-r--r--   0        0        0    23081 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/simpleobo/simple_obo_parser.py
+-rw-r--r--   0        0        0        0 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/skos/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/solor/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/solr/__init__.py
+-rw-r--r--   0        0        0       96 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/sparql/__init__.py
+-rw-r--r--   0        0        0    38067 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/sparql/abstract_sparql_implementation.py
+-rw-r--r--   0        0        0      885 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/sparql/lov_implementation.py
+-rw-r--r--   0        0        0     1721 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/sparql/oak_metamodel_implementation.py
+-rw-r--r--   0        0        0     2658 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/sparql/sparql_implementation.py
+-rw-r--r--   0        0        0     2325 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/sparql/sparql_query.py
+-rw-r--r--   0        0        0       96 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/sqldb/__init__.py
+-rw-r--r--   0        0        0   115796 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/sqldb/sql_implementation.py
+-rw-r--r--   0        0        0     1903 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/sqldb/sqlite_utils.py
+-rw-r--r--   0        0        0        0 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/tabular/__init__.py
+-rw-r--r--   0        0        0    19432 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/tabular/robot_template_implementation.py
+-rw-r--r--   0        0        0     3279 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/tabular/tabular_implementation.py
+-rw-r--r--   0        0        0        0 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/tccm/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/implementations/translator/__init__.py
+-rw-r--r--   0        0        0     5442 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/implementations/translator/translator_implementation.py
+-rw-r--r--   0        0        0      108 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/implementations/ubergraph/__init__.py
+-rw-r--r--   0        0        0    20090 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/implementations/ubergraph/ubergraph_implementation.py
+-rw-r--r--   0        0        0        0 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/implementations/umls/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/implementations/uniprot/__init__.py
+-rw-r--r--   0        0        0    14740 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/implementations/uniprot/uniprot_implementation.py
+-rw-r--r--   0        0        0       96 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/implementations/wikidata/__init__.py
+-rw-r--r--   0        0        0    17267 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/implementations/wikidata/wikidata_implementation.py
+-rw-r--r--   0        0        0        0 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/indexes/__init__.py
+-rw-r--r--   0        0        0     3089 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/indexes/edge_index.py
+-rw-r--r--   0        0        0        0 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/inference/__init__.py
+-rw-r--r--   0        0        0      748 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/inference/owl_reasoner.py
+-rw-r--r--   0        0        0      105 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/inference/reasoner.py
+-rw-r--r--   0        0        0     6960 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/inference/relation_graph_reasoner.py
+-rw-r--r--   0        0        0      913 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/interfaces/__init__.py
+-rw-r--r--   0        0        0    28686 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/interfaces/association_provider_interface.py
+-rw-r--r--   0        0        0    55465 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/interfaces/basic_ontology_interface.py
+-rw-r--r--   0        0        0     9243 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/interfaces/class_enrichment_calculation_interface.py
+-rw-r--r--   0        0        0    21219 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/interfaces/differ_interface.py
+-rw-r--r--   0        0        0     3222 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/interfaces/dumper_interface.py
+-rw-r--r--   0        0        0      788 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/interfaces/embedding_provider_interface.py
+-rw-r--r--   0        0        0    13680 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/interfaces/mapping_provider_interface.py
+-rw-r--r--   0        0        0     3262 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/interfaces/merge_interface.py
+-rw-r--r--   0        0        0     3103 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/interfaces/metadata_interface.py
+-rw-r--r--   0        0        0    24049 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/interfaces/obograph_interface.py
+-rw-r--r--   0        0        0     1003 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/interfaces/obolegacy_interface.py
+-rw-r--r--   0        0        0      786 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/interfaces/ontology_generator_interface.py
+-rw-r--r--   0        0        0      784 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/interfaces/ontology_interface.py
+-rw-r--r--   0        0        0    13645 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/interfaces/owl_interface.py
+-rw-r--r--   0        0        0     8606 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/interfaces/patcher_interface.py
+-rw-r--r--   0        0        0     1955 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/interfaces/rdf_interface.py
+-rw-r--r--   0        0        0     2287 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/interfaces/relation_graph_interface.py
+-rw-r--r--   0        0        0     3759 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/interfaces/search_interface.py
+-rw-r--r--   0        0        0    16173 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/interfaces/semsim_interface.py
+-rw-r--r--   0        0        0     1063 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/interfaces/skos_interface.py
+-rw-r--r--   0        0        0     2113 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/interfaces/subsetter_interface.py
+-rw-r--r--   0        0        0    10140 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/interfaces/summary_statistics_interface.py
+-rw-r--r--   0        0        0    18295 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/interfaces/taxon_constraint_interface.py
+-rw-r--r--   0        0        0    10076 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/interfaces/text_annotator_interface.py
+-rw-r--r--   0        0        0    12915 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/interfaces/validator_interface.py
+-rw-r--r--   0        0        0        0 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/io/__init__.py
+-rw-r--r--   0        0        0     2091 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/io/heatmap_writer.py
+-rw-r--r--   0        0        0     1698 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/io/html_writer.py
+-rw-r--r--   0        0        0     1565 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/io/obograph_writer.py
+-rw-r--r--   0        0        0     3444 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/io/rollup_report_writer.py
+-rw-r--r--   0        0        0      739 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/io/streaming_axiom_writer.py
+-rw-r--r--   0        0        0     9012 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/io/streaming_csv_writer.py
+-rw-r--r--   0        0        0     1284 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/io/streaming_fhir_writer.py
+-rw-r--r--   0        0        0     2524 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/io/streaming_info_writer.py
+-rw-r--r--   0        0        0      785 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/io/streaming_json_lines_writer.py
+-rw-r--r--   0        0        0     1806 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/io/streaming_json_writer.py
+-rw-r--r--   0        0        0      741 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/io/streaming_kgcl_writer.py
+-rw-r--r--   0        0        0     2672 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/io/streaming_markdown_writer.py
+-rw-r--r--   0        0        0     1152 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/io/streaming_nl_writer.py
+-rw-r--r--   0        0        0     1117 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/io/streaming_obo_json_writer.py
+-rw-r--r--   0        0        0     3485 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/io/streaming_obo_writer.py
+-rw-r--r--   0        0        0     1270 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/io/streaming_owl_functional_writer.py
+-rw-r--r--   0        0        0     2244 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/io/streaming_rdf_writer.py
+-rw-r--r--   0        0        0     5126 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/io/streaming_writer.py
+-rw-r--r--   0        0        0     1318 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/io/streaming_yaml_writer.py
+-rw-r--r--   0        0        0      113 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/mappers/__init__.py
+-rw-r--r--   0        0        0     3956 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/mappers/base_mapper.py
+-rw-r--r--   0        0        0     1979 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/mappers/ontology_metadata_mapper.py
+-rw-r--r--   0        0        0     2363 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/parsers/__init__.py
+-rw-r--r--   0        0        0     1525 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/parsers/association_parser.py
+-rw-r--r--   0        0        0      522 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/parsers/association_parser_factory.py
+-rw-r--r--   0        0        0     4732 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/parsers/boomer_parser.py
+-rw-r--r--   0        0        0     2148 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/parsers/gaf_association_parser.py
+-rw-r--r--   0        0        0     2101 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/parsers/gencc_association_parser.py
+-rw-r--r--   0        0        0     1131 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/parsers/hpoa_association_parser.py
+-rw-r--r--   0        0        0     1673 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/parsers/hpoa_g2d_association_parser.py
+-rw-r--r--   0        0        0      603 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/parsers/hpoa_g2p_association_parser.py
+-rw-r--r--   0        0        0      654 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/parsers/kgx_association_parser.py
+-rw-r--r--   0        0        0     1672 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/parsers/mim2gene_association_parser.py
+-rw-r--r--   0        0        0      526 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/parsers/pairwise_association_parser.py
+-rw-r--r--   0        0        0     1433 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/parsers/parser_base.py
+-rw-r--r--   0        0        0      708 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/parsers/phaf_association_parser.py
+-rw-r--r--   0        0        0     8681 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/parsers/xaf_association_parser.py
+-rw-r--r--   0        0        0     2210 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/resource.py
+-rw-r--r--   0        0        0    15958 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/selector.py
+-rw-r--r--   0        0        0        0 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/transformers/__init__.py
+-rw-r--r--   0        0        0      589 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/transformers/chained_ontology_transformer.py
+-rw-r--r--   0        0        0     2757 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/transformers/edge_filter_transformer.py
+-rw-r--r--   0        0        0     1257 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/transformers/graph_transformer.py
+-rw-r--r--   0        0        0     1804 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/transformers/node_filter_transformer.py
+-rw-r--r--   0        0        0      470 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/transformers/ontology_transformer.py
+-rw-r--r--   0        0        0     6353 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/transformers/sep_transformer.py
+-rw-r--r--   0        0        0     1768 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/transformers/transformers_factory.py
+-rw-r--r--   0        0        0      177 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/types.py
+-rw-r--r--   0        0        0        0 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/__init__.py
+-rw-r--r--   0        0        0     1613 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/apikey_manager.py
+-rw-r--r--   0        0        0        0 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/associations/__init__.py
+-rw-r--r--   0        0        0    13441 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/associations/association_differ.py
+-rw-r--r--   0        0        0     3427 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/associations/association_index.py
+-rw-r--r--   0        0        0        0 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/axioms/__init__.py
+-rw-r--r--   0        0        0     7694 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/axioms/disjointness_axiom_analyzer.py
+-rw-r--r--   0        0        0     4093 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/axioms/logical_definition_analyzer.py
+-rw-r--r--   0        0        0     8829 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/axioms/logical_definition_summarizer.py
+-rw-r--r--   0        0        0     2436 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/axioms/logical_definition_utilities.py
+-rw-r--r--   0        0        0     1540 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/basic_utils.py
+-rw-r--r--   0        0        0     1356 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/format_utilities.py
+-rw-r--r--   0        0        0        0 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/graph/__init__.py
+-rw-r--r--   0        0        0     2491 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/graph/networkx_bridge.py
+-rw-r--r--   0        0        0     2857 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/graph/relationship_walker.py
+-rw-r--r--   0        0        0      993 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/identifier_utils.py
+-rw-r--r--   0        0        0      999 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/iterator_utils.py
+-rw-r--r--   0        0        0     1015 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/keyval_cache.py
+-rw-r--r--   0        0        0     3425 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/kgcl_utilities.py
+-rw-r--r--   0        0        0      850 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/label_utilities.py
+-rw-r--r--   0        0        0        0 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/lexical/__init__.py
+-rw-r--r--   0        0        0    19249 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/lexical/lexical_indexer.py
+-rw-r--r--   0        0        0    10235 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/lexical/patternizer.py
+-rw-r--r--   0        0        0     6881 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/lexical/synonymizer.py
+-rw-r--r--   0        0        0        0 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/mapping/__init__.py
+-rw-r--r--   0        0        0    14422 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/mapping/boomer_utils.py
+-rw-r--r--   0        0        0    15527 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/mapping/cross_ontology_diffs.py
+-rw-r--r--   0        0        0      751 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/mapping/mapping_propagator.py
+-rw-r--r--   0        0        0    10929 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/mapping/mapping_validation.py
+-rw-r--r--   0        0        0     2558 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/mapping/sssom_utils.py
+-rw-r--r--   0        0        0      690 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/ner_utilities.py
+-rw-r--r--   0        0        0        0 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/nlp/__init__.py
+-rw-r--r--   0        0        0     3358 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/nlp/natual_language_generation.py
+-rw-r--r--   0        0        0      136 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/oboformat_utils.py
+-rw-r--r--   0        0        0    30409 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/obograph_utils.py
+-rw-r--r--   0        0        0     2275 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/ontology_builder.py
+-rw-r--r--   0        0        0        0 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/publication_utils/__init__.py
+-rw-r--r--   0        0        0     5283 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/publication_utils/doi_wrapper.py
+-rw-r--r--   0        0        0      924 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/publication_utils/pubdb_wrapper.py
+-rw-r--r--   0        0        0     6575 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/publication_utils/pubmed_wrapper.py
+-rw-r--r--   0        0        0      380 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/rate_limiter.py
+-rw-r--r--   0        0        0        0 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/reasoning/__init__.py
+-rw-r--r--   0        0        0      569 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/reasoning/relation_graph.py
+-rw-r--r--   0        0        0        0 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/semsim/__init__.py
+-rw-r--r--   0        0        0     2545 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/semsim/similarity_utils.py
+-rw-r--r--   0        0        0        0 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/stats/__init__.py
+-rw-r--r--   0        0        0     1511 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/stats/hypergeometric.py
+-rw-r--r--   0        0        0        0 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/subsets/__init__.py
+-rw-r--r--   0        0        0     2819 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/subsets/slimmer_utils.py
+-rw-r--r--   0        0        0     4701 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/subsets/subset_analysis.py
+-rw-r--r--   0        0        0    12015 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/subsets/value_set_expander.py
+-rw-r--r--   0        0        0    18045 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/table_filler.py
+-rw-r--r--   0        0        0        0 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/taxon/__init__.py
+-rw-r--r--   0        0        0     1743 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/taxon/taxon_constraint_utils.py
+-rw-r--r--   0        0        0        0 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/validation/__init__.py
+-rw-r--r--   0        0        0    11118 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/validation/definition_ontology_rule.py
+-rw-r--r--   0        0        0     7492 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/validation/disjointness_rule.py
+-rw-r--r--   0        0        0     1729 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/validation/lint_utils.py
+-rw-r--r--   0        0        0     1402 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/validation/ontology_rule.py
+-rw-r--r--   0        0        0     1275 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/validation/rule_runner.py
+-rw-r--r--   0        0        0      122 2024-04-25 00:55:39.900864 oaklib-0.6.4/src/oaklib/utilities/writers/__init__.py
+-rw-r--r--   0        0        0    16522 2024-04-25 00:55:39.900864 oaklib-0.6.4/src/oaklib/utilities/writers/change_handler.py
+-rw-r--r--   0        0        0     9171 1970-01-01 00:00:00.000000 oaklib-0.6.4/PKG-INFO
```

### Comparing `oaklib-0.6.3/LICENSE` & `oaklib-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/README.md` & `oaklib-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/pyproject.toml` & `oaklib-0.6.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oaklib"
-version = "v0.6.3"
+version = "v0.6.4"
 description = "Ontology Access Kit: Python library for common ontology operations over a variety of backends"
 authors = ["cmungall <cjm@berkeleybop.org>"]
 
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0.0"
```

### Comparing `oaklib-0.6.3/src/oaklib/cli.py` & `oaklib-0.6.4/src/oaklib/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 Command Line Interface to OAK
------------------------------
+----------------------
 
 Executed using "runoak" command
 """
 
 # TODO: order commands.
 # See https://stackoverflow.com/questions/47972638/how-can-i-define-the-order-of-click-sub-commands-in-help
 import itertools
@@ -1067,15 +1067,15 @@
 @autolabel_option
 @output_option
 def search(terms, output_type: str, autolabel, output: TextIO):
     """
     Searches ontology for entities that have a label, alias, or other property matching a search term.
 
     Example:
-    -------
+
         runoak -i uberon.obo search limb
 
     This uses the Pronto implementation to load uberon from disk, and does a basic substring
     search over the labels and synonyms - results are not ranked
 
     Bioportal (all ontologies):
 
@@ -1132,36 +1132,36 @@
 @main.command()
 @output_option
 def subsets(output: str):
     """
     Shows information on subsets
 
     Example:
-    -------
+
         runoak -i obolibrary:go.obo subsets
 
     Example:
-    -------
+
         runoak -i cl.owl subsets
 
     For background on subsets, see https://incatools.github.io/ontology-access-kit/concepts.html#subsets
 
     Note you can use subsets in selector queries for other commands; e.g. to fetch all
     terms (directly) in goslim_generic in GO:
 
     Example:
-    -------
+
         runoak -i sqlite:obo:go info .in goslim_generic
 
     Python API:
 
        https://incatools.github.io/ontology-access-kit/interfaces/basic
 
     See Also:
-    --------
+    -
         term-subsets command, which shows relationships of terms to subsets
 
     """
     impl = settings.impl
     if isinstance(impl, BasicOntologyInterface):
         for subset in impl.subsets():
             print(f"{subset} ! {impl.label(subset)}")
@@ -1188,33 +1188,33 @@
 def obsoletes(
     terms, include_merged: bool, show_migration_relationships: bool, output_type: str, output: str
 ):
     """
     Shows all obsolete entities.
 
     Example:
-    -------
+
         runoak -i obolibrary:go.obo obsoletes
 
     To exclude *merged terms*, use the ``--no-include-merged`` flag
 
     Example:
-    -------
+
         runoak -i obolibrary:go.obo obsoletes --no-include-merged
 
     To show migration relationships, use the ``--show-migration-relationships`` flag
 
     Example:
-    -------
+
         runoak -i obolibrary:go.obo obsoletes --show-migration-relationships
 
     You can also specify terms to show obsoletes for:
 
     Example:
-    -------
+
         runoak -i obolibrary:go.obo obsoletes --show-migration-relationships GO:0000187 GO:0000188
 
     More examples:
 
        https://github.com/INCATools/ontology-access-kit/blob/main/notebooks/Commands/TaxonConstraints.ipynb
 
     Python API:
@@ -1281,29 +1281,29 @@
     output_type: str,
     output: str,
 ):
     """
     Shows all descriptive/summary statistics
 
     Example:
-    -------
+
         runoak -i sqlite:obo:pr statistics
 
     By default, this will show combined summary statistics for all terms
 
     You can also break down the statistics in two ways:
 
     - by a collection of branch roots
 
     - by a metadata property (e.g. oio:hasOBONamespace, rdfs:isDefinedBy)
 
     - by prefix (e.g. GO, PR, CL, OBI)
 
     Example:
-    -------
+
         runoak -i sqlite:obo:pr statistics -p oio:hasOBONamespace
 
     Note: the oio:hasOBONamespace is *not* the same as the ID prefix, it is
     a field that is used by a subset of ontologies to partition classes into
     broad groupings, similar to subsets. Its use is non-standard, yet a lot
     of ontologies use this as the main partitioning mechanism.
 
@@ -1330,15 +1330,15 @@
     Change statistics:
 
     You can optionally combine the ontology statistics with a change
     summary relative to another ontology, using the ``--compare-with``
     option.
 
     Example:
-    -------
+
         runoak -i v2.obo statistics --group-by-obo-namespace --compare-with v1.obo
 
     This will also include change stats broken down by KGCL change types. If
     a group-by option is specified, these will be grouped accordingly.
 
     Python API:
 
@@ -1447,15 +1447,15 @@
 def ontology_versions(ontologies, output: str, all: bool):
     """
     Shows ontology versions
 
     Currently only implemented for BioPortal
 
     Example:
-    -------
+
         runoak -i bioportal: ontology-versions mp
 
     All ontologies:
 
         runoak -i bioportal ontology-versions --all
 
     Python API:
@@ -1485,27 +1485,27 @@
 @all_ontologies_option
 @click.argument("ontologies", nargs=-1)
 def ontology_metadata(ontologies, output_type: str, output: str, all: bool):
     """
     Shows ontology metadata
 
     Example:
-    -------
+
         runoak -i bioportal: ontology-metadata obi uberon foodon
 
     Use the ``--all`` option to show all ontologies
 
     Example:
-    -------
+
         runoak -i bioportal: ontology-metadata --all
 
     By default the output is YAML. You can get the results as TSV:
 
     Example:
-    -------
+
         runoak -i bioportal: ontology-metadata --all -O csv
 
     .. warning::
 
         The output data model is not yet standardized -- this may change in future
 
     Python API:
@@ -1543,15 +1543,15 @@
 @additional_metadata_option
 @click.argument("terms", nargs=-1)
 def term_metadata(terms, predicates, additional_metadata: bool, output_type: str, output: str):
     """
     Shows term metadata.
 
     Example:
-    -------
+
         runoak -i sqlite:obo:uberon term-metadata lung heart
 
     You can filter the results for only selected predicates:
 
         runoak -i sqlite:obo:uberon term-metadata lung heart -p id,oio:hasDbXref
 
     The default output is YAML documents, where each YAML document is a term, with
@@ -1662,36 +1662,36 @@
     """
     Annotate a piece of text using a Named Entity Recognition annotation.
 
     Some endpoints such as BioPortal have built-in support for annotation;
     in these cases the endpoint functionality is used:
 
     Example:
-    -------
+
         runoak -i bioportal: annotate "enlarged nucleus in T-cells from peripheral blood"
 
     For other endpoints, the built-in OAK annotator is used. This currently uses a basic
     algorithm based on lexical matching.
 
     Example:
-    -------
+
         runoak -i sqlite:obo:cl annotate "enlarged nucleus in T-cells from peripheral blood"
 
     Using the builtin annotator can be slow, as the lexical index is re-built every time.
     To preserve this, use the ``--lexical-index-file`` (``-L``) option to specify a file to save.
     On subsequent iterations the file is reused.
 
     You can also use ``--text-file`` to pass in a text file to be parsed one line at a time
 
     If gilda is installed as an extra, it can be used,
     but ``--matches-whole-text`` (``-W``) must be specified,
     as gilda only performs grounding.
 
     Example:
-    -------
+
         runoak -i gilda: annotate -W BRCA2
 
     Aliases can be listed in the output by setting the flag
     --include-aliases to `true` (default: false).
 
     Example (using the plugin oakx-spacy):
 
@@ -1826,15 +1826,15 @@
     see https://incatools.github.io/ontology-access-kit/interfaces/obograph
 
     .. note::
 
        This requires that `obographviz <https://github.com/INCATools/obographviz>`_ is installed.
 
     Example:
-    -------
+
         runoak -i sqlite:cl.db viz CL:4023094
 
     Same query on ubergraph:
 
         runoak -i ubergraph: viz CL:4023094
 
     Example, showing only is-a:
@@ -1979,15 +1979,15 @@
 ):
     """
     Display an ancestor graph as an ascii/markdown tree.
 
     For general instructions, see the viz command, which this is analogous too.
 
     Example:
-    -------
+
         runoak -i envo.db tree ENVO:00000372 -p i,p
 
     This produces output like:
 
     .packages::
 
                         * [i] ENVO:00000094 ! volcanic feature
@@ -1998,24 +1998,24 @@
 
     Note: for many ontologies the tree view will explode, especially if no predicates are specified.
     You may wish to start with the is-a tree (-p i).
 
     You can use the --gap-fill option to create a minimal tree:
 
     Example:
-    -------
+
         runoak -i envo.db tree --gap-fill 'pyroclastic shield volcano' 'subglacial volcano' volcano -p i
 
     This will show the tree containing only these terms, and the most direct inferred relationships between them.
 
     You can also give a list of leaf terms and specify --add-mrcas alongside --gap-fill to fill in
     the most informative intermediate classes:
 
     Example:
-    -------
+
         runoak -i envo.db tree --add-mrcas --gap-fill 'pyroclastic shield volcano'\
             'subglacial volcano' 'mud volcano' -p i
 
     This will fill in the term "volcano", as it is the most recent common ancestor of the specified terms
 
     The --max-hops option can control the distance
 
@@ -2122,15 +2122,15 @@
     """
     List all ancestors of a given term or terms.
 
     Here ancestor means the transitive closure of the parent relationship, where
     a parent includes all relationship types, not just is-a.
 
     Example:
-    -------
+
         runoak -i cl.owl ancestors CL:4023094
 
     This will show ancestry over the full relationship graph. Like any relational
     OAK command, this can be filtered by relationship type (predicate), using --predicate (-p).
     For example, constrained to is-a and part-of:
 
         runoak -i cl.owl ancestors CL:4023094 -p i,BFO:0000050
@@ -2246,52 +2246,52 @@
     output_type: str,
     output: str,
 ):
     """
     List all paths between one or more start curies.
 
     Example:
-    -------
+
         runoak -i sqlite:obo:go paths  -p i,p 'nuclear membrane'
 
     This shows all shortest paths from nuclear membrane to all ancestors
 
     Example:
-    -------
+
         runoak -i sqlite:obo:go paths  -p i,p 'nuclear membrane' --target cytoplasm
 
     This shows shortest paths between two nodes
 
     Example:
-    -------
+
         runoak -i sqlite:obo:go paths  -p i,p 'nuclear membrane' 'thylakoid' --target cytoplasm 'thylakoid membrane'
 
     This shows all shortest paths between 4 combinations of starts and ends
 
     You can also use "@" to separate start node list and end node list. Like most OAK commands,
     you can pass either explicit terms, or term queries. For example, if you have two files of IDs,
     then you can do this:
 
         runoak -i sqlite:obo:go paths  -p i,p .idfile START_NODES.txt @ .idfile END_NODES.txt
 
     You can also pass in weights for each predicate, used when calculating shortest paths.
 
     Example:
-    -------
+
         runoak -i sqlite:obo:go paths  -p i,p 'nuclear membrane' --target cytoplasm \
                 --predicate-weights "{i: 0.0001, p: 999}"
 
     This shows all shortest paths after weighting relations
 
     (Note: you can use the same shorthands as in the `--predicates` option)
 
     This command can be combined with others to visualize the paths.
 
     Example:
-    -------
+
         alias go="runoak -i sqlite:obo:go"
         go paths  -p i,p 'nuclear membrane' --target cytoplasm --narrow | go viz --fill-gaps -
 
     This visualizes the path by first exporting the path as a flat list, then passing the
     results to viz, using the fill-gaps option.
 
     More examples:
@@ -2432,15 +2432,15 @@
 @output_option
 @ontological_output_type_option
 def siblings(terms, predicates, output_type: str, output: str):
     """
     List all siblings of a specified term or terms
 
     Example:
-    -------
+
         runoak -i cl.owl siblings CL:4023094
 
     Note that siblings is by default over ALL relationship types, so we recommend
     always being explicit and passing a predicate using -p (--predicates)
 
     """
     impl = settings.impl
@@ -2473,19 +2473,19 @@
 def descendants(
     terms, predicates, graph_traversal_method, display: str, output_type: str, output: TextIO
 ):
     """
     List all descendants of a term
 
     Example:
-    -------
+
         runoak -i sqlite:obo:obi descendants assay -p i
 
     Example:
-    -------
+
         runoak -i sqlite:obo:uberon descendants heart -p i,p
 
     This is the inverse of the 'ancestors' command; see the documentation for
     that command. But note that 'descendants' commands have the potential to be more
     "explosive" than ancestors commands, especially for high level terms, and for when
     predicates are not specified
 
@@ -2527,29 +2527,29 @@
     help="Forces the serialization to be in canonical order, which is useful for diffing",
 )
 def dump(terms, output, output_type: str, config_file: str = None, **kwargs):
     """
     Exports (dumps) the entire contents of an ontology.
 
     Example:
-    -------
+
         runoak -i pato.obo dump -o pato.json -O json
 
     Example:
-    -------
+
         runoak -i pato.owl dump -o pato.ttl -O turtle
 
     You can also pass in a JSON configuration file to parameterize the dump process.
 
     Currently this is only used for fhirjson dumps, the configuration options are specified here:
 
     https://incatools.github.io/ontology-access-kit/converters/obo-graph-to-fhir.html
 
     Example:
-    -------
+
         runoak -i pato.owl dump -o pato.ttl -O fhirjson -c fhir_config.json -o pato.fhir.json
 
     Currently each implementation only supports a subset of formats.
 
     The dump command is also blocked for remote endpoints such as Ubergraph,
     to avoid killer queries.
 
@@ -2586,29 +2586,29 @@
     help="""Name of transformation to apply.""",
 )
 def transform(terms, transform, output, output_type: str, config_file: str = None, **kwargs):
     """
     Transforms an ontology
 
     Example:
-    -------
+
         runoak -i pato.obo dump -o pato.json -O json
 
     Example:
-    -------
+
         runoak -i pato.owl dump -o pato.ttl -O turtle
 
     You can also pass in a JSON configuration file to parameterize the dump process.
 
     Currently this is only used for fhirjson dumps, the configuration options are specified here:
 
     https://incatools.github.io/ontology-access-kit/converters/obo-graph-to-fhir.html
 
     Example:
-    -------
+
         runoak -i pato.owl dump -o pato.ttl -O fhirjson -c fhir_config.json -o pato.fhir.json
 
     Currently each implementation only supports a subset of formats.
 
     The dump command is also blocked for remote endpoints such as Ubergraph,
     to avoid killer queries.
 
@@ -2675,15 +2675,15 @@
             sh:namespace CL: ;
             sh:prefix "CL" .
 
     The default prefixmap is always used, unless options are passed specifying additional
     prefix maps.
 
     Example:
-    -------
+
         runoak --named-prefix-map prefixcc prefixes
 
     If an ontology is loaded, then --used-only can be used to restrict to
     prefixes for entities in that ontology
 
         runoak -i sqlite:obo:cl prefixes --used-only
 
@@ -2785,15 +2785,15 @@
     Determine pairwise similarity between two terms using a variety of metrics
 
     NOTE: this command may be deprecated, consider using similarity
 
     Note: We recommend always specifying explicit predicate lists
 
     Example:
-    -------
+
         runoak -i ubergraph: similarity-pair -p i,p CL:0000540 CL:0000000
 
     You can omit predicates if you like but be warned this may yield
     hard to interpret results.
 
     E.g.
 
@@ -2891,29 +2891,29 @@
 
     Input sets of a terms can be specified in different ways:
 
     - via a file
     - via explicit lists of terms or queries
 
     Example:
-    -------
+
         runoak -i hp.db similarity -p i --set1-file HPO-TERMS1 --set2-file HPO-TERMS2 -O csv
 
     This will compare every term in TERMS1 vs TERMS2
 
     Alternatively standard OAK term queries can be used, with "@" separating the two lists
 
     Example:
-    -------
+
         runoak -i hp.db similarity -p i TERM_1 TERM_2 ... TERM_N @ TERM_N+1 ... TERM_M
 
     The .all term syntax can be used to select all terms in an ontology
 
     Example:
-    -------
+
         runoak -i ma.db similarity -p i,p .all @ .all
 
     This can be mixed with other term selectors; for example to calculate the similarity of "neuron"
     vs all terms in CL:
 
         runoak -i cl.db similarity -p i,p .all @ neuron
 
@@ -3008,15 +3008,15 @@
 ):
     """
     Termset similarity.
 
     This calculates a similarity matrix for two sets of terms.
 
     Example:
-    -------
+
         runoak -i go.db termset-similarity -p i,p nucleus membrane @ "nuclear membrane" vacuole -p i,p
 
     Python API:
 
        https://incatools.github.io/ontology-access-kit/interfaces/semantic-similarity
 
     Data model:
@@ -3063,15 +3063,15 @@
     output_type: str,
     use_associations: bool,
 ):
     """
     Show information content for term or list of terms
 
     Example:
-    -------
+
         runoak -i cl.db information-content -p i .all
 
     Like all OAK commands that operate over graphs, the graph traversal is controlled
     by the `--predicates` option. In the above case, the frequency of each term is equal to
     the number of reflexive is-a descendants of the term divided by total number of terms
 
     By default, the ontology is used as the corpus for computing term frequency.
@@ -3112,15 +3112,15 @@
 @display_option
 @output_type_option
 def info(terms, output: TextIO, display: str, output_type: str):
     """
     Show information on term or set of terms
 
     Example:
-    -------
+
         runoak -i sqlite:obo:cl info CL:4023094
 
     The default output is minimal, showing only ID and label
 
     The --output-type (-O) option can be used to specify other formats for the output.
 
     Currently there are only a few output types are supported. More will be provided in future.
@@ -3171,15 +3171,15 @@
 
 @main.command()
 def languages():
     """
     Show available languages
 
     Example:
-    -------
+
         runoak languages
 
     """
     impl = settings.impl
     if not isinstance(impl, BasicOntologyInterface):
         raise NotImplementedError(f"Cannot execute this using {impl} of type {type(impl)}")
     for lang in impl.languages():
@@ -3205,21 +3205,21 @@
     pivot_languages: bool,
     all_languages: bool,
 ):
     """
     Show labels for term or list of terms
 
     Example:
-    -------
+
         runoak -i cl.owl labels CL:4023093 CL:4023094
 
     You can use the ".all" selector to show all labels:
 
     Example:
-    -------
+
         runoak -i cl.owl labels .all
 
     (this may be blocked for remote endpoints)
 
     You can query for terms that have either no label, or to include only ones with labels:
 
     Nodes with no labels:
@@ -3227,21 +3227,21 @@
         runoak -i cl.owl labels .all --if-absent exclude
 
     Multilingual support: if the adapter supports multilingual querying
     (currently only SQL) *and* the ontology has multilingual support, you can restrict results to
     a particular language.
 
     Example:
-    -------
+
         runoak --preferred-language fr -i sqlite:obo:hpinternational labels .ancestors HP:0020110
 
     You can also query for all languages, and see these pivoted:
 
     Example:
-    -------
+
         runoak  -i sqlite:obo:hpinternational labels .ancestors HP:0020110 --pivot-languages
 
     Python API:
 
        https://incatools.github.io/ontology-access-kit/interfaces/labels
 
     """
@@ -3317,22 +3317,22 @@
     lookup_references: bool,
     set_value,
 ):
     """
     Show textual definitions for term or set of terms
 
     Example:
-    -------
+
 
         runoak -i sqlite:obo:envo definitions 'tropical biome' 'temperate biome'
 
     You can use the ".all" selector to show all definitions for all terms in the ontology:
 
     Example:
-    -------
+
 
         runoak -i sqlite:obo:envo definitions .all
 
     You can also include definition metadata, such as provenance and source:
 
         runoak -i sqlite:obo:cl definitions --additional-metadata neuron
 
@@ -3406,14 +3406,20 @@
 @click.option(
     "--include-entailed/--no-include-entailed",
     default=False,
     show_default=True,
     help="Include entailed indirect relationships",
 )
 @click.option(
+    "--non-redundant-entailed/--no-non-redundant-entailed",
+    default=False,
+    show_default=True,
+    help="Include entailed but exclude entailed redundant relationships",
+)
+@click.option(
     "--include-tbox/--no-include-tbox",
     default=True,
     show_default=True,
     help="Include class-class relationships (subclass and existentials)",
 )
 @click.option(
     "--include-abox/--no-include-abox",
@@ -3435,41 +3441,42 @@
     output_type: str,
     output: str,
     if_absent: bool,
     set_value: str,
     include_entailed: bool,
     include_tbox: bool,
     include_abox: bool,
+    non_redundant_entailed: bool,
     include_metadata: bool,
 ):
     """
     Show all relationships for a term or terms
 
     By default, this shows all relationships where the input term(s) are the *subjects*
 
     Example:
-    -------
+
         runoak -i cl.db relationships CL:4023094
 
     Like all OAK commands, a label can be passed instead of a CURIE
 
     Example:
-    -------
+
         runoak -i cl.db relationships neuron
 
     To reverse the direction, and query where the search term(s) are *objects*, use the --direction flag:
 
     Example:
-    -------
+
         runoak -i cl.db relationships --direction down neuron
 
     Multiple terms can be passed
 
     Example:
-    -------
+
         runoak -i uberon.db relationships heart liver lung
 
     And like all OAK commands, a query can be passed rather than an explicit term list
 
     The following query lists all arteries in the limb together which what structures they supply
 
     Query:
@@ -3505,14 +3512,23 @@
     down_it = impl.relationships(
         objects=curies,
         predicates=actual_predicates,
         include_abox=include_abox,
         include_tbox=include_tbox,
         include_entailed=include_entailed,
     )
+    if non_redundant_entailed:
+        if not isinstance(impl, OboGraphInterface):
+            raise NotImplementedError(f"Cannot execute this using {impl} of type {type(impl)}")
+        up_it = impl.non_redundant_entailed_relationships(
+            subjects=curies,
+            predicates=actual_predicates,
+            include_abox=include_abox,
+            include_tbox=include_tbox,
+        )
     if direction is None or direction == Direction.up.value:
         it = up_it
     elif direction == Direction.down.value:
         it = down_it
     else:
         it = chain(up_it, down_it)
     has_relationships = defaultdict(bool)
@@ -3611,28 +3627,28 @@
         restrictions:
         - fillerId: PATO:0000461
           propertyId: RO:0015010
 
     You can also specify CSV to generate a flattened form of this.
 
     Example:
-    -------
+
         pato logical-definitions .all --output-type csv
 
     You can optionally choose to "--matrix-axes" to transform the output to a matrix form.
     This is a comma-separated pair of axes, where each element is a logical definition element
     type: "f" for filler, "p" for predicate, "g" for genus, "d" for defined class.
 
     Example:
-    -------
+
     - Each property/predicate is a column
     - For repeated properties, columns of the form prop_1, prop_2, ... are generated
 
     Example:
-    -------
+
         pato logical-definitions .all  --matrix-axes d,p --output-type csv
 
     This will generate a row for each defined class with a logical definition, with columns
     for each predicate ("genus" is treated as a predicate here).
 
     Limitations:
 
@@ -3748,30 +3764,30 @@
     """
     Show all disjoints for a set of terms, or whole ontology.
 
     Leave off all arguments for defaults - all terms, YAML OboGraph model
     serialization:
 
     Example:
-    -------
+
         runoak -i sqlite:obo:uberon disjoints
 
     Note that this will include pairwise disjoints, setwise disjoints,
     disjoint unions, and disjoints involving simple class expressions.
 
     A tabular format can be easier to browse, and includes labels by default:
 
     Example:
-    -------
+
         runoak -i sqlite:obo:uberon disjoints --autolabel -O csv
 
     To perform this on a subset:
 
     Example:
-    -------
+
         runoak -i sqlite:obo:cl disjoints --autolabel -O csv  .desc//p=i "immune cell"
 
     Data model:
 
        https://w3id.org/oak/obograph
 
     """
@@ -3865,15 +3881,15 @@
 @output_option
 @owl_type_option
 def terms(output: str, owl_type, filter_obsoletes: bool):
     """
     List all terms in the ontology
 
     Example:
-    -------
+
         runoak -i db/cob.db terms
 
     All terms without obsoletes:
 
         runoak -i prontolib:cl.obo  terms --filter-obsoletes
 
     By default "terms" is considered to be any entity type in the ontology. Use --owl-type to constrain this:
@@ -3917,15 +3933,15 @@
 
     Like all OAK relational commands, this is parameterized by --predicates (-p).
     Note that the default is to return the roots of the relation graph over *all* predicates.
     This can sometimes give unintuitive results, so we recommend always being explicit
     and parameterizing
 
     Example:
-    -------
+
         runoak -i db/cob.db roots
 
     This command is a wrapper onto the "roots" command in the BasicOntologyInterface.
 
     - https://incatools.github.io/ontology-access-kit/interfaces/basic.html#
       oaklib.interfaces.basic_ontology_interface.BasicOntologyInterface.roots
 
@@ -3954,15 +3970,15 @@
     """
     List all leaf nodes in the ontology
 
     Like all OAK relational commands, this is parameterized by --predicates (-p).
     Note that the default is to return the roots of the relation graph over *all* predicates
 
     Example:
-    -------
+
         runoak -i db/cob.db leafs
 
     This command is a wrapper onto the "leafs" command in the BasicOntologyInterface.
 
     - https://incatools.github.io/ontology-access-kit/interfaces/basic.html#
       oaklib.interfaces.basic_ontology_interface.BasicOntologyInterface.leafs
 
@@ -3986,15 +4002,15 @@
 
     Like all OAK relational commands, this is parameterized by --predicates (-p).
     Note that the default is to return the singletons of the relation graph over *all* predicates
 
     Obsoletes are filtered by default
 
     Example:
-    -------
+
         runoak -i db/cob.db singletons
 
     This command is a wrapper onto the "singletons" command in the BasicOntologyInterface.
 
     - https://incatools.github.io/ontology-access-kit/interfaces/basic.html#
       oaklib.interfaces.basic_ontology_interface.BasicOntologyInterface.singletons
 
@@ -4023,15 +4039,15 @@
 )
 @click.argument("terms", nargs=-1)
 def mappings(terms, maps_to_source, autolabel: bool, output, output_type, mapper):
     """
     List all mappings encoded in the ontology
 
     Example:
-    -------
+
         runoak -i sqlite:obo:envo mappings
 
     The default output is SSSOM YAML. To use the (canonical) csv format:
 
         runoak -i sqlite:obo:envo mappings -O sssom
 
     By default, labels are not included. Use --autolabel to include labels (but note
@@ -4095,15 +4111,15 @@
 )
 @click.argument("terms", nargs=-1)
 def normalize(terms, maps_to_source, autolabel: bool, output, output_type):
     """
     Normalize all input identifiers.
 
     Example:
-    -------
+
         runoak -i translator: normalize HGNC:1 HGNC:2 -M NCBIGene
 
     Python API:
 
        https://incatools.github.io/ontology-access-kit/interfaces/mapping-provider
 
     Data model:
@@ -4138,15 +4154,15 @@
 @output_option
 @click.argument("terms", nargs=-1)
 def aliases(terms, output, output_type, obo_model):
     """
     List aliases for a term or set of terms.
 
     Example:
-    -------
+
         runoak -i ubergraph:uberon aliases UBERON:0001988
 
     TERMS should be either an explicit list of terms or queries, or can be a selector query,
     such as '.all' to fetch all terms in the ontology
 
     Show all aliases:
 
@@ -4196,15 +4212,15 @@
 @output_type_option
 @click.argument("terms", nargs=-1)
 def term_subsets(terms, output, output_type):
     """
     List subsets for a term or set of terms.
 
     Example:
-    -------
+
         runoak -i sqlite:obo:uberon term-subsets heart lung
 
     Python API:
 
        https://incatools.github.io/ontology-access-kit/interfaces/basic
 
     """
@@ -4224,15 +4240,15 @@
 @predicates_option
 @click.argument("subsets", nargs=-1)
 def expand_subsets(subsets: list, output, predicates):
     """
     For each subset provide a mapping of each term in the ontology to a subset
 
     Example:
-    -------
+
         runoak -i db/pato.db expand-subsets attribute_slim value_slim
 
     """
     impl = settings.impl
     # writer = StreamingCsvWriter(output)
     if isinstance(impl, OboGraphInterface):
         actual_predicates = _process_predicates_arg(predicates)
@@ -4283,23 +4299,23 @@
 @click.option("--references", multiple=True, help="CURIEs that the axiom references")
 @click.argument("terms", nargs=-1)
 def axioms(terms, output: str, output_type: str, axiom_type: str, about: str, references: tuple):
     """
     Filters axioms
 
     Example:
-    -------
+
         runoak -i cl.ofn axiom
 
     The above will write all axioms.
 
     You can filter by axiom type:
 
     Example:
-    -------
+
         runoak -i cl.ofn axiom --axiom-type SubClassOf
 
     Note this currently only works with the funowl adapter, on functional syntax files
 
     """
     impl = settings.impl
     writer = StreamingAxiomWriter(syntax=output_type, functional_writer=impl.functional_writer)
@@ -4362,19 +4378,19 @@
     This will apply rules using the inferred ancestors of subject terms, as well as inferred
     ancestors/descendants of taxon terms.
 
     The input ontology MUST include both the taxon constraint relationships AND the relevant portion
     of NCBI Taxonomy
 
     Example:
-    -------
+
         runoak -i db/go.db taxon-constraints GO:0034357 --include-redundant -p i,p
 
     Example:
-    -------
+
         runoak -i sqlite:obo:uberon taxon-constraints UBERON:0003884 UBERON:0003941 -p i,p
 
     More examples:
 
        https://github.com/INCATools/ontology-access-kit/blob/main/notebooks/Commands/TaxonConstraints.ipynb
 
     This command is a wrapper onto taxon_constraints_utils:
@@ -4428,27 +4444,27 @@
     """
     Test candidate taxon constraints
 
     Multiple candidate constraints can be passed as arguments. these are in the form of triples
     separated by periods.
 
     Example:
-    -------
+
         runoak  -i db/go.db apply-taxon-constraints -p i,p GO:0005743 only NCBITaxon:2759
         never NCBITaxon:2 . GO:0005634 only NCBITaxon:2
 
     The --evolution-file (-E) option can be used to pass in a file of candidates.
     This should follow the format used in https://arxiv.org/abs/1802.06004
 
     E.g.
 
         GO:0000229,Gain|NCBITaxon:1(root);>Loss|NCBITaxon:2759(Eukaryota);
 
     Example:
-    -------
+
         runoak  -i db/go.db eval-taxon-constraints -p i,p -E tests/input/go-evo-gains-losses.csv
 
     More examples:
 
        https://github.com/INCATools/ontology-access-kit/blob/main/notebooks/Commands/Apply.ipynb
 
     """
@@ -4540,38 +4556,38 @@
     set_value: str,
     **kwargs,
 ):
     """
     Lookup associations from or to entities.
 
     Example:
-    -------
+
         runoak -i sqlite:obo:hp -g test.hpoa -G hpoa associations
 
     The above will show all associations
 
     To query using an ontology term, including is-a closure, specify one or more
     terms or term queries, plus the closure predicate(s), e.g.
 
     Example:
-    -------
+
         runoak -i sqlite:obo:hp -g test.hpoa -G hpoa associations -p i HP:0001392
 
     This shows all annotations either to "Abnormality of the liver" (HP:0001392), or
     to is-a descendants.
 
     Using input specifications:
 
     It can be awkward to specify both input ontology and association path and format. You
     can use input specifications to bundle common combinations of inputs together.
 
     For example, the go-dictybase-input-spec combines go plus dictybase associations.
 
     Example:
-    -------
+
         runoak --i src/oaklib/conf/go-dictybase-input-spec.yaml associations -p i,p GO:0008104
 
     More examples:
 
        https://github.com/INCATools/ontology-access-kit/blob/main/notebooks/Commands/Associations.ipynb
 
     """
@@ -4698,31 +4714,31 @@
     filter,
     **kwargs,
 ):
     """
     Count associations, grouped by subject or object
 
     Example:
-    -------
+
         runoak -i sqlite:obo:hp -g test.hpoa -G hpoa associations-counts
 
     This will default to summarzing by objects (HPO term), showing the number
     of associations for each term.
 
     This will be direct counts only. To include is-a closure, specify
     the closure predicate(s), e.g.
 
     Example:
-    -------
+
         runoak -i sqlite:obo:hp -g test.hpoa -G hpoa associations -p i
 
     You can also group by other fields
 
     Example:
-    -------
+
         runoak -i sqlite:obo:hp -g test.hpoa -G hpoa associations-counts --group-by subject
 
     This will show the number of associations for each disease.
 
     OAK also includes a number of specialized adapters that implement this method
     for particular databases.
 
@@ -4816,15 +4832,15 @@
     Co-annotation matrix query.
 
     This queries for co-annotations between pairs of terms.
 
     See: Wood V., Carbon S., et al, https://royalsocietypublishing.org/doi/10.1098/rsob.200149
 
     Example:
-    -------
+
 
         runoak  -i amigo:NCBITaxon:9606 associations-matrix -p i,p GO:0042416 GO:0014046
 
     As a heatmap:
 
         runoak  -i amigo:NCBITaxon:9606 associations-matrix -p i,p GO:0042416 GO:0014046 -o heatmap > /tmp/heatmap.png
 
@@ -4888,15 +4904,15 @@
     The report will list associations where the subject is one of the terms provided. The
     associations will be grouped by any provided --object-group options. This option can be
     provided multiple times. If the value is a comma separated list of object IDs, the first
     will be used as a primary grouping dimension and the remainder will be used to create
     sub-groups.
 
     Example:
-    -------
+
         runoak -i sqlite:go.db -g wb.gaf -G gaf rollup \
             --object-group GO:0032502,GO:0007568,GO:0048869,GO:0098727 \
             --object-group GO:0008152,GO:0009056,GO:0044238,GO:1901275 \
             --object-group GO:0050896,GO:0051716,GO:0051606,GO:0051606,GO:0014823 \
             --object-group=GO:0023052 \
             --output rollup.html \
             WB:WBGene00000417 WB:WBGene00000912 WB:WBGene00000898 WB:WBGene00006752
@@ -5038,15 +5054,15 @@
     """
     Run class enrichment analysis.
 
     Given a sample file of identifiers (e.g. gene IDs), plus a set of associations (e.g. gene to term
     associations, return the terms that are over-represented in the sample set.
 
     Example:
-    -------
+
         runoak -i sqlite:obo:uberon -g gene2anat.txt -G g2t enrichment -U my-genes.txt -O csv
 
     This runs an enrichment using Uberon on my-genes.txt, using the gene2anat.txt file as the
     association file (assuming simple gene-to-term format). The output is in CSV format.
 
     It is recommended you always provide a background set, including all the entity identifiers
     considered in the experiment.
@@ -5127,15 +5143,15 @@
     other_associations: str,
     **kwargs,
 ):
     """
     Diffs two association sources.
 
     Example:
-    -------
+
         runoak -i sqlite:obo:go  -G gaf  diff-associations \
            --old-date ${date1} --new-date ${date2} \
            -g  "${download_dir}/${group}-${date1}.gaf" \
            -X "${download_dir}/${group}-${date2}.gaf" \
            --group-by publications -p i,p \
            -o "${group}-diff-${date1}-to-${date2}.tsv
 
@@ -5226,26 +5242,26 @@
 ):
     """
     Validate an ontology against ontology metadata
 
     Implementation notes: Currently only works on SQLite
 
     Example:
-    -------
+
         runoak  -i db/ecto.db validate -o results.tsv
 
     The default validation performed is structural (conformance to the ontology_metadata schema)
 
     There is experimental support for additional ontology rules, which includes heuristic methods
     such as aligning text and logical definitions. These are off by default.
 
     To run these, pass --no-skip-ontology-rules
 
     Example:
-    -------
+
         runoak -i db/uberon.db validate --skip-structural-validation --no-skip-ontology-rules
 
     For more information, see the OAK how-to guide:
 
     - https://incatools.github.io/ontology-access-kit/howtos/validate-an-obo-ontology.html
 
     """
@@ -5379,24 +5395,24 @@
 
     By default this will apply basic text mining of text definitions to check
     against machine actionable OBO text definition guideline rules.
     This can result in an initial lag - to skip this, and ONLY perform
     checks for *presence* of definitions, use --skip-text-annotation:
 
     Example:
-    -------
+
 
         runoak validate-definitions -i db/uberon.db --skip-text-annotation
 
     Like most OAK commands, this accepts lists of terms or term queries
     as arguments. You can pass in a CURIE list to selectively validate
     individual classes
 
     Example:
-    -------
+
 
          runoak validate-definitions -i db/cl.db CL:0002053
 
     Only on CL identifiers:
 
         runoak validate-definitions -i db/cl.db i^CL:
 
@@ -5629,15 +5645,15 @@
 
     Note: the specified ontology is modified in place
 
     The input for this command is a list equals-separated pairs, specifying the
     source and the target
 
     Example:
-    -------
+
         runoak -i db/uberon.db migrate-curies --replace SRC1=TGT1 SRC2=TGT2
 
     This command is a wrapper onto the "migrate_curies" command in the PatcherInterface
 
     - https://incatools.github.io/ontology-access-kit/interfaces/patcher.html#
     oaklib.interfaces.patcher_interface.PatcherInterface.migrate_curies
 
@@ -5661,15 +5677,15 @@
 @click.option("--endpoint", "-e", required=True, help="Name of endpoint, e.g. bioportal")
 @click.argument("keyval")
 def set_apikey(endpoint, keyval):
     """
     Sets an API key
 
     Example:
-    -------
+
         oak set-apikey -e bioportal MY-KEY-VALUE
 
     This is stored in an OS-dependent path
 
     """
     set_apikey_value(endpoint, keyval)
 
@@ -5753,15 +5769,15 @@
 def lexmatch(
     output, recreate, ensure_strict_prefixes, rules_file, lexical_index_file, add_labels, terms
 ):
     """
     Performs lexical matching between pairs of terms in one more more ontologies.
 
     Examples
-    --------
+    -
         runoak -i foo.obo lexmatch -o foo.sssom.tsv
 
     In this example, the input ontology file is assumed to contain all pairs of terms to be mapped.
 
     It is more common to map between all pairs of terms in two ontology files. In this case,
     you can merge the ontologies using a tool like ROBOT; or,  to avoid a merge
     preprocessing step, use the --addl (-a) option to specify a second ontology file.
@@ -5931,15 +5947,15 @@
     output_type,
     other_ontology,
 ):
     """
     Compute difference between two ontologies.
 
     Example:
-    -------
+
         runoak -i foo.obo diff -X bar.obo -o diff.yaml
 
     This will produce a list of Changes that are required to go from the main input ontology (--input)
     to the other ontology (--other-ontology, or -X).
 
     The output follows the KGCL data model.
     See https://incatools.github.io/ontology-access-kit/datamodels/kgcl/index.html
@@ -5959,15 +5975,15 @@
         runoak -i foo.obo diff -X bar.obo -o diff.yaml --output-type yaml
 
     The --statistics option can be used to generate summary statistics for the changes.
     These are grouped according to the --group-by-property option. For example,
     the GO uses the oio:hasOBONamespace property to partition classes into 3 categories.
 
     Example:
-    -------
+
         runoak -i go.obo diff -X go-new.obo -o diff.yaml --statistics --group-by-property oio:hasOBONamespace
 
     This will produce a YAML dictionary, with outer keys being the values of the oio:hasOBONamespace property,
     and inner keys being the change types.
 
     If --group-by-property is not specified, or there is no value for this property, then the outer key
     will be "__RESIDUAL__"
@@ -6064,29 +6080,29 @@
     overwrite: bool,
 ):
     """
     Applies a patch to an ontology. The patch should be specified using KGCL syntax, see
     https://github.com/INCATools/kgcl
 
     Example:
-    -------
+
         runoak -i cl.owl.ttl apply "rename CL:0000561 to 'amacrine neuron'"  -o cl.owl.ttl -O ttl
 
     On an obo format file:
 
         runoak -i simpleobo:go-edit.obo apply "rename GO:0005634 from 'nucleus' to 'foo'" -o go-edit-new.obo
 
     With URIs:
 
         runoak -i cl.owl.ttl apply \
           "rename <http://purl.obolibrary.org/obo/CL_0000561> from 'amacrine cell' to 'amacrine neuron'" \
            -o cl.owl.ttl -O ttl
 
     Warning:
-    -------
+
     This command is still experimental. Some things to bear in mind:
 
     - for some ontologies, CURIEs may not work, instead specify a full URI surrounded by <>s
     - only a subset of KGCL commands are supported by each backend
 
     """
     impl = settings.impl
@@ -6158,15 +6174,15 @@
 @output_type_option
 @click.argument("terms", nargs=-1)
 def apply_obsolete(output, output_type, expand: bool, terms, **kwargs):
     """
     Sets an ontology element to be obsolete
 
     Example:
-    -------
+
         runoak -i my.obo apply-obsolete MY:0002200 -o my-modified.obo
 
     Multiple terms can be passed, as labels, IDs, or using OAK queries:
 
         runoak -i my.obo apply-obsolete MY:1 MY:2 MY:3 ... -o my-modified.obo
 
     This may be chained, for example to take all terms matching a search query and then
@@ -6213,15 +6229,15 @@
     in labels and definitions.
 
     The output is a list of changes, in a KCGL-compliant syntax.
 
     By default, changes will be applied
 
     Example:
-    -------
+
         runoak -i my.obo lint
 
     This can be executed in dry-run mode, in which case changes are not applied:
 
         runoak -i my.obo lint --dry-run
 
     One common workflow is to emit the changes to a KCGL file which is manually checked,
@@ -6302,15 +6318,15 @@
     """
     Calculates cross-ontology diff using mappings
 
     Given a pair of ontologies, and mappings that connect terms in both ontologies, this
     command will perform a structural comparison of all mapped pairs of terms
 
     Example:
-    -------
+
         runoak -i sqlite:obo:uberon diff-via-mappings --other-input sqlite:obo:zfa  --source UBERON --source ZFA -O csv
 
     Note the above command does not have any mapping file specified; the mappings that are distributed within
     each ontology is used (in this case, Uberon contains mappings to ZFA)
 
     If the mappings are provided externally:
 
@@ -6449,15 +6465,15 @@
     In some cases, this can also perform reverse lookups; i.e given a table with labels populated and blank IDs,
     then fill in the IDs
 
     In the most basic scenario, you have a table with two columns 'id' and 'label'. These are the "conventional" column
     headers for a table of ontology elements (see later for configuration when you don't follow conventions)
 
     Example:
-    -------
+
         runoak -i cl.owl.ttl fill-table my-table.tsv
 
     (any implementation can be used)
 
     The same command will work for the reverse scenario - when you have labels populated, but IDs are not populated
 
     By default this will throw an error if a lookup is not successful; this can be relaxed
@@ -6489,15 +6505,15 @@
      1. Pass in a YAML structure (on command line or in a YAML file) listing relations
      2. Pass in a LinkML data definitions YAML file
 
     For the first method, you can pass in multiple relations using the --relation arg. For example,
     given a TSV with columns cl_identifier and cl_display_label you can say:
 
     Example:
-    -------
+
         runoak -i cl.owl.ttl fill-table \
           --relation "{primary_key: cl_identifier, dependent_column: cl_display_label, relation: label}"
 
     You can also specify this in a YAML file
 
     For the 2nd method, you need to specify a LinkML schema with a class where (1) at least one field is annotated
     as being an identifier (2) one or more slots have slot_uri elements mapping them to standard metadata elements
@@ -6611,22 +6627,22 @@
     """
     Generate synonyms based on a set of synonymizer rules.
 
     If the `--apply-patch` flag is set, the output will be an ontology file with the changes
     applied. Pass the `--patch` argument to lso get the patch file in KGCL format.
 
     Example:
-    -------
+
 
         runoak -i foo.obo generate-synonyms -R foo_rules.yaml --patch patch.kgcl --apply-patch -o foo_syn.obo
 
     If the `apply-patch` flag is NOT set then the main input will be KGCL commands
 
     Example:
-    -------
+
 
         runoak -i foo.obo generate-synonyms -R foo_rules.yaml -o changes.kgcl
 
     see https://github.com/INCATools/kgcl.
 
     """
     impl = settings.impl
@@ -6689,31 +6705,31 @@
     Generate lexical replacements based on a set of synonymizer rules.
 
 
     If the `--apply-patch` flag is set, the output will be an ontology file with the changes
     applied. Pass the `--patch` argument to lso get the patch file in KGCL format.
 
     Example:
-    -------
+
 
         runoak -i foo.obo generate-lexical-replacements -R foo_rules.yaml\
            --patch patch.kgcl --apply-patch -o foo_syn.obo
 
     If the `apply-patch` flag is NOT set then the main input will be KGCL commands
 
     Example:
-    -------
+
 
         runoak -i foo.obo generate-lexical-replacements -R foo_rules.yaml -o changes.kgcl
 
 
     You can also pass the expressions directly as YAML
 
     Example:
-    -------
+
 
         runoak -i foo.obo generate-lexical-replacements \
           -Y '{match: "nuclear (\\w+)", replacement: "\\1 nucleus"}' .all
 
     see https://github.com/INCATools/kgcl.
 
     Note: this command is very similar to generate-synonyms, but the main use case here
@@ -6778,21 +6794,21 @@
 def generate_definitions(terms, apply_patch, patch, patch_format, output, output_type, **kwargs):
     """
     Generate definitions for a term or terms.
 
     Currently this only works with the llm extension.
 
     Example:
-    -------
+
         runoak -i llm:sqlite:obo:foodon generate-definitions FOODON:03315258
 
     The --style-hints option can be used to provide hints to the definition generator.
 
     Example:
-    -------
+
         runoak -i llm:sqlite:obo:foodon generate-definitions FOODON:03315258 \
           --style-hints "Write the definition in the style of a pretentious food critic"
 
     Generates:
 
         "The pancake, a humble delight in the realm of breakfast fare,
         presents itself as a delectable disc of gastronomic delight..."
@@ -6968,15 +6984,15 @@
     exclude_existing,
     min_descendants,
 ):
     """
     Generate candidate disjointness axioms.
 
     Example:
-    -------
+
         runoak -i sqlite:obo:iao generate-disjoints -O obo
 
     To generate spatial disjointness axioms:
 
         runoak -i sqlite:obo:zfa generate-disjoints -O obo p i,p
 
     """
```

### Comparing `oaklib-0.6.3/src/oaklib/conf/lexmatch-rules-oboinowl-default.yaml` & `oaklib-0.6.4/src/oaklib/conf/lexmatch-rules-oboinowl-default.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/conf/mondo-g2d-input-spec.yaml` & `oaklib-0.6.4/src/oaklib/conf/mondo-g2d-input-spec.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/conf/mondo-hpoa-g2d-input-spec.yaml` & `oaklib-0.6.4/src/oaklib/conf/mondo-hpoa-g2d-input-spec.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/conf/obograph-style.json` & `oaklib-0.6.4/src/oaklib/conf/obograph-style.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/converters/data_model_converter.py` & `oaklib-0.6.4/src/oaklib/converters/data_model_converter.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/converters/logical_definition_flattener.py` & `oaklib-0.6.4/src/oaklib/converters/logical_definition_flattener.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/converters/obo_graph_to_cx_converter.py` & `oaklib-0.6.4/src/oaklib/converters/obo_graph_to_cx_converter.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/converters/obo_graph_to_fhir_converter.py` & `oaklib-0.6.4/src/oaklib/converters/obo_graph_to_fhir_converter.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/converters/obo_graph_to_obo_format_converter.py` & `oaklib-0.6.4/src/oaklib/converters/obo_graph_to_obo_format_converter.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/converters/obo_graph_to_rdf_owl_converter.py` & `oaklib-0.6.4/src/oaklib/converters/obo_graph_to_rdf_owl_converter.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/datamodels/association.owl.ttl` & `oaklib-0.6.4/src/oaklib/datamodels/association.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/datamodels/association.py` & `oaklib-0.6.4/src/oaklib/datamodels/association.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/datamodels/association.yaml` & `oaklib-0.6.4/src/oaklib/datamodels/association.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/datamodels/class_enrichment.owl.ttl` & `oaklib-0.6.4/src/oaklib/datamodels/class_enrichment.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/datamodels/class_enrichment.py` & `oaklib-0.6.4/src/oaklib/datamodels/class_enrichment.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/datamodels/class_enrichment.yaml` & `oaklib-0.6.4/src/oaklib/datamodels/class_enrichment.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/datamodels/cross_ontology_diff.owl.ttl` & `oaklib-0.6.4/src/oaklib/datamodels/cross_ontology_diff.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/datamodels/cross_ontology_diff.py` & `oaklib-0.6.4/src/oaklib/datamodels/cross_ontology_diff.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/datamodels/cross_ontology_diff.yaml` & `oaklib-0.6.4/src/oaklib/datamodels/cross_ontology_diff.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/datamodels/cx.py` & `oaklib-0.6.4/src/oaklib/datamodels/cx.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/datamodels/cx.yaml` & `oaklib-0.6.4/src/oaklib/datamodels/cx.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/datamodels/fhir.owl.ttl` & `oaklib-0.6.4/src/oaklib/datamodels/fhir.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/datamodels/fhir.py` & `oaklib-0.6.4/src/oaklib/datamodels/fhir.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/datamodels/fhir.yaml` & `oaklib-0.6.4/src/oaklib/datamodels/fhir.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/datamodels/input_specification.py` & `oaklib-0.6.4/src/oaklib/datamodels/input_specification.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/datamodels/input_specification.yaml` & `oaklib-0.6.4/src/oaklib/datamodels/input_specification.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/datamodels/item_list.py` & `oaklib-0.6.4/src/oaklib/datamodels/item_list.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/datamodels/item_list.yaml` & `oaklib-0.6.4/src/oaklib/datamodels/item_list.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/datamodels/lexical_index.owl.ttl` & `oaklib-0.6.4/src/oaklib/datamodels/lexical_index.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/datamodels/lexical_index.py` & `oaklib-0.6.4/src/oaklib/datamodels/lexical_index.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/datamodels/lexical_index.schema.json` & `oaklib-0.6.4/src/oaklib/datamodels/lexical_index.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/datamodels/lexical_index.yaml` & `oaklib-0.6.4/src/oaklib/datamodels/lexical_index.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/datamodels/mapping_cluster_datamodel.py` & `oaklib-0.6.4/src/oaklib/datamodels/mapping_cluster_datamodel.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/datamodels/mapping_cluster_datamodel.yaml` & `oaklib-0.6.4/src/oaklib/datamodels/mapping_cluster_datamodel.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/datamodels/mapping_rules_datamodel.owl.ttl` & `oaklib-0.6.4/src/oaklib/datamodels/mapping_rules_datamodel.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/datamodels/mapping_rules_datamodel.py` & `oaklib-0.6.4/src/oaklib/datamodels/mapping_rules_datamodel.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/datamodels/mapping_rules_datamodel.schema.json` & `oaklib-0.6.4/src/oaklib/datamodels/mapping_rules_datamodel.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/datamodels/mapping_rules_datamodel.yaml` & `oaklib-0.6.4/src/oaklib/datamodels/mapping_rules_datamodel.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/datamodels/obograph.owl.ttl` & `oaklib-0.6.4/src/oaklib/datamodels/obograph.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/datamodels/obograph.py` & `oaklib-0.6.4/src/oaklib/datamodels/obograph.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/datamodels/obograph.schema.json` & `oaklib-0.6.4/src/oaklib/datamodels/obograph.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/datamodels/obograph.yaml` & `oaklib-0.6.4/src/oaklib/datamodels/obograph.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/datamodels/ontology_metadata.owl.ttl` & `oaklib-0.6.4/src/oaklib/datamodels/ontology_metadata.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/datamodels/ontology_metadata.py` & `oaklib-0.6.4/src/oaklib/datamodels/ontology_metadata.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/datamodels/ontology_metadata.schema.json` & `oaklib-0.6.4/src/oaklib/datamodels/ontology_metadata.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/datamodels/ontology_metadata.yaml` & `oaklib-0.6.4/src/oaklib/datamodels/ontology_metadata.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/datamodels/oxo.owl.ttl` & `oaklib-0.6.4/src/oaklib/datamodels/oxo.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/datamodels/oxo.py` & `oaklib-0.6.4/src/oaklib/datamodels/oxo.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/datamodels/oxo.yaml` & `oaklib-0.6.4/src/oaklib/datamodels/oxo.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/datamodels/search.py` & `oaklib-0.6.4/src/oaklib/datamodels/search.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/datamodels/search_datamodel.owl.ttl` & `oaklib-0.6.4/src/oaklib/datamodels/search_datamodel.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/datamodels/search_datamodel.py` & `oaklib-0.6.4/src/oaklib/datamodels/search_datamodel.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/datamodels/search_datamodel.yaml` & `oaklib-0.6.4/src/oaklib/datamodels/search_datamodel.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/datamodels/similarity.owl.ttl` & `oaklib-0.6.4/src/oaklib/datamodels/similarity.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/datamodels/similarity.py` & `oaklib-0.6.4/src/oaklib/datamodels/similarity.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/datamodels/similarity.yaml` & `oaklib-0.6.4/src/oaklib/datamodels/similarity.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/datamodels/summary_statistics_datamodel.owl.ttl` & `oaklib-0.6.4/src/oaklib/datamodels/summary_statistics_datamodel.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/datamodels/summary_statistics_datamodel.py` & `oaklib-0.6.4/src/oaklib/datamodels/summary_statistics_datamodel.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/datamodels/summary_statistics_datamodel.schema.json` & `oaklib-0.6.4/src/oaklib/datamodels/summary_statistics_datamodel.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/datamodels/summary_statistics_datamodel.yaml` & `oaklib-0.6.4/src/oaklib/datamodels/summary_statistics_datamodel.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/datamodels/synonymizer_datamodel.py` & `oaklib-0.6.4/src/oaklib/datamodels/synonymizer_datamodel.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/datamodels/synonymizer_datamodel.yaml` & `oaklib-0.6.4/src/oaklib/datamodels/synonymizer_datamodel.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/datamodels/taxon_constraints.owl.ttl` & `oaklib-0.6.4/src/oaklib/datamodels/taxon_constraints.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/datamodels/taxon_constraints.py` & `oaklib-0.6.4/src/oaklib/datamodels/taxon_constraints.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/datamodels/taxon_constraints.yaml` & `oaklib-0.6.4/src/oaklib/datamodels/taxon_constraints.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/datamodels/text_annotator.owl.ttl` & `oaklib-0.6.4/src/oaklib/datamodels/text_annotator.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/datamodels/text_annotator.py` & `oaklib-0.6.4/src/oaklib/datamodels/text_annotator.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/datamodels/text_annotator.schema.json` & `oaklib-0.6.4/src/oaklib/datamodels/text_annotator.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/datamodels/text_annotator.yaml` & `oaklib-0.6.4/src/oaklib/datamodels/text_annotator.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/datamodels/validation_datamodel.owl.ttl` & `oaklib-0.6.4/src/oaklib/datamodels/validation_datamodel.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/datamodels/validation_datamodel.py` & `oaklib-0.6.4/src/oaklib/datamodels/validation_datamodel.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/datamodels/validation_datamodel.schema.json` & `oaklib-0.6.4/src/oaklib/datamodels/validation_datamodel.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/datamodels/validation_datamodel.yaml` & `oaklib-0.6.4/src/oaklib/datamodels/validation_datamodel.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/datamodels/value_set_configuration.owl.ttl` & `oaklib-0.6.4/src/oaklib/datamodels/value_set_configuration.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/datamodels/value_set_configuration.py` & `oaklib-0.6.4/src/oaklib/datamodels/value_set_configuration.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/datamodels/value_set_configuration.yaml` & `oaklib-0.6.4/src/oaklib/datamodels/value_set_configuration.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/datamodels/vocabulary.py` & `oaklib-0.6.4/src/oaklib/datamodels/vocabulary.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/implementations/__init__.py` & `oaklib-0.6.4/src/oaklib/implementations/__init__.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/implementations/aggregator/aggregator_implementation.py` & `oaklib-0.6.4/src/oaklib/implementations/aggregator/aggregator_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/implementations/agrkb/agrkb_implementation.py` & `oaklib-0.6.4/src/oaklib/implementations/agrkb/agrkb_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/implementations/amigo/amigo_implementation.py` & `oaklib-0.6.4/src/oaklib/implementations/amigo/amigo_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/implementations/cx/cx_implementation.py` & `oaklib-0.6.4/src/oaklib/implementations/cx/cx_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/implementations/eutils/eutils_implementation.py` & `oaklib-0.6.4/src/oaklib/implementations/eutils/eutils_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/implementations/eutils/pubmed_implementation.py` & `oaklib-0.6.4/src/oaklib/implementations/eutils/pubmed_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/implementations/funowl/funowl_implementation.py` & `oaklib-0.6.4/src/oaklib/implementations/funowl/funowl_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/implementations/gilda.py` & `oaklib-0.6.4/src/oaklib/implementations/gilda.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/implementations/kgx/kgx_implementation.py` & `oaklib-0.6.4/src/oaklib/implementations/kgx/kgx_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/implementations/llm_implementation.py` & `oaklib-0.6.4/src/oaklib/implementations/llm_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/implementations/monarch/monarch_implementation.py` & `oaklib-0.6.4/src/oaklib/implementations/monarch/monarch_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/implementations/ncbi/ncbi_gene_implementation.py` & `oaklib-0.6.4/src/oaklib/implementations/ncbi/ncbi_gene_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/implementations/obograph/obograph_implementation.py` & `oaklib-0.6.4/src/oaklib/implementations/obograph/obograph_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/implementations/ols/ols_implementation.py` & `oaklib-0.6.4/src/oaklib/implementations/ols/ols_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/implementations/ols/oxo_utils.py` & `oaklib-0.6.4/src/oaklib/implementations/ols/oxo_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/implementations/ontobee/ontobee_implementation.py` & `oaklib-0.6.4/src/oaklib/implementations/ontobee/ontobee_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/implementations/ontoportal/bioportal_implementation.py` & `oaklib-0.6.4/src/oaklib/implementations/ontoportal/bioportal_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/implementations/ontoportal/ontoportal_implementation_base.py` & `oaklib-0.6.4/src/oaklib/implementations/ontoportal/ontoportal_implementation_base.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/implementations/pantherdb/pantherdb_implementation.py` & `oaklib-0.6.4/src/oaklib/implementations/pantherdb/pantherdb_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/implementations/pronto/pronto_implementation.py` & `oaklib-0.6.4/src/oaklib/implementations/pronto/pronto_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/implementations/semsimian/semsimian_implementation.py` & `oaklib-0.6.4/src/oaklib/implementations/semsimian/semsimian_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/implementations/simpleobo/simple_obo_implementation.py` & `oaklib-0.6.4/src/oaklib/implementations/simpleobo/simple_obo_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/implementations/simpleobo/simple_obo_parser.py` & `oaklib-0.6.4/src/oaklib/implementations/simpleobo/simple_obo_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/implementations/sparql/abstract_sparql_implementation.py` & `oaklib-0.6.4/src/oaklib/implementations/sparql/abstract_sparql_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/implementations/sparql/lov_implementation.py` & `oaklib-0.6.4/src/oaklib/implementations/sparql/lov_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/implementations/sparql/oak_metamodel_implementation.py` & `oaklib-0.6.4/src/oaklib/implementations/sparql/oak_metamodel_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/implementations/sparql/sparql_implementation.py` & `oaklib-0.6.4/src/oaklib/implementations/sparql/sparql_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/implementations/sparql/sparql_query.py` & `oaklib-0.6.4/src/oaklib/implementations/sparql/sparql_query.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/implementations/sqldb/sql_implementation.py` & `oaklib-0.6.4/src/oaklib/implementations/sqldb/sql_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/implementations/sqldb/sqlite_utils.py` & `oaklib-0.6.4/src/oaklib/implementations/sqldb/sqlite_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/implementations/tabular/robot_template_implementation.py` & `oaklib-0.6.4/src/oaklib/implementations/tabular/robot_template_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/implementations/tabular/tabular_implementation.py` & `oaklib-0.6.4/src/oaklib/implementations/tabular/tabular_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/implementations/translator/translator_implementation.py` & `oaklib-0.6.4/src/oaklib/implementations/translator/translator_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/implementations/ubergraph/ubergraph_implementation.py` & `oaklib-0.6.4/src/oaklib/implementations/ubergraph/ubergraph_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/implementations/uniprot/uniprot_implementation.py` & `oaklib-0.6.4/src/oaklib/implementations/uniprot/uniprot_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/implementations/wikidata/wikidata_implementation.py` & `oaklib-0.6.4/src/oaklib/implementations/wikidata/wikidata_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/indexes/edge_index.py` & `oaklib-0.6.4/src/oaklib/indexes/edge_index.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/inference/owl_reasoner.py` & `oaklib-0.6.4/src/oaklib/inference/owl_reasoner.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/inference/relation_graph_reasoner.py` & `oaklib-0.6.4/src/oaklib/inference/relation_graph_reasoner.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/interfaces/__init__.py` & `oaklib-0.6.4/src/oaklib/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/interfaces/association_provider_interface.py` & `oaklib-0.6.4/src/oaklib/interfaces/association_provider_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/interfaces/basic_ontology_interface.py` & `oaklib-0.6.4/src/oaklib/interfaces/basic_ontology_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/interfaces/class_enrichment_calculation_interface.py` & `oaklib-0.6.4/src/oaklib/interfaces/class_enrichment_calculation_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/interfaces/differ_interface.py` & `oaklib-0.6.4/src/oaklib/interfaces/differ_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/interfaces/dumper_interface.py` & `oaklib-0.6.4/src/oaklib/interfaces/dumper_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/interfaces/embedding_provider_interface.py` & `oaklib-0.6.4/src/oaklib/interfaces/embedding_provider_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/interfaces/mapping_provider_interface.py` & `oaklib-0.6.4/src/oaklib/interfaces/mapping_provider_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/interfaces/merge_interface.py` & `oaklib-0.6.4/src/oaklib/interfaces/merge_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/interfaces/metadata_interface.py` & `oaklib-0.6.4/src/oaklib/interfaces/metadata_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/interfaces/obograph_interface.py` & `oaklib-0.6.4/src/oaklib/interfaces/obograph_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -255,14 +255,46 @@
             if key in self.transitive_query_cache:
                 return self.transitive_query_cache[key]
         g = self._graph(walk_down(self, start_curies, predicates=predicates))
         if self.transitive_query_cache is not None:
             self.transitive_query_cache[key] = g
         return g
 
+    def non_redundant_entailed_relationships(
+        self,
+        predicates: List[PRED_CURIE] = None,
+        **kwargs,
+    ) -> Iterator[RELATIONSHIP]:
+        """
+        Yields all relationships that are directly entailed.
+
+        See https://github.com/INCATools/ontology-access-kit/issues/739
+
+        :param kwargs: same as relationships
+        :return:
+        """
+        if "include_entailed" in kwargs:
+            kwargs.pop("include_entailed")
+        relationships = list(
+            self.relationships(predicates=predicates, include_entailed=True, **kwargs)
+        )
+        rel_by_sp = defaultdict(list)
+        for s, p, o in relationships:
+            if s == o:
+                continue
+            rel_by_sp[(s, p)].append(o)
+        for (s, p), objs in rel_by_sp.items():
+            redundant_set = set()
+            for o in objs:
+                ancs = list(self.ancestors(o, predicates=predicates, reflexive=False))
+                redundant_set.update(ancs)
+            for o in objs:
+                if o not in redundant_set:
+                    yield s, p, o
+
     def ancestors(
         self,
         start_curies: Union[CURIE, List[CURIE]],
         predicates: List[PRED_CURIE] = None,
         reflexive=True,
         method: Optional[GraphTraversalMethod] = None,
     ) -> Iterable[CURIE]:
```

### Comparing `oaklib-0.6.3/src/oaklib/interfaces/obolegacy_interface.py` & `oaklib-0.6.4/src/oaklib/interfaces/obolegacy_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/interfaces/ontology_generator_interface.py` & `oaklib-0.6.4/src/oaklib/interfaces/ontology_generator_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/interfaces/ontology_interface.py` & `oaklib-0.6.4/src/oaklib/interfaces/ontology_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/interfaces/owl_interface.py` & `oaklib-0.6.4/src/oaklib/interfaces/owl_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/interfaces/patcher_interface.py` & `oaklib-0.6.4/src/oaklib/interfaces/patcher_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/interfaces/rdf_interface.py` & `oaklib-0.6.4/src/oaklib/interfaces/rdf_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/interfaces/relation_graph_interface.py` & `oaklib-0.6.4/src/oaklib/interfaces/relation_graph_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/interfaces/search_interface.py` & `oaklib-0.6.4/src/oaklib/interfaces/search_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/interfaces/semsim_interface.py` & `oaklib-0.6.4/src/oaklib/interfaces/semsim_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/interfaces/skos_interface.py` & `oaklib-0.6.4/src/oaklib/interfaces/skos_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/interfaces/subsetter_interface.py` & `oaklib-0.6.4/src/oaklib/interfaces/subsetter_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/interfaces/summary_statistics_interface.py` & `oaklib-0.6.4/src/oaklib/interfaces/summary_statistics_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/interfaces/taxon_constraint_interface.py` & `oaklib-0.6.4/src/oaklib/interfaces/taxon_constraint_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/interfaces/text_annotator_interface.py` & `oaklib-0.6.4/src/oaklib/interfaces/text_annotator_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/interfaces/validator_interface.py` & `oaklib-0.6.4/src/oaklib/interfaces/validator_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/io/heatmap_writer.py` & `oaklib-0.6.4/src/oaklib/io/heatmap_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/io/html_writer.py` & `oaklib-0.6.4/src/oaklib/io/html_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/io/obograph_writer.py` & `oaklib-0.6.4/src/oaklib/io/obograph_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/io/rollup_report_writer.py` & `oaklib-0.6.4/src/oaklib/io/rollup_report_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/io/streaming_axiom_writer.py` & `oaklib-0.6.4/src/oaklib/io/streaming_axiom_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/io/streaming_csv_writer.py` & `oaklib-0.6.4/src/oaklib/io/streaming_csv_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/io/streaming_fhir_writer.py` & `oaklib-0.6.4/src/oaklib/io/streaming_fhir_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/io/streaming_info_writer.py` & `oaklib-0.6.4/src/oaklib/io/streaming_info_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/io/streaming_json_lines_writer.py` & `oaklib-0.6.4/src/oaklib/io/streaming_json_lines_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/io/streaming_json_writer.py` & `oaklib-0.6.4/src/oaklib/io/streaming_json_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/io/streaming_kgcl_writer.py` & `oaklib-0.6.4/src/oaklib/io/streaming_kgcl_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/io/streaming_markdown_writer.py` & `oaklib-0.6.4/src/oaklib/io/streaming_markdown_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/io/streaming_nl_writer.py` & `oaklib-0.6.4/src/oaklib/io/streaming_nl_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/io/streaming_obo_json_writer.py` & `oaklib-0.6.4/src/oaklib/io/streaming_obo_json_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/io/streaming_obo_writer.py` & `oaklib-0.6.4/src/oaklib/io/streaming_obo_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/io/streaming_owl_functional_writer.py` & `oaklib-0.6.4/src/oaklib/io/streaming_owl_functional_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/io/streaming_rdf_writer.py` & `oaklib-0.6.4/src/oaklib/io/streaming_rdf_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/io/streaming_writer.py` & `oaklib-0.6.4/src/oaklib/io/streaming_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/io/streaming_yaml_writer.py` & `oaklib-0.6.4/src/oaklib/io/streaming_yaml_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/mappers/base_mapper.py` & `oaklib-0.6.4/src/oaklib/mappers/base_mapper.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/mappers/ontology_metadata_mapper.py` & `oaklib-0.6.4/src/oaklib/mappers/ontology_metadata_mapper.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/parsers/__init__.py` & `oaklib-0.6.4/src/oaklib/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/parsers/association_parser.py` & `oaklib-0.6.4/src/oaklib/parsers/association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/parsers/association_parser_factory.py` & `oaklib-0.6.4/src/oaklib/parsers/association_parser_factory.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/parsers/boomer_parser.py` & `oaklib-0.6.4/src/oaklib/parsers/boomer_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/parsers/gaf_association_parser.py` & `oaklib-0.6.4/src/oaklib/parsers/gaf_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/parsers/gencc_association_parser.py` & `oaklib-0.6.4/src/oaklib/parsers/gencc_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/parsers/hpoa_association_parser.py` & `oaklib-0.6.4/src/oaklib/parsers/hpoa_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/parsers/hpoa_g2d_association_parser.py` & `oaklib-0.6.4/src/oaklib/parsers/hpoa_g2d_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/parsers/hpoa_g2p_association_parser.py` & `oaklib-0.6.4/src/oaklib/parsers/hpoa_g2p_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/parsers/kgx_association_parser.py` & `oaklib-0.6.4/src/oaklib/parsers/kgx_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/parsers/mim2gene_association_parser.py` & `oaklib-0.6.4/src/oaklib/parsers/mim2gene_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/parsers/pairwise_association_parser.py` & `oaklib-0.6.4/src/oaklib/parsers/pairwise_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/parsers/parser_base.py` & `oaklib-0.6.4/src/oaklib/parsers/parser_base.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/parsers/phaf_association_parser.py` & `oaklib-0.6.4/src/oaklib/parsers/phaf_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/parsers/xaf_association_parser.py` & `oaklib-0.6.4/src/oaklib/parsers/xaf_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/resource.py` & `oaklib-0.6.4/src/oaklib/resource.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/selector.py` & `oaklib-0.6.4/src/oaklib/selector.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/transformers/chained_ontology_transformer.py` & `oaklib-0.6.4/src/oaklib/transformers/chained_ontology_transformer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/transformers/edge_filter_transformer.py` & `oaklib-0.6.4/src/oaklib/transformers/edge_filter_transformer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/transformers/graph_transformer.py` & `oaklib-0.6.4/src/oaklib/transformers/graph_transformer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/transformers/node_filter_transformer.py` & `oaklib-0.6.4/src/oaklib/transformers/node_filter_transformer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/transformers/sep_transformer.py` & `oaklib-0.6.4/src/oaklib/transformers/sep_transformer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/transformers/transformers_factory.py` & `oaklib-0.6.4/src/oaklib/transformers/transformers_factory.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/utilities/apikey_manager.py` & `oaklib-0.6.4/src/oaklib/utilities/apikey_manager.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/utilities/associations/association_differ.py` & `oaklib-0.6.4/src/oaklib/utilities/associations/association_differ.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/utilities/associations/association_index.py` & `oaklib-0.6.4/src/oaklib/utilities/associations/association_index.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/utilities/axioms/disjointness_axiom_analyzer.py` & `oaklib-0.6.4/src/oaklib/utilities/axioms/disjointness_axiom_analyzer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/utilities/axioms/logical_definition_analyzer.py` & `oaklib-0.6.4/src/oaklib/utilities/axioms/logical_definition_analyzer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/utilities/axioms/logical_definition_summarizer.py` & `oaklib-0.6.4/src/oaklib/utilities/axioms/logical_definition_summarizer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/utilities/axioms/logical_definition_utilities.py` & `oaklib-0.6.4/src/oaklib/utilities/axioms/logical_definition_utilities.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/utilities/basic_utils.py` & `oaklib-0.6.4/src/oaklib/utilities/basic_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/utilities/format_utilities.py` & `oaklib-0.6.4/src/oaklib/utilities/format_utilities.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/utilities/graph/networkx_bridge.py` & `oaklib-0.6.4/src/oaklib/utilities/graph/networkx_bridge.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/utilities/graph/relationship_walker.py` & `oaklib-0.6.4/src/oaklib/utilities/graph/relationship_walker.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/utilities/identifier_utils.py` & `oaklib-0.6.4/src/oaklib/utilities/identifier_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/utilities/iterator_utils.py` & `oaklib-0.6.4/src/oaklib/utilities/iterator_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/utilities/keyval_cache.py` & `oaklib-0.6.4/src/oaklib/utilities/keyval_cache.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/utilities/kgcl_utilities.py` & `oaklib-0.6.4/src/oaklib/utilities/kgcl_utilities.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/utilities/label_utilities.py` & `oaklib-0.6.4/src/oaklib/utilities/label_utilities.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/utilities/lexical/lexical_indexer.py` & `oaklib-0.6.4/src/oaklib/utilities/lexical/lexical_indexer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/utilities/lexical/patternizer.py` & `oaklib-0.6.4/src/oaklib/utilities/lexical/patternizer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/utilities/lexical/synonymizer.py` & `oaklib-0.6.4/src/oaklib/utilities/lexical/synonymizer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/utilities/mapping/boomer_utils.py` & `oaklib-0.6.4/src/oaklib/utilities/mapping/boomer_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/utilities/mapping/cross_ontology_diffs.py` & `oaklib-0.6.4/src/oaklib/utilities/mapping/cross_ontology_diffs.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/utilities/mapping/mapping_propagator.py` & `oaklib-0.6.4/src/oaklib/utilities/mapping/mapping_propagator.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/utilities/mapping/mapping_validation.py` & `oaklib-0.6.4/src/oaklib/utilities/mapping/mapping_validation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/utilities/mapping/sssom_utils.py` & `oaklib-0.6.4/src/oaklib/utilities/mapping/sssom_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/utilities/ner_utilities.py` & `oaklib-0.6.4/src/oaklib/utilities/ner_utilities.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/utilities/nlp/natual_language_generation.py` & `oaklib-0.6.4/src/oaklib/utilities/nlp/natual_language_generation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/utilities/obograph_utils.py` & `oaklib-0.6.4/src/oaklib/utilities/obograph_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/utilities/ontology_builder.py` & `oaklib-0.6.4/src/oaklib/utilities/ontology_builder.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/utilities/publication_utils/doi_wrapper.py` & `oaklib-0.6.4/src/oaklib/utilities/publication_utils/doi_wrapper.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/utilities/publication_utils/pubdb_wrapper.py` & `oaklib-0.6.4/src/oaklib/utilities/publication_utils/pubdb_wrapper.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/utilities/publication_utils/pubmed_wrapper.py` & `oaklib-0.6.4/src/oaklib/utilities/publication_utils/pubmed_wrapper.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/utilities/reasoning/relation_graph.py` & `oaklib-0.6.4/src/oaklib/utilities/reasoning/relation_graph.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/utilities/semsim/similarity_utils.py` & `oaklib-0.6.4/src/oaklib/utilities/semsim/similarity_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/utilities/stats/hypergeometric.py` & `oaklib-0.6.4/src/oaklib/utilities/stats/hypergeometric.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/utilities/subsets/slimmer_utils.py` & `oaklib-0.6.4/src/oaklib/utilities/subsets/slimmer_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/utilities/subsets/subset_analysis.py` & `oaklib-0.6.4/src/oaklib/utilities/subsets/subset_analysis.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/utilities/subsets/value_set_expander.py` & `oaklib-0.6.4/src/oaklib/utilities/subsets/value_set_expander.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/utilities/table_filler.py` & `oaklib-0.6.4/src/oaklib/utilities/table_filler.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/utilities/taxon/taxon_constraint_utils.py` & `oaklib-0.6.4/src/oaklib/utilities/taxon/taxon_constraint_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/utilities/validation/definition_ontology_rule.py` & `oaklib-0.6.4/src/oaklib/utilities/validation/definition_ontology_rule.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/utilities/validation/disjointness_rule.py` & `oaklib-0.6.4/src/oaklib/utilities/validation/disjointness_rule.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/utilities/validation/lint_utils.py` & `oaklib-0.6.4/src/oaklib/utilities/validation/lint_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/utilities/validation/ontology_rule.py` & `oaklib-0.6.4/src/oaklib/utilities/validation/ontology_rule.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/utilities/validation/rule_runner.py` & `oaklib-0.6.4/src/oaklib/utilities/validation/rule_runner.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/src/oaklib/utilities/writers/change_handler.py` & `oaklib-0.6.4/src/oaklib/utilities/writers/change_handler.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.3/PKG-INFO` & `oaklib-0.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oaklib
-Version: 0.6.3
+Version: 0.6.4
 Summary: Ontology Access Kit: Python library for common ontology operations over a variety of backends
 Author: cmungall
 Author-email: cjm@berkeleybop.org
 Requires-Python: >=3.9,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

