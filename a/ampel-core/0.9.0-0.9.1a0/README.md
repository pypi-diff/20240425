# Comparing `tmp/ampel_core-0.9.0.tar.gz` & `tmp/ampel_core-0.9.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ampel_core-0.9.0.tar", max compression
+gzip compressed data, was "ampel_core-0.9.1a0.tar", max compression
```

## Comparing `ampel_core-0.9.0.tar` & `ampel_core-0.9.1a0.tar`

### file list

```diff
@@ -1,278 +1,280 @@
--rw-r--r--   0        0        0     1512 2023-04-06 19:53:42.029189 ampel_core-0.9.0/LICENSE
--rw-r--r--   0        0        0      262 2023-04-06 19:53:42.029189 ampel_core-0.9.0/README.md
--rwxr-xr-x   0        0        0     1251 2023-04-06 19:53:42.029189 ampel_core-0.9.0/ampel/abstract/AbsBufferComplement.py
--rw-r--r--   0        0        0     1551 2023-04-06 19:53:42.029189 ampel_core-0.9.0/ampel/abstract/AbsChannelTemplate.py
--rwxr-xr-x   0        0        0     6900 2023-04-06 19:53:42.029189 ampel_core-0.9.0/ampel/abstract/AbsCompiler.py
--rw-r--r--   0        0        0      853 2023-04-06 19:53:42.029189 ampel_core-0.9.0/ampel/abstract/AbsConfigMorpher.py
--rw-r--r--   0        0        0     1004 2023-04-06 19:53:42.029189 ampel_core-0.9.0/ampel/abstract/AbsConfigUpdater.py
--rwxr-xr-x   0        0        0      871 2023-04-06 19:53:42.029189 ampel_core-0.9.0/ampel/abstract/AbsDocIngester.py
--rwxr-xr-x   0        0        0      886 2023-04-06 19:53:42.029189 ampel_core-0.9.0/ampel/abstract/AbsDocUpdater.py
--rw-r--r--   0        0        0     4524 2023-04-06 19:53:42.029189 ampel_core-0.9.0/ampel/abstract/AbsEventUnit.py
--rw-r--r--   0        0        0     1112 2023-04-06 19:53:42.029189 ampel_core-0.9.0/ampel/abstract/AbsOpsUnit.py
--rwxr-xr-x   0        0        0     2719 2023-04-06 19:53:42.029189 ampel_core-0.9.0/ampel/abstract/AbsProcessController.py
--rwxr-xr-x   0        0        0     2334 2023-04-06 19:53:42.029189 ampel_core-0.9.0/ampel/abstract/AbsT0Muxer.py
--rwxr-xr-x   0        0        0      743 2023-04-06 19:53:42.029189 ampel_core-0.9.0/ampel/abstract/AbsT3Filter.py
--rwxr-xr-x   0        0        0     2502 2023-04-06 19:53:42.029189 ampel_core-0.9.0/ampel/abstract/AbsT3Loader.py
--rwxr-xr-x   0        0        0      767 2023-04-06 19:53:42.029189 ampel_core-0.9.0/ampel/abstract/AbsT3Projector.py
--rwxr-xr-x   0        0        0      777 2023-04-06 19:53:42.029189 ampel_core-0.9.0/ampel/abstract/AbsT3Selector.py
--rwxr-xr-x   0        0        0     1239 2023-04-06 19:53:42.029189 ampel_core-0.9.0/ampel/abstract/AbsT3Stager.py
--rwxr-xr-x   0        0        0      939 2023-04-06 19:53:42.029189 ampel_core-0.9.0/ampel/abstract/AbsT3Supplier.py
--rwxr-xr-x   0        0        0      979 2023-04-06 19:53:42.029189 ampel_core-0.9.0/ampel/abstract/AbsT4ControlUnit.py
--rw-r--r--   0        0        0      593 2023-04-06 19:53:42.029189 ampel_core-0.9.0/ampel/abstract/AbsTargetSource.py
--rwxr-xr-x   0        0        0      700 2023-04-06 19:53:42.029189 ampel_core-0.9.0/ampel/abstract/AbsUnitResultAdapter.py
--rwxr-xr-x   0        0        0    13587 2023-04-06 19:53:42.029189 ampel_core-0.9.0/ampel/abstract/AbsWorker.py
--rw-r--r--   0        0        0      282 2023-04-06 19:53:42.029189 ampel_core-0.9.0/ampel/abstract/README.md
--rwxr-xr-x   0        0        0    11114 2023-04-06 19:53:42.029189 ampel_core-0.9.0/ampel/aux/ComboDictModifier.py
--rw-r--r--   0        0        0     1248 2023-04-06 19:53:42.029189 ampel_core-0.9.0/ampel/aux/SimpleTagFilter.py
--rwxr-xr-x   0        0        0     1575 2023-04-06 19:53:42.029189 ampel_core-0.9.0/ampel/aux/filter/AbsLogicOperatorFilter.py
--rw-r--r--   0        0        0     1192 2023-04-06 19:53:42.029189 ampel_core-0.9.0/ampel/aux/filter/FlatDictArrayFilter.py
--rw-r--r--   0        0        0     1116 2023-04-06 19:53:42.029189 ampel_core-0.9.0/ampel/aux/filter/PrimitiveTypeArrayFilter.py
--rw-r--r--   0        0        0     1768 2023-04-06 19:53:42.029189 ampel_core-0.9.0/ampel/aux/filter/SimpleDictArrayFilter.py
--rw-r--r--   0        0        0     4243 2023-04-06 19:53:42.029189 ampel_core-0.9.0/ampel/cli/AbsCoreCommand.py
--rw-r--r--   0        0        0     2134 2023-04-06 19:53:42.029189 ampel_core-0.9.0/ampel/cli/AbsLoadCommand.py
--rwxr-xr-x   0        0        0     6032 2023-04-06 19:53:42.029189 ampel_core-0.9.0/ampel/cli/AbsStockCommand.py
--rw-r--r--   0        0        0     4200 2023-04-06 19:53:42.029189 ampel_core-0.9.0/ampel/cli/BufferCommand.py
--rw-r--r--   0        0        0    11533 2023-04-06 19:53:42.029189 ampel_core-0.9.0/ampel/cli/ConfigCommand.py
--rw-r--r--   0        0        0     4955 2023-04-06 19:53:42.029189 ampel_core-0.9.0/ampel/cli/DBCommand.py
--rw-r--r--   0        0        0     5939 2023-04-06 19:53:42.029189 ampel_core-0.9.0/ampel/cli/EventCommand.py
--rw-r--r--   0        0        0    23434 2023-04-06 19:53:42.029189 ampel_core-0.9.0/ampel/cli/JobCommand.py
--rw-r--r--   0        0        0     8842 2023-04-06 19:53:42.029189 ampel_core-0.9.0/ampel/cli/LogCommand.py
--rw-r--r--   0        0        0     5808 2023-04-06 19:53:42.029189 ampel_core-0.9.0/ampel/cli/ProcessCommand.py
--rw-r--r--   0        0        0     3321 2023-04-06 19:53:42.029189 ampel_core-0.9.0/ampel/cli/RunCommand.py
--rw-r--r--   0        0        0     6326 2023-04-06 19:53:42.029189 ampel_core-0.9.0/ampel/cli/StartCommand.py
--rw-r--r--   0        0        0     9315 2023-04-06 19:53:42.029189 ampel_core-0.9.0/ampel/cli/T2Command.py
--rw-r--r--   0        0        0     2170 2023-04-06 19:53:42.029189 ampel_core-0.9.0/ampel/cli/T3BufferExporterStager.py
--rw-r--r--   0        0        0     1870 2023-04-06 19:53:42.029189 ampel_core-0.9.0/ampel/cli/T3BufferExporterUnit.py
--rw-r--r--   0        0        0     4388 2023-04-06 19:53:42.029189 ampel_core-0.9.0/ampel/cli/ViewCommand.py
--rw-r--r--   0        0        0     4434 2023-04-06 19:53:42.029189 ampel_core-0.9.0/ampel/cli/export.py
--rw-r--r--   0        0        0     3362 2023-04-06 19:53:42.029189 ampel_core-0.9.0/ampel/cli/utils.py
--rwxr-xr-x   0        0        0     1301 2023-04-06 19:53:42.029189 ampel_core-0.9.0/ampel/config/ScheduleEvaluator.py
--rw-r--r--   0        0        0     1604 2023-04-06 19:53:42.029189 ampel_core-0.9.0/ampel/config/alter/HashT2Config.py
--rw-r--r--   0        0        0     1605 2023-04-06 19:53:42.029189 ampel_core-0.9.0/ampel/config/alter/ResolveRunTimeAliases.py
--rw-r--r--   0        0        0     1746 2023-04-06 19:53:42.029189 ampel_core-0.9.0/ampel/config/builder/BaseConfigChecker.py
--rwxr-xr-x   0        0        0    20019 2023-04-06 19:53:42.029189 ampel_core-0.9.0/ampel/config/builder/ConfigBuilder.py
--rw-r--r--   0        0        0     7539 2023-04-06 19:53:42.029189 ampel_core-0.9.0/ampel/config/builder/ConfigChecker.py
--rw-r--r--   0        0        0     1671 2023-04-06 19:53:42.029189 ampel_core-0.9.0/ampel/config/builder/ConfigValidator.py
--rwxr-xr-x   0        0        0      570 2023-04-06 19:53:42.029189 ampel_core-0.9.0/ampel/config/builder/DisplayOptions.py
--rwxr-xr-x   0        0        0     8493 2023-04-06 19:53:42.029189 ampel_core-0.9.0/ampel/config/builder/DistConfigBuilder.py
--rwxr-xr-x   0        0        0     3669 2023-04-06 19:53:42.029189 ampel_core-0.9.0/ampel/config/builder/FirstPassConfig.py
--rwxr-xr-x   0        0        0     8969 2023-04-06 19:53:42.029189 ampel_core-0.9.0/ampel/config/builder/ProcessMorpher.py
--rw-r--r--   0        0        0     1000 2023-04-06 19:53:42.029189 ampel_core-0.9.0/ampel/config/builder/get_env.py
--rwxr-xr-x   0        0        0     1511 2023-04-06 19:53:42.029189 ampel_core-0.9.0/ampel/config/collector/AbsDictConfigCollector.py
--rwxr-xr-x   0        0        0     2560 2023-04-06 19:53:42.029189 ampel_core-0.9.0/ampel/config/collector/AbsForwardConfigCollector.py
--rwxr-xr-x   0        0        0      770 2023-04-06 19:53:42.029189 ampel_core-0.9.0/ampel/config/collector/AbsListConfigCollector.py
--rwxr-xr-x   0        0        0     1985 2023-04-06 19:53:42.029189 ampel_core-0.9.0/ampel/config/collector/AliasConfigCollector.py
--rwxr-xr-x   0        0        0     1826 2023-04-06 19:53:42.029189 ampel_core-0.9.0/ampel/config/collector/ChannelConfigCollector.py
--rwxr-xr-x   0        0        0     2728 2023-04-06 19:53:42.029189 ampel_core-0.9.0/ampel/config/collector/ConfigCollector.py
--rwxr-xr-x   0        0        0     2387 2023-04-06 19:53:42.029189 ampel_core-0.9.0/ampel/config/collector/DBConfigCollector.py
--rwxr-xr-x   0        0        0     1243 2023-04-06 19:53:42.029189 ampel_core-0.9.0/ampel/config/collector/ForwardProcessConfigCollector.py
--rwxr-xr-x   0        0        0     1958 2023-04-06 19:53:42.029189 ampel_core-0.9.0/ampel/config/collector/LoggingCollector.py
--rwxr-xr-x   0        0        0     1390 2023-04-06 19:53:42.029189 ampel_core-0.9.0/ampel/config/collector/ProcessConfigCollector.py
--rwxr-xr-x   0        0        0     1673 2023-04-06 19:53:42.029189 ampel_core-0.9.0/ampel/config/collector/ResourceConfigCollector.py
--rwxr-xr-x   0        0        0     1648 2023-04-06 19:53:42.029189 ampel_core-0.9.0/ampel/config/collector/T02ConfigCollector.py
--rwxr-xr-x   0        0        0     7085 2023-04-06 19:53:42.029189 ampel_core-0.9.0/ampel/config/collector/UnitConfigCollector.py
--rwxr-xr-x   0        0        0     6743 2023-04-06 19:53:42.029189 ampel_core-0.9.0/ampel/core/AmpelContext.py
--rwxr-xr-x   0        0        0    10976 2023-04-06 19:53:42.029189 ampel_core-0.9.0/ampel/core/AmpelController.py
--rwxr-xr-x   0        0        0    19022 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/core/AmpelDB.py
--rwxr-xr-x   0        0        0    17800 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/core/AmpelRegister.py
--rwxr-xr-x   0        0        0      861 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/core/ContextUnit.py
--rwxr-xr-x   0        0        0     6353 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/core/DataLoader.py
--rwxr-xr-x   0        0        0    10174 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/core/DefaultProcessController.py
--rw-r--r--   0        0        0     4740 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/core/DocBuilder.py
--rwxr-xr-x   0        0        0     4688 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/core/EventHandler.py
--rwxr-xr-x   0        0        0     3642 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/core/Schedulable.py
--rwxr-xr-x   0        0        0    14844 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/core/UnitLoader.py
--rw-r--r--   0        0        0      855 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/demo/DemoFirstPointT2Unit.py
--rw-r--r--   0        0        0     1075 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/demo/DemoPointT2Unit.py
--rw-r--r--   0        0        0     1633 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/demo/DemoProcessor.py
--rw-r--r--   0        0        0     1336 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/demo/DemoT3Unit.py
--rwxr-xr-x   0        0        0      878 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/demo/DemoT4RunTimeAliasGenerator.py
--rwxr-xr-x   0        0        0     3818 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/dev/DevAmpelContext.py
--rw-r--r--   0        0        0      841 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/dev/NoShaper.py
--rwxr-xr-x   0        0        0    27480 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/ingest/ChainedIngestionHandler.py
--rw-r--r--   0        0        0     1435 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/ingest/ChainedT0Muxer.py
--rw-r--r--   0        0        0     3115 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/ingest/StockCompiler.py
--rw-r--r--   0        0        0     2480 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/ingest/T0Compiler.py
--rw-r--r--   0        0        0     5255 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/ingest/T1Compiler.py
--rw-r--r--   0        0        0     3009 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/ingest/T2Compiler.py
--rwxr-xr-x   0        0        0     8036 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/log/AmpelLogger.py
--rwxr-xr-x   0        0        0      389 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/log/AmpelLoggingError.py
--rw-r--r--   0        0        0     1424 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/log/LightLogRecord.py
--rw-r--r--   0        0        0     1195 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/log/LogFlag.py
--rwxr-xr-x   0        0        0     1491 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/log/LoggingErrorReporter.py
--rw-r--r--   0        0        0     3975 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/log/LogsDumper.py
--rw-r--r--   0        0        0      477 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/log/__init__.py
--rwxr-xr-x   0        0        0     6010 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/log/handlers/AmpelStreamHandler.py
--rwxr-xr-x   0        0        0     2443 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/log/handlers/ChanRecordBufHandler.py
--rw-r--r--   0        0        0     2006 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/log/handlers/DefaultRecordBufferingHandler.py
--rw-r--r--   0        0        0     1712 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/log/handlers/EnclosedChanRecordBufHandler.py
--rw-r--r--   0        0        0     1528 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/log/handlers/RecordBufferingHandler.py
--rwxr-xr-x   0        0        0     8251 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/log/utils.py
--rw-r--r--   0        0        0     1212 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/metrics/AmpelDBCollector.py
--rw-r--r--   0        0        0     2387 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/metrics/AmpelMetricsRegistry.py
--rw-r--r--   0        0        0     1940 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/metrics/AmpelProcessCollector.py
--rw-r--r--   0        0        0     5175 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/metrics/prometheus.py
--rwxr-xr-x   0        0        0     1059 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/model/ChannelModel.py
--rwxr-xr-x   0        0        0     1484 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/model/ProcessModel.py
--rw-r--r--   0        0        0       93 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/model/Readme.md
--rw-r--r--   0        0        0      856 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/model/aux/AuxAliasableModel.py
--rw-r--r--   0        0        0     1253 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/model/aux/FilterCriterion.py
--rw-r--r--   0        0        0      580 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/model/builder/BuilderAliasModel.py
--rw-r--r--   0        0        0      526 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/model/builder/RemoteUnitDefinition.py
--rwxr-xr-x   0        0        0      938 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/model/ingest/CompilerOptions.py
--rw-r--r--   0        0        0     2044 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/model/ingest/DualIngestDirective.py
--rw-r--r--   0        0        0      737 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/model/ingest/FilterModel.py
--rw-r--r--   0        0        0     2065 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/model/ingest/IngestBody.py
--rw-r--r--   0        0        0     1286 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/model/ingest/IngestDirective.py
--rw-r--r--   0        0        0     1451 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/model/ingest/MuxModel.py
--rwxr-xr-x   0        0        0     1215 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/model/ingest/T1Combine.py
--rwxr-xr-x   0        0        0      780 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/model/ingest/T1CombineCompute.py
--rwxr-xr-x   0        0        0     1369 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/model/ingest/T1CombineComputeNow.py
--rwxr-xr-x   0        0        0      785 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/model/ingest/T2Compute.py
--rw-r--r--   0        0        0      459 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/model/job/EnvSpec.py
--rw-r--r--   0        0        0     1211 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/model/job/JobModel.py
--rw-r--r--   0        0        0     1715 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/model/job/JobTaskModel.py
--rw-r--r--   0        0        0      407 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/model/job/MongoOpts.py
--rwxr-xr-x   0        0        0     1757 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/model/purge/PurgeContentModel.py
--rw-r--r--   0        0        0     1010 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/model/purge/PurgeLogsModel.py
--rw-r--r--   0        0        0      620 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/model/purge/PurgeModel.py
--rw-r--r--   0        0        0      949 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/model/t3/AliasableModel.py
--rwxr-xr-x   0        0        0     1707 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/model/t3/LoaderDirective.py
--rwxr-xr-x   0        0        0     5003 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/model/t3/QueryMatchModel.py
--rwxr-xr-x   0        0        0      577 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/model/t3/T2FilterModel.py
--rw-r--r--   0        0        0      969 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/model/t3/T3IncludeDirective.py
--rwxr-xr-x   0        0        0     1047 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/model/t3/T3ProjectionDirective.py
--rwxr-xr-x   0        0        0      878 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/model/time/QueryTimeModel.py
--rwxr-xr-x   0        0        0     2007 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/model/time/TimeConstraintModel.py
--rwxr-xr-x   0        0        0      988 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/model/time/TimeDeltaModel.py
--rwxr-xr-x   0        0        0     1592 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/model/time/TimeLastRunModel.py
--rw-r--r--   0        0        0      723 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/model/time/TimeStringModel.py
--rw-r--r--   0        0        0      587 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/model/time/UnixTimeModel.py
--rw-r--r--   0        0        0      691 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/mongo/model/AmpelColModel.py
--rw-r--r--   0        0        0      679 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/mongo/model/AmpelDBModel.py
--rw-r--r--   0        0        0      765 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/mongo/model/FieldModel.py
--rw-r--r--   0        0        0      801 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/mongo/model/IndexModel.py
--rwxr-xr-x   0        0        0     1054 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/mongo/model/MongoClientOptionsModel.py
--rw-r--r--   0        0        0      476 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/mongo/model/MongoClientRoleModel.py
--rw-r--r--   0        0        0      955 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/mongo/model/ShortIndexModel.py
--rw-r--r--   0        0        0     6236 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/mongo/purge/MongoStockDeleter.py
--rwxr-xr-x   0        0        0     1981 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/mongo/query/general.py
--rwxr-xr-x   0        0        0     2395 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/mongo/query/stock.py
--rw-r--r--   0        0        0     6067 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/mongo/query/t1.py
--rwxr-xr-x   0        0        0     3764 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/mongo/query/t2.py
--rwxr-xr-x   0        0        0     5515 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/mongo/query/var/LogsLoader.py
--rwxr-xr-x   0        0        0     4725 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/mongo/query/var/LogsMatcher.py
--rwxr-xr-x   0        0        0     3018 2023-04-06 19:53:42.033189 ampel_core-0.9.0/ampel/mongo/query/var/events.py
--rwxr-xr-x   0        0        0    10343 2023-04-06 19:53:42.037189 ampel_core-0.9.0/ampel/mongo/schema.py
--rwxr-xr-x   0        0        0    13177 2023-04-06 19:53:42.037189 ampel_core-0.9.0/ampel/mongo/update/DBUpdatesBuffer.py
--rwxr-xr-x   0        0        0     1883 2023-04-06 19:53:42.037189 ampel_core-0.9.0/ampel/mongo/update/MongoStockIngester.py
--rwxr-xr-x   0        0        0     9784 2023-04-06 19:53:42.037189 ampel_core-0.9.0/ampel/mongo/update/MongoStockUpdater.py
--rwxr-xr-x   0        0        0     1806 2023-04-06 19:53:42.037189 ampel_core-0.9.0/ampel/mongo/update/MongoT0Ingester.py
--rwxr-xr-x   0        0        0     1515 2023-04-06 19:53:42.037189 ampel_core-0.9.0/ampel/mongo/update/MongoT1Ingester.py
--rwxr-xr-x   0        0        0     1505 2023-04-06 19:53:42.037189 ampel_core-0.9.0/ampel/mongo/update/MongoT2Ingester.py
--rwxr-xr-x   0        0        0      750 2023-04-06 19:53:42.037189 ampel_core-0.9.0/ampel/mongo/update/MongoT3Ingester.py
--rwxr-xr-x   0        0        0    10782 2023-04-06 19:53:42.037189 ampel_core-0.9.0/ampel/mongo/update/var/DBLoggingHandler.py
--rwxr-xr-x   0        0        0     2250 2023-04-06 19:53:42.037189 ampel_core-0.9.0/ampel/mongo/utils.py
--rw-r--r--   0        0        0     4925 2023-04-06 19:53:42.037189 ampel_core-0.9.0/ampel/mongo/view/AbsMongoFlatMultiView.py
--rw-r--r--   0        0        0     2052 2023-04-06 19:53:42.037189 ampel_core-0.9.0/ampel/mongo/view/AbsMongoView.py
--rw-r--r--   0        0        0      963 2023-04-06 19:53:42.037189 ampel_core-0.9.0/ampel/mongo/view/FrozenValuesDict.py
--rw-r--r--   0        0        0      932 2023-04-06 19:53:42.037189 ampel_core-0.9.0/ampel/mongo/view/MongoAndView.py
--rw-r--r--   0        0        0     2390 2023-04-06 19:53:42.037189 ampel_core-0.9.0/ampel/mongo/view/MongoOneView.py
--rw-r--r--   0        0        0      666 2023-04-06 19:53:42.037189 ampel_core-0.9.0/ampel/mongo/view/MongoOrView.py
--rwxr-xr-x   0        0        0     5488 2023-04-06 19:53:42.037189 ampel_core-0.9.0/ampel/ops/AmpelExceptionPublisher.py
--rw-r--r--   0        0        0     1837 2023-04-06 19:53:42.037189 ampel_core-0.9.0/ampel/ops/OpsProcessor.py
--rw-r--r--   0        0        0        0 2023-04-06 19:53:42.037189 ampel_core-0.9.0/ampel/py.typed
--rwxr-xr-x   0        0        0    23965 2023-04-06 19:53:42.037189 ampel_core-0.9.0/ampel/run/server.py
--rwxr-xr-x   0        0        0     1346 2023-04-06 19:53:42.037189 ampel_core-0.9.0/ampel/secret/AESecretProvider.py
--rwxr-xr-x   0        0        0     1873 2023-04-06 19:53:42.037189 ampel_core-0.9.0/ampel/secret/DictSecretProvider.py
--rw-r--r--   0        0        0     1505 2023-04-06 19:53:42.037189 ampel_core-0.9.0/ampel/secret/DirSecretProvider.py
--rwxr-xr-x   0        0        0      885 2023-04-06 19:53:42.037189 ampel_core-0.9.0/ampel/secret/PotemkinSecretProvider.py
--rw-r--r--   0        0        0       26 2023-04-06 19:53:42.037189 ampel_core-0.9.0/ampel/t1/README.md
--rwxr-xr-x   0        0        0      883 2023-04-06 19:53:42.037189 ampel_core-0.9.0/ampel/t1/T1SimpleCombiner.py
--rwxr-xr-x   0        0        0     1532 2023-04-06 19:53:42.037189 ampel_core-0.9.0/ampel/t1/T1SimpleRetroCombiner.py
--rw-r--r--   0        0        0       26 2023-04-06 19:53:42.037189 ampel_core-0.9.0/ampel/t2/README.md
--rw-r--r--   0        0        0     4170 2023-04-06 19:53:42.037189 ampel_core-0.9.0/ampel/t2/T2Utils.py
--rwxr-xr-x   0        0        0    21046 2023-04-06 19:53:42.037189 ampel_core-0.9.0/ampel/t2/T2Worker.py
--rw-r--r--   0        0        0     3548 2023-04-06 19:53:42.037189 ampel_core-0.9.0/ampel/t3/README.md
--rwxr-xr-x   0        0        0     3774 2023-04-06 19:53:42.037189 ampel_core-0.9.0/ampel/t3/T3Processor.py
--rwxr-xr-x   0        0        0     1525 2023-04-06 19:53:42.037189 ampel_core-0.9.0/ampel/t3/include/session/T3SessionAlertsNumber.py
--rwxr-xr-x   0        0        0     1482 2023-04-06 19:53:42.037189 ampel_core-0.9.0/ampel/t3/include/session/T3SessionLastRunTime.py
--rwxr-xr-x   0        0        0     1664 2023-04-06 19:53:42.037189 ampel_core-0.9.0/ampel/t3/stage/BaseViewGenerator.py
--rwxr-xr-x   0        0        0     1063 2023-04-06 19:53:42.037189 ampel_core-0.9.0/ampel/t3/stage/NoViewGenerator.py
--rw-r--r--   0        0        0     3901 2023-04-06 19:53:42.037189 ampel_core-0.9.0/ampel/t3/stage/README.md
--rwxr-xr-x   0        0        0     1335 2023-04-06 19:53:42.037189 ampel_core-0.9.0/ampel/t3/stage/SimpleViewGenerator.py
--rwxr-xr-x   0        0        0     7368 2023-04-06 19:53:42.037189 ampel_core-0.9.0/ampel/t3/stage/T3AdaptativeStager.py
--rw-r--r--   0        0        0     6354 2023-04-06 19:53:42.037189 ampel_core-0.9.0/ampel/t3/stage/T3AggregatingStager.py
--rwxr-xr-x   0        0        0     4982 2023-04-06 19:53:42.037189 ampel_core-0.9.0/ampel/t3/stage/T3BaseStager.py
--rwxr-xr-x   0        0        0     2038 2023-04-06 19:53:42.037189 ampel_core-0.9.0/ampel/t3/stage/T3ChannelStager.py
--rwxr-xr-x   0        0        0     3097 2023-04-06 19:53:42.037189 ampel_core-0.9.0/ampel/t3/stage/T3DistributiveStager.py
--rwxr-xr-x   0        0        0     8016 2023-04-06 19:53:42.037189 ampel_core-0.9.0/ampel/t3/stage/T3ProjectingStager.py
--rwxr-xr-x   0        0        0     3823 2023-04-06 19:53:42.037189 ampel_core-0.9.0/ampel/t3/stage/T3SequentialStager.py
--rwxr-xr-x   0        0        0     1689 2023-04-06 19:53:42.037189 ampel_core-0.9.0/ampel/t3/stage/T3SimpleStager.py
--rwxr-xr-x   0        0        0     5629 2023-04-06 19:53:42.037189 ampel_core-0.9.0/ampel/t3/stage/T3ThreadedStager.py
--rwxr-xr-x   0        0        0     1297 2023-04-06 19:53:42.037189 ampel_core-0.9.0/ampel/t3/stage/ThreadedViewGenerator.py
--rwxr-xr-x   0        0        0     4456 2023-04-06 19:53:42.037189 ampel_core-0.9.0/ampel/t3/stage/filter/T3AmpelBufferFilter.py
--rwxr-xr-x   0        0        0     6450 2023-04-06 19:53:42.037189 ampel_core-0.9.0/ampel/t3/stage/project/T3BaseProjector.py
--rwxr-xr-x   0        0        0     3537 2023-04-06 19:53:42.037189 ampel_core-0.9.0/ampel/t3/stage/project/T3ChannelProjector.py
--rwxr-xr-x   0        0        0     1510 2023-04-06 19:53:42.037189 ampel_core-0.9.0/ampel/t3/supply/SimpleT2BasedSupplier.py
--rwxr-xr-x   0        0        0     3701 2023-04-06 19:53:42.037189 ampel_core-0.9.0/ampel/t3/supply/T3DefaultBufferSupplier.py
--rwxr-xr-x   0        0        0     2583 2023-04-06 19:53:42.037189 ampel_core-0.9.0/ampel/t3/supply/complement/T3ExtJournalAppender.py
--rwxr-xr-x   0        0        0     1765 2023-04-06 19:53:42.037189 ampel_core-0.9.0/ampel/t3/supply/complement/T3LogsAppender.py
--rwxr-xr-x   0        0        0     1298 2023-04-06 19:53:42.037189 ampel_core-0.9.0/ampel/t3/supply/complement/T3RandIntAppender.py
--rwxr-xr-x   0        0        0     4727 2023-04-06 19:53:42.037189 ampel_core-0.9.0/ampel/t3/supply/load/T3LatestStateDataLoader.py
--rwxr-xr-x   0        0        0     1191 2023-04-06 19:53:42.037189 ampel_core-0.9.0/ampel/t3/supply/load/T3SimpleDataLoader.py
--rwxr-xr-x   0        0        0     5069 2023-04-06 19:53:42.037189 ampel_core-0.9.0/ampel/t3/supply/select/T3FilteringStockSelector.py
--rwxr-xr-x   0        0        0     3149 2023-04-06 19:53:42.037189 ampel_core-0.9.0/ampel/t3/supply/select/T3StockSelector.py
--rwxr-xr-x   0        0        0      951 2023-04-06 19:53:42.037189 ampel_core-0.9.0/ampel/t3/unit/T3LogAggregatedStocks.py
--rwxr-xr-x   0        0        0     3082 2023-04-06 19:53:42.037189 ampel_core-0.9.0/ampel/t4/T4Processor.py
--rw-r--r--   0        0        0     1994 2023-04-06 19:53:42.037189 ampel_core-0.9.0/ampel/t4/T4RunTimeContextUpdater.py
--rw-r--r--   0        0        0     1318 2023-04-06 19:53:42.037189 ampel_core-0.9.0/ampel/template/ChannelWithProcsTemplate.py
--rwxr-xr-x   0        0        0     6163 2023-04-06 19:53:42.037189 ampel_core-0.9.0/ampel/template/PeriodicSummaryT3.py
--rwxr-xr-x   0        0        0      464 2023-04-06 19:53:42.037189 ampel_core-0.9.0/ampel/test/DummyStateT2Unit.py
--rw-r--r--   0        0        0     7955 2023-04-06 19:53:42.037189 ampel_core-0.9.0/ampel/test/conftest.py
--rwxr-xr-x   0        0        0     4312 2023-04-06 19:53:42.037189 ampel_core-0.9.0/ampel/test/dummy.py
--rw-r--r--   0        0        0    14551 2023-04-06 19:53:42.037189 ampel_core-0.9.0/ampel/test/pylintrc
--rw-r--r--   0        0        0    69357 2023-04-06 19:53:42.037189 ampel_core-0.9.0/ampel/test/test-data/ZTF20abxvcrk.pkl
--rw-r--r--   0        0        0    15835 2023-04-06 19:53:42.037189 ampel_core-0.9.0/ampel/test/test-data/testing-config.yaml
--rw-r--r--   0        0        0      669 2023-04-06 19:53:42.041189 ampel_core-0.9.0/ampel/test/test_AbsChannelTemplate.py
--rw-r--r--   0        0        0     1955 2023-04-06 19:53:42.041189 ampel_core-0.9.0/ampel/test/test_AmpelContext.py
--rw-r--r--   0        0        0      295 2023-04-06 19:53:42.041189 ampel_core-0.9.0/ampel/test/test_AmpelController.py
--rw-r--r--   0        0        0      238 2023-04-06 19:53:42.041189 ampel_core-0.9.0/ampel/test/test_AmpelMetricsRegistry.py
--rw-r--r--   0        0        0     1474 2023-04-06 19:53:42.041189 ampel_core-0.9.0/ampel/test/test_DBUpdatesBuffer.py
--rw-r--r--   0        0        0     1220 2023-04-06 19:53:42.041189 ampel_core-0.9.0/ampel/test/test_DefaultProcessController.py
--rw-r--r--   0        0        0    13649 2023-04-06 19:53:42.041189 ampel_core-0.9.0/ampel/test/test_IngestionHandler.py
--rw-r--r--   0        0        0     3431 2023-04-06 19:53:42.041189 ampel_core-0.9.0/ampel/test/test_JobCommand.py
--rw-r--r--   0        0        0     1632 2023-04-06 19:53:42.041189 ampel_core-0.9.0/ampel/test/test_PeriodicSummaryT3.py
--rw-r--r--   0        0        0     3466 2023-04-06 19:53:42.041189 ampel_core-0.9.0/ampel/test/test_ProcessMorpher.py
--rw-r--r--   0        0        0     1065 2023-04-06 19:53:42.041189 ampel_core-0.9.0/ampel/test/test_SimpleTagFilter.py
--rw-r--r--   0        0        0     6575 2023-04-06 19:53:42.041189 ampel_core-0.9.0/ampel/test/test_T2Processor.py
--rw-r--r--   0        0        0     4564 2023-04-06 19:53:42.041189 ampel_core-0.9.0/ampel/test/test_T3ChannelProjector.py
--rw-r--r--   0        0        0     2201 2023-04-06 19:53:42.041189 ampel_core-0.9.0/ampel/test/test_T3FilteringStockSelector.py
--rw-r--r--   0        0        0     7258 2023-04-06 19:53:42.041189 ampel_core-0.9.0/ampel/test/test_T3Processor.py
--rw-r--r--   0        0        0      680 2023-04-06 19:53:42.041189 ampel_core-0.9.0/ampel/test/test_T3SimpleDataLoader.py
--rw-r--r--   0        0        0     7030 2023-04-06 19:53:42.041189 ampel_core-0.9.0/ampel/test/test_UnitLoader.py
--rw-r--r--   0        0        0     8909 2023-04-06 19:53:42.041189 ampel_core-0.9.0/ampel/test/test_concurrent.py
--rw-r--r--   0        0        0     4343 2023-04-06 19:53:42.041189 ampel_core-0.9.0/ampel/test/test_config.py
--rw-r--r--   0        0        0    10276 2023-04-06 19:53:42.041189 ampel_core-0.9.0/ampel/test/test_server.py
--rw-r--r--   0        0        0      744 2023-04-06 19:53:42.041189 ampel_core-0.9.0/ampel/test/test_util_mappings.py
--rw-r--r--   0        0        0     2006 2023-04-06 19:53:42.041189 ampel_core-0.9.0/ampel/test/test_util_template.py
--rwxr-xr-x   0        0        0     4842 2023-04-06 19:53:42.041189 ampel_core-0.9.0/ampel/util/collections.py
--rwxr-xr-x   0        0        0     9905 2023-04-06 19:53:42.041189 ampel_core-0.9.0/ampel/util/concurrent.py
--rw-r--r--   0        0        0      822 2023-04-06 19:53:42.041189 ampel_core-0.9.0/ampel/util/config.py
--rw-r--r--   0        0        0     2316 2023-04-06 19:53:42.041189 ampel_core-0.9.0/ampel/util/debug.py
--rw-r--r--   0        0        0     3653 2023-04-06 19:53:42.041189 ampel_core-0.9.0/ampel/util/distrib.py
--rw-r--r--   0        0        0      883 2023-04-06 19:53:42.041189 ampel_core-0.9.0/ampel/util/getch.py
--rwxr-xr-x   0        0        0     6044 2023-04-06 19:53:42.041189 ampel_core-0.9.0/ampel/util/logicschema.py
--rw-r--r--   0        0        0     7514 2023-04-06 19:53:42.041189 ampel_core-0.9.0/ampel/util/pretty.py
--rwxr-xr-x   0        0        0    17510 2023-04-06 19:53:42.041189 ampel_core-0.9.0/ampel/util/register.py
--rw-r--r--   0        0        0     2043 2023-04-06 19:53:42.041189 ampel_core-0.9.0/ampel/util/stock.py
--rwxr-xr-x   0        0        0     3879 2023-04-06 19:53:42.041189 ampel_core-0.9.0/ampel/util/template.py
--rw-r--r--   0        0        0     1070 2023-04-06 19:53:42.041189 ampel_core-0.9.0/ampel/vendor/aiopipe/LICENSE.txt
--rw-r--r--   0        0        0     8895 2023-04-06 19:53:42.041189 ampel_core-0.9.0/ampel/vendor/aiopipe/__init__.py
--rw-r--r--   0        0        0     2837 2023-04-06 19:53:42.041189 ampel_core-0.9.0/conf/ampel-core/ampel.yaml
--rw-r--r--   0        0        0      854 2023-04-06 19:53:42.041189 ampel_core-0.9.0/conf/ampel-core/logging.yaml
--rw-r--r--   0        0        0      586 2023-04-06 19:53:42.041189 ampel_core-0.9.0/conf/ampel-core/mongo/data.yaml
--rw-r--r--   0        0        0      109 2023-04-06 19:53:42.041189 ampel_core-0.9.0/conf/ampel-core/mongo/ext.yaml
--rw-r--r--   0        0        0      341 2023-04-06 19:53:42.041189 ampel_core-0.9.0/conf/ampel-core/mongo/var.yaml
--rw-r--r--   0        0        0     3105 2023-04-06 19:53:42.041189 ampel_core-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     2087 1970-01-01 00:00:00.000000 ampel_core-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1512 2023-12-19 09:17:51.267581 ampel_core-0.9.1a0/LICENSE
+-rw-r--r--   0        0        0      262 2023-12-19 09:17:51.267581 ampel_core-0.9.1a0/README.md
+-rwxr-xr-x   0        0        0     1251 2023-12-19 09:17:51.267581 ampel_core-0.9.1a0/ampel/abstract/AbsBufferComplement.py
+-rw-r--r--   0        0        0     1551 2023-12-19 09:17:51.267581 ampel_core-0.9.1a0/ampel/abstract/AbsChannelTemplate.py
+-rwxr-xr-x   0        0        0     6900 2023-12-19 09:17:51.267581 ampel_core-0.9.1a0/ampel/abstract/AbsCompiler.py
+-rw-r--r--   0        0        0      853 2023-12-19 09:17:51.267581 ampel_core-0.9.1a0/ampel/abstract/AbsConfigMorpher.py
+-rw-r--r--   0        0        0     1004 2023-12-19 09:17:51.267581 ampel_core-0.9.1a0/ampel/abstract/AbsConfigUpdater.py
+-rwxr-xr-x   0        0        0      871 2023-12-19 09:17:51.267581 ampel_core-0.9.1a0/ampel/abstract/AbsDocIngester.py
+-rwxr-xr-x   0        0        0      886 2023-12-19 09:17:51.267581 ampel_core-0.9.1a0/ampel/abstract/AbsDocUpdater.py
+-rw-r--r--   0        0        0     4524 2023-12-19 09:17:51.267581 ampel_core-0.9.1a0/ampel/abstract/AbsEventUnit.py
+-rw-r--r--   0        0        0     1112 2023-12-19 09:17:51.267581 ampel_core-0.9.1a0/ampel/abstract/AbsOpsUnit.py
+-rwxr-xr-x   0        0        0     2719 2023-12-19 09:17:51.267581 ampel_core-0.9.1a0/ampel/abstract/AbsProcessController.py
+-rwxr-xr-x   0        0        0     2334 2023-12-19 09:17:51.267581 ampel_core-0.9.1a0/ampel/abstract/AbsT0Muxer.py
+-rwxr-xr-x   0        0        0      743 2023-12-19 09:17:51.267581 ampel_core-0.9.1a0/ampel/abstract/AbsT3Filter.py
+-rwxr-xr-x   0        0        0     2502 2023-12-19 09:17:51.267581 ampel_core-0.9.1a0/ampel/abstract/AbsT3Loader.py
+-rwxr-xr-x   0        0        0      767 2023-12-19 09:17:51.267581 ampel_core-0.9.1a0/ampel/abstract/AbsT3Projector.py
+-rwxr-xr-x   0        0        0      777 2023-12-19 09:17:51.267581 ampel_core-0.9.1a0/ampel/abstract/AbsT3Selector.py
+-rwxr-xr-x   0        0        0     1239 2023-12-19 09:17:51.267581 ampel_core-0.9.1a0/ampel/abstract/AbsT3Stager.py
+-rwxr-xr-x   0        0        0      939 2023-12-19 09:17:51.267581 ampel_core-0.9.1a0/ampel/abstract/AbsT3Supplier.py
+-rwxr-xr-x   0        0        0      979 2023-12-19 09:17:51.267581 ampel_core-0.9.1a0/ampel/abstract/AbsT4ControlUnit.py
+-rw-r--r--   0        0        0      593 2023-12-19 09:17:51.267581 ampel_core-0.9.1a0/ampel/abstract/AbsTargetSource.py
+-rwxr-xr-x   0        0        0      700 2023-12-19 09:17:51.267581 ampel_core-0.9.1a0/ampel/abstract/AbsUnitResultAdapter.py
+-rwxr-xr-x   0        0        0    15609 2023-12-19 09:17:51.267581 ampel_core-0.9.1a0/ampel/abstract/AbsWorker.py
+-rw-r--r--   0        0        0      282 2023-12-19 09:17:51.271581 ampel_core-0.9.1a0/ampel/abstract/README.md
+-rwxr-xr-x   0        0        0    11114 2023-12-19 09:17:51.271581 ampel_core-0.9.1a0/ampel/aux/ComboDictModifier.py
+-rw-r--r--   0        0        0     1248 2023-12-19 09:17:51.271581 ampel_core-0.9.1a0/ampel/aux/SimpleTagFilter.py
+-rwxr-xr-x   0        0        0     1575 2023-12-19 09:17:51.271581 ampel_core-0.9.1a0/ampel/aux/filter/AbsLogicOperatorFilter.py
+-rw-r--r--   0        0        0     1192 2023-12-19 09:17:51.271581 ampel_core-0.9.1a0/ampel/aux/filter/FlatDictArrayFilter.py
+-rw-r--r--   0        0        0     1116 2023-12-19 09:17:51.271581 ampel_core-0.9.1a0/ampel/aux/filter/PrimitiveTypeArrayFilter.py
+-rw-r--r--   0        0        0     1768 2023-12-19 09:17:51.271581 ampel_core-0.9.1a0/ampel/aux/filter/SimpleDictArrayFilter.py
+-rw-r--r--   0        0        0     4316 2023-12-19 09:17:51.271581 ampel_core-0.9.1a0/ampel/cli/AbsCoreCommand.py
+-rw-r--r--   0        0        0     2134 2023-12-19 09:17:51.271581 ampel_core-0.9.1a0/ampel/cli/AbsLoadCommand.py
+-rwxr-xr-x   0        0        0     6032 2023-12-19 09:17:51.271581 ampel_core-0.9.1a0/ampel/cli/AbsStockCommand.py
+-rw-r--r--   0        0        0     4200 2023-12-19 09:17:51.271581 ampel_core-0.9.1a0/ampel/cli/BufferCommand.py
+-rw-r--r--   0        0        0    11718 2023-12-19 09:17:51.271581 ampel_core-0.9.1a0/ampel/cli/ConfigCommand.py
+-rw-r--r--   0        0        0     5463 2023-12-19 09:17:51.271581 ampel_core-0.9.1a0/ampel/cli/DBCommand.py
+-rw-r--r--   0        0        0     5939 2023-12-19 09:17:51.271581 ampel_core-0.9.1a0/ampel/cli/EventCommand.py
+-rw-r--r--   0        0        0    23458 2023-12-19 09:17:51.271581 ampel_core-0.9.1a0/ampel/cli/JobCommand.py
+-rw-r--r--   0        0        0     8842 2023-12-19 09:17:51.271581 ampel_core-0.9.1a0/ampel/cli/LogCommand.py
+-rw-r--r--   0        0        0     7760 2023-12-19 09:17:51.271581 ampel_core-0.9.1a0/ampel/cli/ProcessCommand.py
+-rw-r--r--   0        0        0     3321 2023-12-19 09:17:51.271581 ampel_core-0.9.1a0/ampel/cli/RunCommand.py
+-rw-r--r--   0        0        0     6326 2023-12-19 09:17:51.271581 ampel_core-0.9.1a0/ampel/cli/StartCommand.py
+-rw-r--r--   0        0        0     9508 2023-12-19 09:17:51.271581 ampel_core-0.9.1a0/ampel/cli/T2Command.py
+-rw-r--r--   0        0        0     2170 2023-12-19 09:17:51.271581 ampel_core-0.9.1a0/ampel/cli/T3BufferExporterStager.py
+-rw-r--r--   0        0        0     1870 2023-12-19 09:17:51.271581 ampel_core-0.9.1a0/ampel/cli/T3BufferExporterUnit.py
+-rw-r--r--   0        0        0     4388 2023-12-19 09:17:51.271581 ampel_core-0.9.1a0/ampel/cli/ViewCommand.py
+-rw-r--r--   0        0        0     4434 2023-12-19 09:17:51.271581 ampel_core-0.9.1a0/ampel/cli/export.py
+-rw-r--r--   0        0        0     3362 2023-12-19 09:17:51.271581 ampel_core-0.9.1a0/ampel/cli/utils.py
+-rwxr-xr-x   0        0        0     1301 2023-12-19 09:17:51.271581 ampel_core-0.9.1a0/ampel/config/ScheduleEvaluator.py
+-rw-r--r--   0        0        0     1604 2023-12-19 09:17:51.271581 ampel_core-0.9.1a0/ampel/config/alter/HashT2Config.py
+-rw-r--r--   0        0        0     1605 2023-12-19 09:17:51.271581 ampel_core-0.9.1a0/ampel/config/alter/ResolveRunTimeAliases.py
+-rw-r--r--   0        0        0     1746 2023-12-19 09:17:51.271581 ampel_core-0.9.1a0/ampel/config/builder/BaseConfigChecker.py
+-rwxr-xr-x   0        0        0    20019 2023-12-19 09:17:51.271581 ampel_core-0.9.1a0/ampel/config/builder/ConfigBuilder.py
+-rw-r--r--   0        0        0     7539 2023-12-19 09:17:51.271581 ampel_core-0.9.1a0/ampel/config/builder/ConfigChecker.py
+-rw-r--r--   0        0        0     1671 2023-12-19 09:17:51.271581 ampel_core-0.9.1a0/ampel/config/builder/ConfigValidator.py
+-rwxr-xr-x   0        0        0      570 2023-12-19 09:17:51.271581 ampel_core-0.9.1a0/ampel/config/builder/DisplayOptions.py
+-rwxr-xr-x   0        0        0     8493 2023-12-19 09:17:51.271581 ampel_core-0.9.1a0/ampel/config/builder/DistConfigBuilder.py
+-rwxr-xr-x   0        0        0     3669 2023-12-19 09:17:51.271581 ampel_core-0.9.1a0/ampel/config/builder/FirstPassConfig.py
+-rwxr-xr-x   0        0        0     8958 2023-12-19 09:17:51.271581 ampel_core-0.9.1a0/ampel/config/builder/ProcessMorpher.py
+-rw-r--r--   0        0        0     1000 2023-12-19 09:17:51.271581 ampel_core-0.9.1a0/ampel/config/builder/get_env.py
+-rwxr-xr-x   0        0        0     1511 2023-12-19 09:17:51.271581 ampel_core-0.9.1a0/ampel/config/collector/AbsDictConfigCollector.py
+-rwxr-xr-x   0        0        0     2560 2023-12-19 09:17:51.271581 ampel_core-0.9.1a0/ampel/config/collector/AbsForwardConfigCollector.py
+-rwxr-xr-x   0        0        0      770 2023-12-19 09:17:51.271581 ampel_core-0.9.1a0/ampel/config/collector/AbsListConfigCollector.py
+-rwxr-xr-x   0        0        0     1985 2023-12-19 09:17:51.271581 ampel_core-0.9.1a0/ampel/config/collector/AliasConfigCollector.py
+-rwxr-xr-x   0        0        0     1826 2023-12-19 09:17:51.271581 ampel_core-0.9.1a0/ampel/config/collector/ChannelConfigCollector.py
+-rwxr-xr-x   0        0        0     2728 2023-12-19 09:17:51.271581 ampel_core-0.9.1a0/ampel/config/collector/ConfigCollector.py
+-rwxr-xr-x   0        0        0     2387 2023-12-19 09:17:51.271581 ampel_core-0.9.1a0/ampel/config/collector/DBConfigCollector.py
+-rwxr-xr-x   0        0        0     1243 2023-12-19 09:17:51.271581 ampel_core-0.9.1a0/ampel/config/collector/ForwardProcessConfigCollector.py
+-rwxr-xr-x   0        0        0     1958 2023-12-19 09:17:51.271581 ampel_core-0.9.1a0/ampel/config/collector/LoggingCollector.py
+-rwxr-xr-x   0        0        0     1390 2023-12-19 09:17:51.271581 ampel_core-0.9.1a0/ampel/config/collector/ProcessConfigCollector.py
+-rwxr-xr-x   0        0        0     1673 2023-12-19 09:17:51.271581 ampel_core-0.9.1a0/ampel/config/collector/ResourceConfigCollector.py
+-rwxr-xr-x   0        0        0     1648 2023-12-19 09:17:51.271581 ampel_core-0.9.1a0/ampel/config/collector/T02ConfigCollector.py
+-rwxr-xr-x   0        0        0     7085 2023-12-19 09:17:51.271581 ampel_core-0.9.1a0/ampel/config/collector/UnitConfigCollector.py
+-rwxr-xr-x   0        0        0     6743 2023-12-19 09:17:51.271581 ampel_core-0.9.1a0/ampel/core/AmpelContext.py
+-rwxr-xr-x   0        0        0    10976 2023-12-19 09:17:51.271581 ampel_core-0.9.1a0/ampel/core/AmpelController.py
+-rwxr-xr-x   0        0        0    19425 2023-12-19 09:17:51.271581 ampel_core-0.9.1a0/ampel/core/AmpelDB.py
+-rwxr-xr-x   0        0        0    17800 2023-12-19 09:17:51.271581 ampel_core-0.9.1a0/ampel/core/AmpelRegister.py
+-rwxr-xr-x   0        0        0      861 2023-12-19 09:17:51.271581 ampel_core-0.9.1a0/ampel/core/ContextUnit.py
+-rwxr-xr-x   0        0        0     6353 2023-12-19 09:17:51.271581 ampel_core-0.9.1a0/ampel/core/DataLoader.py
+-rwxr-xr-x   0        0        0    10174 2023-12-19 09:17:51.271581 ampel_core-0.9.1a0/ampel/core/DefaultProcessController.py
+-rw-r--r--   0        0        0     5121 2023-12-19 09:17:51.271581 ampel_core-0.9.1a0/ampel/core/DocBuilder.py
+-rwxr-xr-x   0        0        0     4688 2023-12-19 09:17:51.271581 ampel_core-0.9.1a0/ampel/core/EventHandler.py
+-rwxr-xr-x   0        0        0     3642 2023-12-19 09:17:51.271581 ampel_core-0.9.1a0/ampel/core/Schedulable.py
+-rwxr-xr-x   0        0        0    14844 2023-12-19 09:17:51.271581 ampel_core-0.9.1a0/ampel/core/UnitLoader.py
+-rw-r--r--   0        0        0      855 2023-12-19 09:17:51.271581 ampel_core-0.9.1a0/ampel/demo/DemoFirstPointT2Unit.py
+-rw-r--r--   0        0        0     1075 2023-12-19 09:17:51.271581 ampel_core-0.9.1a0/ampel/demo/DemoPointT2Unit.py
+-rw-r--r--   0        0        0     1633 2023-12-19 09:17:51.271581 ampel_core-0.9.1a0/ampel/demo/DemoProcessor.py
+-rw-r--r--   0        0        0     1336 2023-12-19 09:17:51.271581 ampel_core-0.9.1a0/ampel/demo/DemoT3Unit.py
+-rwxr-xr-x   0        0        0      878 2023-12-19 09:17:51.271581 ampel_core-0.9.1a0/ampel/demo/DemoT4RunTimeAliasGenerator.py
+-rwxr-xr-x   0        0        0     3818 2023-12-19 09:17:51.271581 ampel_core-0.9.1a0/ampel/dev/DevAmpelContext.py
+-rw-r--r--   0        0        0      841 2023-12-19 09:17:51.271581 ampel_core-0.9.1a0/ampel/dev/NoShaper.py
+-rwxr-xr-x   0        0        0    27580 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/ingest/ChainedIngestionHandler.py
+-rw-r--r--   0        0        0     1435 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/ingest/ChainedT0Muxer.py
+-rw-r--r--   0        0        0     3115 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/ingest/StockCompiler.py
+-rw-r--r--   0        0        0     2480 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/ingest/T0Compiler.py
+-rw-r--r--   0        0        0     5255 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/ingest/T1Compiler.py
+-rw-r--r--   0        0        0     3009 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/ingest/T2Compiler.py
+-rwxr-xr-x   0        0        0     8036 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/log/AmpelLogger.py
+-rwxr-xr-x   0        0        0      389 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/log/AmpelLoggingError.py
+-rw-r--r--   0        0        0     1424 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/log/LightLogRecord.py
+-rw-r--r--   0        0        0     1195 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/log/LogFlag.py
+-rwxr-xr-x   0        0        0     1491 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/log/LoggingErrorReporter.py
+-rw-r--r--   0        0        0     3975 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/log/LogsDumper.py
+-rw-r--r--   0        0        0      477 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/log/__init__.py
+-rwxr-xr-x   0        0        0     6010 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/log/handlers/AmpelStreamHandler.py
+-rwxr-xr-x   0        0        0     2443 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/log/handlers/ChanRecordBufHandler.py
+-rw-r--r--   0        0        0     2006 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/log/handlers/DefaultRecordBufferingHandler.py
+-rw-r--r--   0        0        0     1712 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/log/handlers/EnclosedChanRecordBufHandler.py
+-rw-r--r--   0        0        0     1528 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/log/handlers/RecordBufferingHandler.py
+-rwxr-xr-x   0        0        0     8251 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/log/utils.py
+-rw-r--r--   0        0        0     1212 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/metrics/AmpelDBCollector.py
+-rw-r--r--   0        0        0     6073 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/metrics/AmpelMetricsRegistry.py
+-rw-r--r--   0        0        0     1940 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/metrics/AmpelProcessCollector.py
+-rw-r--r--   0        0        0     5175 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/metrics/prometheus.py
+-rwxr-xr-x   0        0        0     1059 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/model/ChannelModel.py
+-rwxr-xr-x   0        0        0     1484 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/model/ProcessModel.py
+-rw-r--r--   0        0        0       93 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/model/Readme.md
+-rw-r--r--   0        0        0      856 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/model/aux/AuxAliasableModel.py
+-rw-r--r--   0        0        0     1253 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/model/aux/FilterCriterion.py
+-rw-r--r--   0        0        0      580 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/model/builder/BuilderAliasModel.py
+-rw-r--r--   0        0        0      526 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/model/builder/RemoteUnitDefinition.py
+-rwxr-xr-x   0        0        0      938 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/model/ingest/CompilerOptions.py
+-rw-r--r--   0        0        0     2044 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/model/ingest/DualIngestDirective.py
+-rw-r--r--   0        0        0      737 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/model/ingest/FilterModel.py
+-rw-r--r--   0        0        0     2065 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/model/ingest/IngestBody.py
+-rw-r--r--   0        0        0     1286 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/model/ingest/IngestDirective.py
+-rw-r--r--   0        0        0     1451 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/model/ingest/MuxModel.py
+-rwxr-xr-x   0        0        0     1215 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/model/ingest/T1Combine.py
+-rwxr-xr-x   0        0        0      780 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/model/ingest/T1CombineCompute.py
+-rwxr-xr-x   0        0        0     1369 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/model/ingest/T1CombineComputeNow.py
+-rwxr-xr-x   0        0        0      785 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/model/ingest/T2Compute.py
+-rw-r--r--   0        0        0      459 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/model/job/EnvSpec.py
+-rw-r--r--   0        0        0     1211 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/model/job/JobModel.py
+-rw-r--r--   0        0        0     1715 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/model/job/JobTaskModel.py
+-rw-r--r--   0        0        0      407 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/model/job/MongoOpts.py
+-rwxr-xr-x   0        0        0     1757 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/model/purge/PurgeContentModel.py
+-rw-r--r--   0        0        0     1010 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/model/purge/PurgeLogsModel.py
+-rw-r--r--   0        0        0      620 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/model/purge/PurgeModel.py
+-rw-r--r--   0        0        0      949 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/model/t3/AliasableModel.py
+-rwxr-xr-x   0        0        0     1707 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/model/t3/LoaderDirective.py
+-rwxr-xr-x   0        0        0     5003 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/model/t3/QueryMatchModel.py
+-rwxr-xr-x   0        0        0      577 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/model/t3/T2FilterModel.py
+-rw-r--r--   0        0        0      969 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/model/t3/T3IncludeDirective.py
+-rwxr-xr-x   0        0        0     1047 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/model/t3/T3ProjectionDirective.py
+-rwxr-xr-x   0        0        0      878 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/model/time/QueryTimeModel.py
+-rwxr-xr-x   0        0        0     2007 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/model/time/TimeConstraintModel.py
+-rwxr-xr-x   0        0        0      988 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/model/time/TimeDeltaModel.py
+-rwxr-xr-x   0        0        0     1592 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/model/time/TimeLastRunModel.py
+-rw-r--r--   0        0        0      723 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/model/time/TimeStringModel.py
+-rw-r--r--   0        0        0      587 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/model/time/UnixTimeModel.py
+-rw-r--r--   0        0        0      691 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/mongo/model/AmpelColModel.py
+-rw-r--r--   0        0        0      679 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/mongo/model/AmpelDBModel.py
+-rw-r--r--   0        0        0      765 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/mongo/model/FieldModel.py
+-rw-r--r--   0        0        0      801 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/mongo/model/IndexModel.py
+-rwxr-xr-x   0        0        0     1054 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/mongo/model/MongoClientOptionsModel.py
+-rw-r--r--   0        0        0      476 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/mongo/model/MongoClientRoleModel.py
+-rw-r--r--   0        0        0      955 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/mongo/model/ShortIndexModel.py
+-rw-r--r--   0        0        0     6236 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/mongo/purge/MongoStockDeleter.py
+-rwxr-xr-x   0        0        0     1981 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/mongo/query/general.py
+-rwxr-xr-x   0        0        0     2395 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/mongo/query/stock.py
+-rw-r--r--   0        0        0     6067 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/mongo/query/t1.py
+-rwxr-xr-x   0        0        0     3764 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/mongo/query/t2.py
+-rwxr-xr-x   0        0        0     5515 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/mongo/query/var/LogsLoader.py
+-rwxr-xr-x   0        0        0     4725 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/mongo/query/var/LogsMatcher.py
+-rwxr-xr-x   0        0        0     3018 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/mongo/query/var/events.py
+-rwxr-xr-x   0        0        0    10343 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/mongo/schema.py
+-rwxr-xr-x   0        0        0    14244 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/mongo/update/DBUpdatesBuffer.py
+-rwxr-xr-x   0        0        0     1883 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/mongo/update/MongoStockIngester.py
+-rwxr-xr-x   0        0        0     9899 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/mongo/update/MongoStockUpdater.py
+-rwxr-xr-x   0        0        0     1806 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/mongo/update/MongoT0Ingester.py
+-rwxr-xr-x   0        0        0     1515 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/mongo/update/MongoT1Ingester.py
+-rwxr-xr-x   0        0        0     1505 2023-12-19 09:17:51.275581 ampel_core-0.9.1a0/ampel/mongo/update/MongoT2Ingester.py
+-rwxr-xr-x   0        0        0      750 2023-12-19 09:17:51.279581 ampel_core-0.9.1a0/ampel/mongo/update/MongoT3Ingester.py
+-rwxr-xr-x   0        0        0    10782 2023-12-19 09:17:51.279581 ampel_core-0.9.1a0/ampel/mongo/update/var/DBLoggingHandler.py
+-rwxr-xr-x   0        0        0     2250 2023-12-19 09:17:51.279581 ampel_core-0.9.1a0/ampel/mongo/utils.py
+-rw-r--r--   0        0        0     4925 2023-12-19 09:17:51.279581 ampel_core-0.9.1a0/ampel/mongo/view/AbsMongoFlatMultiView.py
+-rw-r--r--   0        0        0     2052 2023-12-19 09:17:51.279581 ampel_core-0.9.1a0/ampel/mongo/view/AbsMongoView.py
+-rw-r--r--   0        0        0      963 2023-12-19 09:17:51.279581 ampel_core-0.9.1a0/ampel/mongo/view/FrozenValuesDict.py
+-rw-r--r--   0        0        0      932 2023-12-19 09:17:51.279581 ampel_core-0.9.1a0/ampel/mongo/view/MongoAndView.py
+-rw-r--r--   0        0        0     2390 2023-12-19 09:17:51.279581 ampel_core-0.9.1a0/ampel/mongo/view/MongoOneView.py
+-rw-r--r--   0        0        0      666 2023-12-19 09:17:51.279581 ampel_core-0.9.1a0/ampel/mongo/view/MongoOrView.py
+-rwxr-xr-x   0        0        0     5488 2023-12-19 09:17:51.279581 ampel_core-0.9.1a0/ampel/ops/AmpelExceptionPublisher.py
+-rw-r--r--   0        0        0     1837 2023-12-19 09:17:51.279581 ampel_core-0.9.1a0/ampel/ops/OpsProcessor.py
+-rw-r--r--   0        0        0        0 2023-12-19 09:17:51.279581 ampel_core-0.9.1a0/ampel/py.typed
+-rwxr-xr-x   0        0        0    23965 2023-12-19 09:17:51.279581 ampel_core-0.9.1a0/ampel/run/server.py
+-rwxr-xr-x   0        0        0     1346 2023-12-19 09:17:51.279581 ampel_core-0.9.1a0/ampel/secret/AESecretProvider.py
+-rwxr-xr-x   0        0        0     1873 2023-12-19 09:17:51.279581 ampel_core-0.9.1a0/ampel/secret/DictSecretProvider.py
+-rw-r--r--   0        0        0     1505 2023-12-19 09:17:51.279581 ampel_core-0.9.1a0/ampel/secret/DirSecretProvider.py
+-rwxr-xr-x   0        0        0      885 2023-12-19 09:17:51.279581 ampel_core-0.9.1a0/ampel/secret/PotemkinSecretProvider.py
+-rw-r--r--   0        0        0       26 2023-12-19 09:17:51.279581 ampel_core-0.9.1a0/ampel/t1/README.md
+-rwxr-xr-x   0        0        0      883 2023-12-19 09:17:51.279581 ampel_core-0.9.1a0/ampel/t1/T1SimpleCombiner.py
+-rwxr-xr-x   0        0        0     1532 2023-12-19 09:17:51.279581 ampel_core-0.9.1a0/ampel/t1/T1SimpleRetroCombiner.py
+-rw-r--r--   0        0        0       26 2023-12-19 09:17:51.279581 ampel_core-0.9.1a0/ampel/t2/README.md
+-rw-r--r--   0        0        0     4170 2023-12-19 09:17:51.279581 ampel_core-0.9.1a0/ampel/t2/T2Utils.py
+-rwxr-xr-x   0        0        0    21611 2023-12-19 09:17:51.279581 ampel_core-0.9.1a0/ampel/t2/T2Worker.py
+-rw-r--r--   0        0        0     3548 2023-12-19 09:17:51.279581 ampel_core-0.9.1a0/ampel/t3/README.md
+-rwxr-xr-x   0        0        0     3774 2023-12-19 09:17:51.279581 ampel_core-0.9.1a0/ampel/t3/T3Processor.py
+-rwxr-xr-x   0        0        0     1525 2023-12-19 09:17:51.279581 ampel_core-0.9.1a0/ampel/t3/include/session/T3SessionAlertsNumber.py
+-rwxr-xr-x   0        0        0     1482 2023-12-19 09:17:51.279581 ampel_core-0.9.1a0/ampel/t3/include/session/T3SessionLastRunTime.py
+-rwxr-xr-x   0        0        0     1664 2023-12-19 09:17:51.279581 ampel_core-0.9.1a0/ampel/t3/stage/BaseViewGenerator.py
+-rwxr-xr-x   0        0        0     1063 2023-12-19 09:17:51.279581 ampel_core-0.9.1a0/ampel/t3/stage/NoViewGenerator.py
+-rw-r--r--   0        0        0     3901 2023-12-19 09:17:51.279581 ampel_core-0.9.1a0/ampel/t3/stage/README.md
+-rwxr-xr-x   0        0        0     1335 2023-12-19 09:17:51.279581 ampel_core-0.9.1a0/ampel/t3/stage/SimpleViewGenerator.py
+-rwxr-xr-x   0        0        0     7368 2023-12-19 09:17:51.279581 ampel_core-0.9.1a0/ampel/t3/stage/T3AdaptativeStager.py
+-rw-r--r--   0        0        0     6354 2023-12-19 09:17:51.279581 ampel_core-0.9.1a0/ampel/t3/stage/T3AggregatingStager.py
+-rwxr-xr-x   0        0        0     4928 2023-12-19 09:17:51.279581 ampel_core-0.9.1a0/ampel/t3/stage/T3BaseStager.py
+-rwxr-xr-x   0        0        0     2038 2023-12-19 09:17:51.279581 ampel_core-0.9.1a0/ampel/t3/stage/T3ChannelStager.py
+-rwxr-xr-x   0        0        0     3097 2023-12-19 09:17:51.279581 ampel_core-0.9.1a0/ampel/t3/stage/T3DistributiveStager.py
+-rwxr-xr-x   0        0        0     8016 2023-12-19 09:17:51.279581 ampel_core-0.9.1a0/ampel/t3/stage/T3ProjectingStager.py
+-rwxr-xr-x   0        0        0     3823 2023-12-19 09:17:51.279581 ampel_core-0.9.1a0/ampel/t3/stage/T3SequentialStager.py
+-rwxr-xr-x   0        0        0     1689 2023-12-19 09:17:51.279581 ampel_core-0.9.1a0/ampel/t3/stage/T3SimpleStager.py
+-rwxr-xr-x   0        0        0     5629 2023-12-19 09:17:51.279581 ampel_core-0.9.1a0/ampel/t3/stage/T3ThreadedStager.py
+-rwxr-xr-x   0        0        0     1297 2023-12-19 09:17:51.279581 ampel_core-0.9.1a0/ampel/t3/stage/ThreadedViewGenerator.py
+-rwxr-xr-x   0        0        0     4456 2023-12-19 09:17:51.279581 ampel_core-0.9.1a0/ampel/t3/stage/filter/T3AmpelBufferFilter.py
+-rwxr-xr-x   0        0        0     6450 2023-12-19 09:17:51.279581 ampel_core-0.9.1a0/ampel/t3/stage/project/T3BaseProjector.py
+-rwxr-xr-x   0        0        0     3537 2023-12-19 09:17:51.279581 ampel_core-0.9.1a0/ampel/t3/stage/project/T3ChannelProjector.py
+-rwxr-xr-x   0        0        0     1510 2023-12-19 09:17:51.279581 ampel_core-0.9.1a0/ampel/t3/supply/SimpleT2BasedSupplier.py
+-rwxr-xr-x   0        0        0     3701 2023-12-19 09:17:51.279581 ampel_core-0.9.1a0/ampel/t3/supply/T3DefaultBufferSupplier.py
+-rwxr-xr-x   0        0        0     2583 2023-12-19 09:17:51.279581 ampel_core-0.9.1a0/ampel/t3/supply/complement/T3ExtJournalAppender.py
+-rwxr-xr-x   0        0        0     1765 2023-12-19 09:17:51.279581 ampel_core-0.9.1a0/ampel/t3/supply/complement/T3LogsAppender.py
+-rwxr-xr-x   0        0        0     1298 2023-12-19 09:17:51.279581 ampel_core-0.9.1a0/ampel/t3/supply/complement/T3RandIntAppender.py
+-rwxr-xr-x   0        0        0     4727 2023-12-19 09:17:51.279581 ampel_core-0.9.1a0/ampel/t3/supply/load/T3LatestStateDataLoader.py
+-rwxr-xr-x   0        0        0     1191 2023-12-19 09:17:51.279581 ampel_core-0.9.1a0/ampel/t3/supply/load/T3SimpleDataLoader.py
+-rwxr-xr-x   0        0        0     5069 2023-12-19 09:17:51.279581 ampel_core-0.9.1a0/ampel/t3/supply/select/T3FilteringStockSelector.py
+-rwxr-xr-x   0        0        0     3149 2023-12-19 09:17:51.279581 ampel_core-0.9.1a0/ampel/t3/supply/select/T3StockSelector.py
+-rwxr-xr-x   0        0        0      951 2023-12-19 09:17:51.279581 ampel_core-0.9.1a0/ampel/t3/unit/T3LogAggregatedStocks.py
+-rwxr-xr-x   0        0        0     3082 2023-12-19 09:17:51.279581 ampel_core-0.9.1a0/ampel/t4/T4Processor.py
+-rw-r--r--   0        0        0     1994 2023-12-19 09:17:51.279581 ampel_core-0.9.1a0/ampel/t4/T4RunTimeContextUpdater.py
+-rw-r--r--   0        0        0     1318 2023-12-19 09:17:51.279581 ampel_core-0.9.1a0/ampel/template/ChannelWithProcsTemplate.py
+-rwxr-xr-x   0        0        0     6163 2023-12-19 09:17:51.279581 ampel_core-0.9.1a0/ampel/template/PeriodicSummaryT3.py
+-rwxr-xr-x   0        0        0      464 2023-12-19 09:17:51.279581 ampel_core-0.9.1a0/ampel/test/DummyStateT2Unit.py
+-rw-r--r--   0        0        0     8253 2023-12-19 09:17:51.279581 ampel_core-0.9.1a0/ampel/test/conftest.py
+-rwxr-xr-x   0        0        0     4837 2023-12-19 09:17:51.279581 ampel_core-0.9.1a0/ampel/test/dummy.py
+-rw-r--r--   0        0        0    14551 2023-12-19 09:17:51.279581 ampel_core-0.9.1a0/ampel/test/pylintrc
+-rw-r--r--   0        0        0    69357 2023-12-19 09:17:51.279581 ampel_core-0.9.1a0/ampel/test/test-data/ZTF20abxvcrk.pkl
+-rw-r--r--   0        0        0    15819 2023-12-19 09:17:51.279581 ampel_core-0.9.1a0/ampel/test/test-data/testing-config.yaml
+-rw-r--r--   0        0        0      669 2023-12-19 09:17:51.283581 ampel_core-0.9.1a0/ampel/test/test_AbsChannelTemplate.py
+-rw-r--r--   0        0        0     1955 2023-12-19 09:17:51.283581 ampel_core-0.9.1a0/ampel/test/test_AmpelContext.py
+-rw-r--r--   0        0        0      295 2023-12-19 09:17:51.283581 ampel_core-0.9.1a0/ampel/test/test_AmpelController.py
+-rw-r--r--   0        0        0     1674 2023-12-19 09:17:51.283581 ampel_core-0.9.1a0/ampel/test/test_AmpelMetricsRegistry.py
+-rw-r--r--   0        0        0     1474 2023-12-19 09:17:51.283581 ampel_core-0.9.1a0/ampel/test/test_DBUpdatesBuffer.py
+-rw-r--r--   0        0        0     1220 2023-12-19 09:17:51.283581 ampel_core-0.9.1a0/ampel/test/test_DefaultProcessController.py
+-rw-r--r--   0        0        0    13649 2023-12-19 09:17:51.283581 ampel_core-0.9.1a0/ampel/test/test_IngestionHandler.py
+-rw-r--r--   0        0        0     3431 2023-12-19 09:17:51.283581 ampel_core-0.9.1a0/ampel/test/test_JobCommand.py
+-rw-r--r--   0        0        0     1632 2023-12-19 09:17:51.283581 ampel_core-0.9.1a0/ampel/test/test_PeriodicSummaryT3.py
+-rw-r--r--   0        0        0     3251 2023-12-19 09:17:51.283581 ampel_core-0.9.1a0/ampel/test/test_ProcessCommand.py
+-rw-r--r--   0        0        0     3466 2023-12-19 09:17:51.283581 ampel_core-0.9.1a0/ampel/test/test_ProcessMorpher.py
+-rw-r--r--   0        0        0     1065 2023-12-19 09:17:51.283581 ampel_core-0.9.1a0/ampel/test/test_SimpleTagFilter.py
+-rw-r--r--   0        0        0     2446 2023-12-19 09:17:51.283581 ampel_core-0.9.1a0/ampel/test/test_T2Command.py
+-rw-r--r--   0        0        0     6814 2023-12-19 09:17:51.283581 ampel_core-0.9.1a0/ampel/test/test_T2Processor.py
+-rw-r--r--   0        0        0     4564 2023-12-19 09:17:51.283581 ampel_core-0.9.1a0/ampel/test/test_T3ChannelProjector.py
+-rw-r--r--   0        0        0     2201 2023-12-19 09:17:51.283581 ampel_core-0.9.1a0/ampel/test/test_T3FilteringStockSelector.py
+-rw-r--r--   0        0        0     7258 2023-12-19 09:17:51.283581 ampel_core-0.9.1a0/ampel/test/test_T3Processor.py
+-rw-r--r--   0        0        0      680 2023-12-19 09:17:51.283581 ampel_core-0.9.1a0/ampel/test/test_T3SimpleDataLoader.py
+-rw-r--r--   0        0        0     7030 2023-12-19 09:17:51.283581 ampel_core-0.9.1a0/ampel/test/test_UnitLoader.py
+-rw-r--r--   0        0        0     8909 2023-12-19 09:17:51.283581 ampel_core-0.9.1a0/ampel/test/test_concurrent.py
+-rw-r--r--   0        0        0     4343 2023-12-19 09:17:51.283581 ampel_core-0.9.1a0/ampel/test/test_config.py
+-rw-r--r--   0        0        0    10276 2023-12-19 09:17:51.283581 ampel_core-0.9.1a0/ampel/test/test_server.py
+-rw-r--r--   0        0        0      744 2023-12-19 09:17:51.283581 ampel_core-0.9.1a0/ampel/test/test_util_mappings.py
+-rw-r--r--   0        0        0     2006 2023-12-19 09:17:51.283581 ampel_core-0.9.1a0/ampel/test/test_util_template.py
+-rwxr-xr-x   0        0        0     4842 2023-12-19 09:17:51.283581 ampel_core-0.9.1a0/ampel/util/collections.py
+-rwxr-xr-x   0        0        0     9998 2023-12-19 09:17:51.283581 ampel_core-0.9.1a0/ampel/util/concurrent.py
+-rw-r--r--   0        0        0      822 2023-12-19 09:17:51.283581 ampel_core-0.9.1a0/ampel/util/config.py
+-rw-r--r--   0        0        0     2316 2023-12-19 09:17:51.283581 ampel_core-0.9.1a0/ampel/util/debug.py
+-rw-r--r--   0        0        0     3653 2023-12-19 09:17:51.283581 ampel_core-0.9.1a0/ampel/util/distrib.py
+-rw-r--r--   0        0        0      883 2023-12-19 09:17:51.283581 ampel_core-0.9.1a0/ampel/util/getch.py
+-rwxr-xr-x   0        0        0     6077 2023-12-19 09:17:51.283581 ampel_core-0.9.1a0/ampel/util/logicschema.py
+-rw-r--r--   0        0        0     7514 2023-12-19 09:17:51.283581 ampel_core-0.9.1a0/ampel/util/pretty.py
+-rwxr-xr-x   0        0        0    17510 2023-12-19 09:17:51.283581 ampel_core-0.9.1a0/ampel/util/register.py
+-rw-r--r--   0        0        0     2043 2023-12-19 09:17:51.283581 ampel_core-0.9.1a0/ampel/util/stock.py
+-rwxr-xr-x   0        0        0     3879 2023-12-19 09:17:51.283581 ampel_core-0.9.1a0/ampel/util/template.py
+-rw-r--r--   0        0        0     1070 2023-12-19 09:17:51.283581 ampel_core-0.9.1a0/ampel/vendor/aiopipe/LICENSE.txt
+-rw-r--r--   0        0        0     8895 2023-12-19 09:17:51.283581 ampel_core-0.9.1a0/ampel/vendor/aiopipe/__init__.py
+-rw-r--r--   0        0        0     2837 2023-12-19 09:17:51.283581 ampel_core-0.9.1a0/conf/ampel-core/ampel.yaml
+-rw-r--r--   0        0        0      854 2023-12-19 09:17:51.283581 ampel_core-0.9.1a0/conf/ampel-core/logging.yaml
+-rw-r--r--   0        0        0      677 2023-12-19 09:17:51.283581 ampel_core-0.9.1a0/conf/ampel-core/mongo/data.yaml
+-rw-r--r--   0        0        0      109 2023-12-19 09:17:51.283581 ampel_core-0.9.1a0/conf/ampel-core/mongo/ext.yaml
+-rw-r--r--   0        0        0      341 2023-12-19 09:17:51.283581 ampel_core-0.9.1a0/conf/ampel-core/mongo/var.yaml
+-rw-r--r--   0        0        0     3104 2023-12-19 09:17:51.287581 ampel_core-0.9.1a0/pyproject.toml
+-rw-r--r--   0        0        0     2141 1970-01-01 00:00:00.000000 ampel_core-0.9.1a0/PKG-INFO
```

### Comparing `ampel_core-0.9.0/LICENSE` & `ampel_core-0.9.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/abstract/AbsBufferComplement.py` & `ampel_core-0.9.1a0/ampel/abstract/AbsBufferComplement.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/abstract/AbsChannelTemplate.py` & `ampel_core-0.9.1a0/ampel/abstract/AbsChannelTemplate.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/abstract/AbsCompiler.py` & `ampel_core-0.9.1a0/ampel/abstract/AbsCompiler.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/abstract/AbsConfigMorpher.py` & `ampel_core-0.9.1a0/ampel/abstract/AbsConfigMorpher.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/abstract/AbsConfigUpdater.py` & `ampel_core-0.9.1a0/ampel/abstract/AbsConfigUpdater.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/abstract/AbsDocIngester.py` & `ampel_core-0.9.1a0/ampel/abstract/AbsDocIngester.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/abstract/AbsDocUpdater.py` & `ampel_core-0.9.1a0/ampel/abstract/AbsDocUpdater.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/abstract/AbsEventUnit.py` & `ampel_core-0.9.1a0/ampel/abstract/AbsEventUnit.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/abstract/AbsOpsUnit.py` & `ampel_core-0.9.1a0/ampel/abstract/AbsOpsUnit.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/abstract/AbsProcessController.py` & `ampel_core-0.9.1a0/ampel/abstract/AbsProcessController.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/abstract/AbsT0Muxer.py` & `ampel_core-0.9.1a0/ampel/abstract/AbsT0Muxer.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/abstract/AbsT3Filter.py` & `ampel_core-0.9.1a0/ampel/abstract/AbsT3Filter.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/abstract/AbsT3Loader.py` & `ampel_core-0.9.1a0/ampel/abstract/AbsT3Loader.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/abstract/AbsT3Projector.py` & `ampel_core-0.9.1a0/ampel/abstract/AbsT3Projector.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/abstract/AbsT3Selector.py` & `ampel_core-0.9.1a0/ampel/abstract/AbsT3Selector.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/abstract/AbsT3Stager.py` & `ampel_core-0.9.1a0/ampel/abstract/AbsT3Stager.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/abstract/AbsT3Supplier.py` & `ampel_core-0.9.1a0/ampel/abstract/AbsT3Supplier.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/abstract/AbsT4ControlUnit.py` & `ampel_core-0.9.1a0/ampel/abstract/AbsT4ControlUnit.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/abstract/AbsTargetSource.py` & `ampel_core-0.9.1a0/ampel/abstract/AbsTargetSource.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/abstract/AbsUnitResultAdapter.py` & `ampel_core-0.9.1a0/ampel/abstract/AbsUnitResultAdapter.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/abstract/AbsWorker.py` & `ampel_core-0.9.1a0/ampel/abstract/AbsWorker.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,22 +3,25 @@
 # File:                Ampel-core/ampel/abstract/AbsWorker.py
 # License:             BSD-3-Clause
 # Author:              valery brinnel <firstname.lastname@gmail.com>
 # Date:                28.05.2021
 # Last Modified Date:  03.04.2023
 # Last Modified By:    valery brinnel <firstname.lastname@gmail.com>
 
