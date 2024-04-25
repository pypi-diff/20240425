# Comparing `tmp/ommx_python_mip_adapter-0.1.0.tar.gz` & `tmp/ommx_python_mip_adapter-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ommx_python_mip_adapter-0.1.0.tar", last modified: Mon Apr 22 06:27:48 2024, max compression
+gzip compressed data, was "ommx_python_mip_adapter-0.1.1.tar", last modified: Thu Apr 25 07:15:26 2024, max compression
```

## Comparing `ommx_python_mip_adapter-0.1.0.tar` & `ommx_python_mip_adapter-0.1.1.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 06:27:48.794463 ommx_python_mip_adapter-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 06:27:48.786463 ommx_python_mip_adapter-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 06:27:48.790463 ommx_python_mip_adapter-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-22 06:27:40.000000 ommx_python_mip_adapter-0.1.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-22 06:27:40.000000 ommx_python_mip_adapter-0.1.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-22 06:27:40.000000 ommx_python_mip_adapter-0.1.0/.github/workflows/test_and_lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-04-22 06:27:40.000000 ommx_python_mip_adapter-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    10846 2024-04-22 06:27:40.000000 ommx_python_mip_adapter-0.1.0/LICENSE-APACHE
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-22 06:27:40.000000 ommx_python_mip_adapter-0.1.0/LICENSE-MIT
--rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-04-22 06:27:48.794463 ommx_python_mip_adapter-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-04-22 06:27:40.000000 ommx_python_mip_adapter-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 06:27:48.786463 ommx_python_mip_adapter-0.1.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 06:27:48.790463 ommx_python_mip_adapter-0.1.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-22 06:27:40.000000 ommx_python_mip_adapter-0.1.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-22 06:27:40.000000 ommx_python_mip_adapter-0.1.0/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 06:27:48.790463 ommx_python_mip_adapter-0.1.0/ommx_python_mip_adapter/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-22 06:27:40.000000 ommx_python_mip_adapter-0.1.0/ommx_python_mip_adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-22 06:27:48.000000 ommx_python_mip_adapter-0.1.0/ommx_python_mip_adapter/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     9189 2024-04-22 06:27:40.000000 ommx_python_mip_adapter-0.1.0/ommx_python_mip_adapter/adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-22 06:27:40.000000 ommx_python_mip_adapter-0.1.0/ommx_python_mip_adapter/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 06:27:48.794463 ommx_python_mip_adapter-0.1.0/ommx_python_mip_adapter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-04-22 06:27:48.000000 ommx_python_mip_adapter-0.1.0/ommx_python_mip_adapter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-22 06:27:48.000000 ommx_python_mip_adapter-0.1.0/ommx_python_mip_adapter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 06:27:48.000000 ommx_python_mip_adapter-0.1.0/ommx_python_mip_adapter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-22 06:27:48.000000 ommx_python_mip_adapter-0.1.0/ommx_python_mip_adapter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-22 06:27:48.000000 ommx_python_mip_adapter-0.1.0/ommx_python_mip_adapter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-22 06:27:40.000000 ommx_python_mip_adapter-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 06:27:48.794463 ommx_python_mip_adapter-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 06:27:48.794463 ommx_python_mip_adapter-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 06:27:40.000000 ommx_python_mip_adapter-0.1.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-04-22 06:27:40.000000 ommx_python_mip_adapter-0.1.0/tests/test_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-22 06:27:40.000000 ommx_python_mip_adapter-0.1.0/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-04-22 06:27:40.000000 ommx_python_mip_adapter-0.1.0/tests/test_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:15:26.851477 ommx_python_mip_adapter-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:15:26.839477 ommx_python_mip_adapter-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:15:26.843478 ommx_python_mip_adapter-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-25 07:15:20.000000 ommx_python_mip_adapter-0.1.1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-25 07:15:20.000000 ommx_python_mip_adapter-0.1.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-25 07:15:20.000000 ommx_python_mip_adapter-0.1.1/.github/workflows/test_and_lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-04-25 07:15:20.000000 ommx_python_mip_adapter-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    10846 2024-04-25 07:15:20.000000 ommx_python_mip_adapter-0.1.1/LICENSE-APACHE
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-25 07:15:20.000000 ommx_python_mip_adapter-0.1.1/LICENSE-MIT
+-rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-04-25 07:15:26.847478 ommx_python_mip_adapter-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-04-25 07:15:20.000000 ommx_python_mip_adapter-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:15:26.843478 ommx_python_mip_adapter-0.1.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:15:26.843478 ommx_python_mip_adapter-0.1.1/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-25 07:15:20.000000 ommx_python_mip_adapter-0.1.1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-25 07:15:20.000000 ommx_python_mip_adapter-0.1.1/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:15:26.843478 ommx_python_mip_adapter-0.1.1/ommx_python_mip_adapter/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-25 07:15:20.000000 ommx_python_mip_adapter-0.1.1/ommx_python_mip_adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-25 07:15:26.000000 ommx_python_mip_adapter-0.1.1/ommx_python_mip_adapter/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14584 2024-04-25 07:15:20.000000 ommx_python_mip_adapter-0.1.1/ommx_python_mip_adapter/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-25 07:15:20.000000 ommx_python_mip_adapter-0.1.1/ommx_python_mip_adapter/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:15:26.847478 ommx_python_mip_adapter-0.1.1/ommx_python_mip_adapter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-04-25 07:15:26.000000 ommx_python_mip_adapter-0.1.1/ommx_python_mip_adapter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-25 07:15:26.000000 ommx_python_mip_adapter-0.1.1/ommx_python_mip_adapter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 07:15:26.000000 ommx_python_mip_adapter-0.1.1/ommx_python_mip_adapter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-25 07:15:26.000000 ommx_python_mip_adapter-0.1.1/ommx_python_mip_adapter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-25 07:15:26.000000 ommx_python_mip_adapter-0.1.1/ommx_python_mip_adapter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-25 07:15:20.000000 ommx_python_mip_adapter-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 07:15:26.851477 ommx_python_mip_adapter-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:15:26.847478 ommx_python_mip_adapter-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 07:15:20.000000 ommx_python_mip_adapter-0.1.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3817 2024-04-25 07:15:20.000000 ommx_python_mip_adapter-0.1.1/tests/test_instance_to_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-04-25 07:15:20.000000 ommx_python_mip_adapter-0.1.1/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8264 2024-04-25 07:15:20.000000 ommx_python_mip_adapter-0.1.1/tests/test_model_to_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-25 07:15:20.000000 ommx_python_mip_adapter-0.1.1/tests/test_model_to_solution.py
```

### Comparing `ommx_python_mip_adapter-0.1.0/.github/workflows/docs.yml` & `ommx_python_mip_adapter-0.1.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `ommx_python_mip_adapter-0.1.0/.github/workflows/publish.yml` & `ommx_python_mip_adapter-0.1.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `ommx_python_mip_adapter-0.1.0/.github/workflows/test_and_lint.yml` & `ommx_python_mip_adapter-0.1.1/.github/workflows/test_and_lint.yml`

 * *Files identical despite different names*

### Comparing `ommx_python_mip_adapter-0.1.0/.gitignore` & `ommx_python_mip_adapter-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `ommx_python_mip_adapter-0.1.0/LICENSE-APACHE` & `ommx_python_mip_adapter-0.1.1/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `ommx_python_mip_adapter-0.1.0/LICENSE-MIT` & `ommx_python_mip_adapter-0.1.1/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `ommx_python_mip_adapter-0.1.0/README.md` & `ommx_python_mip_adapter-0.1.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -4,27 +4,39 @@
 
 This package provides an adaptor for the [Python-MIP](https://www.python-mip.com/) from/to [OMMX](https://github.com/Jij-Inc/ommx)
 
 Python-MIP as a solver in OMMX toolchain
 -----------------------------------------
 ```mermaid
 sequenceDiagram
