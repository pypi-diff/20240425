# Comparing `tmp/snowflake_cli_labs-2.2.0.tar.gz` & `tmp/snowflake_cli_labs-2.2.0rc0.tar.gz`

## Comparing `snowflake_cli_labs-2.2.0.tar` & `snowflake_cli_labs-2.2.0rc0.tar`

### file list

```diff
@@ -1,562 +1,562 @@
--rw-r--r--   0        0        0     2644 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     8948 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/CONTRIBUTING.md
--rw-r--r--   0        0        0    16198 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/RELEASE-NOTES.md
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/SECURITY.md
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/performance_history_analysis.py
--rw-r--r--   0        0        0    13022 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/docs/images/coverage_1.png
--rw-r--r--   0        0        0    24318 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/docs/images/coverage_2.png
--rw-r--r--   0        0        0    12852 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/docs/images/coverage_3.png
--rw-r--r--   0        0        0    24441 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/docs/images/coverage_4.png
--rw-r--r--   0        0        0    14955 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/docs/images/coverage_5.png
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/snyk/dependency-sync.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/snyk/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/__init__.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/__init__.py
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/api/__init__.py
--rw-r--r--   0        0        0     9236 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/api/cli_global_context.py
--rw-r--r--   0        0        0     9591 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/api/config.py
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/api/constants.py
--rw-r--r--   0        0        0     4075 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/api/exceptions.py
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/api/feature_flags.py
--rw-r--r--   0        0        0    11131 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/api/secure_path.py
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/api/secure_utils.py
--rw-r--r--   0        0        0     8776 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/api/sql_execution.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/api/commands/__init__.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/api/commands/alias.py
--rw-r--r--   0        0        0     8968 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/api/commands/decorators.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/api/commands/experimental_behaviour.py
--rw-r--r--   0        0        0    17770 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/api/commands/flags.py
--rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/api/commands/project_initialisation.py
--rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/api/commands/snow_typer.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/api/console/__init__.py
--rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/api/console/abc.py
--rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/api/console/console.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/api/console/enum.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/api/output/__init__.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/api/output/formats.py
--rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/api/output/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/api/plugins/__init__.py
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/api/plugins/plugin_config.py
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/api/plugins/command/__init__.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/api/plugins/command/plugin_hook_specs.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/api/project/__init__.py
--rw-r--r--   0        0        0     3747 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/api/project/definition.py
--rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/api/project/definition_manager.py
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/api/project/errors.py
--rw-r--r--   0        0        0     6172 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/api/project/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/api/project/schemas/__init__.py
--rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/api/project/schemas/project_definition.py
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/api/project/schemas/updatable_model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/api/project/schemas/native_app/__init__.py
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/api/project/schemas/native_app/application.py
--rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/api/project/schemas/native_app/native_app.py
--rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/api/project/schemas/native_app/package.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/api/project/schemas/native_app/path_mapping.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/api/project/schemas/snowpark/__init__.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/api/project/schemas/snowpark/argument.py
--rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/api/project/schemas/snowpark/callable.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/api/project/schemas/snowpark/snowpark.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/api/project/schemas/streamlit/__init__.py
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/api/project/schemas/streamlit/streamlit.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/api/utils/__init__.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/api/utils/cursor.py
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/api/utils/error_handling.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/api/utils/naming_utils.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/api/utils/path_utils.py
--rw-r--r--   0        0        0     3617 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/api/utils/rendering.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/app/__init__.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/app/__main__.py
--rw-r--r--   0        0        0     7292 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/app/cli_app.py
--rw-r--r--   0        0        0     5143 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/app/loggers.py
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/app/main_typer.py
--rw-r--r--   0        0        0     4471 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/app/printing.py
--rw-r--r--   0        0        0     7299 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/app/snow_connector.py
--rw-r--r--   0        0        0     3408 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/app/telemetry.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/app/api_impl/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/app/api_impl/plugin/__init__.py
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/app/api_impl/plugin/plugin_config_provider_impl.py
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/app/commands_registration/__init__.py
--rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/app/commands_registration/builtin_plugins.py
--rw-r--r--   0        0        0     5404 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/app/commands_registration/command_plugins_loader.py
--rw-r--r--   0        0        0     3694 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/app/commands_registration/commands_registration_with_callbacks.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/app/commands_registration/exception_logging.py
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/app/commands_registration/threadsafe.py
--rw-r--r--   0        0        0     5549 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/app/commands_registration/typer_registration.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/app/dev/__init__.py
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/app/dev/commands_structure.py
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/app/dev/pycharm_remote_debug.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/app/dev/docs/__init__.py
--rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/app/dev/docs/generator.py
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/app/dev/docs/templates/overview.rst.jinja2
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/app/dev/docs/templates/usage.rst.jinja2
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/connection/__init__.py
--rw-r--r--   0        0        0     8710 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/connection/commands.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/connection/plugin_spec.py
--rw-r--r--   0        0        0     3617 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/connection/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/git/__init__.py
--rw-r--r--   0        0        0     8045 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/git/commands.py
--rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/git/manager.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/git/plugin_spec.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/nativeapp/__init__.py
--rw-r--r--   0        0        0     9077 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/nativeapp/artifacts.py
--rw-r--r--   0        0        0     9081 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/nativeapp/commands.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/nativeapp/common_flags.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/nativeapp/constants.py
--rw-r--r--   0        0        0     2549 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/nativeapp/exceptions.py
--rw-r--r--   0        0        0    11239 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/nativeapp/init.py
--rw-r--r--   0        0        0    16830 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/nativeapp/manager.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/nativeapp/plugin_spec.py
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/nativeapp/policy.py
--rw-r--r--   0        0        0    12580 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/nativeapp/run_processor.py
--rw-r--r--   0        0        0     7822 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/nativeapp/teardown_processor.py
--rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/nativeapp/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/nativeapp/version/__init__.py
--rw-r--r--   0        0        0     4894 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/nativeapp/version/commands.py
--rw-r--r--   0        0        0    13227 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/nativeapp/version/version_processor.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/object/__init__.py
--rw-r--r--   0        0        0     3193 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/object/commands.py
--rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/object/common.py
--rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/object/manager.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/object/plugin_spec.py
--rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/object/stage_deprecated/commands.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/render/__init__.py
--rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/render/commands.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/render/plugin_spec.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/snowpark/__init__.py
--rw-r--r--   0        0        0    16641 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/snowpark/commands.py
--rw-r--r--   0        0        0     7016 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/snowpark/common.py
--rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/snowpark/manager.py
--rw-r--r--   0        0        0     4144 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/snowpark/models.py
--rw-r--r--   0        0        0     8854 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/snowpark/package_utils.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/snowpark/plugin_spec.py
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/snowpark/snowpark_package_paths.py
--rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/snowpark/snowpark_shared.py
--rw-r--r--   0        0        0     6123 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/snowpark/venv.py
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/snowpark/zipper.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/snowpark/package/__init__.py
--rw-r--r--   0        0        0     8740 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/snowpark/package/anaconda_packages.py
--rw-r--r--   0        0        0     8520 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/snowpark/package/commands.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/snowpark/package/manager.py
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/snowpark/package/utils.py
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/spcs/__init__.py
--rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/spcs/common.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/spcs/plugin_spec.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/spcs/compute_pool/__init__.py
--rw-r--r--   0        0        0     6595 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/spcs/compute_pool/commands.py
--rw-r--r--   0        0        0     4069 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/spcs/compute_pool/manager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/spcs/image_registry/__init__.py
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/spcs/image_registry/commands.py
--rw-r--r--   0        0        0     3305 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/spcs/image_registry/manager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/spcs/image_repository/__init__.py
--rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/spcs/image_repository/commands.py
--rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/spcs/image_repository/manager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/spcs/jobs/__init__.py
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/spcs/jobs/commands.py
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/spcs/jobs/manager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/spcs/services/__init__.py
--rw-r--r--   0        0        0     8438 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/spcs/services/commands.py
--rw-r--r--   0        0        0     5809 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/spcs/services/manager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/sql/__init__.py
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/sql/commands.py
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/sql/manager.py
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/sql/plugin_spec.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/stage/__init__.py
--rw-r--r--   0        0        0     6219 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/stage/commands.py
--rw-r--r--   0        0        0     8893 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/stage/diff.py
--rw-r--r--   0        0        0    11112 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/stage/manager.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/stage/plugin_spec.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/streamlit/__init__.py
--rw-r--r--   0        0        0     4519 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/streamlit/commands.py
--rw-r--r--   0        0        0     7351 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/streamlit/manager.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/streamlit/plugin_spec.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/templates/environment.yml.jinja
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/templates/streamlit_app_launcher.py.jinja
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/templates/default_snowpark/.gitignore
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/templates/default_snowpark/requirements.txt
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/templates/default_snowpark/snowflake.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/templates/default_snowpark/app/__init__.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/templates/default_snowpark/app/common.py
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/templates/default_snowpark/app/functions.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/templates/default_snowpark/app/procedures.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/templates/default_streamlit/.gitignore
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/templates/default_streamlit/environment.yml
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/templates/default_streamlit/snowflake.yml
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/templates/default_streamlit/streamlit_app.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/templates/default_streamlit/common/hello.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/src/snowflake/cli/templates/default_streamlit/pages/my_page.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/test_external_plugins/broken_plugin/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/test_external_plugins/broken_plugin/src/snowflakecli/test_plugins/broken_plugin/__init__.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/test_external_plugins/broken_plugin/src/snowflakecli/test_plugins/broken_plugin/commands.py
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/test_external_plugins/broken_plugin/src/snowflakecli/test_plugins/broken_plugin/plugin_spec.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/test_external_plugins/failing_plugin/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/test_external_plugins/failing_plugin/src/snowflakecli/test_plugins/failing_plugin/__init__.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/test_external_plugins/failing_plugin/src/snowflakecli/test_plugins/failing_plugin/commands.py
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/test_external_plugins/failing_plugin/src/snowflakecli/test_plugins/failing_plugin/plugin_spec.py
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/test_external_plugins/multilingual_hello_command_group/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/test_external_plugins/multilingual_hello_command_group/src/snowflakecli/test_plugins/multilingual_hello/__init__.py
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/test_external_plugins/multilingual_hello_command_group/src/snowflakecli/test_plugins/multilingual_hello/commands.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/test_external_plugins/multilingual_hello_command_group/src/snowflakecli/test_plugins/multilingual_hello/hello_language.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/test_external_plugins/multilingual_hello_command_group/src/snowflakecli/test_plugins/multilingual_hello/manager.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/test_external_plugins/multilingual_hello_command_group/src/snowflakecli/test_plugins/multilingual_hello/plugin_spec.py
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/test_external_plugins/override_build_in_command/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/test_external_plugins/override_build_in_command/src/snowflakecli/test_plugins/override_build_in_command/__init__.py
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/test_external_plugins/override_build_in_command/src/snowflakecli/test_plugins/override_build_in_command/commands.py
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/test_external_plugins/override_build_in_command/src/snowflakecli/test_plugins/override_build_in_command/plugin_spec.py
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/test_external_plugins/snowpark_hello_single_command/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/test_external_plugins/snowpark_hello_single_command/src/snowflakecli/test_plugins/snowpark_hello/__init__.py
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/test_external_plugins/snowpark_hello_single_command/src/snowflakecli/test_plugins/snowpark_hello/commands.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/test_external_plugins/snowpark_hello_single_command/src/snowflakecli/test_plugins/snowpark_hello/manager.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/test_external_plugins/snowpark_hello_single_command/src/snowflakecli/test_plugins/snowpark_hello/plugin_spec.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/__init__.py
--rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/conftest.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/empty_config.toml
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test.toml
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_cli.py
--rw-r--r--   0        0        0     7985 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_command_registration.py
--rw-r--r--   0        0        0     6206 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_common_decorators.py
--rw-r--r--   0        0        0     4259 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_common_global_context.py
--rw-r--r--   0        0        0     7592 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_config.py
--rw-r--r--   0        0        0    24815 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_connection.py
--rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_experimental_behaviour.py
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_help_messages.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_loaded_modules.py
--rw-r--r--   0        0        0     6599 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_logs.py
--rw-r--r--   0        0        0     5235 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_main.py
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_performance.py
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_project_initialisation.py
--rw-r--r--   0        0        0     3637 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_render.py
--rw-r--r--   0        0        0     3562 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_snow_connector.py
--rw-r--r--   0        0        0    10093 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_sql.py
--rw-r--r--   0        0        0     4925 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_utils.py
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_zipper.py
--rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/__snapshots__/test_connection.ambr
--rw-r--r--   0        0        0   529299 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/__snapshots__/test_help_messages.ambr
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/api/__init__.py
--rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/api/test_feature_flags.py
--rw-r--r--   0        0        0    17128 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/api/test_secure_path.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/api/commands/__init__.py
--rw-r--r--   0        0        0     5943 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/api/commands/test_flags.py
--rw-r--r--   0        0        0     5734 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/api/commands/test_snow_typer.py
--rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/api/commands/__snapshots__/test_flags.ambr
--rw-r--r--   0        0        0    13093 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/api/commands/__snapshots__/test_snow_typer.ambr
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/api/console/__init__.py
--rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/api/console/test_cli_console_output.py
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/api/console/test_console_abc.py
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/api/console/test_intermediate_output.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/api/utils/test_naming_utils.py
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/app/test_telemetry.py
--rw-r--r--   0        0        0    17131 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/git/test_git_commands.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/nativeapp/__init__.py
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/nativeapp/patch_utils.py
--rw-r--r--   0        0        0     5478 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/nativeapp/test_artifacts.py
--rw-r--r--   0        0        0     4924 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/nativeapp/test_commands.py
--rw-r--r--   0        0        0    15151 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/nativeapp/test_init.py
--rw-r--r--   0        0        0    23734 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/nativeapp/test_manager.py
--rw-r--r--   0        0        0     6339 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/nativeapp/test_package_scripts.py
--rw-r--r--   0        0        0    43760 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/nativeapp/test_run_processor.py
--rw-r--r--   0        0        0    35934 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/nativeapp/test_teardown_processor.py
--rw-r--r--   0        0        0     3760 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/nativeapp/test_utils.py
--rw-r--r--   0        0        0    22474 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/nativeapp/test_version_create_processor.py
--rw-r--r--   0        0        0     7807 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/nativeapp/test_version_drop_processor.py
--rw-r--r--   0        0        0     2532 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/nativeapp/utils.py
--rw-r--r--   0        0        0    16899 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/nativeapp/__snapshots__/test_commands.ambr
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/nativeapp/__snapshots__/test_init.ambr
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/object/__init__.py
--rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/object/test_common.py
--rw-r--r--   0        0        0     7489 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/object/test_object.py
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/object/test_stage.py
--rw-r--r--   0        0        0     9313 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/object/__snapshots__/test_object.ambr
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/output/__init__.py
--rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/output/test_format_silent_enforcement.py
--rw-r--r--   0        0        0     9704 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/output/test_printing.py
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/output/test_silent_output.py
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/plugin/test_broken_plugin.py
--rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/plugin/test_failing_plugin.py
--rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/plugin/test_override_by_external_plugins.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/project/__init__.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/project/fixtures.py
--rw-r--r--   0        0        0     4775 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/project/test_config.py
--rw-r--r--   0        0        0     5141 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/project/test_definition_manager.py
--rw-r--r--   0        0        0     6898 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/project/test_util.py
--rw-r--r--   0        0        0    19709 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/project/__snapshots__/test_config.ambr
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/snowpark/__init__.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/snowpark/mocks.py
--rw-r--r--   0        0        0     7344 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/snowpark/test_anaconda.py
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/snowpark/test_build.py
--rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/snowpark/test_common.py
--rw-r--r--   0        0        0    11492 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/snowpark/test_function.py
--rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/snowpark/test_models.py
--rw-r--r--   0        0        0     7165 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/snowpark/test_package.py
--rw-r--r--   0        0        0    14097 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/snowpark/test_procedure.py
--rw-r--r--   0        0        0     3116 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/snowpark/__snapshots__/test_function.ambr
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/snowpark/__snapshots__/test_package.ambr
--rw-r--r--   0        0        0     4926 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/snowpark/__snapshots__/test_procedure.ambr
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/snowpark/__snapshots__/test_procedure_coverage.ambr
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/spcs/__init__.py
--rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/spcs/test_common.py
--rw-r--r--   0        0        0    16282 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/spcs/test_compute_pool.py
--rw-r--r--   0        0        0     9321 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/spcs/test_image_repository.py
--rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/spcs/test_jobs.py
--rw-r--r--   0        0        0     6694 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/spcs/test_registry.py
--rw-r--r--   0        0        0    22547 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/spcs/test_services.py
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/spcs/__snapshots__/test_image_repository.ambr
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/spcs/__snapshots__/test_registry.ambr
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/stage/__init__.py
--rw-r--r--   0        0        0     7385 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/stage/test_diff.py
--rw-r--r--   0        0        0    29844 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/stage/test_stage.py
--rw-r--r--   0        0        0     7770 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/stage/__snapshots__/test_stage.ambr
--rw-r--r--   0        0        0    23568 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/streamlit/test_commands.py
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/streamlit/test_config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/__init__.py
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/anaconda_channel_data.json
--rw-r--r--   0        0        0     7793 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/packages_available_in_snowflake_sql_result_rows.json
--rw-r--r--   0        0        0     4526 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/test_data.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/test_streamlit_requirements.txt
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/configs/broken_plugin_config.toml
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/configs/disabled_override_plugin_config.toml
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/configs/failing_plugin_config.toml
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/configs/override_plugin_config.toml
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/INSTALLER
--rwxr-xr-x   0        0        0     1080 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/LICENSE.txt
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/METADATA
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/REQUESTED
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/WHEEL
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/top_level.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/local_packages/.packages/azure/core/file.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/local_packages/.packages/azure/eventhub/file.txt
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/INSTALLER
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/LICENSE
--rw-r--r--   0        0        0    36617 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/METADATA
--rw-r--r--   0        0        0    11535 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/RECORD
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/WHEEL
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/top_level.txt
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/INSTALLER
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/LICENSE
--rw-r--r--   0        0        0    66103 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/METADATA
--rw-r--r--   0        0        0    17195 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/REQUESTED
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/WHEEL
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/top_level.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/local_packages/.packages/httplib2/file.txt
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/LICENSE
--rw-r--r--   0        0        0     2618 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/METADATA
--rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/RECORD
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/WHEEL
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/top_level.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/local_packages/.packages/zendesk/file.txt
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/empty_project/snowflake.yml
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/example_streamlit/environment.yml
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/example_streamlit/snowflake.yml
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/example_streamlit/streamlit_app.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/example_streamlit/pages/my_page.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/example_streamlit_no_defaults/main.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/example_streamlit_no_defaults/snowflake.yml
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/example_streamlit_no_defaults/streamlit_environment.yml
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/example_streamlit_no_defaults/streamlit_pages/first_page.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/example_streamlit_no_stage/environment.yml
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/example_streamlit_no_stage/snowflake.yml
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/example_streamlit_no_stage/streamlit_app.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/example_streamlit_no_stage/pages/my_page.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/integration/snowflake.yml
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/integration/app/README.md
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/integration/app/manifest.yml
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/integration/app/setup.sql
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/integration/package/001-shared.sql
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/integration/package/002-shared.sql
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/integration_external/snowflake.local.yml
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/integration_external/snowflake.yml
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/integration_external/app/README.md
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/integration_external/app/manifest.yml
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/integration_external/app/setup.sql
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/integration_external/package/001-shared.sql
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/integration_external/package/002-shared.sql
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/minimal/snowflake.yml
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/napp_project_1/001-shared.sql
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/napp_project_1/002-shared.sql
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/napp_project_1/setup.sql
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/napp_project_1/snowflake.local.yml
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/napp_project_1/snowflake.yml
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/napp_project_1/app/README.md
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/napp_project_1/app/streamlit/config.py
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/napp_project_1/app/streamlit/main.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/napp_project_with_pkg_warehouse/001-shared.sql
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/napp_project_with_pkg_warehouse/002-shared.sql
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/napp_project_with_pkg_warehouse/setup.sql
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/napp_project_with_pkg_warehouse/snowflake.local.yml
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/napp_project_with_pkg_warehouse/snowflake.yml
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/napp_project_with_pkg_warehouse/app/README.md
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/napp_project_with_pkg_warehouse/app/streamlit/config.py
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/napp_project_with_pkg_warehouse/app/streamlit/main.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/no_definition_version/snowflake.yml
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/snowpark_function_external_access/app.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/snowpark_function_external_access/app.zip
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/snowpark_function_external_access/requirements.txt
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/snowpark_function_external_access/snowflake.yml
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/snowpark_function_fully_qualified_name/app.zip
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/snowpark_function_fully_qualified_name/requirements.txt
--rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/snowpark_function_fully_qualified_name/snowflake.yml
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/snowpark_function_fully_qualified_name/app/app.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/snowpark_function_secrets_without_external_access/app.zip
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/snowpark_function_secrets_without_external_access/snowflake.yml
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/snowpark_functions/app.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/snowpark_functions/app.zip
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/snowpark_functions/requirements.txt
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/snowpark_functions/snowflake.yml
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/snowpark_procedure_external_access/app.py
--rw-r--r--   0        0        0     3727 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/snowpark_procedure_external_access/app.zip
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/snowpark_procedure_external_access/requirements.txt
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/snowpark_procedure_external_access/snowflake.yml
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/snowpark_procedure_fully_qualified_name/app.zip
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/snowpark_procedure_fully_qualified_name/requirements.txt
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/snowpark_procedure_fully_qualified_name/snowflake.yml
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/snowpark_procedure_fully_qualified_name/app/app.py
--rw-r--r--   0        0        0     3727 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/snowpark_procedure_secrets_without_external_access/app.zip
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/snowpark_procedure_secrets_without_external_access/snowflake.yml
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/snowpark_procedures/app.py
--rw-r--r--   0        0        0     3727 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/snowpark_procedures/app.zip
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/snowpark_procedures/requirements.txt
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/snowpark_procedures/snowflake.yml
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/snowpark_procedures_coverage/app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/snowpark_procedures_coverage/app.zip
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/snowpark_procedures_coverage/requirements.txt
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/snowpark_procedures_coverage/snowflake.yml
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/streamlit_full_definition/environment.yml
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/streamlit_full_definition/snowflake.yml
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/streamlit_full_definition/streamlit_app.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/streamlit_full_definition/pages/my_page.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/streamlit_full_definition/utils/utils.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/underspecified/snowflake.yml
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/projects/unknown_fields/snowflake.yml
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/streamlit/another_file_with_list.yml
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/streamlit/another_file_with_single_item.yml
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/streamlit/with_list_in_source_file.yml
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/test_data/streamlit/with_single_item.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/testing_utils/__init__.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/testing_utils/conversion.py
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/testing_utils/files_and_dirs.py
--rw-r--r--   0        0        0     8445 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/testing_utils/fixtures.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests/testing_utils/result_assertions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_e2e/__init__.py
--rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_e2e/conftest.py
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_e2e/test_error_handling.py
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_e2e/test_installation.py
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_e2e/test_snowpark_examples.py
--rw-r--r--   0        0        0     3302 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_e2e/__snapshots__/test_installation.ambr
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_e2e/config/config.toml
--rwxr-xr-x   0        0        0       99 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_e2e/config/malformatted_config.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/__init__.py
--rw-r--r--   0        0        0     5133 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/conftest.py
--rw-r--r--   0        0        0     3007 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/snowflake_connector.py
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/test_config.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/test_connection.py
--rw-r--r--   0        0        0     5375 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/test_external_plugins.py
--rw-r--r--   0        0        0     9649 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/test_git.py
--rw-r--r--   0        0        0    19879 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/test_nativeapp.py
--rw-r--r--   0        0        0     4208 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/test_object.py
--rw-r--r--   0        0        0     7144 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/test_package.py
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/test_session_token.py
--rw-r--r--   0        0        0    28253 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/test_snowpark.py
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/test_snowpark_external_access.py
--rw-r--r--   0        0        0     2980 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/test_sql.py
--rw-r--r--   0        0        0     6319 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/test_stage.py
--rw-r--r--   0        0        0     8498 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/test_streamlit.py
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/test_temporary_connection.py
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/test_utils.py
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/__snapshots__/test_function.ambr
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/__snapshots__/test_git.ambr
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/__snapshots__/test_package.ambr
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/__snapshots__/test_sql.ambr
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/__snapshots__/test_stage.ambr
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/config/config_with_enabled_all_external_plugins.toml
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/config/config_with_enabled_only_one_external_plugin.toml
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/config/connection_configs.toml
--rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/scripts/integration_account_setup.sql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/spcs/__init__.py
--rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/spcs/test_compute_pool.py
--rw-r--r--   0        0        0     3102 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/spcs/test_image_repository.py
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/spcs/test_jobs.py
--rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/spcs/test_registry.py
--rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/spcs/test_services.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/spcs/docker/Dockerfile
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/spcs/docker/bootstrap_containers_setup.sh
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/spcs/docker/echo_service.py
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/spcs/spec/spec.yml
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/spcs/spec/spec_upgrade.yml
--rw-r--r--   0        0        0     6477 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/spcs/testing_utils/compute_pool_utils.py
--rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/spcs/testing_utils/spcs_jobs_utils.py
--rw-r--r--   0        0        0    10521 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/spcs/testing_utils/spcs_services_utils.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/test_data/sql_multi_queries.sql
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/test_data/projects/snowpark/.gitignore
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/test_data/projects/snowpark/requirements.txt
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/test_data/projects/snowpark/snowflake.yml
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/test_data/projects/snowpark/app/app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/test_data/projects/snowpark_coverage/.gitignore
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/test_data/projects/snowpark_coverage/requirements.txt
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/test_data/projects/snowpark_coverage/snowflake.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/test_data/projects/snowpark_coverage/app/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/test_data/projects/snowpark_coverage/app/module/__init__.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/test_data/projects/snowpark_coverage/app/module/procedures.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/test_data/projects/snowpark_external_access/.gitignore
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/test_data/projects/snowpark_external_access/requirements.txt
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/test_data/projects/snowpark_external_access/snowflake.yml
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/test_data/projects/snowpark_external_access/app/app.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/test_data/projects/snowpark_fully_qualified_name/.gitignore
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/test_data/projects/snowpark_fully_qualified_name/requirements.txt
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/test_data/projects/snowpark_fully_qualified_name/snowflake.yml
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/test_data/projects/snowpark_fully_qualified_name/app/app.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/test_data/projects/snowpark_vectorized/.gitignore
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/test_data/projects/snowpark_vectorized/requirements.txt
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/test_data/projects/snowpark_vectorized/snowflake.yml
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/test_data/projects/snowpark_vectorized/app/app.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/test_data/projects/snowpark_version_check/.gitignore
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/test_data/projects/snowpark_version_check/requirements.txt
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/test_data/projects/snowpark_version_check/snowflake.yml
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/test_data/projects/snowpark_version_check/app/app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/test_data/projects/snowpark_with_default_values/requirements.other.txt
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/test_data/projects/snowpark_with_default_values/requirements.txt
--rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/test_data/projects/snowpark_with_default_values/snowflake.yml
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/test_data/projects/snowpark_with_default_values/app/app.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/test_data/projects/snowpark_with_import/.gitignore
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/test_data/projects/snowpark_with_import/requirements.txt
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/test_data/projects/snowpark_with_import/snowflake.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/test_data/projects/snowpark_with_import/app/__init__.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/test_data/projects/snowpark_with_import/app/functions.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/test_data/projects/snowpark_with_single_requirements_having_no_other_deps/.gitignore
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/test_data/projects/snowpark_with_single_requirements_having_no_other_deps/requirements.txt
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/test_data/projects/snowpark_with_single_requirements_having_no_other_deps/snowflake.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/test_data/projects/snowpark_with_single_requirements_having_no_other_deps/app/__init__.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/test_data/projects/snowpark_with_single_requirements_having_no_other_deps/app/functions.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/test_data/projects/snowpark_with_single_requirements_having_transient_deps/.gitignore
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/test_data/projects/snowpark_with_single_requirements_having_transient_deps/requirements.txt
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/test_data/projects/snowpark_with_single_requirements_having_transient_deps/snowflake.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/test_data/projects/snowpark_with_single_requirements_having_transient_deps/app/__init__.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/test_data/projects/snowpark_with_single_requirements_having_transient_deps/app/functions.py
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/test_data/projects/stage_execute/script1.sql
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/test_data/projects/stage_execute/script2.sql
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/test_data/projects/stage_execute/script3.sql
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/test_data/projects/stage_execute/script_template.sql
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/test_data/projects/stage_get_directory_structure/script1.sql
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/test_data/projects/stage_get_directory_structure/dir/script2.sql
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/test_data/projects/stage_get_directory_structure/dir/subdir/script3.sql
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/test_data/projects/streamlit/environment.yml
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/test_data/projects/streamlit/snowflake.yml
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/test_data/projects/streamlit/streamlit_app.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/test_data/projects/streamlit/pages/my_page.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/test_data/projects/streamlit/utils/utils.py
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/testing_utils/__init__.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/testing_utils/naming_utils.py
--rw-r--r--   0        0        0    11583 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/testing_utils/snowpark_utils.py
--rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/testing_utils/sql_utils.py
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/testing_utils/working_directory_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/testing_utils/assertions/__init__.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/testing_utils/assertions/test_file_assertions.py
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/tests_integration/testing_utils/assertions/test_result_assertions.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/.gitignore
--rw-r--r--   0        0        0    11344 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/LICENSE
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/README.md
--rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/pyproject.toml
--rw-r--r--   0        0        0    16120 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0     2644 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     8948 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/CONTRIBUTING.md
+-rw-r--r--   0        0        0    16098 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/RELEASE-NOTES.md
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/SECURITY.md
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/performance_history_analysis.py
+-rw-r--r--   0        0        0    13022 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/docs/images/coverage_1.png
+-rw-r--r--   0        0        0    24318 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/docs/images/coverage_2.png
+-rw-r--r--   0        0        0    12852 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/docs/images/coverage_3.png
+-rw-r--r--   0        0        0    24441 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/docs/images/coverage_4.png
+-rw-r--r--   0        0        0    14955 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/docs/images/coverage_5.png
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/snyk/dependency-sync.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/snyk/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/__init__.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/__init__.py
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/__init__.py
+-rw-r--r--   0        0        0     9236 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/cli_global_context.py
+-rw-r--r--   0        0        0     9591 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/config.py
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/constants.py
+-rw-r--r--   0        0        0     4075 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/exceptions.py
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/feature_flags.py
+-rw-r--r--   0        0        0    11131 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/secure_path.py
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/secure_utils.py
+-rw-r--r--   0        0        0     8506 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/sql_execution.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/commands/__init__.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/commands/alias.py
+-rw-r--r--   0        0        0     8968 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/commands/decorators.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/commands/experimental_behaviour.py
+-rw-r--r--   0        0        0    17770 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/commands/flags.py
+-rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/commands/project_initialisation.py
+-rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/commands/snow_typer.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/console/__init__.py
+-rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/console/abc.py
+-rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/console/console.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/console/enum.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/output/__init__.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/output/formats.py
+-rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/output/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/plugins/__init__.py
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/plugins/plugin_config.py
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/plugins/command/__init__.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/plugins/command/plugin_hook_specs.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/__init__.py
+-rw-r--r--   0        0        0     3747 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/definition.py
+-rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/definition_manager.py
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/errors.py
+-rw-r--r--   0        0        0     6172 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/schemas/__init__.py
+-rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/schemas/project_definition.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/schemas/updatable_model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/schemas/native_app/__init__.py
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/schemas/native_app/application.py
+-rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/schemas/native_app/native_app.py
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/schemas/native_app/package.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/schemas/native_app/path_mapping.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/schemas/snowpark/__init__.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/schemas/snowpark/argument.py
+-rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/schemas/snowpark/callable.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/schemas/snowpark/snowpark.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/schemas/streamlit/__init__.py
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/schemas/streamlit/streamlit.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/utils/__init__.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/utils/cursor.py
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/utils/error_handling.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/utils/naming_utils.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/utils/path_utils.py
+-rw-r--r--   0        0        0     3617 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/utils/rendering.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/__init__.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/__main__.py
+-rw-r--r--   0        0        0     7292 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/cli_app.py
+-rw-r--r--   0        0        0     5143 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/loggers.py
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/main_typer.py
+-rw-r--r--   0        0        0     4471 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/printing.py
+-rw-r--r--   0        0        0     7299 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/snow_connector.py
+-rw-r--r--   0        0        0     3408 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/telemetry.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/api_impl/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/api_impl/plugin/__init__.py
+-rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/api_impl/plugin/plugin_config_provider_impl.py
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/commands_registration/__init__.py
+-rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/commands_registration/builtin_plugins.py
+-rw-r--r--   0        0        0     5404 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/commands_registration/command_plugins_loader.py
+-rw-r--r--   0        0        0     3694 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/commands_registration/commands_registration_with_callbacks.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/commands_registration/exception_logging.py
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/commands_registration/threadsafe.py
+-rw-r--r--   0        0        0     5549 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/commands_registration/typer_registration.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/dev/__init__.py
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/dev/commands_structure.py
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/dev/pycharm_remote_debug.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/dev/docs/__init__.py
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/dev/docs/generator.py
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/dev/docs/templates/overview.rst.jinja2
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/dev/docs/templates/usage.rst.jinja2
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/connection/__init__.py
+-rw-r--r--   0        0        0     8710 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/connection/commands.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/connection/plugin_spec.py
+-rw-r--r--   0        0        0     3617 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/connection/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/git/__init__.py
+-rw-r--r--   0        0        0     8045 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/git/commands.py
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/git/manager.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/git/plugin_spec.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/__init__.py
+-rw-r--r--   0        0        0     9077 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/artifacts.py
+-rw-r--r--   0        0        0     9081 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/commands.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/common_flags.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/constants.py
+-rw-r--r--   0        0        0     2549 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/exceptions.py
+-rw-r--r--   0        0        0    11239 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/init.py
+-rw-r--r--   0        0        0    16830 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/manager.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/plugin_spec.py
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/policy.py
+-rw-r--r--   0        0        0    12580 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/run_processor.py
+-rw-r--r--   0        0        0     7822 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/teardown_processor.py
+-rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/version/__init__.py
+-rw-r--r--   0        0        0     4894 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/version/commands.py
+-rw-r--r--   0        0        0    13227 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/version/version_processor.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/object/__init__.py
+-rw-r--r--   0        0        0     3193 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/object/commands.py
+-rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/object/common.py
+-rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/object/manager.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/object/plugin_spec.py
+-rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/object/stage_deprecated/commands.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/render/__init__.py
+-rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/render/commands.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/render/plugin_spec.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/snowpark/__init__.py
+-rw-r--r--   0        0        0    16641 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/snowpark/commands.py
+-rw-r--r--   0        0        0     7016 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/snowpark/common.py
+-rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/snowpark/manager.py
+-rw-r--r--   0        0        0     4144 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/snowpark/models.py
+-rw-r--r--   0        0        0     8854 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/snowpark/package_utils.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/snowpark/plugin_spec.py
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/snowpark/snowpark_package_paths.py
+-rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/snowpark/snowpark_shared.py
+-rw-r--r--   0        0        0     6123 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/snowpark/venv.py
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/snowpark/zipper.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/snowpark/package/__init__.py
+-rw-r--r--   0        0        0     8740 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/snowpark/package/anaconda_packages.py
+-rw-r--r--   0        0        0     8520 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/snowpark/package/commands.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/snowpark/package/manager.py
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/snowpark/package/utils.py
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/__init__.py
+-rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/common.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/plugin_spec.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/compute_pool/__init__.py
+-rw-r--r--   0        0        0     6595 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/compute_pool/commands.py
+-rw-r--r--   0        0        0     4069 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/compute_pool/manager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/image_registry/__init__.py
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/image_registry/commands.py
+-rw-r--r--   0        0        0     3305 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/image_registry/manager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/image_repository/__init__.py
+-rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/image_repository/commands.py
+-rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/image_repository/manager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/jobs/__init__.py
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/jobs/commands.py
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/jobs/manager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/services/__init__.py
+-rw-r--r--   0        0        0     8438 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/services/commands.py
+-rw-r--r--   0        0        0     5809 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/services/manager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/sql/__init__.py
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/sql/commands.py
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/sql/manager.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/sql/plugin_spec.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/stage/__init__.py
+-rw-r--r--   0        0        0     6219 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/stage/commands.py
+-rw-r--r--   0        0        0     8893 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/stage/diff.py
+-rw-r--r--   0        0        0    11112 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/stage/manager.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/stage/plugin_spec.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/streamlit/__init__.py
+-rw-r--r--   0        0        0     4519 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/streamlit/commands.py
+-rw-r--r--   0        0        0     7351 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/streamlit/manager.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/streamlit/plugin_spec.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/templates/environment.yml.jinja
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/templates/streamlit_app_launcher.py.jinja
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/templates/default_snowpark/.gitignore
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/templates/default_snowpark/requirements.txt
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/templates/default_snowpark/snowflake.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/templates/default_snowpark/app/__init__.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/templates/default_snowpark/app/common.py
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/templates/default_snowpark/app/functions.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/templates/default_snowpark/app/procedures.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/templates/default_streamlit/.gitignore
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/templates/default_streamlit/environment.yml
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/templates/default_streamlit/snowflake.yml
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/templates/default_streamlit/streamlit_app.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/templates/default_streamlit/common/hello.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/templates/default_streamlit/pages/my_page.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/test_external_plugins/broken_plugin/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/test_external_plugins/broken_plugin/src/snowflakecli/test_plugins/broken_plugin/__init__.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/test_external_plugins/broken_plugin/src/snowflakecli/test_plugins/broken_plugin/commands.py
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/test_external_plugins/broken_plugin/src/snowflakecli/test_plugins/broken_plugin/plugin_spec.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/test_external_plugins/failing_plugin/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/test_external_plugins/failing_plugin/src/snowflakecli/test_plugins/failing_plugin/__init__.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/test_external_plugins/failing_plugin/src/snowflakecli/test_plugins/failing_plugin/commands.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/test_external_plugins/failing_plugin/src/snowflakecli/test_plugins/failing_plugin/plugin_spec.py
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/test_external_plugins/multilingual_hello_command_group/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/test_external_plugins/multilingual_hello_command_group/src/snowflakecli/test_plugins/multilingual_hello/__init__.py
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/test_external_plugins/multilingual_hello_command_group/src/snowflakecli/test_plugins/multilingual_hello/commands.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/test_external_plugins/multilingual_hello_command_group/src/snowflakecli/test_plugins/multilingual_hello/hello_language.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/test_external_plugins/multilingual_hello_command_group/src/snowflakecli/test_plugins/multilingual_hello/manager.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/test_external_plugins/multilingual_hello_command_group/src/snowflakecli/test_plugins/multilingual_hello/plugin_spec.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/test_external_plugins/override_build_in_command/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/test_external_plugins/override_build_in_command/src/snowflakecli/test_plugins/override_build_in_command/__init__.py
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/test_external_plugins/override_build_in_command/src/snowflakecli/test_plugins/override_build_in_command/commands.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/test_external_plugins/override_build_in_command/src/snowflakecli/test_plugins/override_build_in_command/plugin_spec.py
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/test_external_plugins/snowpark_hello_single_command/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/test_external_plugins/snowpark_hello_single_command/src/snowflakecli/test_plugins/snowpark_hello/__init__.py
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/test_external_plugins/snowpark_hello_single_command/src/snowflakecli/test_plugins/snowpark_hello/commands.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/test_external_plugins/snowpark_hello_single_command/src/snowflakecli/test_plugins/snowpark_hello/manager.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/test_external_plugins/snowpark_hello_single_command/src/snowflakecli/test_plugins/snowpark_hello/plugin_spec.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/__init__.py
+-rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/conftest.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/empty_config.toml
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test.toml
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_cli.py
+-rw-r--r--   0        0        0     7985 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_command_registration.py
+-rw-r--r--   0        0        0     6206 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_common_decorators.py
+-rw-r--r--   0        0        0     4259 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_common_global_context.py
+-rw-r--r--   0        0        0     7592 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_config.py
+-rw-r--r--   0        0        0    24815 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_connection.py
+-rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_experimental_behaviour.py
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_help_messages.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_loaded_modules.py
+-rw-r--r--   0        0        0     6599 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_logs.py
+-rw-r--r--   0        0        0     5235 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_main.py
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_performance.py
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_project_initialisation.py
+-rw-r--r--   0        0        0     3637 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_render.py
+-rw-r--r--   0        0        0     3562 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_snow_connector.py
+-rw-r--r--   0        0        0    10093 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_sql.py
+-rw-r--r--   0        0        0     4925 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_utils.py
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_zipper.py
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/__snapshots__/test_connection.ambr
+-rw-r--r--   0        0        0   529299 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/__snapshots__/test_help_messages.ambr
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/api/__init__.py
+-rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/api/test_feature_flags.py
+-rw-r--r--   0        0        0    17128 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/api/test_secure_path.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/api/commands/__init__.py
+-rw-r--r--   0        0        0     5943 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/api/commands/test_flags.py
+-rw-r--r--   0        0        0     5734 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/api/commands/test_snow_typer.py
+-rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/api/commands/__snapshots__/test_flags.ambr
+-rw-r--r--   0        0        0    13093 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/api/commands/__snapshots__/test_snow_typer.ambr
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/api/console/__init__.py
+-rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/api/console/test_cli_console_output.py
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/api/console/test_console_abc.py
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/api/console/test_intermediate_output.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/api/utils/test_naming_utils.py
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/app/test_telemetry.py
+-rw-r--r--   0        0        0    17131 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/git/test_git_commands.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/nativeapp/__init__.py
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/nativeapp/patch_utils.py
+-rw-r--r--   0        0        0     5478 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/nativeapp/test_artifacts.py
+-rw-r--r--   0        0        0     4924 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/nativeapp/test_commands.py
+-rw-r--r--   0        0        0    15151 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/nativeapp/test_init.py
+-rw-r--r--   0        0        0    23734 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/nativeapp/test_manager.py
+-rw-r--r--   0        0        0     6339 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/nativeapp/test_package_scripts.py
+-rw-r--r--   0        0        0    43760 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/nativeapp/test_run_processor.py
+-rw-r--r--   0        0        0    35934 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/nativeapp/test_teardown_processor.py
+-rw-r--r--   0        0        0     3760 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/nativeapp/test_utils.py
+-rw-r--r--   0        0        0    22474 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/nativeapp/test_version_create_processor.py
+-rw-r--r--   0        0        0     7807 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/nativeapp/test_version_drop_processor.py
+-rw-r--r--   0        0        0     2532 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/nativeapp/utils.py
+-rw-r--r--   0        0        0    16899 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/nativeapp/__snapshots__/test_commands.ambr
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/nativeapp/__snapshots__/test_init.ambr
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/object/__init__.py
+-rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/object/test_common.py
+-rw-r--r--   0        0        0     7489 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/object/test_object.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/object/test_stage.py
+-rw-r--r--   0        0        0     9313 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/object/__snapshots__/test_object.ambr
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/output/__init__.py
+-rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/output/test_format_silent_enforcement.py
+-rw-r--r--   0        0        0     9704 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/output/test_printing.py
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/output/test_silent_output.py
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/plugin/test_broken_plugin.py
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/plugin/test_failing_plugin.py
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/plugin/test_override_by_external_plugins.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/project/__init__.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/project/fixtures.py
+-rw-r--r--   0        0        0     4775 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/project/test_config.py
+-rw-r--r--   0        0        0     5141 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/project/test_definition_manager.py
+-rw-r--r--   0        0        0     6898 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/project/test_util.py
+-rw-r--r--   0        0        0    19709 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/project/__snapshots__/test_config.ambr
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/snowpark/__init__.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/snowpark/mocks.py
+-rw-r--r--   0        0        0     7344 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/snowpark/test_anaconda.py
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/snowpark/test_build.py
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/snowpark/test_common.py
+-rw-r--r--   0        0        0    11492 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/snowpark/test_function.py
+-rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/snowpark/test_models.py
+-rw-r--r--   0        0        0     7165 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/snowpark/test_package.py
+-rw-r--r--   0        0        0    14097 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/snowpark/test_procedure.py
+-rw-r--r--   0        0        0     3116 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/snowpark/__snapshots__/test_function.ambr
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/snowpark/__snapshots__/test_package.ambr
+-rw-r--r--   0        0        0     4926 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/snowpark/__snapshots__/test_procedure.ambr
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/snowpark/__snapshots__/test_procedure_coverage.ambr
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/spcs/__init__.py
+-rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/spcs/test_common.py
+-rw-r--r--   0        0        0    16282 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/spcs/test_compute_pool.py
+-rw-r--r--   0        0        0     9321 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/spcs/test_image_repository.py
+-rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/spcs/test_jobs.py
+-rw-r--r--   0        0        0     6694 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/spcs/test_registry.py
+-rw-r--r--   0        0        0    22547 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/spcs/test_services.py
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/spcs/__snapshots__/test_image_repository.ambr
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/spcs/__snapshots__/test_registry.ambr
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/stage/__init__.py
+-rw-r--r--   0        0        0     7385 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/stage/test_diff.py
+-rw-r--r--   0        0        0    29844 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/stage/test_stage.py
+-rw-r--r--   0        0        0     7770 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/stage/__snapshots__/test_stage.ambr
+-rw-r--r--   0        0        0    23568 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/streamlit/test_commands.py
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/streamlit/test_config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/__init__.py
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/anaconda_channel_data.json
+-rw-r--r--   0        0        0     7793 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/packages_available_in_snowflake_sql_result_rows.json
+-rw-r--r--   0        0        0     4526 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/test_data.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/test_streamlit_requirements.txt
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/configs/broken_plugin_config.toml
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/configs/disabled_override_plugin_config.toml
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/configs/failing_plugin_config.toml
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/configs/override_plugin_config.toml
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/INSTALLER
+-rwxr-xr-x   0        0        0     1080 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/LICENSE.txt
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/METADATA
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/REQUESTED
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/WHEEL
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/top_level.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/azure/core/file.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/azure/eventhub/file.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/LICENSE
+-rw-r--r--   0        0        0    36617 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/METADATA
+-rw-r--r--   0        0        0    11535 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/RECORD
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/WHEEL
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/top_level.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/LICENSE
+-rw-r--r--   0        0        0    66103 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/METADATA
+-rw-r--r--   0        0        0    17195 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/REQUESTED
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/WHEEL
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/top_level.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/httplib2/file.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     2618 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/METADATA
+-rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/RECORD
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/WHEEL
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/zendesk/file.txt
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/empty_project/snowflake.yml
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/example_streamlit/environment.yml
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/example_streamlit/snowflake.yml
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/example_streamlit/streamlit_app.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/example_streamlit/pages/my_page.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/example_streamlit_no_defaults/main.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/example_streamlit_no_defaults/snowflake.yml
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/example_streamlit_no_defaults/streamlit_environment.yml
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/example_streamlit_no_defaults/streamlit_pages/first_page.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/example_streamlit_no_stage/environment.yml
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/example_streamlit_no_stage/snowflake.yml
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/example_streamlit_no_stage/streamlit_app.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/example_streamlit_no_stage/pages/my_page.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/integration/snowflake.yml
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/integration/app/README.md
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/integration/app/manifest.yml
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/integration/app/setup.sql
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/integration/package/001-shared.sql
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/integration/package/002-shared.sql
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/integration_external/snowflake.local.yml
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/integration_external/snowflake.yml
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/integration_external/app/README.md
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/integration_external/app/manifest.yml
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/integration_external/app/setup.sql
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/integration_external/package/001-shared.sql
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/integration_external/package/002-shared.sql
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/minimal/snowflake.yml
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/napp_project_1/001-shared.sql
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/napp_project_1/002-shared.sql
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/napp_project_1/setup.sql
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/napp_project_1/snowflake.local.yml
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/napp_project_1/snowflake.yml
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/napp_project_1/app/README.md
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/napp_project_1/app/streamlit/config.py
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/napp_project_1/app/streamlit/main.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/napp_project_with_pkg_warehouse/001-shared.sql
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/napp_project_with_pkg_warehouse/002-shared.sql
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/napp_project_with_pkg_warehouse/setup.sql
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/napp_project_with_pkg_warehouse/snowflake.local.yml
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/napp_project_with_pkg_warehouse/snowflake.yml
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/napp_project_with_pkg_warehouse/app/README.md
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/napp_project_with_pkg_warehouse/app/streamlit/config.py
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/napp_project_with_pkg_warehouse/app/streamlit/main.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/no_definition_version/snowflake.yml
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_function_external_access/app.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_function_external_access/app.zip
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_function_external_access/requirements.txt
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_function_external_access/snowflake.yml
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_function_fully_qualified_name/app.zip
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_function_fully_qualified_name/requirements.txt
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_function_fully_qualified_name/snowflake.yml
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_function_fully_qualified_name/app/app.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_function_secrets_without_external_access/app.zip
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_function_secrets_without_external_access/snowflake.yml
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_functions/app.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_functions/app.zip
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_functions/requirements.txt
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_functions/snowflake.yml
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_procedure_external_access/app.py
+-rw-r--r--   0        0        0     3727 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_procedure_external_access/app.zip
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_procedure_external_access/requirements.txt
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_procedure_external_access/snowflake.yml
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_procedure_fully_qualified_name/app.zip
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_procedure_fully_qualified_name/requirements.txt
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_procedure_fully_qualified_name/snowflake.yml
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_procedure_fully_qualified_name/app/app.py
+-rw-r--r--   0        0        0     3727 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_procedure_secrets_without_external_access/app.zip
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_procedure_secrets_without_external_access/snowflake.yml
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_procedures/app.py
+-rw-r--r--   0        0        0     3727 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_procedures/app.zip
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_procedures/requirements.txt
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_procedures/snowflake.yml
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_procedures_coverage/app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_procedures_coverage/app.zip
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_procedures_coverage/requirements.txt
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_procedures_coverage/snowflake.yml
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/streamlit_full_definition/environment.yml
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/streamlit_full_definition/snowflake.yml
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/streamlit_full_definition/streamlit_app.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/streamlit_full_definition/pages/my_page.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/streamlit_full_definition/utils/utils.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/underspecified/snowflake.yml
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/unknown_fields/snowflake.yml
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/streamlit/another_file_with_list.yml
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/streamlit/another_file_with_single_item.yml
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/streamlit/with_list_in_source_file.yml
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/streamlit/with_single_item.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/testing_utils/__init__.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/testing_utils/conversion.py
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/testing_utils/files_and_dirs.py
+-rw-r--r--   0        0        0     8445 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/testing_utils/fixtures.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/testing_utils/result_assertions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_e2e/__init__.py
+-rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_e2e/conftest.py
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_e2e/test_error_handling.py
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_e2e/test_installation.py
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_e2e/test_snowpark_examples.py
+-rw-r--r--   0        0        0     3302 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_e2e/__snapshots__/test_installation.ambr
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_e2e/config/config.toml
+-rwxr-xr-x   0        0        0       99 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_e2e/config/malformatted_config.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/__init__.py
+-rw-r--r--   0        0        0     5133 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/conftest.py
+-rw-r--r--   0        0        0     3007 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/snowflake_connector.py
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_config.py
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_connection.py
+-rw-r--r--   0        0        0     5375 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_external_plugins.py
+-rw-r--r--   0        0        0     9649 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_git.py
+-rw-r--r--   0        0        0    19879 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_nativeapp.py
+-rw-r--r--   0        0        0     4208 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_object.py
+-rw-r--r--   0        0        0     7144 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_package.py
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_session_token.py
+-rw-r--r--   0        0        0    28253 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_snowpark.py
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_snowpark_external_access.py
+-rw-r--r--   0        0        0     2980 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_sql.py
+-rw-r--r--   0        0        0     6319 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_stage.py
+-rw-r--r--   0        0        0     8498 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_streamlit.py
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_temporary_connection.py
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_utils.py
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/__snapshots__/test_function.ambr
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/__snapshots__/test_git.ambr
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/__snapshots__/test_package.ambr
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/__snapshots__/test_sql.ambr
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/__snapshots__/test_stage.ambr
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/config/config_with_enabled_all_external_plugins.toml
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/config/config_with_enabled_only_one_external_plugin.toml
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/config/connection_configs.toml
+-rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/scripts/integration_account_setup.sql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/spcs/__init__.py
+-rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/spcs/test_compute_pool.py
+-rw-r--r--   0        0        0     3102 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/spcs/test_image_repository.py
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/spcs/test_jobs.py
+-rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/spcs/test_registry.py
+-rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/spcs/test_services.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/spcs/docker/Dockerfile
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/spcs/docker/bootstrap_containers_setup.sh
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/spcs/docker/echo_service.py
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/spcs/spec/spec.yml
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/spcs/spec/spec_upgrade.yml
+-rw-r--r--   0        0        0     6477 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/spcs/testing_utils/compute_pool_utils.py
+-rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/spcs/testing_utils/spcs_jobs_utils.py
+-rw-r--r--   0        0        0    10521 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/spcs/testing_utils/spcs_services_utils.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/sql_multi_queries.sql
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark/.gitignore
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark/requirements.txt
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark/snowflake.yml
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark/app/app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_coverage/.gitignore
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_coverage/requirements.txt
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_coverage/snowflake.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_coverage/app/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_coverage/app/module/__init__.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_coverage/app/module/procedures.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_external_access/.gitignore
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_external_access/requirements.txt
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_external_access/snowflake.yml
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_external_access/app/app.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_fully_qualified_name/.gitignore
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_fully_qualified_name/requirements.txt
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_fully_qualified_name/snowflake.yml
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_fully_qualified_name/app/app.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_vectorized/.gitignore
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_vectorized/requirements.txt
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_vectorized/snowflake.yml
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_vectorized/app/app.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_version_check/.gitignore
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_version_check/requirements.txt
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_version_check/snowflake.yml
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_version_check/app/app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_with_default_values/requirements.other.txt
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_with_default_values/requirements.txt
+-rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_with_default_values/snowflake.yml
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_with_default_values/app/app.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_with_import/.gitignore
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_with_import/requirements.txt
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_with_import/snowflake.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_with_import/app/__init__.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_with_import/app/functions.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_with_single_requirements_having_no_other_deps/.gitignore
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_with_single_requirements_having_no_other_deps/requirements.txt
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_with_single_requirements_having_no_other_deps/snowflake.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_with_single_requirements_having_no_other_deps/app/__init__.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_with_single_requirements_having_no_other_deps/app/functions.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_with_single_requirements_having_transient_deps/.gitignore
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_with_single_requirements_having_transient_deps/requirements.txt
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_with_single_requirements_having_transient_deps/snowflake.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_with_single_requirements_having_transient_deps/app/__init__.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_with_single_requirements_having_transient_deps/app/functions.py
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/stage_execute/script1.sql
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/stage_execute/script2.sql
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/stage_execute/script3.sql
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/stage_execute/script_template.sql
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/stage_get_directory_structure/script1.sql
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/stage_get_directory_structure/dir/script2.sql
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/stage_get_directory_structure/dir/subdir/script3.sql
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/streamlit/environment.yml
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/streamlit/snowflake.yml
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/streamlit/streamlit_app.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/streamlit/pages/my_page.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/streamlit/utils/utils.py
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/testing_utils/__init__.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/testing_utils/naming_utils.py
+-rw-r--r--   0        0        0    11583 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/testing_utils/snowpark_utils.py
+-rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/testing_utils/sql_utils.py
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/testing_utils/working_directory_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/testing_utils/assertions/__init__.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/testing_utils/assertions/test_file_assertions.py
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/testing_utils/assertions/test_result_assertions.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/.gitignore
+-rw-r--r--   0        0        0    11344 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/LICENSE
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/README.md
+-rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/pyproject.toml
+-rw-r--r--   0        0        0    16123 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/PKG-INFO
```

