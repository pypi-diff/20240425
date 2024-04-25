# Comparing `tmp/dir2prompt-1.0.3.tar.gz` & `tmp/dir2prompt-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dir2prompt-1.0.3.tar", last modified: Wed Apr  3 04:12:22 2024, max compression
+gzip compressed data, was "dir2prompt-1.0.4.tar", last modified: Thu Apr 25 16:41:51 2024, max compression
```

## Comparing `dir2prompt-1.0.3.tar` & `dir2prompt-1.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 mkieffer   (501) staff       (20)        0 2024-04-03 04:12:22.823168 dir2prompt-1.0.3/
--rw-r--r--   0 mkieffer   (501) staff       (20)     1069 2024-04-02 23:08:45.000000 dir2prompt-1.0.3/LICENSE
--rw-r--r--   0 mkieffer   (501) staff       (20)     6060 2024-04-03 04:12:22.822974 dir2prompt-1.0.3/PKG-INFO
--rw-r--r--   0 mkieffer   (501) staff       (20)     3758 2024-04-03 04:09:21.000000 dir2prompt-1.0.3/README.md
-drwxr-xr-x   0 mkieffer   (501) staff       (20)        0 2024-04-03 04:12:22.822732 dir2prompt-1.0.3/dir2prompt.egg-info/
--rw-r--r--   0 mkieffer   (501) staff       (20)     6060 2024-04-03 04:12:22.000000 dir2prompt-1.0.3/dir2prompt.egg-info/PKG-INFO
--rw-r--r--   0 mkieffer   (501) staff       (20)      257 2024-04-03 04:12:22.000000 dir2prompt-1.0.3/dir2prompt.egg-info/SOURCES.txt
--rw-r--r--   0 mkieffer   (501) staff       (20)        1 2024-04-03 04:12:22.000000 dir2prompt-1.0.3/dir2prompt.egg-info/dependency_links.txt
--rw-r--r--   0 mkieffer   (501) staff       (20)       37 2024-04-03 04:12:22.000000 dir2prompt-1.0.3/dir2prompt.egg-info/entry_points.txt
--rw-r--r--   0 mkieffer   (501) staff       (20)        4 2024-04-03 04:12:22.000000 dir2prompt-1.0.3/dir2prompt.egg-info/top_level.txt
--rw-r--r--   0 mkieffer   (501) staff       (20)     1241 2024-04-03 04:12:19.000000 dir2prompt-1.0.3/pyproject.toml
--rw-r--r--   0 mkieffer   (501) staff       (20)       38 2024-04-03 04:12:22.823212 dir2prompt-1.0.3/setup.cfg
--rw-r--r--   0 mkieffer   (501) staff       (20)     1370 2024-04-03 04:12:15.000000 dir2prompt-1.0.3/setup.py
-drwxr-xr-x   0 mkieffer   (501) staff       (20)        0 2024-04-03 04:12:22.822522 dir2prompt-1.0.3/src/
--rw-r--r--   0 mkieffer   (501) staff       (20)        0 2024-04-02 07:15:41.000000 dir2prompt-1.0.3/src/__init__.py
--rw-r--r--   0 mkieffer   (501) staff       (20)      978 2024-04-02 23:57:47.000000 dir2prompt-1.0.3/src/config.json
--rw-r--r--   0 mkieffer   (501) staff       (20)     7390 2024-04-03 03:29:17.000000 dir2prompt-1.0.3/src/d2p.py
+drwxr-xr-x   0 mkieffer   (501) staff       (20)        0 2024-04-25 16:41:51.109622 dir2prompt-1.0.4/
+-rw-r--r--   0 mkieffer   (501) staff       (20)     1069 2024-04-02 23:08:45.000000 dir2prompt-1.0.4/LICENSE
+-rw-r--r--   0 mkieffer   (501) staff       (20)     6624 2024-04-25 16:41:51.109409 dir2prompt-1.0.4/PKG-INFO
+-rw-r--r--   0 mkieffer   (501) staff       (20)     4322 2024-04-25 15:53:20.000000 dir2prompt-1.0.4/README.md
+drwxr-xr-x   0 mkieffer   (501) staff       (20)        0 2024-04-25 16:41:51.109151 dir2prompt-1.0.4/dir2prompt.egg-info/
+-rw-r--r--   0 mkieffer   (501) staff       (20)     6624 2024-04-25 16:41:51.000000 dir2prompt-1.0.4/dir2prompt.egg-info/PKG-INFO
+-rw-r--r--   0 mkieffer   (501) staff       (20)      257 2024-04-25 16:41:51.000000 dir2prompt-1.0.4/dir2prompt.egg-info/SOURCES.txt
+-rw-r--r--   0 mkieffer   (501) staff       (20)        1 2024-04-25 16:41:51.000000 dir2prompt-1.0.4/dir2prompt.egg-info/dependency_links.txt
+-rw-r--r--   0 mkieffer   (501) staff       (20)       37 2024-04-25 16:41:51.000000 dir2prompt-1.0.4/dir2prompt.egg-info/entry_points.txt
+-rw-r--r--   0 mkieffer   (501) staff       (20)        4 2024-04-25 16:41:51.000000 dir2prompt-1.0.4/dir2prompt.egg-info/top_level.txt
+-rw-r--r--   0 mkieffer   (501) staff       (20)     1241 2024-04-25 16:41:44.000000 dir2prompt-1.0.4/pyproject.toml
+-rw-r--r--   0 mkieffer   (501) staff       (20)       38 2024-04-25 16:41:51.109690 dir2prompt-1.0.4/setup.cfg
+-rw-r--r--   0 mkieffer   (501) staff       (20)     1370 2024-04-03 04:12:15.000000 dir2prompt-1.0.4/setup.py
+drwxr-xr-x   0 mkieffer   (501) staff       (20)        0 2024-04-25 16:41:51.108928 dir2prompt-1.0.4/src/
+-rw-r--r--   0 mkieffer   (501) staff       (20)       40 2024-04-25 14:40:29.000000 dir2prompt-1.0.4/src/__init__.py
+-rw-r--r--   0 mkieffer   (501) staff       (20)      978 2024-04-02 23:57:47.000000 dir2prompt-1.0.4/src/config.json
+-rw-r--r--   0 mkieffer   (501) staff       (20)     7916 2024-04-25 16:39:29.000000 dir2prompt-1.0.4/src/d2p.py
```

### Comparing `dir2prompt-1.0.3/LICENSE` & `dir2prompt-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dir2prompt-1.0.3/PKG-INFO` & `dir2prompt-1.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dir2prompt
-Version: 1.0.3
+Version: 1.0.4
 Summary: Generate prompts for long-context LLMs using the content in your directory
 Home-page: https://github.com/mkieffer1107/dir2prompt
 Author: Max Kieffer
 Author-email: Max Kieffer <wkieffer@ufl.edu>
 License: MIT License
         
         Copyright (c) 2024 mkieffer1107