-    participant O as Other OMMX toolchain
+    participant U as User
     participant A as Adapter
     participant P as Python-MIP
-    O->>A: ommx::Instance and Parameters for Python-MIP;
-    A->>P: Translate into Python-MIP input
+    U->>A: ommx.v1.Instance
+    A->>U: Python-MIP model
+    U->>P: Python-MIP model and Parameters for Python-MIP;
     P->>P: Solve with CBC, Gurobi, or other solvers
-    P->>A: Solution
-    A->>O: ommx:Solution
+    P->>U: Optimized model
+    U->>A: Optimized model and ommx.v1.Instance
+    A->>U: ommx:SolutionList
 ```
 
 Python-MIP as a user interface to create OMMX instance
 -------------------------------------------------------
-TBW
+```mermaid
+sequenceDiagram
+    participant U as User
+    participant A as Adapter
+    participant O as Other OMMX toolchain
+    U->>A: Python-MIP model
+    A->>U: ommx.v1.Instance
+    U->>O: ommx.v1.Instance and Parameters for other solver
+    O->>O: Solve the instance with other solver using other adapter
+    O->>U: ommx.v1.Solution
+```
 
 Usage
 ======
 `ommx-python-mip-adapter` can be installed from PyPI as follows:
 
 ```bash
 pip install ommx-python-mip-adapter