### Comparing `snowflake_cli_labs-2.2.0/.pre-commit-config.yaml` & `snowflake_cli_labs-2.2.0rc0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/CONTRIBUTING.md` & `snowflake_cli_labs-2.2.0rc0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/RELEASE-NOTES.md` & `snowflake_cli_labs-2.2.0rc0/RELEASE-NOTES.md`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
   * `snow git setup` - wizard setting up a git repository stage and creating all necessary objects
   * `snow git fetch` - fetches latest changes from the origin repository into Snowflake repository
   * `snow git list-brahces` - lists all branches in the repository
   * `snow git list-tags` - lists all tags in the repository
   * `snow git list-files` - lists all files on provided branch/tag/commit
   * `snow git copy` - copies files from provided branch/tag/commit into stage or local directory
   * `snow git execute` - execute immediate files from repository
-* Added command for execute immediate `snow stage execute`
+* Added command for execute immediate `snow object stage execute`
 * Fetching available packages list from Snowflake instead of directly from Anaconda with fallback to the old method (for backward compatibility).
   As the new method requires a connection to Snowflake, it adds connection options to the following commands:
   * `snow snowpark build`
   * `snow snowpark package lookup`
   * `snow snowpark package create`
 
 ## Fixes and improvements
@@ -58,15 +58,14 @@
 * Fixed snowpark build paths for builds with --project option (fixed empty zip issue).
 * More clear error messages in `snow snowpark build` command
 * Adding support for any source supported by `pip` in `snow snowpark`.
 * Fixed version parsing for packages lookup on Snowflake Anaconda Channel
 * Fix handling database/schema/role identifiers containing dashes
 * Fix schema override bug in `snow connection test`
 * Hidden incorrectly working config permissions warning on Windows