-import gc, signal
+import gc, signal, sys
 import random
 from math import ceil
 from time import time, sleep
-from typing import ClassVar, Any, TypeVar, Generic, Literal
+from typing import ClassVar, Any, TypeVar, Generic, Literal, Sequence, Generator
 from ampel.base.AmpelBaseModel import AmpelBaseModel
+from contextlib import contextmanager
+from threading import Event
 
 from pymongo.write_concern import WriteConcern
+from pymongo.read_concern import ReadConcern
 
 from ampel.types import OneOrMany, JDict, UBson, Tag
 from ampel.base.decorator import abstractmethod
 from ampel.base.LogicalUnit import LogicalUnit
 from ampel.mongo.utils import maybe_match_array
 from ampel.log.utils import convert_dollars
 from ampel.enum.DocumentCode import DocumentCode
@@ -32,27 +35,47 @@
 from ampel.log.utils import report_exception, report_error
 from ampel.util.hash import build_unsafe_dict_id
 from ampel.abstract.AbsEventUnit import AbsEventUnit
 from ampel.abstract.AbsUnitResultAdapter import AbsUnitResultAdapter
 from ampel.model.UnitModel import UnitModel
 from ampel.mongo.update.MongoStockUpdater import MongoStockUpdater
 from ampel.mongo.utils import maybe_use_each
