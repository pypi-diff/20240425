# Comparing `tmp/pycxpress-0.0.4.tar.gz` & `tmp/pycxpress-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycxpress-0.0.4.tar", max compression
+gzip compressed data, was "pycxpress-0.0.5.tar", max compression
```

## Comparing `pycxpress-0.0.4.tar` & `pycxpress-0.0.5.tar`

### file list

```diff
@@ -1,12 +1,15 @@
--rw-r--r--   0        0        0     1066 2024-04-22 13:24:18.608510 pycxpress-0.0.4/LICENSE
--rw-r--r--   0        0        0     2324 2024-04-22 13:24:18.608510 pycxpress-0.0.4/README.md
--rw-r--r--   0        0        0     3924 2024-04-22 13:24:18.612510 pycxpress-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1030 2024-04-22 13:24:18.612510 pycxpress-0.0.4/src/PyCXpress/__init__.py
--rw-r--r--   0        0        0      947 2024-04-22 13:24:18.612510 pycxpress-0.0.4/src/PyCXpress/__main__.py
--rw-r--r--   0        0        0     6809 2024-04-22 13:24:18.612510 pycxpress-0.0.4/src/PyCXpress/core.py
--rw-r--r--   0        0        0      832 2024-04-22 13:24:18.612510 pycxpress-0.0.4/src/PyCXpress/example/Makefile
--rw-r--r--   0        0        0     1518 2024-04-22 13:24:18.612510 pycxpress-0.0.4/src/PyCXpress/example/main.cpp
--rw-r--r--   0        0        0     2456 2024-04-22 13:24:18.612510 pycxpress-0.0.4/src/PyCXpress/example/model.py
--rw-r--r--   0        0        0     7361 2024-04-22 13:24:18.612510 pycxpress-0.0.4/src/PyCXpress/include/PyCXpress/core.hpp
--rw-r--r--   0        0        0      849 2024-04-22 13:24:18.612510 pycxpress-0.0.4/src/PyCXpress/include/PyCXpress/utils.hpp
--rw-r--r--   0        0        0     3561 1970-01-01 00:00:00.000000 pycxpress-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-25 17:09:19.066959 pycxpress-0.0.5/LICENSE
+-rw-r--r--   0        0        0     2324 2024-04-25 17:09:19.066959 pycxpress-0.0.5/README.md
+-rw-r--r--   0        0        0     4030 2024-04-25 17:09:19.070959 pycxpress-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1036 2024-04-25 17:09:19.070959 pycxpress-0.0.5/src/PyCXpress/__init__.py
+-rw-r--r--   0        0        0      947 2024-04-25 17:09:19.070959 pycxpress-0.0.5/src/PyCXpress/__main__.py
+-rw-r--r--   0        0        0     5428 2024-04-25 17:09:19.070959 pycxpress-0.0.5/src/PyCXpress/core.py
+-rw-r--r--   0        0        0     1501 2024-04-25 17:09:19.070959 pycxpress-0.0.5/src/PyCXpress/debugger.py
+-rw-r--r--   0        0        0      999 2024-04-25 17:09:19.070959 pycxpress-0.0.5/src/PyCXpress/example/Makefile
+-rw-r--r--   0        0        0     1730 2024-04-25 17:09:19.070959 pycxpress-0.0.5/src/PyCXpress/example/main.cpp
+-rw-r--r--   0        0        0     2633 2024-04-25 17:09:19.070959 pycxpress-0.0.5/src/PyCXpress/example/model.py
+-rw-r--r--   0        0        0     9174 2024-04-25 17:09:19.070959 pycxpress-0.0.5/src/PyCXpress/include/PyCXpress/core.hpp
+-rw-r--r--   0        0        0      849 2024-04-25 17:09:19.070959 pycxpress-0.0.5/src/PyCXpress/include/PyCXpress/utils.hpp
+-rw-r--r--   0        0        0     1033 2024-04-25 17:09:19.070959 pycxpress-0.0.5/src/PyCXpress/interface.py
+-rw-r--r--   0        0        0      714 2024-04-25 17:09:19.070959 pycxpress-0.0.5/src/PyCXpress/utils.py
+-rw-r--r--   0        0        0     3669 1970-01-01 00:00:00.000000 pycxpress-0.0.5/PKG-INFO
```

### Comparing `pycxpress-0.0.4/LICENSE` & `pycxpress-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pycxpress-0.0.4/README.md` & `pycxpress-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pycxpress-0.0.4/pyproject.toml` & `pycxpress-0.0.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "PyCXpress"
-version = "0.0.4"
+version = "0.0.5"
 description = "PyCXpress is a high-performance hybrid framework that seamlessly integrates Python and C++ to harness the flexibility of Python and the speed of C++ for efficient and expressive computation, particularly in the realm of deep learning and numerical computing."
 readme = "README.md"
 authors = ["chaoqing <chaoqingwang.nick@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/chaoqing/PyCXpress"
 homepage = "https://github.com/chaoqing/PyCXpress"
 packages = [
@@ -35,15 +35,18 @@
 [tool.poetry.scripts]
 # Entry points for the package https://python-poetry.org/docs/pyproject/#scripts
 "pycxpress" = "PyCXpress.__main__:main"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pybind11 = "^2.12.0"
-numpy = "^1.22"
+numpy = [
+    {version = "<1.22", python = "~3.8"},
+    {version = "^1.22", python = ">=3.9"}
+]
 
 
 [tool.poetry.dev-dependencies]
 bandit = "^1.7.1"
 black = {version = "^24.4", allow-prereleases = true}
 darglint = "^1.8.1"
 build = "^1.2.1"
@@ -59,14 +62,15 @@
 coverage = "^7.4.4"
 coverage-badge = "^1.1.0"
 pytest-html = "^3.1.1"
 pytest-cov = "^5.0.0"
 
 [tool.poetry.group.dev.dependencies]
 debugpy = "^1.8.1"
+find-libpython = "^0.4.0"
 
 [tool.black]
 # https://github.com/psf/black
 target-version = ["py38"]
 line-length = 88
 color = true
```

### Comparing `pycxpress-0.0.4/src/PyCXpress/__init__.py` & `pycxpress-0.0.5/src/PyCXpress/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,14 @@
     "ModelRuntimeType",
     "convert_to_spec_tuple",
     "pycxpress_debugger",
     "get_include",
     "version",
 ]
 
-import sys
 from importlib import metadata as importlib_metadata
 from pathlib import Path
 
 
 def get_version() -> str:
     try:
         return importlib_metadata.version(__name__)
@@ -28,13 +27,13 @@
 
 from .core import (
     ModelAnnotationCreator,
     ModelAnnotationType,
     ModelRuntimeType,
     TensorMeta,
     convert_to_spec_tuple,
-    pycxpress_debugger,
 )
+from .debugger import pycxpress_debugger
 
 
 def get_include() -> str:
     return str(Path(__file__).parent.absolute() / "include")
```

### Comparing `pycxpress-0.0.4/src/PyCXpress/__main__.py` & `pycxpress-0.0.5/src/PyCXpress/__main__.py`

 * *Files identical despite different names*

### Comparing `pycxpress-0.0.4/src/PyCXpress/core.py` & `pycxpress-0.0.5/src/PyCXpress/core.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,82 +1,25 @@
 # mypy: disable_error_code="type-arg,arg-type,union-attr,operator,assignment,misc"
-import logging
-
-logger = logging.getLogger(__name__)
-
-
 from typing import Callable, Dict, Iterable, List, Optional, Tuple, Union
 
-import os
 from collections import namedtuple
 from dataclasses import dataclass
 from enum import Enum, auto
+from itertools import chain
 
 import numpy as np
 from numpy.typing import DTypeLike
 
-# import tensorflow as tf
-
-
-def pycxpress_debugger(
-    host: Optional[str] = None,
-    port: Optional[int] = None,
-    debugger: Optional[str] = None,
-):
-    if debugger is None:
-        return
-
-    if host is None:
-        host = os.environ.get("PYCXPRESS_DEBUGGER_HOST", "localhost")
-
-    if port is None:
-        port = os.environ.get("PYCXPRESS_DEBUGGER_PORT", 5678)
-
-    if debugger.lower() == "pycharm":
-        try:
-            import pydevd_pycharm
-
-            pydevd_pycharm.settrace(
-                host, port=port, stdoutToServer=True, stderrToServer=True, suspend=True
-            )
-        except ConnectionRefusedError:
-            logger.warning(
-                "Can not connect to Python debug server (maybe not started?)"
-            )
-            logger.warning(
-                "Use PYCXPRESS_DEBUGGER_TYPE=debugpy instead as Pycharm professional edition is needed for Python debug server feature."
-            )
-    elif debugger.lower() == "debugpy":
-        import debugpy
-
-        debugpy.listen((host, port))
-        logger.info(f"debugpy listen on {host}:{port}, please use VSCode to attach")
-        debugpy.wait_for_client()
-    else:
-        logger.warning(
-            f"Only PYCXPRESS_DEBUGGER_TYPE=debugpy|pycharm supported but {debugger} provided"
-        )
-
-
-def get_c_type(t: DTypeLike) -> Tuple[str, int]:
-    dtype = np.dtype(t)
-    relation = {
-        np.dtype("bool"): "bool",
-        np.dtype("int8"): "int8_t",
-        np.dtype("int16"): "int16_t",
-        np.dtype("int32"): "int32_t",
-        np.dtype("int64"): "int64_t",
-        np.dtype("uint8"): "uint8_t",
-        np.dtype("uint16"): "uint16_t",
-        np.dtype("uint32"): "uint32_t",
-        np.dtype("uint64"): "uint64_t",
-        np.dtype("float32"): "float",
-        np.dtype("float64"): "double",
-    }
-    return relation.get(dtype, "char"), dtype.itemsize or 1
+from .interface import (
+    InputTensorProtocol,
+    ModelProtocol,
+    OutputTensorProtocol,
+    TensorBufferProtocol,
+)
+from .utils import get_c_type, logger
 
 
 @dataclass
 class TensorMeta:
     dtype: DTypeLike  # the data type similar to np.int_
     shape: Union[
         int, Iterable[int], Callable[..., Union[int, Iterable[int]]]
@@ -158,19 +101,19 @@
             attrs["get_buffer_shape"] = get_buffer_shape
         attrs.setdefault("__slots__", []).append("__buffer_data__")
 
         return super().__new__(mcs, name, bases, attrs)
 
     @staticmethod
     def general_funcs(name: str, field_names: List[str]):
-        def get_buffer_shape(self, name: str):
-            buffer = getattr(self.__buffer_data__, name)
-            return buffer.shape
+        def get_buffer_shape(self, name: str) -> Tuple[int]:
+            shape: Tuple[int] = getattr(self.__buffer_data__, name).shape
+            return shape
 
-        def set_buffer_value(self, name: str, value):
+        def set_buffer_value(self, name: str, value: np.ndarray) -> None:
             buffer = getattr(self.__buffer_data__, name)
             buffer.data = value
 
         def init_func(self):
             _BufferData_ = namedtuple("_BufferData_", field_names)
             self.__buffer_data__ = _BufferData_(
                 *tuple(TensorWithShape() for _ in field_names)
@@ -205,17 +148,28 @@
 
         def del_func(_):
             raise AssertionError("Not supported for output tensor")
 
         return property(fget=get_func, fset=set_func, fdel=del_func, doc=field.doc)
 
 
-def convert_to_spec_tuple(fields: Iterable[TensorMeta]):
-    return tuple(
-        (v["name"], v["dtype"], v["buffer_size"]) for v in [v.to_dict() for v in fields]
+def convert_to_spec_tuple(
+    inputFields: Iterable[TensorMeta], outputFields: Iterable
+) -> Iterable[TensorBufferProtocol]:
+    return chain.from_iterable(
+        [
+            (
+                (v["name"], v["dtype"], v["buffer_size"], False)
+                for v in [v.to_dict() for v in inputFields]
+            ),
+            (
+                (v["name"], v["dtype"], v["buffer_size"], True)
+                for v in [v.to_dict() for v in outputFields]
+            ),
+        ]
     )
 
 
 def main():
     pass
```

### Comparing `pycxpress-0.0.4/src/PyCXpress/example/main.cpp` & `pycxpress-0.0.5/src/PyCXpress/example/main.cpp`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #define PYBIND11_DETAILED_ERROR_MESSAGES
 
 #include <PyCXpress/core.hpp>
 #include <PyCXpress/utils.hpp>
 
 namespace pcx = PyCXpress;
 
-void show_test(pcx::PythonInterpreter &python) {
+void show_test(pcx::Model &python) {
     std::vector<double> data(12);
     for (size_t i = 0; i < 12; i++) {
         data[i] = i;
     }
 
     std::vector<uint8_t> shape = {3, 4};
     memcpy(python.set_buffer("data_to_be_reshaped", {12}), data.data(),
@@ -37,16 +37,23 @@
     std::copy((double *)p, (double *)p + size,
               std::ostream_iterator<double>(std::cout, ", "));
     std::cout << std::endl;
 }
 
 int main(int argc, char *argv[]) {
     auto &python     = utils::Singleton<pcx::PythonInterpreter>::Instance();
+    auto &model0     = python.create_model("model.Model");
+    auto &model1     = python.create_model("model.Model", "odd");
     int   loop_times = 3;
 
+
     while (loop_times--) {
         std::cout << "looping " << loop_times << std::endl;
-        show_test(python);
+        if (loop_times % 2 == 0) {
+            show_test(model0);
+        } else {
+            show_test(model1);
+        }
     }
 
     return 0;
-}
+}
```

### Comparing `pycxpress-0.0.4/src/PyCXpress/example/model.py` & `pycxpress-0.0.5/src/PyCXpress/example/model.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# mypy: disable_error_code="type-arg,attr-defined"
+# mypy: disable_error_code="arg-type,type-arg,attr-defined"
 import os
 
 os.environ["TF_CPP_MIN_LOG_LEVEL"] = "3"
 import logging
 
 logging.basicConfig(level=logging.DEBUG)
 
@@ -65,46 +65,52 @@
     fields=OutputFields,
     type=ModelAnnotationType.Output,
     mode=ModelRuntimeType.EagerExecution,
 ):
     pass
 
 
-def init():
-    return (
-        InputDataSet(),
-        OutputDataSet(),
-        tuple(
-            (
-                *convert_to_spec_tuple(InputFields.values()),
-                *convert_to_spec_tuple(OutputFields.values()),
-            )
-        ),
-        tuple(OutputFields.keys()),
-    )
-
-
-def model(input: InputDataSet, output: OutputDataSet):
-    with nullcontext():
-        # print(input.data_to_be_reshaped)
-        # print(input.new_2d_shape)
-        output.output_a = input.data_to_be_reshaped.reshape(input.new_2d_shape)
-        # print(output.output_a)
+class Model:
+    def __init__(self):
+        self.input = None
+        self.output = None
+
+    def initialize(self):
+        self.input, self.output = InputDataSet(), OutputDataSet()
+
+        return (
+            self.input,
+            self.output,
+            tuple(convert_to_spec_tuple(InputFields.values(), OutputFields.values())),
+        )
+
+    def run(self):
+        self.model(self.input, self.output)
+
+    @staticmethod
+    def model(input: InputDataSet, output: OutputDataSet):
+        with nullcontext():
+            # print(input.data_to_be_reshaped)
+            # print(input.new_2d_shape)
+            output.output_a = input.data_to_be_reshaped.reshape(input.new_2d_shape)
+            # print(output.output_a)
 
 
 def main():
-    input_data, output_data, spec, _ = init()
+
+    model = Model()
+    input_data, output_data, spec = model.initialize()
     print(spec)
 
     input_data.set_buffer_value("data_to_be_reshaped", np.arange(12, dtype=np.float_))
     print(input_data.data_to_be_reshaped)
     input_data.set_buffer_value("new_2d_shape", np.array([3, 4]).astype(np.uint8))
     print(input_data.new_2d_shape)
     output_data.set_buffer_value("output_a", np.arange(12) * 0)
 
-    model(input_data, output_data)
+    model.run()
     print(output_data.output_a)
     print(output_data.get_buffer_shape("output_a"))
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `pycxpress-0.0.4/src/PyCXpress/include/PyCXpress/core.hpp` & `pycxpress-0.0.5/src/PyCXpress/include/PyCXpress/core.hpp`

 * *Files 24% similar despite different names*

```diff
@@ -24,21 +24,25 @@
 namespace py = pybind11;
 using namespace utils;
 
 class PYCXPRESS_EXPORT Buffer {
     typedef unsigned char Bytes;
 
     template <typename T>
-    static py::array __to_array(const std::vector<size_t> &shape, void *data) {
+    static py::array __to_array(const std::vector<size_t> &shape, void *data,
+                                size_t max_size) {
         std::vector<size_t> stride(shape.size());
         *stride.rbegin() = sizeof(T);
         auto ps          = shape.rbegin();
         for (auto pt = stride.rbegin() + 1; pt != stride.rend(); pt++, ps++) {
             *pt = *(pt - 1) * (*ps);
         }
+        if (max_size < stride.front() * shape.front()) {
+            throw std::runtime_error("Buffer size is too small");
+        }
         return py::array_t<T>{shape, std::move(stride), (T *)(data),
                               py::none()};
     }
 
 public:
     Buffer() : m_size(0), m_data(nullptr), m_converter(nullptr) {}
     Buffer(size_t size, const std::string &data_type) : m_size(size) {
@@ -95,133 +99,183 @@
 
     ~Buffer() {
         delete[] m_data;
         m_data = nullptr;
     }
 
     void *set(const std::vector<size_t> &shape) {
-        m_array = m_converter(shape, m_data);
+        m_array = m_converter(shape, m_data, m_size);
         return m_data;
     }
 
-    py::array &get() { return m_array; }
+    inline size_t itemsize() const { return m_size / m_length; }
+
+    py::array &array() { return m_array; }
 
-    void reset() { m_array = m_converter({m_length}, m_data); }
+    void reset() { m_array = m_converter({m_length}, m_data, m_size); }
 
 private:
     size_t    m_size;
     size_t    m_length;
     Bytes    *m_data;
     py::array m_array;
-    py::array (*m_converter)(const std::vector<size_t> &, void *);
+    py::array (*m_converter)(const std::vector<size_t> &, void *, size_t);
 };
 
-class PYCXPRESS_EXPORT PythonInterpreter {
+class PYCXPRESS_EXPORT Model {
 public:
-    explicit PythonInterpreter(bool init_signal_handlers = true, int argc = 0,
-                               const char *const *argv      = nullptr,
-                               bool add_program_dir_to_path = true) {
-        initialize(init_signal_handlers, argc, argv, add_program_dir_to_path);
-    }
-
-    PythonInterpreter(const PythonInterpreter &) = delete;
-    PythonInterpreter(PythonInterpreter &&other) noexcept {
-        other.is_valid = false;
+    explicit Model(const std::string &path) {
+        std::vector<char> module_name(path.data(), path.data() + path.length());
+        if (module_name.empty() || module_name.back() == '.') {
+            throw std::runtime_error("No model class provided");
+        }
+        auto iter = module_name.rbegin();
+        while (iter + 1 != module_name.rend() && '.' != *iter) {
+            ++iter;
+        }
+        if (iter + 1 == module_name.rend()) {
+            throw std::runtime_error("not module provided");
+        }
+        auto ith             = std::distance(iter, module_name.rend());
+        module_name[ith - 1] = 0;
+        module_name.push_back('\0');
+        initialize(module_name.data(), module_name.data() + ith);
+    }
+
+    Model(const Model &)            = delete;
+    Model(Model &&)                 = delete;
+    Model &operator=(const Model &) = delete;
+    Model &operator=(Model &&)      = delete;
+
+    ~Model() {
+        m_buffers.clear();
+        m_output_buffer_sizes.clear();
+        m_model  = py::none();
+        m_input  = py::none();
+        m_output = py::none();
     }
-    PythonInterpreter &operator=(const PythonInterpreter &) = delete;
-    PythonInterpreter &operator=(PythonInterpreter &&)      = delete;
 
-    ~PythonInterpreter() { finalize(); }
 
     void *set_buffer(const std::string         &name,
                      const std::vector<size_t> &shape) {
         auto &buf = m_buffers[name];
         void *p   = buf.set(shape);
-        m_py_input.attr("set_buffer_value")(name, buf.get());
+        m_input.attr("set_buffer_value")(name, buf.array());
         return p;
     }
 
     std::pair<void *, std::vector<size_t>> get_buffer(const std::string &name) {
-        auto &array  = m_buffers[name].get();
+        auto &array  = m_buffers[name].array();
         auto  pShape = m_output_buffer_sizes.find(name);
         if (pShape == m_output_buffer_sizes.end()) {
             return std::make_pair(
                 array.request().ptr,
                 std::vector<size_t>(array.shape(),
                                     array.shape() + array.ndim()));
         } else {
             return std::make_pair(array.request().ptr, pShape->second);
         }
     }
 
     void run() {
-        p_pkg->attr("model")(m_py_input, m_py_output);
+        m_model.attr("run")();
+
+        auto get_buffer_shape = m_output.attr("get_buffer_shape");
+
 
         for (auto &kv : m_output_buffer_sizes) {
             kv.second.clear();
-            py::tuple shape = m_py_output.attr("get_buffer_shape")(kv.first);
+            py::tuple shape = get_buffer_shape(kv.first);
 
             for (auto &d : shape) {
                 kv.second.push_back(d.cast<size_t>());
             }
         }
     }
 
-    void show_buffer(const std::string &name) {
-        auto &buf = m_buffers[name];
-        p_pkg->attr("show")(buf.get());
-    }
-
 private:
-    void initialize(bool init_signal_handlers, int argc,
-                    const char *const *argv, bool add_program_dir_to_path) {
-        py::initialize_interpreter(true, 0, nullptr, true);
-
-        p_pkg = std::make_unique<py::module_>(py::module_::import("model"));
-        py::print(p_pkg->attr("__file__"));
-
-        py::tuple spec, output_fields;
-        std::tie(m_py_input, m_py_output, spec, output_fields) =
-            p_pkg->attr("init")()
-                .cast<
-                    std::tuple<py::object, py::object, py::tuple, py::tuple>>();
+    void initialize(const char *module, const char *name) {
+        m_model = py::module_::import(module).attr(name)();
+
+        py::tuple spec;
+        std::tie(m_input, m_output, spec) =
+            m_model.attr("initialize")()
+                .cast<std::tuple<py::object, py::object, py::tuple>>();
 
+        auto set_buffer_value = m_output.attr("set_buffer_value");
         for (auto d = spec.begin(); d != spec.end(); d++) {
-            auto meta = d->cast<py::tuple>();
-            m_buffers.insert(std::make_pair(
-                meta[0].cast<std::string>(),
-                Buffer{meta[2].cast<size_t>(), meta[1].cast<std::string>()}));
+            auto       meta = d->cast<py::tuple>();
+            const auto name = meta[0].cast<std::string>();
+            auto       buf =
+                m_buffers.insert({name, Buffer{meta[2].cast<size_t>(),
+                                               meta[1].cast<std::string>()}});
+            if (meta[3].cast<bool>()) {
+                m_output_buffer_sizes[name] = {};
+                auto &buffer                = buf.first->second;
+                buffer.reset();
+                set_buffer_value(name, buffer.array());
+            }
         }
+    }
 
-        for (auto d = output_fields.begin(); d != output_fields.end(); d++) {
-            const auto name             = d->cast<std::string>();
-            m_output_buffer_sizes[name] = {};
-            auto &buf                   = m_buffers[name];
-            buf.reset();
-            m_py_output.attr("set_buffer_value")(name, buf.get());
-        }
+
+    std::map<std::string, Buffer>              m_buffers;
+    std::map<std::string, std::vector<size_t>> m_output_buffer_sizes;
+
+    py::object m_model;
+    py::object m_input;
+    py::object m_output;
+};
+
+class PYCXPRESS_EXPORT PythonInterpreter {
+public:
+    explicit PythonInterpreter() {}
+
+    PythonInterpreter(const PythonInterpreter &) = delete;
+    PythonInterpreter(PythonInterpreter &&other) noexcept {
+        other.is_valid = false;
     }
+    PythonInterpreter &operator=(const PythonInterpreter &) = delete;
+    PythonInterpreter &operator=(PythonInterpreter &&)      = delete;
+
+    ~PythonInterpreter() { finalize(); }
 
+    void initialize(bool init_signal_handlers = true, int argc = 0,
+                    const char *const *argv                    = nullptr,
+                    bool               add_program_dir_to_path = true) {
+        // TODO: maybe explicitly `dlopen("/path/to/libpython3.x.so", RTLD_NOW |
+        // RTLD_GLOBAL)` to avoid numpy import error
+        py::initialize_interpreter(init_signal_handlers, argc, argv,
+                                   add_program_dir_to_path);
+        is_valid = true;
+    }
     void finalize() {
-        p_pkg       = nullptr;
-        m_py_input  = py::none();
-        m_py_output = py::none();
+        m_models.clear();
 
         if (is_valid) {
             py::finalize_interpreter();
             is_valid = false;
         }
     }
 
-    bool                         is_valid = true;
-    std::unique_ptr<py::module_> p_pkg;
-
-    std::map<std::string, Buffer>              m_buffers;
-    std::map<std::string, std::vector<size_t>> m_output_buffer_sizes;
+    Model &create_model(const std::string &path,
+                        const std::string &name = "default") {
+        if (!is_valid) {
+            initialize();
+        }
+        if (m_models.find(name) == m_models.end()) {
+            m_models[name] = std::make_unique<Model>(path);
+        } else {
+            std::cerr << "Warning: Model with name " << name
+                      << " already exists" << std::endl;
+        }
+        return *m_models[name].get();
+    }
 
-    py::object m_py_input;
-    py::object m_py_output;
+private:
+    bool                                          is_valid = false;
+    std::map<std::string, std::unique_ptr<Model>> m_models;
 };
 
 };  // namespace PyCXpress
 
 #endif  // __PYCXPRESS_HPP__
```

### Comparing `pycxpress-0.0.4/src/PyCXpress/include/PyCXpress/utils.hpp` & `pycxpress-0.0.5/src/PyCXpress/include/PyCXpress/utils.hpp`

 * *Files identical despite different names*

### Comparing `pycxpress-0.0.4/PKG-INFO` & `pycxpress-0.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyCXpress
-Version: 0.0.4
+Version: 0.0.5
 Summary: PyCXpress is a high-performance hybrid framework that seamlessly integrates Python and C++ to harness the flexibility of Python and the speed of C++ for efficient and expressive computation, particularly in the realm of deep learning and numerical computing.
 Home-page: https://github.com/chaoqing/PyCXpress
 License: MIT
 Keywords: CPP,Embdedding
 Author: chaoqing
 Author-email: chaoqingwang.nick@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -15,15 +15,16 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: numpy (>=1.22,<2.0)
+Requires-Dist: numpy (<1.22) ; python_version >= "3.8" and python_version < "3.9"
+Requires-Dist: numpy (>=1.22,<2.0) ; python_version >= "3.9"
 Requires-Dist: pybind11 (>=2.12.0,<3.0.0)
 Project-URL: Repository, https://github.com/chaoqing/PyCXpress
 Description-Content-Type: text/markdown
 
 # PyCXpress
 
 <div align="center">
```

