# Comparing `tmp/novelai_python-0.4.8.tar.gz` & `tmp/novelai_python-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "novelai_python-0.4.8.tar", last modified: Sat Apr 13 16:05:37 2024, max compression
+gzip compressed data, was "novelai_python-0.4.9.tar", last modified: Thu Apr 25 03:13:58 2024, max compression
```

## Comparing `novelai_python-0.4.8.tar` & `novelai_python-0.4.9.tar`

### file list

```diff
@@ -1,77 +1,77 @@
--rwxr-xr-x   0        0        0    11357 2024-04-13 16:05:24.422073 novelai_python-0.4.8/LICENSE
--rwxr-xr-x   0        0        0      522 2024-04-13 16:05:24.422073 novelai_python-0.4.8/NOTICE.MD
--rwxr-xr-x   0        0        0     3490 2024-04-13 16:05:24.422073 novelai_python-0.4.8/README.md
--rw-r--r--   0        0        0     1201 2024-04-13 16:05:37.270084 novelai_python-0.4.8/pyproject.toml
--rwxr-xr-x   0        0        0     1239 2024-04-13 16:05:24.438073 novelai_python-0.4.8/src/novelai_python/__init__.py
--rwxr-xr-x   0        0        0     1761 2024-04-13 16:05:24.438073 novelai_python-0.4.8/src/novelai_python/_exceptions.py
--rwxr-xr-x   0        0        0      410 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/_response/__init__.py
--rwxr-xr-x   0        0        0      127 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/_response/ai/__init__.py
--rw-r--r--   0        0        0      659 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/_response/ai/generate.py
--rwxr-xr-x   0        0        0      828 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/_response/ai/generate_image.py
--rw-r--r--   0        0        0      724 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/_response/ai/generate_stream.py
--rw-r--r--   0        0        0      185 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/_response/ai/generate_voice.py
--rwxr-xr-x   0        0        0      397 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/_response/ai/upscale.py
--rwxr-xr-x   0        0        0      195 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/_response/schema.py
--rwxr-xr-x   0        0        0      128 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/_response/user/__init__.py
--rwxr-xr-x   0        0        0      721 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/_response/user/information.py
--rwxr-xr-x   0        0        0      204 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/_response/user/login.py
--rwxr-xr-x   0        0        0     2359 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/_response/user/subscription.py
--rwxr-xr-x   0        0        0     1548 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/credential/ApiToken.py
--rwxr-xr-x   0        0        0     1628 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/credential/JwtToken.py
--rwxr-xr-x   0        0        0     1701 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/credential/UserAuth.py
--rwxr-xr-x   0        0        0      424 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/credential/__init__.py
--rwxr-xr-x   0        0        0      462 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/credential/_base.py
--rwxr-xr-x   0        0        0      743 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/sdk/__init__.py
--rwxr-xr-x   0        0        0     1082 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/sdk/ai/LICENSE
--rwxr-xr-x   0        0        0      130 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/sdk/ai/__init__.py
--rw-r--r--   0        0        0     9477 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/sdk/ai/generate/__init__.py
--rw-r--r--   0        0        0     1249 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/sdk/ai/generate/_const.py
--rw-r--r--   0        0        0     1827 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/sdk/ai/generate/_enum.py
--rw-r--r--   0        0        0     6467 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/sdk/ai/generate/_preset.py
--rwxr-xr-x   0        0        0    34778 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/sdk/ai/generate_image/__init__.py
--rw-r--r--   0        0        0    52850 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/sdk/ai/generate_image/_const.py
--rwxr-xr-x   0        0        0     3578 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/sdk/ai/generate_image/_enum.py
--rwxr-xr-x   0        0        0     5306 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/sdk/ai/generate_image/suggest_tags.py
--rw-r--r--   0        0        0     7170 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/sdk/ai/generate_stream.py
--rw-r--r--   0        0        0     7379 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/sdk/ai/generate_voice/__init__.py
--rw-r--r--   0        0        0     2008 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/sdk/ai/generate_voice/_enum.py
--rwxr-xr-x   0        0        0     8223 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/sdk/ai/upscale.py
--rwxr-xr-x   0        0        0      945 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/sdk/schema.py
--rwxr-xr-x   0        0        0      130 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/sdk/user/__init__.py
--rwxr-xr-x   0        0        0     4772 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/sdk/user/information.py
--rwxr-xr-x   0        0        0     5285 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/sdk/user/login.py
--rwxr-xr-x   0        0        0     5045 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/sdk/user/subscription.py
--rwxr-xr-x   0        0        0     7466 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/server.py
--rw-r--r--   0        0        0      534 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/tokenizer/NOTICE.MD
--rw-r--r--   0        0        0     8173 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/tokenizer/__init__.py
--rw-r--r--   0        0        0  1356917 2024-04-13 16:05:24.446073 novelai_python-0.4.8/src/novelai_python/tokenizer/bpe_simple_vocab_16e6.txt.gz
--rw-r--r--   0        0        0  1494140 2024-04-13 16:05:24.454074 novelai_python-0.4.8/src/novelai_python/tokenizer/gpt2-genji_tokenizer.json
--rw-r--r--   0        0        0  1355257 2024-04-13 16:05:24.458073 novelai_python-0.4.8/src/novelai_python/tokenizer/gpt2_tokenizer.json
--rw-r--r--   0        0        0  1033724 2024-04-13 16:05:24.466073 novelai_python-0.4.8/src/novelai_python/tokenizer/nerdstash_v1.model
--rw-r--r--   0        0        0  1033744 2024-04-13 16:05:24.470074 novelai_python-0.4.8/src/novelai_python/tokenizer/nerdstash_v2.model
--rw-r--r--   0        0        0  1033724 2024-04-13 16:05:24.470074 novelai_python-0.4.8/src/novelai_python/tokenizer/novelai.model
--rw-r--r--   0        0        0  1033744 2024-04-13 16:05:24.470074 novelai_python-0.4.8/src/novelai_python/tokenizer/novelai_v2.model
--rw-r--r--   0        0        0  1357239 2024-04-13 16:05:24.478073 novelai_python-0.4.8/src/novelai_python/tokenizer/pile_tokenizer.json
--rw-r--r--   0        0        0     4854 2024-04-13 16:05:24.478073 novelai_python-0.4.8/src/novelai_python/tokenizer/simple_tokenizer.py
--rw-r--r--   0        0        0       24 2024-04-13 16:05:24.478073 novelai_python-0.4.8/src/novelai_python/tool/__init__.py
--rw-r--r--   0        0        0     9084 2024-04-13 16:05:24.478073 novelai_python-0.4.8/src/novelai_python/tool/image_metadata/__init__.py
--rw-r--r--   0        0        0     3316 2024-04-13 16:05:24.478073 novelai_python-0.4.8/src/novelai_python/tool/image_metadata/lsb_extractor.py
--rw-r--r--   0        0        0     2211 2024-04-13 16:05:24.478073 novelai_python-0.4.8/src/novelai_python/tool/image_metadata/lsb_injector.py
--rw-r--r--   0        0        0     3082 2024-04-13 16:05:24.478073 novelai_python-0.4.8/src/novelai_python/tool/paint_mask/__init__.py
--rw-r--r--   0        0        0    17162 2024-04-13 16:05:24.478073 novelai_python-0.4.8/src/novelai_python/tool/random_prompt/__init__.py
--rw-r--r--   0        0        0    84988 2024-04-13 16:05:24.478073 novelai_python-0.4.8/src/novelai_python/tool/random_prompt/tag.py
--rw-r--r--   0        0        0    21015 2024-04-13 16:05:24.478073 novelai_python-0.4.8/src/novelai_python/tool/random_prompt/tag_character.py
--rw-r--r--   0        0        0    15814 2024-04-13 16:05:24.478073 novelai_python-0.4.8/src/novelai_python/tool/random_prompt/tag_nsfw.py
--rwxr-xr-x   0        0        0      525 2024-04-13 16:05:24.478073 novelai_python-0.4.8/src/novelai_python/utils/__init__.py
--rwxr-xr-x   0        0        0     2419 2024-04-13 16:05:24.478073 novelai_python-0.4.8/src/novelai_python/utils/encode.py
--rwxr-xr-x   0        0        0     1243 2024-04-13 16:05:24.478073 novelai_python-0.4.8/src/novelai_python/utils/useful.py
--rwxr-xr-x   0        0        0        0 2024-04-13 16:05:24.478073 novelai_python-0.4.8/tests/__init__.py
--rw-r--r--   0        0        0      870 2024-04-13 16:05:24.478073 novelai_python-0.4.8/tests/test_generate_voice.py
--rwxr-xr-x   0        0        0     2273 2024-04-13 16:05:24.478073 novelai_python-0.4.8/tests/test_random_prompt.py
--rwxr-xr-x   0        0        0      422 2024-04-13 16:05:24.478073 novelai_python-0.4.8/tests/test_server.py
--rwxr-xr-x   0        0        0     1375 2024-04-13 16:05:24.478073 novelai_python-0.4.8/tests/test_server_run.py
--rwxr-xr-x   0        0        0     2772 2024-04-13 16:05:24.478073 novelai_python-0.4.8/tests/test_upscale.py
--rwxr-xr-x   0        0        0     2592 2024-04-13 16:05:24.478073 novelai_python-0.4.8/tests/test_user_information.py
--rwxr-xr-x   0        0        0     3244 2024-04-13 16:05:24.482073 novelai_python-0.4.8/tests/test_user_login.py
--rwxr-xr-x   0        0        0     3270 2024-04-13 16:05:24.482073 novelai_python-0.4.8/tests/test_user_subscription.py
--rw-r--r--   0        0        0     4663 1970-01-01 00:00:00.000000 novelai_python-0.4.8/PKG-INFO
+-rwxr-xr-x   0        0        0    11357 2024-04-25 03:13:43.090355 novelai_python-0.4.9/LICENSE
+-rwxr-xr-x   0        0        0      522 2024-04-25 03:13:43.090355 novelai_python-0.4.9/NOTICE.MD
+-rwxr-xr-x   0        0        0     3490 2024-04-25 03:13:43.090355 novelai_python-0.4.9/README.md
+-rw-r--r--   0        0        0     1201 2024-04-25 03:13:58.498596 novelai_python-0.4.9/pyproject.toml
+-rwxr-xr-x   0        0        0     1239 2024-04-25 03:13:43.106356 novelai_python-0.4.9/src/novelai_python/__init__.py
+-rwxr-xr-x   0        0        0     1761 2024-04-25 03:13:43.106356 novelai_python-0.4.9/src/novelai_python/_exceptions.py
+-rwxr-xr-x   0        0        0      410 2024-04-25 03:13:43.106356 novelai_python-0.4.9/src/novelai_python/_response/__init__.py
+-rwxr-xr-x   0        0        0      127 2024-04-25 03:13:43.106356 novelai_python-0.4.9/src/novelai_python/_response/ai/__init__.py
+-rw-r--r--   0        0        0      659 2024-04-25 03:13:43.106356 novelai_python-0.4.9/src/novelai_python/_response/ai/generate.py
+-rwxr-xr-x   0        0        0      817 2024-04-25 03:13:43.106356 novelai_python-0.4.9/src/novelai_python/_response/ai/generate_image.py
+-rw-r--r--   0        0        0      724 2024-04-25 03:13:43.106356 novelai_python-0.4.9/src/novelai_python/_response/ai/generate_stream.py
+-rw-r--r--   0        0        0      185 2024-04-25 03:13:43.106356 novelai_python-0.4.9/src/novelai_python/_response/ai/generate_voice.py
+-rwxr-xr-x   0        0        0      397 2024-04-25 03:13:43.106356 novelai_python-0.4.9/src/novelai_python/_response/ai/upscale.py
+-rwxr-xr-x   0        0        0      195 2024-04-25 03:13:43.106356 novelai_python-0.4.9/src/novelai_python/_response/schema.py
+-rwxr-xr-x   0        0        0      128 2024-04-25 03:13:43.106356 novelai_python-0.4.9/src/novelai_python/_response/user/__init__.py
+-rwxr-xr-x   0        0        0      721 2024-04-25 03:13:43.106356 novelai_python-0.4.9/src/novelai_python/_response/user/information.py
+-rwxr-xr-x   0        0        0      204 2024-04-25 03:13:43.106356 novelai_python-0.4.9/src/novelai_python/_response/user/login.py
+-rwxr-xr-x   0        0        0     2359 2024-04-25 03:13:43.106356 novelai_python-0.4.9/src/novelai_python/_response/user/subscription.py
+-rwxr-xr-x   0        0        0     1548 2024-04-25 03:13:43.106356 novelai_python-0.4.9/src/novelai_python/credential/ApiToken.py
+-rwxr-xr-x   0        0        0     1628 2024-04-25 03:13:43.106356 novelai_python-0.4.9/src/novelai_python/credential/JwtToken.py
+-rwxr-xr-x   0        0        0     1701 2024-04-25 03:13:43.106356 novelai_python-0.4.9/src/novelai_python/credential/UserAuth.py
+-rwxr-xr-x   0        0        0      424 2024-04-25 03:13:43.106356 novelai_python-0.4.9/src/novelai_python/credential/__init__.py
+-rwxr-xr-x   0        0        0      462 2024-04-25 03:13:43.106356 novelai_python-0.4.9/src/novelai_python/credential/_base.py
+-rwxr-xr-x   0        0        0      743 2024-04-25 03:13:43.106356 novelai_python-0.4.9/src/novelai_python/sdk/__init__.py
+-rwxr-xr-x   0        0        0     1082 2024-04-25 03:13:43.106356 novelai_python-0.4.9/src/novelai_python/sdk/ai/LICENSE
+-rwxr-xr-x   0        0        0      130 2024-04-25 03:13:43.106356 novelai_python-0.4.9/src/novelai_python/sdk/ai/__init__.py
+-rw-r--r--   0        0        0     9477 2024-04-25 03:13:43.106356 novelai_python-0.4.9/src/novelai_python/sdk/ai/generate/__init__.py
+-rw-r--r--   0        0        0     1249 2024-04-25 03:13:43.106356 novelai_python-0.4.9/src/novelai_python/sdk/ai/generate/_const.py
+-rw-r--r--   0        0        0     1821 2024-04-25 03:13:43.106356 novelai_python-0.4.9/src/novelai_python/sdk/ai/generate/_enum.py
+-rw-r--r--   0        0        0     6467 2024-04-25 03:13:43.106356 novelai_python-0.4.9/src/novelai_python/sdk/ai/generate/_preset.py
+-rwxr-xr-x   0        0        0    34778 2024-04-25 03:13:43.106356 novelai_python-0.4.9/src/novelai_python/sdk/ai/generate_image/__init__.py
+-rw-r--r--   0        0        0    52850 2024-04-25 03:13:43.110355 novelai_python-0.4.9/src/novelai_python/sdk/ai/generate_image/_const.py
+-rwxr-xr-x   0        0        0     3861 2024-04-25 03:13:43.110355 novelai_python-0.4.9/src/novelai_python/sdk/ai/generate_image/_enum.py
+-rwxr-xr-x   0        0        0     5306 2024-04-25 03:13:43.110355 novelai_python-0.4.9/src/novelai_python/sdk/ai/generate_image/suggest_tags.py
+-rw-r--r--   0        0        0     7170 2024-04-25 03:13:43.110355 novelai_python-0.4.9/src/novelai_python/sdk/ai/generate_stream.py
+-rw-r--r--   0        0        0     7379 2024-04-25 03:13:43.110355 novelai_python-0.4.9/src/novelai_python/sdk/ai/generate_voice/__init__.py
+-rw-r--r--   0        0        0     2008 2024-04-25 03:13:43.110355 novelai_python-0.4.9/src/novelai_python/sdk/ai/generate_voice/_enum.py
+-rwxr-xr-x   0        0        0     8223 2024-04-25 03:13:43.110355 novelai_python-0.4.9/src/novelai_python/sdk/ai/upscale.py
+-rwxr-xr-x   0        0        0      945 2024-04-25 03:13:43.110355 novelai_python-0.4.9/src/novelai_python/sdk/schema.py
+-rwxr-xr-x   0        0        0      130 2024-04-25 03:13:43.110355 novelai_python-0.4.9/src/novelai_python/sdk/user/__init__.py
+-rwxr-xr-x   0        0        0     4772 2024-04-25 03:13:43.110355 novelai_python-0.4.9/src/novelai_python/sdk/user/information.py
+-rwxr-xr-x   0        0        0     5285 2024-04-25 03:13:43.110355 novelai_python-0.4.9/src/novelai_python/sdk/user/login.py
+-rwxr-xr-x   0        0        0     5045 2024-04-25 03:13:43.110355 novelai_python-0.4.9/src/novelai_python/sdk/user/subscription.py
+-rwxr-xr-x   0        0        0     7579 2024-04-25 03:13:43.110355 novelai_python-0.4.9/src/novelai_python/server.py
+-rw-r--r--   0        0        0      534 2024-04-25 03:13:43.110355 novelai_python-0.4.9/src/novelai_python/tokenizer/NOTICE.MD
+-rw-r--r--   0        0        0     8173 2024-04-25 03:13:43.110355 novelai_python-0.4.9/src/novelai_python/tokenizer/__init__.py
+-rw-r--r--   0        0        0  1356917 2024-04-25 03:13:43.110355 novelai_python-0.4.9/src/novelai_python/tokenizer/bpe_simple_vocab_16e6.txt.gz
+-rw-r--r--   0        0        0  1494140 2024-04-25 03:13:43.118356 novelai_python-0.4.9/src/novelai_python/tokenizer/gpt2-genji_tokenizer.json
+-rw-r--r--   0        0        0  1355257 2024-04-25 03:13:43.126356 novelai_python-0.4.9/src/novelai_python/tokenizer/gpt2_tokenizer.json
+-rw-r--r--   0        0        0  1033724 2024-04-25 03:13:43.130356 novelai_python-0.4.9/src/novelai_python/tokenizer/nerdstash_v1.model
+-rw-r--r--   0        0        0  1033744 2024-04-25 03:13:43.138356 novelai_python-0.4.9/src/novelai_python/tokenizer/nerdstash_v2.model
+-rw-r--r--   0        0        0  1033724 2024-04-25 03:13:43.138356 novelai_python-0.4.9/src/novelai_python/tokenizer/novelai.model
+-rw-r--r--   0        0        0  1033744 2024-04-25 03:13:43.138356 novelai_python-0.4.9/src/novelai_python/tokenizer/novelai_v2.model
+-rw-r--r--   0        0        0  1357239 2024-04-25 03:13:43.146356 novelai_python-0.4.9/src/novelai_python/tokenizer/pile_tokenizer.json
+-rw-r--r--   0        0        0     4854 2024-04-25 03:13:43.146356 novelai_python-0.4.9/src/novelai_python/tokenizer/simple_tokenizer.py
+-rw-r--r--   0        0        0       24 2024-04-25 03:13:43.146356 novelai_python-0.4.9/src/novelai_python/tool/__init__.py
+-rw-r--r--   0        0        0     9084 2024-04-25 03:13:43.146356 novelai_python-0.4.9/src/novelai_python/tool/image_metadata/__init__.py
+-rw-r--r--   0        0        0     3316 2024-04-25 03:13:43.146356 novelai_python-0.4.9/src/novelai_python/tool/image_metadata/lsb_extractor.py
+-rw-r--r--   0        0        0     2211 2024-04-25 03:13:43.146356 novelai_python-0.4.9/src/novelai_python/tool/image_metadata/lsb_injector.py
+-rw-r--r--   0        0        0     3082 2024-04-25 03:13:43.146356 novelai_python-0.4.9/src/novelai_python/tool/paint_mask/__init__.py
+-rw-r--r--   0        0        0    17162 2024-04-25 03:13:43.146356 novelai_python-0.4.9/src/novelai_python/tool/random_prompt/__init__.py
+-rw-r--r--   0        0        0    84988 2024-04-25 03:13:43.146356 novelai_python-0.4.9/src/novelai_python/tool/random_prompt/tag.py
+-rw-r--r--   0        0        0    21015 2024-04-25 03:13:43.146356 novelai_python-0.4.9/src/novelai_python/tool/random_prompt/tag_character.py
+-rw-r--r--   0        0        0    15814 2024-04-25 03:13:43.146356 novelai_python-0.4.9/src/novelai_python/tool/random_prompt/tag_nsfw.py
+-rwxr-xr-x   0        0        0      525 2024-04-25 03:13:43.146356 novelai_python-0.4.9/src/novelai_python/utils/__init__.py
+-rwxr-xr-x   0        0        0     2419 2024-04-25 03:13:43.146356 novelai_python-0.4.9/src/novelai_python/utils/encode.py
+-rwxr-xr-x   0        0        0     1243 2024-04-25 03:13:43.146356 novelai_python-0.4.9/src/novelai_python/utils/useful.py
+-rwxr-xr-x   0        0        0        0 2024-04-25 03:13:43.146356 novelai_python-0.4.9/tests/__init__.py
+-rw-r--r--   0        0        0      870 2024-04-25 03:13:43.146356 novelai_python-0.4.9/tests/test_generate_voice.py
+-rwxr-xr-x   0        0        0     2273 2024-04-25 03:13:43.146356 novelai_python-0.4.9/tests/test_random_prompt.py
+-rwxr-xr-x   0        0        0      422 2024-04-25 03:13:43.146356 novelai_python-0.4.9/tests/test_server.py
+-rwxr-xr-x   0        0        0     1375 2024-04-25 03:13:43.146356 novelai_python-0.4.9/tests/test_server_run.py
+-rwxr-xr-x   0        0        0     2772 2024-04-25 03:13:43.146356 novelai_python-0.4.9/tests/test_upscale.py
+-rwxr-xr-x   0        0        0     2592 2024-04-25 03:13:43.146356 novelai_python-0.4.9/tests/test_user_information.py
+-rwxr-xr-x   0        0        0     3244 2024-04-25 03:13:43.146356 novelai_python-0.4.9/tests/test_user_login.py
+-rwxr-xr-x   0        0        0     3270 2024-04-25 03:13:43.146356 novelai_python-0.4.9/tests/test_user_subscription.py
+-rw-r--r--   0        0        0     4663 1970-01-01 00:00:00.000000 novelai_python-0.4.9/PKG-INFO
```

### Comparing `novelai_python-0.4.8/LICENSE` & `novelai_python-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.8/NOTICE.MD` & `novelai_python-0.4.9/NOTICE.MD`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.8/README.md` & `novelai_python-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.8/pyproject.toml` & `novelai_python-0.4.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "novelai-python"
-version = "0.4.8"
+version = "0.4.9"
 description = "NovelAI Python Binding With Pydantic"
 authors = [
     { name = "sudoskys", email = "coldlando@hotmail.com" },
 ]
 dependencies = [
     "elara>=0.5.5",
     "loguru>=0.7.2",
```