-from ampel.metrics.AmpelMetricsRegistry import AmpelMetricsRegistry, Histogram, Counter
+from ampel.metrics.AmpelMetricsRegistry import AmpelMetricsRegistry, Histogram, TimingCounter, Summary
 from ampel.util.tag import merge_tags
 
 T = TypeVar("T", T1Document, T2Document)
 
 class BackoffConfig(AmpelBaseModel):
 	base: float = 2
 	factor: float = 1
 	jitter: bool = True
 	max_value: float = 10.
 	max_tries: None | int = None
 	max_time: None | float = 60.
 
+stat_time = AmpelMetricsRegistry.summary(
+    "time",
+    "Processing time",
+    unit="microseconds",
+    subsystem="worker",
+    labelnames=("tier", "phase", "unit"),
+)
+
+@contextmanager
+def stop_on_signal(signals: Sequence[signal.Signals], logger: AmpelLogger) -> Generator[Event, None, None]:
+	stop_token = Event()
+	def handle_signal(signum: int, frame):
+		logger.log(LogFlag.SHOUT, f"caught {signal.Signals(signum).name}")
+		stop_token.set()
+	prev_handlers = {sig: signal.signal(sig, handle_signal) for sig in signals}
+	try:
+		yield stop_token
+	finally:
+		for sig, handler in prev_handlers.items():
+			signal.signal(sig, handler)
 
 class AbsWorker(Generic[T], AbsEventUnit, abstract=True):
 	"""
 	Fill results into pending :class:`T2 documents <ampel.content.T2Document.T2Document>`
 	or :class:`T1 documents <ampel.content.T1Document.T1Document>`
 	"""
 
