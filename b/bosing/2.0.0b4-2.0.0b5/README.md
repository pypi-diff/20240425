# Comparing `tmp/bosing-2.0.0b4.tar.gz` & `tmp/bosing-2.0.0b5.tar.gz`

## Comparing `bosing-2.0.0b4.tar` & `bosing-2.0.0b5.tar`

### file list

```diff
@@ -1,43 +1,44 @@
--rw-r--r--   0        0        0      475 1970-01-01 00:00:00.000000 bosing-2.0.0b4/Cargo.toml
--rw-r--r--   0     1001      127      505 2024-04-22 17:07:23.000000 bosing-2.0.0b4/.github/dependabot.yml
--rw-r--r--   0     1001      127     6307 2024-04-22 17:07:23.000000 bosing-2.0.0b4/.github/workflows/ci.yml
--rw-r--r--   0     1001      127      696 2024-04-22 17:07:23.000000 bosing-2.0.0b4/.gitignore
--rw-r--r--   0     1001      127      972 2024-04-22 17:07:23.000000 bosing-2.0.0b4/.readthedocs.yaml
--rw-r--r--   0     1001      127     1068 2024-04-22 17:07:23.000000 bosing-2.0.0b4/LICENSE.txt
--rw-r--r--   0     1001      127     1348 2024-04-22 17:07:23.000000 bosing-2.0.0b4/README.md
--rw-r--r--   0     1001      127    10174 2024-04-22 17:07:23.000000 bosing-2.0.0b4/bosing.pyi
--rw-r--r--   0     1001      127      634 2024-04-22 17:07:23.000000 bosing-2.0.0b4/docs/Makefile
--rw-r--r--   0     1001      127      175 2024-04-22 17:07:23.000000 bosing-2.0.0b4/docs/_templates/autosummary/class.rst
--rw-r--r--   0     1001      127     1147 2024-04-22 17:07:23.000000 bosing-2.0.0b4/docs/_templates/autosummary/module.rst
--rw-r--r--   0     1001      127       82 2024-04-22 17:07:23.000000 bosing-2.0.0b4/docs/api.rst
--rw-r--r--   0     1001      127     1464 2024-04-22 17:07:23.000000 bosing-2.0.0b4/docs/conf.py
--rw-r--r--   0     1001      127     1258 2024-04-22 17:07:23.000000 bosing-2.0.0b4/docs/index.rst
--rw-r--r--   0     1001      127     1716 2024-04-22 17:07:23.000000 bosing-2.0.0b4/docs/instruction.rst
--rw-r--r--   0     1001      127      765 2024-04-22 17:07:23.000000 bosing-2.0.0b4/docs/make.bat
--rw-r--r--   0     1001      127      347 2024-04-22 17:07:23.000000 bosing-2.0.0b4/docs/quickstart.rst
--rw-r--r--   0     1001      127       16 2024-04-22 17:07:23.000000 bosing-2.0.0b4/docs/requirements.txt
--rw-r--r--   0     1001      127     5534 2024-04-22 17:07:23.000000 bosing-2.0.0b4/docs/schedule.rst
--rw-r--r--   0     1001      127     1138 2024-04-22 17:07:23.000000 bosing-2.0.0b4/example/flexible.py
--rw-r--r--   0     1001      127      521 2024-04-22 17:07:23.000000 bosing-2.0.0b4/example/hann.py
--rw-r--r--   0     1001      127      770 2024-04-22 17:07:23.000000 bosing-2.0.0b4/example/interp.py
--rw-r--r--   0     1001      127      682 2024-04-22 17:07:23.000000 bosing-2.0.0b4/example/overlap.py
--rw-r--r--   0     1001      127     2219 2024-04-22 17:07:23.000000 bosing-2.0.0b4/example/schedule.py
--rw-r--r--   0     1001      127     1879 2024-04-22 17:07:23.000000 bosing-2.0.0b4/example/schedule_stress.py
--rw-r--r--   0     1001      127     6064 2024-04-22 17:07:23.000000 bosing-2.0.0b4/ruff_defaults.toml
--rw-r--r--   0     1001      127    60814 2024-04-22 17:07:23.000000 bosing-2.0.0b4/src/lib.rs
--rw-r--r--   0     1001      127    10728 2024-04-22 17:07:23.000000 bosing-2.0.0b4/src/sampler.rs
--rw-r--r--   0     1001      127     2479 2024-04-22 17:07:23.000000 bosing-2.0.0b4/src/schedule/absolute.rs
--rw-r--r--   0     1001      127     7387 2024-04-22 17:07:23.000000 bosing-2.0.0b4/src/schedule/grid.rs
--rw-r--r--   0     1001      127     3311 2024-04-22 17:07:23.000000 bosing-2.0.0b4/src/schedule/play.rs
--rw-r--r--   0     1001      127     2349 2024-04-22 17:07:23.000000 bosing-2.0.0b4/src/schedule/repeat.rs
--rw-r--r--   0     1001      127     3944 2024-04-22 17:07:23.000000 bosing-2.0.0b4/src/schedule/simple.rs
--rw-r--r--   0     1001      127     5741 2024-04-22 17:07:23.000000 bosing-2.0.0b4/src/schedule/stack.rs
--rw-r--r--   0     1001      127    11082 2024-04-22 17:07:23.000000 bosing-2.0.0b4/src/schedule.rs
--rw-r--r--   0     1001      127     6649 2024-04-22 17:07:23.000000 bosing-2.0.0b4/src/shape.rs
--rw-r--r--   0     1001      127     1382 2024-04-22 17:07:23.000000 bosing-2.0.0b4/src/time.rs
--rw-r--r--   0     1001      127       14 2024-04-22 17:07:23.000000 bosing-2.0.0b4/stubtest-allowlist.txt
--rw-r--r--   0     1001      127        0 2024-04-22 17:07:23.000000 bosing-2.0.0b4/tests/__init__.py
--rw-r--r--   0     1001      127     1171 2024-04-22 17:07:23.000000 bosing-2.0.0b4/tests/test_basic.py
--rw-r--r--   0     1001      127    18030 2024-04-22 17:07:28.000000 bosing-2.0.0b4/Cargo.lock
--rw-r--r--   0     1001      127     1879 2024-04-22 17:07:23.000000 bosing-2.0.0b4/pyproject.toml
--rw-r--r--   0        0        0     2230 1970-01-01 00:00:00.000000 bosing-2.0.0b4/PKG-INFO
+-rw-r--r--   0        0        0      475 1970-01-01 00:00:00.000000 bosing-2.0.0b5/Cargo.toml
+-rw-r--r--   0     1001      127      505 2024-04-25 06:57:50.000000 bosing-2.0.0b5/.github/dependabot.yml
+-rw-r--r--   0     1001      127     6307 2024-04-25 06:57:50.000000 bosing-2.0.0b5/.github/workflows/ci.yml
+-rw-r--r--   0     1001      127      696 2024-04-25 06:57:50.000000 bosing-2.0.0b5/.gitignore
+-rw-r--r--   0     1001      127      972 2024-04-25 06:57:50.000000 bosing-2.0.0b5/.readthedocs.yaml
+-rw-r--r--   0     1001      127     1068 2024-04-25 06:57:50.000000 bosing-2.0.0b5/LICENSE.txt
+-rw-r--r--   0     1001      127     1348 2024-04-25 06:57:50.000000 bosing-2.0.0b5/README.md
+-rw-r--r--   0     1001      127    10244 2024-04-25 06:57:50.000000 bosing-2.0.0b5/bosing.pyi
+-rw-r--r--   0     1001      127      634 2024-04-25 06:57:50.000000 bosing-2.0.0b5/docs/Makefile
+-rw-r--r--   0     1001      127      175 2024-04-25 06:57:50.000000 bosing-2.0.0b5/docs/_templates/autosummary/class.rst
+-rw-r--r--   0     1001      127     1147 2024-04-25 06:57:50.000000 bosing-2.0.0b5/docs/_templates/autosummary/module.rst
+-rw-r--r--   0     1001      127       82 2024-04-25 06:57:50.000000 bosing-2.0.0b5/docs/api.rst
+-rw-r--r--   0     1001      127     1464 2024-04-25 06:57:50.000000 bosing-2.0.0b5/docs/conf.py
+-rw-r--r--   0     1001      127     1258 2024-04-25 06:57:50.000000 bosing-2.0.0b5/docs/index.rst
+-rw-r--r--   0     1001      127     1716 2024-04-25 06:57:50.000000 bosing-2.0.0b5/docs/instruction.rst
+-rw-r--r--   0     1001      127      765 2024-04-25 06:57:50.000000 bosing-2.0.0b5/docs/make.bat
+-rw-r--r--   0     1001      127      347 2024-04-25 06:57:50.000000 bosing-2.0.0b5/docs/quickstart.rst
+-rw-r--r--   0     1001      127       16 2024-04-25 06:57:50.000000 bosing-2.0.0b5/docs/requirements.txt
+-rw-r--r--   0     1001      127     5534 2024-04-25 06:57:50.000000 bosing-2.0.0b5/docs/schedule.rst
+-rw-r--r--   0     1001      127     1138 2024-04-25 06:57:50.000000 bosing-2.0.0b5/example/flexible.py
+-rw-r--r--   0     1001      127      521 2024-04-25 06:57:50.000000 bosing-2.0.0b5/example/hann.py
+-rw-r--r--   0     1001      127      770 2024-04-25 06:57:50.000000 bosing-2.0.0b5/example/interp.py
+-rw-r--r--   0     1001      127      682 2024-04-25 06:57:50.000000 bosing-2.0.0b5/example/overlap.py
+-rw-r--r--   0     1001      127     2219 2024-04-25 06:57:50.000000 bosing-2.0.0b5/example/schedule.py
+-rw-r--r--   0     1001      127     2028 2024-04-25 06:57:50.000000 bosing-2.0.0b5/example/schedule_stress.py
+-rw-r--r--   0     1001      127     6064 2024-04-25 06:57:50.000000 bosing-2.0.0b5/ruff_defaults.toml
+-rw-r--r--   0     1001      127     7351 2024-04-25 06:57:50.000000 bosing-2.0.0b5/src/executor.rs
+-rw-r--r--   0     1001      127    62068 2024-04-25 06:57:50.000000 bosing-2.0.0b5/src/lib.rs
+-rw-r--r--   0     1001      127    11167 2024-04-25 06:57:50.000000 bosing-2.0.0b5/src/pulse.rs
+-rw-r--r--   0     1001      127     1667 2024-04-25 06:57:50.000000 bosing-2.0.0b5/src/quant.rs
+-rw-r--r--   0     1001      127     2479 2024-04-25 06:57:50.000000 bosing-2.0.0b5/src/schedule/absolute.rs
+-rw-r--r--   0     1001      127     7387 2024-04-25 06:57:50.000000 bosing-2.0.0b5/src/schedule/grid.rs
+-rw-r--r--   0     1001      127     3311 2024-04-25 06:57:50.000000 bosing-2.0.0b5/src/schedule/play.rs
+-rw-r--r--   0     1001      127     2349 2024-04-25 06:57:50.000000 bosing-2.0.0b5/src/schedule/repeat.rs
+-rw-r--r--   0     1001      127     3944 2024-04-25 06:57:50.000000 bosing-2.0.0b5/src/schedule/simple.rs
+-rw-r--r--   0     1001      127     5741 2024-04-25 06:57:50.000000 bosing-2.0.0b5/src/schedule/stack.rs
+-rw-r--r--   0     1001      127    11082 2024-04-25 06:57:50.000000 bosing-2.0.0b5/src/schedule.rs
+-rw-r--r--   0     1001      127     6649 2024-04-25 06:57:50.000000 bosing-2.0.0b5/src/shape.rs
+-rw-r--r--   0     1001      127       14 2024-04-25 06:57:50.000000 bosing-2.0.0b5/stubtest-allowlist.txt
+-rw-r--r--   0     1001      127        0 2024-04-25 06:57:50.000000 bosing-2.0.0b5/tests/__init__.py
+-rw-r--r--   0     1001      127     1171 2024-04-25 06:57:50.000000 bosing-2.0.0b5/tests/test_basic.py
+-rw-r--r--   0     1001      127    18030 2024-04-25 06:58:08.000000 bosing-2.0.0b5/Cargo.lock
+-rw-r--r--   0     1001      127     1867 2024-04-25 06:57:50.000000 bosing-2.0.0b5/pyproject.toml
+-rw-r--r--   0        0        0     2218 1970-01-01 00:00:00.000000 bosing-2.0.0b5/PKG-INFO
```