### Comparing `novelai_python-0.4.8/src/novelai_python/__init__.py` & `novelai_python-0.4.9/src/novelai_python/__init__.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.8/src/novelai_python/_exceptions.py` & `novelai_python-0.4.9/src/novelai_python/_exceptions.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.8/src/novelai_python/_response/ai/generate.py` & `novelai_python-0.4.9/src/novelai_python/_response/ai/generate.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.8/src/novelai_python/_response/ai/generate_image.py` & `novelai_python-0.4.9/src/novelai_python/_response/ai/generate_image.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,19 +6,20 @@
 from typing import Tuple, List
 
 from pydantic import BaseModel
 
 from ..schema import RespBase
 
 
-class ImageGenerateResp(RespBase):
-    class RequestParams(BaseModel):
-        endpoint: str
-        raw_request: dict = None
+class RequestParams(BaseModel):
+    endpoint: str
+    raw_request: dict = None
+
 
+class ImageGenerateResp(RespBase):
     meta: RequestParams
     files: List[Tuple[str, bytes]] = None
 
     def query_params(self, key: str, default=None):
         if not isinstance(self.meta.raw_request.get("parameters"), dict):
             raise Exception("Resp parameters is not dict")
         return self.meta.raw_request.get("parameters").get(key, default)
```

### Comparing `novelai_python-0.4.8/src/novelai_python/_response/ai/generate_stream.py` & `novelai_python-0.4.9/src/novelai_python/_response/ai/generate_stream.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.8/src/novelai_python/_response/user/information.py` & `novelai_python-0.4.9/src/novelai_python/_response/user/information.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.8/src/novelai_python/_response/user/subscription.py` & `novelai_python-0.4.9/src/novelai_python/_response/user/subscription.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.8/src/novelai_python/credential/ApiToken.py` & `novelai_python-0.4.9/src/novelai_python/credential/ApiToken.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.8/src/novelai_python/credential/JwtToken.py` & `novelai_python-0.4.9/src/novelai_python/credential/JwtToken.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.8/src/novelai_python/credential/UserAuth.py` & `novelai_python-0.4.9/src/novelai_python/credential/UserAuth.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.8/src/novelai_python/sdk/__init__.py` & `novelai_python-0.4.9/src/novelai_python/sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.8/src/novelai_python/sdk/ai/LICENSE` & `novelai_python-0.4.9/src/novelai_python/sdk/ai/LICENSE`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.8/src/novelai_python/sdk/ai/generate/__init__.py` & `novelai_python-0.4.9/src/novelai_python/sdk/ai/generate/__init__.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.8/src/novelai_python/sdk/ai/generate/_const.py` & `novelai_python-0.4.9/src/novelai_python/sdk/ai/generate/_const.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.8/src/novelai_python/sdk/ai/generate/_enum.py` & `novelai_python-0.4.9/src/novelai_python/sdk/ai/generate/_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Description: Enum class for TextLLMModel
 from enum import Enum
-from typing import List, Dict
+from typing import List
 
 
 class TextLLMModel(Enum):
     """
     Enum class for TextLLMModel
     """
     Sigurd = "6B-v4"
```