@@ -100,14 +123,17 @@
 	#: Wait for documents to process
 	backoff_on_query: None | BackoffConfig = None
 
 	#: wait for majority acknowledgement of document updates. this introduces
 	#: significant extra latency for replicated mongo clusters.
 	wait_for_durable_write: bool = True
 
+	#: read only commmitted updates
+	durable_read: bool = False
+
 	#: minimum number of stock document updates to commit at once
 	updates_buffer_size: int = 500
 
 	def __init__(self, **kwargs) -> None:
 
 		super().__init__(**kwargs)
 		self._ampel_db = self.context.db
@@ -136,29 +162,26 @@
 		if not self.wait_for_durable_write:
 			# Only wait for the primary to acknowledge (in-memory) write, rather
 			# than a majority of replica set members to acknowledge write to
 			# their journals. This has much lower latency, but can result in doc
 			# updates being lost if the primary goes down before the write can
 			# be replicated, but if this happens the doc can simply be rerun.
 			self.col = self.col.with_options(write_concern=WriteConcern(w=1, j=False))
+		if self.durable_read:
+			self.col = self.col.with_options(read_concern=ReadConcern(level="majority"))
 
 		if self.send_beacon:
 			self.create_beacon()
 
-		self._run = True
-		self._doc_counter = 0
-		signal.signal(signal.SIGTERM, self.sig_exit)
-		signal.signal(signal.SIGINT, self.sig_exit)
-
 		# _instances stores unit instances so that they can be re-used in run()
 		# Key: set(unit name + config), value: unit instance
 		self._instances: JDict = {}
 
-		self._adapters: dict[str, AbsUnitResultAdapter] = {}
-
+		self._current_run_id: None | int = None
+		self._adapters: dict[int, AbsUnitResultAdapter] = {}
 
 
 	@abstractmethod
 	def process_doc(self,
 		doc: T, stock_updr: MongoStockUpdater, logger: AmpelLogger
 	) -> Any:
 		...
@@ -168,36 +191,36 @@
 		""" :returns: number of t2 docs processed """
 		event_hdlr.set_tier(2)
 		if self.pre_check and self.col.count_documents(self.query) == 0:
 			return EventCode.PRE_CHECK_EXIT
 		return None
 
 
-	def find_one_and_update(self, query: dict, update: dict) -> None | Any:
+	def find_one_and_update(self, query: dict, update: dict, stop_token: Event) -> None | T:
 		"""
 		Get next eligible document, with timeout
 		"""
 		t0 = time()
 		attempts = 0
-		while self._run:
+		while not stop_token.is_set():
 			doc = self.col.find_one_and_update(
 				query | {'$expr': {'$not': {'$lte': [ceil(time()), {'$last': '$meta.retry_after'}]}}},
 				update
 			)
 			if doc is not None or self.backoff_on_query is None:
 				return doc
 			backoff = self.backoff_on_query
 			if backoff.max_time is not None and time()-t0 > backoff.max_time:
 				break
 			if backoff.max_tries is not None and attempts+1 >= backoff.max_tries:
 				break
 			delay = min(backoff.factor*(backoff.base**attempts), backoff.max_value)
 			if backoff.jitter:
 				delay = random.uniform(0, delay)
-			sleep(delay)
+			stop_token.wait(delay)
 			attempts += 1
 		
 		return None
 
 
 	def proceed(self, event_hdlr: EventHandler) -> int:
 		""" :returns: number of t2 docs processed """
@@ -219,49 +242,62 @@
 		stock_updr = MongoStockUpdater(
 			ampel_db = self.context.db, tier = self.tier, run_id = run_id,
 			process_name = self.process_name, logger = logger,
 			raise_exc = self.raise_exc, extra_tag = self.jtag
 		)
 
 		# Loop variables
-		self._doc_counter = 0
+		doc_counter = 0
 		update = {'$set': {'code': DocumentCode.RUNNING}}
 		garbage_collect = self.garbage_collect
 		doc_limit = self.doc_limit
 
-		# Process docs until next() returns None (breaks condition below)
-		self._run = True
-		while self._run:
-
-			# get t1/t2 document (code is usually NEW or NEW_PRIO), excluding
-			# docs with retry times in the future
-			doc = self.find_one_and_update(self.query, update)
-
-			# No match
-			if doc is None:
-				break
-			elif logger.verbose > 1:
-				logger.debug(f'T{self.tier} doc to process', extra={'doc': doc})
-
-			self.process_doc(doc, stock_updr, logger)
-
-			# Check possibly defined doc_limit
-			if doc_limit and self._doc_counter >= doc_limit:
-				break
-
-			if garbage_collect:
-				gc.collect()
-
-		stock_updr.flush()
-		event_hdlr.add_extra(docs=self._doc_counter)
-
-		logger.flush()
-		self._instances.clear()
+		with stop_on_signal(
+			[signal.SIGINT, signal.SIGTERM, signal.SIGQUIT, signal.SIGHUP],
+			logger
+		) as stop_token:
+			try:
+				self._current_run_id = run_id
+				# Process docs until next() returns None (breaks condition below)
+				while not stop_token.is_set():
+
+					# get t1/t2 document (code is usually NEW or NEW_PRIO), excluding
+					# docs with retry times in the future
+					with stat_time.time() as timer:
+						doc = self.find_one_and_update(self.query, update, stop_token)
+						timer.labels(self.tier, "find_one_and_update", doc["unit"] if doc else None)
+
+					# No match
+					if doc is None:
+						if not stop_token.is_set():
+							logger.log(LogFlag.SHOUT, "No more docs to process")
+						break
+					elif logger.verbose > 1:
+						logger.debug(f'T{self.tier} doc to process', extra={'doc': doc})
+
+					with stat_time.labels(self.tier, "process_doc", doc["unit"]).time():
+						self.process_doc(doc, stock_updr, logger)
+					doc_counter += 1
+
+					# Check possibly defined doc_limit
+					if doc_limit and doc_counter >= doc_limit:
+						break
+
+					if garbage_collect:
+						gc.collect()
+			finally:
+				stock_updr.flush()
+				event_hdlr.add_extra(docs=doc_counter)
+
+				logger.flush()
+				self._instances.clear()
+				self._adapters.clear()
+				self._current_run_id = None
 
-		return self._doc_counter
+		return doc_counter
 
 
 	def _processing_error(self,
 		logger: AmpelLogger, doc: T, body: UBson,
 		meta: MetaRecord, msg: None | str = None,
 		extra: None | JDict = None, exception: None | Exception = None
 	) -> None:
@@ -378,20 +414,14 @@
 		}
 
 		if self.job_sig:
 			d['jobid'] = self.job_sig
 
 		return d
 
-
-	def sig_exit(self, signum: int, frame) -> None:
-		""" Executed when SIGTERM/SIGINT is caught. Stops doc processing in run() """
-		self._run = False
-
-
 	def create_beacon(self) -> None:
 		""" Creates a beacon document if it does not exist yet """
 
 		args = {
 			'class': self.__class__.__name__,
 			'unit': self.unit_ids,
 			'code': self.code_match,
@@ -435,25 +465,49 @@
 				logger = logger,
 				_chan = doc.get('channel') # type: ignore # probably not good to
 			)
 
 		return self._instances[k]
 
 
-def register_stats(tier: int) -> tuple[Histogram, Counter]:
+	def get_adapter_instance(self, model: UnitModel) -> AbsUnitResultAdapter:
+		assert self._current_run_id is not None
+		config_id = build_unsafe_dict_id(model.dict())
+
+		if config_id not in self._adapters:
+			unit_instance = self._loader.new_context_unit(
+				model = model,
+				context = self.context,
+				run_id = self._current_run_id,
+				sub_type = AbsUnitResultAdapter,
+			)
+			self._adapters[config_id] = unit_instance
+
+		return self._adapters[config_id]
+
+
+def register_stats(tier: int) -> tuple[Histogram, TimingCounter, Summary]:
 
-	hist = AmpelMetricsRegistry.histogram(
+	latency = AmpelMetricsRegistry.histogram(
 		'latency',
 		f'Delay between T{tier} doc creation and processing',
 		subsystem=f't{tier}',
 		unit='seconds',
 		labelnames=('unit', ),
 	)
 
-	counter = AmpelMetricsRegistry.counter(
+	docs = AmpelMetricsRegistry.counter(
 		'docs_processed',
 		f'Number of T{tier} documents processed',
 		subsystem=f't{tier}',
-		labelnames=('unit', )
+		labelnames=('unit', 'code',)
+	)
+
+	processing_time = AmpelMetricsRegistry.summary(
+		'processing_time',
+		f'Time spent processing of T{tier} documents processed',
+		subsystem=f't{tier}',
+		unit='microseconds',
+		labelnames=('unit', 'phase')
 	)
 
-	return hist, counter
+	return latency, docs, processing_time
```

### Comparing `ampel_core-0.9.0/ampel/aux/ComboDictModifier.py` & `ampel_core-0.9.1a0/ampel/aux/ComboDictModifier.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/aux/SimpleTagFilter.py` & `ampel_core-0.9.1a0/ampel/aux/SimpleTagFilter.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/aux/filter/AbsLogicOperatorFilter.py` & `ampel_core-0.9.1a0/ampel/aux/filter/AbsLogicOperatorFilter.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/aux/filter/FlatDictArrayFilter.py` & `ampel_core-0.9.1a0/ampel/aux/filter/FlatDictArrayFilter.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/aux/filter/PrimitiveTypeArrayFilter.py` & `ampel_core-0.9.1a0/ampel/aux/filter/PrimitiveTypeArrayFilter.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/aux/filter/SimpleDictArrayFilter.py` & `ampel_core-0.9.1a0/ampel/aux/filter/SimpleDictArrayFilter.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/cli/AbsCoreCommand.py` & `ampel_core-0.9.1a0/ampel/cli/AbsCoreCommand.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # File:                Ampel-core/ampel/cli/AbsCoreCommand.py
 # License:             BSD-3-Clause
 # Author:              valery brinnel <firstname.lastname@gmail.com>
 # Date:                18.03.2021
 # Last Modified Date:  11.01.2023
 # Last Modified By:    valery brinnel <firstname.lastname@gmail.com>
 
+import json
 import re, os
 from typing import Any, TypeVar, Literal
 from collections.abc import Sequence, Iterator
 from ampel.config.AmpelConfig import AmpelConfig
 from ampel.abstract.AbsCLIOperation import AbsCLIOperation
 from ampel.core.AmpelContext import AmpelContext
 from ampel.core.UnitLoader import UnitLoader
@@ -57,15 +58,18 @@
 		if logger is None:
 			logger = AmpelLogger.get_logger()
 
 		if env_var_prefix is not None:
 			for var, value in os.environ.items():
 				if var.startswith(env_var_prefix):
 					k = var[len(env_var_prefix):]
-					v = _maybe_int(value)
+					try:
+						v = json.loads(value)
+					except json.JSONDecodeError:
+						v = value
 					logger.info(f"Setting config parameter '{k}' from environment")
 					set_by_path(ampel_conf._config, k, v)
 
 		for k, v in self.get_custom_args(unknown_args):
 
 			if ampel_conf.get(".".join(k.split(".")[:-1])) is None:
 				with out_stack():
```

### Comparing `ampel_core-0.9.0/ampel/cli/AbsLoadCommand.py` & `ampel_core-0.9.1a0/ampel/cli/AbsLoadCommand.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/cli/AbsStockCommand.py` & `ampel_core-0.9.1a0/ampel/cli/AbsStockCommand.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/cli/BufferCommand.py` & `ampel_core-0.9.1a0/ampel/cli/BufferCommand.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/cli/ConfigCommand.py` & `ampel_core-0.9.1a0/ampel/cli/ConfigCommand.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # License:             BSD-3-Clause
 # Author:              valery brinnel <firstname.lastname@gmail.com>
 # Date:                17.07.2021
 # Last Modified Date:  19.12.2022
 # Last Modified By:    valery brinnel <firstname.lastname@gmail.com>
 
 import os, subprocess, json, yaml, shutil
-from io import StringIO
+from io import StringIO, UnsupportedOperation
 from pathlib import Path
 from time import time
 from typing import Any, TextIO, Iterable
 from argparse import ArgumentParser, FileType
 from collections.abc import Sequence, Mapping
 
 from ampel.core.AmpelContext import AmpelContext
@@ -114,15 +114,15 @@
 		)
 		builder.opt('pretty', 'show', action='store_true')
 		builder.opt('stop-on-errors', 'build|install', default=2, type=int)
 		builder.opt('distributions', 'build|install', nargs="+", default=["pyampel-", "ampel-"])
 		builder.opt('exclude-distributions', 'build|install', nargs="+", default=[])
 		builder.opt('file', 'install|validate|transform', type=FileType('r'))
 		builder.opt('secrets', 'validate', type=FileType('r'))
-		builder.opt('out', 'transform', type=FileType('w'))
+		builder.opt('out', 'transform', type=FileType('a'))
 		builder.opt('filter', 'transform')
 		builder.opt('validate', 'transform', action='store_true')
 
 		# Example
 		builder.example('build', '-install')
 		builder.example('build', '-out ampel_conf.yaml')
 		builder.example('build', '-out ampel_conf.yaml -sign -verbose')
@@ -311,11 +311,17 @@
 
 			with StringIO() as output_yaml:
 				yaml.dump(config, output_yaml, sort_keys=False)
 				if args['validate']:
 					output_yaml.seek(0)
 					self._validate(output_yaml)
 				output_yaml.seek(0)
+				# truncate now, in case writing back to the input file
+				try:
+					args['out'].seek(0)
+					args['out'].truncate()
+				except UnsupportedOperation:
+					...
 				args['out'].write(output_yaml.read())
 
 		elif sub_op == 'validate':
 			self._validate(args['file'], args['secrets'])
```

### Comparing `ampel_core-0.9.0/ampel/cli/DBCommand.py` & `ampel_core-0.9.1a0/ampel/cli/DBCommand.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,22 +27,23 @@
 	'prefix': 'Prefix of the collections to delete (ex: AmpelTest)',
 	'config': 'Path to an ampel config file (yaml/json)',
 	'secrets': 'Path to a YAML secrets store in sops format',
 	'log-profile': 'One of: default, compact, headerless, verbose, debug',
 	'debug': 'debug',
 	'force': 'Delete potententially existing view before view creation',
 	'view': 'Create or discard collection views',
+	'index': 'Create or recreate collection indexes',
 }
 
 class DBCommand(AbsCoreCommand):
 
 
 	@staticmethod
 	def get_sub_ops() -> list[str]:
-		return ['import', 'export', 'delete', 'view']
+		return ['import', 'export', 'delete', 'view', 'index']
 
 
 	# Mandatory implementation
 	def get_parser(self, sub_op: None | str = None) -> ArgumentParser | AmpelArgumentParser:
 
 		if sub_op in self.parsers:
 			return self.parsers[sub_op]
@@ -75,16 +76,18 @@
 				{'name': 'channels-or', 'nargs': '+'},
 				{'name': 'channels-and', 'nargs': '+'}
 			]
 		)
 
 		# Optional
 		builder.opt('secrets')
+		builder.opt('one-db', default=False, action='store_true')
 		builder.opt('debug', action='store_true')
-		builder.opt('force', 'view', action='store_true')
+		builder.opt('force', 'view|index', action='store_true')
+		builder.opt('col', 'index', action='append')
 
 		builder.example('import', '-in /path/to/file')
 		builder.example('export', '-out /path/to/file')
 		builder.example('delete', '-mongo.prefix AmpelTest')
 		builder.example('view', '-create -channel CHAN1')
 		builder.example('view', '-create -channels-or CHAN1 CHAN2')
 		builder.example('view', '-discard -channel CHAN1')
@@ -98,28 +101,36 @@
 
 	# Mandatory implementation
 	def run(self, args: dict[str, Any], unknown_args: Sequence[str], sub_op: None | str = None) -> None:
 
 		if sub_op == 'delete':  # cosmetic mainly
 			AmpelDB.create_collection = (lambda x: None) # type: ignore
 
-		ctx: AmpelContext = self.get_context(args, unknown_args)
+		ctx: AmpelContext = self.get_context(args, unknown_args, one_db=args['one_db'], require_existing_db=sub_op != 'index')
 		db = ctx.db
 
 		logger = AmpelLogger.from_profile(
 			ctx, 'console_debug' if args['debug'] else 'console_info',
 			base_flag = LogFlag.MANUAL_RUN
 		)
 
 		if sub_op == 'delete':
 
 			logger.info(f'Deleting databases with prefix {ctx.db.prefix}')
 			ctx.db.drop_all_databases()
 			logger.info('Done')
 
+		elif sub_op == 'index':
+
+			for col_name, col_model in ctx.db.col_config.items():
+				if args['col'] and not col_name in args['col']:
+					continue
+				col = ctx.db.get_collection(col_name)
+				ctx.db.set_col_index(col, col_model, logger, force_overwrite=args['force'])
+
 		elif sub_op == 'view':
 
 			if 'create' not in args and 'discard' not in args:
 				logger.error('Either provide "create" or "discard" in combination with view command')
 				return
 
 			try:
```

### Comparing `ampel_core-0.9.0/ampel/cli/EventCommand.py` & `ampel_core-0.9.1a0/ampel/cli/EventCommand.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/cli/JobCommand.py` & `ampel_core-0.9.1a0/ampel/cli/JobCommand.py`

 * *Files 1% similar despite different names*

```diff
@@ -559,16 +559,16 @@
 	def load_tasks(self,
 		ctx: AmpelContext, job: JobModel, logger: AmpelLogger, debug: bool = False
 	) -> list[dict[str, Any]]:
 
 		jtasks: list[dict[str, Any]] = []
 		for i, model in enumerate(job.task):
 			if isinstance(model.template, Sequence):
-				taskd = apply_templates(ctx, model.template, model.dict(), logger)
-				del taskd['template']
+				taskd = apply_templates(ctx, model.template, model.dict(exclude_unset=True), logger)
+				taskd.pop('template', None)
 				if debug:
 					self.print_task(taskd, logger)
 			elif (
 				isinstance(model.template, dict) and
 				'pre' in model.template and model.template['pre']
 			):
 				taskd = apply_templates(ctx, model.template['pre'], model.dict(), logger)
```

### Comparing `ampel_core-0.9.0/ampel/cli/LogCommand.py` & `ampel_core-0.9.1a0/ampel/cli/LogCommand.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/cli/ProcessCommand.py` & `ampel_core-0.9.1a0/ampel/cli/ProcessCommand.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,32 +3,40 @@
 # File:                Ampel-core/ampel/cli/ProcessCommand.py
 # License:             BSD-3-Clause
 # Author:              jvs
 # Date:                Unspecified
 # Last Modified Date:  14.08.2022
 # Last Modified By:    jvs
 
-import signal, traceback, yaml
+from contextlib import contextmanager
+import json
+import signal, traceback, yaml, os
+from ampel.core.Schedulable import Schedulable
 from argparse import ArgumentParser
 from time import time
-from typing import Any, Optional, Sequence, Union
+from typing import Any, Generator, Optional, Sequence, Union
 
 from ampel.abstract.AbsEventUnit import AbsEventUnit
 from ampel.cli.AbsCoreCommand import AbsCoreCommand
 from ampel.cli.AmpelArgumentParser import AmpelArgumentParser
 from ampel.dev.DevAmpelContext import DevAmpelContext
 from ampel.log.AmpelLogger import AmpelLogger
 from ampel.log.LogFlag import LogFlag
+from ampel.metrics.AmpelMetricsRegistry import AmpelMetricsRegistry
 from ampel.model.ChannelModel import ChannelModel
 from ampel.model.UnitModel import UnitModel
 from ampel.util.freeze import recursive_freeze
+from ampel.core.EventHandler import EventHandler
+from ampel.struct.Resource import Resource
+
 
 def _handle_traceback(signal, frame):
     print(traceback.print_stack(frame))
 
+
 class ProcessCommand(AbsCoreCommand):
     """
     Runs a single process from a task definition (YAML file)
 
     A process is a single step of a Job (see JobCommand), with all templates resolved.
     """
 
@@ -47,42 +55,51 @@
         if self.parser:
             return self.parser
 
         parser = AmpelArgumentParser("process")
         parser.set_help_descr(
             {
                 "debug": "enable traceback printing",
+                "handle-exc": "record exceptions in the db",
                 "log-profile": "logging profile to use",
                 "config": "path to an ampel config file (yaml/json)",
                 "schema": "path to YAML job file",
-                "name": "process name",
+                "name": "task name",
+                "workflow": "parent workflow name",
                 "secrets": "path to a secret store; either SOPS YAML or mounted k8s Secret directory",
                 "db": "database to use",
                 "channel": "path to YAML channel file",
                 "alias": "path to YAML alias file",
             }
         )
 
         parser.req("config")
         parser.req("schema")
         parser.req("name")
         parser.req("db", type=str)
 
+        parser.opt("resources-in")
+        parser.opt("resources-out")
+
         parser.opt("channel")
         parser.opt("alias")
+        parser.opt("workflow", default=None, type=str)
         parser.opt("log-profile", default="prod")
         parser.opt("debug", default=False, action="store_true")
+        parser.opt("handle-exc", default=False, action="store_true")
         parser.opt("secrets", type=str)
 
         # Example
-        parser.example("process -config ampel_conf.yaml schema task_file.yaml -db processing -name taskytask")
+        parser.example(
+            "process -config ampel_conf.yaml schema task_file.yaml -db processing -name taskytask"
+        )
         return parser
 