@@ -62,14 +62,22 @@
 To generate a prompt from a directory, use the `d2p` command followed by the desired options:
 
 ```sh
 d2p --dir [directory path] --filters [file extensions] --outpath [output path] --outfile [output file name] --ignore-dir [directories to ignore] --ignore-file [files to ignore] --config [path to config file]
 
 ```
 
+For ease of use, you can select a directory by passing it in as a positional argument
+
+```sh
+d2p [directory path]
+```
+
+If both the positional argument and the `--dir` flag are provided, the `--dir` flag takes priority.
+
 ## Options ⚙️
 
 `--dir`: The directory to generate the prompt for (default: current directory).
 
 `--filters`: File extensions to include in the prompt (default: all files).
 
 `--outpath`: The output path for the prompt file (default: current directory).
@@ -83,35 +91,36 @@
 `--config`: Path to a custom config file (default: `config.json` in the package directory).
 
 ## Example 🌟
 
 Here's an example of how to use `dir2prompt` to generate a prompt:
 
 ```sh
-d2p --dir /path/<dir_name> --filters .py .txt --ignore-dir experiments __pycache__ --ignore-file old.py
+d2p --dir /path/<dir_name> --filters .py .txt .md .ipynb --ignore-dir experiments __pycache__ --ignore-file old.py
 ```
 
-This command will generate a prompt for the specified directory, including only files with the extensions `.py` and `.txt`, ignoring the `experiments` and `__pycache__` directories, and ignoring the `old.py` file. 
+This command will generate a prompt for the specified directory, including only files with the extensions `.py`, `.txt`, `.md`, `.ipynb`, ignoring the `experiments` and `__pycache__` directories, and ignoring the `old.py` file. 
 