### Comparing `bosing-2.0.0b4/.github/workflows/ci.yml` & `bosing-2.0.0b5/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b4/.gitignore` & `bosing-2.0.0b5/.gitignore`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b4/.readthedocs.yaml` & `bosing-2.0.0b5/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b4/LICENSE.txt` & `bosing-2.0.0b5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b4/README.md` & `bosing-2.0.0b5/README.md`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b4/bosing.pyi` & `bosing-2.0.0b5/bosing.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from collections.abc import Iterable, Sequence
 from typing import ClassVar, Literal, Self, TypeAlias, final
 
 import numpy as np
+import numpy.typing as npt
 
 @final
 class Channel:
     def __new__(
         cls,
         name: str,
         base_freq: float,
@@ -356,8 +357,9 @@
     shapes: Iterable[Shape],
     schedule: Element,
     *,
     time_tolerance: float = ...,
     amp_tolerance: float = ...,
     phase_tolerance: float = ...,
     allow_oversize: bool = ...,
+    crosstalk: npt.ArrayLike | None = ...,
 ) -> dict[str, np.ndarray]: ...
```

### Comparing `bosing-2.0.0b4/docs/Makefile` & `bosing-2.0.0b5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b4/docs/_templates/autosummary/module.rst` & `bosing-2.0.0b5/docs/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b4/docs/conf.py` & `bosing-2.0.0b5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b4/docs/index.rst` & `bosing-2.0.0b5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b4/docs/instruction.rst` & `bosing-2.0.0b5/docs/instruction.rst`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b4/docs/make.bat` & `bosing-2.0.0b5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b4/docs/schedule.rst` & `bosing-2.0.0b5/docs/schedule.rst`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b4/example/flexible.py` & `bosing-2.0.0b5/example/flexible.py`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b4/example/hann.py` & `bosing-2.0.0b5/example/hann.py`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b4/example/interp.py` & `bosing-2.0.0b5/example/interp.py`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b4/example/overlap.py` & `bosing-2.0.0b5/example/overlap.py`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b4/example/schedule.py` & `bosing-2.0.0b5/example/schedule.py`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b4/example/schedule_stress.py` & `bosing-2.0.0b5/example/schedule_stress.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,21 +46,24 @@
             )
             for _ in range(n)
         ),
         measure,
         Barrier(duration=15e-9),
     )
 
-    _ = generate_waveforms(channels, shapes, schedule)
+    crosstalk = np.eye(len(channels), dtype=np.float64)
+    crosstalk[c["u0"] : c["u0"] + nu, c["u0"] : c["u0"] + nu] += 0.1
+
+    _ = generate_waveforms(channels, shapes, schedule, crosstalk=crosstalk)
 
     t1 = time.perf_counter()
     print(f"Time: {t1-t0:.3f}s")
 
 
 def main():
-    for i in cycle(range(1, 100)):
+    for i in cycle(range(349, 350)):
         print(i)
         gen_n(i)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `bosing-2.0.0b4/ruff_defaults.toml` & `bosing-2.0.0b5/ruff_defaults.toml`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b4/src/lib.rs` & `bosing-2.0.0b5/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 //! Although Element struct may contains [`Py<Element>`] as children, it is not
 //! possible to create cyclic references because we don't allow mutate the
 //! children after creation.
 
 use mimalloc::MiMalloc;
-use numpy::{Complex64, PyArray1};
-use pyo3::{
-    exceptions::{PyRuntimeError, PyTypeError, PyValueError},
-    prelude::*,
-};
-use schedule::ElementCommonBuilder;
+use numpy::prelude::*;
+use numpy::{AllowTypeChange, Complex64, PyArray1, PyArrayLike2};
+use pyo3::exceptions::{PyRuntimeError, PyTypeError, PyValueError};
+use pyo3::prelude::*;
 use std::{collections::HashMap, sync::Arc};
 
-use crate::sampler::Sampler;
+use crate::executor::Executor;
+use crate::pulse::Sampler;
+use crate::quant::{Frequency, Time};
+use schedule::ElementCommonBuilder;
 
-mod sampler;
+mod executor;
+mod pulse;
+mod quant;
 mod schedule;
 mod shape;
-mod time;
 
 #[global_allocator]
 static GLOBAL: MiMalloc = MiMalloc;
 
 /// Channel configuration.
 ///
 /// `align_level` is the time axis alignment granularity. With sampling interval
@@ -1952,14 +1954,15 @@
 ///     schedule (Element): Root element of the schedule.
 ///     time_tolerance (float): Tolerance for time comparison. Default is 1e-12.
 ///     amp_tolerance (float): Tolerance for amplitude comparison. Default is
 ///         0.1 / 2^16.
 ///     phase_tolerance (float): Tolerance for phase comparison. Default is
 ///         1e-4.
 ///     allow_oversize (bool): Allow oversize elements. Default is ``False``.
+///     crosstalk (array_like | None): Crosstalk matrix. Default is ``None``.
 /// Returns:
 ///     Dict[str, numpy.ndarray]: Waveforms of the channels. The key is the
 ///         channel name and the value is the waveform.
 /// Raises:
 ///     ValueError: If some input is invalid.
 ///     TypeError: If some input has an invalid type.
 ///     RuntimeError: If waveform generation fails.
@@ -1986,49 +1989,79 @@
     shapes,
     schedule,
     *,
     time_tolerance=1e-12,
     amp_tolerance=0.1 / 2f64.powi(16),
     phase_tolerance=1e-4,
     allow_oversize=false,
+    crosstalk=None,
 ))]
 #[allow(clippy::too_many_arguments)]
 fn generate_waveforms(
     py: Python<'_>,
     channels: Vec<Channel>,
     shapes: Vec<Py<Shape>>,
     schedule: &Bound<'_, Element>,
     time_tolerance: f64,
     amp_tolerance: f64,
     phase_tolerance: f64,
     allow_oversize: bool,
+    crosstalk: Option<PyArrayLike2<'_, f64, AllowTypeChange>>,
 ) -> PyResult<HashMap<String, Py<PyArray1<Complex64>>>> {
     // TODO: use the tolerances
-    let _ = (amp_tolerance, phase_tolerance);
+    let _ = phase_tolerance;
+    if let Some(crosstalk) = &crosstalk {
+        if crosstalk.ndim() != 2 {
+            return Err(PyValueError::new_err("Crosstalk must be a 2D array."));
+        }
+        if crosstalk.shape()[0] != crosstalk.shape()[1] {
+            return Err(PyValueError::new_err("Crosstalk must be a square matrix."));
+        }
+        if crosstalk.shape()[0] != channels.len() {
+            return Err(PyValueError::new_err(
+                "The size of the crosstalk matrix must be the same as the number of channels.",
+            ));
+        }
+    }
+
     let root = schedule.downcast::<Element>()?.get().0.clone();
     let measured = schedule::measure(root, f64::INFINITY);
     let arrange_options = schedule::ScheduleOptions {
         time_tolerance,
         allow_oversize,
     };
     let arranged = schedule::arrange(&measured, 0.0, measured.duration(), &arrange_options)
         .map_err(|e| PyRuntimeError::new_err(e.to_string()))?;
-    let mut sampler = Sampler::new();
+    let mut executor = Executor::new(amp_tolerance, time_tolerance);
     for c in channels.iter() {
-        sampler.add_channel(c.base_freq, c.sample_rate, c.length, c.delay, c.align_level);
+        executor.add_channel(c.base_freq);
     }
     for s in shapes.iter() {
         let s = s.bind(py);
-        sampler.add_shape(Shape::get_rust_shape(s)?);
+        executor.add_shape(Shape::get_rust_shape(s)?);
+    }
+    executor.execute(&arranged);
+    let results = executor.into_result();
+    let mut sampler = Sampler::new();
+    for (c, pl) in channels.iter().zip(results) {
+        sampler.add_channel(
+            pl,
+            c.length,
+            Frequency::new(c.sample_rate).unwrap(),
+            Time::new(c.delay).unwrap(),
+            c.align_level,
+        );
+    }
+    if let Some(crosstalk) = &crosstalk {
+        sampler.set_crosstalk(crosstalk.as_array());
     }
-    sampler.execute(&arranged);
-    let results = sampler.into_result();
+    let waveforms = sampler.sample(time_tolerance);
     let dict = channels
         .into_iter()
-        .zip(results)
+        .zip(waveforms)
         .map(|(c, w)| (c.name, PyArray1::from_vec_bound(py, w).unbind()))
         .collect();
     Ok(dict)
 }
 
 /// Generates microwave pulses for superconducting quantum computing
 /// experiments.
```