-
-    def _get_context(self,
+    def _get_context(
+        self,
         args: dict[str, Any],
         unknown_args: Sequence[str],
         logger: AmpelLogger,
     ) -> DevAmpelContext:
 
         # DevAmpelContext hashes automatically confid from potential IngestDirectives
         ctx = super().get_context(
@@ -102,35 +119,52 @@
         # load channels if provided
         if args["channel"]:
             with open(args["channel"]) as f:
                 for c in yaml.safe_load(f):
                     chan = ChannelModel(**c)
                     logger.info(f"Registering job channel '{chan.channel}'")
                     dict.__setitem__(config_dict["channel"], str(chan.channel), c)
-        
+
         # load custom aliases if provided
         if args["alias"]:
             with open(args["alias"]) as f:
                 for k, v in yaml.safe_load(f).items():
                     if k not in ("t0", "t1", "t2", "t3"):
                         raise ValueError(f"Unrecognized alias: {k}")
                     if "alias" not in config_dict:
                         dict.__setitem__(config_dict, "alias", {})
                     for kk, vv in v.items():
                         logger.info(f"Registering job alias '{kk}'")
                         if k not in config_dict["alias"]:
                             dict.__setitem__(config_dict["alias"], k, {})
                         dict.__setitem__(config_dict["alias"][k], kk, vv)
-        
+
         ctx.config._config = recursive_freeze(config_dict)
-        
+
         return ctx
 
+    @contextmanager
+    def push_metrics(self, process_name: str, logger: AmpelLogger) -> Generator:
+        if not (pushgateway := os.environ.get("PROMETHEUS_PUSHGATEWAY")):
+            yield
+            return
+
+        task = Schedulable()
+        task.get_scheduler().every(30).seconds.do(
+            AmpelMetricsRegistry.push, pushgateway, process_name, reset=True
+        )
+        with task.run_in_thread():
+            yield
+        try:
+            task.get_scheduler().run_all()
+        except Exception as exc:
+            logger.error("Failed to push metrics", exc_info=exc)
 
-    def run(self,
+    def run(
+        self,
         args: dict[str, Any],
         unknown_args: Sequence[str],
         sub_op: Optional[str] = None,
     ) -> None:
 
         if args["debug"]:
             signal.signal(signal.SIGUSR1, _handle_traceback)
@@ -139,35 +173,59 @@
         logger = AmpelLogger.get_logger(base_flag=LogFlag.MANUAL_RUN)
 
         logger.info(f"Running task {args['name']}")
 
         with open(args["schema"], "r") as f:
             unit_model = UnitModel(**yaml.safe_load(f))
         # always raise exceptions
-        unit_model.override = (unit_model.override or {}) | {"raise_exc": True}
+        unit_model.override = (unit_model.override or {}) | {
+            "raise_exc": not args["handle_exc"]
+        }
 
         ctx = self._get_context(
             args,
             unknown_args,
             logger,
         )
 
+        if args["workflow"]:
+            process_name = f'{args["workflow"]}.{args["name"]}'
+        else:
+            process_name = args["name"]
+
+        if args["resources_in"]:
+            with open(args["resources_in"]) as f:
+                resources = {k: Resource(**v) for k, v in json.load(f).items()}
+        else:
+            resources = None
+
         proc = ctx.loader.new_context_unit(
             model=unit_model,
             context=ctx,
-            process_name=args["name"],
+            process_name=process_name,
             sub_type=AbsEventUnit,
             base_log_flag=LogFlag.MANUAL_RUN,
             log_profile=args["log_profile"],
         )
-        x = proc.run()
+        event_hdlr = EventHandler(
+            proc.process_name,
+            ctx.get_database(),
+            job_sig=proc.job_sig,
+            raise_exc=proc.raise_exc,
+            resources=resources,
+        )
+        with self.push_metrics(process_name, logger):
+            x = proc.run(event_hdlr=event_hdlr)
         logger.info(f"{unit_model.unit} return value: {x}")
 
+        if args["resources_out"]:
+            with open(args["resources_out"], "w") as f:
+                json.dump(
+                    {k: v.dict() for k, v in (event_hdlr.resources or {}).items()}, f
+                )
+
         dm = divmod(time() - start_time, 60)
         logger.info(
             "Task processing done. Time required: %s minutes %s seconds\n"
             % (round(dm[0]), round(dm[1]))
         )
         logger.flush()
-        # signal.signal(signal.SIGALRM, _handle_traceback)
-        # signal.alarm(1)
-        print("ProcessCommand.run() done; returning")
```

### Comparing `ampel_core-0.9.0/ampel/cli/RunCommand.py` & `ampel_core-0.9.1a0/ampel/cli/RunCommand.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/cli/StartCommand.py` & `ampel_core-0.9.1a0/ampel/cli/StartCommand.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/cli/T2Command.py` & `ampel_core-0.9.1a0/ampel/cli/T2Command.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 	"config": "Path to an ampel config file (yaml/json)",
 	"secrets": "Path to a YAML secrets store in sops format",
 	'out': 'Path to file were output will be written (printed to stdout otherwise)',
 	'db': 'Database prefix. If set, "-mongo.prefix" value will be ignored',
 	"unit": "Unit id/name",
 	"limit": "Limit number of returned documents",
 	"unit-config": "Unit config (integer number). Use string 'null' to match null",
-	"code": "T2 code (0: COMPLETED, -1: NEW)",
+	"code": "T2 code, given either as a name or integer (COMPLETED: 0, NEW: -1)",
 	"link": "T2 document link (hex)",
 	"stock": "Stock(s) associated with t2 doc (OR matched if multi-valued)",
 	'id-mapper': 'Convert stock ids using the provided id mapper (ex: ZTFIdMapper)',
 	"custom-match": "Custom mongodb match as JSON string (ex: {\"body.result.mychi2\": {\"$gt\": 1.0}})",
 	'no-resolve-stock': 'Keep stock as int when matching using id-mapper',
 	"resolve-config": "Translate 'config' field from int back to dict",
 	"human-times": "Translate timestamps to human-readable strings",
@@ -117,15 +117,18 @@
 		)
 
 		# Examples
 		for el in sub_ops:
 			p = f"ampel t2 {el} -config ampel_conf.yaml "
 			a = " -out /path/to/file" if el == "save" else ""
 			builder.example(el, '-unit T2SNCosmo -db AmpelTest', prepend=p, append=a)
-			builder.example(el, '-channel MY_CHANNEL -code -1', prepend=p, append=a)
+			if el.endswith("reset"):
+				builder.example(el, '-channel MY_CHANNEL -code T2_MISSING_DEPENDENCY TOO_MANY_TRIALS RUNNING', prepend=p, append=a)
+			else:
+				builder.example(el, '-channel MY_CHANNEL -code -1', prepend=p, append=a)
 			builder.example(el, '-stock 122621027 122620210 -unit DemoTiedLightCurveT2Unit', prepend=p, append=a)
 
 		builder.example(
 			'show|save',
 			'-db AmpelTest -human-times -stock ZTF20aaqubac -resolve-config -id-mapper ZTFIdMapper'
 		)
```

### Comparing `ampel_core-0.9.0/ampel/cli/T3BufferExporterStager.py` & `ampel_core-0.9.1a0/ampel/cli/T3BufferExporterStager.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/cli/T3BufferExporterUnit.py` & `ampel_core-0.9.1a0/ampel/cli/T3BufferExporterUnit.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/cli/ViewCommand.py` & `ampel_core-0.9.1a0/ampel/cli/ViewCommand.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/cli/export.py` & `ampel_core-0.9.1a0/ampel/cli/export.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/cli/utils.py` & `ampel_core-0.9.1a0/ampel/cli/utils.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/config/ScheduleEvaluator.py` & `ampel_core-0.9.1a0/ampel/config/ScheduleEvaluator.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/config/alter/HashT2Config.py` & `ampel_core-0.9.1a0/ampel/config/alter/HashT2Config.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/config/alter/ResolveRunTimeAliases.py` & `ampel_core-0.9.1a0/ampel/config/alter/ResolveRunTimeAliases.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/config/builder/BaseConfigChecker.py` & `ampel_core-0.9.1a0/ampel/config/builder/BaseConfigChecker.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/config/builder/ConfigBuilder.py` & `ampel_core-0.9.1a0/ampel/config/builder/ConfigBuilder.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/config/builder/ConfigChecker.py` & `ampel_core-0.9.1a0/ampel/config/builder/ConfigChecker.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/config/builder/ConfigValidator.py` & `ampel_core-0.9.1a0/ampel/config/builder/ConfigValidator.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/config/builder/DisplayOptions.py` & `ampel_core-0.9.1a0/ampel/config/builder/DisplayOptions.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/config/builder/DistConfigBuilder.py` & `ampel_core-0.9.1a0/ampel/config/builder/DistConfigBuilder.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/config/builder/FirstPassConfig.py` & `ampel_core-0.9.1a0/ampel/config/builder/FirstPassConfig.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/config/builder/ProcessMorpher.py` & `ampel_core-0.9.1a0/ampel/config/builder/ProcessMorpher.py`

 * *Files 0% similar despite different names*

```diff
@@ -269,15 +269,15 @@
 
 			if isinstance(conf, dict):
 
 				if override := d.get("override"):
 					conf |= override
 
 				if fqn := out_config['unit'][t2_unit].get('fqn'):
-					T2Unit = getattr(import_module(fqn), fqn.split('.')[-1])
+					T2Unit = getattr(import_module(fqn), t2_unit)
 					conf = T2Unit.validate(conf) # dictify ?
 				else:
 					self.logger.warn(
 						f"T2 unit {t2_unit} not installed locally. "
 						f"Building *unsafe* conf dict hash: "
 						f"changes in unit defaults between releases will go undetected",
 						extra=extra
```

### Comparing `ampel_core-0.9.0/ampel/config/builder/get_env.py` & `ampel_core-0.9.1a0/ampel/config/builder/get_env.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/config/collector/AbsDictConfigCollector.py` & `ampel_core-0.9.1a0/ampel/config/collector/AbsDictConfigCollector.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/config/collector/AbsForwardConfigCollector.py` & `ampel_core-0.9.1a0/ampel/config/collector/AbsForwardConfigCollector.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/config/collector/AbsListConfigCollector.py` & `ampel_core-0.9.1a0/ampel/config/collector/AbsListConfigCollector.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/config/collector/AliasConfigCollector.py` & `ampel_core-0.9.1a0/ampel/config/collector/AliasConfigCollector.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/config/collector/ChannelConfigCollector.py` & `ampel_core-0.9.1a0/ampel/config/collector/ChannelConfigCollector.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/config/collector/ConfigCollector.py` & `ampel_core-0.9.1a0/ampel/config/collector/ConfigCollector.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/config/collector/DBConfigCollector.py` & `ampel_core-0.9.1a0/ampel/config/collector/DBConfigCollector.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/config/collector/ForwardProcessConfigCollector.py` & `ampel_core-0.9.1a0/ampel/config/collector/ForwardProcessConfigCollector.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/config/collector/LoggingCollector.py` & `ampel_core-0.9.1a0/ampel/config/collector/LoggingCollector.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/config/collector/ProcessConfigCollector.py` & `ampel_core-0.9.1a0/ampel/config/collector/ProcessConfigCollector.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/config/collector/ResourceConfigCollector.py` & `ampel_core-0.9.1a0/ampel/config/collector/ResourceConfigCollector.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/config/collector/T02ConfigCollector.py` & `ampel_core-0.9.1a0/ampel/config/collector/T02ConfigCollector.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/config/collector/UnitConfigCollector.py` & `ampel_core-0.9.1a0/ampel/config/collector/UnitConfigCollector.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/core/AmpelContext.py` & `ampel_core-0.9.1a0/ampel/core/AmpelContext.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/core/AmpelController.py` & `ampel_core-0.9.1a0/ampel/core/AmpelController.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/core/AmpelDB.py` & `ampel_core-0.9.1a0/ampel/core/AmpelDB.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,18 +8,19 @@
 # Last Modified By  : vb <vbrinnel@physik.hu-berlin.de>
 
 import secrets, collections.abc
 from typing import Any, Literal
 from functools import cached_property
 from collections import defaultdict  # type: ignore[attr-defined]
 from collections.abc import Sequence
-from pymongo import MongoClient, ReadPreference
+from pymongo import MongoClient
 from pymongo.database import Database
 from pymongo.collection import Collection
 from pymongo.errors import ConfigurationError, DuplicateKeyError, OperationFailure, CollectionInvalid
+from pymongo.read_preferences import SecondaryPreferred
 
 from ampel.types import ChannelId
 from ampel.mongo.utils import get_ids
 from ampel.log.AmpelLogger import AmpelLogger
 from ampel.config.AmpelConfig import AmpelConfig
 from ampel.base.AmpelUnit import AmpelUnit
 from ampel.secret.AmpelVault import AmpelVault
@@ -54,14 +55,17 @@
 	mongo_options: MongoClientOptionsModel = MongoClientOptionsModel()
 	vault: None | AmpelVault
 	require_exists: bool = False
 	one_db: bool = False
 	#: Route reads to secondaries of a replica set. This can increase
 	#: performance at the expense of consistency
 	read_from_secondary: bool = True
+	#: Ignore secondary if it is more than max_staleness seconds behind the
+	#: primary
+	max_staleness: int = 300
 
 
 	@classmethod
 	def new(cls,
 		config: AmpelConfig,
 		vault: None | AmpelVault = None,
 		require_exists: bool | str = False,
@@ -122,15 +126,21 @@
 			for db_config in self.databases
 			for col in db_config.collections
 		}
 
 		self.mongo_collections: dict[str, dict[str, Collection]] = {}
 		self.mongo_clients: dict[str, MongoClient] = {} # map role with client
 
-		if self.require_exists and not self._get_pymongo_db("data", role="w").list_collection_names():
+		if (
+			self.require_exists
+			and not all(
+				self._get_pymongo_db(db.name, role=db.role.w).list_collection_names()
+				for db in self.databases
+			)
+		):
 			raise UnknownDatabase(f"Database(s) with prefix {self.prefix} do not exist")
 
 
 	@cached_property
 	def col_trace_ids(self) -> Collection:
 		return self.get_collection('trace')
 	
@@ -201,15 +211,15 @@
 				...
 			except OperationFailure as exc:
 				# also raised when collection was created concurrently
 				if exc.code != 48: # NamespaceExists
 					raise
 		self.mongo_collections[col_name][mode] = db.get_collection(
 			col_name,
-			read_preference=ReadPreference.SECONDARY_PREFERRED if self.read_from_secondary else None
+			read_preference=SecondaryPreferred(max_staleness=self.max_staleness) if self.read_from_secondary else None
 		)
 
 		return self.mongo_collections[col_name][mode]
 
 
 	def _get_pymongo_db(self, db_name: str, *, role: str) -> Database:
 		"""
@@ -338,19 +348,19 @@
 		col: Collection,
 		index_data: IndexModel | ShortIndexModel,
 		logger: 'AmpelLogger'
 	) -> None:
 
 		try:
 			idx_params = index_data.dict(exclude_unset=True)
-			logger.info(f"  Creating index: {idx_params}")
+			logger.info(f"  Creating index for {col.database.name}.{col.name}: {idx_params}")
 			col.create_index(idx_params['index'], **idx_params.get('args', {}))
 		except Exception as e:
 			logger.error(
-				f"Index creation failed for '{col.name}' (args: {idx_params})",
+				f"Index creation failed for '{col.database.name}.{col.name}': (args: {idx_params})",
 				exc_info=e
 			)
 
 
 	def create_one_view(self,
 		channel: ChannelId,
 		logger: 'None | AmpelLogger' = None,
@@ -397,15 +407,16 @@
 	def create_view(self,
 		view: AbsMongoView,
 		col_prefix: str,
 		logger: 'None | AmpelLogger' = None,
 		force: bool = False
 	) -> None:
 
-		db = self._get_pymongo_db("data", role="w")
+		db_conf = self._get_db_config("stock")
+		db = self._get_pymongo_db(db_conf.name, role=db_conf.role.w)
 		if force:
 			col_names = db.list_collection_names()
 
 		for el in ("stock", "t0", "t1", "t2", "t3"):
 
 			agg = getattr(view, el)()
 
@@ -438,15 +449,16 @@
 		if not isinstance(channels, collections.abc.Sequence) or len(channels) == 1:
 			raise ValueError("Incorrect argument")
 		self.delete_view("_AND_".join(map(str, channels)), logger)
 
 
 	def delete_view(self, view_prefix: str, logger: 'None | AmpelLogger' = None) -> None:
 
-		db = self._get_pymongo_db("data", role="w")
+		db_conf = self._get_db_config("stock")
+		db = self._get_pymongo_db(db_conf.name, role=db_conf.role.w)
 		for el in ("stock", "t0", "t1", "t2", "t3"):
 			db.drop_collection(f'{view_prefix}_{el}')
 
 
 	def __repr__(self) -> str:
 		return "<AmpelDB>"
```

### Comparing `ampel_core-0.9.0/ampel/core/AmpelRegister.py` & `ampel_core-0.9.1a0/ampel/core/AmpelRegister.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/core/ContextUnit.py` & `ampel_core-0.9.1a0/ampel/core/ContextUnit.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/core/DataLoader.py` & `ampel_core-0.9.1a0/ampel/core/DataLoader.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/core/DefaultProcessController.py` & `ampel_core-0.9.1a0/ampel/core/DefaultProcessController.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/core/DocBuilder.py` & `ampel_core-0.9.1a0/ampel/core/DocBuilder.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from ampel.base.AmpelUnit import AmpelUnit
 from ampel.struct.UnitResult import UnitResult
 from ampel.content.T3Document import T3Document
 from ampel.content.T4Document import T4Document
 from ampel.content.MetaRecord import MetaRecord
 from ampel.enum.DocumentCode import DocumentCode
 from ampel.enum.MetaActionCode import MetaActionCode
+from ampel.model.UnitModel import UnitModel
 from ampel.util.tag import merge_tags
 from ampel.util.hash import build_unsafe_dict_id
 
 T = TypeVar("T", T3Document, T4Document)
 
 
 class DocBuilder(ContextUnit):
@@ -46,15 +47,33 @@
 
 	#: Used if human_timestamp is true
 	human_timestamp_format: str = "%Y-%m-%d %H:%M:%S.%f"
 
 
 	def __init__(self, **kwargs) -> None:
 		super().__init__(**kwargs)
-		self.adapters: dict[str, AbsUnitResultAdapter] = {}
+		self.adapters: dict[int, AbsUnitResultAdapter] = {}
+
+
+	def get_adapter_instance(self, model: UnitModel, event_hdlr: EventHandler) -> AbsUnitResultAdapter:
+		config_id = build_unsafe_dict_id(model.dict())
+
+		if (
+			config_id not in self.adapters or
+			self.adapters[config_id].run_id != event_hdlr.get_run_id()
+		):
+			unit_instance = self.context.loader.new_context_unit(
+				model = model,
+				context = self.context,
+				run_id = event_hdlr.get_run_id(),
+				sub_type = AbsUnitResultAdapter,
+			)
+			self.adapters[config_id] = unit_instance
+
+		return self.adapters[config_id]
 
 	
 	def craft_doc(self,
 		event_hdlr: EventHandler,
 		unit: AmpelUnit,
 		res: None | UBson | UnitResult,
 		ts: float,
@@ -111,21 +130,16 @@
 				else:
 					d['tag'] = res.tag
 			elif self.tag:
 				d['tag'] = self.tag
 
 			if res.body:
 
-				if res.adapter:
-					if res.adapter not in self.adapters:
-						self.adapters[res.adapter] = getattr(
-							import_module(f"ampel.core.adapter.{res.adapter}"),
-							res.adapter
-						)(context=self.context, run_id=event_hdlr.get_run_id())
-					res = self.adapters[res.adapter].handle(res)
+				if res.adapter_model:
+					res = self.get_adapter_instance(res.adapter_model, event_hdlr).handle(res)
 
 				d['body'] = res.body
 				actact |= MetaActionCode.ADD_BODY
 
 		else:
 
 			if self.tag:
```

### Comparing `ampel_core-0.9.0/ampel/core/EventHandler.py` & `ampel_core-0.9.1a0/ampel/core/EventHandler.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/core/Schedulable.py` & `ampel_core-0.9.1a0/ampel/core/Schedulable.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/core/UnitLoader.py` & `ampel_core-0.9.1a0/ampel/core/UnitLoader.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/demo/DemoFirstPointT2Unit.py` & `ampel_core-0.9.1a0/ampel/demo/DemoFirstPointT2Unit.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/demo/DemoPointT2Unit.py` & `ampel_core-0.9.1a0/ampel/demo/DemoPointT2Unit.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/demo/DemoProcessor.py` & `ampel_core-0.9.1a0/ampel/demo/DemoProcessor.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/demo/DemoT3Unit.py` & `ampel_core-0.9.1a0/ampel/demo/DemoT3Unit.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/demo/DemoT4RunTimeAliasGenerator.py` & `ampel_core-0.9.1a0/ampel/demo/DemoT4RunTimeAliasGenerator.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/dev/DevAmpelContext.py` & `ampel_core-0.9.1a0/ampel/dev/DevAmpelContext.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/dev/NoShaper.py` & `ampel_core-0.9.1a0/ampel/dev/NoShaper.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/ingest/ChainedIngestionHandler.py` & `ampel_core-0.9.1a0/ampel/ingest/ChainedIngestionHandler.py`

 * *Files 0% similar despite different names*

```diff
@@ -480,163 +480,162 @@
 		"""
 		Create database documents.
 		:param filter_results: the value returned from
 		  :func:`~ampel.abstract.AbsAlertFilter.AbsAlertFilter.process` if alert was accepted
 		:param jm_extra: extra info to be added to journal or meta enties. Ex: {'alert_id': 123}
 		"""
 
-		self.updates_buffer._block_autopush = True
-		ingest_start = time()
+		with self.updates_buffer.group_updates():
+			ingest_start = time()
 
-		# process *modifies* dict instances loaded by fastavro
-		dps: list[DataPoint] = self.shaper.process(alert_dps, stock_id)
+			# process *modifies* dict instances loaded by fastavro
+			dps: list[DataPoint] = self.shaper.process(alert_dps, stock_id)
 
-		if not dps: # Not sure if this can happen
-			return
+			if not dps: # Not sure if this can happen
+				return
 
-		add_other_tag: None | MetaActivity = {'action': MetaActionCode.ADD_OTHER_TAG, 'tag': tag} if tag else None
+			add_other_tag: None | MetaActivity = {'action': MetaActionCode.ADD_OTHER_TAG, 'tag': tag} if tag else None
 
-		# Set of chans (last parameter) is used for logging
-		mux_cache: dict[AbsT0Muxer, tuple[None | list[DataPoint], None | list[DataPoint], set[ChannelId]]] = {}
-		t1_comb_cache: T1CombineCache = {}
-		t1_comp_cache: T1ComputeCache = {}
+			# Set of chans (last parameter) is used for logging
+			mux_cache: dict[AbsT0Muxer, tuple[None | list[DataPoint], None | list[DataPoint], set[ChannelId]]] = {}
+			t1_comb_cache: T1CombineCache = {}
+			t1_comp_cache: T1ComputeCache = {}
 
-		# ingestion blocks
-		ibs = self.iblocks
+			# ingestion blocks
+			ibs = self.iblocks
 
-		for i, fres in filter_results:
+			for i, fres in filter_results:
 
-			# Add alert and shaper version info to stock journal entry
-			jentry: dict[str, Any] = {
-				'action': JournalActionCode.STOCK_ADD_CHANNEL | JournalActionCode.STOCK_BUMP_UPD,
-				'traceid': self.base_trace_id | {'shaper': self.shaper_trace_id}
-			}
+				# Add alert and shaper version info to stock journal entry
+				jentry: dict[str, Any] = {
+					'action': JournalActionCode.STOCK_ADD_CHANNEL | JournalActionCode.STOCK_BUMP_UPD,
+					'traceid': self.base_trace_id | {'shaper': self.shaper_trace_id}
+				}
 
-			if jm_extra:
-				jentry = jm_extra | jentry
+				if jm_extra:
+					jentry = jm_extra | jentry
 
-			if i > 0: # Known stock (for the current channel)
-				ib = ibs[i][0]
-			else: # New stock
-				ib = ibs[-i][1]
+				if i > 0: # Known stock (for the current channel)
+					ib = ibs[i][0]
+				else: # New stock
+					ib = ibs[-i][1]
 
-			# Muxer requested
-			if mux := ib.mux:
+				# Muxer requested
+				if mux := ib.mux:
 
-				# Add muxer version info to stock journal entry
-				jentry['traceid']['muxer'] = mux.trace_id
+					# Add muxer version info to stock journal entry
+					jentry['traceid']['muxer'] = mux.trace_id
 
-				# Potentially load previous results from cache
-				if mux.unit in mux_cache:
-					dps_insert, dps_combine, s = mux_cache[mux.unit]
-					s.add(ib.channel)
-				else:
-					dps_insert, dps_combine = mux.unit.process(dps, stock_id)
-					mux_cache[mux.unit] = dps_insert, dps_combine, {ib.channel}
+					# Potentially load previous results from cache
+					if mux.unit in mux_cache:
+						dps_insert, dps_combine, s = mux_cache[mux.unit]
+						s.add(ib.channel)
+					else:
+						dps_insert, dps_combine = mux.unit.process(dps, stock_id)
+						mux_cache[mux.unit] = dps_insert, dps_combine, {ib.channel}
 
-				if dps_combine:
+					if dps_combine:
 
-					if x := [
-						dp for dp in dps_combine
-						if 'channel' in dp and ib.channel not in dp['channel']
-					]:
-						dps_insert = (dps_insert + x) if dps_insert else x
-
-				if dps_insert:
-
-					self.t0_compiler.add(dps_insert, ib.channel, self.shaper_trace_id, jm_extra)
-
-					# TODO: make this addition optional (a stock with a million dps would create pblms)
-					jentry['upsert'] = [el['id'] for el in dps_insert]
-					jentry['action'] |= JournalActionCode.T0_ADD_CHANNEL
-
-					if mux.point_t2:
-						jentry['action'] |= JournalActionCode.T2_ADD_CHANNEL
-						self.ingest_point_t2s(
-							dps_insert, fres, stock_id, ib.channel, mux.point_t2, add_other_tag,
-							jm_extra if self.include_extra_meta > 1 else None
+						if x := [
+							dp for dp in dps_combine
+							if 'channel' in dp and ib.channel not in dp['channel']
+						]:
+							dps_insert = (dps_insert + x) if dps_insert else x
+
+					if dps_insert:
+
+						self.t0_compiler.add(dps_insert, ib.channel, self.shaper_trace_id, jm_extra)
+
+						# TODO: make this addition optional (a stock with a million dps would create pblms)
+						jentry['upsert'] = [el['id'] for el in dps_insert]
+						jentry['action'] |= JournalActionCode.T0_ADD_CHANNEL
+
+						if mux.point_t2:
+							jentry['action'] |= JournalActionCode.T2_ADD_CHANNEL
+							self.ingest_point_t2s(
+								dps_insert, fres, stock_id, ib.channel, mux.point_t2, add_other_tag,
+								jm_extra if self.include_extra_meta > 1 else None
+							)
+
+					# Muxed T1 and associated T2 ingestions
+					if dps_combine and mux.combine:
+						self.ingest_t12(
+							dps_combine, fres, stock_id, jentry, mux.combine,
+							t1_comb_cache, t1_comp_cache, add_other_tag,
+							jm_extra if self.include_extra_meta else None
 						)
 
-				# Muxed T1 and associated T2 ingestions
-				if dps_combine and mux.combine:
+				else:
+					self.t0_compiler.add(dps, ib.channel, self.shaper_trace_id)
+
+				# Non-muxed T1 and associated T2 ingestions
+				if ib.combine:
 					self.ingest_t12(
-						dps_combine, fres, stock_id, jentry, mux.combine,
-						t1_comb_cache, t1_comp_cache, add_other_tag,
-						jm_extra if self.include_extra_meta else None
+						dps, fres, stock_id, jentry, ib.combine, t1_comb_cache, t1_comp_cache,
+						add_other_tag, meta_extra = jm_extra if self.include_extra_meta else None
+					)
+					
+				# Non-muxed point T2s
+				if ib.point_t2:
+					self.ingest_point_t2s(
+						dps, fres, stock_id, ib.channel, ib.point_t2, add_other_tag,
+						jm_extra if self.include_extra_meta > 1 else None
 					)
 
-			else:
-				self.t0_compiler.add(dps, ib.channel, self.shaper_trace_id)
-
-			# Non-muxed T1 and associated T2 ingestions
-			if ib.combine:
-				self.ingest_t12(
-					dps, fres, stock_id, jentry, ib.combine, t1_comb_cache, t1_comp_cache,
-					add_other_tag, meta_extra = jm_extra if self.include_extra_meta else None
-				)
-				
-			# Non-muxed point T2s
-			if ib.point_t2:
-				self.ingest_point_t2s(
-					dps, fres, stock_id, ib.channel, ib.point_t2, add_other_tag,
-					jm_extra if self.include_extra_meta > 1 else None
-				)
+				# Stock T2s
+				if ib.stock_t2:
+					for t2b in ib.stock_t2:
+						self.stock_t2_compiler.add(
+							t2b.unit, t2b.config, stock_id, stock_id,
+							ib.channel, self.base_trace_id, add_other_tag,
+							jm_extra if self.include_extra_meta else None
+						)
 
-			# Stock T2s
-			if ib.stock_t2:
-				for t2b in ib.stock_t2:
-					self.stock_t2_compiler.add(
-						t2b.unit, t2b.config, stock_id, stock_id,
-						ib.channel, self.base_trace_id, add_other_tag,
-						jm_extra if self.include_extra_meta else None
-					)
+				# Flush potential unit logs
+				###########################
 
-			# Flush potential unit logs
-			###########################
+				logger = self.logger
+				for muxer, (_, _, chans) in mux_cache.items():
+					if muxer._buf_hdlr.buffer: # type: ignore[attr-defined]
+						muxer._buf_hdlr.forward( # type: ignore[attr-defined]
+							logger, stock=stock_id, channel=list(chans), extra = jm_extra
+						)
 
-			logger = self.logger
-			for muxer, (_, _, chans) in mux_cache.items():
-				if muxer._buf_hdlr.buffer: # type: ignore[attr-defined]
-					muxer._buf_hdlr.forward( # type: ignore[attr-defined]
-						logger, stock=stock_id, channel=list(chans), extra = jm_extra
-					)
+				for (t1_unit, _), (_, chans) in t1_comb_cache.items():
+					if t1_unit._buf_hdlr.buffer: # type: ignore[union-attr]
+						t1_unit._buf_hdlr.forward( # type: ignore[union-attr]
+							logger, stock=stock_id, channel=list(chans), extra = jm_extra
+						)
 
-			for (t1_unit, _), (_, chans) in t1_comb_cache.items():
-				if t1_unit._buf_hdlr.buffer: # type: ignore[union-attr]
-					t1_unit._buf_hdlr.forward( # type: ignore[union-attr]
-						logger, stock=stock_id, channel=list(chans), extra = jm_extra
+				if not self.stock_compiler.register:
+					self.stock_compiler.add(
+						stock_id, ib.channel, journal = jentry, # type: ignore[arg-type]
+						tag = add_other_tag['tag'] if add_other_tag else None # type: ignore[arg-type]
 					)
 
-			if not self.stock_compiler.register:
-				self.stock_compiler.add(
-					stock_id, ib.channel, journal = jentry, # type: ignore[arg-type]
-					tag = add_other_tag['tag'] if add_other_tag else None # type: ignore[arg-type]
-				)
-
-		# Commit
-		########
-		now = int(time()) if self.int_time else time()
+			# Commit
+			########
+			now = int(time()) if self.int_time else time()
 
-		self.t0_compiler.commit(self.t0_ingester, now)
+			self.t0_compiler.commit(self.t0_ingester, now)
 
-		if self.t1_compiler.t1s:
-			self.t1_compiler.commit(self.t1_ingester, now)
+			if self.t1_compiler.t1s:
+				self.t1_compiler.commit(self.t1_ingester, now)
 
-		if self.stock_t2_compiler.t2s:
-			self.stock_t2_compiler.commit(self.t2_ingester, now)
+			if self.stock_t2_compiler.t2s:
+				self.stock_t2_compiler.commit(self.t2_ingester, now)
 
-		if self.point_t2_compiler.t2s:
-			self.point_t2_compiler.commit(self.t2_ingester, now)
+			if self.point_t2_compiler.t2s:
+				self.point_t2_compiler.commit(self.t2_ingester, now)
 
-		if self.state_t2_compiler.t2s:
-			self.state_t2_compiler.commit(self.t2_ingester, now)
+			if self.state_t2_compiler.t2s:
+				self.state_t2_compiler.commit(self.t2_ingester, now)
 
-		self.stock_compiler.commit(self.stock_ingester, now, body=stock_body)
-		self.ingest_stats.append(time() - ingest_start)
-		self.updates_buffer._block_autopush = False
+			self.stock_compiler.commit(self.stock_ingester, now, body=stock_body)
+			self.ingest_stats.append(time() - ingest_start)
 
 
 	def ingest_point_t2s(self,
 		dps: list[DataPoint],
 		fres: bool | int,
 		stock_id: StockId,
 		channel: ChannelId,
@@ -743,15 +742,16 @@
 						code = DocumentCode.OK
 						macts[0]['action'] |= MetaActionCode.SET_CODE
 				else:
 					t1_dps = tres
 					code = DocumentCode.OK
 					macts[0]['action'] |= MetaActionCode.SET_CODE
 
-				if excl := [el['id'] for el in dps if el['id'] not in t1_dps]:
+				t1_dps_set = set(t1_dps)
+				if excl := [el['id'] for el in dps if el['id'] not in t1_dps_set]:
 					macts[0]['action'] |= MetaActionCode.ADD_T1_EXCL
 					macts[0]['excl'] = excl
 
 				je = jentry.copy()
 				je['traceid'] = jentry['traceid'].copy()
 				je['traceid']['combiner'] = t1b.trace_id
```

### Comparing `ampel_core-0.9.0/ampel/ingest/ChainedT0Muxer.py` & `ampel_core-0.9.1a0/ampel/ingest/ChainedT0Muxer.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/ingest/StockCompiler.py` & `ampel_core-0.9.1a0/ampel/ingest/StockCompiler.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/ingest/T0Compiler.py` & `ampel_core-0.9.1a0/ampel/ingest/T0Compiler.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/ingest/T1Compiler.py` & `ampel_core-0.9.1a0/ampel/ingest/T1Compiler.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/ingest/T2Compiler.py` & `ampel_core-0.9.1a0/ampel/ingest/T2Compiler.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/log/AmpelLogger.py` & `ampel_core-0.9.1a0/ampel/log/AmpelLogger.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/log/LightLogRecord.py` & `ampel_core-0.9.1a0/ampel/log/LightLogRecord.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/log/LogFlag.py` & `ampel_core-0.9.1a0/ampel/log/LogFlag.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/log/LoggingErrorReporter.py` & `ampel_core-0.9.1a0/ampel/log/LoggingErrorReporter.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/log/LogsDumper.py` & `ampel_core-0.9.1a0/ampel/log/LogsDumper.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/log/handlers/AmpelStreamHandler.py` & `ampel_core-0.9.1a0/ampel/log/handlers/AmpelStreamHandler.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/log/handlers/ChanRecordBufHandler.py` & `ampel_core-0.9.1a0/ampel/log/handlers/ChanRecordBufHandler.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/log/handlers/DefaultRecordBufferingHandler.py` & `ampel_core-0.9.1a0/ampel/log/handlers/DefaultRecordBufferingHandler.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/log/handlers/EnclosedChanRecordBufHandler.py` & `ampel_core-0.9.1a0/ampel/log/handlers/EnclosedChanRecordBufHandler.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/log/handlers/RecordBufferingHandler.py` & `ampel_core-0.9.1a0/ampel/log/handlers/RecordBufferingHandler.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/log/utils.py` & `ampel_core-0.9.1a0/ampel/log/utils.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/metrics/AmpelDBCollector.py` & `ampel_core-0.9.1a0/ampel/metrics/AmpelDBCollector.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/metrics/AmpelProcessCollector.py` & `ampel_core-0.9.1a0/ampel/metrics/AmpelProcessCollector.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/metrics/prometheus.py` & `ampel_core-0.9.1a0/ampel/metrics/prometheus.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/model/ChannelModel.py` & `ampel_core-0.9.1a0/ampel/model/ChannelModel.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/model/ProcessModel.py` & `ampel_core-0.9.1a0/ampel/model/ProcessModel.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/model/aux/AuxAliasableModel.py` & `ampel_core-0.9.1a0/ampel/model/aux/AuxAliasableModel.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/model/aux/FilterCriterion.py` & `ampel_core-0.9.1a0/ampel/model/aux/FilterCriterion.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/model/builder/BuilderAliasModel.py` & `ampel_core-0.9.1a0/ampel/model/builder/BuilderAliasModel.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/model/builder/RemoteUnitDefinition.py` & `ampel_core-0.9.1a0/ampel/model/builder/RemoteUnitDefinition.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/model/ingest/CompilerOptions.py` & `ampel_core-0.9.1a0/ampel/model/ingest/CompilerOptions.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/model/ingest/DualIngestDirective.py` & `ampel_core-0.9.1a0/ampel/model/ingest/DualIngestDirective.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/model/ingest/FilterModel.py` & `ampel_core-0.9.1a0/ampel/model/ingest/FilterModel.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/model/ingest/IngestBody.py` & `ampel_core-0.9.1a0/ampel/model/ingest/IngestBody.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/model/ingest/IngestDirective.py` & `ampel_core-0.9.1a0/ampel/model/ingest/IngestDirective.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/model/ingest/MuxModel.py` & `ampel_core-0.9.1a0/ampel/model/ingest/MuxModel.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/model/ingest/T1Combine.py` & `ampel_core-0.9.1a0/ampel/model/ingest/T1Combine.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/model/ingest/T1CombineCompute.py` & `ampel_core-0.9.1a0/ampel/model/ingest/T1CombineCompute.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/model/ingest/T1CombineComputeNow.py` & `ampel_core-0.9.1a0/ampel/model/ingest/T1CombineComputeNow.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/model/ingest/T2Compute.py` & `ampel_core-0.9.1a0/ampel/model/ingest/T2Compute.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/model/job/JobModel.py` & `ampel_core-0.9.1a0/ampel/model/job/JobModel.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/model/job/JobTaskModel.py` & `ampel_core-0.9.1a0/ampel/model/job/JobTaskModel.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/model/purge/PurgeContentModel.py` & `ampel_core-0.9.1a0/ampel/model/purge/PurgeContentModel.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/model/purge/PurgeLogsModel.py` & `ampel_core-0.9.1a0/ampel/model/purge/PurgeLogsModel.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/model/purge/PurgeModel.py` & `ampel_core-0.9.1a0/ampel/model/purge/PurgeModel.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/model/t3/AliasableModel.py` & `ampel_core-0.9.1a0/ampel/model/t3/AliasableModel.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/model/t3/LoaderDirective.py` & `ampel_core-0.9.1a0/ampel/model/t3/LoaderDirective.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/model/t3/QueryMatchModel.py` & `ampel_core-0.9.1a0/ampel/model/t3/QueryMatchModel.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/model/t3/T2FilterModel.py` & `ampel_core-0.9.1a0/ampel/model/t3/T2FilterModel.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/model/t3/T3IncludeDirective.py` & `ampel_core-0.9.1a0/ampel/model/t3/T3IncludeDirective.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/model/t3/T3ProjectionDirective.py` & `ampel_core-0.9.1a0/ampel/model/t3/T3ProjectionDirective.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/model/time/QueryTimeModel.py` & `ampel_core-0.9.1a0/ampel/model/time/QueryTimeModel.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/model/time/TimeConstraintModel.py` & `ampel_core-0.9.1a0/ampel/model/time/TimeConstraintModel.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/model/time/TimeDeltaModel.py` & `ampel_core-0.9.1a0/ampel/model/time/TimeDeltaModel.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/model/time/TimeLastRunModel.py` & `ampel_core-0.9.1a0/ampel/model/time/TimeLastRunModel.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/model/time/TimeStringModel.py` & `ampel_core-0.9.1a0/ampel/model/time/TimeStringModel.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/model/time/UnixTimeModel.py` & `ampel_core-0.9.1a0/ampel/model/time/UnixTimeModel.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/mongo/model/AmpelColModel.py` & `ampel_core-0.9.1a0/ampel/mongo/model/AmpelColModel.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/mongo/model/AmpelDBModel.py` & `ampel_core-0.9.1a0/ampel/mongo/model/AmpelDBModel.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/mongo/model/FieldModel.py` & `ampel_core-0.9.1a0/ampel/mongo/model/FieldModel.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/mongo/model/IndexModel.py` & `ampel_core-0.9.1a0/ampel/mongo/model/IndexModel.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/mongo/model/MongoClientOptionsModel.py` & `ampel_core-0.9.1a0/ampel/mongo/model/MongoClientOptionsModel.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/mongo/model/ShortIndexModel.py` & `ampel_core-0.9.1a0/ampel/mongo/model/ShortIndexModel.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/mongo/purge/MongoStockDeleter.py` & `ampel_core-0.9.1a0/ampel/mongo/purge/MongoStockDeleter.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/mongo/query/general.py` & `ampel_core-0.9.1a0/ampel/mongo/query/general.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/mongo/query/stock.py` & `ampel_core-0.9.1a0/ampel/mongo/query/stock.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/mongo/query/t1.py` & `ampel_core-0.9.1a0/ampel/mongo/query/t1.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/mongo/query/t2.py` & `ampel_core-0.9.1a0/ampel/mongo/query/t2.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/mongo/query/var/LogsLoader.py` & `ampel_core-0.9.1a0/ampel/mongo/query/var/LogsLoader.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/mongo/query/var/LogsMatcher.py` & `ampel_core-0.9.1a0/ampel/mongo/query/var/LogsMatcher.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/mongo/query/var/events.py` & `ampel_core-0.9.1a0/ampel/mongo/query/var/events.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/mongo/schema.py` & `ampel_core-0.9.1a0/ampel/mongo/schema.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/mongo/update/DBUpdatesBuffer.py` & `ampel_core-0.9.1a0/ampel/mongo/update/DBUpdatesBuffer.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,16 +9,17 @@
 
 from time import time
 from math import inf
 from multiprocessing.pool import ThreadPool
 from pymongo.errors import BulkWriteError
 from pymongo.collection import Collection
 from pymongo import UpdateOne, InsertOne, UpdateMany
-from typing import Any, Literal, Union, Mapping
-from collections.abc import Callable, Iterable
+from typing import Any, Generator, Literal, Union, Mapping
+from collections.abc import Callable, Iterable, Iterator
+from contextlib import contextmanager
 
 from ampel.core.Schedulable import Schedulable
 from ampel.log.utils import report_exception, report_error, convert_dollars
 from ampel.log.AmpelLogger import AmpelLogger
 from ampel.core.AmpelDB import AmpelDB, intcol
 from ampel.metrics.AmpelMetricsRegistry import AmpelMetricsRegistry
 
@@ -83,23 +84,25 @@
 	"""
 
 	def __init__(self,
 		ampel_db: AmpelDB,
 		run_id: int | list[int],
 		logger: AmpelLogger,
 		error_callback: None | Callable[[], None] = None,
+		acknowledge_callback: None | Callable[[Iterator[Any]], None] = None,
 		catch_signals: bool = True,
 		log_doc_ids: None | Iterable[int] = None,
-		push_interval: None | float = 3.,
+		push_interval: None | int = 3,
 		max_size: None | int = None,
 		threads: None | int = None,
 		raise_exc: bool = False
 	):
 		"""
 		:param error_callback: callback method to be called on errors
+		:param acknowledge_callback: method to call to acknowledge processing of a message bunch
 		:param catch_signals: see Schedulable docstring
 		:param log_doc_ids: logs inserted/updated document IDs for the given collections.
 		Collection integer identifiers are: 't0' -> 0, 't1' -> 1, 't2' -> 2, 'stock' -> 3.
 		Thus, if you want to activate this behavior for all collections, use log_doc_ids=[0, 1, 2, 3].
 		Notes: 1) it this will significantly increase the log size/amount.
 		2) the "_id" of T2 documents is generated server-side and bulk_write does not return it,
 		so it is not avail 'as is'. We instead log the natching filter (t2id, config, link)
@@ -113,14 +116,15 @@
 		was yet noticed using a meaningful value such as 4 (OSX, python 3.8.1). Since bulk_write drops the GIL,
 		a multithreading-like effect already occurs without the specific use a threads.
 		"""
 
 		Schedulable.__init__(self, catch_signals=catch_signals)
 		self._new_buffer()
 		self.error_callback = error_callback
+		self.acknowledge_callback = acknowledge_callback
 
 		self._cols: dict[AmpelMainCol, Collection] = {
 			col_name: ampel_db.get_collection(col_name)
 			for col_name in self.db_ops.keys()
 		}
 
 		self.stats: dict[AmpelMainCol, int] = {
@@ -134,49 +138,57 @@
 		self.max_size = max_size
 		self.log_doc_ids = set(log_doc_ids) if log_doc_ids else None
 
 		self._autopush_asap = False
 		self._block_autopush = False
 		self._last_update = time()
 
+		self.push_interval = push_interval
 		if push_interval:
-			self.push_interval = push_interval
 			self.get_scheduler() \
 				.every(push_interval) \
 				.seconds \
 				.do(self.request_autopush)
 
 			self._job = self.get_scheduler().jobs[0]
-		else:
-			self.push_interval = inf
 
 		self.thread_pool = ThreadPool(threads) if threads else None
 
 		self.raise_exc = raise_exc
 
 
 	def _new_buffer(self) -> None:
 		""" Creates new buffer for pymongo operations """
 
 		# total number of updates (of all kinds/collections)
 		self.db_ops: dict[AmpelMainCol, list[DBOp]] = {
 			't2': [], 't0': [], 'stock': [], 't1': []
 		}
+		self._messages_to_ack: set[Any] = set()
 
 
 	def stop(self) -> None:
 
 		super().stop()
 		self.push_updates(force=True)
 
 		if self.thread_pool:
 			self.thread_pool.close()
 			self.thread_pool.join()
 
 
+	def acknowledge_on_push(self, message: Any) -> None:
+		"""
+		Add a message to be passed to acknowledge_callback when the current
+		buffer has been pushed
+		"""
+		if self.acknowledge_callback:
+			self._messages_to_ack.add(message)
+
+
 	def add_updates(self, updates: dict[AmpelMainCol, list[DBOp]]) -> None:
 		"""
 		:raises: KeyError if dict key is unknown (known keys: stock, t0, t1, t2)
 		"""
 		for k, v in updates.items():
 			self.db_ops[k] += v
 
@@ -203,18 +215,31 @@
 		self.db_ops['t2'].append(update)
 
 
 	def add_stock_update(self, update: DBOp) -> None:
 		self.db_ops['stock'].append(update)
 
 
+	@contextmanager
+	def group_updates(self) -> Generator:
+		"""
+		Ensure that updates issued in this context are grouped together
+		"""
+		block_autopush = self._block_autopush
+		self._block_autopush = True
+		try:
+			yield
+		finally:
+			self._block_autopush = block_autopush
+
+
 	def request_autopush(self) -> None:
 
 		t = time()
-		if t - self._last_update > self.push_interval:
+		if self.push_interval is None or t - self._last_update > self.push_interval:
 			if self._block_autopush:
 				self._autopush_asap = True
 			else:
 				self.push_updates()
 
 
 	def check_push(self) -> None:
@@ -250,25 +275,34 @@
 		self._last_update = time()
 		if self._autopush_asap:
 			self._autopush_asap = False
 			self._job._schedule_next_run()
 
 		# Reference instance buffer locally before creating a new one
 		db_ops = self.db_ops
+		messages = self._messages_to_ack
 		self._new_buffer()
 
 		for col_name in db_ops.keys():
 			if db_ops[col_name]:
 				if self.thread_pool:
 					self.thread_pool.starmap(
 						self.call_bulk_write, ([col_name, db_ops[col_name]], )
 					)
 				else:
 					self.call_bulk_write(col_name, db_ops[col_name])
 
+		if self.acknowledge_callback and messages:
+			try:
+				self.acknowledge_callback(iter(messages))
+			except Exception as exc:
+				if self.raise_exc:
+					raise
+				report_exception(self._ampel_db, self.logger, exc=exc)
+
 
 	def call_bulk_write(self, col_name: AmpelMainCol, db_ops: list, *, extra: None | dict = None) -> None:
 		"""
 		:param col_name: Ampel DB collection name (ex: stock, t0, t1, t2)
 		:param db_ops: list of pymongo operations
 		:raises: None, but stops the AlertConsumer processing by using the method
 		cancel_run() when unrecoverable exceptions occur.
```

### Comparing `ampel_core-0.9.0/ampel/mongo/update/MongoStockIngester.py` & `ampel_core-0.9.1a0/ampel/mongo/update/MongoStockIngester.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/mongo/update/MongoStockUpdater.py` & `ampel_core-0.9.1a0/ampel/mongo/update/MongoStockUpdater.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # Last Modified By:    valery brinnel <firstname.lastname@gmail.com>
 
 from time import time
 from bson import ObjectId
 from pymongo.errors import BulkWriteError
 from pymongo.operations import UpdateMany, UpdateOne
 from typing import Any, Literal, get_args
-from collections.abc import Sequence
+from collections.abc import Sequence, Mapping
 
 from ampel.core.AmpelDB import AmpelDB
 from ampel.types import ChannelId, Tag, StockId
 from ampel.log import AmpelLogger, VERBOSE
 from ampel.log.utils import report_exception
 from ampel.mongo.utils import maybe_use_each
 from ampel.enum.JournalActionCode import JournalActionCode
@@ -221,21 +221,23 @@
 					self._multi_updates[s] = [um]
 
 			self._updates.append(um)
 			if self.auto_flush and len(self._updates) > self.auto_flush:
 				self.flush()
 
 
-	def _merge_updates(self, op: UpdateOne, d: dict) -> None:
+	def _merge_updates(self, op: UpdateOne, d: Mapping[str, Any] | Sequence[Mapping[str, Any]]) -> None:
 		"""
 		modifies provided UpdateOne structure
 		:raises: ValueError in case update structures are not conform ex: {'$addToSet': {'name': {'a': 1}}}
 		"""
 
 		opd = op._doc
+		assert isinstance(d, Mapping)
+		assert isinstance(opd, dict)
 
 		if '$max' in d:
 			if '$max' in opd:
 				for k in d['$max']:
 					if k in opd['$max']:
 						opd['$max'][k] = max(opd['$max'][k], d['$max'][k])
 					else:
```

### Comparing `ampel_core-0.9.0/ampel/mongo/update/MongoT0Ingester.py` & `ampel_core-0.9.1a0/ampel/mongo/update/MongoT0Ingester.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/mongo/update/MongoT1Ingester.py` & `ampel_core-0.9.1a0/ampel/mongo/update/MongoT1Ingester.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/mongo/update/MongoT2Ingester.py` & `ampel_core-0.9.1a0/ampel/mongo/update/MongoT2Ingester.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/mongo/update/MongoT3Ingester.py` & `ampel_core-0.9.1a0/ampel/mongo/update/MongoT3Ingester.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/mongo/update/var/DBLoggingHandler.py` & `ampel_core-0.9.1a0/ampel/mongo/update/var/DBLoggingHandler.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/mongo/utils.py` & `ampel_core-0.9.1a0/ampel/mongo/utils.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/mongo/view/AbsMongoFlatMultiView.py` & `ampel_core-0.9.1a0/ampel/mongo/view/AbsMongoFlatMultiView.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/mongo/view/AbsMongoView.py` & `ampel_core-0.9.1a0/ampel/mongo/view/AbsMongoView.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/mongo/view/FrozenValuesDict.py` & `ampel_core-0.9.1a0/ampel/mongo/view/FrozenValuesDict.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/mongo/view/MongoAndView.py` & `ampel_core-0.9.1a0/ampel/mongo/view/MongoAndView.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/mongo/view/MongoOneView.py` & `ampel_core-0.9.1a0/ampel/mongo/view/MongoOneView.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/mongo/view/MongoOrView.py` & `ampel_core-0.9.1a0/ampel/mongo/view/MongoOrView.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/ops/AmpelExceptionPublisher.py` & `ampel_core-0.9.1a0/ampel/ops/AmpelExceptionPublisher.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/ops/OpsProcessor.py` & `ampel_core-0.9.1a0/ampel/ops/OpsProcessor.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/run/server.py` & `ampel_core-0.9.1a0/ampel/run/server.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/secret/AESecretProvider.py` & `ampel_core-0.9.1a0/ampel/secret/AESecretProvider.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/secret/DictSecretProvider.py` & `ampel_core-0.9.1a0/ampel/secret/DictSecretProvider.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/secret/DirSecretProvider.py` & `ampel_core-0.9.1a0/ampel/secret/DirSecretProvider.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/secret/PotemkinSecretProvider.py` & `ampel_core-0.9.1a0/ampel/secret/PotemkinSecretProvider.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/t1/T1SimpleCombiner.py` & `ampel_core-0.9.1a0/ampel/t1/T1SimpleCombiner.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/t1/T1SimpleRetroCombiner.py` & `ampel_core-0.9.1a0/ampel/t1/T1SimpleRetroCombiner.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/t2/T2Utils.py` & `ampel_core-0.9.1a0/ampel/t2/T2Utils.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/t2/T2Worker.py` & `ampel_core-0.9.1a0/ampel/t2/T2Worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,27 +51,28 @@
 ]
 
 abs_t2 = (
 	AbsStockT2Unit, AbsPointT2Unit, AbsStateT2Unit, AbsTiedPointT2Unit,
 	AbsTiedStateT2Unit, AbsCustomStateT2Unit, AbsTiedCustomStateT2Unit
 )
 
-stat_latency, stat_count = register_stats(tier=2)
+stat_latency, stat_count, stat_time = register_stats(tier=2)
 
 class BackoffConfig(AmpelBaseModel):
 	code_match: Sequence[int] = [
 		DocumentCode.T2_PENDING_DEPENDENCY, # input t2 doc has not yet resolved
 		DocumentCode.T2_MISSING_DEPENDENCY, # input t2 docs not found
 		DocumentCode.T2_UNKNOWN_LINK, # input t1 doc not found
 		DocumentCode.T2_MISSING_INFO, # t0 docs not found
 	]
 	base: float = 2
 	factor: float = 1
 	jitter: bool = True
 
+DOCUMENT_CODES: dict[int, str] = {v: k for k,v in DocumentCode.__members__.items()}
 
 class T2Worker(AbsWorker[T2Document]):
 	"""
 	Fill results into pending :class:`T2 documents <ampel.content.T2Document.T2Document>`.
 	"""
 
 	#: process only those :class:`T2 documents <ampel.content.T2Document.T2Document>`
@@ -130,33 +131,41 @@
 		doc: T2Document,
 		stock_updr: MongoStockUpdater,
 		logger: AmpelLogger
 	) -> tuple[UBson, int]:
 
 		before_run = time()
 
-		t2_unit = self.get_unit_instance(doc, logger)
+		try:
+			t2_unit = self.get_unit_instance(doc, logger)
+
+			if not isinstance(t2_unit, abs_t2):
+				raise ValueError(f"Unsupported unit: {doc['unit']}")
+
+		except Exception as e:
+
+			if self.raise_exc:
+				raise
 
-		if not isinstance(t2_unit, abs_t2):
-			raise ValueError(f"Unsupported unit: {doc['unit']}")
+			self._processing_error(
+				logger, doc, None, exception=e, msg='Could not instantiate unit',
+				meta = self.gen_meta(stock_updr.run_id, None, 0)
+			)
+
+			return None, DocumentCode.EXCEPTION
 
 		if (trials := self._get_trials(doc)) <= self.max_try:
-			ret = self.run_t2_unit(t2_unit, doc, logger, stock_updr)
+			with stat_time.labels(doc["unit"], "run").time():
+				ret = self.run_t2_unit(t2_unit, doc, logger, stock_updr)
 		else:
 			ret = UnitResult(code=DocumentCode.TOO_MANY_TRIALS)
 
 		# Used as timestamp and to compute duration below (using before_run)
 		now = time()
 
-		# _id is an ObjectId, but declared as bytes in ampel-interface to avoid
-		# an explicit dependency on pymongo
-		if doc['meta']: # robustify against manual changes of the db
-			stat_latency.labels(doc['unit']).observe(now - doc['meta'][0]['ts'])
-		stat_count.labels(doc['unit']).inc()
-		self._doc_counter += 1
 		body = None
 		tag = None
 		code = 0
 
 		try:
 
 			# New (channel-less) journal entry for the associated stock document
@@ -183,21 +192,16 @@
 
 			# The channel-less activity of this t2 worker
 			activity = meta['activity'][0]
 
 			# Unit requested customizations
 			if isinstance(ret, UnitResult):
 
-				if ret.adapter:
-					if ret.adapter not in self._adapters:
-						self._adapters[ret.adapter] = getattr(
-							import_module(f"ampel.core.adapter.{ret.adapter}"),
-							ret.adapter
-						)(context=self.context, run_id=stock_updr.run_id)
-					ret = self._adapters[ret.adapter].handle(ret)
+				if ret.adapter_model:
+					ret = self.get_adapter_instance(ret.adapter_model).handle(ret)
 
 				if ret.body:
 					body = ret.body
 					activity['action'] |= MetaActionCode.ADD_BODY
 					jrec['action'] |= JournalActionCode.T2_ADD_BODY
 
 				if ret.tag:
@@ -223,15 +227,15 @@
 					logger.info(
 						f'T2 unit {t2_unit.__class__.__name__} returned document '
 						f'code: {code} ({DocumentCode(code).name})',
 						extra={'unit': doc['unit'], 'stock': doc['stock']}
 					)
 
 				if ret.journal:
-					jrec.update(ret.journal) # type: ignore
+					ret.journal.into(jrec)
 					activity['action'] |= MetaActionCode.EXTRA_JOURNAL
 					jrec['action'] |= JournalActionCode.T2_EXTRA_JOURNAL
 
 			# Unit returned bson-like content
 			elif isinstance(ret, ubson):
 				body = ret
 				activity['action'] |= MetaActionCode.ADD_BODY
@@ -242,32 +246,40 @@
 				code = DocumentCode.ERROR
 				self._processing_error(
 					logger, doc, None, meta, extra={'ret': ret},
 					msg='Invalid content returned by T2 unit'
 				)
 
 			meta['code'] = code
-			self.commit_update(
-				{'_id': doc['_id']}, # type: ignore[typeddict-item]
-				meta, logger, body=body, tag=tag, code=code
-			)
+			with stat_time.labels(doc["unit"], "commit_update").time():
+				self.commit_update(
+					{'_id': doc['_id']}, # type: ignore[typeddict-item]
+					meta, logger, body=body, tag=tag, code=code
+				)
 
 			# Update stock document
 			if len(stock_updr._updates) >= self.updates_buffer_size:
 				stock_updr.flush()
 
 		except Exception as e:
 
 			if self.raise_exc:
 				raise e
 
 			self._processing_error(
 				logger, doc, None, exception=e, msg='An exception occured',
 				meta = self.gen_meta(stock_updr.run_id, t2_unit._trace_id, round(now - before_run, 3))
 			)
+			code = DocumentCode.EXCEPTION
+
+		# _id is an ObjectId, but declared as bytes in ampel-interface to avoid
+		# an explicit dependency on pymongo
+		if doc['meta']: # robustify against manual changes of the db
+			stat_latency.labels(doc['unit']).observe(now - doc['meta'][0]['ts'])
+		stat_count.labels(doc['unit'], DOCUMENT_CODES.get(code, 'unknown')).inc()
 
 		return body, code
 
 
 	# NB: spell out union arg to ensure a common context for the TypeVar T
 	def load_input_docs(self,
 		t2_unit: AbsT2, t2_doc: T2Document, logger: AmpelLogger, stock_updr: MongoStockUpdater
@@ -305,19 +317,20 @@
 				AbsStateT2Unit,
 				AbsCustomStateT2Unit,
 				AbsTiedStateT2Unit,
 				AbsTiedCustomStateT2Unit
 			)
 		):
 			dps: list[DataPoint] = []
-			t1_doc: None | T1Document = next(
-				self.col_t1.find(
-					{'stock': t2_doc['stock'], 'link': t2_doc['link']}
-				), None
-			)
+			with stat_time.labels(t2_doc["unit"], "load_t1").time():
+				t1_doc: None | T1Document = next(
+					self.col_t1.find(
+						{'stock': t2_doc['stock'], 'link': t2_doc['link']}
+					), None
+				)
 
 			# compound doc must exist (None could mean an ingester bug)
 			if t1_doc is None:
 				if not self._is_retriable(t2_doc, DocumentCode.T2_UNKNOWN_LINK):
 					report_error(
 						self._ampel_db, msg='T1Document not found', logger=logger,
 						info={'id': t2_doc['link'], 'doc': t2_doc}
@@ -327,18 +340,19 @@
 			# Datarights: suppress channel info (T3 uses instead a
 			# 'projection' procedure that should not be necessary here)
 			t1_doc.pop('channel') # type: ignore[misc]
 
 			t1_dps_ids = list(t1_doc['dps'])
 
 			# Sort DPS from DB in the same order than referenced by 'dps' from t1 doc
-			dps = sorted(
-				self.col_t0.find({'id': {'$in': t1_dps_ids}}),
-				key = lambda dp: t1_dps_ids.index(dp['id'])
-			)
+			with stat_time.labels(t2_doc["unit"], "load_t0").time():
+				dps = sorted(
+					self.col_t0.find({'id': {'$in': t1_dps_ids}}),
+					key = lambda dp: t1_dps_ids.index(dp['id'])
+				)
 
 			# Should never happen (only in case of ingestion bug)
 			if not dps:
 				if not self._is_retriable(t2_doc, DocumentCode.T2_MISSING_INFO):
 					report_error(
 						self._ampel_db, msg='Datapoints not found',
 						logger=logger, info={'t1': t1_doc, 't2': t2_doc}
@@ -398,15 +412,16 @@
 									extra={'recipient': t2_doc['unit'], 'stock': t2_doc['stock']}
 								)
 						else:
 							d['link'] = maybe_match_array(t1_dps_ids)
 
 					queries.append(d)
 
-				qres = self.run_tied_queries(queries, t2_doc, stock_updr, logger)
+				with stat_time.labels(t2_doc["unit"], "load_tied").time():
+					qres = self.run_tied_queries(queries, t2_doc, stock_updr, logger)
 
 				# Dependency missing
 				if isinstance(qres, UnitResult):
 					return qres
 
 				if isinstance(t2_unit, AbsTiedStateT2Unit):
 					return t1_doc, dps, qres
@@ -646,15 +661,16 @@
 			return UnitResult(code=DocumentCode.INTERNAL_ERROR)
 
 		if isinstance(args, UnitResult):
 			return args
 
 		try:
 
-			ret = t2_unit.process(*args)
+			with stat_time.labels(t2_doc["unit"], "process").time():
+				ret = t2_unit.process(*args)
 
 			if t2_unit._buf_hdlr.buffer: # type: ignore[union-attr]
 				t2_unit._buf_hdlr.forward( # type: ignore[union-attr]
 					logger, stock=t2_doc['stock']
 				)
 
 			return ret
```

### Comparing `ampel_core-0.9.0/ampel/t3/README.md` & `ampel_core-0.9.1a0/ampel/t3/README.md`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/t3/T3Processor.py` & `ampel_core-0.9.1a0/ampel/t3/T3Processor.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/t3/include/session/T3SessionAlertsNumber.py` & `ampel_core-0.9.1a0/ampel/t3/include/session/T3SessionAlertsNumber.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/t3/include/session/T3SessionLastRunTime.py` & `ampel_core-0.9.1a0/ampel/t3/include/session/T3SessionLastRunTime.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/t3/stage/BaseViewGenerator.py` & `ampel_core-0.9.1a0/ampel/t3/stage/BaseViewGenerator.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/t3/stage/NoViewGenerator.py` & `ampel_core-0.9.1a0/ampel/t3/stage/NoViewGenerator.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/t3/stage/README.md` & `ampel_core-0.9.1a0/ampel/t3/stage/README.md`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/t3/stage/SimpleViewGenerator.py` & `ampel_core-0.9.1a0/ampel/t3/stage/SimpleViewGenerator.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/t3/stage/T3AdaptativeStager.py` & `ampel_core-0.9.1a0/ampel/t3/stage/T3AdaptativeStager.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/t3/stage/T3AggregatingStager.py` & `ampel_core-0.9.1a0/ampel/t3/stage/T3AggregatingStager.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/t3/stage/T3BaseStager.py` & `ampel_core-0.9.1a0/ampel/t3/stage/T3BaseStager.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,14 @@
 	#: Note that if True, a T3 document will be created even if a t3 unit returns None
 	save_stock_ids: bool = False
 
 
 	def __init__(self, **kwargs) -> None:
 
 		super().__init__(**kwargs)
-		self.adapters: dict[str, AbsUnitResultAdapter] = {}
 		self.stock_updr = MongoStockUpdater(
 			ampel_db = self.context.db,
 			tier = 3,
 			run_id = self.event_hdlr.get_run_id(),
 			process_name = self.event_hdlr.process_name,
 			logger = self.logger,
 			raise_exc = self.event_hdlr.raise_exc,
```

### Comparing `ampel_core-0.9.0/ampel/t3/stage/T3ChannelStager.py` & `ampel_core-0.9.1a0/ampel/t3/stage/T3ChannelStager.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/t3/stage/T3DistributiveStager.py` & `ampel_core-0.9.1a0/ampel/t3/stage/T3DistributiveStager.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/t3/stage/T3ProjectingStager.py` & `ampel_core-0.9.1a0/ampel/t3/stage/T3ProjectingStager.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/t3/stage/T3SequentialStager.py` & `ampel_core-0.9.1a0/ampel/t3/stage/T3SequentialStager.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/t3/stage/T3SimpleStager.py` & `ampel_core-0.9.1a0/ampel/t3/stage/T3SimpleStager.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/t3/stage/T3ThreadedStager.py` & `ampel_core-0.9.1a0/ampel/t3/stage/T3ThreadedStager.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/t3/stage/ThreadedViewGenerator.py` & `ampel_core-0.9.1a0/ampel/t3/stage/ThreadedViewGenerator.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/t3/stage/filter/T3AmpelBufferFilter.py` & `ampel_core-0.9.1a0/ampel/t3/stage/filter/T3AmpelBufferFilter.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/t3/stage/project/T3BaseProjector.py` & `ampel_core-0.9.1a0/ampel/t3/stage/project/T3BaseProjector.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/t3/stage/project/T3ChannelProjector.py` & `ampel_core-0.9.1a0/ampel/t3/stage/project/T3ChannelProjector.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/t3/supply/SimpleT2BasedSupplier.py` & `ampel_core-0.9.1a0/ampel/t3/supply/SimpleT2BasedSupplier.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/t3/supply/T3DefaultBufferSupplier.py` & `ampel_core-0.9.1a0/ampel/t3/supply/T3DefaultBufferSupplier.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/t3/supply/complement/T3ExtJournalAppender.py` & `ampel_core-0.9.1a0/ampel/t3/supply/complement/T3ExtJournalAppender.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/t3/supply/complement/T3LogsAppender.py` & `ampel_core-0.9.1a0/ampel/t3/supply/complement/T3LogsAppender.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/t3/supply/complement/T3RandIntAppender.py` & `ampel_core-0.9.1a0/ampel/t3/supply/complement/T3RandIntAppender.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/t3/supply/load/T3LatestStateDataLoader.py` & `ampel_core-0.9.1a0/ampel/t3/supply/load/T3LatestStateDataLoader.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/t3/supply/load/T3SimpleDataLoader.py` & `ampel_core-0.9.1a0/ampel/t3/supply/load/T3SimpleDataLoader.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/t3/supply/select/T3FilteringStockSelector.py` & `ampel_core-0.9.1a0/ampel/t3/supply/select/T3FilteringStockSelector.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/t3/supply/select/T3StockSelector.py` & `ampel_core-0.9.1a0/ampel/t3/supply/select/T3StockSelector.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/t3/unit/T3LogAggregatedStocks.py` & `ampel_core-0.9.1a0/ampel/t3/unit/T3LogAggregatedStocks.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/t4/T4Processor.py` & `ampel_core-0.9.1a0/ampel/t4/T4Processor.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/t4/T4RunTimeContextUpdater.py` & `ampel_core-0.9.1a0/ampel/t4/T4RunTimeContextUpdater.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/template/ChannelWithProcsTemplate.py` & `ampel_core-0.9.1a0/ampel/template/ChannelWithProcsTemplate.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/template/PeriodicSummaryT3.py` & `ampel_core-0.9.1a0/ampel/template/PeriodicSummaryT3.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/test/conftest.py` & `ampel_core-0.9.1a0/ampel/test/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -138,29 +138,37 @@
     assert integration_context.db.get_collection("stock").count_documents({}) == 1
 
 
 @pytest.fixture
 def ingest_stock_t2(integration_context: DevAmpelContext, ampel_logger):
     run_id = 0
     updates_buffer = DBUpdatesBuffer(integration_context.db, run_id=run_id, logger=ampel_logger)
-    ingester = MongoT2Ingester(
-        updates_buffer=updates_buffer,
-    )
     stock_id = "stockystock"
-    compiler = T2Compiler(run_id=run_id, tier=2)
-    compiler.add(
+    now = datetime.datetime.now().timestamp()
+    t2_compiler = T2Compiler(run_id=run_id, tier=2)
+    t2_compiler.add(
         unit="DummyStockT2Unit",
         config=None,
         stock=stock_id,
         link=stock_id,
         channel="TEST_CHANNEL",
         traceid={},
     )
-    compiler.commit(ingester, datetime.datetime.now().timestamp())
-    ingester.updates_buffer.push_updates()
+    t2_compiler.commit(
+        MongoT2Ingester(updates_buffer=updates_buffer), now
+    )
+    
+    stock_compiler = StockCompiler(run_id=run_id, tier=2)
+    stock_compiler.add(stock_id, "TEST_CHANNEL", {"tier": 2})
+    stock_compiler.commit(
+        MongoStockIngester(updates_buffer=updates_buffer), now
+    )
+    
+    updates_buffer.push_updates()
+    assert integration_context.db.get_collection("stock").count_documents({}) == 1
     assert integration_context.db.get_collection("t2").count_documents({}) == 1
 
     integration_context.register_unit(DummyStockT2Unit)
 
 
 @pytest.fixture(params=["DummyStateT2Unit", "DummyPointT2Unit", "DummyStockT2Unit"])
 def ingest_tied_t2(integration_context: DevAmpelContext, ampel_logger, request):
```

### Comparing `ampel_core-0.9.0/ampel/test/dummy.py` & `ampel_core-0.9.1a0/ampel/test/dummy.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 
 from ampel.content.DataPoint import DataPoint
 from ampel.content.T1Document import T1Document
 from ampel.view.T2DocView import T2DocView
 from ampel.model.StateT2Dependency import StateT2Dependency
 from ampel.abstract.AbsT0Muxer import AbsT0Muxer
 from ampel.model.ingest.CompilerOptions import CompilerOptions
+from ampel.struct.Resource import Resource
 
 
 class Sleepy(AbsEventUnit):
     """
     A processor that does nothing (especially not touching the db, which is not
     mocked in subprocesses)
     """
@@ -128,14 +129,31 @@
     value: str
     expected_value: str
 
     def proceed(self, event_hdlr: EventHandler) -> Any:
         assert self.value == self.expected_value
 
 
+class DummyResourceInputUnit(DummyInputUnit):
+
+    # add an extra level of indirection via resources
+    def proceed(self, event_hdlr: EventHandler) -> Any:
+        assert event_hdlr.resources
+        assert event_hdlr.resources[self.value].value == self.expected_value
+
+
+class DummyResourceOutputUnit(AbsEventUnit):
+
+    name: str
+    value: str
+
+    def proceed(self, event_hdlr: EventHandler) -> Any:
+        event_hdlr.add_resource(Resource(name=self.name, value=self.value))
+
+
 class DummyProcessorTemplate(AbsConfigMorpher):
 
     value: str
     expected_value: str
 
     def morph(self, config: dict[str, Any], logger: AmpelLogger) -> dict[str, Any]:
         return {'unit': "DummyInputUnit", 'config': self.dict(exclude={'template'})}
```

### Comparing `ampel_core-0.9.0/ampel/test/pylintrc` & `ampel_core-0.9.1a0/ampel/test/pylintrc`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/test/test-data/ZTF20abxvcrk.pkl` & `ampel_core-0.9.1a0/ampel/test/test-data/ZTF20abxvcrk.pkl`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/test/test-data/testing-config.yaml` & `ampel_core-0.9.1a0/ampel/test/test-data/testing-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -599,23 +599,24 @@
     base:
       - AbsEventUnit
   DummyOutputUnit:
     fqn: ampel.test.dummy
     version: 0.8.0a1
     base:
       - AbsEventUnit
-  DemoT3Unit:
-    fqn: ampel.demo.DemoT3Unit
-    version: 0.8.2a2
+  DummyResourceInputUnit:
+    fqn: ampel.test.dummy
+    version: 0.8.0a1
     base:
-    - DemoT3Unit
-    - AbsT3Unit
-    - LogicalUnit
-    distrib: ampel-core
-    file: /Users/jakob/Documents/ZTF/Ampel-v0.8/Ampel-core/conf/ampel-cor
+      - AbsEventUnit
+  DummyResourceOutputUnit:
+    fqn: ampel.test.dummy
+    version: 0.8.0a1
+    base:
+      - AbsEventUnit
 process:
   t0: {}
   t1: {}
   t2: {}
   t3: {}
   ops: {}
 alias:
```

### Comparing `ampel_core-0.9.0/ampel/test/test_AbsChannelTemplate.py` & `ampel_core-0.9.1a0/ampel/test/test_AbsChannelTemplate.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/test/test_AmpelContext.py` & `ampel_core-0.9.1a0/ampel/test/test_AmpelContext.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/test/test_DBUpdatesBuffer.py` & `ampel_core-0.9.1a0/ampel/test/test_DBUpdatesBuffer.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/test/test_DefaultProcessController.py` & `ampel_core-0.9.1a0/ampel/test/test_DefaultProcessController.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/test/test_IngestionHandler.py` & `ampel_core-0.9.1a0/ampel/test/test_IngestionHandler.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/test/test_JobCommand.py` & `ampel_core-0.9.1a0/ampel/test/test_JobCommand.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/test/test_PeriodicSummaryT3.py` & `ampel_core-0.9.1a0/ampel/test/test_PeriodicSummaryT3.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/test/test_ProcessMorpher.py` & `ampel_core-0.9.1a0/ampel/test/test_ProcessMorpher.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/test/test_SimpleTagFilter.py` & `ampel_core-0.9.1a0/ampel/test/test_SimpleTagFilter.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/test/test_T2Processor.py` & `ampel_core-0.9.1a0/ampel/test/test_T2Processor.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,28 +36,29 @@
     t2 = T2Worker(context=integration_context, raise_exc=True, process_name="t2")
 
     stats = {}
     with collect_diff(stats):
         assert t2.run() == 1
 
     assert (
-        stats[("ampel_t2_docs_processed_total", (("unit", "DummyStockT2Unit"),))] == 1
+        stats[("ampel_t2_docs_processed_total", (("unit", "DummyStockT2Unit"), ('code', 'OK')))] == 1
     )
     assert stats[("ampel_t2_latency_seconds_sum", (("unit", "DummyStockT2Unit"),))] > 0
 
 
-def test_error_reporting(integration_context: DevAmpelContext):
+@pytest.mark.parametrize("config", [None, {"raise_exc": True}])
+def test_error_reporting(integration_context: DevAmpelContext, config):
     integration_context.register_unit(DummyPointT2Unit)
     # DummyPointT2Unit will raise an error on the malformed T0 doc
     integration_context.db.get_collection("t0").insert_one({"id": 42})
     channels = ["channel_a", "channel_b"]
     doc: T2Document = {
         "unit": "DummyPointT2Unit",
         "code": DocumentCode.NEW,
-        "config": None,
+        "config": config,
         "col": "t0",
         "stock": 42,
         "link": 42,
         "channel": channels,
         "meta": [
             {"ts": 0, "tier": 2}
         ],
@@ -65,15 +66,19 @@
     }
     integration_context.db.get_collection("t2").insert_one(doc) # type: ignore[arg-type]
     t2 = T2Worker(context=integration_context, raise_exc=False, process_name="t2", run_dependent_t2s=True)
     assert t2.run() == 1
     assert (doc := integration_context.db.get_collection("t2").find_one({})) # type: ignore[assignment]
     assert doc["code"] == DocumentCode.EXCEPTION
     assert (trouble := integration_context.db.get_collection('trouble').find_one({}))
-    assert trouble["channel"] == channels
+    if config is None:
+        assert trouble["channel"] == channels
+        assert trouble.get("msg") is None
+    else:
+        assert trouble["extra"]["msg"] == "Could not instantiate unit"
 
 
 def test_tied_t2s(integration_context, ingest_tied_t2):
     assert (num_dps := integration_context.db.get_collection("t0").count_documents({}))
     t2 = T2Worker(
         context=integration_context, raise_exc=True, process_name="t2", run_dependent_t2s=True
     )
```

### Comparing `ampel_core-0.9.0/ampel/test/test_T3ChannelProjector.py` & `ampel_core-0.9.1a0/ampel/test/test_T3ChannelProjector.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/test/test_T3FilteringStockSelector.py` & `ampel_core-0.9.1a0/ampel/test/test_T3FilteringStockSelector.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/test/test_T3Processor.py` & `ampel_core-0.9.1a0/ampel/test/test_T3Processor.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/test/test_T3SimpleDataLoader.py` & `ampel_core-0.9.1a0/ampel/test/test_T3SimpleDataLoader.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/test/test_UnitLoader.py` & `ampel_core-0.9.1a0/ampel/test/test_UnitLoader.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/test/test_concurrent.py` & `ampel_core-0.9.1a0/ampel/test/test_concurrent.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/test/test_config.py` & `ampel_core-0.9.1a0/ampel/test/test_config.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/test/test_server.py` & `ampel_core-0.9.1a0/ampel/test/test_server.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/test/test_util_mappings.py` & `ampel_core-0.9.1a0/ampel/test/test_util_mappings.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/test/test_util_template.py` & `ampel_core-0.9.1a0/ampel/test/test_util_template.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/util/collections.py` & `ampel_core-0.9.1a0/ampel/util/collections.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/util/concurrent.py` & `ampel_core-0.9.1a0/ampel/util/concurrent.py`

 * *Files 2% similar despite different names*

```diff
@@ -192,14 +192,16 @@
 
         try:
             async with parent_w.open() as tx:
                 tx.write(fp.getbuffer())
                 await tx.drain()
 
             async with parent_r.open() as rx:
+                exitcode: int | BaseException
+                payload: bytes | BaseException
                 try:
                     exitcode, payload = await asyncio.gather(
                         proc.wait(), rx.read(), return_exceptions=True
                     )
                     if isinstance(exitcode, BaseException):
                         raise exitcode
                     elif exitcode < 0:
```

### Comparing `ampel_core-0.9.0/ampel/util/config.py` & `ampel_core-0.9.1a0/ampel/util/config.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/util/debug.py` & `ampel_core-0.9.1a0/ampel/util/debug.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/util/distrib.py` & `ampel_core-0.9.1a0/ampel/util/distrib.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/util/getch.py` & `ampel_core-0.9.1a0/ampel/util/getch.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/util/logicschema.py` & `ampel_core-0.9.1a0/ampel/util/logicschema.py`

 * *Files 0% similar despite different names*

```diff
@@ -182,18 +182,18 @@
 	elif isinstance(arg, dict):
 		v = arg
 
 	else:
 		raise ValueError("Unsupported arg type: %s" % type(arg))
 
 	if "any_of" in v:
-		s = set()
+		s: set[T] = set()
 		for el in v['any_of']:
 			if isinstance(el, in_type):
-				s.add(el)
+				s.add(el) # type: ignore[arg-type]
 			elif isinstance(el, dict):
 				for ell in next(iter(el.values())):
 					s.add(ell)
 			else:
 				raise ValueError("unsupported format (1)")
 		return s
```

### Comparing `ampel_core-0.9.0/ampel/util/pretty.py` & `ampel_core-0.9.1a0/ampel/util/pretty.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/util/register.py` & `ampel_core-0.9.1a0/ampel/util/register.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/util/stock.py` & `ampel_core-0.9.1a0/ampel/util/stock.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/util/template.py` & `ampel_core-0.9.1a0/ampel/util/template.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/vendor/aiopipe/LICENSE.txt` & `ampel_core-0.9.1a0/ampel/vendor/aiopipe/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/ampel/vendor/aiopipe/__init__.py` & `ampel_core-0.9.1a0/ampel/vendor/aiopipe/__init__.py`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/conf/ampel-core/ampel.yaml` & `ampel_core-0.9.1a0/conf/ampel-core/ampel.yaml`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/conf/ampel-core/logging.yaml` & `ampel_core-0.9.1a0/conf/ampel-core/logging.yaml`

 * *Files identical despite different names*

### Comparing `ampel_core-0.9.0/conf/ampel-core/mongo/data.yaml` & `ampel_core-0.9.1a0/conf/ampel-core/mongo/data.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -13,22 +13,28 @@
     args:
       unique: true
   - field: stock
     args:
       sparse: true
 - name: t1
   indexes:
-  - field: stock
+  - index:
+    - field: stock
+    - field: link
+    args:
+      unique: true
   - field: channel
   - field: code
     args:
       sparse: true
 - name: t2
   indexes:
-  - field: stock
+  - index:
+    - field: stock
+    - field: link
   - field: channel
   - field: code
   - field: meta.ts
 - name: t3
   indexes:
   - field: process
   - field: meta.ts
```

### Comparing `ampel_core-0.9.0/pyproject.toml` & `ampel_core-0.9.1a0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ampel-core"
-version = "0.9.0"
+version = "0.9.1a0"
 description = "Alice in Modular Provenance-Enabled Land"
 authors = ["Valery Brinnel"]
 maintainers = ["Jakob van Santen <jakob.van.santen@desy.de>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://ampelproject.github.io"
 repository = "https://github.com/AmpelProject/Ampel-core"
@@ -40,42 +40,42 @@
 'config_Build_or_update_config._Fetch_or_append_config_elements' = 'ampel.cli.ConfigCommand'
 #'start_Run_ampel_continuously._Processes_are_scheduled_according_to_config' = 'ampel.cli.StartCommand'
 't2_Match_and_either_reset_or_view_raw_t2_documents' = 'ampel.cli.T2Command'
 'buffer_Match_and_view_or_save_ampel_buffers' = 'ampel.cli.BufferCommand'
 'event_Show_events_information' = 'ampel.cli.EventCommand'
 
 [tool.poetry.dependencies]
-ampel-interface = {version = "^0.9.0"}
-python = ">=3.10,<3.12"
+ampel-interface = {version = "^0.9.1a1"}
+python = "^3.10"
 pymongo = "^4.0"
 pydantic = "^1.9.0"
 sjcl = "^0.2.1"
 schedule = "^1.0.0"
 yq = "^3.0.0"
 prometheus-client = ">=0.16,<0.17"
 xxhash = "^3.0.0"
 psutil = "^5.8.0"
 appdirs = "^1.4.4"
 requests = "^2.0"
 fastapi = {version = ">=0.95,<0.96", optional = true}
 uvicorn = {version = ">=0.21.1,<0.22.0", optional = true, extras = ["standard"]}
-Sphinx = {version = ">=6.1.2,<6.2.0", optional = true}
+Sphinx = {version = ">=7.0.1,<7.1.0", optional = true}
 sphinx-press-theme = {version = ">=0.5.1,<0.9.0", optional = true}
 sphinx-autodoc-typehints = {version = "^1.11.1", optional = true}
 tomlkit = {version = "^0.11.0", optional = true}
 slack-sdk = {version = "^3.18.1", optional = true}
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.2.2"
-pytest-cov = "^4.0.0"
-mypy = "^1.1"
-pytest-asyncio = "^0.21.0"
-pytest-mock = "^3.10.0"
+pytest = "^7.4.2"
+pytest-cov = "^4.1.0"
+mypy = "^1.5.1"
+pytest-asyncio = "^0.21.1"
+pytest-mock = "^3.11.1"
 mongomock = "^4.1.2"
-httpx = "^0.23.3"
+httpx = "^0.25.0"
 types-setuptools = "^65.1.0"
 types-PyYAML = "^6.0.12"
 
 [tool.poetry.extras]
 server = ["fastapi", "uvicorn"]
 docs = ["Sphinx", "sphinx-press-theme", "sphinx-autodoc-typehints", "tomlkit"]
 slack = ["slack_sdk"]
```

### Comparing `ampel_core-0.9.0/PKG-INFO` & `ampel_core-0.9.1a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: ampel-core
-Version: 0.9.0
+Version: 0.9.1a0
 Summary: Alice in Modular Provenance-Enabled Land
 Home-page: https://ampelproject.github.io
 License: BSD-3-Clause
 Author: Valery Brinnel
 Maintainer: Jakob van Santen
 Maintainer-email: jakob.van.santen@desy.de
-Requires-Python: >=3.10,<3.12
+Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Typing :: Typed
 Provides-Extra: docs
 Provides-Extra: server
 Provides-Extra: slack
-Requires-Dist: Sphinx (>=6.1.2,<6.2.0) ; extra == "docs"
-Requires-Dist: ampel-interface (>=0.9.0,<0.10.0)
+Requires-Dist: Sphinx (>=7.0.1,<7.1.0) ; extra == "docs"
+Requires-Dist: ampel-interface (>=0.9.1a1,<0.10.0)
 Requires-Dist: appdirs (>=1.4.4,<2.0.0)
 Requires-Dist: fastapi (>=0.95,<0.96) ; extra == "server"
 Requires-Dist: prometheus-client (>=0.16,<0.17)
 Requires-Dist: psutil (>=5.8.0,<6.0.0)
 Requires-Dist: pydantic (>=1.9.0,<2.0.0)
 Requires-Dist: pymongo (>=4.0,<5.0)
 Requires-Dist: requests (>=2.0,<3.0)
```