-Note that ignored directories are not included in the directory tree, but that ignored files are. However, the content of the ignored files will not be written to the final prompt under the `<files>` tag.
+Note that ignored directories are not included in the directory tree, but that ignored files are. However, the content of the ignored files will not be written to the final prompt under the `<files>` tag. This might be changed later...
 
 In this example, the generated prompt will be saved as a `.txt` file in the directory that `d2p` is called in with the name `<dir_name>_prompt.txt`, and will have the following structure:
 
 **<dir_name>_prompt.txt**
 ```xml
 <context>
 <directory_tree>
 project/
 ├── README.md
-├── experiments/
 ├── requirements.txt
 └── src/
     ├── __init__.py
     ├── main.py
-    └── old.py
+    ├── old.py
+    ├── production.ipynb
+    └── testing.rs
 </directory_tree>
 
 <files>
 
 <file>
 <path>README.md</path>
 <content>
@@ -146,14 +155,32 @@
     print("Hello, World!")
 
 if __name__ == "__main__":
     main()
 </content>
 </file>
 
+<file>
+<path>src/production.ipynb</path>
+<content>
+---------- Cell 1 (markdown) ----------
+### Biologically inspired artificial neuron 
+
+$$
+y = mx + b
+$$
+
+---------- Cell 2 (code) ----------
+def neuron(x, m, b):
+    return m * x + b
+
+
+</content>
+</file>
+
 </files>
 </context>
 ```
 
 You can then feed this prompt into an LLM to provide it with context about your project 🦾
 
 ## Config File 📋
```

### Comparing `dir2prompt-1.0.3/README.md` & `dir2prompt-1.0.4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -18,14 +18,22 @@
 To generate a prompt from a directory, use the `d2p` command followed by the desired options:
 
 ```sh
 d2p --dir [directory path] --filters [file extensions] --outpath [output path] --outfile [output file name] --ignore-dir [directories to ignore] --ignore-file [files to ignore] --config [path to config file]
 
 ```
 
+For ease of use, you can select a directory by passing it in as a positional argument
+
+```sh
+d2p [directory path]
+```
+
+If both the positional argument and the `--dir` flag are provided, the `--dir` flag takes priority.
+
 ## Options ⚙️
 
 `--dir`: The directory to generate the prompt for (default: current directory).
 
 `--filters`: File extensions to include in the prompt (default: all files).
 
 `--outpath`: The output path for the prompt file (default: current directory).
@@ -39,35 +47,36 @@
 `--config`: Path to a custom config file (default: `config.json` in the package directory).
 
 ## Example 🌟
 
 Here's an example of how to use `dir2prompt` to generate a prompt:
 
 ```sh
-d2p --dir /path/<dir_name> --filters .py .txt --ignore-dir experiments __pycache__ --ignore-file old.py
+d2p --dir /path/<dir_name> --filters .py .txt .md .ipynb --ignore-dir experiments __pycache__ --ignore-file old.py
 ```
 
-This command will generate a prompt for the specified directory, including only files with the extensions `.py` and `.txt`, ignoring the `experiments` and `__pycache__` directories, and ignoring the `old.py` file. 
+This command will generate a prompt for the specified directory, including only files with the extensions `.py`, `.txt`, `.md`, `.ipynb`, ignoring the `experiments` and `__pycache__` directories, and ignoring the `old.py` file. 
 
-Note that ignored directories are not included in the directory tree, but that ignored files are. However, the content of the ignored files will not be written to the final prompt under the `<files>` tag.
+Note that ignored directories are not included in the directory tree, but that ignored files are. However, the content of the ignored files will not be written to the final prompt under the `<files>` tag. This might be changed later...
 
 In this example, the generated prompt will be saved as a `.txt` file in the directory that `d2p` is called in with the name `<dir_name>_prompt.txt`, and will have the following structure:
 
 **<dir_name>_prompt.txt**
 ```xml
 <context>
 <directory_tree>
 project/
 ├── README.md
-├── experiments/
 ├── requirements.txt
 └── src/
     ├── __init__.py
     ├── main.py
-    └── old.py
+    ├── old.py
+    ├── production.ipynb
+    └── testing.rs
 </directory_tree>
 
 <files>
 
 <file>
 <path>README.md</path>
 <content>
@@ -102,14 +111,32 @@
     print("Hello, World!")
 
 if __name__ == "__main__":
     main()
 </content>
 </file>
 
+<file>
+<path>src/production.ipynb</path>
+<content>
+---------- Cell 1 (markdown) ----------
+### Biologically inspired artificial neuron 
+
+$$
+y = mx + b
+$$
+
+---------- Cell 2 (code) ----------
+def neuron(x, m, b):
+    return m * x + b
+
+
+</content>
+</file>
+
 </files>
 </context>
 ```
 
 You can then feed this prompt into an LLM to provide it with context about your project 🦾
 
 ## Config File 📋
