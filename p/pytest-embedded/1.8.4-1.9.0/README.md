# Comparing `tmp/pytest_embedded-1.8.4.tar.gz` & `tmp/pytest_embedded-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_embedded-1.8.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pytest_embedded-1.9.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pytest_embedded-1.8.4.tar` & `pytest_embedded-1.9.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     1094 2024-04-23 07:21:22.781428 pytest_embedded-1.8.4/LICENSE
--rw-r--r--   0        0        0      120 2024-04-23 07:21:22.781428 pytest_embedded-1.8.4/README.md
--rw-r--r--   0        0        0     3345 2024-04-23 07:21:22.781428 pytest_embedded-1.8.4/pyproject.toml
--rw-r--r--   0        0        0      150 2024-04-23 07:21:22.781428 pytest_embedded-1.8.4/pytest_embedded/__init__.py
--rw-r--r--   0        0        0     1487 2024-04-23 07:21:22.781428 pytest_embedded-1.8.4/pytest_embedded/app.py
--rw-r--r--   0        0        0     7556 2024-04-23 07:21:22.781428 pytest_embedded-1.8.4/pytest_embedded/dut.py
--rw-r--r--   0        0        0     6852 2024-04-23 07:21:22.781428 pytest_embedded-1.8.4/pytest_embedded/log.py
--rw-r--r--   0        0        0    55320 2024-04-23 07:21:22.781428 pytest_embedded-1.8.4/pytest_embedded/plugin.py
--rw-r--r--   0        0        0    10807 2024-04-23 07:21:22.781428 pytest_embedded-1.8.4/pytest_embedded/unity.py
--rw-r--r--   0        0        0    10022 2024-04-23 07:21:22.781428 pytest_embedded-1.8.4/pytest_embedded/utils.py
--rw-r--r--   0        0        0    20777 2024-04-23 07:21:22.781428 pytest_embedded-1.8.4/tests/test_base.py
--rw-r--r--   0        0        0     1461 1970-01-01 00:00:00.000000 pytest_embedded-1.8.4/PKG-INFO
+-rw-r--r--   0        0        0     1094 2024-04-25 11:36:08.631318 pytest_embedded-1.9.0/LICENSE
+-rw-r--r--   0        0        0      120 2024-04-25 11:36:08.631318 pytest_embedded-1.9.0/README.md
+-rw-r--r--   0        0        0     3345 2024-04-25 11:36:08.631318 pytest_embedded-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0      200 2024-04-25 11:36:08.631318 pytest_embedded-1.9.0/pytest_embedded/__init__.py
+-rw-r--r--   0        0        0     1487 2024-04-25 11:36:08.631318 pytest_embedded-1.9.0/pytest_embedded/app.py
+-rw-r--r--   0        0        0     7556 2024-04-25 11:36:08.631318 pytest_embedded-1.9.0/pytest_embedded/dut.py
+-rw-r--r--   0        0        0    26482 2024-04-25 11:36:08.631318 pytest_embedded-1.9.0/pytest_embedded/dut_factory.py
+-rw-r--r--   0        0        0     7125 2024-04-25 11:36:08.631318 pytest_embedded-1.9.0/pytest_embedded/log.py
+-rw-r--r--   0        0        0    42768 2024-04-25 11:36:08.631318 pytest_embedded-1.9.0/pytest_embedded/plugin.py
+-rw-r--r--   0        0        0    10807 2024-04-25 11:36:08.631318 pytest_embedded-1.9.0/pytest_embedded/unity.py
+-rw-r--r--   0        0        0    10206 2024-04-25 11:36:08.631318 pytest_embedded-1.9.0/pytest_embedded/utils.py
+-rw-r--r--   0        0        0    20777 2024-04-25 11:36:08.631318 pytest_embedded-1.9.0/tests/test_base.py
+-rw-r--r--   0        0        0     1461 1970-01-01 00:00:00.000000 pytest_embedded-1.9.0/PKG-INFO
```

### Comparing `pytest_embedded-1.8.4/LICENSE` & `pytest_embedded-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_embedded-1.8.4/pyproject.toml` & `pytest_embedded-1.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytest_embedded-1.8.4/pytest_embedded/app.py` & `pytest_embedded-1.9.0/pytest_embedded/app.py`

 * *Files identical despite different names*

### Comparing `pytest_embedded-1.8.4/pytest_embedded/dut.py` & `pytest_embedded-1.9.0/pytest_embedded/dut.py`

 * *Files identical despite different names*

### Comparing `pytest_embedded-1.8.4/pytest_embedded/log.py` & `pytest_embedded-1.9.0/pytest_embedded/log.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,38 @@
 import datetime
 import errno
 import logging
 import multiprocessing
 import os
 import subprocess
