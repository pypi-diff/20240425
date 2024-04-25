# Comparing `tmp/tamp-1.3.1.tar.gz` & `tmp/tamp-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tamp-1.3.1.tar", max compression
+gzip compressed data, was "tamp-1.4.0.tar", max compression
```

## Comparing `tamp-1.3.1.tar` & `tamp-1.4.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    11357 2024-01-15 16:54:12.790141 tamp-1.3.1/LICENSE
--rw-r--r--   0        0        0    17787 2024-01-15 16:54:12.790141 tamp-1.3.1/README.rst
--rw-r--r--   0        0        0     3051 2024-01-15 16:54:12.790141 tamp-1.3.1/build.py
--rw-r--r--   0        0        0     5890 2024-01-15 16:54:33.986014 tamp-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     2788 2024-01-15 16:54:33.986014 tamp-1.3.1/tamp/__init__.py
--rw-r--r--   0        0        0     1625 2024-01-15 16:54:12.794141 tamp-1.3.1/tamp/__init__.pyi
--rw-r--r--   0        0        0       57 2024-01-15 16:54:12.794141 tamp-1.3.1/tamp/__main__.py
--rw-r--r--   0        0        0       65 2024-01-15 16:54:12.794141 tamp-1.3.1/tamp/_c_common.pxd
--rw-r--r--   0        0        0      343 2024-01-15 16:54:12.794141 tamp-1.3.1/tamp/_c_common.pyx
--rw-r--r--   0        0        0     4498 2024-01-15 16:54:12.794141 tamp-1.3.1/tamp/_c_compressor.pyx
--rw-r--r--   0        0        0     4168 2024-01-15 16:54:12.794141 tamp-1.3.1/tamp/_c_decompressor.pyx
--rw-r--r--   0        0        0      829 2024-01-15 16:54:12.794141 tamp-1.3.1/tamp/_c_src/tamp/common.c
--rw-r--r--   0        0        0     1791 2024-01-15 16:54:12.794141 tamp-1.3.1/tamp/_c_src/tamp/common.h
--rw-r--r--   0        0        0    12165 2024-01-15 16:54:12.794141 tamp-1.3.1/tamp/_c_src/tamp/compressor.c
--rw-r--r--   0        0        0     6884 2024-01-15 16:54:12.794141 tamp-1.3.1/tamp/_c_src/tamp/compressor.h
--rw-r--r--   0        0        0     9378 2024-01-15 16:54:12.794141 tamp-1.3.1/tamp/_c_src/tamp/decompressor.c
--rw-r--r--   0        0        0     4098 2024-01-15 16:54:12.794141 tamp-1.3.1/tamp/_c_src/tamp/decompressor.h
--rw-r--r--   0        0        0        0 2024-01-15 16:54:12.794141 tamp-1.3.1/tamp/cli/__init__.py
--rw-r--r--   0        0        0     2266 2024-01-15 16:54:12.794141 tamp-1.3.1/tamp/cli/main.py
--rw-r--r--   0        0        0     8656 2024-01-15 16:54:12.794141 tamp-1.3.1/tamp/compressor.py
--rw-r--r--   0        0        0     6871 2024-01-15 16:54:12.794141 tamp-1.3.1/tamp/compressor_viper.py
--rw-r--r--   0        0        0     2802 2024-01-15 16:54:12.794141 tamp-1.3.1/tamp/ctamp.pxd
--rw-r--r--   0        0        0     7882 2024-01-15 16:54:12.794141 tamp-1.3.1/tamp/decompressor.py
--rw-r--r--   0        0        0     7408 2024-01-15 16:54:12.794141 tamp-1.3.1/tamp/decompressor_viper.py
--rw-r--r--   0        0        0        0 2024-01-15 16:54:12.794141 tamp-1.3.1/tamp/py.typed
--rw-r--r--   0        0        0    18496 1970-01-01 00:00:00.000000 tamp-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-25 03:32:47.549439 tamp-1.4.0/LICENSE
+-rw-r--r--   0        0        0    18981 2024-04-25 03:32:47.549439 tamp-1.4.0/README.rst
+-rw-r--r--   0        0        0     3051 2024-04-25 03:32:47.553439 tamp-1.4.0/build.py
+-rw-r--r--   0        0        0     6089 2024-04-25 03:33:05.917614 tamp-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2306 2024-04-25 03:33:05.917614 tamp-1.4.0/tamp/__init__.py
+-rw-r--r--   0        0        0     1625 2024-04-25 03:32:47.557439 tamp-1.4.0/tamp/__init__.pyi
+-rw-r--r--   0        0        0       57 2024-04-25 03:32:47.557439 tamp-1.4.0/tamp/__main__.py
+-rw-r--r--   0        0        0       65 2024-04-25 03:32:47.557439 tamp-1.4.0/tamp/_c_common.pxd
+-rw-r--r--   0        0        0      343 2024-04-25 03:32:47.557439 tamp-1.4.0/tamp/_c_common.pyx
+-rw-r--r--   0        0        0     4451 2024-04-25 03:32:47.557439 tamp-1.4.0/tamp/_c_compressor.pyx
+-rw-r--r--   0        0        0     4739 2024-04-25 03:32:47.557439 tamp-1.4.0/tamp/_c_decompressor.pyx
+-rw-r--r--   0        0        0      892 2024-04-25 03:32:47.557439 tamp-1.4.0/tamp/_c_src/tamp/common.c
+-rw-r--r--   0        0        0     1791 2024-04-25 03:32:47.557439 tamp-1.4.0/tamp/_c_src/tamp/common.h
+-rw-r--r--   0        0        0    12165 2024-04-25 03:32:47.557439 tamp-1.4.0/tamp/_c_src/tamp/compressor.c
+-rw-r--r--   0        0        0     6884 2024-04-25 03:32:47.557439 tamp-1.4.0/tamp/_c_src/tamp/compressor.h
+-rw-r--r--   0        0        0     9734 2024-04-25 03:32:47.557439 tamp-1.4.0/tamp/_c_src/tamp/decompressor.c
+-rw-r--r--   0        0        0     4098 2024-04-25 03:32:47.557439 tamp-1.4.0/tamp/_c_src/tamp/decompressor.h
+-rw-r--r--   0        0        0        0 2024-04-25 03:32:47.557439 tamp-1.4.0/tamp/cli/__init__.py
+-rw-r--r--   0        0        0     2266 2024-04-25 03:32:47.557439 tamp-1.4.0/tamp/cli/main.py
+-rw-r--r--   0        0        0    10867 2024-04-25 03:32:47.557439 tamp-1.4.0/tamp/compressor.py
+-rw-r--r--   0        0        0     6871 2024-04-25 03:32:47.557439 tamp-1.4.0/tamp/compressor_viper.py
+-rw-r--r--   0        0        0     2802 2024-04-25 03:32:47.557439 tamp-1.4.0/tamp/ctamp.pxd
+-rw-r--r--   0        0        0    10206 2024-04-25 03:32:47.557439 tamp-1.4.0/tamp/decompressor.py
+-rw-r--r--   0        0        0     7320 2024-04-25 03:32:47.557439 tamp-1.4.0/tamp/decompressor_viper.py
+-rw-r--r--   0        0        0        0 2024-04-25 03:32:47.557439 tamp-1.4.0/tamp/py.typed
+-rw-r--r--   0        0        0    19690 1970-01-01 00:00:00.000000 tamp-1.4.0/PKG-INFO
```

### Comparing `tamp-1.3.1/LICENSE` & `tamp-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tamp-1.3.1/README.rst` & `tamp-1.4.0/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -8,32 +8,50 @@
 |Python compat| |PyPi| |GHA tests| |Codecov report| |readthedocs|
 
 .. inclusion-marker-do-not-remove
 
 Tamp
 ====
 
-Tamp is a low-memory, DEFLATE-inspired lossless compression library.
+Tamp is a low-memory, DEFLATE-inspired lossless compression library intended for embedded targets.
+
+Tamp delivers the highest data compression ratios, while using the least amount of RAM and firmware storage.
+
+
+**Documentation:** https://tamp.readthedocs.io/en/latest/
+
+**Source Code:** https://github.com/BrianPugh/tamp
+
 
 Features
 ========
 
-* Various implementations available:
+* Various language implementations available:
+
+  * Pure Python reference:
+
+    * ``tamp/__init__.py``, ``tamp/compressor.py``, ``tamp/decompressor.py``
 
-  * Pure Python:
+    * ``pip install tamp`` will use a python-bound C implementation optimized for speed.
 
-    * ``tamp/compressor.py``, ``tamp/decompressor.py``
+  * Micropython:
 
-    * When available, Tamp will use a python-bound C implementation for speed.
+    * Native Module (suggested micropython implementation).
+
+      * ``mpy_bindings/``
+
+    * Viper.
+
+      * ``tamp/__init__.py``, ``tamp/compressor_viper.py``, ``tamp/decompressor_viper.py``
 
   * C library:
 
     * ``tamp/_c_src/``
 
-* High compression ratios and low memory use.
+* High compression ratios, low memory use, and fast.
 
 * Compact compression and decompression implementations.
 
   * Compiled C library is <4KB (compressor + decompressor).
 
 * Mid-stream flushing.
 