```

### Comparing `dir2prompt-1.0.3/dir2prompt.egg-info/PKG-INFO` & `dir2prompt-1.0.4/dir2prompt.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dir2prompt
-Version: 1.0.3
+Version: 1.0.4
 Summary: Generate prompts for long-context LLMs using the content in your directory
 Home-page: https://github.com/mkieffer1107/dir2prompt
 Author: Max Kieffer
 Author-email: Max Kieffer <wkieffer@ufl.edu>
 License: MIT License
         
         Copyright (c) 2024 mkieffer1107
@@ -62,14 +62,22 @@
 To generate a prompt from a directory, use the `d2p` command followed by the desired options:
 
 ```sh
 d2p --dir [directory path] --filters [file extensions] --outpath [output path] --outfile [output file name] --ignore-dir [directories to ignore] --ignore-file [files to ignore] --config [path to config file]
 
 ```
 
+For ease of use, you can select a directory by passing it in as a positional argument
+
+```sh
+d2p [directory path]
+```
+
+If both the positional argument and the `--dir` flag are provided, the `--dir` flag takes priority.
+
 ## Options ⚙️
 
 `--dir`: The directory to generate the prompt for (default: current directory).
 
 `--filters`: File extensions to include in the prompt (default: all files).
 
 `--outpath`: The output path for the prompt file (default: current directory).
@@ -83,35 +91,36 @@
 `--config`: Path to a custom config file (default: `config.json` in the package directory).
 
 ## Example 🌟
 
 Here's an example of how to use `dir2prompt` to generate a prompt:
 
 ```sh
-d2p --dir /path/<dir_name> --filters .py .txt --ignore-dir experiments __pycache__ --ignore-file old.py
+d2p --dir /path/<dir_name> --filters .py .txt .md .ipynb --ignore-dir experiments __pycache__ --ignore-file old.py
 ```
 
-This command will generate a prompt for the specified directory, including only files with the extensions `.py` and `.txt`, ignoring the `experiments` and `__pycache__` directories, and ignoring the `old.py` file. 
+This command will generate a prompt for the specified directory, including only files with the extensions `.py`, `.txt`, `.md`, `.ipynb`, ignoring the `experiments` and `__pycache__` directories, and ignoring the `old.py` file. 
 
-Note that ignored directories are not included in the directory tree, but that ignored files are. However, the content of the ignored files will not be written to the final prompt under the `<files>` tag.
+Note that ignored directories are not included in the directory tree, but that ignored files are. However, the content of the ignored files will not be written to the final prompt under the `<files>` tag. This might be changed later...
 
 In this example, the generated prompt will be saved as a `.txt` file in the directory that `d2p` is called in with the name `<dir_name>_prompt.txt`, and will have the following structure:
 
 **<dir_name>_prompt.txt**
 ```xml
 <context>
 <directory_tree>
 project/
 ├── README.md
-├── experiments/
 ├── requirements.txt
 └── src/
     ├── __init__.py
     ├── main.py
-    └── old.py
+    ├── old.py
+    ├── production.ipynb
+    └── testing.rs
 </directory_tree>
 
 <files>
 
 <file>
 <path>README.md</path>
 <content>
@@ -146,14 +155,32 @@
     print("Hello, World!")
 
 if __name__ == "__main__":
     main()
 </content>
 </file>
 
+<file>
+<path>src/production.ipynb</path>
+<content>
+---------- Cell 1 (markdown) ----------
+### Biologically inspired artificial neuron 
+
+$$
+y = mx + b
+$$
+
+---------- Cell 2 (code) ----------
+def neuron(x, m, b):
+    return m * x + b
+
+
+</content>
+</file>
+
 </files>
 </context>
 ```
 
 You can then feed this prompt into an LLM to provide it with context about your project 🦾
 
 ## Config File 📋
```

### Comparing `dir2prompt-1.0.3/pyproject.toml` & `dir2prompt-1.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dir2prompt"
-version = "1.0.3"
+version = "1.0.4"
 license = {file = "LICENSE"}
 authors = [
   { name="Max Kieffer", email="wkieffer@ufl.edu" },
 ]
 description = "Generate prompts for long-context LLMs using the content in your directory"
 readme = "README.md"
 requires-python = ">=3.6"