-* Make errors from `snow connection test` more meaningful when role, warehouse or database does not exist.
 
 # v2.1.2
 
 ## Fixes and improvements
 * Add `pip` as Snowflake-cli dependency
 * Optimize `connection test` command
 * Fix venv creation issues in `snowpark package create` and `snowpark build` command
```

### Comparing `snowflake_cli_labs-2.2.0/performance_history_analysis.py` & `snowflake_cli_labs-2.2.0rc0/performance_history_analysis.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/docs/images/coverage_1.png` & `snowflake_cli_labs-2.2.0rc0/docs/images/coverage_1.png`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/docs/images/coverage_2.png` & `snowflake_cli_labs-2.2.0rc0/docs/images/coverage_2.png`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/docs/images/coverage_3.png` & `snowflake_cli_labs-2.2.0rc0/docs/images/coverage_3.png`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/docs/images/coverage_4.png` & `snowflake_cli_labs-2.2.0rc0/docs/images/coverage_4.png`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/docs/images/coverage_5.png` & `snowflake_cli_labs-2.2.0rc0/docs/images/coverage_5.png`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/api/__init__.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/__init__.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/api/cli_global_context.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/cli_global_context.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/api/config.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/config.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/api/constants.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/constants.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/api/exceptions.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/api/feature_flags.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/feature_flags.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/api/secure_path.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/secure_path.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/api/secure_utils.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/secure_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/api/sql_execution.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/sql_execution.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,21 +60,15 @@
         *_, last_result = self._execute_queries(query, **kwargs)
         return last_result
 
     def _execute_queries(self, queries: str, **kwargs):
         return list(self._execute_string(dedent(queries), **kwargs))
 
     def use(self, object_type: ObjectType, name: str):
-        try:
-            self._execute_query(f"use {object_type.value.sf_name} {name}")
-        except ProgrammingError:
-            # Rewrite the error to make the message more useful.
-            raise ProgrammingError(
-                f"Could not use {object_type} {name}. Object does not exist, or operation cannot be performed."
-            )
+        return self._execute_query(f"use {object_type.value.sf_name} {name}")
 
     @contextmanager
     def use_role(self, new_role: str):
         """
         Switches to a different role for a while, then switches back.
         This is a no-op if the requested role is already active.
         """
```

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/api/commands/decorators.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/commands/decorators.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/api/commands/flags.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/commands/flags.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/api/commands/project_initialisation.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/commands/project_initialisation.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/api/commands/snow_typer.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/commands/snow_typer.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/api/console/abc.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/console/abc.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/api/console/console.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/console/console.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/api/output/types.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/output/types.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/api/plugins/command/__init__.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/plugins/command/__init__.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/api/project/definition.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/definition.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/api/project/definition_manager.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/definition_manager.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/api/project/errors.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/errors.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/api/project/util.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/util.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/api/project/schemas/project_definition.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/schemas/project_definition.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/api/project/schemas/updatable_model.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/schemas/updatable_model.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/api/project/schemas/native_app/application.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/schemas/native_app/application.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/api/project/schemas/native_app/native_app.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/schemas/native_app/native_app.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/api/project/schemas/native_app/package.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/schemas/native_app/package.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/api/project/schemas/snowpark/callable.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/schemas/snowpark/callable.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/api/project/schemas/snowpark/snowpark.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/schemas/snowpark/snowpark.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/api/project/schemas/streamlit/streamlit.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/schemas/streamlit/streamlit.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/api/utils/cursor.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/utils/cursor.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/api/utils/naming_utils.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/utils/naming_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/api/utils/path_utils.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/utils/path_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/api/utils/rendering.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/utils/rendering.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/app/cli_app.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/cli_app.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/app/loggers.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/loggers.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/app/main_typer.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/main_typer.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/app/printing.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/printing.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/app/snow_connector.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/snow_connector.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/app/telemetry.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/telemetry.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/app/api_impl/plugin/plugin_config_provider_impl.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/api_impl/plugin/plugin_config_provider_impl.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/app/commands_registration/builtin_plugins.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/commands_registration/builtin_plugins.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/app/commands_registration/command_plugins_loader.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/commands_registration/command_plugins_loader.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/app/commands_registration/commands_registration_with_callbacks.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/commands_registration/commands_registration_with_callbacks.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/app/commands_registration/threadsafe.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/commands_registration/threadsafe.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/app/commands_registration/typer_registration.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/commands_registration/typer_registration.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/app/dev/commands_structure.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/dev/commands_structure.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/app/dev/pycharm_remote_debug.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/dev/pycharm_remote_debug.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/app/dev/docs/generator.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/dev/docs/generator.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/app/dev/docs/templates/usage.rst.jinja2` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/dev/docs/templates/usage.rst.jinja2`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/connection/commands.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/connection/commands.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/connection/util.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/connection/util.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/git/commands.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/git/commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -197,15 +197,15 @@
     requires_connection=True,
 )
 def fetch(
     repository_name: str = RepoNameArgument,
     **options,
 ) -> CommandResult:
     """
-    Fetch changes from origin to Snowflake repository.
+    Fetch changes from origin to snowflake repository.
     """
     return QueryResult(GitManager().fetch(repo_name=repository_name))
 
 
 @app.command(
     "copy",
     requires_connection=True,
```

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/git/manager.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/git/manager.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/nativeapp/artifacts.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/artifacts.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/nativeapp/commands.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/commands.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/nativeapp/common_flags.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/common_flags.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/nativeapp/constants.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/constants.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/nativeapp/exceptions.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/exceptions.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/nativeapp/init.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/init.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/nativeapp/manager.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/manager.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/nativeapp/policy.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/policy.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/nativeapp/run_processor.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/run_processor.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/nativeapp/teardown_processor.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/teardown_processor.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/nativeapp/utils.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/utils.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/nativeapp/version/commands.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/version/commands.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/nativeapp/version/version_processor.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/version/version_processor.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/object/commands.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/object/commands.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/object/common.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/object/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 @dataclass
 class Tag:
     name: str
     value: str
 
     def __post_init__(self):
         if not is_valid_identifier(self.name):
-            raise ValueError("name of a tag must be a valid Snowflake identifier")
+            raise ValueError("name of a tag must be a valid snowflake identifier")
 
     def value_string_literal(self):
         return to_string_literal(self.value)
 
 
 class TagError(ClickException):
     def __init__(self):
```

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/object/manager.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/object/manager.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/object/stage_deprecated/commands.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/object/stage_deprecated/commands.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/render/commands.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/render/commands.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/snowpark/commands.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/snowpark/commands.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/snowpark/common.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/snowpark/common.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/snowpark/manager.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/snowpark/manager.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/snowpark/models.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/snowpark/models.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/snowpark/package_utils.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/snowpark/package_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/snowpark/snowpark_package_paths.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/snowpark/snowpark_package_paths.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/snowpark/snowpark_shared.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/snowpark/snowpark_shared.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/snowpark/venv.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/snowpark/venv.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/snowpark/zipper.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/snowpark/zipper.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/snowpark/package/anaconda_packages.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/snowpark/package/anaconda_packages.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
     def is_package_available(
         self, package: Requirement, skip_version_check: bool = False
     ) -> bool:
         """
         Checks of a requirement is available in the Snowflake Anaconda Channel.
 
-        As Snowflake currently doesn't support extra syntax (ex. `jinja2[diagrams]`), if such
+        As snowflake currently doesn't support extra syntax (ex. `jinja2[diagrams]`), if such
         extra is present in the dependency, we mark it as unavailable.
         """
         if not package.name or package.extras:
             return False
         if package.name not in self._packages:
             return False
         if skip_version_check or not package.specs:
```

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/snowpark/package/commands.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/snowpark/package/commands.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/snowpark/package/manager.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/snowpark/package/manager.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/spcs/__init__.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/__init__.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/spcs/common.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/common.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/spcs/compute_pool/commands.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/compute_pool/commands.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/spcs/compute_pool/manager.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/compute_pool/manager.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/spcs/image_registry/commands.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/image_registry/commands.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/spcs/image_registry/manager.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/image_registry/manager.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/spcs/image_repository/commands.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/image_repository/commands.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/spcs/image_repository/manager.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/image_repository/manager.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/spcs/jobs/commands.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/jobs/commands.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/spcs/jobs/manager.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/jobs/manager.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/spcs/services/commands.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/services/commands.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/spcs/services/manager.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/services/manager.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/sql/commands.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/sql/commands.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/sql/manager.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/sql/manager.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/stage/commands.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/stage/commands.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/stage/diff.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/stage/diff.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/stage/manager.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/stage/manager.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/streamlit/commands.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/streamlit/commands.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/plugins/streamlit/manager.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/streamlit/manager.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/templates/streamlit_app_launcher.py.jinja` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/templates/streamlit_app_launcher.py.jinja`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/templates/default_snowpark/snowflake.yml` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/templates/default_snowpark/snowflake.yml`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/src/snowflake/cli/templates/default_snowpark/app/procedures.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/templates/default_snowpark/app/procedures.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/test_external_plugins/multilingual_hello_command_group/src/snowflakecli/test_plugins/multilingual_hello/commands.py` & `snowflake_cli_labs-2.2.0rc0/test_external_plugins/multilingual_hello_command_group/src/snowflakecli/test_plugins/multilingual_hello/commands.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/test_external_plugins/multilingual_hello_command_group/src/snowflakecli/test_plugins/multilingual_hello/manager.py` & `snowflake_cli_labs-2.2.0rc0/test_external_plugins/multilingual_hello_command_group/src/snowflakecli/test_plugins/multilingual_hello/manager.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/test_external_plugins/snowpark_hello_single_command/src/snowflakecli/test_plugins/snowpark_hello/commands.py` & `snowflake_cli_labs-2.2.0rc0/test_external_plugins/snowpark_hello_single_command/src/snowflakecli/test_plugins/snowpark_hello/commands.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/test_external_plugins/snowpark_hello_single_command/src/snowflakecli/test_plugins/snowpark_hello/manager.py` & `snowflake_cli_labs-2.2.0rc0/test_external_plugins/snowpark_hello_single_command/src/snowflakecli/test_plugins/snowpark_hello/manager.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/conftest.py` & `snowflake_cli_labs-2.2.0rc0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/test_cli.py` & `snowflake_cli_labs-2.2.0rc0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/test_command_registration.py` & `snowflake_cli_labs-2.2.0rc0/tests/test_command_registration.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/test_common_decorators.py` & `snowflake_cli_labs-2.2.0rc0/tests/test_common_decorators.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/test_common_global_context.py` & `snowflake_cli_labs-2.2.0rc0/tests/test_common_global_context.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/test_config.py` & `snowflake_cli_labs-2.2.0rc0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/test_connection.py` & `snowflake_cli_labs-2.2.0rc0/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/test_experimental_behaviour.py` & `snowflake_cli_labs-2.2.0rc0/tests/test_experimental_behaviour.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/test_help_messages.py` & `snowflake_cli_labs-2.2.0rc0/tests/test_help_messages.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/test_logs.py` & `snowflake_cli_labs-2.2.0rc0/tests/test_logs.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/test_main.py` & `snowflake_cli_labs-2.2.0rc0/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/test_project_initialisation.py` & `snowflake_cli_labs-2.2.0rc0/tests/test_project_initialisation.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/test_render.py` & `snowflake_cli_labs-2.2.0rc0/tests/test_render.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/test_snow_connector.py` & `snowflake_cli_labs-2.2.0rc0/tests/test_snow_connector.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/test_sql.py` & `snowflake_cli_labs-2.2.0rc0/tests/test_sql.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/test_utils.py` & `snowflake_cli_labs-2.2.0rc0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/test_zipper.py` & `snowflake_cli_labs-2.2.0rc0/tests/test_zipper.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/__snapshots__/test_connection.ambr` & `snowflake_cli_labs-2.2.0rc0/tests/__snapshots__/test_connection.ambr`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/__snapshots__/test_help_messages.ambr` & `snowflake_cli_labs-2.2.0rc0/tests/__snapshots__/test_help_messages.ambr`

 * *Files 0% similar despite different names*

```diff
@@ -1081,15 +1081,15 @@
   '''
 # ---
 # name: test_help_messages[git.fetch]
   '''
                                                                                   
    Usage: default git fetch [OPTIONS] REPOSITORY_NAME                             
                                                                                   
-   Fetch changes from origin to Snowflake repository.                             
+   Fetch changes from origin to snowflake repository.                             
                                                                                   
   ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
   │ *    repository_name      TEXT  Identifier of the git repository. For        │
   │                                 example: my_repo                             │
   │                                 [default: None]                              │
   │                                 [required]                                   │
   ╰──────────────────────────────────────────────────────────────────────────────╯
@@ -1468,15 +1468,15 @@
   │ copy            Copies all files from given state of repository to local     │
   │                 directory or stage.                                          │
   │ execute         Execute immediate all files from the repository path. Files  │
   │                 can be filtered with glob like pattern, e.g.                 │
   │                 `@my_repo/branches/main/*.sql`,                              │
   │                 `@my_repo/branches/main/dev/*`. Only files with `.sql`       │
   │                 extension will be executed.                                  │
-  │ fetch           Fetch changes from origin to Snowflake repository.           │
+  │ fetch           Fetch changes from origin to snowflake repository.           │
   │ list-branches   List all branches in the repository.                         │
   │ list-files      List files from given state of git repository.               │
   │ list-tags       List all tags in the repository.                             │
   │ setup           Sets up a git repository object.                             │
   ╰──────────────────────────────────────────────────────────────────────────────╯
```

### Comparing `snowflake_cli_labs-2.2.0/tests/api/test_feature_flags.py` & `snowflake_cli_labs-2.2.0rc0/tests/api/test_feature_flags.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/api/test_secure_path.py` & `snowflake_cli_labs-2.2.0rc0/tests/api/test_secure_path.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/api/commands/test_flags.py` & `snowflake_cli_labs-2.2.0rc0/tests/api/commands/test_flags.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/api/commands/test_snow_typer.py` & `snowflake_cli_labs-2.2.0rc0/tests/api/commands/test_snow_typer.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/api/commands/__snapshots__/test_flags.ambr` & `snowflake_cli_labs-2.2.0rc0/tests/api/commands/__snapshots__/test_flags.ambr`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/api/commands/__snapshots__/test_snow_typer.ambr` & `snowflake_cli_labs-2.2.0rc0/tests/api/commands/__snapshots__/test_snow_typer.ambr`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/api/console/test_cli_console_output.py` & `snowflake_cli_labs-2.2.0rc0/tests/api/console/test_cli_console_output.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/api/console/test_console_abc.py` & `snowflake_cli_labs-2.2.0rc0/tests/api/console/test_console_abc.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/api/console/test_intermediate_output.py` & `snowflake_cli_labs-2.2.0rc0/tests/api/console/test_intermediate_output.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/app/test_telemetry.py` & `snowflake_cli_labs-2.2.0rc0/tests/app/test_telemetry.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/git/test_git_commands.py` & `snowflake_cli_labs-2.2.0rc0/tests/git/test_git_commands.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/nativeapp/patch_utils.py` & `snowflake_cli_labs-2.2.0rc0/tests/nativeapp/patch_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/nativeapp/test_artifacts.py` & `snowflake_cli_labs-2.2.0rc0/tests/nativeapp/test_artifacts.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/nativeapp/test_commands.py` & `snowflake_cli_labs-2.2.0rc0/tests/nativeapp/test_commands.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/nativeapp/test_init.py` & `snowflake_cli_labs-2.2.0rc0/tests/nativeapp/test_init.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/nativeapp/test_manager.py` & `snowflake_cli_labs-2.2.0rc0/tests/nativeapp/test_manager.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/nativeapp/test_package_scripts.py` & `snowflake_cli_labs-2.2.0rc0/tests/nativeapp/test_package_scripts.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/nativeapp/test_run_processor.py` & `snowflake_cli_labs-2.2.0rc0/tests/nativeapp/test_run_processor.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/nativeapp/test_teardown_processor.py` & `snowflake_cli_labs-2.2.0rc0/tests/nativeapp/test_teardown_processor.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/nativeapp/test_utils.py` & `snowflake_cli_labs-2.2.0rc0/tests/nativeapp/test_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/nativeapp/test_version_create_processor.py` & `snowflake_cli_labs-2.2.0rc0/tests/nativeapp/test_version_create_processor.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/nativeapp/test_version_drop_processor.py` & `snowflake_cli_labs-2.2.0rc0/tests/nativeapp/test_version_drop_processor.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/nativeapp/utils.py` & `snowflake_cli_labs-2.2.0rc0/tests/nativeapp/utils.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/nativeapp/__snapshots__/test_commands.ambr` & `snowflake_cli_labs-2.2.0rc0/tests/nativeapp/__snapshots__/test_commands.ambr`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/nativeapp/__snapshots__/test_init.ambr` & `snowflake_cli_labs-2.2.0rc0/tests/nativeapp/__snapshots__/test_init.ambr`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/object/test_common.py` & `snowflake_cli_labs-2.2.0rc0/tests/object/test_common.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/object/test_object.py` & `snowflake_cli_labs-2.2.0rc0/tests/object/test_object.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/object/test_stage.py` & `snowflake_cli_labs-2.2.0rc0/tests/object/test_stage.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/object/__snapshots__/test_object.ambr` & `snowflake_cli_labs-2.2.0rc0/tests/object/__snapshots__/test_object.ambr`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/output/test_format_silent_enforcement.py` & `snowflake_cli_labs-2.2.0rc0/tests/output/test_format_silent_enforcement.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/output/test_printing.py` & `snowflake_cli_labs-2.2.0rc0/tests/output/test_printing.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/output/test_silent_output.py` & `snowflake_cli_labs-2.2.0rc0/tests/output/test_silent_output.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/plugin/test_broken_plugin.py` & `snowflake_cli_labs-2.2.0rc0/tests/plugin/test_broken_plugin.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/plugin/test_failing_plugin.py` & `snowflake_cli_labs-2.2.0rc0/tests/plugin/test_failing_plugin.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/plugin/test_override_by_external_plugins.py` & `snowflake_cli_labs-2.2.0rc0/tests/plugin/test_override_by_external_plugins.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/project/fixtures.py` & `snowflake_cli_labs-2.2.0rc0/tests/project/fixtures.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/project/test_config.py` & `snowflake_cli_labs-2.2.0rc0/tests/project/test_config.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/project/test_definition_manager.py` & `snowflake_cli_labs-2.2.0rc0/tests/project/test_definition_manager.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/project/test_util.py` & `snowflake_cli_labs-2.2.0rc0/tests/project/test_util.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/project/__snapshots__/test_config.ambr` & `snowflake_cli_labs-2.2.0rc0/tests/project/__snapshots__/test_config.ambr`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/snowpark/mocks.py` & `snowflake_cli_labs-2.2.0rc0/tests/snowpark/mocks.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/snowpark/test_anaconda.py` & `snowflake_cli_labs-2.2.0rc0/tests/snowpark/test_anaconda.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/snowpark/test_build.py` & `snowflake_cli_labs-2.2.0rc0/tests/snowpark/test_build.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/snowpark/test_common.py` & `snowflake_cli_labs-2.2.0rc0/tests/snowpark/test_common.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/snowpark/test_function.py` & `snowflake_cli_labs-2.2.0rc0/tests/snowpark/test_function.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/snowpark/test_models.py` & `snowflake_cli_labs-2.2.0rc0/tests/snowpark/test_models.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/snowpark/test_package.py` & `snowflake_cli_labs-2.2.0rc0/tests/snowpark/test_package.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/snowpark/test_procedure.py` & `snowflake_cli_labs-2.2.0rc0/tests/snowpark/test_procedure.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/snowpark/__snapshots__/test_function.ambr` & `snowflake_cli_labs-2.2.0rc0/tests/snowpark/__snapshots__/test_function.ambr`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/snowpark/__snapshots__/test_package.ambr` & `snowflake_cli_labs-2.2.0rc0/tests/snowpark/__snapshots__/test_package.ambr`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/snowpark/__snapshots__/test_procedure.ambr` & `snowflake_cli_labs-2.2.0rc0/tests/snowpark/__snapshots__/test_procedure.ambr`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/spcs/test_common.py` & `snowflake_cli_labs-2.2.0rc0/tests/spcs/test_common.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/spcs/test_compute_pool.py` & `snowflake_cli_labs-2.2.0rc0/tests/spcs/test_compute_pool.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/spcs/test_image_repository.py` & `snowflake_cli_labs-2.2.0rc0/tests/spcs/test_image_repository.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/spcs/test_jobs.py` & `snowflake_cli_labs-2.2.0rc0/tests/spcs/test_jobs.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/spcs/test_registry.py` & `snowflake_cli_labs-2.2.0rc0/tests/spcs/test_registry.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/spcs/test_services.py` & `snowflake_cli_labs-2.2.0rc0/tests/spcs/test_services.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/spcs/__snapshots__/test_image_repository.ambr` & `snowflake_cli_labs-2.2.0rc0/tests/spcs/__snapshots__/test_image_repository.ambr`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/spcs/__snapshots__/test_registry.ambr` & `snowflake_cli_labs-2.2.0rc0/tests/spcs/__snapshots__/test_registry.ambr`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/stage/test_diff.py` & `snowflake_cli_labs-2.2.0rc0/tests/stage/test_diff.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/stage/test_stage.py` & `snowflake_cli_labs-2.2.0rc0/tests/stage/test_stage.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/stage/__snapshots__/test_stage.ambr` & `snowflake_cli_labs-2.2.0rc0/tests/stage/__snapshots__/test_stage.ambr`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/streamlit/test_commands.py` & `snowflake_cli_labs-2.2.0rc0/tests/streamlit/test_commands.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/streamlit/test_config.py` & `snowflake_cli_labs-2.2.0rc0/tests/streamlit/test_config.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/test_data/anaconda_channel_data.json` & `snowflake_cli_labs-2.2.0rc0/tests/test_data/anaconda_channel_data.json`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/test_data/packages_available_in_snowflake_sql_result_rows.json` & `snowflake_cli_labs-2.2.0rc0/tests/test_data/packages_available_in_snowflake_sql_result_rows.json`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/test_data/test_data.py` & `snowflake_cli_labs-2.2.0rc0/tests/test_data/test_data.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/LICENSE.txt` & `snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/METADATA` & `snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/RECORD` & `snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/LICENSE` & `snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/METADATA` & `snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/RECORD` & `snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/LICENSE` & `snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/METADATA` & `snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/RECORD` & `snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/LICENSE` & `snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/METADATA` & `snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/RECORD` & `snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/test_data/projects/integration/app/manifest.yml` & `snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/integration/app/manifest.yml`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/test_data/projects/integration_external/app/manifest.yml` & `snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/integration_external/app/manifest.yml`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/test_data/projects/snowpark_function_external_access/app.zip` & `snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_function_external_access/app.zip`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/test_data/projects/snowpark_function_fully_qualified_name/snowflake.yml` & `snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_function_fully_qualified_name/snowflake.yml`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/test_data/projects/snowpark_function_secrets_without_external_access/app.zip` & `snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_function_secrets_without_external_access/app.zip`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/test_data/projects/snowpark_functions/app.zip` & `snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_functions/app.zip`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/test_data/projects/snowpark_procedure_external_access/app.zip` & `snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_procedure_external_access/app.zip`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/test_data/projects/snowpark_procedure_fully_qualified_name/snowflake.yml` & `snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_procedure_fully_qualified_name/snowflake.yml`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/test_data/projects/snowpark_procedure_secrets_without_external_access/app.zip` & `snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_procedure_secrets_without_external_access/app.zip`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/test_data/projects/snowpark_procedures/app.py` & `snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_procedures/app.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/test_data/projects/snowpark_procedures/app.zip` & `snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_procedures/app.zip`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/test_data/projects/snowpark_procedures_coverage/app.py` & `snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_procedures_coverage/app.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/testing_utils/files_and_dirs.py` & `snowflake_cli_labs-2.2.0rc0/tests/testing_utils/files_and_dirs.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests/testing_utils/fixtures.py` & `snowflake_cli_labs-2.2.0rc0/tests/testing_utils/fixtures.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests_e2e/conftest.py` & `snowflake_cli_labs-2.2.0rc0/tests_e2e/conftest.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests_e2e/test_error_handling.py` & `snowflake_cli_labs-2.2.0rc0/tests_e2e/test_error_handling.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests_e2e/test_installation.py` & `snowflake_cli_labs-2.2.0rc0/tests_e2e/test_installation.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests_e2e/test_snowpark_examples.py` & `snowflake_cli_labs-2.2.0rc0/tests_e2e/test_snowpark_examples.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests_e2e/__snapshots__/test_installation.ambr` & `snowflake_cli_labs-2.2.0rc0/tests_e2e/__snapshots__/test_installation.ambr`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests_integration/conftest.py` & `snowflake_cli_labs-2.2.0rc0/tests_integration/conftest.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests_integration/snowflake_connector.py` & `snowflake_cli_labs-2.2.0rc0/tests_integration/snowflake_connector.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests_integration/test_config.py` & `snowflake_cli_labs-2.2.0rc0/tests_integration/test_config.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests_integration/test_connection.py` & `snowflake_cli_labs-2.2.0rc0/tests_integration/test_connection.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,11 +39,8 @@
 def test_connection_not_existing_schema(
     runner, test_database, snowflake_session, snowflake_home
 ):
     schema = "schema_which_does_not_exist"
     with mock_single_env_var(SCHEMA_ENV_PARAMETER, value=schema):
         result = runner.invoke_with_connection(["connection", "test"])
         assert result.exit_code == 1, result.output
-        assert (
-            f'Could not use schema "{schema.upper()}". Object does not exist'
-            in result.output
-        )
+        assert "Object does not exist" in result.output
```

### Comparing `snowflake_cli_labs-2.2.0/tests_integration/test_external_plugins.py` & `snowflake_cli_labs-2.2.0rc0/tests_integration/test_external_plugins.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests_integration/test_git.py` & `snowflake_cli_labs-2.2.0rc0/tests_integration/test_git.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests_integration/test_nativeapp.py` & `snowflake_cli_labs-2.2.0rc0/tests_integration/test_nativeapp.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests_integration/test_object.py` & `snowflake_cli_labs-2.2.0rc0/tests_integration/test_object.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests_integration/test_package.py` & `snowflake_cli_labs-2.2.0rc0/tests_integration/test_package.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests_integration/test_session_token.py` & `snowflake_cli_labs-2.2.0rc0/tests_integration/test_session_token.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests_integration/test_snowpark.py` & `snowflake_cli_labs-2.2.0rc0/tests_integration/test_snowpark.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests_integration/test_snowpark_external_access.py` & `snowflake_cli_labs-2.2.0rc0/tests_integration/test_snowpark_external_access.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests_integration/test_sql.py` & `snowflake_cli_labs-2.2.0rc0/tests_integration/test_sql.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests_integration/test_stage.py` & `snowflake_cli_labs-2.2.0rc0/tests_integration/test_stage.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests_integration/test_streamlit.py` & `snowflake_cli_labs-2.2.0rc0/tests_integration/test_streamlit.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests_integration/test_temporary_connection.py` & `snowflake_cli_labs-2.2.0rc0/tests_integration/test_temporary_connection.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests_integration/test_utils.py` & `snowflake_cli_labs-2.2.0rc0/tests_integration/test_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests_integration/__snapshots__/test_function.ambr` & `snowflake_cli_labs-2.2.0rc0/tests_integration/__snapshots__/test_function.ambr`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests_integration/__snapshots__/test_stage.ambr` & `snowflake_cli_labs-2.2.0rc0/tests_integration/__snapshots__/test_stage.ambr`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests_integration/scripts/integration_account_setup.sql` & `snowflake_cli_labs-2.2.0rc0/tests_integration/scripts/integration_account_setup.sql`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests_integration/spcs/test_compute_pool.py` & `snowflake_cli_labs-2.2.0rc0/tests_integration/spcs/test_compute_pool.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests_integration/spcs/test_image_repository.py` & `snowflake_cli_labs-2.2.0rc0/tests_integration/spcs/test_image_repository.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests_integration/spcs/test_jobs.py` & `snowflake_cli_labs-2.2.0rc0/tests_integration/spcs/test_jobs.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests_integration/spcs/test_registry.py` & `snowflake_cli_labs-2.2.0rc0/tests_integration/spcs/test_registry.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests_integration/spcs/test_services.py` & `snowflake_cli_labs-2.2.0rc0/tests_integration/spcs/test_services.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests_integration/spcs/docker/echo_service.py` & `snowflake_cli_labs-2.2.0rc0/tests_integration/spcs/docker/echo_service.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests_integration/spcs/testing_utils/compute_pool_utils.py` & `snowflake_cli_labs-2.2.0rc0/tests_integration/spcs/testing_utils/compute_pool_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests_integration/spcs/testing_utils/spcs_jobs_utils.py` & `snowflake_cli_labs-2.2.0rc0/tests_integration/spcs/testing_utils/spcs_jobs_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests_integration/spcs/testing_utils/spcs_services_utils.py` & `snowflake_cli_labs-2.2.0rc0/tests_integration/spcs/testing_utils/spcs_services_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests_integration/test_data/projects/snowpark/snowflake.yml` & `snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark/snowflake.yml`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests_integration/test_data/projects/snowpark/app/app.py` & `snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark/app/app.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests_integration/test_data/projects/snowpark_coverage/app/module/procedures.py` & `snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_coverage/app/module/procedures.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests_integration/test_data/projects/snowpark_external_access/snowflake.yml` & `snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_external_access/snowflake.yml`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests_integration/test_data/projects/snowpark_external_access/app/app.py` & `snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_external_access/app/app.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests_integration/test_data/projects/snowpark_fully_qualified_name/snowflake.yml` & `snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_fully_qualified_name/snowflake.yml`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests_integration/test_data/projects/snowpark_fully_qualified_name/app/app.py` & `snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_fully_qualified_name/app/app.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests_integration/test_data/projects/snowpark_with_default_values/snowflake.yml` & `snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_with_default_values/snowflake.yml`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests_integration/testing_utils/naming_utils.py` & `snowflake_cli_labs-2.2.0rc0/tests_integration/testing_utils/naming_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests_integration/testing_utils/snowpark_utils.py` & `snowflake_cli_labs-2.2.0rc0/tests_integration/testing_utils/snowpark_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests_integration/testing_utils/sql_utils.py` & `snowflake_cli_labs-2.2.0rc0/tests_integration/testing_utils/sql_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests_integration/testing_utils/working_directory_utils.py` & `snowflake_cli_labs-2.2.0rc0/tests_integration/testing_utils/working_directory_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/tests_integration/testing_utils/assertions/test_result_assertions.py` & `snowflake_cli_labs-2.2.0rc0/tests_integration/testing_utils/assertions/test_result_assertions.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/LICENSE` & `snowflake_cli_labs-2.2.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/README.md` & `snowflake_cli_labs-2.2.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/pyproject.toml` & `snowflake_cli_labs-2.2.0rc0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0/PKG-INFO` & `snowflake_cli_labs-2.2.0rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: snowflake-cli-labs
-Version: 2.2.0
+Version: 2.2.0rc0
 Summary: Snowflake CLI
 Project-URL: Source code, https://github.com/snowflakedb/snowflake-cli
 Project-URL: Bug Tracker, https://github.com/snowflakedb/snowflake-cli/issues
 Author: Snowflake Inc.
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