@@ -41,32 +59,58 @@
 
 * Customizable dictionary for greater compression of small messages.
 
 * Convenient CLI interface.
 
 Installation
 ============
-Tamp contains 3 implementations:
+Tamp contains 4 implementations:
+
+1. A reference desktop CPython implementation that is optimized for readability (and **not** speed).
 
-1. A desktop Cpython implementation that is optimized for readability
+2. A Micropython Native Module implementation (fast).
 
-2. A micropython viper implementation that is optimized for runtime performance.
+3. A Micropython Viper implementation (not recommended, please use Native Module).
 
-3. A C implementation (with python bindings) for accelerated desktop use and to be used in C projects.
+4. A C implementation (with python bindings) for accelerated desktop use and to be used in C projects (very fast).
+
+This section instructs how to install each implementation.
 
 Desktop Python
 ^^^^^^^^^^^^^^
 The Tamp library and CLI requires Python ``>=3.8`` and can be installed via:
 
 .. code-block:: bash
 
    pip install tamp
 
 MicroPython
 ^^^^^^^^^^^
+
+MicroPython Native Module
+-------------------------
+Tamp provides pre-compiled `native modules` that are easy to install, are small, and are incredibly fast.
+
+Download the appropriate ``.mpy`` file from the `release page`_.
+
+   * Match the micropython version.
+
+   * Match the architecture to the microcontroller (e.g. ``armv6m`` for a pi pico).
+
+Rename the file to ``tamp.mpy`` and transfer it to your board. If using `Belay`_, tamp can be installed by adding the following to ``pyproject.toml``.
+
+.. code-block:: toml
+
+   [tool.belay.dependencies]
+   tamp = "https://github.com/BrianPugh/tamp/releases/download/v1.4.0/tamp-1.4.0-mpy1.22-armv6m.mpy"
+
+MicroPython Viper
+-----------------
+**NOT RECOMMENDED, PLEASE USE NATIVE MODULE**
+
 For micropython use, there are 3 main files:
 
 1. ``tamp/__init__.py`` - Always required.
 
 2. ``tamp/decompressor_viper.py`` - Required for on-device decompression.
 
 3. ``tamp/compressor_viper.py`` - Required for on-device compression.
@@ -112,34 +156,24 @@
 Use ``tamp compress`` to compress a file or stream.
 If no input file is specified, data from stdin will be read.
 If no output is specified, the compressed output stream will be written to stdout.
 
 .. code-block:: bash
 
    $ tamp compress --help
+   Usage: tamp compress [ARGS] [OPTIONS]
 
-    Usage: tamp compress [OPTIONS] [INPUT_PATH]
-
-    Compress an input file or stream.
-
-   ╭─ Arguments ────────────────────────────────────────────────────────────────────────╮
-   │   input_path      [INPUT_PATH]  Input file to compress or decompress. Defaults to  │
-   │                                 stdin.                                             │
-   ╰────────────────────────────────────────────────────────────────────────────────────╯
-   ╭─ Options ──────────────────────────────────────────────────────────────────────────╮
-   │ --output   -o      PATH                      Output file. Defaults to stdout.      │
-   │ --window   -w      INTEGER RANGE [8<=x<=15]  Number of bits used to represent the  │
-   │                                              dictionary window.                    │
-   │                                              [default: 10]                         │
-   │ --literal  -l      INTEGER RANGE [5<=x<=8]   Number of bits used to represent a    │
-   │                                              literal.                              │
-   │                                              [default: 8]                          │
-   │ --help                                       Show this message and exit.           │
-   ╰────────────────────────────────────────────────────────────────────────────────────╯
+   Compress an input file or stream.
 
+   ╭─ Parameters ───────────────────────────────────────────────────────────────────────────────╮
+   │ INPUT,--input    -i  Input file to compress. Defaults to stdin.                            │
+   │ OUTPUT,--output  -o  Output compressed file. Defaults to stdout.                           │
+   │ --window         -w  Number of bits used to represent the dictionary window. [default: 10] │
+   │ --literal        -l  Number of bits used to represent a literal. [default: 8]              │
+   ╰────────────────────────────────────────────────────────────────────────────────────────────╯
 
 Example usage:
 
 .. code-block:: bash
 
    tamp compress enwik8 -o enwik8.tamp  # Compress a file
    echo "hello world" | tamp compress | wc -c  # Compress a stream and print the compressed size.
@@ -160,27 +194,23 @@
 -------------
 Use ``tamp decompress`` to decompress a file or stream.
 If no input file is specified, data from stdin will be read.
 If no output is specified, the compressed output stream will be written to stdout.
 
 .. code-block:: bash
 
-  $ tamp decompress --help
-
-  Usage: tamp decompress [OPTIONS] [INPUT_PATH]
+   $ tamp decompress --help
+   Usage: tamp decompress [ARGS] [OPTIONS]
 
-  Decompress an input file or stream.
+   Decompress an input file or stream.
 
- ╭─ Arguments ────────────────────────────────────────────────────────────────────────╮
- │   input_path      [INPUT_PATH]  Input file. If not provided, reads from stdin.     │
- ╰────────────────────────────────────────────────────────────────────────────────────╯
- ╭─ Options ──────────────────────────────────────────────────────────────────────────╮
- │ --output  -o      PATH  Output file. Defaults to stdout.                           │
- │ --help                  Show this message and exit.                                │
- ╰────────────────────────────────────────────────────────────────────────────────────╯
+   ╭─ Parameters ───────────────────────────────────────────────────────────────────────────────╮
+   │ INPUT,--input    -i  Input file to decompress. Defaults to stdin.                          │
+   │ OUTPUT,--output  -o  Output decompressed file. Defaults to stdout.                         │
+   ╰────────────────────────────────────────────────────────────────────────────────────────────╯
 
 Example usage:
 
 .. code-block:: bash
 
    tamp decompress enwik8.tamp -o enwik8
    echo "hello world" | tamp compress | tamp decompress
@@ -264,71 +294,77 @@
 memory during both compression and decompression (see next section). Tamp accomplishes
 competitive performance while using around 10x less memory.
 
 Memory Usage
 ^^^^^^^^^^^^
 The following table shows approximately how much memory each algorithm uses during compression and decompression.
 
-+---------------+-------------------+------------------------------+-------------------+
-| Action        | tamp              | zlib                         | heatshrink        |
-+===============+===================+==============================+===================+
-| Compression   | (1 << windowBits) | (1 << (windowBits+2)) + 7 KB | (1 << windowBits) |
-+---------------+-------------------+------------------------------+-------------------+
-| Decompression | (1 << windowBits) | (1 << windowBits) + 7 KB     | (1 << windowBits) |
-+---------------+-------------------+------------------------------+-------------------+
++---------------+-------------------+------------------------------+-------------------------+-----------------------+
+| Action        | tamp              | zlib                         | heatshrink              | deflate (micropython) |
++===============+===================+==============================+=========================+=======================+
+| Compression   | (1 << windowBits) | (1 << (windowBits+2)) + 7 KB | (1 << (windowBits + 1)) | (1 << windowBits)     |
++---------------+-------------------+------------------------------+-------------------------+-----------------------+
+| Decompression | (1 << windowBits) | (1 << windowBits) + 7 KB     | (1 << (windowBits + 1)) | (1 << windowBits)     |
++---------------+-------------------+------------------------------+-------------------------+-----------------------+
 
-Both tamp and heatshrink have a few dozen bytes of overhead in addition to the primary window buffer, but are implementation-specific and ignored for clarity here.
+All libraries have a few dozen bytes of overhead in addition to the primary window buffer, but are implementation-specific and ignored for clarity here.
+Tamp uses significantly less memory than ZLib, and half the memory of Heatshrink.
 
 Runtime
 ^^^^^^^
 As a rough benchmark, here is the performance (in seconds) of these different compression algorithms on the 100MB enwik8 dataset.
 These tests were performed on an M1 Macbook Air.
 
 +---------------+--------------------+-------+------+--------------+-----------------+
 | Action        | tamp               | tamp  | zlib | heatshrink   | heatshrink      |
 |               | (Python Reference) | (C)   |      | (with index) | (without index) |
 +===============+====================+=======+======+==============+=================+
 | Compression   | 109.5              | 16.45 | 4.84 | 6.22         | 41.729          |
 +---------------+--------------------+-------+------+--------------+-----------------+
-| Decompression | 54.0               | 0.70  | 0.98 | 0.82         | 0.82            |
+| Decompression | 76.0               | 0.142 | 0.98 | 0.82         | 0.82            |
 +---------------+--------------------+-------+------+--------------+-----------------+
 
 Heatshrink v0.4.1 was used in these benchmarks.
-When heathshrink uses an index, an additional ``(1 << (windowBits + 1))`` bytes of memory are used, tripling the memory requirement.
+When heathshrink uses an index, an additional ``(1 << (windowBits + 1))`` bytes of memory are used, resulting in 4x more memory-usage than Tamp.
 Tamp could use a similar indexing to increase compression speed, but has chosen not to to focus on the primary goal of a low-memory compressor.
 
 To give an idea of Tamp's speed on an embedded device, the following table shows compression/decompression in **bytes/second of the first 100KB of enwik8 on a pi pico (rp2040)** at the default 125MHz clock rate.
