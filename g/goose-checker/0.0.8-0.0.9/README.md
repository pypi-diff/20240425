# Comparing `tmp/goose_checker-0.0.8.tar.gz` & `tmp/goose_checker-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goose_checker-0.0.8.tar", max compression
+gzip compressed data, was "goose_checker-0.0.9.tar", max compression
```

## Comparing `goose_checker-0.0.8.tar` & `goose_checker-0.0.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1071 2024-04-19 02:46:29.815952 goose_checker-0.0.8/LICENSE
--rw-r--r--   0        0        0     1448 2024-04-19 02:46:29.815952 goose_checker-0.0.8/README.md
--rw-r--r--   0        0        0     5553 2024-04-19 02:46:29.815952 goose_checker-0.0.8/goose_checker/chains.py
--rw-r--r--   0        0        0     4394 2024-04-19 02:46:29.815952 goose_checker-0.0.8/goose_checker/cli.py
--rw-r--r--   0        0        0      779 2024-04-19 02:46:29.815952 goose_checker-0.0.8/goose_checker/context.py
--rw-r--r--   0        0        0     1390 2024-04-19 02:46:29.815952 goose_checker-0.0.8/goose_checker/diff.py
--rw-r--r--   0        0        0     2776 2024-04-19 02:46:29.815952 goose_checker-0.0.8/goose_checker/goose_ascii.py
--rw-r--r--   0        0        0     2386 2024-04-19 02:46:29.815952 goose_checker-0.0.8/goose_checker/models.py
--rw-r--r--   0        0        0     1164 2024-04-19 02:46:29.815952 goose_checker-0.0.8/goose_checker/prompts.py
--rw-r--r--   0        0        0      924 2024-04-19 02:46:29.815952 goose_checker-0.0.8/goose_checker/response_schema.py
--rw-r--r--   0        0        0      573 2024-04-19 02:46:29.815952 goose_checker-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     2159 1970-01-01 00:00:00.000000 goose_checker-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-04-19 21:41:19.074140 goose_checker-0.0.9/LICENSE
+-rw-r--r--   0        0        0     1448 2024-04-19 21:41:19.074140 goose_checker-0.0.9/README.md
+-rw-r--r--   0        0        0     5613 2024-04-19 21:41:19.074140 goose_checker-0.0.9/goose_checker/chains.py
+-rw-r--r--   0        0        0     4394 2024-04-19 21:41:19.074140 goose_checker-0.0.9/goose_checker/cli.py
+-rw-r--r--   0        0        0      779 2024-04-19 21:41:19.074140 goose_checker-0.0.9/goose_checker/context.py
+-rw-r--r--   0        0        0     1390 2024-04-19 21:41:19.074140 goose_checker-0.0.9/goose_checker/diff.py
+-rw-r--r--   0        0        0     2776 2024-04-19 21:41:19.074140 goose_checker-0.0.9/goose_checker/goose_ascii.py
+-rw-r--r--   0        0        0     2476 2024-04-19 21:41:19.074140 goose_checker-0.0.9/goose_checker/models.py
+-rw-r--r--   0        0        0     1081 2024-04-19 21:41:19.074140 goose_checker-0.0.9/goose_checker/prompts.py
+-rw-r--r--   0        0        0      816 2024-04-19 21:41:19.074140 goose_checker-0.0.9/goose_checker/response_schema.py
+-rw-r--r--   0        0        0      573 2024-04-19 21:41:19.078140 goose_checker-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2159 1970-01-01 00:00:00.000000 goose_checker-0.0.9/PKG-INFO
```

### Comparing `goose_checker-0.0.8/LICENSE` & `goose_checker-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `goose_checker-0.0.8/README.md` & `goose_checker-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `goose_checker-0.0.8/goose_checker/chains.py` & `goose_checker-0.0.9/goose_checker/chains.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import tiktoken
 from langchain.output_parsers import ResponseSchema, StructuredOutputParser
 from langchain.prompts import PromptTemplate
 
 from goose_checker.context import TerraformContext, get_terraform_context
 from goose_checker.diff import GitDiff