### Comparing `novelai_python-0.4.8/src/novelai_python/sdk/ai/generate/_preset.py` & `novelai_python-0.4.9/src/novelai_python/sdk/ai/generate/_preset.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.8/src/novelai_python/sdk/ai/generate_image/__init__.py` & `novelai_python-0.4.9/src/novelai_python/sdk/ai/generate_image/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from tenacity import retry, stop_after_attempt, wait_random, retry_if_exception
 from typing_extensions import override
 
 from ._const import len_values, tempmin_value, sm_value, dyn_value, map_value
 from ._enum import Model, Sampler, NoiseSchedule, ControlNetModel, Action, UCPreset, INPAINTING_MODEL_LIST
 from ...schema import ApiBaseModel
 from ...._exceptions import APIError, AuthError, ConcurrentGenerationError, SessionHttpError
-from ...._response.ai.generate_image import ImageGenerateResp
+from ...._response.ai.generate_image import ImageGenerateResp, RequestParams
 from ....credential import CredentialBase
 from ....utils import try_jsonfy
 
 
 def is_multiple_of_01(num, precision=1e-10):
     remainder = num % 0.01
     return abs(remainder) < precision or abs(0.01 - remainder) < precision
@@ -449,15 +449,15 @@
                             2.951823174884865E-6 * resolution
                             + 5.753298233447344E-7 * resolution * steps
                         )
                         * smea_factor
                 )
         per_sample = max(math.ceil(per_sample * strength), 2)
 