-This isn't exactly an apples-to-apples comparison because the C benchmark does not use a filesystem (and thusly, reduced overhead) nor dynamic memory allocation, but is good enough to get the idea across.
+The C benchmark **does not** use a filesystem nor dynamic memory allocation, so it represents the maximum speed Tamp can achieve.
+In all tests, a 1KB window (10 bit) was used.
+
++---------------+---------------------+-----------------------------+------------+-----------------------+
+| Action        | tamp                | tamp                        | tamp       | deflate.DeflatIO      |
+|               | (Micropython Viper) | (Micropython Native Module) | (C)        | (micropython builtin) |
++===============+=====================+=============================+============+=======================+
+| Compression   | ~4,300              | ~12,770                     | ~28,500    | ~6,715                |
++---------------+---------------------+-----------------------------+------------+-----------------------+
+| Decompression | ~42,000             | ~644,010                    | ~1,042,524 | ~146,477              |
++---------------+---------------------+-----------------------------+------------+-----------------------+
 
-+---------------+---------------------+------------+
-| Action        | tamp                | tamp       |
-|               | (Micropython Viper) | (C)        |
-+===============+=====================+============+
-| Compression   | ~4,300              | ~28,500    |
-+---------------+---------------------+------------+
-| Decompression | ~42,000             | ~1,042,524 |
-+---------------+---------------------+------------+
+Tamp resulted in a **51637** byte archive, while Micropython's builtin ``deflate`` resulted in a larger **59442** byte archive.
 
 Binary Size
 ^^^^^^^^^^^
 To give an idea on the resulting binary sizes, Tamp and other libraries were compiled for the Pi Pico (``armv6m``).
 All libraries were compiled with ``-O3``.
 Numbers reported in bytes.
 
-+--------------------+------------+--------------+---------------------------+
-| Library            | Compressor | Decompressor | Compressor + Decompressor |
-+====================+============+==============+===========================+
-| Tamp (micropython) | 4429       | 4205         | 7554                      |
-+--------------------+------------+--------------+---------------------------+
-| Tamp (C)           | 2008       | 1972         | 3864                      |
-+--------------------+------------+--------------+---------------------------+
-| Heatshrink         | 2956       | 3876         | 6832                      |
-+--------------------+------------+--------------+---------------------------+
-| uzlib              | 2355       | 3963         | 6318                      |
-+--------------------+------------+--------------+---------------------------+
++----------------------------------+------------+--------------+---------------------------+
+| Library                          | Compressor | Decompressor | Compressor + Decompressor |
++==================================+============+==============+===========================+
+| Tamp (micropython viper)         | 4429       | 4205         | 7554                      |
++----------------------------------+------------+--------------+---------------------------+
+| Tamp (micropython native module) | 3264       | 3079         | 5537                      |
++----------------------------------+------------+--------------+---------------------------+
+| Tamp (C)                         | 2008       | 1972         | 3864                      |
++----------------------------------+------------+--------------+---------------------------+
+| Heatshrink                       | 2956       | 3876         | 6832                      |
++----------------------------------+------------+--------------+---------------------------+
+| uzlib                            | 2355       | 3963         | 6318                      |
++----------------------------------+------------+--------------+---------------------------+
 
 Heatshrink doesn't include a high level API; in an apples-to-apples comparison the Tamp library would be even smaller.
 
 
 .. |GHA tests| image:: https://github.com/BrianPugh/tamp/workflows/tests/badge.svg
    :target: https://github.com/BrianPugh/tamp/actions?query=workflow%3Atests
    :alt: GHA Status
@@ -344,7 +380,9 @@
 .. _Belay: https://github.com/BrianPugh/belay
 .. _zlib:  https://docs.python.org/3/library/zlib.html
 .. _heatshrink: https://github.com/atomicobject/heatshrink
 .. _Silesia Corpus: https://sun.aei.polsl.pl//~sdeor/index.php?page=silesia
 .. _Enwik8: https://mattmahoney.net/dc/textdata.html
 .. _mip: https://docs.micropython.org/en/latest/reference/packages.html#installing-packages-with-mip
 .. _the documentation: https://tamp.readthedocs.io/en/latest/c_library.html
+.. _native modules: https://docs.micropython.org/en/latest/develop/natmod.html
+.. _release page: https://github.com/BrianPugh/tamp/releases
```

### Comparing `tamp-1.3.1/build.py` & `tamp-1.4.0/build.py`

 * *Files identical despite different names*

### Comparing `tamp-1.3.1/pyproject.toml` & `tamp-1.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -5,24 +5,30 @@
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 style = "semver"
 
 [tool.poetry]
 name = "tamp"
-version = "1.3.1"  # Do not change, let poetry-dynamic-versioning handle it.
+version = "1.4.0"  # Do not change, let poetry-dynamic-versioning handle it.
 homepage = "https://github.com/BrianPugh/tamp"
 repository = "https://github.com/BrianPugh/tamp"
 license = "Apache-2.0"
 description = ""
 authors = ["Brian Pugh"]
 readme = "README.rst"
 packages = [{include = "tamp"}]
 include = ["tamp/*.so", "tamp/*.dll", "tamp/*.pyd"]
 
+[tool.poetry-dynamic-versioning.substitution]
+files = [
+    "tamp/__init__.py",
+    "mpy_bindings/bindings_common.py"
+]
+
 [tool.poetry.build]
 generate-setup-file = false
 script = 'build.py'
 
 [tool.poetry.scripts]
 tamp = "tamp.cli.main:run_app"
 
@@ -52,14 +58,15 @@
 mpremote = ">=1.20.0"
 cython = ">=0.29.34"
 pytest-subtests = ">=0.10.0"
 numpy = [
     {version = ">=1.24", python = ">=3.8,<3.12"},
     {version = ">=1.26", python = ">=3.12"}
 ]
+pyelftools = "^0.29"
 
 [tool.poetry.group.profile]
 optional = true
 
 [tool.poetry.group.profile.dependencies]
 line-profiler = "<4.0.0"
 
@@ -195,14 +202,17 @@
     "typer.Option",
 ]
 
 [tool.ruff.pydocstyle]
 convention = "numpy"
 
 [tool.ruff.per-file-ignores]