```

### Comparing `dir2prompt-1.0.3/setup.py` & `dir2prompt-1.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `dir2prompt-1.0.3/src/config.json` & `dir2prompt-1.0.4/src/config.json`

 * *Files identical despite different names*

### Comparing `dir2prompt-1.0.3/src/d2p.py` & `dir2prompt-1.0.4/src/d2p.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,14 +40,16 @@
             prefix = "├── " 
 
         # when printing contents nested in child dirs, we need to make sure to print the
         # vertical bars to the left of these contents that connect the contents of the parent dir
         if level > 0:
             tree_str += "│   " * (level - 1)
             tree_str += "│   "
+        # print(f"{'│   ' * level}{item} ({level})")
+
 
         # now add the item to the tree string and move to the next line for the next item
         if os.path.isdir(item_path):
             item += "/"
         tree_str += prefix + item + "\n"
 
         if os.path.isdir(item_path):
@@ -94,19 +96,20 @@
     prompt = f"<context>\n"
     prompt += f"<directory_tree>\n{tree_str}</directory_tree>\n\n"
 
     prompt += "<files>\n\n"
     for file in file_paths:
         # read only filtered files, if specified
         if filters is None or any(file.endswith(ext) for ext in filters):
+            filepath = os.path.join(dir, file)
             try:
                 if file.endswith(".ipynb"):
-                    file_content = read_notebook(file)
+                    file_content = read_notebook(filepath)
                 else:
-                    with open(os.path.join(dir, file), "r") as f:
+                    with open(filepath, "r") as f:
                         file_content = f.read()
 
                 # add file string to prompt
                 prompt += f"<file>\n"
                 prompt += f"<path>{file}</path>\n"
                 if not file_content.strip():
                     file_content = "EMPTY FILE"
@@ -135,23 +138,32 @@
     path = os.path.join(outpath, f"{outfile}.txt")
     with open(path, "w") as f:
         f.write(contents)
 
 
 def parse_options():
     parser = argparse.ArgumentParser(description="Generate a prompt for a directory")
-    parser.add_argument("--dir", type=str, default=".", help="Directory to generate prompt for")
+    parser.add_argument("pos_dir", type=str, default=".", nargs="?", help="Directory to generate prompt for (positional argument)")
+    parser.add_argument("--dir", type=str, help="Directory to generate prompt for (optional flag)")
     parser.add_argument("--filters", type=str, nargs="+", help="File extensions to filter for")
     parser.add_argument("--outpath", type=str, default=".", help="Output path for prompt file")
     parser.add_argument("--outfile", type=str, help="Output file name for prompt file (default: <dir>_prompt)")
     parser.add_argument("--ignore-dir", type=str, nargs="+", help="Additional directories to ignore: specify directory names (e.g., .git, __pycache__, etc.)")
     parser.add_argument("--ignore-file", type=str, nargs="+", help="Additional file types to ignore: specify extensions with or without dot (e.g., py, ipynb, .c, etc.)")
     parser.add_argument("--config", type=str, help="Path to the custom configuration file (default: config.json)")
     args = parser.parse_args()
 
+    # prioritize --dir flag over positional argument -- args.dir will be None if flag not invoked
+    # but pos_dir will always at least be the default value of "."
+    args.dir = args.dir or args.pos_dir
+
+    # remove "/" from beginning and end of dir path so that we can work with the name alone
+    if args.dir.startswith("/"): args.dir = args.dir[1:]
+    if args.dir.endswith("/"): args.dir = args.dir[:-1]
+
     # set the outfile name
     if args.outfile is None:
         if args.dir == ".":
             # replace "." with the actual base directory name
             dir_name = os.path.basename(os.getcwd()) 
         else:
             dir_name = os.path.basename(args.dir)
@@ -162,19 +174,15 @@
         args.config = str(files("src").joinpath("config.json"))
     return args
 
 
 def main():
     args = parse_options()
 
-    try:
-        config = load_config(args.config)
-    except Exception as e:
-        raise Exception(f"Config file not found: {args.config}") from e
-
+    config = load_config(args.config)
     IGNORE_DIRS = config["IGNORE_DIRS"]
     IGNORE_FILES = config["IGNORE_FILES"]
 
     # extend the default ignore lists with cli args
     if args.ignore_dir:
         IGNORE_DIRS.extend(args.ignore_dir)
     if args.ignore_file:
```