### Comparing `bosing-2.0.0b4/src/sampler.rs` & `bosing-2.0.0b5/src/pulse.rs`

 * *Files 26% similar despite different names*

```diff
@@ -1,278 +1,283 @@
-use std::{f64::consts::TAU, sync::Arc};
+use std::{
+    collections::HashMap,
+    f64::consts::TAU,
+    ops::{Add, Mul},
+    sync::Arc,
+};
 
 use cached::proc_macro::cached;
-use itertools::izip;
+use float_cmp::approx_eq;
+use itertools::{izip, Itertools};
+use ndarray::ArrayView2;
 use numpy::Complex64;
-use ordered_float::NotNan;
 
 use crate::{
-    schedule::{self, ArrangedElement, ElementVariant},
+    quant::{AlignedIndex, Frequency, Time},
     shape::Shape,
-    time::{AlignedIndex, Time},
 };
 
+/// A pulse envelope
+///
+/// If `shape` is `None`, constructor will set `plateau` to `width + plateau`
+/// and `width` to `0`.
+#[derive(Debug, Clone, PartialEq, Eq, Hash)]
+pub struct Envelope {
+    shape: Option<Shape>,
+    width: Time,
+    plateau: Time,
+}
+
+impl Envelope {
+    pub fn new(mut shape: Option<Shape>, mut width: Time, mut plateau: Time) -> Self {
+        if shape.is_none() {
+            plateau += width;
+            width = Time::new(0.0).unwrap();
+        }
+        if width.value() == 0.0 {
+            shape = None
+        }
+        Self {
+            shape,
+            width,
+            plateau,
+        }
+    }
+}
+
+#[derive(Debug, Clone, PartialEq, Eq, Hash)]
+struct ListBin {
+    envelope: Envelope,
+    global_freq: Frequency,
+    local_freq: Frequency,
+}
+
+#[derive(Debug, Clone, Copy)]
+struct PulseAmplitude {
+    // Amplitude of the pulse
+    amp: Complex64,
+    // Drag amplitude of the pulse (but not multiplied by sample rate yet)
+    drag: Complex64,
+}
+
+impl Add for PulseAmplitude {
+    type Output = Self;
+
+    fn add(self, other: Self) -> Self {
+        Self {
+            amp: self.amp + other.amp,
+            drag: self.drag + other.drag,
+        }
+    }
+}
+
+impl Mul<f64> for PulseAmplitude {
+    type Output = Self;
+
+    fn mul(self, rhs: f64) -> Self {
+        Self {
+            amp: self.amp * rhs,
+            drag: self.drag * rhs,
+        }
+    }
+}
+
+#[derive(Debug, Clone)]
+pub struct PulseList {
+    items: HashMap<ListBin, Vec<(Time, PulseAmplitude)>>,
+}
+
 #[derive(Debug, Clone, Default)]
-pub struct Sampler {
+pub struct Sampler<'a> {
     channels: Vec<Channel>,
-    shapes: Vec<Shape>,
+    crosstalk: Option<ArrayView2<'a, f64>>,
 }
 
-impl Sampler {
+impl<'a> Sampler<'a> {
     pub fn new() -> Self {
         Self::default()
     }
 
     pub fn add_channel(
         &mut self,
-        base_freq: f64,
-        sample_rate: f64,
+        pulses: PulseList,
         length: usize,
-        delay: f64,
+        sample_rate: Frequency,
+        delay: Time,
         align_level: i32,
     ) {
-        self.channels.push(Channel::new(
-            base_freq,
-            sample_rate,
+        self.channels.push(Channel {
+            pulses,
             length,
-            delay,
+            sample_rate,
             align_level,
-        ));
-    }
-
-    pub fn add_shape(&mut self, shape: Shape) {
-        self.shapes.push(shape);
-    }
-
-    pub fn execute(&mut self, element: &ArrangedElement) {
-        self.execute_dispatch(element, 0.0);
-    }
-
-    pub fn into_result(self) -> Vec<Vec<Complex64>> {
-        self.channels.into_iter().map(|c| c.waveform).collect()
+            delay,
+        });
     }
 
-    fn execute_dispatch(&mut self, element: &ArrangedElement, time: f64) {
-        if element.element().common().phantom() {
-            return;
-        }
-        let time = time + element.inner_time();
-        let duration = element.inner_duration();
-        match element.element().variant() {
-            ElementVariant::Play(e) => self.execute_play(e, time, duration),
-            ElementVariant::ShiftPhase(e) => self.execute_shift_phase(e),
-            ElementVariant::SetPhase(e) => self.execute_set_phase(e, time),
-            ElementVariant::ShiftFreq(e) => self.execute_shift_freq(e, time),
-            ElementVariant::SetFreq(e) => self.execute_set_freq(e, time),
-            ElementVariant::SwapPhase(e) => self.execute_swap_phase(e, time),
-            ElementVariant::Barrier(_) => (),
-            ElementVariant::Repeat(e) => {
-                let child = &element.try_get_children().expect("Invalid arrange data")[0];
-                self.execute_repeat(e, child, time, duration);
-            }
-            ElementVariant::Stack(_) | ElementVariant::Absolute(_) | ElementVariant::Grid(_) => {
-                let children = element.try_get_children().expect("Invalid arrange data");
-                self.execute_container(children, time);
-            }
-        }
+    pub fn set_crosstalk(&mut self, crosstalk: ArrayView2<'a, f64>) {
+        self.crosstalk = Some(crosstalk);
     }
 
-    fn execute_play(&mut self, element: &schedule::Play, time: f64, duration: f64) {
-        let shape = element.shape_id().map(|id| self.shapes[id].clone());
-        let width = element.width();
-        let plateau = if element.flexible() {
-            duration - width
+    pub fn sample(&self, time_tolerance: f64) -> Vec<Vec<Complex64>> {
+        if let Some(crosstalk) = self.crosstalk {
+            crosstalk
+                .columns()
+                .into_iter()
+                .zip(&self.channels)
+                .map(|(column, output)| {
+                    let lists = column
+                        .iter()
+                        .copied()
+                        .zip(&self.channels)
+                        .map(|(multiplier, input)| (multiplier, &input.pulses));
+                    merge_and_sample(
+                        lists,
+                        output.length,
+                        output.sample_rate,
+                        output.delay,
+                        output.align_level,
+                        time_tolerance,
+                    )
+                })
+                .collect()
         } else {
-            element.plateau()
-        };
-        let amplitude = element.amplitude();
-        let drag_coef = element.drag_coef();
-        let freq = element.frequency();
-        let phase = element.phase();
-        let channel = &mut self.channels[element.channel_id()];
-        let time = Time::new(time).unwrap();
-        let width = Time::new(width).unwrap();
-        let plateau = Time::new(plateau).unwrap();
-        channel.sample(
-            shape, time, width, plateau, amplitude, drag_coef, freq, phase,
-        );
-    }
-
-    fn execute_shift_phase(&mut self, element: &schedule::ShiftPhase) {
-        let delta_phase = element.phase();
-        let channel = &mut self.channels[element.channel_id()];
-        channel.shift_phase(delta_phase);
-    }
-
-    fn execute_set_phase(&mut self, element: &schedule::SetPhase, time: f64) {
-        let phase = element.phase();
-        let channel = &mut self.channels[element.channel_id()];
-        channel.set_phase(phase, time);
-    }
-
-    fn execute_shift_freq(&mut self, element: &schedule::ShiftFreq, time: f64) {
-        let delta_freq = element.frequency();
-        let channel = &mut self.channels[element.channel_id()];
-        channel.shift_freq(delta_freq, time);
-    }
-
-    fn execute_set_freq(&mut self, element: &schedule::SetFreq, time: f64) {
-        let freq = element.frequency();
-        let channel = &mut self.channels[element.channel_id()];
-        channel.set_freq(freq, time);
-    }
-
-    fn execute_swap_phase(&mut self, element: &schedule::SwapPhase, time: f64) {
-        let ch1 = element.channel_id1();
-        let ch2 = element.channel_id2();
-        // Workaround for unstable get_many_mut
-        if ch1 == ch2 {
-            return;
-        }
-        let (ch1, ch2) = if ch1 < ch2 { (ch1, ch2) } else { (ch2, ch1) };
-        let (a, b) = self.channels.split_at_mut(ch2);
-        let channel = &mut a[ch1];
-        let other = &mut b[0];
-        channel.swap_phase(other, time);
-    }
-
-    fn execute_repeat(
-        &mut self,
-        element: &schedule::Repeat,
-        child: &ArrangedElement,
-        time: f64,
-        duration: f64,
-    ) {
-        let count = element.count();
-        if count == 0 {
-            return;
-        }
-        let spacing = element.spacing();
-        let time_step = (duration + spacing) / count as f64;
-        for i in 0..count {
-            let child_time = time + i as f64 * time_step;
-            self.execute_dispatch(child, child_time);
-        }
-    }
-
-    fn execute_container(&mut self, children: &[ArrangedElement], time: f64) {
-        for child in children {
-            self.execute_dispatch(child, time);
+            self.channels
+                .iter()
+                .map(|c| {
+                    let list = c
+                        .pulses
+                        .items
+                        .iter()
+                        .map(|(bin, items)| (bin.clone(), items.iter().copied()));
+                    sample_pulse_list(list, c.length, c.sample_rate, c.delay, c.align_level)
+                })
+                .collect()
         }
     }
 }
 
 #[derive(Debug, Clone)]
 struct Channel {
-    base_freq: f64,
-    delta_freq: f64,
-    phase: f64,
-    sample_rate: f64,
-    waveform: Vec<Complex64>,
-    delay: Time,
+    pulses: PulseList,
+    length: usize,
+    sample_rate: Frequency,
     align_level: i32,
+    delay: Time,
 }
 
-impl Channel {
-    fn new(base_freq: f64, sample_rate: f64, length: usize, delay: f64, align_level: i32) -> Self {
+#[derive(Debug, Clone)]
+pub struct PulseListBuilder {
+    items: HashMap<ListBin, Vec<(Time, PulseAmplitude)>>,
+    amp_tolerance: f64,
+    time_tolerance: f64,
+}
+
+impl PulseListBuilder {
+    pub fn new(amp_tolerance: f64, time_tolerance: f64) -> Self {
         Self {
-            base_freq,
-            delta_freq: 0.0,
-            phase: 0.0,
-            sample_rate,
-            waveform: vec![Complex64::default(); length],
-            delay: Time::new(delay).unwrap(),
-            align_level,
+            items: HashMap::new(),
+            amp_tolerance,
+            time_tolerance,
         }
     }
 
-    fn shift_freq(&mut self, delta_freq: f64, time: f64) {
-        let delta_phase = -delta_freq * time;
-        self.delta_freq += delta_freq;
-        self.phase += delta_phase;
-    }
-
-    fn set_freq(&mut self, freq: f64, time: f64) {
-        let delta_freq = freq - self.delta_freq;
-        let delta_phase = -delta_freq * time;
-        self.delta_freq = freq;
-        self.phase += delta_phase;
-    }
-
-    fn shift_phase(&mut self, delta_phase: f64) {
-        self.phase += delta_phase;
-    }
-
-    fn set_phase(&mut self, phase: f64, time: f64) {
-        self.phase = phase - self.delta_freq * time;
-    }
-
-    fn total_freq(&self) -> f64 {
-        self.base_freq + self.delta_freq
-    }
-
-    fn swap_phase(&mut self, other: &mut Self, time: f64) {
-        let delta_freq = self.total_freq() - other.total_freq();
-        let phase1 = self.phase;
-        let phase2 = other.phase;
-        self.phase = phase2 - delta_freq * time;
-        other.phase = phase1 + delta_freq * time;
-    }
-
-    fn sample(
+    pub fn push(
         &mut self,
-        shape: Option<Shape>,
+        envelope: Envelope,
+        global_freq: Frequency,
+        local_freq: Frequency,
         time: Time,
-        width: Time,
-        plateau: Time,
         amplitude: f64,
         drag_coef: f64,
-        freq: f64,
         phase: f64,
     ) {
-        let t_start = time + self.delay;
-        let i_frac_start = AlignedIndex::new(t_start, self.sample_rate, self.align_level).unwrap();
-        let i_start = i_frac_start.ceil();
-        let index_offset = i_frac_start.index_offset();
-        let global_freq = self.total_freq();
-        let local_freq = freq;
-        let total_freq = global_freq + local_freq;
-        let dt = 1.0 / self.sample_rate;
-        let phase0 = phase
-            + self.phase
-            + global_freq * (i_start.value() * dt - self.delay.value())
-            + local_freq * index_offset.value() * dt;
-        let dphase = total_freq * dt;
-        let phase0 = phase0 * TAU;
-        let dphase = dphase * TAU;
-        let waveform = &mut self.waveform[i_start.value() as usize..];
-        if let Some(shape) = shape {
-            let sample_rate = NotNan::new(self.sample_rate).unwrap();
-            let envelope = get_envelope(shape, width, plateau, index_offset, sample_rate);
-            let drag_coef = drag_coef * self.sample_rate;
-            mix_add_envelope(waveform, &envelope, amplitude, drag_coef, phase0, dphase);
-        } else {
-            let i_plateau = ((width + plateau).value() * self.sample_rate).ceil() as usize;
-            mix_add_plateau(&mut waveform[..i_plateau], amplitude, phase0, dphase);
+        if approx_eq!(f64, amplitude, 0.0, epsilon = self.amp_tolerance) {
+            return;
         }
+        let bin = ListBin {
+            envelope,
+            global_freq,
+            local_freq,
+        };
+        let amp = Complex64::from_polar(amplitude, TAU * phase);
+        let drag = amp * Complex64::i() * drag_coef;
+        let amplitude = PulseAmplitude { amp, drag };
+        self.items.entry(bin).or_default().push((time, amplitude));
+    }
+
+    pub fn build(mut self) -> PulseList {
+        for pulses in self.items.values_mut() {
+            pulses.sort_unstable_by_key(|(time, _)| *time);
+            let mut i = 0;
+            for j in 1..pulses.len() {
+                if approx_eq!(
+                    f64,
+                    pulses[i].0.value(),
+                    pulses[j].0.value(),
+                    epsilon = self.time_tolerance
+                ) {
+                    pulses[i].1 = pulses[i].1 + pulses[j].1;
+                } else {
+                    i += 1;
+                    pulses[i] = pulses[j];
+                }
+            }
+            pulses.truncate(i + 1);
+        }
+        PulseList { items: self.items }
+    }
+}
+
+fn mix_add_envelope(
+    waveform: &mut [Complex64],
+    envelope: &[f64],
+    amplitude: Complex64,
+    drag_amp: Complex64,
+    phase0: f64,
+    dphase: f64,
+) {
+    let mut carrier = Complex64::from_polar(1.0, phase0);
+    let dcarrier = Complex64::from_polar(1.0, dphase);
+    let slope_iter = (0..envelope.len()).map(|i| {
+        let left = if i > 0 { envelope[i - 1] } else { 0.0 };
+        let right = if i < envelope.len() - 1 {
+            envelope[i + 1]
+        } else {
+            0.0
+        };
+        (right - left) / 2.0
+    });
+    for (y, env, slope) in izip!(waveform.iter_mut(), envelope.iter().copied(), slope_iter) {
+        *y += carrier * (amplitude * env + drag_amp * slope);
+        carrier *= dcarrier;
+    }
+}
+
+fn mix_add_plateau(waveform: &mut [Complex64], amplitude: Complex64, phase: f64, dphase: f64) {
+    let mut carrier = Complex64::from_polar(1.0, phase) * amplitude;
+    let dcarrier = Complex64::from_polar(1.0, dphase);
+    for y in waveform.iter_mut() {
+        *y += carrier;
+        carrier *= dcarrier;
     }
 }
 
 #[cached(size = 1024)]
 fn get_envelope(
     shape: Shape,
     width: Time,
     plateau: Time,
     index_offset: AlignedIndex,
-    sample_rate: NotNan<f64>,
+    sample_rate: Frequency,
 ) -> Arc<Vec<f64>> {
     let width = width.value();
     let plateau = plateau.value();
     let index_offset = index_offset.value();
-    let sample_rate = sample_rate.into_inner();
+    let sample_rate = sample_rate.value();
     let dt = 1.0 / sample_rate;
     let t_offset = index_offset * dt;
     let t1 = width / 2.0 - t_offset;
     let t2 = width / 2.0 + plateau - t_offset;
     let t3 = width + plateau - t_offset;
     let length = (t3 * sample_rate).ceil() as usize;
     let plateau_start_index = (t1 * sample_rate).ceil() as usize;
@@ -287,41 +292,98 @@
         envelope[plateau_start_index..plateau_end_index].fill(1.0);
         let x2 = (plateau_end_index as f64 * dt - t2) / width;
         shape.sample_array(x2, dx, &mut envelope[plateau_end_index..]);
     }
     Arc::new(envelope)
 }
 
-fn mix_add_envelope(
-    waveform: &mut [Complex64],
-    envelope: &[f64],
-    amplitude: f64,
-    drag_coef: f64,
-    phase: f64,
-    dphase: f64,
-) {
-    let mut carrier = Complex64::from_polar(amplitude, phase);
-    let dcarrier = Complex64::from_polar(1.0, dphase);
-    let slope_iter = (0..envelope.len()).map(|i| {
-        let left = if i > 0 { envelope[i - 1] } else { 0.0 };
-        let right = if i < envelope.len() - 1 {
-            envelope[i + 1]
-        } else {
-            0.0
-        };
-        (right - left) / 2.0
-    });
-    let drag_coef = Complex64::new(0.0, drag_coef);
-    for (y, env, slope) in izip!(waveform.iter_mut(), envelope.iter().copied(), slope_iter) {
-        *y += carrier * (env + drag_coef * slope);
-        carrier *= dcarrier;
+fn merge_and_sample<'a>(
+    lists: impl IntoIterator<Item = (f64, &'a PulseList)>,
+    length: usize,
+    sample_rate: Frequency,
+    delay: Time,
+    align_level: i32,
+    time_tolerance: f64,
+) -> Vec<Complex64> {
+    let mut merged: HashMap<ListBin, Vec<_>> = HashMap::new();
+    for (multiplier, list) in lists {
+        if multiplier == 0.0 {
+            continue;
+        }
+        for (bin, items) in &list.items {
+            merged.entry(bin.clone()).or_default().push(
+                items
+                    .iter()
+                    .map(move |&(time, amp)| (time, amp * multiplier)),
+            )
+        }
     }
+    let merged = merged.into_iter().map(|(bin, items)| {
+        (
+            bin,
+            items
+                .into_iter()
+                .kmerge_by(|a, b| a.0 < b.0)
+                .coalesce(|a, b| {
+                    if approx_eq!(f64, a.0.value(), b.0.value(), epsilon = time_tolerance) {
+                        Ok((a.0, a.1 + b.1))
+                    } else {
+                        Err((a, b))
+                    }
+                }),
+        )
+    });
+    sample_pulse_list(merged, length, sample_rate, delay, align_level)
 }
 
-fn mix_add_plateau(waveform: &mut [Complex64], amplitude: f64, phase: f64, dphase: f64) {
-    let mut carrier = Complex64::from_polar(amplitude, phase);
-    let dcarrier = Complex64::from_polar(1.0, dphase);
-    for y in waveform.iter_mut() {
-        *y += carrier;
-        carrier *= dcarrier;
+fn sample_pulse_list<PL, L>(
+    list: PL,
+    length: usize,
+    sample_rate: Frequency,
+    delay: Time,
+    align_level: i32,
+) -> Vec<Complex64>
+where
+    PL: IntoIterator<Item = (ListBin, L)>,
+    L: IntoIterator<Item = (Time, PulseAmplitude)>,
+{
+    let mut waveform = vec![Complex64::new(0.0, 0.0); length];
+    for (bin, items) in list {
+        let ListBin {
+            envelope,
+            global_freq,
+            local_freq,
+        } = bin;
+        for (time, PulseAmplitude { amp, drag }) in items {
+            let t_start = time + delay;
+            let i_frac_start = AlignedIndex::new(t_start, sample_rate, align_level).unwrap();
+            let i_start = i_frac_start.ceil();
+            let index_offset = i_frac_start.index_offset();
+            let global_freq = global_freq.value();
+            let local_freq = local_freq.value();
+            let total_freq = global_freq + local_freq;
+            let dt = 1.0 / sample_rate.value();
+            let phase0 = global_freq * (i_start.value() * dt - delay.value())
+                + local_freq * index_offset.value() * dt;
+            let dphase = total_freq * dt;
+            let phase0 = phase0 * TAU;
+            let dphase = dphase * TAU;
+            let waveform = &mut waveform[i_start.value() as usize..];
+            if let Some(shape) = &envelope.shape {
+                let envelope = get_envelope(
+                    shape.clone(),
+                    envelope.width,
+                    envelope.plateau,
+                    index_offset,
+                    sample_rate,
+                );
+                let drag = drag * sample_rate.value();
+                mix_add_envelope(waveform, &envelope, amp, drag, phase0, dphase);
+            } else {
+                let plateau = envelope.plateau;
+                let i_plateau = (plateau.value() * sample_rate.value()).ceil() as usize;
+                mix_add_plateau(&mut waveform[..i_plateau], amp, phase0, dphase);
+            }
+        }
     }
+    waveform
 }
```