+"mpy_bindings/*.py" = [
+    "F821",  # Undefined names
+]
 "tamp/*_viper.py" = [
     "F821",  # Undefined names (e.g. `ptr8`)
 ]
 "tests/*.py" = [
     "D100",
     "D101",
     "D102",
```

### Comparing `tamp-1.3.1/tamp/__init__.py` & `tamp-1.4.0/tamp/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-# Don't manually change, let poetry-dynamic-versioning-plugin handle it.
-__version__ = "1.3.1"
+__version__ = "1.4.0"
 
 
 class ExcessBitsError(Exception):
     """Provided data has more bits than expected ``literal`` bits."""
 
 
 def bit_size(value):
@@ -18,49 +17,39 @@
     while True:
         seed ^= (seed << 13) & 0xFFFFFFFF
         seed ^= (seed >> 17) & 0xFFFFFFFF
         seed ^= (seed << 5) & 0xFFFFFFFF
         yield seed
 
 
-def initialize_dictionary(size, seed=None):
+def initialize_dictionary(source, seed=None):
     if seed is None:
         seed = 3758097560
     elif seed == 0:
-        return bytearray(size)
+        return bytearray(source)
+
+    out = source if isinstance(source, bytearray) else bytearray(source)
+    size = len(out)
 
     chars = b" \x000ei>to<ans\nr/."  # 16 most common chars in dataset
 
     def _gen_stream(xorshift32):
         for _ in range(size >> 3):
             value = next(xorshift32)
             for _ in range(8):
                 yield chars[value & 0x0F]
                 value >>= 4
 
-    return bytearray(_gen_stream(_xorshift32(seed)))
+    for i, c in enumerate(_gen_stream(_xorshift32(seed))):
+        out[i] = c
+
+    return out
 
 
 def compute_min_pattern_size(window, literal):
-    """Compute whether the minimum pattern length should be 2 or 3."""
-    """
-    # Easy to understand version; commented out for smaller optimized version;
-    if window > 15 or window < 8:
-        raise ValueError
-    if literal == 5:
-        return 2 + (window > 10)
-    elif literal == 6:
-        return 2 + (window > 12)
-    elif literal == 7:
-        return 2 + (window > 14)
-    elif literal == 8:
-        return 2
-    else:
-        raise ValueError
-    """
     if not (7 < window < 16 and 4 < literal < 9):
         raise ValueError
 
     return 2 + (window > (10 + ((literal - 5) << 1)))
 
 
 try:
@@ -87,18 +76,12 @@
 
 
 def open(f, mode="rb", **kwargs):
     if "r" in mode and "w" in mode:
         raise ValueError
 
     if "r" in mode:  # Decompressor
-        if "b" in mode:
-            return Decompressor(f, **kwargs)
-        else:
-            return TextDecompressor(f, **kwargs)
+        return Decompressor(f, **kwargs) if "b" in mode else TextDecompressor(f, **kwargs)
     elif "w" in mode:  # Compressor
-        if "b" in mode:
-            return Compressor(f, **kwargs)
-        else:
-            return TextCompressor(f, **kwargs)
+        return Compressor(f, **kwargs) if "b" in mode else TextCompressor(f, **kwargs)
     else:
         raise ValueError
```

### Comparing `tamp-1.3.1/tamp/__init__.pyi` & `tamp-1.4.0/tamp/__init__.pyi`

 * *Files identical despite different names*

### Comparing `tamp-1.3.1/tamp/_c_compressor.pyx` & `tamp-1.4.0/tamp/_c_compressor.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -127,15 +127,14 @@
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
 
 
 class TextCompressor(Compressor):
-    """Compresses text to a file or stream."""
 
     def write(self, data: str) -> int:
         return super().write(data.encode())
 
 
 def compress(data: Union[bytes, str], *args, **kwargs) -> bytes:
     with BytesIO() as f:
```

### Comparing `tamp-1.3.1/tamp/_c_decompressor.pyx` & `tamp-1.4.0/tamp/_c_decompressor.pyx`

 * *Files 21% similar despite different names*

```diff
@@ -60,73 +60,87 @@
         self._window_buffer = dictionary if dictionary else bytearray(1 << conf.window)
         self._window_buffer_ptr = <unsigned char *>self._window_buffer
 
         res = ctamp.tamp_decompressor_init(self._c_decompressor, &conf, self._window_buffer_ptr)
         if res < 0:
             raise ERROR_LOOKUP.get(res, NotImplementedError)
 
-    def read(self, int size = -1) -> bytearray:
+    def readinto(self, bytearray buf) -> int:
         cdef:
-            bytearray output_buffer = bytearray(CHUNK_SIZE)
-            unsigned char *output_buffer_ptr = output_buffer
-
-            size_t input_chunk_consumed
-            size_t output_size
-            size_t output_written_size
-
-        if size < 0:
-            size = 0x7FFFFFFF
-
-        output_list = []
+            unsigned char *output_buffer_ptr = buf
+            size_t output_written_size, input_chunk_consumed
 
+        size = len(buf)
         while size:
             output_size = min(CHUNK_SIZE, size)
 
             res = ctamp.tamp_decompressor_decompress(
                 self._c_decompressor,
                 output_buffer_ptr,
                 output_size,
                 &output_written_size,
                 self.input_buffer_ptr + self.input_consumed,
                 self.input_size,
                 &input_chunk_consumed
             )
             self.input_size -= input_chunk_consumed
             self.input_consumed += input_chunk_consumed
+            output_buffer_ptr += output_written_size
             size -= output_written_size
 
-            output_list.append(output_buffer[:output_written_size])
-
             if res == ctamp.TAMP_INPUT_EXHAUSTED:
                 # Read in more data
                 self.input_size = self.f.readinto(self.input_buffer)
                 self.input_consumed = 0
                 if self.input_size == 0:
                     break;
+            elif res == ctamp.TAMP_OUTPUT_FULL:
+                break
             elif res < 0:
                 raise ERROR_LOOKUP.get(res, NotImplementedError)
 
             # Check signals for things like KeyboardInterrupt
             PyErr_CheckSignals()
 
-        return bytearray().join(output_list)
+        return len(buf) - size
+
+    def read(self, int size = -1) -> bytearray:
+        if size == 0:
+            return bytearray()
+
+        chunk_size = CHUNK_SIZE
+        out = []
+        while True:
+            buf = bytearray(chunk_size if size < 0 else size)
+            chunk_size <<= 1  # Keep allocating larger chunks as we go on.
+            read_size = self.readinto(buf)
+            if size > 0:
+                # Read the entire contents in one go.
+                out.append(buf)
+                break
+            else:
+                if read_size < len(buf):
+                    if read_size:
+                        out.append(buf[:read_size])
+                    break
+                else:
+                    out.append(buf)
+        return out[0] if len(out) == 1 else bytearray(b"".join(out))
 
     def close(self):
         if self._close_f_on_close:
             self.f.close()
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
 
 class TextDecompressor(Decompressor):
-    """Decompresses a file or stream of tamp-compressed data into text."""
-
     def read(self, *args, **kwargs) -> str:
         return super().read(*args, **kwargs).decode()
 
 
 def decompress(data: bytes, *args, **kwargs) -> bytearray:
     with BytesIO(data) as f:
         d = Decompressor(f, *args, **kwargs)
```

### Comparing `tamp-1.3.1/tamp/_c_src/tamp/common.c` & `tamp-1.4.0/tamp/_c_src/tamp/common.c`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     x ^= x << 5;
     *state = x;
     return x;
 }
 
 
 void tamp_initialize_dictionary(unsigned char *buffer, size_t size){
-    uint32_t seed = 3758097560;
+    uint32_t seed = 3758097560;  // This was experimentally discovered with tools/find_seed.py
     uint32_t randbuf = 0;
     for(size_t i=0; i < size; i++){
         if( TAMP_UNLIKELY((i & 0x7) == 0) )
             randbuf = xorshift32(&seed);
         buffer[i] = common_characters[randbuf & 0x0F];
         randbuf >>= 4;
     }
```

### Comparing `tamp-1.3.1/tamp/_c_src/tamp/common.h` & `tamp-1.4.0/tamp/_c_src/tamp/common.h`

 * *Files identical despite different names*

### Comparing `tamp-1.3.1/tamp/_c_src/tamp/compressor.c` & `tamp-1.4.0/tamp/_c_src/tamp/compressor.c`

 * *Files identical despite different names*

### Comparing `tamp-1.3.1/tamp/_c_src/tamp/compressor.h` & `tamp-1.4.0/tamp/_c_src/tamp/compressor.h`

 * *Files identical despite different names*

### Comparing `tamp-1.3.1/tamp/_c_src/tamp/decompressor.c` & `tamp-1.4.0/tamp/_c_src/tamp/decompressor.c`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,23 @@
 #include "common.h"
 
 #define MAX(x, y) (((x) > (y)) ? (x) : (y))
 #define MIN(x, y) (((x) < (y)) ? (x) : (y))
 
 #define FLUSH 15
 
+/**
+ * This array was generated with tools/huffman_jump_table.py
+ *
+ * The idea is that the resulting code is smaller/faster as a lookup table than a bunch of if/else statements.
+ *
+ * Of each element:
+ *  * The upper 4 bits express the number of bits to decode.
+ *  * The lower 4 bits express the decoded value, with FLUSH being represented as 0b1111
+ */
 static const uint8_t HUFFMAN_TABLE[128] = {50, 50, 50, 50, 50, 50, 50, 50, 50, 50, 50, 50, 50, 50, 50, 50, 85, 85, 85, 85, 122, 123, 104, 104, 86, 86, 86, 86, 93, 93, 93, 93, 68, 68, 68, 68, 68, 68, 68, 68, 105, 105, 124, 127, 87, 87, 87, 87, 51, 51, 51, 51, 51, 51, 51, 51, 51, 51, 51, 51, 51, 51, 51, 51, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17};
 
 
 /**
  * @brief Decode a huffman match-size symbol from the decompressor's bit_buffer.
  *
  * Internally updates bit_buffer and bit_buffer_pos.
```

### Comparing `tamp-1.3.1/tamp/_c_src/tamp/decompressor.h` & `tamp-1.4.0/tamp/_c_src/tamp/decompressor.h`

 * *Files identical despite different names*

### Comparing `tamp-1.3.1/tamp/cli/main.py` & `tamp-1.4.0/tamp/cli/main.py`

 * *Files identical despite different names*

### Comparing `tamp-1.3.1/tamp/compressor.py` & `tamp-1.4.0/tamp/compressor.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,35 @@
 from collections import deque
 from io import BytesIO
 
 try:
-    from typing import Union
+    from typing import Optional, Union
 except ImportError:
     pass
 
 from . import ExcessBitsError, bit_size, compute_min_pattern_size, initialize_dictionary
 
-try:
-    from micropython import const
-except ImportError:
-
-    def const(x):
-        return x  # noqa: E721
-
-
 # encodes [min_pattern_bytes, min_pattern_bytes + 13] pattern lengths
-huffman_codes = b"\x00\x03\x08\x0b\x14$&+KT\x94\x95\xaa'"
+_huffman_codes = b"\x00\x03\x08\x0b\x14$&+KT\x94\x95\xaa'"
 # These bit lengths pre-add the 1 bit for the 0-value is_literal flag.
-huffman_bits = b"\x02\x03\x05\x05\x06\x07\x07\x07\x08\x08\x09\x09\x09\x07"
-FLUSH_CODE = const(0xAB)  # 8 bits
+_huffman_bits = b"\x02\x03\x05\x05\x06\x07\x07\x07\x08\x08\x09\x09\x09\x07"
+_FLUSH_CODE = 0xAB  # 8 bits
 
 
-class BitWriter:
+class _BitWriter:
     """Writes bits to a stream."""
 
     def __init__(self, f, close_f_on_close=False):
         self.close_f_on_close = close_f_on_close
         self.f = f
         self.buffer = 0  # Basically a uint24
         self.bit_pos = 0
 
     def write_huffman(self, pattern_size):
-        return self.write(huffman_codes[pattern_size], huffman_bits[pattern_size])
+        return self.write(_huffman_codes[pattern_size], _huffman_bits[pattern_size])
 
     def write(self, bits, num_bits, flush=True):
         bits &= (1 << num_bits) - 1
         self.bit_pos += num_bits
         self.buffer |= bits << (32 - self.bit_pos)
 
         bytes_written = 0
@@ -49,15 +41,15 @@
                 self.bit_pos -= 8
                 bytes_written += 1
         return bytes_written
 
     def flush(self, write_token=True):
         bytes_written = 0
         if self.bit_pos > 0 and write_token:
-            bytes_written += self.write(FLUSH_CODE, 9)
+            bytes_written += self.write(_FLUSH_CODE, 9)
 
         while self.bit_pos > 0:
             byte = (self.buffer >> 24) & 0xFF
             self.f.write(byte.to_bytes(1, "big"))
             self.bit_pos = 0
             self.buffer = 0
             bytes_written += 1
@@ -68,15 +60,15 @@
 
     def close(self):
         self.flush(write_token=False)
         if self.close_f_on_close:
             self.f.close()
 
 
-class RingBuffer:
+class _RingBuffer:
     def __init__(self, buffer):
         self.buffer = buffer
         self.size = len(buffer)
         self.pos = 0  # Always pointing to the byte-to-be-overwritten
 
     def write_byte(self, byte):  # ~10% of time
         self.buffer[self.pos] = byte
@@ -93,52 +85,62 @@
 class Compressor:
     """Compresses data to a file or stream."""
 
     def __init__(
         self,
         f,
         *,
-        window=10,
-        literal=8,
-        dictionary=None,
+        window: int = 10,
+        literal: int = 8,
+        dictionary: Optional[bytearray] = None,
     ):
         """
         Parameters
         ----------
+        f: Union[str, Path, FileLike]
+            Path/FileHandle/Stream to write compressed data to.
         window: int
             Size of window buffer in bits.
-            Defaults to 10 (1024 byte buffer).
+            Higher values will typically result in higher compression ratios and higher computation cost.
+            A same size buffer is required at decompression time.
+            Valid range: ``[8, 15]``.
+            Defaults to ``10`` (``1024`` byte buffer).
         literal: int
-            Size of literals in bits.
-            Defaults to 8.
+            Number of used bits in each byte of data.
+            The default ``8`` bits can store all data.
+            A common other value is ``7`` for storing ascii characters where the most-significant-bit is always 0.
+            Smaller values result in higher compression ratios for no additional computation cost.
+            Valid range: ``[5, 8]``.
         dictionary: Optional[bytearray]
-            Use the given initialized buffer inplace.
-            At decompression time, the same buffer must be provided.
+            Use the given **initialized** buffer inplace.
+            At decompression time, the same initialized buffer must be provided.
             ``window`` must agree with the dictionary size.
+            If providing a pre-allocated buffer, but with default initialization, it must
+            first be initialized with :func:`~tamp.initialize_dictionary`
         """
         if not hasattr(f, "write"):  # It's probably a path-like object.
             # TODO: then close it on close
             f = open(str(f), "wb")
             close_f_on_close = True
         else:
             close_f_on_close = False
 
-        self._bit_writer = BitWriter(f, close_f_on_close=close_f_on_close)
+        self._bit_writer = _BitWriter(f, close_f_on_close=close_f_on_close)
         if dictionary and bit_size(len(dictionary) - 1) != window:
             raise ValueError("Dictionary-window size mismatch.")
 
         self.window_bits = window
         self.literal_bits = literal
 
         self.min_pattern_size = compute_min_pattern_size(window, literal)
         self.max_pattern_size = self.min_pattern_size + 13
 
         self.literal_flag = 1 << self.literal_bits
 
-        self._window_buffer = RingBuffer(
+        self._window_buffer = _RingBuffer(
             buffer=dictionary if dictionary else initialize_dictionary(1 << window),
         )
 
         self._input_buffer = deque(maxlen=self.max_pattern_size)
 
         # Callbacks for debugging/metric collection; can be externally set.
         self.token_cb = None
@@ -188,20 +190,20 @@
                 raise ExcessBitsError
 
             bytes_written += self._bit_writer.write(char | self.literal_flag, self.literal_bits + 1)
             self._window_buffer.write_byte(char)
 
         return bytes_written
 
-    def write(self, data: bytes) -> int:
+    def write(self, data: Union[bytes, bytearray]) -> int:
         """Compress ``data`` to stream.
 
         Parameters
         ----------
-        data: bytes
+        data: Union[bytes, bytearray]
             Data to be compressed.
 
         Returns
         -------
         int
             Number of compressed bytes written.
             May be zero when data is filling up internal buffers.
@@ -212,82 +214,114 @@
             self._input_buffer.append(char)
             if len(self._input_buffer) == self._input_buffer.maxlen:
                 bytes_written += self._compress_input_buffer_single()
 
         return bytes_written
 
     def flush(self, write_token: bool = True) -> int:
-        """Flushes internal buffers.
+        """Flushes all internal buffers.
+
+        This compresses any data remaining in the input buffer,
+        and flushes any remaining data in the output buffer to
+        disk.
 
         Parameters
         ----------
         write_token: bool
             If appropriate, write a ``FLUSH`` token.
-            Defaults to ``True``.
+            Defaults to :obj:`True`.
 
         Returns
         -------
         int
-            Number of compressed bytes flushed.
+            Number of compressed bytes flushed to disk.
         """
         bytes_written = 0
         if self.flush_cb:
             self.flush_cb()
         while self._input_buffer:
             bytes_written += self._compress_input_buffer_single()
         bytes_written += self._bit_writer.flush(write_token=write_token)
         return bytes_written
 
     def close(self) -> int:
-        """Flushes internal buffers and close the output file or stream.
+        """Flushes all internal buffers and closes the output file or stream, if tamp opened it.
 
         Returns
         -------
         int
-            Number of compressed bytes flushed.
+            Number of compressed bytes flushed to disk.
         """
         bytes_written = 0
         bytes_written += self.flush(write_token=False)
         self._bit_writer.close()
         return bytes_written
 
-    def __enter__(self):
+    def __enter__(self) -> "Compressor":
+        """Use :class:`Compressor` as a context manager.
+
+        .. code-block:: python
+
+           with tamp.Compressor("output.tamp") as f:
+               f.write(b"foo")
+        """
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
+        """Calls :meth:`~Compressor.close` on contextmanager exit."""
         self.close()
 
 
 class TextCompressor(Compressor):
     """Compresses text to a file or stream."""
 
     def write(self, data: str) -> int:
         return super().write(data.encode())
 
 
-def compress(data: Union[bytes, str], *args, **kwargs) -> bytes:
+def compress(
+    data: Union[bytes, str],
+    *,
+    window: int = 10,
+    literal: int = 8,
+    dictionary: Optional[bytearray] = None,
+) -> bytes:
     """Single-call to compress data.
 
     Parameters
     ----------
     data: Union[str, bytes]
         Data to compress.
-    *args: tuple
-        Passed along to :class:`Compressor`.
-    **kwargs : dict
-        Passed along to :class:`Compressor`.
+    window: int
+        Size of window buffer in bits.
+        Higher values will typically result in higher compression ratios and higher computation cost.
+        A same size buffer is required at decompression time.
+        Valid range: ``[8, 15]``.
+        Defaults to ``10`` (``1024`` byte buffer).
+    literal: int
+        Number of used bits in each byte of data.
+        The default ``8`` bits can store all data.
+        A common other value is ``7`` for storing ascii characters where the most-significant-bit is always 0.
+        Valid range: ``[5, 8]``.
+    dictionary: Optional[bytearray]
+        Use the given **initialized** buffer inplace.
+        At decompression time, the same initialized buffer must be provided.
+        ``window`` must agree with the dictionary size.
+        If providing a pre-allocated buffer, but with default initialization, it must
+        first be initialized with :func:`~tamp.initialize_dictionary`
+
 
     Returns
     -------
     bytes
         Compressed data
     """
     with BytesIO() as f:
         if isinstance(data, str):
-            c = TextCompressor(f, *args, **kwargs)
+            c = TextCompressor(f, window=window, literal=literal, dictionary=dictionary)
             c.write(data)
         else:
-            c = Compressor(f, *args, **kwargs)
+            c = Compressor(f, window=window, literal=literal, dictionary=dictionary)
             c.write(data)
         c.flush(write_token=False)
         f.seek(0)
         return f.read()
```

### Comparing `tamp-1.3.1/tamp/compressor_viper.py` & `tamp-1.4.0/tamp/compressor_viper.py`

 * *Files identical despite different names*

### Comparing `tamp-1.3.1/tamp/ctamp.pxd` & `tamp-1.4.0/tamp/ctamp.pxd`

 * *Files identical despite different names*

### Comparing `tamp-1.3.1/tamp/decompressor.py` & `tamp-1.4.0/tamp/decompressor.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 from io import BytesIO
 
+try:
+    from typing import Optional
+except ImportError:
+    pass
+
 from . import compute_min_pattern_size, initialize_dictionary
 
+_CHUNK_SIZE = 1 << 20
 _FLUSH = object()
 
 # Each key here are the huffman codes or'd with 0x80
 # This is so that each lookup is easy/quick.
-huffman_lookup = {
+_huffman_lookup = {
     0b0: 0,
     0b11: 1,
     0b1000: 2,
     0b1011: 3,
     0b10100: 4,
     0b100100: 5,
     0b100110: 6,
@@ -21,25 +27,25 @@
     0b10010101: 11,
     0b10101010: 12,
     0b100111: 13,
     0b10101011: _FLUSH,
 }
 
 
-class BitReader:
+class _BitReader:
     """Reads bits from a stream."""
 
     def __init__(self, f, close_f_on_close=False):
         self.close_f_on_close = close_f_on_close
         self.f = f
         self.clear()
 
     def read_huffman(self):
         proposed_code = 0
-        lookup = huffman_lookup
+        lookup = _huffman_lookup
         read = self.read
         for _ in range(8):
             proposed_code |= read(1)
             try:
                 return lookup[proposed_code]
             except KeyError:
                 proposed_code <<= 1
@@ -69,15 +75,14 @@
         self.buffer = 0
         self.bit_pos = 0
 
         self.backup_buffer = None
         self.backup_bit_pos = None
 
     def close(self):
-        self.f.close()
         if self.close_f_on_close:
             self.f.close()
 
     def __len__(self):
         return self.bit_pos
 
     def __enter__(self):
@@ -94,15 +99,15 @@
             self.buffer = self.backup_buffer
             self.bit_pos = self.backup_bit_pos
 
         self.backup_buffer = None
         self.backup_bit_pos = None
 
 
-class RingBuffer:
+class _RingBuffer:
     def __init__(self, buffer):
         self.buffer = buffer
         self.size = len(buffer)
         self.pos = 0  # Always pointing to the byte-to-be-overwritten
         self.index = self.buffer.index
 
     def write_byte(self, byte):  # ~10% of time
@@ -116,164 +121,216 @@
             self.write_byte(byte)
 
 
 class Decompressor:
     """Decompresses a file or stream of tamp-compressed data.
 
     Can be used as a context manager to automatically handle file
-    opening and closing::
+    opening and closing:
+
+    .. code-block:: python
 
         with tamp.Decompressor("compressed.tamp") as f:
             decompressed_data = f.read()
     """
 
-    def __init__(self, f, *, dictionary=None):
+    def __init__(self, f, *, dictionary: Optional[bytearray] = None):
         """
         Parameters
         ----------
         f: Union[file, str]
             File-like object to read compressed bytes from.
-        dictionary: bytearray
-            Use dictionary inplace as window buffer.
+        dictionary: Optional[bytearray]
+            Use the given **initialized** buffer inplace.
+            At compression time, the same initialized buffer must be provided.
+            Decompression stream's ``window`` must agree with the dictionary size.
+            If providing a pre-allocated buffer, but with default initialization, it must
+            first be initialized with :func:`~tamp.initialize_dictionary`
         """
         if not hasattr(f, "read"):  # It's probably a path-like object.
             f = open(str(f), "rb")
             close_f_on_close = True
         else:
             close_f_on_close = False
 
-        self._bit_reader = BitReader(f, close_f_on_close=close_f_on_close)
+        self._bit_reader = _BitReader(f, close_f_on_close=close_f_on_close)
 
         # Read Header
         self.window_bits = self._bit_reader.read(3) + 8
         self.literal_bits = self._bit_reader.read(2) + 5
         uses_custom_dictionary = self._bit_reader.read(1)
         reserved = self._bit_reader.read(1)
         more_header_bytes = self._bit_reader.read(1)
 
         if reserved:
             raise NotImplementedError
 
         if more_header_bytes:
             raise NotImplementedError
 
-        if uses_custom_dictionary ^ bool(dictionary):
+        if uses_custom_dictionary and dictionary is None:
             raise ValueError
 
-        self._window_buffer = RingBuffer(
-            buffer=dictionary if dictionary else initialize_dictionary(1 << self.window_bits),
+        self._window_buffer = _RingBuffer(
+            buffer=(dictionary if dictionary else initialize_dictionary(1 << self.window_bits)),
         )
 
         self.min_pattern_size = compute_min_pattern_size(self.window_bits, self.literal_bits)
 
         self.overflow = bytearray()
 
-    def read(self, size=-1) -> bytearray:
-        """Decompresses data to bytes.
+    def readinto(self, buf: bytearray) -> int:
+        """Decompresses data into provided buffer.
 
         Parameters
         ----------
-        size: int
-            Maximum number of bytes to return.
-            If a negative value is provided, all data will be returned.
-            Defaults to ``-1``.
+        buf: bytearray
+            Buffer to decode data into.
 
         Returns
         -------
-        bytearray
-            Decompressed data.
+        int
+            Number of bytes decompressed into buffer.
         """
-        if size < 0:
-            size = 0xFFFFFFFF
-
-        if len(self.overflow) > size:
-            out = self.overflow[:size]
-            self.overflow = self.overflow[size:]
-            return out
+        if len(self.overflow) > len(buf):
+            buf[:] = self.overflow[: len(buf)]
+            written = len(buf)
+            self.overflow = self.overflow[len(buf) :]
+            return written
         elif self.overflow:
-            out = self.overflow
+            buf[: len(self.overflow)] = self.overflow
+            written = len(self.overflow)
             self.overflow = bytearray()
         else:
-            out = bytearray()
+            written = 0
 
-        while len(out) < size:
+        while written < len(buf):
             try:
                 with self._bit_reader:
                     is_literal = self._bit_reader.read(1)
 
                     if is_literal:
                         c = self._bit_reader.read(self.literal_bits)
                         self._window_buffer.write_byte(c)
-                        out.append(c)
+                        buf[written] = c
+                        written += 1
                     else:
                         match_size = self._bit_reader.read_huffman()
                         if match_size is _FLUSH:
                             self._bit_reader.clear()
                             continue
                         match_size += self.min_pattern_size
                         index = self._bit_reader.read(self.window_bits)
 
                         string = self._window_buffer.buffer[index : index + match_size]
                         self._window_buffer.write_bytes(string)
 
-                        out.extend(string)
-                        if len(out) > size:
-                            self.overflow[:] = out[size:]
-                            out = out[:size]
+                        to_buf = min(len(buf) - written, match_size)
+                        buf[written : written + to_buf] = string[:to_buf]
+                        written += to_buf
+                        if to_buf < match_size:
+                            self.overflow[:] = string[to_buf:]
                             break
             except EOFError:
                 break
 
-        return out
+        return written
+
+    def read(self, size: int = -1) -> bytearray:
+        """Decompresses data to bytes.
+
+        Parameters
+        ----------
+        size: int
+            Maximum number of bytes to return.
+            If a negative value is provided, all data will be returned.
+            Defaults to ``-1``.
+
+        Returns
+        -------
+        bytearray
+            Decompressed data.
+        """
+        if size == 0:
+            return bytearray()
+
+        chunk_size = _CHUNK_SIZE
+        out = []
+        while True:
+            buf = bytearray(chunk_size if size < 0 else size)
+            chunk_size <<= 1  # Keep allocating larger chunks as we go on.
+            read_size = self.readinto(buf)
+            if size > 0:
+                # Read the entire contents in one go.
+                out.append(buf)
+                break
+            else:
+                if read_size < len(buf):
+                    if read_size:
+                        out.append(buf[:read_size])
+                    break
+                else:
+                    out.append(buf)
+        return out[0] if len(out) == 1 else bytearray(b"".join(out))
 
     def close(self):
-        """Closes the input file or stream."""
+        """Closes the input file or stream, if tamp opened it."""
         self._bit_reader.close()
 
     def __enter__(self):
+        """Use :class:`Decompressor` as a context manager.
+
+        .. code-block:: python
+
+           with tamp.Decompressor("output.tamp") as f:
+               decompressed_data = f.read()
+        """
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
+        """Calls :meth:`~Decompressor.close` on contextmanager exit."""
         self.close()
 
 
 class TextDecompressor(Decompressor):
     """Decompresses a file or stream of tamp-compressed data into text."""
 
-    def read(self, *args, **kwargs) -> str:
+    def read(self, size: int = -1) -> str:
         """Decompresses data to text.
 
         Parameters
         ----------
         size: int
             Maximum number of bytes to return.
             If a negative value is provided, all data will be returned.
             Defaults to ``-1``.
 
         Returns
         -------
         str
             Decompressed text.
         """
-        return super().read(*args, **kwargs).decode()
+        return super().read(size).decode()
 
 
-def decompress(data: bytes, *args, **kwargs) -> bytearray:
+def decompress(data: bytes, *, dictionary: Optional[bytearray] = None) -> bytearray:
     """Single-call to decompress data.
 
     Parameters
     ----------
     data: bytes
-        Plaintext data to compress.
-    *args: tuple
-        Passed along to :class:`Decompressor`.
-    **kwargs : dict
-        Passed along to :class:`Decompressor`.
+        Tamp-compressed data to decompress.
+    dictionary: Optional[bytearray]
+        Use the given **initialized** buffer inplace.
+        At compression time, the same initialized buffer must be provided.
+        Decompression stream's ``window`` must agree with the dictionary size.
+        If providing a pre-allocated buffer, but with default initialization, it must
+        first be initialized with :func:`~tamp.initialize_dictionary`
 
     Returns
     -------
     bytearray
         Decompressed data.
     """
     with BytesIO(data) as f:
-        d = Decompressor(f, *args, **kwargs)
+        d = Decompressor(f, dictionary=dictionary)
         return d.read()
```

### Comparing `tamp-1.3.1/tamp/decompressor_viper.py` & `tamp-1.4.0/tamp/decompressor_viper.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,22 +42,19 @@
 
         self.min_pattern_size = compute_min_pattern_size(self.w_bits, self.literal_bits)
 
         self.overflow_buf = bytearray(self.min_pattern_size + 13)
         self.overflow_pos = 0
         self.overflow_size = 0
 
-    def readinto(self, buf):
-        raise NotImplementedError
-
     @micropython.viper
-    def _decompress_into(self, out) -> int:
+    def readinto(self, buf) -> int:
         """Attempt to fill out, will place into overflow."""
-        out_capacity = int(len(out))  # const
-        out_buf = ptr8(out)
+        out_capacity = int(len(buf))  # const
+        out_buf = ptr8(buf)
 
         huffman_table = ptr8(_HUFFMAN_TABLE)
 
         literal_bits = int(self.literal_bits)
 
         overflow_buf = self.overflow_buf
         overflow_buf_ptr = ptr8(overflow_buf)
@@ -76,15 +73,15 @@
 
         min_pattern_size = int(self.min_pattern_size)
         int(len(overflow_buf))
 
         # Copy overflow into out if available
         overflow_copy = int(min(overflow_size, out_capacity))
         for i in range(overflow_copy):
-            out[i] = overflow_buf_ptr[overflow_pos + i]
+            buf[i] = overflow_buf_ptr[overflow_pos + i]
         out_pos = overflow_copy
         overflow_pos += overflow_copy
         overflow_size -= overflow_copy
 
         full_mask = int(0x3FFFFFFF)
 
         # Decompress more
@@ -180,26 +177,26 @@
         elif size < 0:
             # Read into a bunch of chunks, then do a single join.
             chunks = []
             chunk_size = 1024
             decompressed_bytes = 0
             while True:
                 chunk = bytearray(chunk_size)
-                chunk_decompressed_bytes = self._decompress_into(chunk)
+                chunk_decompressed_bytes = self.readinto(chunk)
                 if chunk_decompressed_bytes != chunk_size:
                     chunk = chunk[:chunk_decompressed_bytes]
                 chunks.append(chunk)
 
                 if chunk_decompressed_bytes != chunk_size:
                     break
 
             out = b"".join(chunks)
         else:
             out = bytearray(size)
-            decompressed_bytes = self._decompress_into(out)
+            decompressed_bytes = self.readinto(out)
             if decompressed_bytes != size:
                 out = out[:decompressed_bytes]
 
         return out
 
     def close(self):
         if self._close_f_on_close:
```

### Comparing `tamp-1.3.1/PKG-INFO` & `tamp-1.4.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tamp
-Version: 1.3.1
+Version: 1.4.0
 Summary: 
 Home-page: https://github.com/BrianPugh/tamp
 License: Apache-2.0
 Author: Brian Pugh
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -28,32 +28,50 @@
 |Python compat| |PyPi| |GHA tests| |Codecov report| |readthedocs|
 
 .. inclusion-marker-do-not-remove
 
 Tamp
 ====
 
-Tamp is a low-memory, DEFLATE-inspired lossless compression library.
+Tamp is a low-memory, DEFLATE-inspired lossless compression library intended for embedded targets.
+
+Tamp delivers the highest data compression ratios, while using the least amount of RAM and firmware storage.
+
+
+**Documentation:** https://tamp.readthedocs.io/en/latest/
+
+**Source Code:** https://github.com/BrianPugh/tamp
+
 
 Features
 ========
 
-* Various implementations available:
+* Various language implementations available:
+
+  * Pure Python reference:
+
+    * ``tamp/__init__.py``, ``tamp/compressor.py``, ``tamp/decompressor.py``
 
-  * Pure Python:
+    * ``pip install tamp`` will use a python-bound C implementation optimized for speed.
 
-    * ``tamp/compressor.py``, ``tamp/decompressor.py``
+  * Micropython:
 
-    * When available, Tamp will use a python-bound C implementation for speed.
+    * Native Module (suggested micropython implementation).
+
+      * ``mpy_bindings/``
+
+    * Viper.
+
+      * ``tamp/__init__.py``, ``tamp/compressor_viper.py``, ``tamp/decompressor_viper.py``
 
   * C library:
 
     * ``tamp/_c_src/``
 
-* High compression ratios and low memory use.
+* High compression ratios, low memory use, and fast.
 
 * Compact compression and decompression implementations.
 
   * Compiled C library is <4KB (compressor + decompressor).
 
 * Mid-stream flushing.
 
@@ -61,32 +79,58 @@
 
 * Customizable dictionary for greater compression of small messages.
 
 * Convenient CLI interface.
 
 Installation
 ============
-Tamp contains 3 implementations:
+Tamp contains 4 implementations:
+
+1. A reference desktop CPython implementation that is optimized for readability (and **not** speed).
 
-1. A desktop Cpython implementation that is optimized for readability
+2. A Micropython Native Module implementation (fast).
 
-2. A micropython viper implementation that is optimized for runtime performance.
+3. A Micropython Viper implementation (not recommended, please use Native Module).
 
-3. A C implementation (with python bindings) for accelerated desktop use and to be used in C projects.
+4. A C implementation (with python bindings) for accelerated desktop use and to be used in C projects (very fast).
+
+This section instructs how to install each implementation.
 
 Desktop Python
 ^^^^^^^^^^^^^^
 The Tamp library and CLI requires Python ``>=3.8`` and can be installed via:
 
 .. code-block:: bash
 
    pip install tamp
 
 MicroPython
 ^^^^^^^^^^^
+
+MicroPython Native Module
+-------------------------
+Tamp provides pre-compiled `native modules` that are easy to install, are small, and are incredibly fast.
+
+Download the appropriate ``.mpy`` file from the `release page`_.
+
+   * Match the micropython version.
+
+   * Match the architecture to the microcontroller (e.g. ``armv6m`` for a pi pico).
+
+Rename the file to ``tamp.mpy`` and transfer it to your board. If using `Belay`_, tamp can be installed by adding the following to ``pyproject.toml``.
+
+.. code-block:: toml
+
+   [tool.belay.dependencies]
+   tamp = "https://github.com/BrianPugh/tamp/releases/download/v1.4.0/tamp-1.4.0-mpy1.22-armv6m.mpy"
+
+MicroPython Viper
+-----------------
+**NOT RECOMMENDED, PLEASE USE NATIVE MODULE**
+
 For micropython use, there are 3 main files:
 
 1. ``tamp/__init__.py`` - Always required.
 
 2. ``tamp/decompressor_viper.py`` - Required for on-device decompression.
 
 3. ``tamp/compressor_viper.py`` - Required for on-device compression.
@@ -132,34 +176,24 @@
 Use ``tamp compress`` to compress a file or stream.
 If no input file is specified, data from stdin will be read.
 If no output is specified, the compressed output stream will be written to stdout.
 
 .. code-block:: bash
 
    $ tamp compress --help
+   Usage: tamp compress [ARGS] [OPTIONS]
 
-    Usage: tamp compress [OPTIONS] [INPUT_PATH]
-
-    Compress an input file or stream.
-
-   ╭─ Arguments ────────────────────────────────────────────────────────────────────────╮
-   │   input_path      [INPUT_PATH]  Input file to compress or decompress. Defaults to  │
-   │                                 stdin.                                             │
-   ╰────────────────────────────────────────────────────────────────────────────────────╯
-   ╭─ Options ──────────────────────────────────────────────────────────────────────────╮
-   │ --output   -o      PATH                      Output file. Defaults to stdout.      │
-   │ --window   -w      INTEGER RANGE [8<=x<=15]  Number of bits used to represent the  │
-   │                                              dictionary window.                    │
-   │                                              [default: 10]                         │
-   │ --literal  -l      INTEGER RANGE [5<=x<=8]   Number of bits used to represent a    │
-   │                                              literal.                              │
-   │                                              [default: 8]                          │
-   │ --help                                       Show this message and exit.           │
-   ╰────────────────────────────────────────────────────────────────────────────────────╯
+   Compress an input file or stream.
 
+   ╭─ Parameters ───────────────────────────────────────────────────────────────────────────────╮
+   │ INPUT,--input    -i  Input file to compress. Defaults to stdin.                            │
+   │ OUTPUT,--output  -o  Output compressed file. Defaults to stdout.                           │
+   │ --window         -w  Number of bits used to represent the dictionary window. [default: 10] │
+   │ --literal        -l  Number of bits used to represent a literal. [default: 8]              │
+   ╰────────────────────────────────────────────────────────────────────────────────────────────╯
 
 Example usage:
 
 .. code-block:: bash
 
    tamp compress enwik8 -o enwik8.tamp  # Compress a file
    echo "hello world" | tamp compress | wc -c  # Compress a stream and print the compressed size.
@@ -180,27 +214,23 @@
 -------------
 Use ``tamp decompress`` to decompress a file or stream.
 If no input file is specified, data from stdin will be read.
 If no output is specified, the compressed output stream will be written to stdout.
 
 .. code-block:: bash
 
-  $ tamp decompress --help
-
-  Usage: tamp decompress [OPTIONS] [INPUT_PATH]
+   $ tamp decompress --help
+   Usage: tamp decompress [ARGS] [OPTIONS]
 
-  Decompress an input file or stream.
+   Decompress an input file or stream.
 
- ╭─ Arguments ────────────────────────────────────────────────────────────────────────╮
- │   input_path      [INPUT_PATH]  Input file. If not provided, reads from stdin.     │
- ╰────────────────────────────────────────────────────────────────────────────────────╯
- ╭─ Options ──────────────────────────────────────────────────────────────────────────╮
- │ --output  -o      PATH  Output file. Defaults to stdout.                           │
- │ --help                  Show this message and exit.                                │
- ╰────────────────────────────────────────────────────────────────────────────────────╯
+   ╭─ Parameters ───────────────────────────────────────────────────────────────────────────────╮
+   │ INPUT,--input    -i  Input file to decompress. Defaults to stdin.                          │
+   │ OUTPUT,--output  -o  Output decompressed file. Defaults to stdout.                         │
+   ╰────────────────────────────────────────────────────────────────────────────────────────────╯
 
 Example usage:
 
 .. code-block:: bash
 
    tamp decompress enwik8.tamp -o enwik8
    echo "hello world" | tamp compress | tamp decompress
@@ -284,71 +314,77 @@
 memory during both compression and decompression (see next section). Tamp accomplishes
 competitive performance while using around 10x less memory.
 
 Memory Usage
 ^^^^^^^^^^^^
 The following table shows approximately how much memory each algorithm uses during compression and decompression.
 
-+---------------+-------------------+------------------------------+-------------------+
-| Action        | tamp              | zlib                         | heatshrink        |
-+===============+===================+==============================+===================+
-| Compression   | (1 << windowBits) | (1 << (windowBits+2)) + 7 KB | (1 << windowBits) |
-+---------------+-------------------+------------------------------+-------------------+
-| Decompression | (1 << windowBits) | (1 << windowBits) + 7 KB     | (1 << windowBits) |
-+---------------+-------------------+------------------------------+-------------------+
++---------------+-------------------+------------------------------+-------------------------+-----------------------+
+| Action        | tamp              | zlib                         | heatshrink              | deflate (micropython) |
++===============+===================+==============================+=========================+=======================+
+| Compression   | (1 << windowBits) | (1 << (windowBits+2)) + 7 KB | (1 << (windowBits + 1)) | (1 << windowBits)     |
++---------------+-------------------+------------------------------+-------------------------+-----------------------+
+| Decompression | (1 << windowBits) | (1 << windowBits) + 7 KB     | (1 << (windowBits + 1)) | (1 << windowBits)     |
++---------------+-------------------+------------------------------+-------------------------+-----------------------+
 
-Both tamp and heatshrink have a few dozen bytes of overhead in addition to the primary window buffer, but are implementation-specific and ignored for clarity here.
+All libraries have a few dozen bytes of overhead in addition to the primary window buffer, but are implementation-specific and ignored for clarity here.
+Tamp uses significantly less memory than ZLib, and half the memory of Heatshrink.
 
 Runtime
 ^^^^^^^
 As a rough benchmark, here is the performance (in seconds) of these different compression algorithms on the 100MB enwik8 dataset.
 These tests were performed on an M1 Macbook Air.
 
 +---------------+--------------------+-------+------+--------------+-----------------+
 | Action        | tamp               | tamp  | zlib | heatshrink   | heatshrink      |
 |               | (Python Reference) | (C)   |      | (with index) | (without index) |
 +===============+====================+=======+======+==============+=================+
 | Compression   | 109.5              | 16.45 | 4.84 | 6.22         | 41.729          |
 +---------------+--------------------+-------+------+--------------+-----------------+
-| Decompression | 54.0               | 0.70  | 0.98 | 0.82         | 0.82            |
+| Decompression | 76.0               | 0.142 | 0.98 | 0.82         | 0.82            |
 +---------------+--------------------+-------+------+--------------+-----------------+
 
 Heatshrink v0.4.1 was used in these benchmarks.
-When heathshrink uses an index, an additional ``(1 << (windowBits + 1))`` bytes of memory are used, tripling the memory requirement.
+When heathshrink uses an index, an additional ``(1 << (windowBits + 1))`` bytes of memory are used, resulting in 4x more memory-usage than Tamp.
 Tamp could use a similar indexing to increase compression speed, but has chosen not to to focus on the primary goal of a low-memory compressor.
 
 To give an idea of Tamp's speed on an embedded device, the following table shows compression/decompression in **bytes/second of the first 100KB of enwik8 on a pi pico (rp2040)** at the default 125MHz clock rate.
-This isn't exactly an apples-to-apples comparison because the C benchmark does not use a filesystem (and thusly, reduced overhead) nor dynamic memory allocation, but is good enough to get the idea across.
+The C benchmark **does not** use a filesystem nor dynamic memory allocation, so it represents the maximum speed Tamp can achieve.
+In all tests, a 1KB window (10 bit) was used.
+
++---------------+---------------------+-----------------------------+------------+-----------------------+
+| Action        | tamp                | tamp                        | tamp       | deflate.DeflatIO      |
+|               | (Micropython Viper) | (Micropython Native Module) | (C)        | (micropython builtin) |
++===============+=====================+=============================+============+=======================+
+| Compression   | ~4,300              | ~12,770                     | ~28,500    | ~6,715                |
++---------------+---------------------+-----------------------------+------------+-----------------------+
+| Decompression | ~42,000             | ~644,010                    | ~1,042,524 | ~146,477              |
++---------------+---------------------+-----------------------------+------------+-----------------------+
 
-+---------------+---------------------+------------+
-| Action        | tamp                | tamp       |
-|               | (Micropython Viper) | (C)        |
-+===============+=====================+============+
-| Compression   | ~4,300              | ~28,500    |
-+---------------+---------------------+------------+
-| Decompression | ~42,000             | ~1,042,524 |
-+---------------+---------------------+------------+
+Tamp resulted in a **51637** byte archive, while Micropython's builtin ``deflate`` resulted in a larger **59442** byte archive.
 
 Binary Size
 ^^^^^^^^^^^
 To give an idea on the resulting binary sizes, Tamp and other libraries were compiled for the Pi Pico (``armv6m``).
 All libraries were compiled with ``-O3``.
 Numbers reported in bytes.
 
-+--------------------+------------+--------------+---------------------------+
-| Library            | Compressor | Decompressor | Compressor + Decompressor |
-+====================+============+==============+===========================+
-| Tamp (micropython) | 4429       | 4205         | 7554                      |
-+--------------------+------------+--------------+---------------------------+
-| Tamp (C)           | 2008       | 1972         | 3864                      |
-+--------------------+------------+--------------+---------------------------+
-| Heatshrink         | 2956       | 3876         | 6832                      |
-+--------------------+------------+--------------+---------------------------+
-| uzlib              | 2355       | 3963         | 6318                      |
-+--------------------+------------+--------------+---------------------------+
++----------------------------------+------------+--------------+---------------------------+
+| Library                          | Compressor | Decompressor | Compressor + Decompressor |
++==================================+============+==============+===========================+
+| Tamp (micropython viper)         | 4429       | 4205         | 7554                      |
++----------------------------------+------------+--------------+---------------------------+
+| Tamp (micropython native module) | 3264       | 3079         | 5537                      |
++----------------------------------+------------+--------------+---------------------------+
+| Tamp (C)                         | 2008       | 1972         | 3864                      |
++----------------------------------+------------+--------------+---------------------------+
+| Heatshrink                       | 2956       | 3876         | 6832                      |
++----------------------------------+------------+--------------+---------------------------+
+| uzlib                            | 2355       | 3963         | 6318                      |
++----------------------------------+------------+--------------+---------------------------+
 
 Heatshrink doesn't include a high level API; in an apples-to-apples comparison the Tamp library would be even smaller.
 
 
 .. |GHA tests| image:: https://github.com/BrianPugh/tamp/workflows/tests/badge.svg
    :target: https://github.com/BrianPugh/tamp/actions?query=workflow%3Atests
    :alt: GHA Status
@@ -364,8 +400,10 @@
 .. _Belay: https://github.com/BrianPugh/belay
 .. _zlib:  https://docs.python.org/3/library/zlib.html
 .. _heatshrink: https://github.com/atomicobject/heatshrink
 .. _Silesia Corpus: https://sun.aei.polsl.pl//~sdeor/index.php?page=silesia
 .. _Enwik8: https://mattmahoney.net/dc/textdata.html
 .. _mip: https://docs.micropython.org/en/latest/reference/packages.html#installing-packages-with-mip
 .. _the documentation: https://tamp.readthedocs.io/en/latest/c_library.html
+.. _native modules: https://docs.micropython.org/en/latest/develop/natmod.html
+.. _release page: https://github.com/BrianPugh/tamp/releases
```