@@ -62,11 +74,27 @@
 # Create `ommx.v1.SolutionList` from Optimized `mip.Model`
 ommx_solutions_bytes = adapter.model_to_solution(
     model, ommx_instance_bytes
 )
 
 print(SolutionList.FromString(ommx_solutions_bytes))
 ```
+You can get `ommx.v1.Instance` from a Python-MIP model as the following:
+```python markdown-code-runner
+import mip
+import ommx_python_mip_adapter as adapter
+from ommx.v1.instance_pb2 import Instance
+
+model = mip.Model()
+x1=model.add_var(name="1", var_type=mip.INTEGER, lb=0, ub=5)
+x2=model.add_var(name="2", var_type=mip.CONTINUOUS, lb=0, ub=5)
+model.objective = - x1 - 2 * x2
+model.add_constr(x1 + x2 - 6 <= 0)
+
+ommx_instance_bytes = adapter.model_to_instance(model)
+
+print(Instance.FromString(ommx_instance_bytes))
+```
 
 Reference
 ==============
 - [OMMX-Python-MIP-Adapter API Reference](https://jij-inc.github.io/ommx-python-mip-adapter/index.html)
```

### Comparing `ommx_python_mip_adapter-0.1.0/docs/source/conf.py` & `ommx_python_mip_adapter-0.1.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `ommx_python_mip_adapter-0.1.0/ommx_python_mip_adapter/adapter.py` & `ommx_python_mip_adapter-0.1.1/ommx_python_mip_adapter/adapter.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import typing as tp
 
 import mip
 
+from mip.exceptions import ParameterNotAvailable
 from ommx.v1.constraint_pb2 import Constraint
-from ommx.v1.decision_variables_pb2 import DecisionVariable
+from ommx.v1.decision_variables_pb2 import DecisionVariable, Bound
 from ommx.v1.function_pb2 import Function
 from ommx.v1.instance_pb2 import Instance