-from goose_checker.models import GooseChecker, GooseCheckerResponse
-from goose_checker.prompts import (aggregation_prompt, base_prompt,
-                                   terraform_prompt)
-from goose_checker.response_schema import (approve_or_deny_schema,
-                                           other_issues_explanation_schema,
-                                           silly_mistakes_explaination_schema,
-                                           silly_mistakes_aggregation_schema)
+from goose_checker.models import GooseChecker, GooseCheckerResponse, ApprovalChainResponse
+from goose_checker.prompts import aggregation_prompt, base_prompt, terraform_prompt
+from goose_checker.response_schema import (
+    approve_or_deny_schema,
+    cot_issues,
+    list_issues,
+    improvements_aggregation,
+)
 
 
 def get_token_len(string, model_name: str = "gpt-3.5-turbo"):
     encoding = tiktoken.encoding_for_model(model_name)  # Make this dynamic
     num_tokens = len(encoding.encode(string))
     return num_tokens
 
@@ -47,18 +48,16 @@
 
     return {"subprompt": subprompt, "tokens_used": tokens_used}
 
 
 def base_checker(diff: GitDiff, goose_checker: GooseChecker) -> GooseCheckerResponse:
 
     # Core chain to analyze terraform diff
-    response_schemas = [
-        silly_mistakes_explaination_schema,
-        other_issues_explanation_schema,
-    ]
+    response_schemas = [cot_issues,
+                        list_issues]
     output_parser = StructuredOutputParser.from_response_schemas(response_schemas)
     format_instructions = output_parser.get_format_instructions()
     model = goose_checker._get_model()
 
     diff_and_tokens_used: dict = _build_diff_subprompt(diff, goose_checker.quota)
 
     prompt_template = PromptTemplate.from_template(
@@ -70,28 +69,26 @@
     )
 
     chain = prompt_template | model | output_parser
 
     output = chain.invoke({})
     return GooseCheckerResponse(
         file_name=diff.file_name,
-        silly_mistakes=output["silly_mistakes_explanation"],
-        other_issues=output["other_issues_explanation"],
+        chain_of_thought=output["chain_of_thought_on_issues"],
+        issues=output["list_issues"].split(","),
     )
 
 
 def terraform_checker(
     diff: GitDiff, goose_checker: GooseChecker
 ) -> GooseCheckerResponse:
 
     # Core chain to analyze terraform diff
-    response_schemas = [
-        silly_mistakes_explaination_schema,
-        other_issues_explanation_schema,
-    ]
+    response_schemas = [cot_issues,
+                        list_issues]
     output_parser = StructuredOutputParser.from_response_schemas(response_schemas)
     format_instructions = output_parser.get_format_instructions()
     model = goose_checker._get_model()
     format_len = get_token_len(format_instructions)
 
     # 1. Build Context
     terraform_context = get_terraform_context(diff)
@@ -124,41 +121,47 @@
     )
 
     chain = prompt_template | model | output_parser
 
     output = chain.invoke({})
     return GooseCheckerResponse(
         file_name=diff.file_name,
-        silly_mistakes=output["silly_mistakes_explanation"],
-        other_issues=output["other_issues_explanation"],
+        chain_of_thought=output["chain_of_thought_on_issues"],
+        issues=output["list_issues"].split(","),
     )
 
 
 def approve_or_deny(
     responses: list[GooseCheckerResponse], goose_checker: GooseChecker
-) -> tuple[bool, str]:
-    response_schemas = [silly_mistakes_aggregation_schema, approve_or_deny_schema]
+) -> ApprovalChainResponse:
+    response_schemas = [improvements_aggregation, approve_or_deny_schema]
     output_parser = StructuredOutputParser.from_response_schemas(response_schemas)
     format_instructions = output_parser.get_format_instructions()
     model = goose_checker._get_model()
 
     evaluations_subprompt = ""
 
     for response in responses:
         evaluations_subprompt = f"""
         file_name: {response.file_name}
-        silly_mistakes: {response.silly_mistakes}
+        Feedback: {response.chain_of_thought}
         """
 
     prompt_template = PromptTemplate.from_template(
         aggregation_prompt,
         partial_variables={
             "format_instructions": format_instructions,
             "evaluations_subprompt": evaluations_subprompt,
         },
     )
 
     chain = prompt_template | model | output_parser
 
     result = chain.invoke({})
 