-        if uncond_scale != 1.0:
+        if int(uncond_scale) != 1:
             per_sample = math.ceil(per_sample * 1.3)
 
         return per_sample * n_samples
 
     @classmethod
     def build(cls,
               prompt: str,
@@ -751,15 +751,15 @@
                         code=response.status_code,
                         response=try_jsonfy(response.content)
                     )
                 for filename in file_list:
                     data = zip_file.read(filename)
                     unzip_content.append((filename, data))
             return ImageGenerateResp(
-                meta=ImageGenerateResp.RequestParams(
+                meta=RequestParams(
                     endpoint=self.base_url,
                     raw_request=request_data,
                 ),
                 files=unzip_content
             )
         except curl_cffi.requests.errors.RequestsError as exc:
             logger.exception(exc)
```

### Comparing `novelai_python-0.4.8/src/novelai_python/sdk/ai/generate_image/_const.py` & `novelai_python-0.4.9/src/novelai_python/sdk/ai/generate_image/_const.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.8/src/novelai_python/sdk/ai/generate_image/_enum.py` & `novelai_python-0.4.9/src/novelai_python/sdk/ai/generate_image/_enum.py`

 * *Files 14% similar despite different names*

```diff
@@ -89,33 +89,38 @@
     RES_1920_1088 = (1920, 1088)
 
 
 class Model(Enum):
     NAI_DIFFUSION_3 = "nai-diffusion-3"
     NAI_DIFFUSION_3_INPAINTING = "nai-diffusion-3-inpainting"
 
+    NAI_DIFFUSION_FURRY_3 = "nai-diffusion-furry-3"
+    NAI_DIFFUSION_FURRY_3_INPAINTING = "nai-diffusion-furry-3-inpainting"
+
     NAI_DIFFUSION = "nai-diffusion"
     NAI_DIFFUSION_2 = "nai-diffusion-2"
     NAI_DIFFUSION_INPAINTING = "nai-diffusion-inpainting"
 
     SAFE_DIFFUSION = "safe-diffusion"
     SAFE_DIFFUSION_INPAINTING = "safe-diffusion-inpainting"
 
     NAI_DIFFUSION_FURRY = "nai-diffusion-furry"
     # NAI_DIFFUSION_FURRY2 = "nai-diffusion-furry2"
     FURRY_DIFFUSION_INPAINTING = "furry-diffusion-inpainting"
 
     CUSTOM = "custom"
 
 
-INPAINTING_MODEL_LIST = [Model.NAI_DIFFUSION_3_INPAINTING,
-                         Model.NAI_DIFFUSION_INPAINTING,
-                         Model.SAFE_DIFFUSION_INPAINTING,
-                         Model.FURRY_DIFFUSION_INPAINTING
-                         ]
+INPAINTING_MODEL_LIST = [
+    Model.NAI_DIFFUSION_3_INPAINTING,
+    Model.NAI_DIFFUSION_INPAINTING,
+    Model.SAFE_DIFFUSION_INPAINTING,
+    Model.FURRY_DIFFUSION_INPAINTING,
+    Model.NAI_DIFFUSION_FURRY_3_INPAINTING
+]
 
 PROMOTION = {
     "Stable Diffusion 1D44365E": Model.SAFE_DIFFUSION,
     "Stable Diffusion F4D50568": Model.SAFE_DIFFUSION,
     "Stable Diffusion 81274D13": Model.NAI_DIFFUSION,
     "Stable Diffusion 3B3287AF": Model.NAI_DIFFUSION,
     "Stable Diffusion 4CC42576": Model.NAI_DIFFUSION_FURRY,
@@ -123,8 +128,11 @@
     "Stable Diffusion 1D09D794": Model.NAI_DIFFUSION_FURRY,
     "Stable Diffusion F64BA557": Model.NAI_DIFFUSION_FURRY,
     "Stable Diffusion 49BFAF6A": Model.NAI_DIFFUSION_2,
     "Stable Diffusion F1022D28": Model.NAI_DIFFUSION_2,
     "Stable Diffusion XL B0BDF6C1": Model.NAI_DIFFUSION_3,
     "Stable Diffusion XL C1E1DE52": Model.NAI_DIFFUSION_3,
     "Stable Diffusion XL 8BA2AF87": Model.NAI_DIFFUSION_3,
+    "Stable Diffusion XL 4BE8C60C": Model.NAI_DIFFUSION_FURRY_3,
+    "Stable Diffusion XL C8704949": Model.NAI_DIFFUSION_FURRY_3,
+    "Stable Diffusion XL 9CC2F394": Model.NAI_DIFFUSION_FURRY_3,
 }
```

### Comparing `novelai_python-0.4.8/src/novelai_python/sdk/ai/generate_image/suggest_tags.py` & `novelai_python-0.4.9/src/novelai_python/sdk/ai/generate_image/suggest_tags.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.8/src/novelai_python/sdk/ai/generate_stream.py` & `novelai_python-0.4.9/src/novelai_python/sdk/ai/generate_stream.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.8/src/novelai_python/sdk/ai/generate_voice/__init__.py` & `novelai_python-0.4.9/src/novelai_python/sdk/ai/generate_voice/__init__.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.8/src/novelai_python/sdk/ai/generate_voice/_enum.py` & `novelai_python-0.4.9/src/novelai_python/sdk/ai/generate_voice/_enum.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.8/src/novelai_python/sdk/ai/upscale.py` & `novelai_python-0.4.9/src/novelai_python/sdk/ai/upscale.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.8/src/novelai_python/sdk/schema.py` & `novelai_python-0.4.9/src/novelai_python/sdk/schema.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.8/src/novelai_python/sdk/user/information.py` & `novelai_python-0.4.9/src/novelai_python/sdk/user/information.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.8/src/novelai_python/sdk/user/login.py` & `novelai_python-0.4.9/src/novelai_python/sdk/user/login.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.8/src/novelai_python/sdk/user/subscription.py` & `novelai_python-0.4.9/src/novelai_python/sdk/user/subscription.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.8/src/novelai_python/server.py` & `novelai_python-0.4.9/src/novelai_python/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -222,15 +222,19 @@
         opus: bool = False,
         version: Union[Literal["v2", "v1"], str] = "v2",
         current_token: str = Depends(get_current_token)
 ):
     """
     生成图片
     :param current_token: Authorization
-    :param req: GenerateImageInfer
+    :param text: str
+    :param voice: int
+    :param seed: Optional[str]
+    :param opus: bool
+    :param version: Union[Literal["v2", "v1"], str]
     :return:
     """
     try:
         req = VoiceGenerate(text=text, voice=voice, seed=seed, opus=opus, version=version)
         _result = await req.request(session=get_session(current_token))
         return StreamingResponse(io.BytesIO(_result.audio), media_type='audio/mpeg', headers={
             'Content-Disposition': 'attachment;filename=audio.mp3'
```

### Comparing `novelai_python-0.4.8/src/novelai_python/tokenizer/NOTICE.MD` & `novelai_python-0.4.9/src/novelai_python/tokenizer/NOTICE.MD`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.8/src/novelai_python/tokenizer/__init__.py` & `novelai_python-0.4.9/src/novelai_python/tokenizer/__init__.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.8/src/novelai_python/tokenizer/bpe_simple_vocab_16e6.txt.gz` & `novelai_python-0.4.9/src/novelai_python/tokenizer/bpe_simple_vocab_16e6.txt.gz`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.8/src/novelai_python/tokenizer/gpt2-genji_tokenizer.json` & `novelai_python-0.4.9/src/novelai_python/tokenizer/gpt2-genji_tokenizer.json`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.8/src/novelai_python/tokenizer/gpt2_tokenizer.json` & `novelai_python-0.4.9/src/novelai_python/tokenizer/gpt2_tokenizer.json`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.8/src/novelai_python/tokenizer/nerdstash_v1.model` & `novelai_python-0.4.9/src/novelai_python/tokenizer/nerdstash_v1.model`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.8/src/novelai_python/tokenizer/nerdstash_v2.model` & `novelai_python-0.4.9/src/novelai_python/tokenizer/nerdstash_v2.model`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.8/src/novelai_python/tokenizer/novelai.model` & `novelai_python-0.4.9/src/novelai_python/tokenizer/novelai.model`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.8/src/novelai_python/tokenizer/novelai_v2.model` & `novelai_python-0.4.9/src/novelai_python/tokenizer/novelai_v2.model`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.8/src/novelai_python/tokenizer/pile_tokenizer.json` & `novelai_python-0.4.9/src/novelai_python/tokenizer/pile_tokenizer.json`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.8/src/novelai_python/tokenizer/simple_tokenizer.py` & `novelai_python-0.4.9/src/novelai_python/tokenizer/simple_tokenizer.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.8/src/novelai_python/tool/image_metadata/__init__.py` & `novelai_python-0.4.9/src/novelai_python/tool/image_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.8/src/novelai_python/tool/image_metadata/lsb_extractor.py` & `novelai_python-0.4.9/src/novelai_python/tool/image_metadata/lsb_extractor.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.8/src/novelai_python/tool/image_metadata/lsb_injector.py` & `novelai_python-0.4.9/src/novelai_python/tool/image_metadata/lsb_injector.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.8/src/novelai_python/tool/paint_mask/__init__.py` & `novelai_python-0.4.9/src/novelai_python/tool/paint_mask/__init__.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.8/src/novelai_python/tool/random_prompt/__init__.py` & `novelai_python-0.4.9/src/novelai_python/tool/random_prompt/__init__.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.8/src/novelai_python/tool/random_prompt/tag.py` & `novelai_python-0.4.9/src/novelai_python/tool/random_prompt/tag.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.8/src/novelai_python/tool/random_prompt/tag_character.py` & `novelai_python-0.4.9/src/novelai_python/tool/random_prompt/tag_character.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.8/src/novelai_python/tool/random_prompt/tag_nsfw.py` & `novelai_python-0.4.9/src/novelai_python/tool/random_prompt/tag_nsfw.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.8/src/novelai_python/utils/__init__.py` & `novelai_python-0.4.9/src/novelai_python/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.8/src/novelai_python/utils/encode.py` & `novelai_python-0.4.9/src/novelai_python/utils/encode.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.8/src/novelai_python/utils/useful.py` & `novelai_python-0.4.9/src/novelai_python/utils/useful.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.8/tests/test_generate_voice.py` & `novelai_python-0.4.9/tests/test_generate_voice.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.8/tests/test_random_prompt.py` & `novelai_python-0.4.9/tests/test_random_prompt.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.8/tests/test_server_run.py` & `novelai_python-0.4.9/tests/test_server_run.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.8/tests/test_upscale.py` & `novelai_python-0.4.9/tests/test_upscale.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.8/tests/test_user_information.py` & `novelai_python-0.4.9/tests/test_user_information.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.8/tests/test_user_login.py` & `novelai_python-0.4.9/tests/test_user_login.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.8/tests/test_user_subscription.py` & `novelai_python-0.4.9/tests/test_user_subscription.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.8/PKG-INFO` & `novelai_python-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: novelai-python
-Version: 0.4.8
+Version: 0.4.9
 Summary: NovelAI Python Binding With Pydantic
 Author-Email: sudoskys <coldlando@hotmail.com>
 License: Apache License 2.0
 Project-URL: Repository, https://github.com/LlmKira/novelai-python/
 Project-URL: Issues, https://github.com/LlmKira/novelai-python/issues
 Requires-Python: >=3.9
 Requires-Dist: elara>=0.5.5
```