+import sys
 import tempfile
 import textwrap
 import uuid
 from multiprocessing import queues
 from typing import AnyStr, List, Optional, Union
 
 import pexpect.fdpexpect
 from pexpect import EOF, TIMEOUT
 from pexpect.utils import poll_ignore_interrupts, select_ignore_interrupts
 
 from .utils import Meta, remove_asci_color_code, to_bytes, to_str
 
+if sys.platform == 'darwin':
+    _ctx = multiprocessing.get_context('fork')
+else:
+    _ctx = multiprocessing.get_context()
+
 
 class MessageQueue(queues.Queue):
+    def __init__(self, *args, **kwargs):
+        if 'ctx' not in kwargs:
+            kwargs['ctx'] = _ctx
+        super().__init__(*args, **kwargs)
+
     def put(self, obj, **kwargs):
         if not isinstance(obj, (str, bytes)):
             super().put(obj, **kwargs)
             return
 
         if obj == '' or obj == b'':
             return
@@ -129,15 +140,15 @@
         else:
             print(to_str(process.stdout.read()))
 
     if process.returncode != expect_returncode:
         raise subprocess.CalledProcessError(process.returncode, process.args)
 
 
-class _PopenRedirectProcess(multiprocessing.Process):
+class _PopenRedirectProcess(_ctx.Process):
     def __init__(self, msg_queue: MessageQueue, logfile: str):
         self._q = msg_queue
 
         self.logfile = logfile
 
         super().__init__(target=self._forward_io, daemon=True)  # killed by the main process
```

### Comparing `pytest_embedded-1.8.4/pytest_embedded/plugin.py` & `pytest_embedded-1.9.0/pytest_embedded/plugin.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,18 +10,16 @@
 import os
 import shelve
 import subprocess
 import sys
 import tempfile
 import typing as t
 import xml.dom.minidom
-from collections import Counter, defaultdict
-from dataclasses import dataclass
+from collections import Counter
 from operator import itemgetter
-from pathlib import Path
 
 import pytest
 from _pytest.config import Config
 from _pytest.fixtures import (
     FixtureDef,
     FixtureRequest,
     SubRequest,
@@ -30,25 +28,40 @@
 )
 from _pytest.main import Session
 from _pytest.outcomes import TEST_OUTCOME
 from _pytest.python import Function
 
 from .app import App
 from .dut import Dut
+from .dut_factory import (
+    DutFactory,
+    _fixture_classes_and_options_fn,
+    _listener_gn,
+    _pexpect_fr_gn,
+    app_fn,
+    dut_gn,
+    gdb_gn,
+    msg_queue_gn,
+    openocd_gn,
+    pexpect_proc_fn,
+    qemu_gn,
+    serial_gn,
+    set_parametrized_fixtures_cache,
+    wokwi_gn,
+)
 from .log import MessageQueue, PexpectProcess
 from .unity import JunitMerger, escape_illegal_xml_chars
 from .utils import (
-    FIXTURES_SERVICES,
     SERVICE_LIB_NAMES,
+    ClassCliOptions,
     Meta,
     PackageNotInstalledError,
     UnknownServiceError,
     find_by_suffix,
     to_list,
-    to_str,
 )
 
 if t.TYPE_CHECKING:
     from pytest_embedded_idf import CaseTester, IdfDut, LinuxSerial
     from pytest_embedded_jtag import Gdb, OpenOcd
     from pytest_embedded_qemu import Qemu
     from pytest_embedded_serial import Serial