-    return (result["approve_or_deny"], result["silly_mistakes"])
+    if isinstance(result['approve_or_deny'], str):
+        if result['approve_or_deny'].lower().strip() == "true":
+            result['approve_or_deny'] = True
+        elif result['approve_or_deny'].lower().strip() == "false":
+            result['approve_or_deny'] = False
+
+    return ApprovalChainResponse(approved = result["approve_or_deny"], instructions_to_engineer = result["instructions_to_engineer"])
```

### Comparing `goose_checker-0.0.8/goose_checker/cli.py` & `goose_checker-0.0.9/goose_checker/cli.py`

 * *Files identical despite different names*

### Comparing `goose_checker-0.0.8/goose_checker/context.py` & `goose_checker-0.0.9/goose_checker/context.py`

 * *Files identical despite different names*

### Comparing `goose_checker-0.0.8/goose_checker/diff.py` & `goose_checker-0.0.9/goose_checker/diff.py`

 * *Files identical despite different names*

### Comparing `goose_checker-0.0.8/goose_checker/goose_ascii.py` & `goose_checker-0.0.9/goose_checker/goose_ascii.py`

 * *Files identical despite different names*

### Comparing `goose_checker-0.0.8/goose_checker/models.py` & `goose_checker-0.0.9/goose_checker/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,17 +13,20 @@
 
     def _get_model(self):
         raise NotImplementedError("Subclasses must implement this method")
 
 
 class GooseCheckerResponse(BaseModel):
     file_name: str
-    silly_mistakes: str
-    other_issues: str
+    chain_of_thought: str
+    issues: list
 
+class ApprovalChainResponse(BaseModel):
+    approved: bool
+    instructions_to_engineer: str
 
 class OpenAIGooseChecker(GooseChecker):
     model: str
 
     @property
     def quota(self) -> int:
         if self.model == "gpt-3.5-turbo":
```

### Comparing `goose_checker-0.0.8/goose_checker/prompts.py` & `goose_checker-0.0.9/goose_checker/prompts.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,35 @@
 terraform_prompt = """
 << INSTRUCTIONS >>
 You are an software engineer reviewing a pull request by analyzing the DIFF of a terraform file
-Consider the following code snippets provided as CONTEXT, keep in mind they may not be complete
+Keep in mind the DIFF may not be complete so at the edges of the diff you may see mistakes that are not actually mistakes.
 
 
 << CONTEXT >>
 {context_subprompt}
 
 << DIFF >>
 {diff_subprompt}
 
 << TASK >>
 
-Focus on the following:
-1. Naming conventions and idiomatic code
-2. Consistency between CONTEXT and the DIFF
-
 << FORMAT INSTRUCTIONS >>
 {format_instructions}
 """
 
 base_prompt = """
 << INSTRUCTIONS >>
 You are an software engineer reviewing a pull request by analyzing the DIFF
-Keep in mind the DIFF may not be complete
+Keep in mind the DIFF may not be complete so at the edges of the diff you may see mistakes that are not actually mistakes.
 
 << DIFF >>
 {diff_subprompt}
 
 << TASK >>
 
-Focus on the following:
-1. Naming conventions and idiomatic code
-2. Clean Code
-
-
 << FORMAT INSTRUCTIONS >>
 {format_instructions}
 
 """
 
 
 aggregation_prompt = """
```

### Comparing `goose_checker-0.0.8/pyproject.toml` & `goose_checker-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "goose-checker"
-version = "0.0.8"
+version = "0.0.9"
 description = "State of the Art Silly Goose Detection Technology"
 authors = ["AdamPaslawski <adampaslawski@gmail.com>"]
 readme = "README.md"
 packages = [{include = "goose_checker"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `goose_checker-0.0.8/PKG-INFO` & `goose_checker-0.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goose-checker
-Version: 0.0.8
+Version: 0.0.9
 Summary: State of the Art Silly Goose Detection Technology
 Author: AdamPaslawski
 Author-email: adampaslawski@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