### Comparing `bosing-2.0.0b4/src/schedule/absolute.rs` & `bosing-2.0.0b5/src/schedule/absolute.rs`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b4/src/schedule/grid.rs` & `bosing-2.0.0b5/src/schedule/grid.rs`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b4/src/schedule/play.rs` & `bosing-2.0.0b5/src/schedule/play.rs`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b4/src/schedule/repeat.rs` & `bosing-2.0.0b5/src/schedule/repeat.rs`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b4/src/schedule/simple.rs` & `bosing-2.0.0b5/src/schedule/simple.rs`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b4/src/schedule/stack.rs` & `bosing-2.0.0b5/src/schedule/stack.rs`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b4/src/schedule.rs` & `bosing-2.0.0b5/src/schedule.rs`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b4/src/shape.rs` & `bosing-2.0.0b5/src/shape.rs`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b4/src/time.rs` & `bosing-2.0.0b5/src/quant.rs`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,50 @@
-use std::ops::Add;
+use std::ops::{Add, AddAssign};
 
-use anyhow::{anyhow, Result};
+use anyhow::Result;
 use ordered_float::NotNan;
 
 #[derive(Debug, Clone, Copy, PartialEq, Eq, Hash, PartialOrd, Ord)]
 pub struct Time(NotNan<f64>);
 
 #[derive(Debug, Clone, Copy, PartialEq, Eq, Hash, PartialOrd, Ord)]