+from ommx.v1.linear_pb2 import Linear
 from ommx.v1.solution_pb2 import Solution, SolutionList
 
 from ommx_python_mip_adapter.exception import OMMXPythonMIPAdapterError
 
 
 class PythonMIPBuilder:
     def __init__(
@@ -117,14 +119,139 @@
         self._set_decision_variables()
         self._set_objective_function()
         self._set_constraints()
 
         return self._model
 
 
+class OMMXInstanceBuilder:
+    def __init__(
+        self,
+        model: mip.Model,
+    ):
+        self._model = model
+
+    def _decision_variables(self) -> tp.List[DecisionVariable]:
+        decision_variables = []
+
+        for var in self._model.vars:
+            if var.var_type == mip.BINARY:
+                kind = DecisionVariable.KIND_BINARY
+            elif var.var_type == mip.INTEGER:
+                kind = DecisionVariable.KIND_INTEGER
+            elif var.var_type == mip.CONTINUOUS:
+                kind = DecisionVariable.KIND_CONTINUOUS
+            else:
+                raise OMMXPythonMIPAdapterError(
+                    f"Not supported variable type. "
+                    f"idx: {var.idx} name: {var.name}, type: {var.var_type}"
+                )
+
+            decision_variables.append(
+                DecisionVariable(
+                    id=var.idx,
+                    kind=kind,
+                    bound=Bound(lower=var.lb, upper=var.ub),
+                    description=DecisionVariable.Description(name=var.name)
+                )
+            )
+
+        return decision_variables
+    
+
+    def _make_function_from_lin_expr(
+        self,
+        lin_expr: mip.LinExpr,
+    ) -> Function:
+        terms = [
+            Linear.Term(id=var.idx, coefficient=coeff)    # type: ignore
+            for var, coeff in lin_expr.expr.items()
+        ]
+        constant: float = lin_expr.const    # type: ignore
+
+        # If the terms are empty, the function is a constant.
+        if len(terms) == 0:
+            return Function(constant=constant)
+        else:
+            return Function(
+                linear=Linear(terms=terms, constant=constant)
+            )
+
+
+    def _objective(self) -> Function:
+        # In Python-MIP, it is allowed not to set the objective function.
+        # If it isn't set, the model behaves as if the objective function is set to 0.
+        # However, an error occurs when accessing `.objective`.
+        # So if an error occurs, treat the objective function as 0.
+        try:
+            objective = self._model.objective
+        except ParameterNotAvailable:
+            return Function(constant=0)
+        
+        return self._make_function_from_lin_expr(objective)
+
+
+    def _constraints(self) -> tp.List[Constraint]:
+        constraints = []
+
+        for constr in self._model.constrs:
+            id = constr.idx
+            lin_expr = constr.expr
+            name = constr.name
+
+            if lin_expr.sense == "=":
+                constraint = Constraint(
+                    id=id,
+                    equality=Constraint.EQUALITY_EQUAL_TO_ZERO,
+                    function=self._make_function_from_lin_expr(lin_expr),
+                    description=Constraint.Description(name=name),
+                )
+            elif lin_expr.sense == "<":
+                constraint = Constraint(
+                    id=id,
+                    equality=Constraint.EQUALITY_LESS_THAN_OR_EQUAL_TO_ZERO,
+                    function=self._make_function_from_lin_expr(lin_expr),
+                    description=Constraint.Description(name=name),
+                )
+            elif lin_expr.sense == ">":
+                # `ommx.v1.Constraint` does not support `GREATER_THAN_OR_EQUAL_TO_ZERO`.
+                # So multiply the linear expression by -1.
+                constraint = Constraint(
+                    id=id,
+                    equality=Constraint.EQUALITY_LESS_THAN_OR_EQUAL_TO_ZERO,
+                    function=self._make_function_from_lin_expr(-lin_expr),
+                    description=Constraint.Description(name=name),
+                )
+            else:
+                raise OMMXPythonMIPAdapterError(
+                    f"Not supported constraint sense: "
+                    f"name: {constr.name}, sense: {lin_expr.sense}"
+                )
+            
+            constraints.append(constraint)
+
+        return constraints
+
+
+    def _sense(self):
+        if self._model.sense == mip.MAXIMIZE:
+            return Instance.SENSE_MAXIMIZE
+        else:
+            return Instance.SENSE_MINIMIZE
+
+
+    def build(self) -> bytes:
+        return Instance(
+            decision_variables=self._decision_variables(),
+            objective=self._objective(),
+            constraints=self._constraints(),
+            sense=self._sense(),
+        ).SerializeToString()
+
+
 def instance_to_model(
     ommx_instance_bytes: bytes,
     *,
     sense: str = mip.MINIMIZE,
     solver_name: str = mip.CBC,
     solver: tp.Optional[mip.Solver] = None,
 ) -> mip.Model:
@@ -181,14 +308,43 @@
         sense=sense,
         solver_name=solver_name,
         solver=solver,
     )
     return builder.build()
 
 