@@ -193,15 +206,15 @@
         'Set to True to skip auto check core dump in UART/flash '
         'and panic handler support while teardown the failing test case. '
         'Requires valid partition tool, project_description.json under the build dir. (Default: False)',
     )
     idf_group.addoption(
         '--panic-output-decode-script',
         help='Panic output decode script that is used in conjunction with the check-panic-coredump option '
-        'to parse panic output. (Default: use gdb_panic_server.py from package esp_idf_panic_decoder)',
+        'to parse panic output. (Default: $IDF_PATH/tools/gdb_panic_server.py)',
     )
 
     jtag_group = parser.getgroup('embedded-jtag')
     jtag_group.addoption('--gdb-prog-path', help='GDB program path. (Default: "xtensa-esp32-elf-gdb")')
     jtag_group.addoption(
         '--gdb-cli-args',
         help='GDB cli arguments. (Default: "--quiet"',
@@ -289,18 +302,14 @@
         return True
     elif isinstance(v, str) and v.lower() in ['n', 'no', 'false']:
         return False
     else:
         return v
 
 
-def _drop_none_kwargs(kwargs: t.Dict[t.Any, t.Any]):
-    return {k: v for k, v in kwargs.items() if v is not None}
-
-
 def _prettify_xml(file_path: str):
     dom = xml.dom.minidom.parse(file_path)
     pretty_xml_as_string = dom.toprettyxml()
     with open(file_path, 'w') as f:
         f.write(pretty_xml_as_string)
 
 
@@ -628,118 +637,54 @@
         name = f'dut-{dut_index}'
     else:
         name = 'dut'
 
     return os.path.join(test_case_tempdir, f'{name}{logfile_extension}')
 
 
-# Suppress UserWarning on resource_tracker.py
-if sys.platform == 'darwin':
-    multiprocessing.set_start_method('fork')
-
-_ctx = multiprocessing.get_context()
-_stdout = sys.__stdout__
-
-
 @pytest.fixture
 @multi_dut_generator_fixture
 def msg_queue() -> MessageQueue:  # kwargs passed by `multi_dut_generator_fixture()`
-    return MessageQueue(ctx=_ctx)
+    return msg_queue_gn()
 
 
 @pytest.fixture
 @multi_dut_argument
 def with_timestamp(request: FixtureRequest) -> bool:
     """Enable parametrization for the same cli option"""
     return _request_param_or_config_option_or_default(request, 'with_timestamp', None)
 
 
-def _listen(q: MessageQueue, filepath: str, with_timestamp: bool = True, count: int = 1, total: int = 1) -> None:
-    _added_prefix = False
-    while True:
-        msg = q.get()
-        if not msg:
-            continue
-
-        with open(filepath, 'ab') as fw:
-            fw.write(msg)
-            fw.flush()
-
-        _s = to_str(msg)
-        if not _s:
-            continue
-
-        prefix = ''
-        if total > 1:
-            source = f'dut-{count}'
-        else:
-            source = None
-
-        if source:
-            prefix = f'[{source}] ' + prefix
-
-        if with_timestamp:
-            prefix = datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S') + ' ' + prefix
-
-        if not _added_prefix:
-            _s = prefix + _s
-            _added_prefix = True
-        _s = _s.replace('\r\n', '\n')  # remove extra \r. since multi-dut \r would mess up the log
-        _s = _s.replace('\n', '\n' + prefix)
-        if prefix and _s.endswith(prefix):
-            _s = _s.rsplit(prefix, maxsplit=1)[0]
-            _added_prefix = False
-
-        _stdout.write(_s)
-        _stdout.flush()
-
-
 @pytest.fixture
 @multi_dut_generator_fixture
 def _listener(msg_queue, _pexpect_logfile, with_timestamp, dut_index, dut_total) -> multiprocessing.Process:
     """
     The listener would create a `_listen` process. The `_listen` process would get the string from the message queue,
     and do two things together:
 
     1. print the string to `sys.stdout`
     2. write the string to `_pexpect_logfile`
     """
-    os.makedirs(os.path.dirname(_pexpect_logfile), exist_ok=True)
-    kwargs = {
-        'with_timestamp': with_timestamp,
-        'count': dut_index,
-        'total': dut_total,
-    }
-
-    return _ctx.Process(
-        target=_listen,
-        args=(
-            msg_queue,
-            _pexpect_logfile,
-        ),
-        kwargs=_drop_none_kwargs(kwargs),
-    )
+    return _listener_gn(**locals())
 
 
 @pytest.fixture
 @multi_dut_generator_fixture
 def _pexpect_fr(_pexpect_logfile, _listener) -> t.BinaryIO:
-    Path(_pexpect_logfile).touch()
-    _listener.start()
-    return open(_pexpect_logfile, 'rb')
+    return _pexpect_fr_gn(**locals())
 
 
 @pytest.fixture
 # here we use @multi_dut_fixture
 # otherwise the close() method would be called, and would raise the OSError
 # The file descriptor would be closed at `_pexpect_fr`
 @multi_dut_fixture
 def pexpect_proc(_pexpect_fr) -> PexpectProcess:
     """Pexpect process that run the expect functions on"""
-    return PexpectProcess(_pexpect_fr)
+    return pexpect_proc_fn(**locals())
 
 
 @pytest.fixture
 @multi_dut_generator_fixture
 def redirect(msg_queue: MessageQueue) -> t.Callable[..., contextlib.redirect_stdout]:
     """
     A context manager that could help duplicate all the `sys.stdout` to `msg_queue`.
@@ -1021,24 +966,17 @@
             importlib.import_module(SERVICE_LIB_NAMES[s].replace('-', '_'))
         except ModuleNotFoundError:
             raise PackageNotInstalledError(s)
 
     return ['base', *services]
 
 
-@dataclass
-class ClassCliOptions:
-    classes: t.Dict[str, type]
-    mixins: t.Dict[str, t.List[type]]
-    kwargs: t.Dict[str, t.Dict[str, t.Any]]
-
-
-@pytest.fixture
+@pytest.fixture(autouse=True)
 @multi_dut_fixture
-def _fixture_classes_and_options(
+def parametrize_fixtures(
     _services,
     # parametrize fixtures
     app_path,
     build_dir,
     port,
     port_location,
     port_mac,
@@ -1064,21 +1002,37 @@
     qemu_cli_args,
     qemu_extra_args,
     wokwi_cli_path,
     wokwi_timeout,
     skip_regenerate_image,
     encrypt,
     keyfile,
+    # common fixtures
+    test_case_name,
+    _meta,
+):
+    set_parametrized_fixtures_cache(locals())
+    return locals()
+
+
+@pytest.fixture(autouse=True)
+def close_factory_duts():
+    yield
+    DutFactory.close()
+
+
+@pytest.fixture
+@multi_dut_fixture
+def _fixture_classes_and_options(
+    parametrize_fixtures,
     # pre-initialized fixtures
     dut_index,
     _pexpect_logfile,
-    test_case_name,
     pexpect_proc,
     msg_queue,
-    _meta,
 ) -> ClassCliOptions:
     """
     classes: the class that the fixture should instantiate
     {
         <fixture_name>: <class_name>,
         ...
     }
@@ -1090,320 +1044,63 @@
             ...
         },
         }
     }
         ...
     }
     """
-    classes: t.Dict[str, type] = {}
-    mixins: t.Dict[str, t.List[type]] = defaultdict(list)
-    kwargs: t.Dict[str, t.Dict[str, t.Any]] = defaultdict(dict)
-
-    for fixture in FIXTURES_SERVICES.keys():
-        if fixture == 'app':
-            kwargs['app'] = {'app_path': app_path, 'build_dir': build_dir}
-            if 'idf' in _services:
-                if 'qemu' in _services:
-                    from pytest_embedded_qemu import DEFAULT_IMAGE_FN, QemuApp
-
-                    classes[fixture] = QemuApp
-                    kwargs[fixture].update({
-                        'msg_queue': msg_queue,
-                        'part_tool': part_tool,
-                        'qemu_image_path': qemu_image_path,
-                        'skip_regenerate_image': skip_regenerate_image,
-                        'encrypt': encrypt,
-                        'keyfile': keyfile,
-                        'qemu_prog_path': qemu_prog_path,
-                    })
-                else:
-                    from pytest_embedded_idf import IdfApp
+    kwargs = locals()
+    kwargs.update(kwargs.pop('parametrize_fixtures'))
 
-                    classes[fixture] = IdfApp
-                    kwargs[fixture].update({
-                        'part_tool': part_tool,
-                    })
-            elif 'arduino' in _services:
-                from pytest_embedded_arduino import ArduinoApp
-
-                classes[fixture] = ArduinoApp
-            else:
-                from .app import App
-
-                classes[fixture] = App
-        elif fixture == 'serial':
-            if 'esp' in _services:
-                from pytest_embedded_serial_esp import EspSerial
-
-                kwargs[fixture] = {
-                    'pexpect_proc': pexpect_proc,
-                    'msg_queue': msg_queue,
-                    'target': target,
-                    'beta_target': beta_target,
-                    'port': os.getenv('ESPPORT') or port,
-                    'port_location': port_location,
-                    'port_mac': port_mac,
-                    'baud': int(baud or EspSerial.DEFAULT_BAUDRATE),
-                    'esptool_baud': int(os.getenv('ESPBAUD') or esptool_baud or EspSerial.ESPTOOL_DEFAULT_BAUDRATE),
-                    'esp_flash_force': esp_flash_force,
-                    'skip_autoflash': skip_autoflash,
-                    'erase_all': erase_all,
-                    'meta': _meta,
-                }
-                if 'idf' in _services:
-                    from pytest_embedded_idf import IdfSerial
-
-                    classes[fixture] = IdfSerial
-                    kwargs[fixture].update({
-                        'app': None,
-                        'confirm_target_elf_sha256': confirm_target_elf_sha256,
-                        'erase_nvs': erase_nvs,
-                    })
-                elif 'arduino' in _services:
-                    from pytest_embedded_arduino import ArduinoSerial
-
-                    classes[fixture] = ArduinoSerial
-                    kwargs[fixture].update({
-                        'app': None,
-                    })
-                else:
-                    from pytest_embedded_serial_esp import EspSerial
-
-                    classes[fixture] = EspSerial
-            elif 'serial' in _services or 'jtag' in _services:
-                from pytest_embedded_serial.serial import Serial
-
-                classes[fixture] = Serial
-                kwargs[fixture] = {
-                    'msg_queue': msg_queue,
-                    'port': port,
-                    'port_location': port_location,
-                    'baud': int(baud or Serial.DEFAULT_BAUDRATE),
-                    'meta': _meta,
-                }
-        elif fixture in ['openocd', 'gdb']:
-            if 'jtag' in _services:
-                if fixture == 'openocd':
-                    from pytest_embedded_jtag import OpenOcd
-
-                    classes[fixture] = OpenOcd
-                    kwargs[fixture] = {
-                        'msg_queue': msg_queue,
-                        'app': None,
-                        'openocd_prog_path': openocd_prog_path,
-                        'openocd_cli_args': openocd_cli_args,
-                        'port_offset': dut_index,
-                        'meta': _meta,
-                    }
-                elif not no_gdb:
-                    from pytest_embedded_jtag import Gdb
-
-                    classes[fixture] = Gdb
-                    kwargs[fixture] = {
-                        'msg_queue': msg_queue,
-                        'gdb_prog_path': gdb_prog_path,
-                        'gdb_cli_args': gdb_cli_args,
-                        'meta': _meta,
-                    }
-        elif fixture == 'qemu':
-            if 'qemu' in _services:
-                from pytest_embedded_qemu import (
-                    DEFAULT_IMAGE_FN,
-                    ENCRYPTED_IMAGE_FN,
-                    Qemu,
-                )
-
-                classes[fixture] = Qemu
-                kwargs[fixture] = {
-                    'msg_queue': msg_queue,
-                    'qemu_image_path': qemu_image_path
-                    or os.path.join(
-                        app_path or '', build_dir or 'build', ENCRYPTED_IMAGE_FN if encrypt else DEFAULT_IMAGE_FN
-                    ),
-                    'qemu_prog_path': qemu_prog_path,
-                    'qemu_cli_args': qemu_cli_args,
-                    'qemu_extra_args': qemu_extra_args,
-                    'app': None,
-                    'meta': _meta,
-                    'dut_index': dut_index,
-                }
-        elif fixture == 'wokwi':
-            if 'wokwi' in _services:
-                from pytest_embedded_wokwi import WokwiCLI
-
-                classes[fixture] = WokwiCLI
-                kwargs[fixture].update({
-                    'wokwi_cli_path': wokwi_cli_path,
-                    'wokwi_timeout': wokwi_timeout,
-                    'msg_queue': msg_queue,
-                    'app': None,
-                    'meta': _meta,
-                })
-        elif fixture == 'dut':
-            classes[fixture] = Dut
-            kwargs[fixture] = {
-                'pexpect_proc': pexpect_proc,
-                'msg_queue': msg_queue,
-                'app': None,
-                'pexpect_logfile': _pexpect_logfile,
-                'test_case_name': test_case_name,
-                'meta': _meta,
-            }
-            if 'idf' in _services and 'esp' not in _services:
-                # esp,idf will use IdfDut, which based on IdfUnityDutMixin already
-                from pytest_embedded_idf.unity_tester import IdfUnityDutMixin
-
-                mixins[fixture].append(IdfUnityDutMixin)
-
-            if 'wokwi' in _services:
-                from pytest_embedded_wokwi import WokwiDut
-
-                classes[fixture] = WokwiDut
-                kwargs[fixture].update({
-                    'wokwi': None,
-                })
-
-                if 'idf' in _services:
-                    from pytest_embedded_wokwi.idf import IDFFirmwareResolver
-
-                    kwargs['wokwi'].update({'firmware_resolver': IDFFirmwareResolver()})
-                else:
-                    raise SystemExit('wokwi service should be used together with idf service')
-            elif 'qemu' in _services:
-                from pytest_embedded_qemu import QemuDut
-
-                classes[fixture] = QemuDut
-                kwargs[fixture].update({
-                    'qemu': None,
-                })
-            elif 'jtag' in _services:
-                if 'idf' in _services:
-                    from pytest_embedded_idf import IdfDut
-
-                    classes[fixture] = IdfDut
-                else:
-                    from pytest_embedded_serial import SerialDut
-
-                    classes[fixture] = SerialDut
-
-                kwargs[fixture].update({
-                    'serial': None,
-                    'openocd': None,
-                    'gdb': None,
-                })
-            elif 'serial' in _services or 'esp' in _services:
-                if 'esp' in _services and 'idf' in _services:
-                    from pytest_embedded_idf import IdfDut
-
-                    classes[fixture] = IdfDut
-                    kwargs[fixture].update({
-                        'skip_check_coredump': skip_check_coredump,
-                        'panic_output_decode_script': panic_output_decode_script,
-                    })
-                else:
-                    from pytest_embedded_serial import SerialDut
-
-                    classes[fixture] = SerialDut
-
-                kwargs[fixture].update({
-                    'serial': None,
-                })
-
-    return ClassCliOptions(classes, mixins, kwargs)
+    return _fixture_classes_and_options_fn(**kwargs)
 
 
 ####################
 # Derived Fixtures #
 ####################
 @pytest.fixture
 @multi_dut_fixture
 def app(_fixture_classes_and_options: ClassCliOptions) -> App:
     """A pytest fixture to gather information from the specified built binary folder"""
-    cls = _fixture_classes_and_options.classes['app']
-    kwargs = _fixture_classes_and_options.kwargs['app']
-    return cls(**_drop_none_kwargs(kwargs))
+    return app_fn(**locals())
 
 
 @pytest.fixture
 @multi_dut_generator_fixture
 def serial(_fixture_classes_and_options, msg_queue, app) -> t.Optional[t.Union['Serial', 'LinuxSerial']]:
     """A serial subprocess that could read/redirect/write"""
-    if hasattr(app, 'target') and app.target == 'linux':
-        from pytest_embedded_idf import LinuxSerial
-
-        cls = LinuxSerial
-        kwargs = {
-            'app': app,
-            'msg_queue': msg_queue,
-        }
-        return cls(**kwargs)
-
-    if 'serial' not in _fixture_classes_and_options.classes:
-        return None
-
-    cls = _fixture_classes_and_options.classes['serial']
-    kwargs = _fixture_classes_and_options.kwargs['serial']
-    if 'app' in kwargs and kwargs['app'] is None:
-        kwargs['app'] = app
-    return cls(**_drop_none_kwargs(kwargs))
+    return serial_gn(**locals())
 
 
 @pytest.fixture
 @multi_dut_generator_fixture
 def openocd(_fixture_classes_and_options: ClassCliOptions) -> t.Optional['OpenOcd']:
     """An openocd subprocess that could read/redirect/write"""
-    if 'openocd' not in _fixture_classes_and_options.classes:
-        return None
-
-    cls = _fixture_classes_and_options.classes['openocd']
-    kwargs = _fixture_classes_and_options.kwargs['openocd']
-    return cls(**_drop_none_kwargs(kwargs))
+    return openocd_gn(**locals())
 
 
 @pytest.fixture
 @multi_dut_generator_fixture
 def gdb(_fixture_classes_and_options: ClassCliOptions) -> t.Optional['Gdb']:
     """A gdb subprocess that could read/redirect/write"""
-    if 'gdb' not in _fixture_classes_and_options.classes:
-        return None
-
-    cls = _fixture_classes_and_options.classes['gdb']
-    kwargs = _fixture_classes_and_options.kwargs['gdb']
-    return cls(**_drop_none_kwargs(kwargs))
+    return gdb_gn(**locals())
 
 
 @pytest.fixture
 @multi_dut_generator_fixture
 def qemu(_fixture_classes_and_options: ClassCliOptions, app) -> t.Optional['Qemu']:
     """A qemu subprocess that could read/redirect/write"""
-    if 'qemu' not in _fixture_classes_and_options.classes:
-        return None
-
-    cls = _fixture_classes_and_options.classes['qemu']
-    kwargs = _fixture_classes_and_options.kwargs['qemu']
-
-    if 'app' in kwargs and kwargs['app'] is None:
-        kwargs['app'] = app
-
-    return cls(**_drop_none_kwargs(kwargs))
+    return qemu_gn(**locals())
 
 
 @pytest.fixture
 @multi_dut_generator_fixture
 def wokwi(_fixture_classes_and_options: ClassCliOptions, app) -> t.Optional['WokwiCLI']:
     """A wokwi subprocess that could read/redirect/write"""
-    if 'wokwi' not in _fixture_classes_and_options.classes:
-        return None
-
-    cls = _fixture_classes_and_options.classes['wokwi']
-    kwargs = _fixture_classes_and_options.kwargs['wokwi']
-
-    if 'app' in kwargs and kwargs['app'] is None:
-        kwargs['app'] = app
-    return cls(**_drop_none_kwargs(kwargs))
+    return wokwi_gn(**locals())
 
 
 @pytest.fixture
 @multi_dut_generator_fixture
 def dut(
     _fixture_classes_and_options: ClassCliOptions,
     openocd: t.Optional['OpenOcd'],
@@ -1413,42 +1110,15 @@
     qemu: t.Optional['Qemu'],
     wokwi: t.Optional['WokwiCLI'],
 ) -> t.Union[Dut, t.List[Dut]]:
     """
     A device under test (DUT) object that could gather output from various sources and redirect them to the pexpect
     process, and run `expect()` via its pexpect process.
     """
-    kwargs = _fixture_classes_and_options.kwargs['dut']
-    mixins = _fixture_classes_and_options.mixins['dut']
-
-    # since there's no way to know the target before setup finished
-    # we have to use the `app.target` to determine the dut class here
-    if hasattr(app, 'target') and app.target == 'linux':
-        from pytest_embedded_idf import LinuxDut
-
-        cls = LinuxDut
-        kwargs['serial'] = None  # replace it later with LinuxSerial
-    else:
-        cls = _fixture_classes_and_options.classes['dut']
-
-    for k, v in kwargs.items():
-        if v is None:
-            if k == 'app':
-                kwargs[k] = app
-            elif k == 'serial':
-                kwargs[k] = serial
-            elif k == 'openocd':
-                kwargs[k] = openocd
-            elif k == 'gdb':
-                kwargs[k] = gdb
-            elif k == 'qemu':
-                kwargs[k] = qemu
-            elif k == 'wokwi':
-                kwargs[k] = wokwi
-    return cls(**_drop_none_kwargs(kwargs), mixins=mixins)
+    return dut_gn(**locals())
 
 
 @pytest.fixture
 def unity_tester(dut: t.Union['IdfDut', t.Tuple['IdfDut']]) -> t.Optional['CaseTester']:
     try:
         from pytest_embedded_idf import CaseTester, IdfDut
     except ImportError:
```

### Comparing `pytest_embedded-1.8.4/pytest_embedded/unity.py` & `pytest_embedded-1.9.0/pytest_embedded/unity.py`

 * *Files identical despite different names*

### Comparing `pytest_embedded-1.8.4/pytest_embedded/utils.py` & `pytest_embedded-1.9.0/pytest_embedded/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import dataclasses
 import functools
 import importlib
 import logging
 import os
 import re
 import typing as t
+from dataclasses import dataclass
 
 if t.TYPE_CHECKING:
     from . import App
 
 #############
 # Constants #
 #############
@@ -30,14 +31,22 @@
     'openocd': ['jtag'],
     'gdb': ['jtag'],
     'qemu': ['qemu'],
     'wokwi': ['wokwi'],
     'dut': ['base', 'serial', 'jtag', 'qemu', 'idf', 'wokwi'],
 }
 
+
+@dataclass
+class ClassCliOptions:
+    classes: t.Dict[str, type]
+    mixins: t.Dict[str, t.List[type]]
+    kwargs: t.Dict[str, t.Dict[str, t.Any]]
+
+
 _T = t.TypeVar('_T')
 
 _MIXIN_REQUIRED_SERVICES = {
     'IdfUnityMixin': ['idf'],
 }
 
 _MIXIN_REQUIRED_SERVICES_KEY = '_based_on_services'
```

### Comparing `pytest_embedded-1.8.4/tests/test_base.py` & `pytest_embedded-1.9.0/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `pytest_embedded-1.8.4/PKG-INFO` & `pytest_embedded-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-embedded
-Version: 1.8.4
+Version: 1.9.0
 Summary: A pytest plugin that designed for embedded testing.
 Author-email: Fu Hanxi <fuhanxi@espressif.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
```