+pub struct Frequency(NotNan<f64>);
+
+#[derive(Debug, Clone, Copy, PartialEq, Eq, Hash, PartialOrd, Ord)]
 pub struct AlignedIndex(NotNan<f64>);
 
 impl Time {
     pub fn new(value: f64) -> Result<Self> {
-        Ok(Self(
-            NotNan::new(value).map_err(|_| anyhow!("NaN in Time value"))?,
-        ))
+        Ok(Self(NotNan::new(value)?))
+    }
+
+    pub fn value(&self) -> f64 {
+        self.0.into_inner()
+    }
+}
+
+impl Frequency {
+    pub fn new(value: f64) -> Result<Self> {
+        Ok(Self(NotNan::new(value)?))
     }
 
     pub fn value(&self) -> f64 {
         self.0.into_inner()
     }
 }
 
 impl AlignedIndex {
-    pub fn new(time: Time, sample_rate: f64, align_level: i32) -> Result<Self> {
-        let scaled_sr = scaleb(sample_rate, -align_level);
+    pub fn new(time: Time, sample_rate: Frequency, align_level: i32) -> Result<Self> {
+        fn scaleb(x: f64, s: i32) -> f64 {
+            x * (s as f64).exp2()
+        }
+        let scaled_sr = scaleb(sample_rate.value(), -align_level);
         let i = (time.value() * scaled_sr).ceil();
         let aligned_index = scaleb(i, align_level);
-        Ok(Self(
-            NotNan::new(aligned_index).map_err(|_| anyhow!("NaN in AlignedIndex value"))?,
-        ))
+        Ok(Self(NotNan::new(aligned_index)?))
     }
 
     pub fn value(&self) -> f64 {
         self.0.into_inner()
     }
 
     pub fn ceil(&self) -> Self {
@@ -40,18 +52,20 @@
     }
 
     pub fn index_offset(&self) -> Self {
         Self(NotNan::new(self.0.ceil() - self.0.into_inner()).unwrap())
     }
 }
 
-fn scaleb(x: f64, s: i32) -> f64 {
-    x * (s as f64).exp2()
-}
-
 impl Add for Time {
     type Output = Self;
 
     fn add(self, rhs: Self) -> Self::Output {
         Self(self.0 + rhs.0)
     }
 }
+
+impl AddAssign for Time {
+    fn add_assign(&mut self, rhs: Self) {
+        self.0 += rhs.0;
+    }
+}
```

### Comparing `bosing-2.0.0b4/tests/test_basic.py` & `bosing-2.0.0b5/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b4/Cargo.lock` & `bosing-2.0.0b5/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "bosing"
-version = "2.0.0-beta.4"
+version = "2.0.0-beta.5"
 dependencies = [
  "anyhow",
  "bspline",
  "cached",
  "enum_dispatch",
  "float-cmp",
  "itertools",
```

### Comparing `bosing-2.0.0b4/pyproject.toml` & `bosing-2.0.0b5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering",
     "License :: OSI Approved :: MIT License",
 ]
 dependencies = ["numpy"]
 
 [project.urls]
-Documentation = "https://github.com/kahojyun/Bosing#readme"
+Documentation = "https://bosing.readthedocs.io"
 Issues = "https://github.com/kahojyun/Bosing/issues"
 Source = "https://github.com/kahojyun/Bosing"
 
 [tool.maturin]
 features = ["pyo3/extension-module"]
 
 [tool.hatch.envs.default]
```

### Comparing `bosing-2.0.0b4/PKG-INFO` & `bosing-2.0.0b5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: bosing
-Version: 2.0.0b4
+Version: 2.0.0b5
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: MIT License
@@ -12,15 +12,15 @@
 License-File: LICENSE.txt
 Summary: Waveform generator for pulse sequences in quantum computing
 Keywords: 
 Author-email: kaho <kaho0769@qq.com>
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: Documentation, https://github.com/kahojyun/Bosing#readme
+Project-URL: Documentation, https://bosing.readthedocs.io
 Project-URL: Issues, https://github.com/kahojyun/Bosing/issues
 Project-URL: Source, https://github.com/kahojyun/Bosing
 
 # Bosing
 
 [![Documentation Status](https://readthedocs.org/projects/bosing/badge/?version=latest)](https://bosing.readthedocs.io/zh-cn/latest/?badge=latest)
```