+def model_to_instance(model: mip.Model) -> bytes:
+    """
+    The function to convert Python-MIP Model to ommx.v1.Instance.
+
+    Args:
+        model (mip.Model): Python-MIP Model.
+    
+    Returns:
+        bytes: Serialized ommx.v1.Instance.
+
+    Raises:
+        OMMXPythonMIPAdapterError: If converting is not possible.
+
+    Examples:
+        >>> import mip
+        >>> import ommx_python_mip_adapter as adapter
+        >>> from ommx.v1.instance_pb2 import Instance
+        >>> model = mip.Model()
+        >>> x1=model.add_var(name="1", var_type=mip.INTEGER, lb=0, ub=5)
+        >>> x2=model.add_var(name="2", var_type=mip.CONTINUOUS, lb=0, ub=5)
+        >>> model.objective = - x1 - 2 * x2
+        >>> constr = model.add_constr(x1 + x2 - 6 <= 0)
+        >>> ommx_instance_bytes = adapter.model_to_instance(model)
+        >>> ommx_instance = Instance.FromString(ommx_instance_bytes)
+    """
+    builder = OMMXInstanceBuilder(model)
+    return builder.build()
+
+
 def model_to_solution(
     model: mip.Model,
     ommx_instance_bytes: bytes,
 ) -> bytes:
     """
     The function to create ommx.v1.SolutionList from optimized Python-MIP Model.
```

### Comparing `ommx_python_mip_adapter-0.1.0/ommx_python_mip_adapter.egg-info/SOURCES.txt` & `ommx_python_mip_adapter-0.1.1/ommx_python_mip_adapter.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -14,10 +14,11 @@
 ommx_python_mip_adapter/exception.py
 ommx_python_mip_adapter.egg-info/PKG-INFO
 ommx_python_mip_adapter.egg-info/SOURCES.txt
 ommx_python_mip_adapter.egg-info/dependency_links.txt
 ommx_python_mip_adapter.egg-info/requires.txt
 ommx_python_mip_adapter.egg-info/top_level.txt
 tests/conftest.py
-tests/test_adapter.py
-tests/test_import.py
-tests/test_integration.py
+tests/test_instance_to_model.py
+tests/test_integration.py
+tests/test_model_to_instance.py
+tests/test_model_to_solution.py
```

### Comparing `ommx_python_mip_adapter-0.1.0/pyproject.toml` & `ommx_python_mip_adapter-0.1.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "License :: OSI Approved :: Apache Software License",
     "License :: OSI Approved :: MIT License",
 ]
 dependencies = [
-    "ommx >= 0.1.1, < 0.2.0",
+    "ommx >= 0.2.0, < 0.3.0",
     "mip",
 ]
 
 
 [project.optional-dependencies]
 dev = [
     "markdown-code-runner",
```

### Comparing `ommx_python_mip_adapter-0.1.0/tests/test_adapter.py` & `ommx_python_mip_adapter-0.1.1/tests/test_instance_to_model.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-import mip
 import pytest
 
 from ommx.v1.constraint_pb2 import Constraint
 from ommx.v1.decision_variables_pb2 import DecisionVariable
 from ommx.v1.function_pb2 import Function
 from ommx.v1.instance_pb2 import Instance
 from ommx.v1.linear_pb2 import Linear
 from ommx.v1.quadratic_pb2 import Quadratic
-from ommx.testing import SingleFeasibleLPGenerator, DataType
 
 import ommx_python_mip_adapter as adapter
 
 from ommx_python_mip_adapter.exception import OMMXPythonMIPAdapterError
 
+
 def test_error_invalid_instance():
     with pytest.raises(OMMXPythonMIPAdapterError) as e:
         adapter.instance_to_model(b"invalid")
     assert "Invalid `ommx_instance_bytes`" in str(e.value)
 
 
 def test_error_not_suppoerted_decision_variable():
@@ -122,26 +121,7 @@
         ],
     )
     ommx_instance_bytes = ommx_instance.SerializeToString()
 
     with pytest.raises(OMMXPythonMIPAdapterError) as e:
         adapter.instance_to_model(ommx_instance_bytes)
     assert "Not supported constraint equality" in str(e.value)
-
-
-def test_error_not_optimized_model():
-    model = mip.Model()
-
-    with pytest.raises(OMMXPythonMIPAdapterError) as e:
-        adapter.model_to_solution(model, b"")
-    assert "`model.status` must be " in str(e.value)
-
-
-def test_error_invalid_ommx_instance_bytes():
-    generator = SingleFeasibleLPGenerator(10, DataType.INT)
-    ommx_instance_bytes = generator.get_v1_instance()
-    model = adapter.instance_to_model(ommx_instance_bytes)
-    model.optimize()
-
-    with pytest.raises(OMMXPythonMIPAdapterError) as e:
-        adapter.model_to_solution(model, b"invalid")
-    assert "Invalid `ommx_instance_bytes`" in str(e.value)
```

### Comparing `ommx_python_mip_adapter-0.1.0/tests/test_integration.py` & `ommx_python_mip_adapter-0.1.1/tests/test_integration.py`

 * *Files identical despite different names*

