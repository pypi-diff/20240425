# Comparing `tmp/miditok-3.0.2.tar.gz` & `tmp/miditok-3.0.3.tar.gz`

## Comparing `miditok-3.0.2.tar` & `miditok-3.0.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 miditok-3.0.2/miditok/__init__.py
--rw-r--r--   0        0        0     2877 2020-02-02 00:00:00.000000 miditok-3.0.2/miditok/bpe_iterator.py
--rw-r--r--   0        0        0    31558 2020-02-02 00:00:00.000000 miditok-3.0.2/miditok/classes.py
--rw-r--r--   0        0        0    15941 2020-02-02 00:00:00.000000 miditok-3.0.2/miditok/constants.py
--rw-r--r--   0        0        0   136294 2020-02-02 00:00:00.000000 miditok-3.0.2/miditok/midi_tokenizer.py
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 miditok-3.0.2/miditok/data_augmentation/__init__.py
--rw-r--r--   0        0        0    17565 2020-02-02 00:00:00.000000 miditok-3.0.2/miditok/data_augmentation/data_augmentation.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 miditok-3.0.2/miditok/pytorch_data/__init__.py
--rw-r--r--   0        0        0     6188 2020-02-02 00:00:00.000000 miditok-3.0.2/miditok/pytorch_data/collators.py
--rw-r--r--   0        0        0    12536 2020-02-02 00:00:00.000000 miditok-3.0.2/miditok/pytorch_data/datasets.py
--rw-r--r--   0        0        0    14978 2020-02-02 00:00:00.000000 miditok-3.0.2/miditok/pytorch_data/split_midi_utils.py
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 miditok-3.0.2/miditok/tokenizations/__init__.py
--rw-r--r--   0        0        0    33853 2020-02-02 00:00:00.000000 miditok-3.0.2/miditok/tokenizations/cp_word.py
--rw-r--r--   0        0        0    32920 2020-02-02 00:00:00.000000 miditok-3.0.2/miditok/tokenizations/midi_like.py
--rw-r--r--   0        0        0    23233 2020-02-02 00:00:00.000000 miditok-3.0.2/miditok/tokenizations/mmm.py
--rw-r--r--   0        0        0    20524 2020-02-02 00:00:00.000000 miditok-3.0.2/miditok/tokenizations/mumidi.py
--rw-r--r--   0        0        0    20971 2020-02-02 00:00:00.000000 miditok-3.0.2/miditok/tokenizations/octuple.py
--rw-r--r--   0        0        0    31919 2020-02-02 00:00:00.000000 miditok-3.0.2/miditok/tokenizations/remi.py
--rw-r--r--   0        0        0    15096 2020-02-02 00:00:00.000000 miditok-3.0.2/miditok/tokenizations/structured.py
--rw-r--r--   0        0        0    22215 2020-02-02 00:00:00.000000 miditok-3.0.2/miditok/tokenizations/tsd.py
--rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 miditok-3.0.2/miditok/utils/__init__.py
--rw-r--r--   0        0        0    38500 2020-02-02 00:00:00.000000 miditok-3.0.2/miditok/utils/utils.py
--rw-r--r--   0        0        0     3511 2020-02-02 00:00:00.000000 miditok-3.0.2/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 miditok-3.0.2/LICENSE
--rw-r--r--   0        0        0     7187 2020-02-02 00:00:00.000000 miditok-3.0.2/README.md
--rw-r--r--   0        0        0     5644 2020-02-02 00:00:00.000000 miditok-3.0.2/pyproject.toml
--rw-r--r--   0        0        0     8858 2020-02-02 00:00:00.000000 miditok-3.0.2/PKG-INFO
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 miditok-3.0.3/miditok/__init__.py
+-rw-r--r--   0        0        0    36469 2020-02-02 00:00:00.000000 miditok-3.0.3/miditok/classes.py
+-rw-r--r--   0        0        0    16410 2020-02-02 00:00:00.000000 miditok-3.0.3/miditok/constants.py
+-rw-r--r--   0        0        0   152188 2020-02-02 00:00:00.000000 miditok-3.0.3/miditok/midi_tokenizer.py
+-rw-r--r--   0        0        0     3446 2020-02-02 00:00:00.000000 miditok-3.0.3/miditok/tokenizer_training_iterator.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 miditok-3.0.3/miditok/data_augmentation/__init__.py
+-rw-r--r--   0        0        0    17993 2020-02-02 00:00:00.000000 miditok-3.0.3/miditok/data_augmentation/data_augmentation.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 miditok-3.0.3/miditok/pytorch_data/__init__.py
+-rw-r--r--   0        0        0     6398 2020-02-02 00:00:00.000000 miditok-3.0.3/miditok/pytorch_data/collators.py
+-rw-r--r--   0        0        0    13467 2020-02-02 00:00:00.000000 miditok-3.0.3/miditok/pytorch_data/datasets.py
+-rw-r--r--   0        0        0    15275 2020-02-02 00:00:00.000000 miditok-3.0.3/miditok/pytorch_data/split_utils.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 miditok-3.0.3/miditok/tokenizations/__init__.py
+-rw-r--r--   0        0        0    34063 2020-02-02 00:00:00.000000 miditok-3.0.3/miditok/tokenizations/cp_word.py
+-rw-r--r--   0        0        0    33406 2020-02-02 00:00:00.000000 miditok-3.0.3/miditok/tokenizations/midi_like.py
+-rw-r--r--   0        0        0     8480 2020-02-02 00:00:00.000000 miditok-3.0.3/miditok/tokenizations/mmm.py
+-rw-r--r--   0        0        0    20525 2020-02-02 00:00:00.000000 miditok-3.0.3/miditok/tokenizations/mumidi.py
+-rw-r--r--   0        0        0    21179 2020-02-02 00:00:00.000000 miditok-3.0.3/miditok/tokenizations/octuple.py
+-rw-r--r--   0        0        0    32677 2020-02-02 00:00:00.000000 miditok-3.0.3/miditok/tokenizations/remi.py
+-rw-r--r--   0        0        0    15685 2020-02-02 00:00:00.000000 miditok-3.0.3/miditok/tokenizations/structured.py
+-rw-r--r--   0        0        0    22761 2020-02-02 00:00:00.000000 miditok-3.0.3/miditok/tokenizations/tsd.py
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 miditok-3.0.3/miditok/utils/__init__.py
+-rw-r--r--   0        0        0    39617 2020-02-02 00:00:00.000000 miditok-3.0.3/miditok/utils/utils.py
+-rw-r--r--   0        0        0     3511 2020-02-02 00:00:00.000000 miditok-3.0.3/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 miditok-3.0.3/LICENSE
+-rw-r--r--   0        0        0     7295 2020-02-02 00:00:00.000000 miditok-3.0.3/README.md
+-rw-r--r--   0        0        0     5522 2020-02-02 00:00:00.000000 miditok-3.0.3/pyproject.toml
+-rw-r--r--   0        0        0     8966 2020-02-02 00:00:00.000000 miditok-3.0.3/PKG-INFO
```

### Comparing `miditok-3.0.2/miditok/__init__.py` & `miditok-3.0.3/miditok/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,32 +3,34 @@
 
 Here we only import tokenizer classes and submodules.
 """
 
 from miditok import data_augmentation
 
 from .classes import Event, TokenizerConfig, TokSequence
-from .midi_tokenizer import MIDITokenizer
+from .midi_tokenizer import MusicTokenizer
 from .tokenizations import (
     MMM,
     REMI,
     TSD,
     CPWord,
     MIDILike,
     MuMIDI,
     Octuple,
     Structured,
 )
+from .tokenizer_training_iterator import TokTrainingIterator
 from .utils import utils
 
 __all__ = [
-    "MIDITokenizer",
+    "MusicTokenizer",
     "Event",
     "TokSequence",
     "TokenizerConfig",
+    "TokTrainingIterator",
     "MIDILike",
     "REMI",
     "TSD",
     "Structured",
     "Octuple",
     "CPWord",
     "MuMIDI",
```

### Comparing `miditok-3.0.2/miditok/bpe_iterator.py` & `miditok-3.0.3/miditok/tokenizer_training_iterator.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,62 +1,80 @@
 """Iterator to be used when training a tokenizer with the 🤗tokenizers library."""
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from symusic import Score
 
-from .constants import MIDI_FILES_EXTENSIONS, MIDI_LOADING_EXCEPTION
+from .classes import TokSequence
+from .constants import SCORE_LOADING_EXCEPTION
 
 if TYPE_CHECKING:
     from collections.abc import Sequence
     from pathlib import Path
 
-    from .midi_tokenizer import MIDITokenizer
+    from .midi_tokenizer import MusicTokenizer
 
 
-class BPEIterator:
+class TokTrainingIterator:
     r"""
-    An iterable class to be used when training a tokenizer with BPE.
+    An iterable class to be used when training a tokenizer.
 
-    It loads MIDI files and tokenize them on the fly, to be used with the Hugging Face
-    tokenizers library to build a vocabulary with BPE.
+    It loads music files (MIDI, abc) and tokenize them on the fly, to be used with the
+    Hugging Face tokenizers library to build a vocabulary with BPE, Unigram or WordPiece
+    models.
 
     :param tokenizer: tokenizer to use for training.
     :param files_paths: sequence of paths of files to load for training.
     """
 
-    def __init__(self, tokenizer: MIDITokenizer, files_paths: Sequence[Path]) -> None:
+    def __init__(
+        self,
+        tokenizer: MusicTokenizer,
+        files_paths: Sequence[Path],
+    ) -> None:
         self.tokenizer = tokenizer
         self.files_paths = files_paths
         self.__iter_count = 0
 
     def load_file(self, path: Path) -> list[str]:
         """
-        Load a MIDI file and convert it to its byte representation.
+        Load a music file and convert it to its byte representation.
 
         :param path: path to the file to load.
         :return: the byte representation of the file.
         """
-        if path.suffix in MIDI_FILES_EXTENSIONS:
-            try:
-                midi = Score(path)
-            except MIDI_LOADING_EXCEPTION:
-                return []
-            token_ids = self.tokenizer(midi)
-            if self.tokenizer.one_token_stream:
-                token_ids = token_ids.ids
-            else:
-                token_ids = [seq.ids for seq in token_ids]
+        # Load and tokenize file
+        try:
+            score = Score(path)
+        except SCORE_LOADING_EXCEPTION:
+            return []
+        # Need to specify `encode_ids=False` as it might be already pretrained
+        tokseq = self.tokenizer(score, encode_ids=False)
+
+        # Split ids if requested
+        if self.tokenizer.config.encode_ids_split in ["bar", "beat"]:
+            if isinstance(tokseq, TokSequence):
+                tokseq = [tokseq]
+
+            new_seqs = []
+            for seq in tokseq:
+                if self.tokenizer.config.encode_ids_split == "bar":
+                    new_seqs += seq.split_per_bars()
+                else:
+                    new_seqs += seq.split_per_beats()
+            tokseq = [seq for seq in new_seqs if len(seq) > 0]
+
+        # Convert ids to bytes for training
+        if isinstance(tokseq, TokSequence):
+            token_ids = tokseq.ids
         else:
-            token_ids = self.tokenizer.load_tokens(path)["ids"]
-
-        # list of str (bytes)
+            token_ids = [seq.ids for seq in tokseq]
         bytes_ = self.tokenizer._ids_to_bytes(token_ids, as_one_str=True)
-        if self.tokenizer.one_token_stream:
+        if isinstance(bytes_, str):
             bytes_ = [bytes_]
 
         return bytes_
 
     def __len__(self) -> int:
         """
         Return the number of files in the training corpus.
@@ -70,15 +88,15 @@
         Convert the ``idx``th file to its byte representation.
 
         :param idx: idx of the file to convert.
         :return: byte representation of the file.
         """
         return self.load_file(self.files_paths[idx])
 
-    def __iter__(self) -> BPEIterator:  # noqa:D105
+    def __iter__(self) -> TokTrainingIterator:  # noqa:D105
         return self
 
     def __next__(self) -> list[str]:  # noqa:D105
         if self.__iter_count >= len(self):
             self.__iter_count = 0
             raise StopIteration
```

### Comparing `miditok-3.0.2/miditok/classes.py` & `miditok-3.0.3/miditok/classes.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Common classes."""
 
 from __future__ import annotations
 
 import json
 import warnings
 from copy import deepcopy
-from dataclasses import dataclass
+from dataclasses import dataclass, replace
 from math import log2
 from pathlib import Path
-from typing import TYPE_CHECKING, Any
+from typing import TYPE_CHECKING, Any, Literal
 
 from numpy import ndarray
 
 from .constants import (
     BEAT_RES,
     BEAT_RES_REST,
     CHORD_MAPS,
@@ -20,15 +20,17 @@
     CHORD_UNKNOWN,
     CURRENT_MIDITOK_VERSION,
     CURRENT_SYMUSIC_VERSION,
     CURRENT_TOKENIZERS_VERSION,
     DELETE_EQUAL_SUCCESSIVE_TEMPO_CHANGES,
     DELETE_EQUAL_SUCCESSIVE_TIME_SIG_CHANGES,
     DRUM_PITCH_RANGE,
+    ENCODE_IDS_SPLIT,
     LOG_TEMPOS,
+    MANDATORY_SPECIAL_TOKENS,
     MAX_PITCH_INTERVAL,
     NUM_TEMPOS,
     NUM_VELOCITIES,
     ONE_TOKEN_STREAM_FOR_PROGRAMS,
     PITCH_BEND_RANGE,
     PITCH_INTERVALS_MAX_TIME_DIST,
     PITCH_RANGE,
@@ -105,28 +107,75 @@
 
     A ``TokSequence`` can represent tokens by their several forms:
     * tokens (list of str): tokens as sequence of strings;
     * ids (list of int), these are the one to be fed to models;
     * events (list of Event): Event objects that can carry time or other information
     useful for debugging;
     * bytes (str): ids are converted into unique bytes, all joined together in a single
-    string. This is used by MidiTok internally for BPE.
+    string. This is used internally by MidiTok for the tokenizer's model (BPE, Unigram,
+    WordPiece).
 
     Bytes are used internally by MidiTok for Byte Pair Encoding.
-    The ``ids_are_bpe_encoded`` attribute tells if ``ids`` is encoded with BPE.
+    The ``are_ids_encoded`` attribute tells if ``ids`` is encoded.
 
-    :py:meth:`miditok.MIDITokenizer.complete_sequence`
+    :py:meth:`miditok.MusicTokenizer.complete_sequence` can be used to complete the
+    non-initialized attributes.
     """
 
     tokens: list[str | list[str]] = None
-    ids: list[int | list[int]] = None  # BPE can be applied on ids
+    ids: list[int | list[int]] = None  # can be encoded with BPE/Unigram/WordPiece
     bytes: str = None  # noqa: A003
     events: list[Event | list[Event]] = None
-    ids_bpe_encoded: bool = False
-    _ids_no_bpe: list[int | list[int]] = None
+    are_ids_encoded: bool = False
+    _ticks_bars: list[int] = None  # slice/add not handled
+    _ticks_beats: list[int] = None  # slice/add not handled
+    _ids_decoded: list[int | list[int]] = None
+
+    def split_per_bars(self) -> list[TokSequence]:
+        """
+        Split the sequence into subsequences corresponding to each bar.
+
+        The method can only be called from sequences properly tokenized, otherwise it
+        will throw an error.
+
+        :return: list of subsequences for each bar.
+        """
+        return self._split_per_ticks(self._ticks_bars)
+
+    def split_per_beats(self) -> list[TokSequence]:
+        """
+        Split the sequence into subsequences corresponding to each beat.
+
+        The method can only be called from sequences properly tokenized, otherwise it
+        will throw an error.
+
+        :return: list of subsequences for each beat.
+        """
+        return self._split_per_ticks(self._ticks_beats)
+
+    def _split_per_ticks(self, ticks: list[int]) -> list[TokSequence]:
+        idxs = [0]
+        ti_prev = 0
+        for bi in range(1, len(ticks)):
+            ti = ti_prev
+            while ti < len(self.events) and self.events[ti].time < ticks[bi]:
+                ti += 1
+            if ti == len(self.events):
+                break
+            idxs.append(ti)
+            ti_prev = ti
+
+        # Split the sequence
+        idxs.append(None)
+        subsequences = [self[idxs[i - 1] : idxs[i]] for i in range(1, len(idxs))]
+        # Remove their _ticks_bars and _ticks_beats
+        for subseq in subsequences:
+            subseq._ticks_bars = subseq._ticks_beats = None
+
+        return subsequences
 
     def __len__(self) -> int:
         """
         Return the length of the sequence.
 
         :return: number of elements in the sequence.
         """
@@ -134,49 +183,66 @@
             return len(self.ids)
         if self.tokens is not None:
             return len(self.tokens)
         if self.events is not None:
             return len(self.events)
         if self.bytes is not None:
             return len(self.bytes)
-        if self._ids_no_bpe is not None:
-            return len(self._ids_no_bpe)
+        if self._ids_decoded is not None:
+            return len(self._ids_decoded)
 
         msg = (
             "This TokSequence seems to not be initialized, all its attributes "
             "are None."
         )
         raise ValueError(msg)
 
-    def __getitem__(self, idx: int) -> int | str | Event:
+    def __getitem__(self, val: int | slice) -> int | str | Event | TokSequence:
         """
-        Return the ``idx``th element of the sequence.
+        Return the ``idx``th element or slice of the sequence.
 
-        It checks by order: ids, tokens, events, bytes.
+        If an integer is providing, it checks by order: ids, tokens, events, bytes.
 
-        :param idx: index of the element to retrieve.
+        :param val: index of the element to retrieve.
         :return: ``idx``th element.
         """
+        if isinstance(val, slice):
+            return self.__slice(val)
+
         if self.ids is not None:
-            return self.ids[idx]
+            return self.ids[val]
         if self.tokens is not None:
-            return self.tokens[idx]
+            return self.tokens[val]
         if self.events is not None:
-            return self.events[idx]
+            return self.events[val]
         if self.bytes is not None:
-            return self.bytes[idx]
-        if self._ids_no_bpe is not None:
-            return self._ids_no_bpe[idx]
+            return self.bytes[val]
+        if self._ids_decoded is not None:
+            return self._ids_decoded[val]
 
         msg = (
             "This TokSequence seems to not be initialized, all its attributes "
             "are None."
         )
         raise ValueError(msg)
 
+    def __slice(self, sli: slice) -> TokSequence:
+        """
+        Slice the ``TokSequence``.
+
+        :param sli: slice object.
+        :return: the slice of the self ``TokSequence``.
+        """
+        seq = replace(self)
+        attributes = ["tokens", "ids", "bytes", "events", "_ids_decoded"]
+        for attr in attributes:
+            if getattr(self, attr):
+                setattr(seq, attr, getattr(self, attr)[sli])
+        return seq
+
     def __eq__(self, other: TokSequence) -> bool:
         r"""
         Check that too sequences are equal.
 
         This is performed by comparing their attributes (ids, tokens...).
         **Both sequences must have at least one common attribute initialized (not None)
         for this method to work, otherwise it will return False.**.
@@ -191,46 +257,89 @@
         for i, attr in enumerate(attributes):
             if getattr(self, attr) is not None and getattr(other, attr) is not None:
                 eq[i] = getattr(self, attr) == getattr(other, attr)
                 one_common_attr = True
 
         return one_common_attr and all(eq)
 
+    def __add__(self, other: TokSequence) -> TokSequence:
+        """
+        Concatenate two ``TokSequence`` objects.
+
+        The `ìds``, ``tokens``, ``events`` and ``bytes`` will be concatenated.
+
+        :param other: other ``TokSequence``.
+        :return: the concatenation of the two sequences.
+        """
+        seq = replace(self)
+        seq += other
+        return seq
+
+    def __iadd__(self, other: TokSequence) -> TokSequence:
+        """
+        Concatenate the self ``TokSequence`` to another one.
+
+        The `ìds``, ``tokens``, ``events`` and ``bytes`` will be concatenated.
+
+        :param other: other ``TokSequence``.
+        :return: self.
+        """
+        if not isinstance(other, TokSequence):
+            msg = (
+                "Addition to a `TokSequence` object can only be performed with other"
+                f"`TokSequence` objects. Received: {other.__class__.__name__}"
+            )
+            raise ValueError(msg)
+        attributes = ["tokens", "ids", "bytes", "events", "_ids_decoded"]
+        for attr in attributes:
+            self_attr, other_attr = getattr(self, attr), getattr(other, attr)
+            if self_attr is not None and other_attr is not None:
+                setattr(self, attr, self_attr + other_attr)
+
+        return self
+
 
 class TokenizerConfig:
     r"""
     Tokenizer configuration, to be used with all tokenizers.
 
-    :param pitch_range: range of MIDI pitches to use. Pitches can take values between
+    :param pitch_range: range of note pitches to use. Pitches can take values between
         0 and 127 (included). The `General MIDI 2 (GM2) specifications
         <https://www.midi.org/specifications-old/item/general-midi-2>`_ indicate the
         **recommended** ranges of pitches per MIDI program (instrument). These
         recommended ranges can also be found in ``miditok.constants``. In all cases,
         the range from 21 to 108 (included) covers all the recommended values. When
-        processing a MIDI, the notes with pitches under or above this range can be
+        processing a MIDI file, the notes with pitches under or above this range can be
         discarded. (default: ``(21, 109)``)
     :param beat_res: beat resolutions, as a dictionary in the form:
         ``{(beat_x1, beat_x2): beat_res_1, (beat_x2, beat_x3): beat_res_2, ...}``.
         The keys are tuples indicating a range of beats, ex 0 to 3 for the first bar,
         and the values are the resolution (in samples per beat) to apply to the ranges,
         ex 8. This allows to use ``Duration`` / ``TimeShift`` tokens of different
         lengths / resolutions. Note: for tokenization with ``Position`` tokens, the
         total number of possible positions will be set at four times the maximum
         resolution given (``max(beat_res.values)``\).
         (default: ``{(0, 4): 8, (4, 12): 4}``)
-    :param num_velocities: number of velocity bins. In the MIDI norm, velocities can
+    :param num_velocities: number of velocity bins. In the MIDI protocol, velocities can
         take up to 128 values (0 to 127). This parameter allows to reduce the number
-        of velocity values. The velocities of the MIDIs resolution will be downsampled
-        to ``num_velocities`` values, equally separated between 0 and 127.
-        (default: ``32``)
-    :param special_tokens: list of special tokens. This must be given as a list of
-        strings, that should represent either the token type alone (e.g. ``PAD``) or
-        the token type and its value separated by an underscore (e.g. ``Genre_rock``).
-        If two or more underscores are given, all but the last one will be replaced
-        with dashes (-). (default: ``["PAD", "BOS", "EOS", "MASK"]``\)
+        of velocity values. The velocities of the file will be downsampled to
+        ``num_velocities`` values, equally spaced between 0 and 127. (default: ``32``)
+    :param special_tokens: list of special tokens. The "PAD" token is required and
+        will be included in the vocabulary anyway if you did not include it in
+        ``special_tokens``. This must be given as a list of strings, that should
+        represent either the token type alone (e.g. ``PAD``) or the token type and its
+        value separated by an underscore (e.g. ``Genre_rock``). If two or more
+        underscores are given, all but the last one will be replaced with dashes (-).
+        (default: ``["PAD", "BOS", "EOS", "MASK"]``\)
+    :param encode_ids_split: allows to split the token ids before encoding them with the
+        tokenizer's model (BPE, Unigram, WordPiece), similarly to how words are split
+        with spaces in text. Doing so, the tokenizer will learn tokens that represent
+        note/musical events successions only occurring within bars or beats. Possible
+        values for this argument are ``"bar"``, ``beat`` or ``no``. (default:
+        ``bar``)
     :param use_chords: will use ``Chord`` tokens, if the tokenizer is compatible. A
         ``Chord`` token indicates the presence of a chord at a certain time step.
         MidiTok uses a chord detection method based on onset times and duration. This
         allows MidiTok to detect precisely chords without ambiguity, whereas most chord
         detection methods in symbolic music based on chroma features can't. Note that
         using chords will increase the tokenization time, especially if you are working
         on music with a high "note density". (default: ``False``)
@@ -244,17 +353,17 @@
         to predict tempo changes. Tempo values are quantized accordingly to the
         ``num_tempos`` and ``tempo_range`` entries in the ``additional_tokens``
         dictionary (default is 32 tempos from 40 to 250). (default: ``False``)
     :param use_time_signatures: will use ``TimeSignature`` tokens, if the tokenizer is
         compatible. ``TimeSignature`` tokens will specify the current time signature.
         Note that :ref:`REMI` adds a ``TimeSignature`` token at the beginning of each
         Bar (i.e. after ``Bar`` tokens), while :ref:`TSD` and :ref:`MIDI-Like` will
-        only represent time signature changes (MIDI messages) as they come. If you want
-        more "recalls" of the current time signature within your token sequences, you
-        can preprocess your MIDI file to add more ``TimeSignatureChange`` objects.
+        only represent time signature changes as they come. If you want more "recalls"
+        of the current time signature within your token sequences, you can preprocess
+        a ``symusic.Score`` object to add more ``symusic.TimeSignature`` objects.
         (default: ``False``)
     :param use_sustain_pedals: will use ``Pedal`` tokens to represent the sustain pedal
         events. In multitrack setting, The value of each ``Pedal`` token will be equal
         to the program of the track. (default: ``False``)
     :param use_pitch_bends: will use ``PitchBend`` tokens. In multitrack setting, a
         ``Program`` token will be added before each ``PitchBend` token.
         (default: ``False``)
@@ -267,24 +376,24 @@
         (default: False)
     :param use_programs: will use ``Program`` tokens to specify the instrument/MIDI
         program of the notes, if the tokenizer is compatible (:ref:`TSD`, :ref:`REMI`,
         :ref:`MIDI-Like`, :ref:`Structured` and :ref:`CPWord`). Use this parameter with
         the ``programs``, ``one_token_stream_for_programs`` and `program_changes`
         arguments. By default, it will prepend a ``Program`` tokens before each
         ``Pitch``/``NoteOn`` token to indicate its associated instrument, and will
-        treat all the tracks of a MIDI as a single sequence of tokens. :ref:`CPWord`,
+        treat all the tracks of a file as a single sequence of tokens. :ref:`CPWord`,
         :ref:`Octuple` and :ref:`MuMIDI` add a ``Program`` tokens with the stacks of
         ``Pitch``, ``Velocity`` and ``Duration`` tokens. The :ref:`Octuple`, :ref:`MMM`
         and :ref:`MuMIDI` tokenizers use natively ``Program`` tokens, this option is
         always enabled. (default: ``False``)
     :param use_pitchdrum_tokens: will use dedicated ``PitchDrum`` tokens for pitches
-        of drums tracks. In the MIDI norm, the pitches of drums tracks corresponds to
-        discrete drum elements (bass drum, high tom, cymbals...) which are unrelated to
-        the pitch value of other instruments/programs. Using dedicated tokens for drums
-        allow to disambiguate this, and is thus recommended. (default: ``True``)
+        of drums tracks. In the MIDI protocol, the pitches of drums tracks corresponds
+        to discrete drum elements (bass drum, high tom, cymbals...) which are unrelated
+        to the pitch value of other instruments/programs. Using dedicated tokens for
+        drums allow to disambiguate this, and is thus recommended. (default: ``True``)
     :param beat_res_rest: the beat resolution of ``Rest`` tokens. It follows the same
         data pattern as the ``beat_res`` argument, however the maximum resolution for
         rests cannot be higher than the highest "global" resolution (``beat_res``).
         Rests are considered complementary to other time tokens (``TimeShift``, ``Bar``
         and ``Position``). If in a given situation, ``Rest`` tokens cannot represent
         time with the exact precision, other time times will complement them.
         (default: ``{(0, 1): 8, (1, 2): 4, (2, 12): 2}``)
@@ -299,65 +408,66 @@
         use this argument. Leave ``None`` to not represent unknown chords.
         (default: ``None``)
     :param num_tempos: number of tempos "bins" to use. (default: ``32``)
     :param tempo_range: range of minimum and maximum tempos within which the bins fall.
         (default: ``(40, 250)``)
     :param log_tempos: will use log scaled tempo values instead of linearly scaled.
         (default: ``False``)
-    :param remove_duplicated_notes: will remove duplicated notes before tokenizing
-        MIDIs. Notes with the same onset time and pitch value will be deduplicated.
+    :param remove_duplicated_notes: will remove duplicated notes before tokenizing.
+        Notes with the same onset time and pitch value will be deduplicated.
         This option will slightly increase the tokenization time. This option will add
-        an extra note sorting step in the MIDI preprocessing, which can increase the
-        overall tokenization time. (default: ``False``)
+        an extra note sorting step in the music file preprocessing, which can increase
+        the overall tokenization time. (default: ``False``)
     :param delete_equal_successive_tempo_changes: setting this option True will delete
-        identical successive tempo changes when preprocessing a MIDI file after loading
-        it. For examples, if a MIDI has two tempo changes for tempo 120 at tick 1000
+        identical successive tempo changes when preprocessing a music file after loading
+        it. For examples, if a file has two tempo changes for tempo 120 at tick 1000
         and the next one is for tempo 121 at tick 1200, during preprocessing the tempo
         values are likely to be downsampled and become identical (120 or 121). If
         that's the case, the second tempo change will be deleted and not tokenized.
         This parameter doesn't apply for tokenizations that natively inject the tempo
         information at recurrent timings (e.g. :ref:`Octuple`). For others, note that
         setting it True might reduce the number of ``Tempo`` tokens and in turn the
         recurrence of this information. Leave it False if you want to have recurrent
-        ``Tempo`` tokens, that you might inject yourself by adding ``TempoChange``
-        objects to your MIDIs. (default: ``False``)
+        ``Tempo`` tokens, that you might inject yourself by adding ``symusic.Tempo``
+        objects to a ``symusic.Score``. (default: ``False``)
     :param time_signature_range: range as a dictionary
         ``{denom_i: [num_i1, ..., num_in]/(min_num_i, max_num_i)}``.
         (default: ``{8: [3, 12, 6], 4: [5, 6, 3, 2, 1, 4]}``)
     :param sustain_pedal_duration: by default, the tokenizer will use ``PedalOff``
         tokens to mark the offset times of pedals. By setting this parameter True, it
         will instead use ``Duration`` tokens to explicitly express their durations. If
         you use this parameter, make sure to configure ``beat_res`` to cover the
         durations you expect. (default: ``False``)
     :param pitch_bend_range: range of the pitch bend to consider, to be given as a
         tuple with the form ``(lowest_value, highest_value, num_of_values)``. There
         will be ``num_of_values`` tokens equally spaced between ``lowest_value` and
         `highest_value``. (default: ``(-8192, 8191, 32)``)
     :param delete_equal_successive_time_sig_changes: setting this option True will
-        delete identical successive time signature changes when preprocessing a MIDI
-        file after loading it. For examples, if a MIDI has two time signature changes
+        delete identical successive time signature changes when preprocessing a music
+        file after loading it. For examples, if a file has two time signature changes
         for 4/4 at tick 1000 and the next one is also 4/4 at tick 1200, the second time
         signature change will be deleted and not tokenized. This parameter doesn't
         apply for tokenizations that natively inject the time signature information at
         recurrent timings (e.g. :ref:`Octuple`). For others, note that setting it
         ``True`` might reduce the number of ``TimeSig`` tokens and in turn the
         recurrence of this information. Leave it ``False`` if you want to have
         recurrent ``TimeSig`` tokens, that you might inject yourself by adding
-        ``TimeSignatureChange`` objects to your MIDIs. (default: ``False``)
+        ``symusic.TimeSignature`` objects to a ``symusic.Score``. (default: ``False``)
     :param programs: sequence of MIDI programs to use. Note that ``-1`` is used and
         reserved for drums tracks. (default: ``list(range(-1, 128))``, from -1 to 127
         included)
     :param one_token_stream_for_programs: when using programs (``use_programs``), this
-        parameters will make the tokenizer treat all the tracks of a MIDI as a single
-        stream of tokens. A ``Program`` token will prepend each ``Pitch``, ``NoteOn``
-        and ``NoteOff`` tokens to indicate their associated program / instrument. Note
-        that this parameter is always set to True for :ref:`MuMIDI` and :ref:`MMM`.
-        Setting it to False will make the tokenizer not use ``Programs``, but will
-        allow to still have ``Program`` tokens in the vocabulary. (default: ``True``)
-    :param program_changes: to be used with ``use_programs``. If given True, the
+        parameters will make the tokenizer serialize all the tracks of a
+        ``symusic.Score`` in a single sequence of tokens. A ``Program`` token will
+        prepend each ``Pitch``, ``NoteOn`` and ``NoteOff`` tokens to indicate their
+        associated program / instrument. Note that this parameter is always set to True
+        for :ref:`MuMIDI` and :ref:`MMM`. Disabling will make the tokenizer not use
+        ``Programs``, but will allow to still have ``Program`` tokens in the vocabulary.
+        (default: ``True``)
+    :param program_changes: to be used with ``use_programs``. If given ``True``, the
         tokenizer will place ``Program`` tokens whenever a note is being played by an
         instrument different from the last one. This mimics the ProgramChange MIDI
         messages. If given False, a ``Program`` token will precede each note tokens
         instead. This parameter only apply for :ref:`REMI`, :ref:`TSD` and
         :ref:`MIDI-Like`. If you set it True while your tokenizer is not int
         ``one_token_stream`` mode, a ``Program`` token at the beginning of each track
         token sequence. (default: ``False``)
@@ -376,14 +486,15 @@
 
     def __init__(
         self,
         pitch_range: tuple[int, int] = PITCH_RANGE,
         beat_res: dict[tuple[int, int], int] = BEAT_RES,
         num_velocities: int = NUM_VELOCITIES,
         special_tokens: Sequence[str] = SPECIAL_TOKENS,
+        encode_ids_split: Literal["bar", "beat", "no"] = ENCODE_IDS_SPLIT,
         use_chords: bool = USE_CHORDS,
         use_rests: bool = USE_RESTS,
         use_tempos: bool = USE_TEMPOS,
         use_time_signatures: bool = USE_TIME_SIGNATURE,
         use_sustain_pedals: bool = USE_SUSTAIN_PEDALS,
         use_pitch_bends: bool = USE_PITCH_BENDS,
         use_programs: bool = USE_PROGRAMS,
@@ -436,38 +547,49 @@
             )
             raise ValueError(msg)
         if use_time_signatures:
             for denominator in time_signature_range:
                 if not log2(denominator).is_integer():
                     msg = (
                         "`time_signature_range` contains an invalid time signature "
-                        "denominator. The MIDI norm only supports powers of 2"
-                        f"denominators. Received {denominator}"
+                        "denominator. MidiTok only supports powers of 2 denominators, "
+                        f"does the MIDI protocol. Received {denominator}."
                     )
                     raise ValueError(msg)
 
         # Global parameters
         self.pitch_range: tuple[int, int] = pitch_range
         self.beat_res: dict[tuple[int, int], int] = beat_res
         self.num_velocities: int = num_velocities
+        self.remove_duplicated_notes = remove_duplicated_notes
+        self.encode_ids_split = encode_ids_split
+
+        # Special tokens
         self.special_tokens: list[str] = []
-        for special_token in special_tokens:
+        for special_token in list(special_tokens) + MANDATORY_SPECIAL_TOKENS:
             parts = special_token.split("_")
             if len(parts) == 1:
                 parts.append("None")
             elif len(parts) > 2:
                 parts = ["-".join(parts[:-1]), parts[-1]]
                 warnings.warn(
                     f"miditok.TokenizerConfig: special token {special_token} must"
                     " contain one underscore (_).This token will be saved as"
                     f" {'_'.join(parts)}.",
                     stacklevel=2,
                 )
-            self.special_tokens.append("_".join(parts))
-        self.remove_duplicated_notes = remove_duplicated_notes
+            token = "_".join(parts)
+            if token not in self.special_tokens:
+                self.special_tokens.append(token)
+            else:
+                warnings.warn(
+                    f"The special token {token} is present twice in your configuration."
+                    f" Skipping its duplicated occurrence.",
+                    stacklevel=2,
+                )
 
         # Additional token types params, enabling additional token types
         self.use_chords: bool = use_chords
         self.use_rests: bool = use_rests
         self.use_tempos: bool = use_tempos
         self.use_time_signatures: bool = use_time_signatures
         self.use_sustain_pedals: bool = use_sustain_pedals
@@ -569,16 +691,15 @@
 
         :param input_dict: Dictionary that will be used to instantiate the
             configuration object.
         :param kwargs: Additional parameters from which to initialize the
             configuration object.
         :returns: The ``TokenizerConfig`` object instantiated from those parameters.
         """
-        input_dict.update(**input_dict["additional_params"])
-        input_dict.pop("additional_params")
+        input_dict.update(**input_dict.pop("additional_params"))
         for key in IGNORED_CONFIG_KEY_DICT:
             if key in input_dict:
                 input_dict.pop(key)
         return cls(**input_dict, **kwargs)
 
     def to_dict(self, serialize: bool = False) -> dict[str, Any]:
         r"""
@@ -592,25 +713,25 @@
         dict_config = deepcopy(self.__dict__)
         if serialize:
             self.__serialize_dict(dict_config)
         return dict_config
 
     def __serialize_dict(self, dict_: dict) -> None:
         r"""
-        Convert numpy arrays to lists recursively within a dictionary.
+        Recursively convert non-json-serializable values of a dict to lists.
 
         :param dict_: dictionary to serialize
         """
         for key in dict_:
             if isinstance(dict_[key], dict):
                 self.__serialize_dict(dict_[key])
             elif isinstance(dict_[key], ndarray):
                 dict_[key] = dict_[key].tolist()
 
-    def save_to_json(self, out_path: str | Path) -> None:
+    def save_to_json(self, out_path: Path) -> None:
         r"""
         Save a tokenizer configuration object to the `out_path` path.
 
         :param out_path: path to the output configuration JSON file.
         """
         if isinstance(out_path, str):
             out_path = Path(out_path)
@@ -625,15 +746,15 @@
         dict_config["symusic_version"] = CURRENT_SYMUSIC_VERSION
         dict_config["hf_tokenizers_version"] = CURRENT_TOKENIZERS_VERSION
 
         with out_path.open("w") as outfile:
             json.dump(dict_config, outfile, indent=4)
 
     @classmethod
-    def load_from_json(cls, config_file_path: str | Path) -> TokenizerConfig:
+    def load_from_json(cls, config_file_path: Path) -> TokenizerConfig:
         r"""
         Load a tokenizer configuration from the `config_path` path.
 
         :param config_file_path: path to the configuration JSON file to load.
         """
         if isinstance(config_file_path, str):
             config_file_path = Path(config_file_path)
@@ -650,14 +771,22 @@
         dict_config["time_signature_range"] = {
             int(res): beat_range
             for res, beat_range in dict_config["time_signature_range"].items()
         }
 
         return cls.from_dict(dict_config)
 
+    def copy(self) -> TokenizerConfig:
+        """
+        Copy the ``TokSequence``.
+
+        :return: a copy of the ``TokSequence``.
+        """
+        return deepcopy(self)
+
     def __eq__(self, other: TokenizerConfig) -> bool:
         """
         Check two configs are equal.
 
         :param other: other config object to compare.
         :return: `True` if all attributes are equal, `False` otherwise.
         """
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `miditok-3.0.2/miditok/constants.py` & `miditok-3.0.3/miditok/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,42 +3,45 @@
 from importlib.metadata import version
 
 CURRENT_MIDITOK_VERSION = version("miditok")
 CURRENT_TOKENIZERS_VERSION = version("tokenizers")
 CURRENT_SYMUSIC_VERSION = version("symusic")
 
 MIDI_FILES_EXTENSIONS = {".mid", ".midi", ".MID", ".MIDI"}
-MIDI_LOADING_EXCEPTION = (
+ABC_FILES_EXTENSIONS = {".abc", ".ABC"}
+SUPPORTED_MUSIC_FILE_EXTENSIONS = MIDI_FILES_EXTENSIONS | ABC_FILES_EXTENSIONS
+SCORE_LOADING_EXCEPTION = (
     RuntimeError,
     ValueError,
     OSError,
     FileNotFoundError,
     IOError,
     EOFError,
 )
 DEFAULT_TOKENIZER_FILE_NAME = "tokenizer.json"
 
-# Starting id of chr() method for BPE, as the 5 (0 to 4 included) firsts are ignored by
-# 🤗tokenizers. We also skip the 32nd (0x20) (space) as it causes issues when loading a
-# BPE model with spaces in merged.
+# Starting id of chr() method for bytes equivalent of tokens.
+# The  first 5 (0 to 4 included) are ignored by 🤗tokenizers. We also skip the 32nd
+# (0x20) (space) as it is used to split sequences of characters into words.
 # Issue for reference: https://github.com/huggingface/tokenizers/issues/566
 # List of unicode characters: https://www.fileformat.info/info/charset/UTF-8/list.htm
 CHR_ID_START = 33
 
-# MIDI encodings default parameters, used when tokenizing a dataset and using tokens
-# These are the parameters from which a MIDI file will be tokenized
-# the recommended pitches for piano in the GM2 specs are from 21 to 108
+# Default parameters for TokenizerConfig, used when tokenizing a dataset and using
+# tokens. These parameters impact the file preprocessing (downsampling).
+# The recommended pitches for piano in the GM2 specs are from 21 to 108
 PITCH_RANGE = (21, 109)
 BEAT_RES = {(0, 4): 8, (4, 12): 4}  # samples per beat
 # number of velocity bins, velocities values from 0 to 127 will be quantized
 NUM_VELOCITIES = 32
 # default special tokens
 BOS_TOKEN_NAME = "BOS"
 EOS_TOKEN_NAME = "EOS"
 SPECIAL_TOKENS = ["PAD", BOS_TOKEN_NAME, EOS_TOKEN_NAME, "MASK"]
+MANDATORY_SPECIAL_TOKENS = ["PAD"]
 
 USE_CHORDS = False
 USE_RESTS = False
 USE_TEMPOS = False
 USE_TIME_SIGNATURE = False
 USE_SUSTAIN_PEDALS = False
 USE_PITCH_BENDS = False
@@ -109,23 +112,32 @@
 DRUM_PITCH_RANGE = (27, 88)
 
 # Other
 REMOVE_DUPLICATED_NOTES = False
 
 
 # Tokenizers specific parameters
-MMM_DENSITY_BINS_MAX = (10, 20)
+MMM_COMPATIBLE_TOKENIZERS = {"TSD", "REMI", "MIDILike"}
+USE_BAR_END_TOKENS = False  # REMI
 
-# Defaults values when writing new MIDI files
+# Defaults values when writing new files
 TEMPO = 120
 TIME_SIGNATURE = (4, 4)
 KEY_SIGNATURE_KEY = KEY_SIGNATURE_TONALITY = 0  # C major
 DELETE_EQUAL_SUCCESSIVE_TIME_SIG_CHANGES = False
 
-# For MIDI split in DatasetMIDI
+# Tokenizer training
+DEFAULT_TRAINING_MODEL_NAME = "BPE"
+ENCODE_IDS_SPLIT = "bar"
+WORDPIECE_MAX_INPUT_CHARS_PER_WORD_BAR = 400
+WORDPIECE_MAX_INPUT_CHARS_PER_WORD_BEAT = 100
+UNIGRAM_MAX_PIECE_LENGTH = 32
+UNIGRAM_SPECIAL_TOKEN_SUFFIX = "-unigram"
+
+# For file split in DatasetMIDI
 MAX_NUM_FILES_NUM_TOKENS_PER_NOTE = 200
 
 # Used with chords
 PITCH_CLASSES = [
     "C",
     "C#",
     "D",
```

### Comparing `miditok-3.0.2/miditok/midi_tokenizer.py` & `miditok-3.0.3/miditok/midi_tokenizer.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import math
 import sys
 import warnings
 from abc import ABC, abstractmethod
 from collections.abc import Callable, Iterable, Sequence
 from copy import deepcopy
 from pathlib import Path
+from typing import Literal
 
 import numpy as np
 from huggingface_hub import ModelHubMixin as HFHubMixin
 from huggingface_hub import hf_hub_download
 from symusic import (
     ControlChange,
     Note,
@@ -32,51 +33,64 @@
     TimeSignatureTickList,
 )
 
 try:
     from miditoolkit import MidiFile
 except ImportError:
     MidiFile = None
-from tokenizers import Tokenizer as TokenizerFast
-from tokenizers.models import BPE
-from tokenizers.trainers import BpeTrainer
+from tokenizers import AddedToken
+from tokenizers import Tokenizer as _HFTokenizer
+from tokenizers import models as _tok_models
+from tokenizers import trainers as _tok_trainers
 from tqdm import tqdm
 
-from .bpe_iterator import BPEIterator
 from .classes import Event, TokenizerConfig, TokSequence
 from .constants import (
+    ABC_FILES_EXTENSIONS,
     BOS_TOKEN_NAME,
     CHR_ID_START,
     CURRENT_MIDITOK_VERSION,
     CURRENT_SYMUSIC_VERSION,
     CURRENT_TOKENIZERS_VERSION,
     DEFAULT_TOKENIZER_FILE_NAME,
+    DEFAULT_TRAINING_MODEL_NAME,
     EOS_TOKEN_NAME,
-    MIDI_FILES_EXTENSIONS,
-    MIDI_LOADING_EXCEPTION,
     PITCH_CLASSES,
+    SCORE_LOADING_EXCEPTION,
+    SUPPORTED_MUSIC_FILE_EXTENSIONS,
     TEMPO,
     TIME_SIGNATURE,
+    UNIGRAM_MAX_PIECE_LENGTH,
+    UNIGRAM_SPECIAL_TOKEN_SUFFIX,
     UNKNOWN_CHORD_PREFIX,
+    WORDPIECE_MAX_INPUT_CHARS_PER_WORD_BAR,
+    WORDPIECE_MAX_INPUT_CHARS_PER_WORD_BEAT,
 )
+from .tokenizer_training_iterator import TokTrainingIterator
 from .utils import (
     compute_ticks_per_bar,
     convert_ids_tensors_to_list,
     detect_chords,
-    get_midi_programs,
-    get_midi_ticks_per_beat,
+    get_score_programs,
+    get_score_ticks_per_beat,
     merge_same_program_tracks,
     remove_duplicated_notes,
 )
-from .utils.utils import miditoolkit_to_symusic, np_get_closest, tempo_qpm_to_mspq
+from .utils.utils import (
+    add_bar_beats_ticks_to_tokseq,
+    get_deepest_common_subdir,
+    miditoolkit_to_symusic,
+    np_get_closest,
+    tempo_qpm_to_mspq,
+)
 
 
-class MIDITokenizer(ABC, HFHubMixin):
+class MusicTokenizer(ABC, HFHubMixin):
     r"""
-    MIDI tokenizer base class, acting as a common framework.
+    Base music tokenizer class, acting as a common framework.
 
     This is the base class of all tokenizers, containing the common methods and
     attributes. It serves as a framework, and implement most of the tokenization
     global workflow. Child classes should only implement specific methods, for their
     specific behaviors, leaving most of the logic here.
 
     :param tokenizer_config: the tokenizer's configuration, as a
@@ -93,23 +107,23 @@
     ) -> None:
         # Initialize params
         self.config = deepcopy(tokenizer_config)
         # vocab of prime tokens, can be viewed as unique char / bytes
         self._vocab_base = {}
         # the other way, to decode id (int) -> token (str)
         self.__vocab_base_inv = {}
-        # id (int) -> byte (str), as this might not be chr(id) after BPE training
+        # id (int) -> byte (str), as this might not be chr(id) after tokenizer training
         self._vocab_base_id_to_byte = {}
         # byte (str) -> token (str), for basic tokens
         self._vocab_base_byte_to_token = {}
-        # byte(s) -> token(s), for faster BPE decoding
-        self._vocab_bpe_bytes_to_tokens = {}
-        self.has_bpe = False
-        # Fast BPE tokenizer backed with 🤗tokenizers
-        self._bpe_model = None
+        # byte(s) -> token(s), for faster BPE/Unigram/WordPiece decoding
+        self._vocab_learned_bytes_to_tokens = {}
+        # Fast tokenizer model backed with 🤗tokenizers
+        self._model = None
+        self._model_name = None
         # Used in _notes_to_events, especially MIDILike
         self._note_on_off = False
         # Determines how the tokenizer will handle multiple tracks: either each track
         # as a single independent token stream (False), or all the tracks as a single
         # token stream (True).
         self.one_token_stream = False
 
@@ -141,22 +155,22 @@
         # on the maximum number of positions per beat
         # (`self.config.max_num_pos_per_beat`) and the time signatures it supports.
         # The highest note value will ba assigned a tick/beat value equal to
         # `self.config.max_num_pos_per_beat`, the other note values will have a
         # ticks/beat based on this base, i.e. `self.config.max_num_pos_per_beat`
         # multiplied by the factor between each note value and the maximum note value.
         self._tpb_per_ts = self.__create_tpb_per_ts()
-        # Default time division to use when decoding tokens to a MIDI.
+        # Default time division to use when decoding tokens to a ``symusic.Score``.
         # This is left as a class attribute and not a property as the config is not
         # intended to be modified after its creation. Ultimately, this could be
         # ensured by converting TokenizerConfig to a frozen dataclass.
         # It shouldn't be used in place of the real ticks/beat value, which depends on
         # the current time signature denominator. The only exception is for tokenizers
         # which does not support time signature, i.e. which only consider 4/4.
-        # During preprocessing, the MIDI will be resampled to a new time division equal
+        # During preprocessing, the Score will be resampled to a new time division equal
         # to the number of ticks per beat of the lowest time signature denominator it
         # contains. This is done in order to resample as much as possible while keeping
         # most of the accuracy. Some sections might need to be resampled again, when
         # the time signature denominator will be higher (i.e. higher number of absolute
         # ticks per beat).
         # Related: https://github.com/Yikai-Liao/symusic/issues/10
         self.time_division = self._tpb_per_ts[TIME_SIGNATURE[1]]
@@ -203,17 +217,17 @@
 
         # Pitch bends
         self.pitch_bends = np.zeros(1)
         if self.config.use_pitch_bends:
             self.pitch_bends = self.__create_pitch_bends()
 
         # Vocabulary and token types graph
-        if (
-            len(self.vocab) == 0
-        ):  # in case it was not already loaded by load_params, such as with BPE
+        # The vocabulary might have already been created if the tokenizer is being
+        # loaded.
+        if len(self.vocab) == 0:
             self.__create_vocabulary()
         self.tokens_types_graph = self._create_token_types_graph()
         self._add_special_tokens_to_types_graph()
         self._token_types_indexes = {}
         self._update_token_types_indexes()
 
         # For logging
@@ -221,14 +235,27 @@
 
     def _tweak_config_before_creating_voc(self) -> None:
         # called after setting the tokenizer's TokenizerConfig (.config). To be
         # customized by tokenizer classes.
         pass
 
     @property
+    def pad_token_id(self) -> int:
+        """
+        Return the id of the padding token (`PAD_None`). It is usually 0.
+
+        :return: id of the padding token (`PAD_None`).
+        """
+        return (
+            self._vocab_base["PAD_None"]
+            if not self.is_multi_voc
+            else self._vocab_base[0]["PAD_None"]
+        )
+
+    @property
     def vocab(
         self,
     ) -> dict[str, int] | list[dict[str, int]]:  # token (str) to its id (int)
         """
         Get the base vocabulary, as a dictionary mapping tokens (str) to their ids.
 
         The different (hidden / protected) vocabulary attributes of the class are:
@@ -237,181 +264,230 @@
             tokens;
         * ``.__vocab_base_inv`` : Dict[int: str] id -> token - Inverse of
             ``._base_vocab`` , to go the other way;
         * ``._vocab_base_id_to_byte`` : Dict[int: str] id -> byte - Link ids to their
             associated unique bytes;
         * ``._vocab_base_byte_to_token`` : Dict[str: str] - similar as above but for
             tokens;
-        * ``._vocab_bpe_bytes_to_tokens`` : Dict[str: List[str]] byte(s) -> token(s)
-            used to decode BPE;
-        * ``._bpe_model.get_vocab()`` : Dict[str: int] byte -> id - bpe model
-            vocabulary, based on unique bytes.
-
-        Before training the tokenizer with BPE, bytes are obtained by running
-        ``chr(id)`` . After training, if we did start from an empty vocabulary, some
-        base tokens might be removed from ``._vocab_base`` , if they were never found
-        in the training samples. The base vocabulary being changed, ``chr(id)`` would
-        then bind to incorrect bytes (on which byte succession would not have been
-        learned). We register the original id/token/byte association in
-        ``._vocab_base_id_to_byte`` and ``._vocab_base_byte_to_token`` .
+        * ``._vocab_learned_bytes_to_tokens`` : Dict[str: List[str]] byte(s) -> token(s)
+            used to decode BPE/Unigram/WordPiece token ids;
+        * ``._model.get_vocab()`` : Dict[str: int] byte -> id - BPE/Unigram/WordPiece
+            model vocabulary, based on unique bytes.
+
+        Before training the tokenizer, bytes are obtained by running ``chr(id)`` .
+        After training, if we did start from an empty vocabulary, some base tokens might
+        be removed from ``._vocab_base`` , if they were never found in the training
+        samples. The base vocabulary being changed, ``chr(id)`` would then bind to
+        incorrect bytes (on which byte succession would not have been learned). We
+        register the original id/token/byte association in ``._vocab_base_id_to_byte``
+        and ``._vocab_base_byte_to_token`` .
 
         :return: the base vocabulary.
         """
         return self._vocab_base
 
     @property
-    def vocab_bpe(self) -> None | dict[str, int]:  # byte (str) to its id (int)
+    def vocab_model(self) -> None | dict[str, int]:  # byte (str) to its id (int)
         r"""
         Return the vocabulary learnt with BPE.
 
         In case the tokenizer has not been trained with BPE, it returns None.
 
         :return: the BPE model's vocabulary.
         """
-        if not self.has_bpe:
+        if not self.is_trained:
             return None
-        return self._bpe_model.get_vocab()
+        return self._model.get_vocab()
+
+    @property
+    def vocab_size(self) -> int:
+        """
+        Return the size of the vocabulary, by calling ``len(tokenizer)``.
+
+        :return: size of the vocabulary.
+        """
+        return len(self)
 
     @property
     def special_tokens(self) -> list[str]:
         r"""
         Return the special tokens in the vocabulary.
 
         :return: special tokens of the tokenizer
         """
         return self.config.special_tokens
 
     @property
-    def special_tokens_ids(self) -> Sequence[int]:
+    def special_tokens_ids(self) -> list[int]:
         r"""
         Return the ids of the special tokens in the vocabulary.
 
         :return: ids of the special tokens of the tokenizer
         """
         return [self[token] for token in self.special_tokens]
 
+    @property
+    def is_trained(self) -> bool:
+        """
+        Indicate if the tokenizer is trained (``True``).
+
+        :return: a boolean, equal to ``True`` if the tokenizer is trained, ``False``
+            otherwise.
+        """
+        return self._model is not None
+
     def _min_rest(self, ticks_per_beat: int) -> int:
         """
         Return the minimum rest value in ticks, for a given ``ticks_per_beat``.
 
         :param ticks_per_beat: number of ticks in a beat. This depends on the current
-            time signature, and is equal to the MIDI's time division if the denominator
+            time signature, and is equal to the Score's time division if the denominator
             is 4 (quarter).
         :return: minimum rest in ticks.
         """
         if not self.config.use_rests:
             return 0
         return int(self._tpb_to_rest_array[ticks_per_beat][0])
 
-    def preprocess_midi(self, midi: Score) -> Score:
+    def preprocess_score(self, score: Score) -> Score:
         r"""
-        Pre-process a MIDI file to resample its time and events values.
+        Pre-process a ``symusic.Score`` object to resample its time and events values.
 
-        This method is called before parsing a MIDI's contents for tokenization.
+        This method is called before parsing a Score's contents for tokenization.
         Its notes attributes (times, pitches, velocities) will be downsampled and
         sorted, duplicated notes removed, as well as tempos. Empty tracks (with no
-        note) will be removed from the MIDI object. Notes with pitches
+        note) will be removed from the ``symusic.Score`` object. Notes with pitches
         outside ``self.config.pitch_range`` will be deleted.
 
-        :param midi: MIDI object to preprocess.
+        :param score: ``symusic.Score`` object to preprocess.
         """
         # Filter time signatures.
-        # We need to do this first to determine the MIDI's new time division.
+        # We need to do this first to determine the Score's new time division.
         if self.config.use_time_signatures:
-            self._filter_unsupported_time_signatures(midi.time_signatures)
+            self._filter_unsupported_time_signatures(score.time_signatures)
             # We mock the first with 0, even if there are already time signatures. This
-            # is required as if the MIDI only had */2 time signatures, we must make
+            # is required as if the Score only had */2 time signatures, we must make
             # sure the resampling tpq is calculated according to a maximum denom of 4
-            # if the beginning of the MIDI is mocked at 4/4.
-            if len(midi.time_signatures) == 0 or midi.time_signatures[0].time != 0:
-                midi.time_signatures.insert(0, TimeSignature(0, *TIME_SIGNATURE))
+            # if the beginning of the Score is mocked at 4/4.
+            if len(score.time_signatures) == 0 or score.time_signatures[0].time != 0:
+                score.time_signatures.insert(0, TimeSignature(0, *TIME_SIGNATURE))
             # The new time division is chosen depending on its highest time signature
             # denominator, and is equivalent to the highest possible tick/beat ratio.
-            max_midi_denom = max(ts.denominator for ts in midi.time_signatures)
-            new_tpq = int(self.config.max_num_pos_per_beat * max_midi_denom / 4)
+            max_ts_denom = max(ts.denominator for ts in score.time_signatures)
+            new_tpq = int(self.config.max_num_pos_per_beat * max_ts_denom / 4)
         else:
+            # In this case, we set the time signature as being only 4/4.
+            # This is required as we will add the ticks of the bars and beats to the
+            # TokSequence, to split it per bars/beats when encoding the ids.
+            score.time_signatures = TimeSignatureTickList(
+                [TimeSignature(0, *TIME_SIGNATURE)]
+            )
             new_tpq = self.config.max_num_pos_per_beat
 
         # Resample time (not inplace)
-        if midi.ticks_per_quarter != new_tpq:
-            midi = midi.resample(new_tpq, min_dur=1)
+        if score.ticks_per_quarter != new_tpq:
+            score = score.resample(new_tpq, min_dur=1)
 
         # Merge instruments of the same program / inst before preprocessing them.
         # This allows to avoid potential duplicated notes in some multitrack settings
         # This can however mess up chord detections.
         if self.config.use_programs and self.one_token_stream:
-            merge_same_program_tracks(midi.tracks)
+            merge_same_program_tracks(score.tracks)
 
         # Process time signature changes
         # We need to do it before computing the ticks_per_beat sections
-        if self.config.use_time_signatures and len(midi.time_signatures) > 0:
+        if self.config.use_time_signatures and len(score.time_signatures) > 0:
             self._preprocess_time_signatures(
-                midi.time_signatures, midi.ticks_per_quarter
+                score.time_signatures, score.ticks_per_quarter
             )
 
         # Compute resampling ratios to update times of events when several time sig,
         # and ticks per beat ratios.
-        # Resampling factors are used to resample times of events when the MIDI has
+        # Resampling factors are used to resample times of events when the Score has
         # several different time signature denominators.
         # ticks_per_beat ratios are used to adjust durations values according to the
-        # the tokenizer's vocabulary, i.e. *Duration* tokens.
+        # tokenizer's vocabulary, i.e. *Duration* tokens.
         if not self._note_on_off or (
             self.config.use_sustain_pedals and self.config.sustain_pedal_duration
         ):
             if self.config.use_time_signatures:
-                ticks_per_beat = get_midi_ticks_per_beat(midi)
+                ticks_per_beat = get_score_ticks_per_beat(score)
             else:
-                ticks_per_beat = np.array([[midi.end(), midi.ticks_per_quarter]])
+                ticks_per_beat = np.array([[score.end(), score.ticks_per_quarter]])
         else:
             ticks_per_beat = None
         if (
             self.config.use_time_signatures
-            and len({ts.denominator for ts in midi.time_signatures}) > 1
+            and len({ts.denominator for ts in score.time_signatures}) > 1
         ):
-            tpq_resampling_factors = self._get_midi_resampling_factor(midi)
+            tpq_resampling_factors = self._get_score_resampling_factor(score)
         else:
             tpq_resampling_factors = None
 
         # Preprocess track events
-        for t in range(len(midi.tracks) - 1, -1, -1):
-            if len(midi.tracks[t].notes) == 0:
-                del midi.tracks[t]
+        for t in range(len(score.tracks) - 1, -1, -1):
+            # Delete track only there is nothing inside being used
+            if (
+                len(score.tracks[t].notes) == 0
+                and (
+                    not self.config.use_pitch_bends
+                    or len(score.tracks[t].pitch_bends) == 0
+                )
+                and (
+                    not self.config.use_sustain_pedals
+                    or len(score.tracks[t].pedals) == 0
+                )
+            ):
+                del score.tracks[t]
                 continue
-            # Preprocesses notes
-            midi.tracks[t].notes = self._preprocess_notes(
-                midi.tracks[t].notes,
-                midi.tracks[t].is_drum,
-                tpq_resampling_factors,
-                ticks_per_beat,
-            )
 
-            if len(midi.tracks[t].notes) == 0:
-                del midi.tracks[t]
-                continue
+            # Preprocesses notes
+            if len(score.tracks[t].notes) > 0:
+                score.tracks[t].notes = self._preprocess_notes(
+                    score.tracks[t].notes,
+                    score.tracks[t].is_drum,
+                    tpq_resampling_factors,
+                    ticks_per_beat,
+                )
 
             # Resample pitch bend values
-            if self.config.use_pitch_bends and len(midi.tracks[t].pitch_bends) > 0:
-                midi.tracks[t].pitch_bends = self._preprocess_pitch_bends(
-                    midi.tracks[t].pitch_bends, tpq_resampling_factors
+            if self.config.use_pitch_bends and len(score.tracks[t].pitch_bends) > 0:
+                score.tracks[t].pitch_bends = self._preprocess_pitch_bends(
+                    score.tracks[t].pitch_bends, tpq_resampling_factors
                 )
 
             # Resample pedals durations
-            if self.config.use_sustain_pedals and len(midi.tracks[t].pedals) > 0:
-                midi.tracks[t].pedals = self._preprocess_pedals(
-                    midi.tracks[t].pedals, tpq_resampling_factors, ticks_per_beat
+            if self.config.use_sustain_pedals and len(score.tracks[t].pedals) > 0:
+                score.tracks[t].pedals = self._preprocess_pedals(
+                    score.tracks[t].pedals, tpq_resampling_factors, ticks_per_beat
+                )
+
+            # Delete track only there is nothing inside being used
+            if (
+                len(score.tracks[t].notes) == 0
+                and (
+                    not self.config.use_pitch_bends
+                    or len(score.tracks[t].pitch_bends) == 0
+                )
+                and (
+                    not self.config.use_sustain_pedals
+                    or len(score.tracks[t].pedals) == 0
                 )
+            ):
+                del score.tracks[t]
+                continue
 
         # Process tempo changes
         if self.config.use_tempos:
-            midi.tempos = self._preprocess_tempos(midi.tempos, tpq_resampling_factors)
+            score.tempos = self._preprocess_tempos(score.tempos, tpq_resampling_factors)
 
         # We do not change key signature changes, markers and lyrics here as they are
         # not used by MidiTok (yet)
 
-        return midi
+        return score
 
     def _filter_unsupported_time_signatures(
         self, time_signatures: TimeSignatureTickList
     ) -> None:
         """
         Remove time signatures from a list that are unsupported by the tokenizer.
 
@@ -420,17 +496,17 @@
         for i in range(len(time_signatures) - 1, -1, -1):
             if (
                 time_signatures[i].numerator,
                 time_signatures[i].denominator,
             ) not in self.time_signatures:
                 if self._verbose:
                     warnings.warn(
-                        f"The MIDI contains a time signature ({time_signatures[i]}) "
+                        f"The file contains a time signature ({time_signatures[i]}) "
                         f"outside of those supported by the tokenizer ("
-                        f"{self.time_signatures}). You should either discard this MIDI"
+                        f"{self.time_signatures}). You should either discard this file"
                         f" or support this time signature, or alternatively deleting "
                         f"it however if you are using a beat-based tokenizer (REMI) "
                         f"the bars will be incorrectly detected.",
                         stacklevel=2,
                     )
                 del time_signatures[i]
 
@@ -451,21 +527,21 @@
         deleted.
 
         :param notes: notes to preprocess.
         :param is_drums: specifies if the track is drums, as the notes pitches may be
             filtered differently.
         :param resampling_factors: sections of resampling factors, when we need to
             adjust the times of events to a specific ticks/beat value. This is required
-            when the MIDI has time signatures with different denominators. The factors
+            when the file has time signatures with different denominators. The factors
             are given as a numpy array of shape ``(N,2)``, for ``N`` changes of ticks
             per beat, and the second dimension representing the end tick of each
             section and the number of ticks per beat respectively. (default: ``None``)
         :param ticks_per_beat: array indicating the number of ticks per beat per time
             signature denominator section. The numbers of ticks per beat depend on the
-            time signatures of the MIDI being parsed. The array has a shape ``(N,2)``,
+            time signatures of the file being parsed. The array has a shape ``(N,2)``,
             for ``N`` changes of ticks per beat, and the second dimension representing
             the end tick of each section and the number of ticks per beat respectively.
             This argument is not required if
             ``tokenizer.config.sustain_pedal_duration`` is disabled.
             (default: ``None``)
         :param min_duration: minimum duration (in tick) to set to notes that have
             durations of 0 ticks after resampling. (default: ``1``)
@@ -484,14 +560,16 @@
             )
         )[0]
         if len(idx_out_of_pitch_range) > 0:
             mask = np.ones(len(note_soa["time"]), dtype=bool)
             mask[idx_out_of_pitch_range] = False
             for key in note_soa:
                 note_soa[key] = note_soa[key][mask]
+        if len(note_soa["time"]) == 0:
+            return NoteTickList()
 
         # Compute new velocities
         note_soa["velocity"] = np_get_closest(
             self.velocities, np.array(note_soa["velocity"])
         )
 
         # Adjust times if needed
@@ -510,15 +588,15 @@
         elif resampling_factors is not None:
             note_soa["duration"] = self._adjust_time_to_tpb(
                 note_soa["duration"], resampling_factors, min_duration
             )
             self._adjust_offset_spanning_across_time_sig(note_soa, resampling_factors)
 
         # Symusic automatically sorts the notes by (time, duration, pitch) keys when
-        # reading a MIDI file. We hence don't need to sort the notes.
+        # reading a music file. We hence don't need to sort the notes.
         # However, when using `NoteOn`/`NoteOff`, we can encounter note order
         # alterations with the velocity values as they are not sorted on velocities and
         # that the tokens are decoded following a FIFO logic.
         # To alleviate this, a user can sort them before calling the tokenizer.
         # We do not do it here as it is not considered a disturbing issue, and that it
         # would add a significant overhead preprocessing time. This is however done in
         # the tokenization tests of MidiTok for concerned tokenizers in order to keep
@@ -544,21 +622,21 @@
         For tempo changes occurring at the same tick/time, we only keep the last one.
         Consecutive identical tempo changes will be removed if
         ``self.config.delete_equal_successive_tempo_changes`` is True.
 
         :param tempos: tempo changes to resample.
         :param resampling_factors: sections of resampling factors, when we need to
             adjust the times of events to a specific ticks/beat value. This is required
-            when the MIDI has time signatures with different denominators. The factors
+            when the file has time signatures with different denominators. The factors
             are given as a numpy array of shape ``(N,2)``, for ``N`` changes of ticks
             per beat, and the second dimension representing the end tick of each
             section and the number of ticks per beat respectively. (default: ``None``)
         """
         # If we delete the successive equal tempo changes, we need to sort them by time
-        # Fortunately, sorting is already performed by symusic when loading the MIDI.
+        # Fortunately, sorting is already performed by symusic when loading the file.
 
         # Use the default tempo if there is None (shouldn't happen)
         if len(tempos) == 0:
             tempos.insert(0, Tempo(0, self.default_tempo))
             return tempos
 
         tempos_soa = tempos.numpy()
@@ -620,20 +698,20 @@
         Resamples the time signature changes.
 
         Time signature will be delayed to the next bar. See MIDI 1.0 Detailed
         specifications, pages 54 - 56, for more information on delayed time signature
         messages.
         If the ``delete_equal_successive_time_sig_changes`` parameter is set ``True``
         in the tokenizer's configuration, the time signatures must be sorted by time
-        before calling this method. This is done by symusic when loading a MIDI. If
-        this method is called for a MIDI created from another way, make sure they
-        are sorted: ``midi.time_signatures.sort()``.
+        before calling this method. This is done by symusic when loading a file. If
+        this method is called for a file created from another way, make sure they
+        are sorted: ``score.time_signatures.sort()``.
 
         :param time_sigs: time signature changes to quantize.
-        :param time_division: time division in ticks per quarter of the MIDI.
+        :param time_division: time division in ticks per quarter of the Score.
         """
 
         def are_ts_equals(ts1: TimeSignature, ts2: TimeSignature) -> bool:
             return (ts1.numerator, ts1.denominator) == (ts2.numerator, ts2.denominator)
 
         i = 0
         ticks_per_bar = compute_ticks_per_bar(time_sigs[0], time_division)
@@ -695,15 +773,15 @@
 
         Overlapping pitch bends will be deduplicated by keeping the one having the
         highest absolute value at a given tick.
 
         :param pitch_bends: pitch bend events.
         :param resampling_factors: sections of resampling factors, when we need to
             adjust the times of events to a specific ticks/beat value. This is required
-            when the MIDI has time signatures with different denominators. The factors
+            when the Score has time signatures with different denominators. The factors
             are given as a numpy array of shape ``(N,2)``, for ``N`` changes of ticks
             per beat, and the second dimension representing the end tick of each
             section and the number of ticks per beat respectively. (default: ``None``)
         """
         pitch_bends_soa = pitch_bends.numpy()
 
         # Find closest value
@@ -745,21 +823,21 @@
     ) -> PedalTickList:
         r"""
         Resamples the pedals durations.
 
         :param pedals: pedals to preprocess.
         :param resampling_factors: sections of resampling factors, when we need to
             adjust the times of events to a specific ticks/beat value. This is required
-            when the MIDI has time signatures with different denominators. The factors
+            when the Score has time signatures with different denominators. The factors
             are given as a numpy array of shape ``(N,2)``, for ``N`` changes of ticks
             per beat, and the second dimension representing the end tick of each
             section and the number of ticks per beat respectively. (default: ``None``)
         :param ticks_per_beat: array indicating the number of ticks per beat per
             portions. The numbers of ticks per beat depend on the time signatures of
-            the MIDI being parsed. The array has a shape ``(N,2)``, for ``N`` changes
+            the Score being parsed. The array has a shape ``(N,2)``, for ``N`` changes
             of ticks per beat, and the second dimension representing the end tick of
             each portion and the number of ticks per beat respectively. This argument
             is not required if ``tokenizer.config.sustain_pedal_duration`` is disabled.
             (default: ``None``)
         :param min_duration: minimum duration (in tick) to set to notes that have
             durations of 0 ticks after resampling. (default: ``1``)
         """
@@ -884,60 +962,63 @@
         The durations of notes or pedals will be set to the closest ones of those in
         the tokenizer's vocabulary. The new durations are calculated depending on the
         time signature, i.e. number of ticks in a beat.
 
         :param notes_pedals_soa: structure of arrays (soa) of notes or pedals.
         :param ticks_per_beat: array indicating the number of ticks per beat per
             portions. The numbers of ticks per beat depend on the time signatures of
-            the MIDI being parsed. The array has a shape ``(N,2)``, for ``N`` changes
+            the Score being parsed. The array has a shape ``(N,2)``, for ``N`` changes
             of ticks per beat, and the second dimension representing the end tick of
             each portion and the number of ticks per beat respectively.
         """
         # Batch by tpb section
         dur_idx_first = 0
+        tick_last_event = notes_pedals_soa["time"][-1]
         for tpb_idx, (last_tick_tpb, tpb) in enumerate(ticks_per_beat):
             # Get idx of the concerned notes.
             # There shouldn't be equal successive tpb values in ticks_per_beat.
             # If last tpb --> set last note to max_tick to avoid iterating notes
-            if tpb_idx + 1 == len(ticks_per_beat):
-                dur_idx_last = len(notes_pedals_soa["duration"])
+            if tpb_idx + 1 == len(ticks_per_beat) or last_tick_tpb > tick_last_event:
+                dur_idx_last = None
             else:
                 dur_idx_last = dur_idx_first + np.argmax(
                     notes_pedals_soa["time"][dur_idx_first:] >= last_tick_tpb
                 )
             notes_pedals_soa["duration"][dur_idx_first:dur_idx_last] = np_get_closest(
                 self._tpb_to_time_array[tpb],
                 notes_pedals_soa["duration"][dur_idx_first:dur_idx_last],
             )
             dur_idx_first = dur_idx_last
+            if dur_idx_last is None:
+                break
 
-    def _midi_to_tokens(self, midi: Score) -> TokSequence | list[TokSequence]:
+    def _score_to_tokens(self, score: Score) -> TokSequence | list[TokSequence]:
         r"""
-        Convert a **preprocessed** MIDI object to a sequence of tokens.
+        Convert a **preprocessed** ``symusic.Score`` object to a sequence of tokens.
 
         The workflow of this method is as follows: the global events (*Tempo*,
         *TimeSignature*...) and track events (*Pitch*, *Velocity*, *Pedal*...) are
         gathered into a list, then the time events are added. If `one_token_stream` is
         ``True``, all events of all tracks are treated all at once, otherwise the
         events of each track are treated independently.
 
-        :param midi: the MIDI :class:`symusic.Score` object to convert.
+        :param score: the :class:`symusic.Score` object to convert.
         :return: a :class:`miditok.TokSequence` if ``tokenizer.one_token_stream`` is
             ``True``, else a list of :class:`miditok.TokSequence` objects.
         """
         # Create events list
         all_events = []
         if not self.one_token_stream:
-            if len(midi.tracks) == 0:
+            if len(score.tracks) == 0:
                 all_events.append([])
             else:
-                all_events = [[] for _ in range(len(midi.tracks))]
+                all_events = [[] for _ in range(len(score.tracks))]
 
         # Global events (Tempo, TimeSignature)
-        global_events = self._create_midi_events(midi)
+        global_events = self._create_global_events(score)
         if self.one_token_stream:
             all_events += global_events
         else:
             for i in range(len(all_events)):
                 all_events[i] += global_events
 
         # Compute ticks_per_beat sections depending on the time signatures
@@ -945,82 +1026,86 @@
         if (
             not self._note_on_off
             or (self.config.use_sustain_pedals and self.config.sustain_pedal_duration)
             or self.config.use_chords
             or self.config.use_pitch_intervals
         ):
             if self.config.use_time_signatures:
-                ticks_per_beat = get_midi_ticks_per_beat(midi)
+                ticks_per_beat = get_score_ticks_per_beat(score)
             else:
-                ticks_per_beat = np.array([[midi.end(), self.time_division]])
+                ticks_per_beat = np.array([[score.end(), self.time_division]])
         else:
             ticks_per_beat = None
 
         # Adds track tokens
-        for ti, track in enumerate(midi.tracks):
+        for ti, track in enumerate(score.tracks):
             track_events = self._create_track_events(track, ticks_per_beat)
             if self.one_token_stream:
                 all_events += track_events
             else:
                 if self.config.program_changes:
                     # ProgramNoteOff desc to make sure it appears before Pedals and
                     # everything else
+                    program = track.program if not track.is_drum else -1
                     track_events.insert(
-                        0, Event("Program", track.program, 0, desc="ProgramNoteOff")
+                        0, Event("Program", program, 0, desc="ProgramNoteOff")
                     )
                 all_events[ti] += track_events
                 self._sort_events(all_events[ti])
         if self.one_token_stream:
             self._sort_events(all_events)
             # Add ProgramChange (named Program) tokens if requested.
             if self.config.program_changes:
                 self._insert_program_change_events(all_events)
 
         # Add time events
         if self.one_token_stream:
-            all_events = self._add_time_events(all_events, midi.ticks_per_quarter)
+            all_events = self._add_time_events(all_events, score.ticks_per_quarter)
             tok_sequence = TokSequence(events=all_events)
             self.complete_sequence(tok_sequence)
         else:
             tok_sequence = []
             for i in range(len(all_events)):
                 all_events[i] = self._add_time_events(
-                    all_events[i], midi.ticks_per_quarter
+                    all_events[i], score.ticks_per_quarter
                 )
                 tok_sequence.append(TokSequence(events=all_events[i]))
                 self.complete_sequence(tok_sequence[-1])
 
         return tok_sequence
 
     def _sort_events(self, events: list[Event]) -> None:
-        # Can be overridden by subclasses if required (MMM)
+        # Can be overridden by subclasses if required (MIDILike)
         events.sort(key=lambda e: e.time)
 
     def _create_track_events(
         self, track: Track, ticks_per_beat: np.ndarray = None
     ) -> list[Event]:
         r"""
         Extract the tokens/events from a track (``symusic.Track``).
 
         Concerned events are: *Pitch*, *Velocity*, *Duration*, *NoteOn*, *NoteOff* and
         optionally *Chord*, *Pedal* and *PitchBend*.
         **If the tokenizer is using pitch intervals, the notes must be sorted by time
-        then pitch values. This is done in** ``preprocess_midi``.
+        then pitch values. This is done in** ``preprocess_score``.
 
         :param track: ``symusic.Track`` to extract events from.
         :param ticks_per_beat: array indicating the number of ticks per beat per
             section. The numbers of ticks per beat depend on the time signatures of
-            the MIDI being parsed. The array has a shape ``(N,2)``, for ``N`` changes
+            the Score being parsed. The array has a shape ``(N,2)``, for ``N`` changes
             of ticks per beat, and the second dimension representing the end tick of
             each portion and the number of ticks per beat respectively.
             This argument is not required if the tokenizer is not using *Duration*,
             *PitchInterval* or *Chord* tokens. (default: ``None``)
         :return: sequence of corresponding ``Event``s.
         """
-        program = track.program if not track.is_drum else -1
+        if self.config.use_programs:
+            program = track.program if not track.is_drum else -1
+        else:
+            program = 0
         events = []
         # max_time_interval is adjusted depending on the time signature denom / tpb
         max_time_interval = 0
         if self.config.use_pitch_intervals:
             max_time_interval = (
                 ticks_per_beat[0, 1] * self.config.pitch_intervals_max_time_dist
             )
@@ -1253,119 +1338,138 @@
                     (ei, Event("Program", event.program, event.time))
                 )
             previous_type = event.type_
 
         for idx, event in reversed(program_change_events):
             events.insert(idx, event)
 
-    def _create_midi_events(self, midi: Score) -> list[Event]:
+    def _create_global_events(self, score: Score) -> list[Event]:
         r"""
-        Create the *global* MIDI additional tokens: `Tempo` and `TimeSignature`.
+        Create the *global* music tokens: `Tempo` and `TimeSignature`.
 
-        :param midi: midi to extract the events from.
-        :return: list of Events.
+        :param score: ``symusic.Score`` to extract the events from.
+        :return: list of ``miditok.classes.Event``.
         """
         events = []
 
         # First adds time signature tokens if specified
         if self.config.use_time_signatures:
             events += [
                 Event(
                     type_="TimeSig",
                     value=f"{time_sig.numerator}/{time_sig.denominator}",
                     time=time_sig.time,
                 )
-                for time_sig in midi.time_signatures
+                for time_sig in score.time_signatures
             ]
 
         # Adds tempo events if specified
         if self.config.use_tempos:
             events += [
                 Event(
                     type_="Tempo",
                     value=round(tempo.tempo, 2),  # req to handle c++ values
                     time=tempo.time,
                     desc=tempo.tempo,
                 )
-                for tempo in midi.tempos
+                for tempo in score.tempos
             ]
 
         return events
 
     @abstractmethod
     def _add_time_events(self, events: list[Event], time_division: int) -> list[Event]:
         r"""
         Create the time events from a list of global and track events.
 
         Internal method intended to be implemented by child classes.
         The returned sequence is the final token sequence ready to be converted to ids
         to be fed to a model.
 
         :param events: sequence of global and track events to create tokens time from.
-        :param time_division: time division in ticks per quarter of the MIDI being
-            tokenized.
+        :param time_division: time division in ticks per quarter of the
+            ``symusic.Score`` being tokenized.
         :return: the same events, with time events inserted.
         """
         raise NotImplementedError
 
-    def midi_to_tokens(
+    def midi_to_tokens(self, *args, **kwargs) -> Score | list[Score]:  # noqa: D102, ANN002
+        warnings.warn(
+            "miditok: The `midi_to_tokens` method had been renamed `encode`. It is now "
+            "depreciated and will be removed in future updates.",
+            stacklevel=2,
+        )
+        return self.encode(*args, **kwargs)
+
+    def encode(
         self,
-        midi: Score,
-        apply_bpe: bool = True,
+        score: Score | Path,
+        encode_ids: bool = True,
     ) -> TokSequence | list[TokSequence]:
         r"""
-        Tokenize a MIDI file.
+        Tokenize a music file (MIDI/abc), given as a ``symusic.Score`` or a file path.
 
+        You can provide a ``Path`` to the file to tokenize, or a ``symusic.Score``
+        object.
         This method returns a (list of) :class:`miditok.TokSequence`.
 
         If you are implementing your own tokenization by subclassing this class,
-        **override the** protected ``_midi_to_tokens`` **method**.
+        **override the protected** ``_score_to_tokens`` **method**.
 
-        :param midi: the MIDI object to convert.
-        :param apply_bpe: will apply BPE if the tokenizer's vocabulary was trained
-            with. (default: ``True``)
+        :param score: the ``symusic.Score`` object to convert.
+        :param encode_ids: the backbone model (BPE, Unigram, WordPiece) will encode the
+            tokens and compress the sequence. Can only be used if the tokenizer has been
+            trained. (default: ``True``)
         :return: a :class:`miditok.TokSequence` if ``tokenizer.one_token_stream`` is
             ``True``, else a list of :class:`miditok.TokSequence` objects.
         """
-        # Preprocess the MIDI file
-        midi = self.preprocess_midi(midi)
+        # Load the file if a path was given
+        if not isinstance(score, ScoreTick):
+            score = Score(score)
+
+        # Preprocess the music file
+        score = self.preprocess_score(score)
 
         # Tokenize it
-        tokens = self._midi_to_tokens(midi)
-        if apply_bpe and self.has_bpe:
-            self.apply_bpe(tokens)
+        tokens = self._score_to_tokens(score)
+        # Add bar/beat ticks here to TokSeq as they need to be from preprocessed Score
+        add_bar_beats_ticks_to_tokseq(tokens, score)
+
+        # Encode the ids if the tokenizer is trained
+        if encode_ids and self.is_trained:
+            self.encode_token_ids(tokens)
 
         return tokens
 
     def complete_sequence(self, seq: TokSequence, complete_bytes: bool = False) -> None:
         r"""
         Complete (inplace) a :class:`miditok.TokSequence`.
 
         The input sequence can have some of its attributes (``ids``, ``tokens``) not
         initialized (i.e. ``None``). This method will initialize them from the present
         ones. The ``events`` attribute will not be filled as it is only intended for
         debug purpose. The ``bytes`` attribute will be created if ``complete_bytes`` is
-        provided as ``True`` and if the tokenizer is trained with BPE.
+        provided as ``True`` and if the tokenizer has been trained.
 
         :param seq: input :class:`miditok.TokSequence`, must have at least one
             attribute defined.
         :param complete_bytes: will complete the bytes form of each token. This is only
-            applicable if the tokenizer is trained with BPE.
+            applicable if the tokenizer has been trained.
         """
         if seq.tokens is None:
             if seq.events is not None:
                 seq.tokens = self._events_to_tokens(seq.events)
             elif seq.ids is not None:
                 seq.tokens = self._ids_to_tokens(seq.ids)
             elif seq.bytes is not None:
                 seq.tokens = self._bytes_to_tokens(seq.bytes)
         if seq.ids is None:
             seq.ids = self._tokens_to_ids(seq.tokens)
 
-        if complete_bytes and self.has_bpe and seq.bytes is None:
+        if complete_bytes and self.is_trained and seq.bytes is None:
             seq.bytes = self._ids_to_bytes(seq.ids, as_one_str=True)
 
     def _tokens_to_ids(
         self, tokens: Sequence[str | list[str]]
     ) -> list[int | list[int]]:
         r"""
         Convert a list of tokens (str) into their ids format (int).
@@ -1385,16 +1489,17 @@
 
     def _ids_to_tokens(
         self, ids: list[int | list[int]], as_str: bool = True
     ) -> list[str | Event | list[str | Event]]:
         r"""
         Convert a sequence of ids (int) to their tokens format (str or Event).
 
-        **This method will not work with ids encoded with BPE. You will need to decode
-        them first (:py:meth:`miditok.MIDITokenizer.decode_bpe`)**.
+        **This method will not work with ids encoded with the tokenizer's model. You
+        will need to decode them first (
+        :py:meth:`miditok.MusicTokenizer.decode_token_ids`)**.
 
         :param ids: sequence of ids (int) to convert.
         :param as_str: return the tokens as string objects, otherwise Event objects
             (default: True)
         :return: the sequence of corresponding tokens (str or Event).
         """
         tokens = []
@@ -1440,16 +1545,17 @@
     def _ids_to_bytes(
         self, ids: list[int | list[int]], as_one_str: bool = False
     ) -> str | list[str]:
         r"""
         Convert a list of ids into their bytes format.
 
         It can be returned either as a list of bytes or as a unique string of bytes.
-        **This method will not work with ids encoded with BPE. You will need to decode
-        them first (:py:meth:`miditok.MIDITokenizer.decode_bpe`)**.
+        **This method will not work with ids encoded with the tokenizer's model. You
+        will need to decode them first (
+        :py:meth:`miditok.MusicTokenizer.decode_token_ids`)**.
 
         :param ids: token ids (int) to convert.
         :param as_one_str: will return the bytes all concatenated into one string.
             (default: ``False``)
         :return: the tokens converted into strings of unique bytes.
         """
         if len(ids) == 0:
@@ -1473,15 +1579,15 @@
         if len(bytes_) == 0:
             return []
         if isinstance(bytes_[0], list):  # multiple vocabularies
             return [self._bytes_to_tokens(byte_) for byte_ in bytes_]
 
         tokens = []
         for byte_ in bytes_:
-            token_str = self._vocab_bpe_bytes_to_tokens[byte_]
+            token_str = self._vocab_learned_bytes_to_tokens[byte_]
             tokens.append(token_str if as_str else Event(*token_str.split("_")))
         return [tok for toks in tokens for tok in toks]  # flatten
 
     def _convert_sequence_to_tokseq(
         self,
         input_seq: list[int | str | list[int | str]] | np.ndarray,
     ) -> TokSequence | list[TokSequence]:
@@ -1538,135 +1644,147 @@
 
         # Convert to TokSequence
         if not self.one_token_stream and num_io_dims == num_seq_dims:
             seq = []
             for obj in arg[1]:
                 kwarg = {arg[0]: obj}
                 seq.append(TokSequence(**kwarg))
-                if self.has_bpe and seq[-1].ids is not None:
-                    seq[-1].ids_bpe_encoded = self._are_ids_bpe_encoded(seq[-1].ids)
+                if self.is_trained and seq[-1].ids is not None:
+                    seq[-1].are_ids_encoded = self._are_ids_encoded(seq[-1].ids)
         else:  # 1 subscript, one_token_stream and no multi-voc
             kwarg = {arg[0]: arg[1]}
             seq = TokSequence(**kwarg)
-            if self.has_bpe:
-                seq.ids_bpe_encoded = self._are_ids_bpe_encoded(seq.ids)
+            if self.is_trained:
+                seq.are_ids_encoded = self._are_ids_encoded(seq.ids)
 
         return seq
 
-    def _are_ids_bpe_encoded(self, ids: list[int] | np.ndarray) -> bool:
+    def _are_ids_encoded(self, ids: list[int] | np.ndarray) -> bool:
         r"""
-        Tells if a sequence of token ids are encoded with BPE.
+        Indicate if token ids are encoded with a model (BPE, Unigram, WordPiece).
 
         This is performed by checking if any id has a value superior or equal to the
         length of the base vocabulary.
 
         :param ids: ids to check.
-        :return: boolean, ``True`` if ids are encoded with BPE, ``False`` otherwise.
+        :return: boolean, ``True`` if ids are encoded by a model, ``False`` otherwise.
         """
         return np.any(np.array(ids) >= len(self.vocab))
 
     def _preprocess_tokseq_before_decoding(self, tokseq: TokSequence) -> None:
         if tokseq.tokens is None:
-            if tokseq.ids_bpe_encoded:
-                self.decode_bpe(tokseq)
+            if tokseq.are_ids_encoded:
+                self.decode_token_ids(tokseq)
             self.complete_sequence(tokseq)
 
-    def tokens_to_midi(
+    def tokens_to_midi(self, *args, **kwargs) -> Score:  # noqa: D102, ANN002
+        warnings.warn(
+            "miditok: The `tokens_to_midi` method had been renamed `decode`. It is now "
+            "depreciated and will be removed in future updates.",
+            stacklevel=2,
+        )
+        return self.decode(*args, **kwargs)
+
+    def decode(
         self,
         tokens: TokSequence | list[TokSequence] | list[int | list[int]] | np.ndarray,
         programs: list[tuple[int, bool]] | None = None,
-        output_path: str | None = None,
+        output_path: str | Path | None = None,
     ) -> Score:
         r"""
-        Detokenize one or multiple sequences of tokens into a MIDI file.
+        Detokenize one or several sequences of tokens into a ``symusic.Score``.
 
         You can give the tokens sequences either as :class:`miditok.TokSequence`
         objects, lists of integers, numpy arrays or PyTorch/Jax/Tensorflow tensors.
-        The MIDI's time division will be the same as the tokenizer's:
+        The Score's time division will be the same as the tokenizer's:
         ``tokenizer.time_division``.
 
         :param tokens: tokens to convert. Can be either a list of
             :class:`miditok.TokSequence`, a Tensor (PyTorch and Tensorflow are
             supported), a numpy array or a Python list of ints. The first dimension
             represents tracks, unless the tokenizer handle tracks altogether as a
             single token sequence (``tokenizer.one_token_stream == True``).
         :param programs: programs of the tracks. If none is given, will default to
             piano, program 0. (default: ``None``)
         :param output_path: path to save the file. (default: ``None``)
-        :return: the midi object (``symusic.Score``).
+        :return: the ``symusic.Score`` object.
         """
         if not isinstance(tokens, (TokSequence, list)) or (
             isinstance(tokens, list)
             and any(not isinstance(seq, TokSequence) for seq in tokens)
         ):
             tokens = self._convert_sequence_to_tokseq(tokens)
 
         # Preprocess TokSequence(s)
         if isinstance(tokens, TokSequence):
             self._preprocess_tokseq_before_decoding(tokens)
         else:  # list[TokSequence]
             for seq in tokens:
                 self._preprocess_tokseq_before_decoding(seq)
 
-        midi = self._tokens_to_midi(tokens, programs)
+        score = self._tokens_to_score(tokens, programs)
 
         # Create controls for pedals
-        # This is required so that they are saved when the MIDI is dumped, as symusic
+        # This is required so that they are saved when the Score is dumped, as symusic
         # will only write the control messages.
         if self.config.use_sustain_pedals:
-            for track in midi.tracks:
+            for track in score.tracks:
                 for pedal in track.pedals:
                     track.controls.append(ControlChange(pedal.time, 64, 127))
                     track.controls.append(ControlChange(pedal.end, 64, 0))
                 if len(track.pedals) > 0:
                     track.controls.sort()
 
         # Set default tempo and time signatures at tick 0 if not present
-        if len(midi.tempos) == 0 or midi.tempos[0].time != 0:
-            midi.tempos.insert(0, Tempo(0, self.default_tempo))
-        if len(midi.time_signatures) == 0 or midi.time_signatures[0].time != 0:
-            midi.time_signatures.insert(0, TimeSignature(0, *TIME_SIGNATURE))
+        if len(score.tempos) == 0 or score.tempos[0].time != 0:
+            score.tempos.insert(0, Tempo(0, self.default_tempo))
+        if len(score.time_signatures) == 0 or score.time_signatures[0].time != 0:
+            score.time_signatures.insert(0, TimeSignature(0, *TIME_SIGNATURE))
 
-        # Write MIDI file
+        # Write file
         if output_path:
-            Path(output_path).mkdir(parents=True, exist_ok=True)
-            midi.dump_midi(output_path)
-        return midi
+            output_path = Path(output_path)
+            output_path.mkdir(parents=True, exist_ok=True)
+            if output_path.suffix in ABC_FILES_EXTENSIONS:
+                score.dump_abc(output_path)
+            else:
+                score.dump_midi(output_path)
+        return score
 
     @abstractmethod
-    def _tokens_to_midi(
+    def _tokens_to_score(
         self,
         tokens: TokSequence | list[TokSequence],
         programs: list[tuple[int, bool]] | None = None,
     ) -> Score:
         r"""
-        Convert tokens (:class:`miditok.TokSequence`) into a MIDI.
+        Convert tokens (:class:`miditok.TokSequence`) into a ``symusic.Score``.
 
-        This is an internal method called by ``self.tokens_to_midi``, intended to be
-        implemented by classes inheriting :class:`miditok.MidiTokenizer`.
+        This is an internal method called by ``self.decode``, intended to be
+        implemented by classes inheriting :class:`miditok.MusicTokenizer`.
 
         :param tokens: tokens to convert. Can be either a list of
             :class:`miditok.TokSequence` or a list of :class:`miditok.TokSequence`s.
         :param programs: programs of the tracks. If none is given, will default to
             piano, program 0. (default: ``None``)
-        :return: the midi object (:class:`symusic.Score`).
+        :return: the ``symusic.Score`` object.
         """
         raise NotImplementedError
 
     @abstractmethod
     def _create_base_vocabulary(self) -> list[str | list[str]]:
         r"""
         Create the vocabulary, as a list of string tokens.
 
         Each token is given as the form ``"Type_Value"``, with its type and value
         separated with an underscore. Example: ``Pitch_58``.
-        The :class:`miditok.MIDITokenizer` main class will then create the "real"
+        The :class:`miditok.MusicTokenizer` main class will then create the "real"
         vocabulary as a dictionary. Special tokens have to be given when creating the
         tokenizer, and will be added to the vocabulary by
-        :class:`miditok.MIDITokenizer`.
+        :class:`miditok.MusicTokenizer`.
 
         :return: the vocabulary as a list of string.
         """
         raise NotImplementedError
 
     def __create_vocabulary(self) -> None:
         r"""
@@ -1679,17 +1797,18 @@
 
         if isinstance(vocab[0], list):  # multi-voc
             self._vocab_base = [{} for _ in range(len(vocab))]
             self.__vocab_base_inv = [{} for _ in range(len(vocab))]
             for vid in range(len(vocab)):
                 vocab[vid] = self.special_tokens + vocab[vid]
                 for tok in vocab[vid]:
-                    self.add_to_vocab(tok, vid)
+                    self.add_to_vocab(tok, vocab_idx=vid)
         else:
-            vocab = self.special_tokens + vocab
+            for tok in self.special_tokens:
+                self.add_to_vocab(tok, special_token=True)
             for tok in vocab:
                 self.add_to_vocab(tok)
 
     def _add_note_tokens_to_vocab_list(self, vocab: list[str]) -> None:
         # NoteOn + NoteOff
         if self._note_on_off:
             vocab += [f"NoteOn_{i}" for i in range(*self.config.pitch_range)]
@@ -1807,52 +1926,63 @@
             )
         except KeyError:  # no tokens of this type, returns an empty list
             return []
 
     def add_to_vocab(
         self,
         token: str | Event,
+        special_token: bool = False,
         vocab_idx: int | None = None,
         byte_: str | None = None,
-        add_to_bpe_model: bool = False,
+        add_to_model: bool = False,
     ) -> None:
         r"""
         Add an event to the vocabulary. Its id will be the length of the vocab.
 
         :param token: token to add, as a formatted string of the form "Type_Value",
             e.g. Pitch_80, or an Event.
+        :param special_token: whether the token is special. (default: ``False``)
         :param vocab_idx: idx of the vocabulary (in case of embedding pooling).
             (default: ``None``)
-        :param byte_: unique byte associated to the token. This is used when building
-            the vocabulary with fast BPE. If None is given, it will default to
-            ``chr(id_ + CHR_ID_START)`` . (default: ``None``)
-        :param add_to_bpe_model: the token will be added to the bpe_model vocabulary
+        :param byte_: unique byte associated to the token. The associated byte of a
+            token is used to encode-decode ids with the tokenizer's model (BPE, Unigram,
+            WordPiece). If None is given, it will default to ``chr(id_ + CHR_ID_START)``
+            . (default: ``None``)
+        :param add_to_model: the token will be added to the model vocabulary
             too. (default: ``None``)
         """
         token_str = token if isinstance(token, str) else str(token)
 
+        if special_token:
+            parts = token_str.split("_")
+            if len(parts) == 1:
+                parts.append("None")
+            elif len(parts) > 2:
+                parts = ["-".join(parts[:-1]), parts[-1]]
+            token = "_".join(parts)
+            if token not in self.config.special_tokens:
+                self.config.special_tokens.append(token)
+
         if vocab_idx is not None:
             self._vocab_base[vocab_idx][token_str] = len(self._vocab_base[vocab_idx])
             self.__vocab_base_inv[vocab_idx][
                 len(self.__vocab_base_inv[vocab_idx])
             ] = token_str
         else:
-            id_ = len(self._bpe_model.get_vocab()) if self.has_bpe else len(self.vocab)
+            id_ = len(self._model.get_vocab()) if self.is_trained else len(self.vocab)
             self._vocab_base[token_str] = id_
             self.__vocab_base_inv[len(self.__vocab_base_inv)] = token_str
 
-            # For BPE
+            # Byte
             if byte_ is None:
                 byte_ = chr(id_ + CHR_ID_START)
-            self._vocab_base_id_to_byte[
-                id_
-            ] = byte_  # these vocabs are created at init, when the
+            self._vocab_base_id_to_byte[id_] = byte_
             self._vocab_base_byte_to_token[byte_] = token
-            if self._bpe_model is not None and add_to_bpe_model:
-                self._bpe_model.add_tokens([byte_])
+            if self._model is not None and add_to_model:
+                self._model.add_tokens([byte_])
 
     def _create_chords_tokens(self) -> list[str]:
         """
         Create the *Chord* tokens that will populate the base vocabulary.
 
         This protected method is intended to be used when creating the vocabulary.
 
@@ -1892,15 +2022,15 @@
             applicable. (default: ``None``)
         :return: the type of the token, as a string
         """
         token = self.__get_from_voc(id_, vocab_id)
         return token.split("_")[0]
 
     @abstractmethod
-    def _create_token_types_graph(self) -> dict[str, list[str]]:
+    def _create_token_types_graph(self) -> dict[str, set[str]]:
         r"""
         Create a dictionary describing the possible token type successions.
 
         This method is unimplemented and need to be overridden by inheriting classes.
         See other classes (:class:`miditok.REMI._create_token_types_graph`, ...)
         for examples of how to implement it.
 
@@ -1912,27 +2042,27 @@
         r"""
         Add (inplace) special tokens types to the token types graph dictionary.
 
         Two exceptions are made for the special BOS (Beginning of Sequence) and EOS
         (End of Sequence) tokens: No token type can precede a BOS token, and EOS token
         cannot precede any other token.
         """
-        original_token_types = list(self.tokens_types_graph.keys())
+        original_token_types = set(self.tokens_types_graph.keys())
         for special_token in self.config.special_tokens:
             special_token_type = special_token.split("_")[0]
             if special_token_type == EOS_TOKEN_NAME:
-                self.tokens_types_graph[EOS_TOKEN_NAME] = []
+                self.tokens_types_graph[EOS_TOKEN_NAME] = set()
             else:
                 self.tokens_types_graph[special_token_type] = (
-                    original_token_types + list(self.config.special_tokens)
+                    original_token_types | set(self.config.special_tokens)
                 )
 
             if special_token_type != BOS_TOKEN_NAME:
                 for token_type in original_token_types:
-                    self.tokens_types_graph[token_type].append(special_token_type)
+                    self.tokens_types_graph[token_type].add(special_token_type)
 
     def _create_durations_tuples(self) -> list[tuple[int, int, int]]:
         r"""
         Create the possible durations in beat / position units as tuples of intergers.
 
         The tuples follow the form: ``(beat, pos, res)`` where ``beat`` is the number
         of beats, ``pos`` the number of "positions" and ``res`` the beat resolution
@@ -1977,46 +2107,46 @@
         """
         max_denom = max(ts[1] for ts in self.time_signatures)
         return {
             denom: self.config.max_num_pos_per_beat * (max_denom // denom)
             for denom in self.config.time_signature_range
         }
 
-    def _get_midi_resampling_factor(self, midi: Score) -> np.ndarray:
+    def _get_score_resampling_factor(self, score: Score) -> np.ndarray:
         """
-        Compute the portions of numbers of ticks in a beat in a MIDI.
+        Compute the portions of numbers of ticks in a beat in a ``symusic.Score``.
 
         The method returns a numpy array of shape ``(N,2)``, for N ticks-per-beat
         changes, and the second dimension corresponding to the ending tick and the
         number of ticks per beat of the portion.
         **The time signatures must be sorted by time.**
 
-        :param midi: MIDI to analyze.
+        :param score: ``symusic.Score`` to analyze.
         :return: ticks per beat values as a numpy array.
         """
         resampling_factors = [
             [
-                midi.time_signatures[tsi + 1].time,
-                midi.ticks_per_quarter
+                score.time_signatures[tsi + 1].time,
+                score.ticks_per_quarter
                 // (
                     self.config.max_num_pos_per_beat
-                    * (midi.time_signatures[tsi].denominator / 4)
+                    * (score.time_signatures[tsi].denominator / 4)
                 ),
             ]
-            for tsi in range(len(midi.time_signatures) - 1)
+            for tsi in range(len(score.time_signatures) - 1)
         ]
 
-        # Handles the last one up to the max tick of the MIDI
+        # Handles the last one up to the max tick of the Score
         resampling_factors.append(
             [
-                midi.end() + 1,
-                midi.ticks_per_quarter
+                score.end() + 1,
+                score.ticks_per_quarter
                 // (
                     self.config.max_num_pos_per_beat
-                    * (midi.time_signatures[-1].denominator / 4)
+                    * (score.time_signatures[-1].denominator / 4)
                 ),
             ]
         )
 
         # Remove equal successive ones
         for i in range(len(resampling_factors) - 1, 0, -1):
             if resampling_factors[i][1] == resampling_factors[i - 1][1]:
@@ -2118,15 +2248,15 @@
         Convert a time token value of the form beat.position.resolution, in ticks.
 
         This method is used to decode time tokens such as *Duration*, *TimeShift* or
         *Rest*.
 
         :param token_duration: Duration / TimeShift token value.
         :param ticks_per_beat: number of ticks in a beat. This depends on the current
-            time signature, and is equal to the MIDI's time division if the denominator
+            time signature, and is equal to the Score's time division if the denominator
             is 4 (quarter).
         :return: the duration / time-shift in ticks.
         """
         if isinstance(token_duration, str):
             token_duration = tuple(map(int, token_duration.split(".")))
         beat, pos, res = token_duration
         # We don't need to round anything here, as `ticks_per_beat` is always divisible
@@ -2144,15 +2274,15 @@
 
         This method is not used for *Duration* tokens, as their values are rounded to
         the closest values in. It is however used to create successions of time values
         for *TimeShift* and *Rest* tokens.
 
         :param duration: duration in tick to convert.
         :param ticks_per_beat: number of ticks in a beat. This depends on the current
-            time signature, and is equal to the MIDI's time division if the denominator
+            time signature, and is equal to the Score's time division if the denominator
             is 4 (quarter).
         :param rest: the duration is a rest, hence the created tokens will be based on
             the ``self.rests`` values.
         :return: list of associated token values, and the list of the elapsed offset in
             tick for each of these values.
         """
         if rest:
@@ -2255,328 +2385,514 @@
 
         :param token_time_sig: TimeSig token value.
         :return: the numerator and denominator of a time signature.
         """
         numerator, denominator = map(int, token_time_sig.split("/"))
         return numerator, denominator
 
-    def has_midi_time_signatures_not_in_vocab(self, midi: Score) -> bool:
+    def score_has_time_signatures_not_in_vocab(self, score: Score) -> bool:
         r"""
-        Check if a MIDI contains time signatures not supported by the tokenizer.
+        Check if a ``symusic.Score`` contains unsupported time signatures.
 
-        :param midi: MIDI file
-        :return: boolean indicating whether the MIDI can be processed by the tokenizer.
+        :param score: ``symusic.Score`` object.
+        :return: boolean indicating whether the score can be processed by the tokenizer.
         """
         if self.config.use_time_signatures:
-            for time_sig in midi.time_signatures:
+            for time_sig in score.time_signatures:
                 if (
                     time_sig.numerator,
                     time_sig.denominator,
                 ) not in self.time_signatures:
                     return True
         return False
 
-    def learn_bpe(
+    def learn_bpe(self, *args, **kwargs) -> Score:  # noqa: D102, ANN002
+        warnings.warn(
+            "miditok: The `learn_bpe` method had been renamed `train`. It is now "
+            "depreciated and will be removed in future updates.",
+            stacklevel=2,
+        )
+        return self.train(*args, **kwargs)
+
+    def train(
         self,
         vocab_size: int,
+        model: Literal["BPE", "Unigram", "WordPiece"] | _tok_models.Model | None = None,
         iterator: Iterable | None = None,
-        files_paths: list[Path | str] | None = None,
-        start_from_empty_voc: bool = False,
+        files_paths: Sequence[Path] | None = None,
         **kwargs,
     ) -> None:
         r"""
-        Construct the vocabulary from BPE backed by the 🤗tokenizers library.
+        Train the tokenizer to build its vocabulary with BPE, Unigram or WordPiece.
 
         The data used for training can either be given through the ``iterator``
         argument as an iterable object yielding strings, or by ``files_paths`` as a
-        list of paths to MIDI files that will be tokenized.
+        list of paths to music files that will be tokenized.
         You can read the Hugging Face `🤗tokenizers documentation
-        <https://huggingface.co/docs/tokenizers/training_from_memory>`_,
-        `🤗tokenizers API documentation <https://huggingface.co/docs/tokenizers/python/v0.9.4/api/reference.html#>`_
-        and `🤗tokenizers course <https://huggingface.co/course/chapter6/2?fw=pt>`_
-        for more details about the ``iterator`` and input type.
+        <https://huggingface.co/docs/tokenizers/index>`_, and `🤗tokenizers course
+        <https://huggingface.co/course/chapter6/2?fw=pt>`_ for more details about the
+        ``iterator`` and input type.
+
+        **A few considerations must be noted:**
+
+        1. The WordPiece model has a ``max_input_chars_per_word`` attribute, which
+        controls the maximum number of "base tokens" a sequence of ids can contain until
+        it discards and replaces it with a predefined "unknown" token (``unk_token``
+        model attribute). This means that, depending on the base sequence lengths of
+        your files, the tokenizer will likely discard them. This can be addressed by
+        either: 1) splitting the token sequence per bars or beats before encoding ids
+        (highly recommended) into smaller subsequences whose lengths will likely be
+        lower to the model's ``max_input_chars_per_word`` attribute; 2) set the model's
+        ``max_input_chars_per_word`` attribute to a value higher than most of the
+        sequences of ids encoded by the WordPiece model.
+        A high ``max_input_chars_per_word`` value will however drastically increase the
+        encoding and decoding times, reducing its interest. The default values set by
+        MidiTok are ``400`` when splitting ids in bar subsequences and ``100`` when
+        splitting ids in beat subsequences.
+        The ``max_input_chars_per_word`` and ``unk_token`` model attributes can be set
+        by referencing them in the keyword arguments of this method (``kwargs``).
+        2. The Hugging Face Unigram model training `is not 100% deterministic
+        <https://github.com/huggingface/tokenizers/issues/668>`_. As such and if you are
+        using Unigram, you should train your tokenizer only once before using it to save
+        tokenized files or train a model. Otherwise, some token ids might be swapped,
+        resulting in incoherent encodings-decodings.
 
         **The training progress bar will not appear with non-proper terminals.**
         (cf `GitHub issue <https://github.com/huggingface/tokenizers/issues/157>`_ )
 
         :param vocab_size: size of the vocabulary to learn / build.
+        :param model: backbone model to use to train the tokenizer. MidiTok relies on
+            the Hugging Face tokenizers library, and supports the ``BPE``, ``Unigram``
+            and ``WordPiece`` models. This argument can be either a string indicating
+            the model to use, an already initialized model, or ``None`` if you want to
+            retrain a tokenizer already trained. (default: ``None``, default to
+            ``BPE`` if the tokenizer is not already trained, keeps the same model
+            otherwise)
         :param iterator: an iterable object yielding the training data, as lists of
             string. It can be a list or a Generator. This iterator will be passed to
-            the BPE model for training. It musts implement the ``__len__`` method. If
+            the model for training. It musts implement the ``__len__`` method. If
             None is given, you must use the ``tokens_paths`` argument. (default: None)
-        :param files_paths: paths of the files to load and use. They can be either MIDI
-            or tokens (json) files. (default: None)
-        :param start_from_empty_voc: the training will start from an empty base
-            vocabulary. The tokenizer will then have a base vocabulary only based on
-            the unique bytes present in the training data. If you set this argument to
-            True, you should use the tokenizer only with the training data, as new data
-            might contain "unknown" tokens missing from the vocabulary. Comparing this
-            to text, setting this argument to True would create a tokenizer that will
-            only know the characters present in the training data, and would not be
-            compatible/know other characters. This argument can allow to optimize the
-            vocabulary size. If you are unsure about this, leave it to False.
-            (default: False)
-        :param kwargs: any additional argument to pass to the trainer. See the
+        :param files_paths: paths of the music files to load and use. (default: None)
+        :param kwargs: any additional argument to pass to the trainer or model. See the
             `tokenizers docs <https://huggingface.co/docs/tokenizers/api/trainers>`_
             for more details.
         """
+        # Checks the arguments/config are compatible for training
         if self.is_multi_voc:
             warnings.warn(
                 "This tokenizer is based on multiple vocabularies/embedding pooling."
-                "It is therefore not compatible with Byte Pair Encoding (BPE). Skipping"
-                "this method call (learn_bpe).",
+                "It therefore cannot be trained. Skipping `tokenizer.train` function"
+                "call.",
                 stacklevel=2,
             )
             return
         if iterator is None and files_paths is None:
             msg = (
                 "You must give an iterator or a list of paths to tokens to train the"
-                "tokenizer with BPE."
+                "tokenizer."
             )
             raise ValueError(msg)
-
-        if vocab_size <= len(self.vocab):
+        if vocab_size <= len(self._vocab_base):
             warnings.warn(
-                f"vocab_size ({vocab_size}) need to be higher than the size of the"
-                f"current vocabulary ({len(self.vocab)}). Skipping BPE training.",
+                f"miditok - tokenizer.train: `vocab_size` ({vocab_size}) need to be "
+                f"higher than the number of base tokens ({len(self._vocab_base)}). "
+                f"Skipping tokenizer training.",
                 stacklevel=2,
             )
             return
 
         # If no iterator, loads tokens / samples to analyze
         if iterator is None:
-            iterator = BPEIterator(self, files_paths)
+            iterator = TokTrainingIterator(self, files_paths)
+
+        # Define the initial alphabet
+        initial_alphabet = {
+            chr(i + CHR_ID_START): i
+            for tok, i in self._vocab_base.items()
+            if len(tok) == 1  # to discard special tokens with Unigram
+        }
 
-        # Create new tokenizer model
-        if self._bpe_model is None or start_from_empty_voc:
-            num_bytes = (
-                len(self.config.special_tokens)
-                if start_from_empty_voc
-                else len(self._vocab_base)
-            )
-            voc_start = {chr(i + CHR_ID_START): i for i in range(num_bytes)}
-            self._bpe_model = TokenizerFast(
-                BPE(
-                    vocab=voc_start,
-                    merges=[],
-                    dropout=None,
-                    continuing_subword_prefix="",
-                    end_of_word_suffix="",
-                    fuse_unk=False,
+        # Define the model
+        # A `tokenizers.Tokenizer` can feature: a normalizer, pre-tokenizer, model,
+        # post-processor and decoder. We (in MidiTok) are only interested in the
+        # model part, as other components will only perform operations on bytes and are
+        # only relevant for text. MidiTok already "normalize" (preprocess music file),
+        # pre-tokenize (split on bars/beats), and decoding is done differently for each
+        # music tokenization.
+        # Keep current model if `arg` is None:
+        retraining = False
+        if self._model is not None and model is None:
+            tokenizer = self.__reload_hf_tokenizer(self._model)
+            retraining = True
+        # User provided a HF model
+        elif isinstance(model, _tok_models.Model):
+            tokenizer = _HFTokenizer(model)
+        # User provided a str class model
+        elif isinstance(model, str) or model is None:
+            if model is None:  # default
+                model = DEFAULT_TRAINING_MODEL_NAME
+            model_kwargs = {"vocab": [] if model == "Unigram" else initial_alphabet}
+            if model == "BPE":
+                model_kwargs["merges"] = []
+                model_kwargs["continuing_subword_prefix"] = ""
+                model_kwargs["end_of_word_suffix"] = ""
+            elif model == "WordPiece":
+                model_kwargs["unk_token"] = kwargs.pop(
+                    "unk_token", chr(self.pad_token_id + CHR_ID_START)
+                )
+                model_kwargs["continuing_subword_prefix"] = ""
+                model_kwargs["max_input_chars_per_word"] = kwargs.pop(
+                    "max_input_chars_per_word",
+                    WORDPIECE_MAX_INPUT_CHARS_PER_WORD_BAR
+                    if self.config.encode_ids_split == "bar"
+                    else WORDPIECE_MAX_INPUT_CHARS_PER_WORD_BEAT,
                 )
+            tokenizer = _HFTokenizer(getattr(_tok_models, model)(**model_kwargs))
+        else:
+            msg = (
+                "miditok - tokenizer.train: the `model` argument must be a str specify "
+                "the model to use ('BPE', 'Unigram', 'WordPiece'), an already"
+                "initialized model or a `None` to either resume training or default to "
+                f"{DEFAULT_TRAINING_MODEL_NAME}."
             )
+            raise ValueError(msg)
 
-        # Trains the tokenizer
-        special_tokens_bytes = []
-        if len(self.config.special_tokens) > 0:
-            special_tokens_bytes = self._ids_to_bytes(
-                self._tokens_to_ids(self.config.special_tokens)
+        # Converts model to json
+        tokenizer_json = json.loads(tokenizer.to_str())
+        # Remove added tokens for now (uses IDs of tokens)
+        added_tokens = tokenizer_json.pop("added_tokens")
+        model_name = tokenizer_json["model"]["type"]
+
+        # Warnings
+        if retraining and model_name == "Unigram":
+            warnings.warn(
+                "miditok - tokenizer.train: You are retraining a tokenizer with "
+                "Unigram. The Hugging Face Unigram model training is not 100% "
+                "deterministic. As such and if you are using it, you should train your "
+                "tokenizer only once before using it to save tokenized files or train "
+                "a model. Otherwise some token ids might be swapped, resulting in "
+                "incoherent encodings-decodings.",
+                stacklevel=2,
+            )
+        if (
+            model == "WordPiece" or isinstance(model, _tok_models.WordPiece)
+        ) and self.config.encode_ids_split == "no":
+            warnings.warn(
+                "miditok - tokenizer.train: you are training a WordPiece tokenizer "
+                "without splitting the token ids per bars or beats. It is recommended "
+                "do so, as the tokenizer will either 1) replace ids sequences longer "
+                "than its `max_input_chars_per_word` attribute ("
+                f"{tokenizer_json['model']['max_input_chars_per_word']}) with its "
+                f"`unk_token` attribute {tokenizer_json['model']['unk_token']}) thus "
+                "not guaranteeing keeping data integrity when encoding token ids, "
+                "unless you 2) set a large enough `max_input_chars_per_word` attribute "
+                "being greater than the maximum base tokens sequence length of your "
+                "data, which is likely to hurt performances and result in larger"
+                "encoding-decoding time.",
+                stacklevel=2,
             )
-        trainer = BpeTrainer(
+
+        # Get the special tokens from the current tokenizer if none are specified.
+        special_tokens, special_tokens_str = [], []
+        for added_token in added_tokens:
+            special = added_token.pop("special", None)
+            _ = added_token.pop("id", None)
+            if not special:
+                continue
+            special_tokens.append(AddedToken(**added_token))
+            special_tokens_str.append(added_token["content"])
+        # Make sure all the special tokens of the tokenizer are referenced
+        for token_id, token_str in zip(self.special_tokens_ids, self.special_tokens):
+            # For Unigram, we have to make an exception for special tokens. A special
+            # token cannot be just a character from the initial vocabulary. As such, we
+            # prepend and append a special character to the byte of each special token.
+            # Example: Pad_None = "!" becomes "!!!", BOS_None = "#" becomes "!#!"
+            # As a result, each special token will take two "slots" in the vocabulary:
+            # one for its distinct byte and one for its byte combination.
+            special_token_byte = self._vocab_base_id_to_byte[token_id]
+            if model_name == "Unigram" and not token_str.endswith(
+                UNIGRAM_SPECIAL_TOKEN_SUFFIX
+            ):
+                special_char = chr(CHR_ID_START)
+                special_token_byte = f"{special_char}{special_token_byte}{special_char}"
+            if special_token_byte not in special_tokens_str:
+                if model_name == "Unigram":
+                    special_token_str = (
+                        f"{self.__vocab_base_inv[token_id]}"
+                        f"{UNIGRAM_SPECIAL_TOKEN_SUFFIX}"
+                    )
+                    if special_token_str not in self.vocab:
+                        self.add_to_vocab(
+                            special_token_str,
+                            special_token=True,
+                            byte_=special_token_byte,
+                        )
+                special_tokens.append(AddedToken(special_token_byte))
+
+        # Trainer needs to know the end of word / continuing subword thingies in BPE
+        if model_name in ["BPE", "WordPiece"]:
+            if (
+                "continuing_subword_prefix" not in kwargs
+                and tokenizer_json["model"]["continuing_subword_prefix"] is not None
+            ):
+                kwargs["continuing_subword_prefix"] = tokenizer_json["model"][
+                    "continuing_subword_prefix"
+                ]
+            if (
+                model_name == "BPE"
+                and "end_of_word_suffix" not in kwargs
+                and tokenizer_json["model"]["end_of_word_suffix"] is not None
+            ):
+                kwargs["end_of_word_suffix"] = tokenizer_json["model"][
+                    "end_of_word_suffix"
+                ]
+        elif model_name == "Unigram" and tokenizer_json["model"]["unk_id"] is not None:
+            if "max_piece_length" not in kwargs:
+                kwargs["max_piece_length"] = UNIGRAM_MAX_PIECE_LENGTH
+            unk_id = tokenizer_json["model"]["unk_id"]
+            kwargs["unk_token"] = tokenizer_json["model"]["vocab"][unk_id][0]
+
+        # Trains the tokenizer
+        name_trainer = f"{'Bpe' if model_name == 'BPE' else model_name}Trainer"
+        trainer = getattr(_tok_trainers, name_trainer)(
             vocab_size=vocab_size,
-            special_tokens=special_tokens_bytes,
             show_progress=True,
+            special_tokens=special_tokens,
+            initial_alphabet=list(initial_alphabet.keys()),
             **kwargs,
         )
-        self._bpe_model.train_from_iterator(
-            iterator, length=len(iterator), trainer=trainer
-        )
+        tokenizer.train_from_iterator(iterator, length=len(iterator), trainer=trainer)
 
-        # Update other vocabs accordingly
-        if start_from_empty_voc:
-            # If we do not give an existing vocabulary to the tokenizer, 🤗tokenizers
-            # first fill its vocabulary with all bytes present in the training samples,
-            # sorted by byte / char index. Some bytes / tokens might be missing from
-            # tokenizer.get_vocab(), as simply not present in training samples. We must
-            # get rid of them from the base vocabulary
-            new_vocab = dict(
-                sorted(self._bpe_model.get_vocab().items(), key=lambda item: item[1])
-            )
-            byte_to_token_old = deepcopy(self._vocab_base_byte_to_token)
-
-            # Rebuild base vocabularies dicts
-            self._vocab_base = {}  # token -> id
-            self.__vocab_base_inv = {}  # id -> token
-            self._vocab_base_byte_to_token = {}  # for all basic tokens
-            self._vocab_base_id_to_byte = {}
-            # dict is ordered so id val is incremented each time, from 0
-            for byte_ in new_vocab:
-                if byte_ in byte_to_token_old:
-                    token = byte_to_token_old[
-                        byte_
-                    ]  # get the original token associated to the byte
-                    self.add_to_vocab(
-                        token, byte_=byte_, add_to_bpe_model=False
-                    )  # adds it to _vocab_base
-
-        # Update __vocab_bpe_bytes_to_tokens for faster decoding
-        self._vocab_bpe_bytes_to_tokens = {
+        # Update _vocab_learned_bytes_to_tokens for faster decoding
+        self._vocab_learned_bytes_to_tokens = {
             k: [self._vocab_base_byte_to_token[b] for b in k]
-            for k in self._bpe_model.get_vocab()
+            for k in tokenizer.get_vocab()
         }
 
-        self.has_bpe = True
+        self._model = tokenizer
+        self._model_name = model_name
+
+    @staticmethod
+    def __reload_hf_tokenizer(tokenizer: _HFTokenizer) -> _HFTokenizer:
+        # Converts model to json
+        tokenizer_json = json.loads(tokenizer.to_str())
+
+        # Remove vocab
+        # Apr 16th 2024 - MidiTok v3.0.3: when resuming training, we restart all over
+        # from a clean vocabulary. As tokenizers v0.19.0, resuming a training does
+        # not further reduce/compress the sequences even with a larger vocabulary.
+        if tokenizer_json["model"]["type"] == "BPE":
+            tokenizer_json["model"]["vocab"] = {}
+            tokenizer_json["model"]["merges"] = []
+        elif tokenizer_json["model"]["type"] == "Unigram":
+            tokenizer_json["model"]["vocab"] = []
+            if tokenizer_json["model"]["unk_id"] is not None:
+                unk_id = tokenizer_json["model"]["unk_id"]
+                unk_token = tokenizer_json["model"]["vocab"][unk_id][0]
+                tokenizer_json["model"]["unk_id"] = 0
+                tokenizer_json["model"]["vocab"] = [[unk_token, 0.0]]
+        elif tokenizer_json["model"]["type"] == "WordPiece":
+            tokenizer_json["model"]["vocab"] = {}
+        else:
+            msg = (
+                "This method does not support this type of tokenizer (found "
+                f"{tokenizer_json['model']['type']}) only BPE, Unigram or WordPiece."
+            )
+            raise ValueError(msg)
+
+        return _HFTokenizer.from_str(json.dumps(tokenizer_json))
+
+    def apply_bpe(self, *args, **kwargs) -> Score:  # noqa: D102, ANN002
+        warnings.warn(
+            "miditok: The `apply_bpe` method had been renamed `encode_token_ids`. It is"
+            " now depreciated and will be removed in future updates.",
+            stacklevel=2,
+        )
+        return self.encode_token_ids(*args, **kwargs)
 
-    def apply_bpe(self, seq: TokSequence | list[TokSequence]) -> None:
+    def encode_token_ids(self, seq: TokSequence | list[TokSequence]) -> None:
         """
-        Apply Byte Pair Encoding (BPE) to a TokSequence, or list of TokSequences.
+        Encode a :class:`miditok.TokSequence` with BPE, Unigram or WordPiece.
 
-        If a list is given, BPE will be applied by batch on all sequences at the time.
+        The method works inplace and only alters the sequence's ``.ids``.
+        The method also works with lists of :class:`miditok.TokSequence`.
+        If a list is given, the model will encode all sequences in one batch to speed up
+        the operation.
 
-        :param seq: Sequence(s) to apply BPE.
+        :param seq: :class:`miditok.TokSequence` to encode ids.
         """
-        if isinstance(seq, list):
-            for seq_ in seq:
-                self.complete_sequence(seq_, complete_bytes=True)
-            encoded_tokens = self._bpe_model.encode_batch(
-                [[t.bytes] for t in seq], is_pretokenized=True
-            )
-            for seq_, bpe_tokens in zip(seq, encoded_tokens):
-                seq_.ids = bpe_tokens.ids
-                seq_.ids_bpe_encoded = True
 
+        def _split_seq_bytes(seq__: TokSequence) -> list[str]:
+            self.complete_sequence(seq__, complete_bytes=True)
+            if self.config.encode_ids_split == "bar":
+                return [subseq.bytes for subseq in seq__.split_per_bars()]
+            if self.config.encode_ids_split == "beat":
+                return [subseq.bytes for subseq in seq__.split_per_beats()]
+            return [seq__.bytes]
+
+        # No recursivity as we can leverage batching here
+        if isinstance(seq, list):
+            all_bytes = [_split_seq_bytes(seq_) for seq_ in seq]
+            encoded_tokens = self._model.encode_batch(all_bytes, is_pretokenized=True)
+            for seq_, ids_encoded in zip(seq, encoded_tokens):
+                seq_.ids = ids_encoded.ids
+                seq_.are_ids_encoded = True
         else:
-            self.complete_sequence(seq, complete_bytes=True)
-            encoded_tokens = self._bpe_model.encode([seq.bytes], is_pretokenized=True)
+            all_bytes = _split_seq_bytes(seq)
+            encoded_tokens = self._model.encode(all_bytes, is_pretokenized=True)
             seq.ids = encoded_tokens.ids
-            seq.ids_bpe_encoded = True
+            seq.are_ids_encoded = True
+
+    def decode_bpe(self, *args, **kwargs) -> Score:  # noqa: D102, ANN002
+        warnings.warn(
+            "miditok: The `decode_bpe` method had been renamed `decode_token_ids`. It "
+            "is now depreciated and will be removed in future updates.",
+            stacklevel=2,
+        )
+        return self.decode_token_ids(*args, **kwargs)
 
-    def decode_bpe(self, seq: TokSequence | list[TokSequence]) -> None:
+    def decode_token_ids(self, seq: TokSequence | list[TokSequence]) -> None:
         r"""
-        Decode (inplace) the BPE of the ids of a :class:`miditok.TokSequence`.
+        Decode the ids of a :class:`miditok.TokSequence` with BPE, Unigram or WordPiece.
 
-        This method only modifies the ``.ids`` attribute of the input sequence(s) only
+        This method only modifies the ``.ids`` attribute of the input sequence(s)
         and does not complete it. This method can be used recursively on lists of
         :class:`miditok.TokSequence`.
 
         :param seq: token sequence to decompose.
         """
+        # This method directly convert encoded ids to base tokens
         if isinstance(seq, list):
-            [self.decode_bpe(seq_) for seq_ in seq]
+            [self.decode_token_ids(seq_) for seq_ in seq]
 
-        elif isinstance(seq, TokSequence) and seq.ids_bpe_encoded:
-            encoded_bytes = [self._bpe_model.id_to_token(id_) for id_ in seq.ids]
+        elif isinstance(seq, TokSequence) and seq.are_ids_encoded:
+            encoded_bytes = [self._model.id_to_token(id_) for id_ in seq.ids]
             decoded_tokens = [
-                self._vocab_bpe_bytes_to_tokens[byte_] for byte_ in encoded_bytes
+                self._vocab_learned_bytes_to_tokens[byte_] for byte_ in encoded_bytes
             ]
             decoded_tokens = [
                 item for sublist in decoded_tokens for item in sublist
             ]  # flatten
             seq.tokens = decoded_tokens
             seq.ids = self._tokens_to_ids(decoded_tokens)
-            seq.ids_bpe_encoded = False
+            seq.are_ids_encoded = False
 
-    def tokenize_midi_dataset(
+    def tokenize_midi_dataset(self, *args, **kwargs) -> Score | list[Score]:  # noqa: D102, ANN002
+        warnings.warn(
+            "miditok: The `tokenize_midi_dataset` method had been renamed "
+            "`tokenize_dataset`. It is now depreciated and will be removed in future "
+            "updates.",
+            stacklevel=2,
+        )
+        return self.tokenize_dataset(*args, **kwargs)
+
+    def tokenize_dataset(
         self,
-        midi_paths: str | Path | Sequence[str | Path],
+        files_paths: str | Path | Sequence[str | Path],
         out_dir: str | Path,
         overwrite_mode: bool = True,
         validation_fn: Callable[[Score], bool] | None = None,
         save_programs: bool | None = None,
         verbose: bool = True,
     ) -> None:
         r"""
-        Tokenize a dataset or list of MIDI files and save them in Json files.
+        Tokenize a dataset or list of music files and save them in Json files.
 
         The resulting json files will have an ``ids`` entry containing the token ids.
         The format of the ids will correspond to the format of the tokenizer
         (``tokenizer.io_format``). Note that the file tree of the source files, up to
-        the deepest common root directory if `midi_paths` is given as a list of paths,
+        the deepest common root directory if `files_paths` is given as a list of paths,
         will be reproducing in ``out_dir``. The config of the tokenizer will be saved
         as a file named ``tokenizer_config_file_name`` (default: ``tokenizer.json``)
         in the ``out_dir`` directory.
 
-        :param midi_paths: paths of the MIDI files. It can also be a path to a
-            directory, in which case this method will recursively find the MIDI files
-            within (.mid, .midi extensions).
+        :param files_paths: paths of the music files (MIDI, abc). It can also be a path
+            to a directory, in which case this method will recursively find the MIDI and
+            abc files within (.mid, .midi and .abc extensions, case insensitive).
         :param out_dir: output directory to save the converted files.
         :param overwrite_mode: if True, will overwrite files if they already exist when
             trying to save the new ones created by the method. This is enabled by
             default, as it is good practice to use dedicated directories for each
             tokenized dataset. If False, if a file already exist, the new one will be
             saved in the same directory, with the same name with a number appended at
             the end. Both token files and tokenizer config are concerned.
             (default: ``True``)
-        :param validation_fn: a function checking if the MIDI is valid on your
-            requirements (e.g. time signature, minimum/maximum length, instruments...).
-            (default: ``None``)
-        :param save_programs: will save the programs of the tracks of the MIDI as an
-            entry in the Json file. That this option is probably unnecessary when using
-            a multitrack tokenizer (`config.use_programs`), as the program information
-            is present within the tokens, and that the tracks having the same programs
-            are likely to have been merged. (default: ``False`` if
-            ``config.use_programs``, else ``True``)
-        :param verbose: will throw warnings of errors when loading MIDI files, or if
-            some MIDI content is incorrect or need your attention. (default: ``True``)
+        :param validation_fn: a function checking if a music file is valid validates
+            your conditions (e.g. time signature, minimum/maximum length,
+            instruments...). (default: ``None``)
+        :param save_programs: will save the programs of the tracks of the files as an
+            entry in the Json file. This option is probably unnecessary when using a
+            multitrack tokenizer (`config.use_programs`), as the program information is
+            present within the tokens, and that the tracks having the same programs are
+            likely to have been merged. (default: ``False`` if ``config.use_programs``,
+            else ``True``)
+        :param verbose: will throw warnings of errors when loading files, or if
+            some files content is incorrect or need your attention. (default: ``True``)
         """
         self._verbose = verbose
-        out_dir = Path(out_dir)
+        out_dir = Path(out_dir).resolve()
         out_dir.mkdir(parents=True, exist_ok=True)
 
-        # User gave a path to a directory, we'll scan it to find MIDI files
-        if not isinstance(midi_paths, Sequence):
-            if isinstance(midi_paths, str):
-                midi_paths = Path(midi_paths)
-            root_dir = midi_paths
-            midi_paths = [
+        # User gave a path to a directory, we'll scan it to find MIDI/abc files
+        if not isinstance(files_paths, Sequence):
+            if isinstance(files_paths, str):
+                files_paths = Path(files_paths)
+            root_dir = files_paths
+            files_paths = [
                 path
-                for path in midi_paths.glob("**/*")
-                if path.suffix in MIDI_FILES_EXTENSIONS
+                for path in files_paths.glob("**/*")
+                if path.suffix in SUPPORTED_MUSIC_FILE_EXTENSIONS
             ]
         # User gave a list of paths, we need to find the root / deepest common subdir
         else:
-            all_parts = [Path(path).parent.parts for path in midi_paths]
-            max_depth = max(len(parts) for parts in all_parts)
-            root_parts = []
-            for depth in range(max_depth):
-                if len({parts[depth] for parts in all_parts}) > 1:
-                    break
-                root_parts.append(all_parts[0][depth])
-            root_dir = Path(*root_parts)
+            root_dir = get_deepest_common_subdir(files_paths)
 
         if save_programs is None:
             save_programs = not self.config.use_programs
 
-        desc = f'Tokenizing MIDIs ({"/".join(list(out_dir.parts[-2:]))})'
-        for midi_path in tqdm(midi_paths, desc=desc):
-            # Some MIDIs can contain errors, if so the loop continues
-            midi_path = Path(midi_path)
+        # Tokenizing
+        # Note: tests with multiprocessing show significant slower runtime with 4
+        # workers.
+        desc = f"Tokenizing music files ({'/'.join(list(out_dir.parts[-2:]))})"
+        for file_path in tqdm(files_paths, desc=desc):
+            # Some files can contain errors, if so the loop continues
+            file_path = Path(file_path)
             try:
-                midi = Score(midi_path)
+                score = Score(file_path)
             except FileNotFoundError:
                 if self._verbose:
-                    warnings.warn(f"File not found: {midi_path}", stacklevel=2)
+                    warnings.warn(f"File not found: {file_path}", stacklevel=2)
                 continue
-            except MIDI_LOADING_EXCEPTION:
+            except SCORE_LOADING_EXCEPTION:
                 continue
 
-            # Passing the MIDI to validation tests if given
-            if validation_fn is not None and not validation_fn(midi):
+            # Passing the Score to validation tests if given
+            if validation_fn is not None and not validation_fn(score):
                 continue
 
-            # Tokenizing the MIDI
-            tokens = self.midi_to_tokens(midi)
+            # Tokenizing the Score
+            tokens = self.encode(score)
 
             # Set output file path
-            out_path = out_dir / midi_path.parent.relative_to(root_dir)
+            out_path = out_dir / file_path.resolve().parent.relative_to(root_dir)
             out_path.mkdir(parents=True, exist_ok=True)
-            out_path /= f"{midi_path.stem}.json"
+            out_path /= f"{file_path.stem}.json"
 
             # If non-overwrite, set the new file name
             if not overwrite_mode and out_path.is_file():
                 i = 1
                 while out_path.is_file():
-                    out_path = out_path.parent / f"{midi_path.stem}_{i}.json"
+                    out_path = out_path.parent / f"{file_path.stem}_{i}.json"
                     i += 1
 
             # Save the tokens as JSON
             self.save_tokens(
                 tokens,
                 out_path,
-                get_midi_programs(midi) if save_programs else None,
+                get_score_programs(score) if save_programs else None,
             )
 
         # Set it back to False
         self._verbose = False
 
     def tokens_errors(
         self,
@@ -2600,31 +2916,31 @@
         # If list of TokSequence -> recursive
         if isinstance(tokens, list):
             return [self.tokens_errors(tok_seq) for tok_seq in tokens]
         if len(tokens) == 0:
             return 0
 
         num_tok_predicted = len(tokens)  # used to norm the score
-        if self.has_bpe:
-            self.decode_bpe(tokens)
+        if self.is_trained:
+            self.decode_token_ids(tokens)
         self.complete_sequence(tokens)
 
         # Compute number of errors and norm by number of tokens predicted
         return self._tokens_errors(tokens.tokens) / num_tok_predicted
 
     def _tokens_errors(self, tokens: list[str | list[str]]) -> int:
         r"""
         Return the number of errors in a sequence of tokens.
 
         The method checks if a sequence of tokens is made of good token types
         successions and values. The number of errors should not be higher than the
         number of tokens.
 
         This method is intended to be overridden by tokenizer classes. The
-        implementation in the ``MIDITokenizer`` class will check token types,
+        implementation in the ``MusicTokenizer`` class will check token types,
         duplicated notes and time errors. It works for ``REMI``, ``TSD`` and
         ``Structured``.
 
         :param tokens: sequence of tokens string to check.
         :return: the number of errors predicted (no more than one per token).
         """
         err_type = 0  # i.e. incompatible next type predicted
@@ -2649,15 +2965,15 @@
 
         for ti, token in enumerate(tokens[1:]):
             # err_tokens = tokens[ti - 4 : ti + 4]  # uncomment for debug
             event_type, event_value = token.split("_")
 
             # Good token type
             if event_type in self.tokens_types_graph[previous_type]:
-                if event_type == "Bar":  # reset
+                if token == "Bar_None":  # reset
                     current_pos = -1
                     current_pitches = {p: [] for p in self.config.programs}
                 elif event_type in ["TimeShift", "Time-Shift", "Rest"]:
                     current_pitches = {p: [] for p in self.config.programs}
                 elif event_type in note_tokens_types:
                     if event_type in {"Pitch", "NoteOn", "PitchDrum"}:
                         pitch_val = int(event_value)
@@ -2720,35 +3036,35 @@
         :param tokens: tokens, as list, numpy array, torch or tensorflow Tensor.
         :param path: path of the file to save.
         :param programs: (optional), programs of the associated tokens, should be given
             as a tuples (int, bool) for (program, is_drum).
         :param kwargs: any additional information to save within the JSON file.
         """
         ids = []
-        ids_bpe_encoded = None
+        ids_encoded = None
 
         if isinstance(tokens, TokSequence):
             if tokens.ids is None:
                 self.complete_sequence(tokens)
-            ids_bpe_encoded = tokens.ids_bpe_encoded
+            ids_encoded = tokens.are_ids_encoded
             ids = tokens.ids
         elif isinstance(tokens, list) and len(tokens) == 0:
             pass
         elif isinstance(tokens[0], TokSequence):
-            ids_bpe_encoded = []
+            ids_encoded = []
             for seq in tokens:
                 if seq.ids is None:
                     self.complete_sequence(seq)
-                ids_bpe_encoded.append(seq.ids_bpe_encoded)
+                ids_encoded.append(seq.are_ids_encoded)
                 ids.append(seq.ids)
         else:
             ids = convert_ids_tensors_to_list(tokens)
 
-        if "ids_bpe_encoded" not in kwargs and ids_bpe_encoded is not None:
-            kwargs["ids_bpe_encoded"] = ids_bpe_encoded
+        if "ids_encoded" not in kwargs and ids_encoded is not None:
+            kwargs["ids_encoded"] = ids_encoded
 
         with Path(path).open("w") as outfile:
             dic = {"ids": ids, **kwargs}
             if programs is not None:
                 dic["programs"] = programs
             json.dump(dic, outfile)
 
@@ -2831,30 +3147,29 @@
             file. It can be used to override the default attributes saved in the parent
             method. (default: ``None``)
         :param filename: name of the file to save, to be used in case ``out_path`` leads
             to a directory. (default: ``"tokenizer.json"``)
         """
         if additional_attributes is None:
             additional_attributes = {}
-        if self.has_bpe:  # saves whole vocab if BPE
+        if self.is_trained:  # saves whole vocab if trained
             additional_attributes["_vocab_base"] = self._vocab_base
-            additional_attributes["_bpe_model"] = self._bpe_model.to_str()
+            additional_attributes["_model"] = self._model.to_str()
             additional_attributes[
                 "_vocab_base_byte_to_token"
             ] = self._vocab_base_byte_to_token
 
         dict_config = self.config.to_dict(serialize=True)
         for beat_res_key in ["beat_res", "beat_res_rest"]:
             dict_config[beat_res_key] = {
                 f"{k1}_{k2}": v for (k1, k2), v in dict_config[beat_res_key].items()
             }
         params = {
             "config": dict_config,
             "one_token_stream": self.one_token_stream,
-            "has_bpe": self.has_bpe,
             "tokenization": self.__class__.__name__,
             "miditok_version": CURRENT_MIDITOK_VERSION,
             "symusic_version": CURRENT_SYMUSIC_VERSION,
             "hf_tokenizers_version": CURRENT_TOKENIZERS_VERSION,
             **additional_attributes,
         }
 
@@ -2874,15 +3189,15 @@
         cache_dir: str | Path | None,
         force_download: bool,
         proxies: dict | None,
         resume_download: bool,
         local_files_only: bool,
         token: str | bool | None,
         **kwargs,
-    ) -> MIDITokenizer:
+    ) -> MusicTokenizer:
         # Called by `ModelHubMixin.from_pretrained`
         pretrained_path = Path(model_id)
         if pretrained_path.is_file():
             params_path = pretrained_path
         else:
             filename = kwargs.get("filename", DEFAULT_TOKENIZER_FILE_NAME)
             if (pretrained_path / filename).is_file():
@@ -2902,15 +3217,15 @@
                     library_version=CURRENT_MIDITOK_VERSION,
                 )
 
         # Checking config file tokenization
         with Path(params_path).open() as file:
             tokenization = json.load(file)["tokenization"]
         cls_name = cls.__name__
-        if cls_name not in ["MIDITokenizer", tokenization]:
+        if cls_name not in ["MusicTokenizer", tokenization]:
             warnings.warn(
                 ".from_pretrained called with an invalid class name. The current class"
                 f"is {cls_name} whereas the config file comes from a {tokenization} "
                 f"tokenizer. Returning an instance of {tokenization}.",
                 stacklevel=2,
             )
 
@@ -2948,27 +3263,27 @@
         for key, value in params.items():
             if key in ["tokenization", "miditok_version"]:
                 continue
             if key == "_vocab_base":
                 self._vocab_base = value
                 self.__vocab_base_inv = {v: k for k, v in value.items()}
                 continue
-            if key == "_bpe_model":
+            if key == "_model":
                 # using 🤗tokenizers builtin method
-                self._bpe_model = TokenizerFast.from_str(value)
+                self._model = _HFTokenizer.from_str(value)
                 continue
             if key == "_vocab_base_byte_to_token":
                 self._vocab_base_byte_to_token = value
                 token_to_byte = {v: k for k, v in value.items()}
                 self._vocab_base_id_to_byte = {
                     i: token_to_byte[tok] for tok, i in self._vocab_base.items()
                 }
-                self._vocab_bpe_bytes_to_tokens = {
+                self._vocab_learned_bytes_to_tokens = {
                     k: [self._vocab_base_byte_to_token[b] for b in k]
-                    for k in self._bpe_model.get_vocab()
+                    for k in self._model.get_vocab()
                 }
                 continue
             if key == "config":
                 if "chord_maps" in value:
                     value["chord_maps"] = {
                         chord_quality: tuple(chord_map)
                         for chord_quality, chord_map in value["chord_maps"].items()
@@ -3002,14 +3317,18 @@
                 elif key in old_add_tokens_attr:
                     key = old_add_tokens_attr[key]
                 setattr(self.config, key, value)
                 continue
             if key == "unique_track":
                 # For config files <= v2.1.1 before the attribute is renamed
                 self.one_token_stream = value
+                continue
+            if key == "has_bpe":
+                # For config files < v3.0.3 before the attribute becomes a property
+                continue
 
             setattr(self, key, value)
 
     @property
     def is_multi_voc(self) -> bool:
         """
         Indicate if the tokenizer uses embedding pooling / have multiple vocabularies.
@@ -3037,86 +3356,86 @@
         if self.is_multi_voc:
             format_.append("C")
 
         return tuple(d for d in format_)
 
     def __call__(
         self,
-        obj: Score | TokSequence | list[TokSequence, int, list[int]],
+        obj: Score | TokSequence | list[TokSequence, int, list[int]] | np.ndarray,
         *args,  # noqa: ANN002
         **kwargs,
     ) -> TokSequence | list[TokSequence] | Score:
         r"""
-        Tokenize a MIDI file, or decode tokens into a MIDI.
+        Tokenize a music file (MIDI/abc), or decode tokens into a ``symusic.Score``.
 
-        Calling a tokenizer allows to directly convert a MIDI to tokens or vice-versa.
-        The method automatically detects MIDI and token objects, as well as paths and
-        can directly load MIDI or token json files before converting them. This will
-        call the :py:func:`miditok.MIDITokenizer.midi_to_tokens` if you provide a MIDI
-        object or path to a MIDI file, or the
-        :py:func:`miditok.MIDITokenizer.tokens_to_midi` method otherwise.
+        Calling a tokenizer allows to directly convert a music file (MIDI/abc) to tokens
+        or vice-versa. The method automatically detects ``symusic.Score`` and
+        :class:`miditok.TokSequence` objects, as well as paths to music or json files.
+        It will call the :py:func:`miditok.MusicTokenizer.encode` if you provide a
+        ``symusic.Score`` object or path to a music file, or the
+        :py:func:`miditok.MusicTokenizer.decode` method otherwise.
 
-        :param obj: a `symusic.Score` object, a sequence of tokens, or a path to
-            a MIDI or tokens json file.
+        :param obj: a `symusic.Score` object, a :class:`miditok.TokSequence` object, or
+            a path to a music or tokens json file.
         :return: the converted object.
         """
-        # Tokenize MIDI
-        if isinstance(obj, ScoreTick):
-            return self.midi_to_tokens(obj, *args, **kwargs)
+        # Tokenize `Score`
+        if isinstance(obj, Score):
+            return self.encode(obj, *args, **kwargs)
 
-        # Loads a file (.mid or .json)
+        # Path provided: Encode/decode a file
         if isinstance(obj, (str, Path)):
-            path = Path(obj)
-            if path.suffix in MIDI_FILES_EXTENSIONS:
-                midi = Score(obj)
-                return self.midi_to_tokens(midi, *args, **kwargs)
-
-            tokens = self.load_tokens(path)
-            return self.tokens_to_midi(tokens["ids"], *args, **kwargs)
+            obj = Path(obj)
+            # tokens
+            if obj.suffix == "json":
+                tokens = self.load_tokens(obj)
+                return self.decode(tokens["ids"], *args, **kwargs)
+            # music file
+            return self.encode(obj, *args, **kwargs)
 
         # Depreciated miditoolkit object
         if MidiFile is not None and isinstance(obj, MidiFile):
             warnings.warn(
                 "You are using a depreciated `miditoolkit.MidiFile` object. MidiTok"
-                "is now (>v3.0.0) using symusic.Score as MIDI backend. Your MIDI will"
+                "is now (>v3.0.0) using symusic.Score as MIDI backend. Your file will"
                 "be converted on the fly, however please consider using symusic.",
                 stacklevel=2,
             )
-            return self.midi_to_tokens(miditoolkit_to_symusic(obj), *args, **kwargs)
+            return self.encode(miditoolkit_to_symusic(obj), *args, **kwargs)
 
-        # Consider it tokens --> converts to MIDI
-        return self.tokens_to_midi(obj, *args, **kwargs)
+        # Decode tokens, may be a TokSequence, numpy array or tensor
+        return self.decode(obj, *args, **kwargs)
 
     def __len__(self) -> int:
         r"""
         Return the length of the vocabulary.
 
         If the tokenizer uses embedding pooling/have multiple vocabularies, it will
-        return the **sum** of their lengths. If the vocabulary was learned with fast
-        BPE, it will return the length of the BPE vocabulary, i.e. the proper number of
+        return the **sum** of their lengths. If the tokenizer has been trained, this
+        method returns the length of its model's vocabulary, i.e. the proper number of
         possible token ids. Otherwise, it will return the length of the base
-        vocabulary. Use the :py:func:`miditok.MIDITokenizer.len` property
+        vocabulary. Use the :py:func:`miditok.MusicTokenizer.len` property
         (``tokenizer.len``) to get the list of lengths.
 
         :return: length of the vocabulary.
         """
         if self.is_multi_voc:
             return sum([len(v) for v in self.vocab])
-        if self.has_bpe:
-            return len(self._bpe_model.get_vocab())
+        if self.is_trained:
+            return len(self._model.get_vocab())
         return len(self.vocab)
 
     @property
     def len(self) -> int | list[int]:  # noqa: A003
         r"""
         Return the length of the vocabulary.
 
         If the tokenizer uses embedding pooling/have multiple vocabularies, it will
         return the **list** of their lengths. Use the
-        :py:func:`miditok.MIDITokenizer.__len__` magic method
+        :py:func:`miditok.MusicTokenizer.__len__` magic method
         (``len(tokenizer)``) to get the sum of the lengths.
 
         :return: length of the vocabulary.
         """
         return [len(v) for v in self.vocab] if self.is_multi_voc else len(self)
 
     def __repr__(self) -> str:
@@ -3132,19 +3451,19 @@
         if self.one_token_stream:
             tmp.append("one token stream")
         if self.is_multi_voc:
             tmp.append("multi-voc")
         if len(tmp) > 0:
             out_str += f"({', '.join(tmp)})"
 
-        # BPE
-        if self.has_bpe:
-            out_str += ", with BPE"
+        # Trained
+        if self.is_trained:
+            out_str += f", trained with {self._model_name}"
         else:
-            out_str += ", without BPE"
+            out_str += ", not trained"
         return out_str
 
     def __getitem__(
         self, item: int | str | tuple[int, int | str]
     ) -> str | int | list[int]:
         r"""
         Convert a token (int) to an event (str), or vice-versa.
@@ -3191,27 +3510,27 @@
             voc = (
                 self.__vocab_base_inv[vocab_id]
                 if self.is_multi_voc
                 else self.__vocab_base_inv
             )
         return voc[item]
 
-    def __eq__(self, other: MIDITokenizer) -> bool:
+    def __eq__(self, other: MusicTokenizer) -> bool:
         r"""
         Check that two tokenizers are identical.
 
         This is done by comparing their vocabularies, and configuration.
 
         :param other: tokenizer to compare.
         :return: True if the vocabulary(ies) are identical, False otherwise.
         """
         if not isinstance(other, type(self)):
             return False
-        bpe_voc_eq = True
-        if self._bpe_model is not None and other._bpe_model is not None:
-            bpe_voc_eq = self._bpe_model.get_vocab() == other._bpe_model.get_vocab()
+        vocab_trained_eq = self.is_trained == other.is_trained
+        if self.is_trained and other.is_trained:
+            vocab_trained_eq = self._model.get_vocab() == other._model.get_vocab()
         return (
             self._vocab_base == other._vocab_base
-            and bpe_voc_eq
+            and vocab_trained_eq
             and self._vocab_base_byte_to_token == other._vocab_base_byte_to_token
             and self.config == other.config
         )
```

### Comparing `miditok-3.0.2/miditok/data_augmentation/__init__.py` & `miditok-3.0.3/miditok/data_augmentation/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,17 +9,17 @@
     MIDI on combinations of offsets;
 * :py:func:`miditok.data_augmentation.augment_midi_dataset`: augment a list of MIDI
     files on combinations of offsets.
 
 """
 
 from .data_augmentation import (
-    augment_midi,
-    augment_midi_dataset,
-    augment_midi_multiple_offsets,
+    augment_dataset,
+    augment_score,
+    augment_score_multiple_offsets,
 )
 
 __all__ = [
-    "augment_midi",
-    "augment_midi_dataset",
-    "augment_midi_multiple_offsets",
+    "augment_score",
+    "augment_dataset",
+    "augment_score_multiple_offsets",
 ]
```

### Comparing `miditok-3.0.2/miditok/data_augmentation/data_augmentation.py` & `miditok-3.0.3/miditok/data_augmentation/data_augmentation.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,44 +9,45 @@
 import numpy as np
 from symusic import Score
 from tqdm import tqdm
 
 from miditok.constants import (
     MIDI_FILES_EXTENSIONS,
     MIDI_INSTRUMENTS,
-    MIDI_LOADING_EXCEPTION,
+    SCORE_LOADING_EXCEPTION,
+    SUPPORTED_MUSIC_FILE_EXTENSIONS,
 )
 
 
-def augment_midi_dataset(
+def augment_dataset(
     data_path: Path | str,
     pitch_offsets: list[int] | None = None,
     velocity_offsets: list[int] | None = None,
     duration_offsets: list[int] | None = None,
     all_offset_combinations: bool = False,
     restrict_on_program_tessitura: bool = True,
     velocity_range: tuple[int, int] = (1, 127),
     duration_in_ticks: bool = False,
     min_duration: int | float = 0.03125,
     out_path: Path | str | None = None,
     copy_original_in_new_location: bool = True,
     save_data_aug_report: bool = True,
 ) -> None:
     r"""
-    Perform data augmentation on a dataset of MIDI files.
+    Perform data augmentation on a dataset of music files.
 
     The new created files have names in two parts, separated with a "#" character. Make
     sure your files do not have '§' in their names if you intend to reuse the
     information of the second part in some script.
     **Drum tracks are not augmented.**.
 
     :param data_path: root path to the folder containing tokenized json files.
     :param pitch_offsets: list of pitch offsets for augmentation. (default: ``None``)
     :param velocity_offsets: list of velocity offsets for augmentation. If you plan to
-        tokenize this MIDI, the velocity offsets should be chosen accordingly to the
+        tokenize these files, the velocity offsets should be chosen accordingly to the
         number of velocities in your tokenizer's vocabulary (``num_velocities``).
         (default: ``None``)
     :param duration_offsets: list of duration offsets for augmentation, to be given
         either in beats if ``duration_in_ticks`` is ``False``, in ticks otherwise.
         (default: ``None``)
     :param all_offset_combinations: will perform data augmentation on all the possible
         combinations of offset values. If set to ``False``, the method will only
@@ -55,70 +56,75 @@
         recommended pitch values of each instrument/program as the range of possible
         values after augmentation. Otherwise, the ``(0, 127)`` range will be used.
         (default: ``True``)
     :param velocity_range: minimum and maximum velocity values. (default: ``(1, 127)``)
     :param duration_in_ticks: if given ``True``, the ``duration_offset`` argument will
         be considered as expressed in ticks. Otherwise, it is considered in beats, and
         the equivalent in ticks will be determined by multiplying it by the MIDI's
-        time division. (default: False)
+        time division (480 by default for abc files). (default: False)
     :param min_duration: minimum duration limit to apply if ``duration_offset`` is
         negative. If ``duration_in_ticks`` is ``True``, it must be given in ticks,
         otherwise in beats as a float or integer. (default: 0.03125)
     :param out_path: output path to save the augmented files. Original (non-augmented)
-        MIDIs will be saved to this location. If none is given, they will be saved in
+        files will be saved to this location. If none is given, they will be saved in
         the same location as the data_path. (default: None)
     :param copy_original_in_new_location: if given True, the original (non-augmented)
-        MIDIs will be saved in the out_path location too. (default: True)
+        files will be saved in the out_path location too. (default: True)
     :param save_data_aug_report: will save numbers from the data augmentation in a
         ``data_augmentation_report.txt`` file in the output directory. (default: True)
     """
     if out_path is None:
         out_path = Path(data_path)
     else:
         if isinstance(out_path, str):
             out_path = Path(out_path)
         out_path.mkdir(parents=True, exist_ok=True)
     files_paths = [
-        path for path in data_path.glob("**/*") if path.suffix in MIDI_FILES_EXTENSIONS
+        path
+        for path in data_path.glob("**/*")
+        if path.suffix in SUPPORTED_MUSIC_FILE_EXTENSIONS
     ]
 
     num_augmentations, num_tracks_augmented = 0, 0
     for file_path in tqdm(files_paths, desc="Performing data augmentation"):
         try:
-            midi = Score(file_path)
-        except MIDI_LOADING_EXCEPTION:
+            score = Score(file_path)
+        except SCORE_LOADING_EXCEPTION:
             continue
 
-        augmented_midis = augment_midi_multiple_offsets(
-            midi,
+        augmented_scores = augment_score_multiple_offsets(
+            score,
             pitch_offsets,
             velocity_offsets,
             duration_offsets,
             all_offset_combinations,
             restrict_on_program_tessitura,
             velocity_range,
             duration_in_ticks,
             min_duration,
         )
-        for aug_offsets, midi_aug in augmented_midis:
-            if len(midi_aug.tracks) == 0:
+        for aug_offsets, score_aug in augmented_scores:
+            if len(score_aug.tracks) == 0:
                 continue
             suffix = "#" + "_".join(
                 [
                     f"{t}{offset}"
                     for t, offset in zip(["p", "v", "d"], aug_offsets)
                     if offset != 0
                 ]
             )
             saving_path = out_path / file_path.parent.relative_to(data_path)
             saving_path.mkdir(parents=True, exist_ok=True)
-            saving_path /= f"{file_path.stem}{suffix}.mid"
-            midi_aug.dump_midi(saving_path)
+            saving_path /= f"{file_path.stem}{suffix}{file_path.suffix}"
+            if file_path.suffix in MIDI_FILES_EXTENSIONS:
+                score_aug.dump_midi(saving_path)
+            else:
+                score_aug.dump_abc(saving_path)
             num_augmentations += 1
-            num_tracks_augmented += len(midi_aug.tracks)
+            num_tracks_augmented += len(score_aug.tracks)
         if copy_original_in_new_location and out_path != data_path:
             saving_path = out_path / file_path.relative_to(data_path)
             saving_path.parent.mkdir(parents=True, exist_ok=True)
             copy2(file_path, saving_path)
 
     # Saves data augmentation report, json encoded with txt extension to not mess with
     # others json files
@@ -130,43 +136,43 @@
                     "num_files_before": len(files_paths),
                     "num_files_after": len(files_paths) + num_augmentations,
                 },
                 outfile,
             )
 
 
-def _filter_offset_tuples_to_midi(
+def _filter_offset_tuples_to_score(
     pitch_offsets: list[int],
-    midi: Score,
+    score: Score,
     restrict_on_program_tessitura: bool,
 ) -> list[int]:
     r"""
     Remove pitch offset values that would cause errors or are out of tessitura.
 
     :param pitch_offsets: list of pitch offsets for augmentation.
-    :param midi: midi object to augment (default: None)
+    :param score: ``symusic.Score`` object to augment (default: None)
     :param restrict_on_program_tessitura: if ``True``, the method will consider the
         recommended pitch values of each instrument/program as the range of possible
         values after augmentation. Otherwise, the ``(0, 127)`` range will be used.
     :return: the filtered offsets of pitch.
     """
-    # Get min and max pitches in the MIDI (except drum tracks)
+    # Get min and max pitches in the Score (except drum tracks)
     all_pitches = [
         np.array([note.pitch for note in track.notes])
-        for track in midi.tracks
+        for track in score.tracks
         if not track.is_drum
     ]
     min_pitches = [np.min(pitches) for pitches in all_pitches]
     max_pitches = [np.max(pitches) for pitches in all_pitches]
 
     # Determine the minimum and maximum possible pitch offsets
     if restrict_on_program_tessitura:
         min_possible_pitch_offset, max_possible_pitch_offset = -127, 127
         for min_pitch, max_pitch, track in zip(
-            min_pitches, max_pitches, [t for t in midi.tracks if not t.is_drum]
+            min_pitches, max_pitches, [t for t in score.tracks if not t.is_drum]
         ):
             pitch_range = MIDI_INSTRUMENTS[track.program]["pitch_range"]
             min_possible_pitch_offset = max(
                 min_possible_pitch_offset, pitch_range.start - min_pitch
             )
             max_possible_pitch_offset = min(
                 max_possible_pitch_offset, pitch_range.stop - max_pitch
@@ -179,43 +185,43 @@
         pitch_offset
         for pitch_offset in pitch_offsets
         if min_possible_pitch_offset <= pitch_offset <= max_possible_pitch_offset
     ]
 
 
 def _create_offsets_tuples(
-    midi: Score,
+    score: Score,
     pitch_offsets: list[int] | None = None,
     velocity_offsets: list[int] | None = None,
     duration_offsets: list[int] | None = None,
     all_offset_combinations: bool = False,
     restrict_on_program_tessitura: bool = True,
 ) -> list[tuple[int, int, int]]:
     """
     Create the data augmentation tuples combinations from lists of offsets.
 
-    :param midi: midi object to augment.
+    :param score: ``symusic.Score`` object to augment.
     :param pitch_offsets: list of pitch offsets for augmentation.
     :param velocity_offsets: list of velocity offsets for augmentation. If you plan to
-        tokenize this MIDI, the velocity offsets should be chosen accordingly to the
+        tokenize this file, the velocity offsets should be chosen accordingly to the
         number of velocities in your tokenizer's vocabulary (``num_velocities``).
     :param duration_offsets: list of duration offsets for augmentation, to be given
         either in beats if ``duration_in_ticks`` is ``False``, in ticks otherwise.
     :param all_offset_combinations: will perform data augmentation on all the possible
         combinations of offset values. If set to ``False``, the method will only
         augment on the offsets separately without combining them.
     :param restrict_on_program_tessitura: if ``True``, the method will consider the
         recommended pitch values of each instrument/program as the range of possible
         values after augmentation. Otherwise, the ``(0, 127)`` range will be used.
         (default: ``True``)
     :return:
     """
     # Remove pitch offsets that would cause errors or are out of tessitura
-    pitch_offsets = _filter_offset_tuples_to_midi(
-        pitch_offsets, midi, restrict_on_program_tessitura
+    pitch_offsets = _filter_offset_tuples_to_score(
+        pitch_offsets, score, restrict_on_program_tessitura
     )
     # Create basic offsets
     offsets = [(pitch_offset, 0, 0) for pitch_offset in pitch_offsets]
     offsets += [(0, velocity_offset, 0) for velocity_offset in velocity_offsets]
     offsets += [(0, 0, duration_offset) for duration_offset in duration_offsets]
 
     # Adds all possible combinations
@@ -233,111 +239,111 @@
                         # This could be optimized by removing the "in" and parametrize
                         if new_offset not in offsets:
                             offsets.append(new_offset)
 
     return offsets
 
 
-def augment_midi(
-    midi: Score,
+def augment_score(
+    score: Score,
     pitch_offset: int = 0,
     velocity_offset: int = 0,
     duration_offset: int | float = 0,
     velocity_range: tuple[int, int] = (1, 127),
     duration_in_ticks: bool = False,
     min_duration: int | float = 0.03125,
 ) -> Score:
     r"""
-    Augment a MIDI object by shifting its pitch, velocity and/or duration values.
+    Augment a Score object by shifting its pitch, velocity and/or duration values.
 
     Velocity and duration values will be clipped according to the ``velocity_range``
     and ``min_duration`` arguments. Drum tracks are only augmented on the velocity.
-    If you are using a pitch offset, make sure the MIDI doesn't contain notes with
+    If you are using a pitch offset, make sure the files doesn't contain notes with
     pitches that would end outside the conventional ``(0, 127)`` range, the method will
     otherwise crash.
 
-    :param midi: midi object to augment.
+    :param score: ``symusic.Score`` object to augment.
     :param pitch_offset: pitch offset for augmentation. (default: ``0``)
     :param velocity_offset: velocity offset for augmentation. If you plan to tokenize
-        this MIDI, the velocity offset should be chosen accordingly to the number of
+        this file, the velocity offset should be chosen accordingly to the number of
         velocities in your tokenizer's vocabulary (``num_velocities``).
         (default: ``0``)
     :param duration_offset: duration offset for augmentation, to be given
         either in beats if ``duration_in_ticks`` is ``False``, in ticks otherwise.
         (default: ``0``)
     :param velocity_range: minimum and maximum velocity values. (default: ``(1, 127)``)
     :param duration_in_ticks: if given ``True``, the ``duration_offset`` argument will
         be considered as expressed in ticks. Otherwise, it is considered in beats, and
         the equivalent in ticks will be determined by multiplying it by the MIDI's
-        time division. (default: ``False``)
+        time division (480 by default for abc files). (default: ``False``)
     :param min_duration: minimum duration limit to apply if ``duration_offset`` is
         negative. If ``duration_in_ticks`` is ``True``, it must be given in ticks,
         otherwise in beats as a float or integer. (default: ``0.03125``)
-    :return: the augmented MIDI object.
+    :return: the augmented ``symusic.Score`` object.
     """
-    midi_aug = copy(midi)
+    score_aug = copy(score)
 
     if pitch_offset != 0:
-        for track in midi_aug.tracks:
+        for track in score_aug.tracks:
             if not track.is_drum:
                 track.shift_pitch(pitch_offset, inplace=True)
 
     if velocity_offset != 0:
-        for track in midi_aug.tracks:
+        for track in score_aug.tracks:
             for note in track.notes:
                 vel_shifted = note.velocity + velocity_offset
                 if velocity_offset < 0:
                     note.velocity = max(min(velocity_range), vel_shifted)
                 else:
                     note.velocity = min(max(velocity_range), vel_shifted)
 
     if duration_offset != 0:
         if not duration_in_ticks:
-            duration_offset = max(round(duration_offset * midi.ticks_per_quarter), 1)
-            min_duration = max(round(min_duration * midi.ticks_per_quarter), 1)
+            duration_offset = max(round(duration_offset * score.ticks_per_quarter), 1)
+            min_duration = max(round(min_duration * score.ticks_per_quarter), 1)
         # If in ticks but the offset is a float, we round it to the closest integer.
         elif isinstance(duration_offset, float):
             duration_offset = round(duration_offset)
             min_duration = round(min_duration)
-        for track in midi_aug.tracks:
+        for track in score_aug.tracks:
             if not track.is_drum:
                 for note in track.notes:
                     if duration_offset < 0:
                         # If note.duration <= min_duration, it is left unchanged
                         if note.duration > min_duration:
                             note.duration = max(
                                 min_duration, note.duration + duration_offset
                             )
                     else:
                         note.duration += duration_offset
 
-    return midi_aug
+    return score_aug
 
 
-def augment_midi_multiple_offsets(
-    midi: Score,
+def augment_score_multiple_offsets(
+    score: Score,
     pitch_offsets: list[int] | None = None,
     velocity_offsets: list[int] | None = None,
     duration_offsets: list[int] | None = None,
     all_offset_combinations: bool = False,
     restrict_on_program_tessitura: bool = True,
     velocity_range: tuple[int, int] = (1, 127),
     duration_in_ticks: bool = False,
     min_duration: int | float = 0.03125,
 ) -> list[tuple[tuple[int, int, int], Score]]:
     r"""
-    Perform data augmentations on a MIDI object with multiple offset values.
+    Perform data augmentation on a ``symusic.Score`` object with multiple offset values.
 
     Velocity and duration values will be clipped according to the ``velocity_range`` and
     ``min_duration`` arguments. Drum tracks are only augmented on the velocity.
 
-    :param midi: midi object to augment.
+    :param score: ``symusic.Score`` object to augment.
     :param pitch_offsets: list of pitch offsets for augmentation.
     :param velocity_offsets: list of velocity offsets for augmentation. If you plan to
-        tokenize this MIDI, the velocity offsets should be chosen accordingly to the
+        tokenize this file, the velocity offsets should be chosen accordingly to the
         number of velocities in your tokenizer's vocabulary (``num_velocities``).
         (default: ``None``)
     :param duration_offsets: list of duration offsets for augmentation, to be given
         either in beats if ``duration_in_ticks`` is ``False``, in ticks otherwise.
         (default: ``None``)
     :param all_offset_combinations: will perform data augmentation on all the possible
         combinations of offset values. If set to ``False``, the method will only
@@ -346,44 +352,44 @@
         recommended pitch values of each instrument/program as the range of possible
         values after augmentation. Otherwise, the ``(0, 127)`` range will be used.
         (default: ``True``)
     :param velocity_range: minimum and maximum velocity values. (default: ``(1, 127)``)
     :param duration_in_ticks: if given ``True``, the ``duration_offset`` argument will
         be considered as expressed in ticks. Otherwise, it is considered in beats, and
         the equivalent in ticks will be determined by multiplying it by the MIDI's
-        time division. (default: False)
+        time division (480 by default for abc files). (default: False)
     :param min_duration: minimum duration limit to apply if ``duration_offset`` is
         negative. If ``duration_in_ticks`` is ``True``, it must be given in ticks,
         otherwise in beats as a float or integer. (default: 0.03125)
-    :return: augmented MIDI objects.
+    :return: augmented ``symusic.Score`` objects.
     """
     # Create offset tuples
     # If duration offsets are given in beats, we convert them to ticks here so
     # that the conversion is not done multiple times in downstream methods
     if duration_offsets and not duration_in_ticks:
         duration_offsets = [
-            round(duration_offset * midi.ticks_per_quarter)
+            round(duration_offset * score.ticks_per_quarter)
             for duration_offset in duration_offsets
         ]
-        min_duration = max(round(min_duration * midi.ticks_per_quarter), 1)
+        min_duration = max(round(min_duration * score.ticks_per_quarter), 1)
     offsets = _create_offsets_tuples(
-        midi,
+        score,
         pitch_offsets,
         velocity_offsets,
         duration_offsets,
         all_offset_combinations,
         restrict_on_program_tessitura,
     )
 
     # Create augmented versions
     return [
         (
             offsets_tuple,
-            augment_midi(
-                midi,
+            augment_score(
+                score,
                 *offsets_tuple,
                 velocity_range=velocity_range,
                 duration_in_ticks=True,
                 min_duration=min_duration,
             ),
         )
         for offsets_tuple in offsets
```

### Comparing `miditok-3.0.2/miditok/pytorch_data/__init__.py` & `miditok-3.0.3/miditok/pytorch_data/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """Dataset classes and data collators to be used with PyTorch when training a model."""
 
 from .collators import DataCollator
 from .datasets import (
     DatasetJSON,
     DatasetMIDI,
 )
-from .split_midi_utils import (
+from .split_utils import (
     get_average_num_tokens_per_note,
     split_dataset_to_subsequences,
-    split_midi_per_note_density,
-    split_midis_for_training,
+    split_files_for_training,
+    split_score_per_note_density,
     split_seq_in_subsequences,
 )
 
 __all__ = [
     "DatasetMIDI",
     "DatasetJSON",
     "DataCollator",
     "get_average_num_tokens_per_note",
-    "split_midis_for_training",
-    "split_midi_per_note_density",
+    "split_files_for_training",
+    "split_score_per_note_density",
     "split_dataset_to_subsequences",
     "split_seq_in_subsequences",
 ]
```

### Comparing `miditok-3.0.2/miditok/pytorch_data/collators.py` & `miditok-3.0.3/miditok/pytorch_data/collators.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,19 +64,27 @@
             tensors.
         """
         out_batch = {}
         x, y = None, None
 
         # Figure out inputs
         if self.inputs_kwarg_name in batch[0]:
-            x = [seq[self.inputs_kwarg_name] for seq in batch]
+            x = [
+                seq[self.inputs_kwarg_name]
+                for seq in batch
+                if seq[self.inputs_kwarg_name] is not None
+            ]
 
         # Figure out labels
         if self.labels_kwarg_name in batch[0]:
-            y = [seq[self.labels_kwarg_name] for seq in batch]
+            y = [
+                seq[self.labels_kwarg_name]
+                for seq in batch
+                if seq[self.labels_kwarg_name] is not None
+            ]
         elif self.copy_inputs_as_labels:
             y = deepcopy(x)
 
         # Pad inputs / convert to Tensors
         if x is not None:
             x = _pad_batch(x, self.pad_token, self.pad_on_left)
         if y is not None:
```

### Comparing `miditok-3.0.2/miditok/pytorch_data/datasets.py` & `miditok-3.0.3/miditok/pytorch_data/datasets.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,19 +6,21 @@
 from typing import TYPE_CHECKING, Any
 
 from symusic import Score
 from torch import LongTensor
 from torch.utils.data import Dataset
 from tqdm import tqdm
 
+from miditok.constants import SCORE_LOADING_EXCEPTION
+
 if TYPE_CHECKING:
     from collections.abc import Callable, Mapping, Sequence
     from pathlib import Path
 
-    from miditok import MIDITokenizer, TokSequence
+    from miditok import MusicTokenizer, TokSequence
 
 
 class _DatasetABC(Dataset, ABC):
     r"""
     Abstract ``Dataset`` class.
 
     It holds samples (and optionally labels) and implements the basic magic methods.
@@ -72,55 +74,62 @@
 
         self.__iter_count += 1
         return self[self.__iter_count - 1]
 
 
 class DatasetMIDI(_DatasetABC):
     r"""
-    A ``Dataset`` loading and tokenizing MIDIs during training.
+    A ``Dataset`` loading and tokenizing music files (MIDI, abc) during training.
 
-    This class can be used for either tokenize MIDIs on the fly when iterating it, or
-    by pre-tokenizing all the MIDIs at its initialization and store the tokens in
+    This class can be used for either tokenize music files on the fly when iterating it,
+    or by pre-tokenizing all the files at its initialization and store the tokens in
     memory.
 
     **Important note:** you should probably use this class in concert with the
-    :py:func:`miditok.pytorch_data.split_midis_for_training` method in order to train
-    your model with chunks of MIDIs of token sequence lengths close to ``max_seq_len``.
-    When using this class with MIDI chunks, the ``BOS`` and ``EOS`` tokens will only be
+    :py:func:`miditok.pytorch_data.split_files_for_training` method in order to train
+    your model with chunks of music files having token sequence lengths close to the
+    ``max_seq_len`` value.
+    When using this class with file chunks, the ``BOS`` and ``EOS`` tokens will only be
     added to the first and last chunks respectively. This allows to not train the model
     with ``EOS`` tokens that would incorrectly inform the model the end of the data
     samples, and break the causality chain of consecutive chunks with incorrectly
     placed ``BOS`` tokens.
 
     Additionally, you can use the ``func_to_get_labels`` argument to provide a method
     allowing to use labels (one label per file).
 
-    :param files_paths: paths to MIDI files to load.
+    **Handling of corrupted files:**
+    Some MIDI files may be corrupted, as for example containing unexpected values.
+    In such cases, if the ``DatasetMIDI`` pre-tokenizes, it will simply ignore these
+    files. Otherwise, the ``DatasetMIDI`` will return dictionaries with ``None`` values
+    when iterated.
+
+    :param files_paths: paths to the music files to load.
     :param tokenizer: tokenizer.
     :param max_seq_len: maximum sequence length (in num of tokens)
     :param bos_token_id: *BOS* token id. (default: ``None``)
     :param eos_token_id: *EOS* token id. (default: ``None``)
     :param pre_tokenize:
     :param func_to_get_labels: a function to retrieve the label of a file. The method
         must take two positional arguments: the first is either the
-        :class:`miditok.TokSequence` returned when tokenizing a MIDI, the second is the
+        :class:`miditok.TokSequence` returned when tokenizing a file, the second is the
         path to the file just loaded. The method must return an integer which
         corresponds to the label id (and not the absolute value, e.g. if you are
         classifying 10 musicians, return the id from 0 to 9 included corresponding to
         the musician). (default: ``None``)
     :param sample_key_name: name of the dictionary key containing the sample data when
         iterating the dataset. (default: ``"input_ids"``)
     :param labels_key_name: name of the dictionary key containing the labels data when
         iterating the dataset. (default: ``"labels"``)
     """
 
     def __init__(
         self,
         files_paths: Sequence[Path],
-        tokenizer: MIDITokenizer,
+        tokenizer: MusicTokenizer,
         max_seq_len: int,
         bos_token_id: int | None = None,
         eos_token_id: int | None = None,
         pre_tokenize: bool = False,
         func_to_get_labels: Callable[
             [Score, TokSequence | list[TokSequence], Path],
             int | list[int] | LongTensor,
@@ -139,84 +148,97 @@
         self.eos_token_id = eos_token_id
         self.pre_tokenize = pre_tokenize
         self.func_to_get_labels = func_to_get_labels
         self.sample_key_name = sample_key_name
         self.labels_key_name = labels_key_name
         self.samples, self.labels = ([], []) if func_to_get_labels else (None, None)
 
-        # Pre-tokenize the MIDI files
+        # Pre-tokenize the files
         if pre_tokenize:
             for file_path in tqdm(
                 self.files_paths,
                 desc="Pre-tokenizing",
                 miniters=int(len(self.files_paths) / 20),
                 maxinterval=480,
             ):
-                midi = Score(file_path)
-                tokseq = self._tokenize_midi(midi)
+                try:
+                    score = Score(file_path)
+                except SCORE_LOADING_EXCEPTION:
+                    continue
+                tokseq = self._tokenize_score(score)
                 if tokenizer.one_token_stream:
                     tokseq = [tokseq]
                 for seq in tokseq:
                     self.samples.append(LongTensor(seq.ids))
                     if func_to_get_labels:
-                        label = func_to_get_labels(midi, seq, file_path)
+                        label = func_to_get_labels(score, seq, file_path)
                         if not isinstance(label, LongTensor):
                             label = LongTensor(label)
                         self.labels.append(label)
 
     def __getitem__(self, idx: int) -> dict[str, LongTensor]:
         """
         Return the ``idx`` elements of the dataset.
 
         If the dataset is pre-tokenized, the method will return the token ids.
-        Otherwise, it will tokenize the ``idx``th MIDI file on the fly.
+        Otherwise, it will tokenize the ``idx``th file on the fly. If the file to is
+        corrupted, the method will return an dictionary with ``None`` values.
 
         :param idx: idx of the file/sample.
         :return: the token ids, with optionally the associated label.
         """
         labels = None
 
         # Already pre-tokenized
         if self.pre_tokenize:
             token_ids = self.samples[idx]
             if self.func_to_get_labels is not None:
                 labels = self.labels[idx]
 
         # Tokenize on the fly
         else:
-            midi = Score(self.files_paths[idx])
-            tokseq = self._tokenize_midi(midi)
-            # If not one_token_stream, we only take the first track/sequence
-            token_ids = tokseq.ids if self.tokenizer.one_token_stream else tokseq[0].ids
-            if self.func_to_get_labels is not None:
-                # tokseq can be given as a list of TokSequence to get the labels
-                labels = self.func_to_get_labels(midi, tokseq, self.files_paths[idx])
-                if not isinstance(labels, LongTensor):
-                    labels = LongTensor(labels)
-
-        item = {self.sample_key_name: LongTensor(token_ids)}
-        if labels is not None:
+            try:
+                score = Score(self.files_paths[idx])
+                tseq = self._tokenize_score(score)
+                # If not one_token_stream, we only take the first track/sequence
+                token_ids = tseq.ids if self.tokenizer.one_token_stream else tseq[0].ids
+                if self.func_to_get_labels is not None:
+                    # tokseq can be given as a list of TokSequence to get the labels
+                    labels = self.func_to_get_labels(score, tseq, self.files_paths[idx])
+                    if not isinstance(labels, LongTensor):
+                        labels = LongTensor(
+                            [labels] if isinstance(labels, int) else labels
+                        )
+            except SCORE_LOADING_EXCEPTION:
+                token_ids = None
+
+        item = {
+            self.sample_key_name: LongTensor(token_ids)
+            if token_ids is not None
+            else None
+        }
+        if self.func_to_get_labels is not None:
             item[self.labels_key_name] = labels
 
         return item
 
-    def _tokenize_midi(self, midi: Score) -> TokSequence | list[TokSequence]:
+    def _tokenize_score(self, score: Score) -> TokSequence | list[TokSequence]:
         # Tokenize it
-        tokseq = self.tokenizer.midi_to_tokens(midi)
+        tokseq = self.tokenizer.encode(score)
 
         # If tokenizing on the fly a multi-stream tokenizer, only keeps the first track
         if not self.pre_tokenize and not self.tokenizer.one_token_stream:
             tokseq = [tokseq[0]]
 
-        # If this file is a chunk (split_midis_for_training), determine its id.
+        # If this file is a chunk (split_files_for_training), determine its id.
         # By default, we add BOS and EOS tokens following the values of
         # self.bos_token_id and self.eos_token_id (that may be None), except when the
         # file is identified as a chunk.
         add_bos_token = add_eos_token = True
-        for marker in midi.markers:
+        for marker in score.markers:
             if marker.time != 0:
                 break
             if marker.text.startswith("miditok: chunk"):
                 chunk_id, chunk_id_last = map(
                     int, marker.text.split(" ")[-1].split("/")
                 )
                 add_bos_token = chunk_id == 0
@@ -253,33 +275,33 @@
 
     def __repr__(self) -> str:  # noqa:D105
         return self.__str__()
 
     def __str__(self) -> str:  # noqa:D105
         if self.pre_tokenize:
             return f"Pre-tokenized dataset with {len(self.samples)} samples"
-        return f"{len(self.files_paths)} MIDI files."
+        return f"{len(self.files_paths)} files."
 
 
 class DatasetJSON(_DatasetABC):
     r"""
-    Basic ``Dataset`` loading JSON files of tokenized MIDIs.
+    Basic ``Dataset`` loading JSON files of tokenized music files.
 
     When indexed (``dataset[idx]``), a ``DatasetJSON`` will load the
     ``files_paths[idx]`` JSON file and return the token ids, that can be used to train
     generative models.
 
     **This class is only compatible with tokens saved as a single stream of tokens
     (** ``tokenizer.one_token_stream`` **).** If you plan to use it with token files
     containing multiple token streams, you should first split each track token sequence
     with the :py:func:`miditok.pytorch_data.split_dataset_to_subsequences` method.
 
     If your dataset contains token sequences with lengths largely varying, you might
     want to first split it into subsequences with the
-    :py:func:`miditok.pytorch_data.split_midis_for_training` method before loading
+    :py:func:`miditok.pytorch_data.split_files_for_training` method before loading
     it to avoid losing data.
 
     :param files_paths: list of paths to files to load.
     :param max_seq_len: maximum sequence length (in num of tokens). (default: ``None``)
     :param bos_token_id: *BOS* token id. (default: ``None``)
     :param eos_token_id: *EOS* token id. (default: ``None``)
     """
```

### Comparing `miditok-3.0.2/miditok/pytorch_data/split_midi_utils.py` & `miditok-3.0.3/miditok/pytorch_data/split_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,211 +1,218 @@
-"""Utils methods for MIDI/tokens split."""
+"""Utils methods for Score/tokens split."""
 from __future__ import annotations
 
 import json
 from copy import deepcopy
 from pathlib import Path
 from typing import TYPE_CHECKING, Any
 from warnings import warn
 
 from symusic import Score, TextMeta
 from torch import LongTensor
 from tqdm import tqdm
 
-from miditok.constants import MAX_NUM_FILES_NUM_TOKENS_PER_NOTE
+from miditok.constants import (
+    MAX_NUM_FILES_NUM_TOKENS_PER_NOTE,
+    MIDI_FILES_EXTENSIONS,
+    SCORE_LOADING_EXCEPTION,
+    SUPPORTED_MUSIC_FILE_EXTENSIONS,
+)
 from miditok.utils import (
-    extract_chunk_from_midi,
     get_bars_ticks,
     get_num_notes_per_bar,
-    split_midi_per_tracks,
+    split_score_per_tracks,
 )
+from miditok.utils.utils import get_deepest_common_subdir
 
 if TYPE_CHECKING:
     from collections.abc import Sequence
 
-    from miditok import MIDITokenizer
+    from miditok import MusicTokenizer
 
 
-def split_midis_for_training(
+def split_files_for_training(
     files_paths: Sequence[Path],
-    tokenizer: MIDITokenizer,
+    tokenizer: MusicTokenizer,
     save_dir: Path,
     max_seq_len: int,
     average_num_tokens_per_note: float | None = None,
     num_overlap_bars: int = 1,
     min_seq_len: int | None = None,
 ) -> list[Path]:
     """
-    Split a list of MIDIs into smaller chunks to use for training.
+    Split a list of music files into smaller chunks to use for training.
 
-    MIDI splitting allows to split each MIDI from a dataset into chunks of lengths
-    calculated in function of the note densities of its bars in order to reduce the
-    padding of the batches, using the
-    :py:func:`miditok.pytorch_data.split_midi_per_note_density` method.
-    The MIDIs are only split at bars, in order have chunks starting at relevant times.
+    Splitting files allows to split them into chunks of lengths calculated in function
+    of the note densities of its bars in order to reduce the padding of the batches,
+    using the :py:func:`miditok.pytorch_data.split_score_per_note_density` method.
+    The files are only split at bars, in order have chunks starting at relevant times.
 
-    MIDI splitting can be performed on a dataset once. This method will save a hidden
+    File splitting can be performed on a dataset once. This method will save a hidden
     file, with a name corresponding to the hash of the list of file paths, in the
     ``save_dir`` directory. When called, it will first check that this file does not
-    already exist, and if it is the case will return the paths to all the MIDI files
-    within ``save_dir``.
+    already exist, and if it is the case will return the paths to all the files within
+    ``save_dir``.
 
     **If your tokenizer does not tokenize all tracks in one sequence of tokens**
-    (``tokenizer.one_token_stream``), the MIDI tracks will be split independently.
+    (``tokenizer.one_token_stream``), the music tracks will be split independently.
 
-    :param files_paths: paths to MIDI files to split.
+    :param files_paths: paths to music files to split.
     :param tokenizer: tokenizer.
-    :param save_dir: path to the directory to save the MIDI splits.
+    :param save_dir: path to the directory to save the files splits.
     :param max_seq_len: maximum token sequence length that the model will be trained
         with.
     :param average_num_tokens_per_note: average number of tokens per note associated to
         this tokenizer. If given ``None``, this value will automatically be calculated
-        from the first 200 MIDI files with the
+        from the first 200 files with the
         :py:func:`miditok.pytorch_data.get_average_num_tokens_per_note` method.
     :param num_overlap_bars: will create chunks with consecutive overlapping bars. For
-        example, if this argument is given ``1``, two consecutive MIDI chunks might
-        end at the bar *n* and start at the bar *n-1* respectively, thus they will
-        encompass the same bar. This allows to create a causality chain between chunks.
-        This value should be determined based on the ``average_num_tokens_per_note``
-        value of the tokenizer and the ``max_seq_len`` value, so that it is neither
-        too high nor too low. (default: ``1``).
+        example, if this argument is given ``1``, two consecutive chunks might end at
+        the bar *n* and start at the bar *n-1* respectively, thus they will encompass
+        the same bar. This allows to create a causality chain between chunks. This value
+        should be determined based on the ``average_num_tokens_per_note`` value of the
+        tokenizer and the ``max_seq_len`` value, so that it is neither too high nor too
+        low. (default: ``1``).
     :param min_seq_len: minimum sequence length, only used when splitting at the last
-        bar of the MIDI. (default: ``None``, see default value of
-        :py:func:`miditok.pytorch_data.split_midi_per_note_density`)
-    :return: the paths to the MIDI splits.
+        bar of the file. (default: ``None``, see default value of
+        :py:func:`miditok.pytorch_data.split_score_per_note_density`)
+    :return: the paths to the files splits.
     """
     # Safety checks
-    midi_split_hidden_file_path = save_dir / f".{hash(tuple(files_paths))}"
-    if midi_split_hidden_file_path.is_file():
+    split_hidden_file_path = save_dir / f".{hash(tuple(files_paths))}"
+    if split_hidden_file_path.is_file():
         warn(
-            f"These MIDI have already been split in the saving directory ({save_dir})."
-            f" Skipping MIDI splitting.",
+            f"These files have already been split in the saving directory ({save_dir})."
+            f" Skipping file splitting.",
             stacklevel=2,
         )
-        return list(save_dir.glob("**/*.mid"))
+        return [
+            path
+            for path in save_dir.glob("**/*")
+            if path.suffix in SUPPORTED_MUSIC_FILE_EXTENSIONS
+        ]
     if not average_num_tokens_per_note:
         average_num_tokens_per_note = get_average_num_tokens_per_note(
             tokenizer, files_paths[:MAX_NUM_FILES_NUM_TOKENS_PER_NOTE]
         )
 
     # Determine the deepest common subdirectory to replicate file tree
-    all_parts = [path.parent.parts for path in files_paths]
-    max_depth = max(len(parts) for parts in all_parts)
-    root_parts = []
-    for depth in range(max_depth):
-        if len({parts[depth] for parts in all_parts}) > 1:
-            break
-        root_parts.append(all_parts[0][depth])
-    root_dir = Path(*root_parts)
+    root_dir = get_deepest_common_subdir(files_paths)
 
-    # Splitting MIDIs
+    # Splitting files
     new_files_paths = []
     for file_path in tqdm(
         files_paths,
-        desc=f"Splitting MIDIs ({save_dir})",
+        desc=f"Splitting music files ({save_dir})",
         miniters=int(len(files_paths) / 20),
         maxinterval=480,
     ):
-        midis = [Score(file_path)]
+        try:
+            scores = [Score(file_path)]
+        except SCORE_LOADING_EXCEPTION:
+            continue
 
         # Separate track first if needed
         tracks_separated = False
-        if not tokenizer.one_token_stream and len(midis[0].tracks) > 1:
-            midis = split_midi_per_tracks(midis[0])
+        if not tokenizer.one_token_stream and len(scores[0].tracks) > 1:
+            scores = split_score_per_tracks(scores[0])
             tracks_separated = True
 
         # Split per note density
-        for ti, midi_to_split in enumerate(midis):
-            midi_splits = split_midi_per_note_density(
-                midi_to_split,
+        for ti, score_to_split in enumerate(scores):
+            score_chunks = split_score_per_note_density(
+                score_to_split,
                 max_seq_len,
                 average_num_tokens_per_note,
                 num_overlap_bars,
                 min_seq_len,
             )
 
             # Save them
-            for _i, midi_to_save in enumerate(midi_splits):
+            for _i, chunk_to_save in enumerate(score_chunks):
                 # Skip it if there are no notes, this can happen with
                 # portions of tracks with no notes but tempo/signature
                 # changes happening later
-                if len(midi_to_save.tracks) == 0 or midi_to_save.note_num() == 0:
+                if len(chunk_to_save.tracks) == 0 or chunk_to_save.note_num() == 0:
                     continue
                 # Add a marker to indicate chunk number
-                midi_to_save.markers.append(
-                    TextMeta(0, f"miditok: chunk {_i}/{len(midi_splits) - 1}")
+                chunk_to_save.markers.append(
+                    TextMeta(0, f"miditok: chunk {_i}/{len(score_chunks) - 1}")
                 )
                 if tracks_separated:
-                    file_name = f"{file_path.stem}_t{ti}_{_i}.mid"
+                    file_name = f"{file_path.stem}_t{ti}_{_i}{file_path.suffix}"
                 else:
-                    file_name = f"{file_path.stem}_{_i}.mid"
+                    file_name = f"{file_path.stem}_{_i}{file_path.suffix}"
                 # use with_stem when dropping support for python 3.8
                 saving_path = (
                     save_dir / file_path.relative_to(root_dir).parent / file_name
                 )
                 saving_path.parent.mkdir(parents=True, exist_ok=True)
-                midi_to_save.dump_midi(saving_path)
+                if file_path.suffix in MIDI_FILES_EXTENSIONS:
+                    chunk_to_save.dump_midi(saving_path)
+                else:
+                    chunk_to_save.dump_abc(saving_path)
                 new_files_paths.append(saving_path)
 
-    # Save file in save_dir to indicate MIDI split has been performed
-    with midi_split_hidden_file_path.open("w") as f:
-        f.write(f"{len(files_paths)} files after MIDI splits")
+    # Save file in save_dir to indicate file split has been performed
+    with split_hidden_file_path.open("w") as f:
+        f.write(f"{len(files_paths)} files after file splits")
 
     return new_files_paths
 
 
-def split_midi_per_note_density(
-    midi: Score,
+def split_score_per_note_density(
+    score: Score,
     max_seq_len: int,
     average_num_tokens_per_note: float,
     num_overlap_bars: int = 1,
     min_seq_len: int | None = None,
 ) -> list[Score]:
     """
-    Split a MIDI (at bars) into chunks depending on their note densities.
+    Split a ``symusic.Score`` (at bars) into chunks depending on their note densities.
 
-    This method aims to split MIDIs at bars to reduce the amount of padding to apply to
-    batches during training. It offers several parameters to control where to split
-    depending on the desired outcome, e.g. reduce padding or keep the largest amount of
-    data at the cost of padding.
+    This method aims to split music files at bars to reduce the amount of padding to
+    apply to batches during training. It offers several parameters to control where to
+    split depending on the desired outcome, e.g. reduce padding or keep the largest
+    amount of data at the cost of padding.
 
     This method will estimate the number of tokens for each bar depending on the
     tokenizer's average number of tokens per note (tpn), will loop over the estimated
-    number of tokens per bar to determine the bars at which the MIDI will be "cut".
+    number of tokens per bar to determine the bars at which the file will be "cut".
 
     It is recommended to use this method with a non-zero ``num_overlap_bars``, as
-    overlapping allows to keep a form of causality throughout a MIDI sample from one
-    chunk to another. It also reduces padding, but will slightly increase the overall
-    training duration.
+    overlapping allows to keep a form of causality throughout a file from one chunk to
+    another. It also reduces padding, but will slightly increase the overall training
+    time.
 
-    :param midi: MIDI to split.
+    :param score: ``symusic.Score`` to split.
     :param max_seq_len: maximum number of tokens per sequence.
     :param average_num_tokens_per_note: average number of tokens per note associated to
         this tokenizer.
     :param num_overlap_bars: will create chunks with consecutive overlapping bars. For
-        example, if this argument is given ``1``, two consecutive MIDI chunks might
+        example, if this argument is given ``1``, two consecutive music chunks might
         end at the bar *n* and start at the bar *n-1* respectively, thus they will
         encompass the same bar. This allows to create a causality chain between chunks.
         This value should be determined based on the ``average_num_tokens_per_note``
         value of the tokenizer and the ``max_seq_len`` value, so that it is neither
         too high nor too low. (default: ``1``).
     :param min_seq_len: minimum sequence length, only used when splitting at the last
-        bar of the MIDI. (default: ``max_seq_len // 4``)
-    :return: the list of split MIDIs.
+        bar of the file. (default: ``max_seq_len // 4``)
+    :return: the list of ``symusic.Score`` chunks.
     """
     if num_overlap_bars < 0:
         msg = (
             f"`num_overlap_bars` must be greater or equal to 0 (received "
             f"{num_overlap_bars})."
         )
         raise ValueError(msg)
     if min_seq_len is None:
         min_seq_len = max_seq_len // 4
-    bar_ticks = get_bars_ticks(midi)
-    num_notes_per_bar = get_num_notes_per_bar(midi)
+    bar_ticks = get_bars_ticks(score)
+    num_notes_per_bar = get_num_notes_per_bar(score)
     num_tokens_per_bar = [
         npb * average_num_tokens_per_note for npb in num_notes_per_bar
     ]
 
     ticks_split = []
     num_tokens_current_chunk = num_bars_current_chunk = 0
     bi = bi_start_chunk = 0
@@ -258,46 +265,49 @@
             num_bars_current_chunk += 1
 
         # Continue to the next bar
         bi += 1
 
     # Add the last chunk if its token sequence length is greater than the minimum
     if num_tokens_current_chunk >= min_seq_len:
-        ticks_split.append((bar_ticks[bi_start_chunk], midi.end() + 1))
+        ticks_split.append((bar_ticks[bi_start_chunk], score.end() + 1))
 
     if len(ticks_split) == 1:
-        return [midi]
+        return [score]
 
-    midis_splits = []
-    for tick_start, tick_end in ticks_split:
-        midis_splits.append(extract_chunk_from_midi(midi, tick_start, tick_end))
-    return midis_splits
+    return [
+        score.clip(t_start, t_end).shift_time(-t_start)
+        for t_start, t_end in ticks_split
+    ]
 
 
 def get_average_num_tokens_per_note(
-    tokenizer: MIDITokenizer, files_paths: Sequence[Path]
+    tokenizer: MusicTokenizer, files_paths: Sequence[Path]
 ) -> float:
     """
-    Return the average number of tokens per note (tpn) for a list of MIDIs.
+    Return the average number of tokens per note (tpn) for a list of music files.
 
-    With BPE, the average tpn is likely to be very low.
+    With a trained tokenizer, the average tpn is likely to be very low.
 
     :param tokenizer: tokenizer.
-    :param files_paths: list of MIDI file paths.
+    :param files_paths: list of paths to music files.
     :return: the average tokens per note.
     """
     num_tokens_per_note = []
     for file_path in files_paths:
-        midi = Score(file_path)
-        tok_seq = tokenizer(midi)
+        try:
+            score = Score(file_path)
+        except SCORE_LOADING_EXCEPTION:
+            continue
+        tok_seq = tokenizer(score)
         if tokenizer.one_token_stream:
-            num_notes = midi.note_num()
+            num_notes = score.note_num()
             num_tokens_per_note.append(len(tok_seq) / num_notes)
         else:
-            for track, seq in zip(midi.tracks, tok_seq):
+            for track, seq in zip(score.tracks, tok_seq):
                 num_tokens_per_note.append(len(seq) / track.note_num())
 
     return sum(num_tokens_per_note) / len(num_tokens_per_note)
 
 
 def split_seq_in_subsequences(
     seq: Sequence[any], min_seq_len: int, max_seq_len: int
```

### Comparing `miditok-3.0.2/miditok/tokenizations/__init__.py` & `miditok-3.0.3/miditok/tokenizations/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Tokenizer module.
 
-This module implement tokenizer classes, which inherit from `MIDITokenizer` and
-override specific methods such as `_add_time_events` or `_tokens_to_midi` with
+This module implement tokenizer classes, which inherit from `MusicTokenizer` and
+override specific methods such as `_add_time_events` or `_tokens_to_score` with
 their specific behaviors/representations.
 """
 
 from .cp_word import CPWord
 from .midi_like import MIDILike
 from .mmm import MMM
 from .mumidi import MuMIDI
```

### Comparing `miditok-3.0.2/miditok/tokenizations/cp_word.py` & `miditok-3.0.3/miditok/tokenizations/cp_word.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,27 +5,27 @@
 import warnings
 
 import numpy as np
 from symusic import Note, Score, Tempo, TimeSignature, Track
 
 from miditok.classes import Event, TokSequence
 from miditok.constants import MIDI_INSTRUMENTS, TIME_SIGNATURE
-from miditok.midi_tokenizer import MIDITokenizer
+from miditok.midi_tokenizer import MusicTokenizer
 from miditok.utils import compute_ticks_per_bar, compute_ticks_per_beat
 
 _ADD_TOK_ATTRIBUTES = [
     "use_programs",
     "use_chords",
     "use_rests",
     "use_tempos",
     "use_time_signatures",
 ]
 
 
-class CPWord(MIDITokenizer):
+class CPWord(MusicTokenizer):
     r"""
     Compound Word tokenizer.
 
     Introduced with the
     `Compound Word Transformer (Hsiao et al.) <https://ojs.aaai.org/index.php/AAAI/article/view/16091>`_,
     this tokenization is similar to :ref:`REMI` but uses embedding pooling operations
     to reduce the overall sequence length: note tokens (*Pitch*, *Velocity* and
@@ -47,15 +47,15 @@
     The output hidden states of the model will then be fed to several output layers
     (one per token type). This means that the training requires to add multiple losses.
     For generation, the decoding implies sample from several distributions, which can
     be very delicate. Hence, we do not recommend this tokenization for generation with
     small models.
     **Note:** When decoding multiple token sequences (of multiple tracks), i.e. when
     ``config.use_programs`` is False, only the tempos and time signatures of the first
-    sequence will be decoded for the whole MIDI.
+    sequence will be decoded for the whole music.
     """
 
     def _tweak_config_before_creating_voc(self) -> None:
         if self.config.use_time_signatures and self.config.use_rests:
             # NOTE: this configuration could work by adding a Bar token with the new
             # TimeSig after the Rest, but the decoding should handle this to not add
             # another bar. Or it could work by making Rests not crossing new bars.
@@ -98,16 +98,16 @@
         Create the time events from a list of global and track events.
 
         Internal method intended to be implemented by child classes.
         The returned sequence is the final token sequence ready to be converted to ids
         to be fed to a model.
 
         :param events: sequence of global and track events to create tokens time from.
-        :param time_division: time division in ticks per quarter of the MIDI being
-            tokenized.
+        :param time_division: time division in ticks per quarter of the
+            ``symusic.Score`` being tokenized.
         :return: the same events, with time events inserted.
         """
         # Add time events
         all_events = []
         current_bar = -1
         bar_at_last_ts_change = 0
         previous_tick = -1
@@ -381,37 +381,37 @@
             if program is not None:
                 cp_token[self.vocab_types_idx["Program"]] = create_event(
                     "Program", program
                 )
 
         return cp_token
 
-    def _tokens_to_midi(
+    def _tokens_to_score(
         self,
         tokens: TokSequence | list[TokSequence],
         programs: list[tuple[int, bool]] | None = None,
     ) -> Score:
         r"""
-        Convert tokens (:class:`miditok.TokSequence`) into a MIDI.
+        Convert tokens (:class:`miditok.TokSequence`) into a ``symusic.Score``.
 
-        This is an internal method called by ``self.tokens_to_midi``, intended to be
-        implemented by classes inheriting :class:`miditok.MidiTokenizer`.
+        This is an internal method called by ``self.decode``, intended to be
+        implemented by classes inheriting :class:`miditok.MusicTokenizer`.
 
         :param tokens: tokens to convert. Can be either a list of
             :class:`miditok.TokSequence` or a list of :class:`miditok.TokSequence`s.
         :param programs: programs of the tracks. If none is given, will default to
             piano, program 0. (default: ``None``)
-        :return: the midi object (:class:`symusic.Score`).
+        :return: the ``symusic.Score`` object.
         """
         # Unsqueeze tokens in case of one_token_stream
         if self.one_token_stream:  # ie single token seq
             tokens = [tokens]
         for i in range(len(tokens)):
             tokens[i] = tokens[i].tokens
-        midi = Score(self.time_division)
+        score = Score(self.time_division)
 
         # RESULTS
         tracks: dict[int, Track] = {}
         tempo_changes = [Tempo(-1, self.default_tempo)]
         time_signature_changes = []
         tempo_changes[0].tempo = -1
 
@@ -419,19 +419,24 @@
             if prog not in tracks:
                 tracks[prog] = Track(
                     program=0 if prog == -1 else prog,
                     is_drum=prog == -1,
                     name="Drums" if prog == -1 else MIDI_INSTRUMENTS[prog]["name"],
                 )
 
+        def is_track_empty(track: Track) -> bool:
+            return (
+                len(track.notes) == len(track.controls) == len(track.pitch_bends) == 0
+            )
+
         current_tick = tick_at_last_ts_change = tick_at_current_bar = 0
         current_bar = -1
         bar_at_last_ts_change = 0
         current_program = 0
-        current_instrument = None
+        current_track = None
         previous_note_end = 0
         for si, seq in enumerate(tokens):
             # First look for the first time signature if needed
             if si == 0:
                 if self.config.use_time_signatures:
                     for compound_token in seq:
                         token_family = compound_token[0].split("_")[1]
@@ -449,28 +454,28 @@
                                 break
                         else:
                             break
                 if len(time_signature_changes) == 0:
                     time_signature_changes.append(TimeSignature(0, *TIME_SIGNATURE))
             current_time_sig = time_signature_changes[0]
             ticks_per_bar = compute_ticks_per_bar(
-                current_time_sig, midi.ticks_per_quarter
+                current_time_sig, score.ticks_per_quarter
             )
             ticks_per_beat = self._tpb_per_ts[current_time_sig.denominator]
             ticks_per_pos = ticks_per_beat // self.config.max_num_pos_per_beat
             # Set track / sequence program if needed
             if not self.one_token_stream:
                 current_tick = tick_at_last_ts_change = tick_at_current_bar = 0
                 current_bar = -1
                 bar_at_last_ts_change = 0
                 previous_note_end = 0
                 is_drum = False
                 if programs is not None:
                     current_program, is_drum = programs[si]
-                current_instrument = Track(
+                current_track = Track(
                     program=current_program,
                     is_drum=is_drum,
                     name="Drums"
                     if current_program == -1
                     else MIDI_INSTRUMENTS[current_program]["name"],
                 )
 
@@ -492,15 +497,15 @@
                     if self.config.use_programs:
                         current_program = int(compound_token[5].split("_")[1])
                     new_note = Note(current_tick, duration, pitch, vel)
                     if self.one_token_stream:
                         check_inst(current_program)
                         tracks[current_program].notes.append(new_note)
                     else:
-                        current_instrument.notes.append(new_note)
+                        current_track.notes.append(new_note)
                     previous_note_end = max(previous_note_end, current_tick + duration)
 
                 elif token_family == "Metric":
                     bar_pos = compound_token[1].split("_")[0]
                     if bar_pos == "Bar":
                         current_bar += 1
                         if current_bar > 0:
@@ -519,15 +524,15 @@
                             ):
                                 current_time_sig = TimeSignature(current_tick, num, den)
                                 if si == 0:
                                     time_signature_changes.append(current_time_sig)
                                 tick_at_last_ts_change = tick_at_current_bar
                                 bar_at_last_ts_change = current_bar
                                 ticks_per_bar = compute_ticks_per_bar(
-                                    current_time_sig, midi.ticks_per_quarter
+                                    current_time_sig, score.ticks_per_quarter
                                 )
                                 ticks_per_beat = self._tpb_per_ts[
                                     current_time_sig.denominator
                                 ]
                                 ticks_per_pos = (
                                     ticks_per_beat // self.config.max_num_pos_per_beat
                                 )
@@ -572,47 +577,47 @@
                             tick_at_current_bar += (
                                 real_current_bar - current_bar
                             ) * ticks_per_bar
                             current_bar = real_current_bar
 
                     previous_note_end = max(previous_note_end, current_tick)
 
-            # Add current_inst to midi and handle notes still active
-            if not self.one_token_stream:
-                midi.tracks.append(current_instrument)
+            # Add current_inst to score and handle notes still active
+            if not self.one_token_stream and not is_track_empty(current_track):
+                score.tracks.append(current_track)
 
         # Delete mocked
         # And handle first tempo (tick 0) here instead of super
         del tempo_changes[0]
         if len(tempo_changes) == 0 or (
             tempo_changes[0].time != 0
             and round(tempo_changes[0].tempo, 2) != self.default_tempo
         ):
             tempo_changes.insert(0, Tempo(0, self.default_tempo))
         elif round(tempo_changes[0].tempo, 2) == self.default_tempo:
             tempo_changes[0].time = 0
 
-        # create MidiFile
+        # Add global events to score
         if self.one_token_stream:
-            midi.tracks = list(tracks.values())
-        midi.tempos = tempo_changes
-        midi.time_signatures = time_signature_changes
+            score.tracks = list(tracks.values())
+        score.tempos = tempo_changes
+        score.time_signatures = time_signature_changes
 
-        return midi
+        return score
 
     def _create_base_vocabulary(self) -> list[list[str]]:
         r"""
         Create the vocabulary, as a list of string tokens.
 
         Each token is given as the form ``"Type_Value"``, with its type and value
         separated with an underscore. Example: ``Pitch_58``.
-        The :class:`miditok.MIDITokenizer` main class will then create the "real"
+        The :class:`miditok.MusicTokenizer` main class will then create the "real"
         vocabulary as a dictionary. Special tokens have to be given when creating the
         tokenizer, and will be added to the vocabulary by
-        :class:`miditok.MIDITokenizer`.
+        :class:`miditok.MusicTokenizer`.
 
         :return: the vocabulary as a list of string.
         """
         vocab = [[] for _ in range(5)]
 
         vocab[0].append("Family_Metric")
         vocab[0].append("Family_Note")
@@ -670,50 +675,50 @@
             vocab += [
                 ["Ignore_None"]
                 + [f"TimeSig_{i[0]}/{i[1]}" for i in self.time_signatures]
             ]
 
         return vocab
 
-    def _create_token_types_graph(self) -> dict[str, list[str]]:
+    def _create_token_types_graph(self) -> dict[str, set[str]]:
         r"""
         Return a graph/dictionary of the possible token types successions.
 
         :return: the token types transitions dictionary.
         """
         dic = {
-            "Bar": ["Position", "Bar"],
-            "Position": ["Pitch"],
-            "Pitch": ["Pitch", "Bar", "Position"],
+            "Bar": {"Position", "Bar"},
+            "Position": {"Pitch"},
+            "Pitch": {"Pitch", "Bar", "Position"},
         }
 
         if self.config.use_chords:
-            dic["Rest"] = ["Rest", "Position"]
-            dic["Pitch"] += ["Rest"]
+            dic["Rest"] = {"Rest", "Position"}
+            dic["Pitch"] |= {"Rest"}
 
         if self.config.use_rests:
-            dic["Rest"] = ["Rest", "Position", "Bar"]
-            dic["Pitch"] += ["Rest"]
+            dic["Rest"] = {"Rest", "Position", "Bar"}
+            dic["Pitch"] |= {"Rest"}
 
         if self.config.use_tempos:
             # Because a tempo change can happen at any moment
-            dic["Position"] += ["Position", "Bar"]
+            dic["Position"] |= {"Position", "Bar"}
             if self.config.use_rests:
-                dic["Position"].append("Rest")
-                dic["Rest"].append("Position")
+                dic["Position"].add("Rest")
+                dic["Rest"].add("Position")
 
         for key in dic:
-            dic[key].append("Ignore")
-        dic["Ignore"] = list(dic.keys())
+            dic[key].add("Ignore")
+        dic["Ignore"] = set(dic.keys())
 
         if self.config.use_pitchdrum_tokens:
             dic["PitchDrum"] = dic["Pitch"]
             for key, values in dic.items():
                 if "Pitch" in values:
-                    dic[key].append("PitchDrum")
+                    dic[key].add("PitchDrum")
 
         return dic
 
     def _tokens_errors(self, tokens: list[list[str]]) -> int:
         r"""
         Return the number of errors in a sequence of tokens.
```

### Comparing `miditok-3.0.2/miditok/tokenizations/midi_like.py` & `miditok-3.0.3/miditok/tokenizations/midi_like.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 
 from __future__ import annotations
 
 from symusic import Note, Pedal, PitchBend, Score, Tempo, TimeSignature, Track
 
 from miditok.classes import Event, TokSequence
 from miditok.constants import MIDI_INSTRUMENTS, TIME_SIGNATURE
-from miditok.midi_tokenizer import MIDITokenizer
+from miditok.midi_tokenizer import MusicTokenizer
 from miditok.utils import compute_ticks_per_beat
 
 
-class MIDILike(MIDITokenizer):
+class MIDILike(MusicTokenizer):
     r"""
     MIDI-Like tokenizer.
 
     Introduced in `This time with feeling (Oore et al.) <https://arxiv.org/abs/1808.03715>`_
     and later used with `Music Transformer (Huang et al.) <https://openreview.net/forum?id=rJe4ShAcF7>`_
     and `MT3 (Gardner et al.) <https://openreview.net/forum?id=iMSjopcOn0p>`_,
-    this tokenization simply converts MIDI messages (*NoteOn*, *NoteOff*,
+    this tokenization converts music files to MIDI messages (*NoteOn*, *NoteOff*,
     *TimeShift*...) to tokens, hence the name "MIDI-Like".
     ``MIDILike`` decode tokens following a FIFO (First In First Out) logic. When
     decoding tokens, you can limit the duration of the created notes by setting a
     ``max_duration`` entry in the tokenizer's config
     (``config.additional_params["max_duration"]``) to be given as a tuple of three
     integers following ``(num_beats, num_frames, res_frames)``, the resolutions being
     in the frames per beat.
@@ -36,31 +36,31 @@
     same pitch are overlapping, i.e. a first one is still being played when a second
     one is also played, the offset time of the first will be set to the onset time of
     the second. This is done to prevent unwanted duration alterations that could happen
     in such case, as the `NoteOff` token associated to the first note will also end the
     second one.
     **Note:** When decoding multiple token sequences (of multiple tracks), i.e. when
     ``config.use_programs`` is False, only the tempos and time signatures of the first
-    sequence will be decoded for the whole MIDI.
+    sequence will be decoded for the whole music.
     """
 
     def _tweak_config_before_creating_voc(self) -> None:
         self._note_on_off = True
 
     def _add_time_events(self, events: list[Event], time_division: int) -> list[Event]:
         r"""
         Create the time events from a list of global and track events.
 
         Internal method intended to be implemented by child classes.
         The returned sequence is the final token sequence ready to be converted to ids
         to be fed to a model.
 
         :param events: sequence of global and track events to create tokens time from.
-        :param time_division: time division in ticks per quarter of the MIDI being
-            tokenized.
+        :param time_division: time division in ticks per quarter of the
+            ``symusic.Score`` being tokenized.
         :return: the same events, with time events inserted.
         """
         # Add time events
         all_events = []
         previous_tick = 0
         previous_note_end = 0
         ticks_per_beat = compute_ticks_per_beat(TIME_SIGNATURE[1], time_division)
@@ -149,15 +149,15 @@
         context of appearance. This is required, especially for multitrack
         one-token-stream situations where there can be several tokens appearing at
         the same moment (tick) from different tracks, that need to be sorted.
 
         :param event: event to determine priority.
         :return: priority as an int
         """
-        # Global MIDI tokens first
+        # Global tokens first
         if event.type_ in {"Tempo", "TimeSig"}:
             return 0
         # Then NoteOff
         if event.type_ in {"NoteOff", "DrumOff"} or (
             event.type_ == "Program" and event.desc == "ProgramNoteOff"
         ):
             return 1
@@ -171,37 +171,37 @@
         ):
             return 3
         if event.type_ == "ControlChange":
             return 4
         # Track notes then
         return 10
 
-    def _tokens_to_midi(
+    def _tokens_to_score(
         self,
         tokens: TokSequence | list[TokSequence],
         programs: list[tuple[int, bool]] | None = None,
     ) -> Score:
         r"""
-        Convert tokens (:class:`miditok.TokSequence`) into a MIDI.
+        Convert tokens (:class:`miditok.TokSequence`) into a ``symusic.Score``.
 
-        This is an internal method called by ``self.tokens_to_midi``, intended to be
-        implemented by classes inheriting :class:`miditok.MidiTokenizer`.
+        This is an internal method called by ``self.decode``, intended to be
+        implemented by classes inheriting :class:`miditok.MusicTokenizer`.
 
         :param tokens: tokens to convert. Can be either a list of
             :class:`miditok.TokSequence` or a list of :class:`miditok.TokSequence`s.
         :param programs: programs of the tracks. If none is given, will default to
             piano, program 0. (default: ``None``)
-        :return: the midi object (:class:`symusic.Score`).
+        :return: the ``symusic.Score`` object.
         """
         # Unsqueeze tokens in case of one_token_stream
         if self.one_token_stream:  # ie single token seq
             tokens = [tokens]
         for i in range(len(tokens)):
             tokens[i] = tokens[i].tokens
-        midi = Score(self.time_division)
+        score = Score(self.time_division)
         max_duration_str = self.config.additional_params.get("max_duration", None)
         max_duration = None
 
         # RESULTS
         tracks: dict[int, Track] = {}
         tempo_changes, time_signature_changes = [], []
         active_notes: dict[int, dict[int, list[tuple[int, int]]]] = {
@@ -234,41 +234,44 @@
                                         onset_tick,
                                         max_duration,
                                         pitch_,
                                         vel_,
                                     )
                                 )
                 else:
-                    for pitch_, note_ons in active_notes[
-                        current_instrument.program
-                    ].items():
+                    for pitch_, note_ons in active_notes[current_track.program].items():
                         for onset_tick, vel_ in note_ons:
-                            current_instrument.notes.append(
+                            current_track.notes.append(
                                 Note(onset_tick, max_duration, pitch_, vel_)
                             )
 
-        current_instrument = None
+        def is_track_empty(track: Track) -> bool:
+            return (
+                len(track.notes) == len(track.controls) == len(track.pitch_bends) == 0
+            )
+
+        current_track = None
         for si, seq in enumerate(tokens):
             # Set tracking variables
             current_tick = 0
             current_program = 0
             previous_pitch_onset = {prog: -128 for prog in self.config.programs}
             previous_pitch_chord = {prog: -128 for prog in self.config.programs}
             active_pedals = {}
-            ticks_per_beat = midi.ticks_per_quarter
+            ticks_per_beat = score.ticks_per_quarter
             if max_duration_str is not None:
                 max_duration = self._time_token_to_ticks(
                     max_duration_str, ticks_per_beat
                 )
             # Set track / sequence program if needed
             if not self.one_token_stream:
                 is_drum = False
                 if programs is not None:
                     current_program, is_drum = programs[si]
-                current_instrument = Track(
+                current_track = Track(
                     program=current_program,
                     is_drum=is_drum,
                     name="Drums"
                     if current_program == -1
                     else MIDI_INSTRUMENTS[current_program]["name"],
                 )
 
@@ -322,17 +325,23 @@
                         if max_duration is not None and duration > max_duration:
                             duration = max_duration
                         new_note = Note(note_onset_tick, duration, pitch, vel)
                         if self.one_token_stream:
                             check_inst(current_program)
                             tracks[current_program].notes.append(new_note)
                         else:
-                            current_instrument.notes.append(new_note)
+                            current_track.notes.append(new_note)
                 elif tok_type == "Program":
                     current_program = int(tok_val)
+                    if not self.one_token_stream and self.config.program_changes:
+                        if current_program != -1:
+                            current_track.program = current_program
+                        else:
+                            current_track.program = 0
+                            current_track.is_drum = True
                 elif tok_type == "Tempo" and si == 0:
                     tempo_changes.append(Tempo(current_tick, float(tok_val)))
                 elif tok_type == "TimeSig":
                     num, den = self._parse_token_time_signature(tok_val)
                     ticks_per_beat = self._tpb_per_ts[den]
                     if max_duration is not None:
                         max_duration = self._time_token_to_ticks(
@@ -354,15 +363,15 @@
                             # Add instrument if it doesn't exist, can happen for the
                             # first tokens
                             new_pedal = Pedal(current_tick, duration)
                             if self.one_token_stream:
                                 check_inst(pedal_prog)
                                 tracks[pedal_prog].pedals.append(new_pedal)
                             else:
-                                current_instrument.pedals.append(new_pedal)
+                                current_track.pedals.append(new_pedal)
                     elif pedal_prog not in active_pedals:
                         active_pedals[pedal_prog] = current_tick
                 elif tok_type == "PedalOff":
                     pedal_prog = (
                         int(tok_val) if self.config.use_programs else current_program
                     )
                     if pedal_prog in active_pedals:
@@ -375,57 +384,57 @@
                             tracks[pedal_prog].pedals.append(
                                 Pedal(
                                     active_pedals[pedal_prog],
                                     current_tick - active_pedals[pedal_prog],
                                 )
                             )
                         else:
-                            current_instrument.pedals.append(new_pedal)
+                            current_track.pedals.append(new_pedal)
                         del active_pedals[pedal_prog]
                 elif tok_type == "PitchBend":
                     new_pitch_bend = PitchBend(current_tick, int(tok_val))
                     if self.one_token_stream:
                         check_inst(current_program)
                         tracks[current_program].pitch_bends.append(new_pitch_bend)
                     else:
-                        current_instrument.pitch_bends.append(new_pitch_bend)
+                        current_track.pitch_bends.append(new_pitch_bend)
 
-            # Add current_inst to midi and handle notes still active
-            if not self.one_token_stream:
-                midi.tracks.append(current_instrument)
+            # Add current_inst to score and handle notes still active
+            if not self.one_token_stream and not is_track_empty(current_track):
+                score.tracks.append(current_track)
                 clear_active_notes()
-                active_notes[current_instrument.program] = {
+                active_notes[current_track.program] = {
                     pi: []
                     for pi in range(
                         self.config.pitch_range[0], self.config.pitch_range[1] + 1
                     )
                 }
 
         # Handle notes still active
         if self.one_token_stream:
             clear_active_notes()
 
-        # create MidiFile
+        # Add global events to the Score
         if self.one_token_stream:
-            midi.tracks = list(tracks.values())
-        midi.tempos = tempo_changes
-        midi.time_signatures = time_signature_changes
+            score.tracks = list(tracks.values())
+        score.tempos = tempo_changes
+        score.time_signatures = time_signature_changes
 
-        return midi
+        return score
 
     def _create_base_vocabulary(self) -> list[str]:
         r"""
         Create the vocabulary, as a list of string tokens.
 
         Each token is given as the form ``"Type_Value"``, with its type and value
         separated with an underscore. Example: ``Pitch_58``.
-        The :class:`miditok.MIDITokenizer` main class will then create the "real"
+        The :class:`miditok.MusicTokenizer` main class will then create the "real"
         vocabulary as a dictionary. Special tokens have to be given when creating the
         tokenizer, and will be added to the vocabulary by
-        :class:`miditok.MIDITokenizer`.
+        :class:`miditok.MusicTokenizer`.
 
         :return: the vocabulary as a list of string.
         """
         vocab = []
 
         # NoteOn/NoteOff/Velocity
         self._add_note_tokens_to_vocab_list(vocab)
@@ -443,194 +452,197 @@
             vocab += [
                 f'Duration_{".".join(map(str, duration))}'
                 for duration in self.durations
             ]
 
         return vocab
 
-    def _create_token_types_graph(self) -> dict[str, list[str]]:
+    def _create_token_types_graph(self) -> dict[str, set[str]]:
         r"""
         Return a graph/dictionary of the possible token types successions.
 
         :return: the token types transitions dictionary.
         """
-        dic = {"NoteOn": ["Velocity"]}
+        dic: dict[str, set[str]] = {"NoteOn": {"Velocity"}}
 
         if self.config.use_programs:
             first_note_token_type = (
                 "NoteOn" if self.config.program_changes else "Program"
             )
-            dic["Program"] = ["NoteOn", "NoteOff"]
+            dic["Program"] = {"NoteOn", "NoteOff"}
         else:
             first_note_token_type = "NoteOn"
-        dic["Velocity"] = [first_note_token_type, "TimeShift"]
-        dic["NoteOff"] = ["NoteOff", first_note_token_type, "TimeShift"]
-        dic["TimeShift"] = ["NoteOff", first_note_token_type, "TimeShift"]
+        dic["Velocity"] = {first_note_token_type, "TimeShift"}
+        dic["NoteOff"] = {"NoteOff", first_note_token_type, "TimeShift"}
+        dic["TimeShift"] = {"NoteOff", first_note_token_type, "TimeShift"}
         if self.config.use_pitch_intervals:
-            for token_type in ("PitchIntervalTime", "PitchIntervalChord"):
-                dic[token_type] = ["Velocity"]
-                if self.config.use_programs:
-                    dic["Program"].append(token_type)
+            for token_type in {"PitchIntervalTime", "PitchIntervalChord"}:
+                dic[token_type] = {"Velocity"}
+                if (
+                    self.config.use_programs
+                    and self.config.one_token_stream_for_programs
+                ):
+                    dic["Program"].add(token_type)
                 else:
-                    dic["Velocity"].append(token_type)
-                    dic["NoteOff"].append(token_type)
-                    dic["TimeShift"].append(token_type)
+                    dic["Velocity"].add(token_type)
+                    dic["NoteOff"].add(token_type)
+                    dic["TimeShift"].add(token_type)
         if self.config.program_changes:
-            for token_type in ["Velocity", "NoteOff"]:
-                dic[token_type].append("Program")
+            for token_type in {"Velocity", "NoteOff"}:
+                dic[token_type].add("Program")
 
         if self.config.use_chords:
-            dic["Chord"] = [first_note_token_type]
-            dic["TimeShift"] += ["Chord"]
-            dic["NoteOff"] += ["Chord"]
+            dic["Chord"] = {first_note_token_type}
+            dic["TimeShift"] |= {"Chord"}
+            dic["NoteOff"] |= {"Chord"}
             if self.config.use_programs:
-                dic["Program"].append("Chord")
+                dic["Program"].add("Chord")
             if self.config.use_pitch_intervals:
-                dic["Chord"] += ["PitchIntervalTime", "PitchIntervalChord"]
+                dic["Chord"] |= {"PitchIntervalTime", "PitchIntervalChord"}
 
         if self.config.use_tempos:
-            dic["TimeShift"] += ["Tempo"]
-            dic["Tempo"] = [first_note_token_type, "TimeShift"]
+            dic["TimeShift"] |= {"Tempo"}
+            dic["Tempo"] = {first_note_token_type, "TimeShift"}
             if not self.config.use_programs or self.config.program_changes:
-                dic["Tempo"].append("NoteOff")
+                dic["Tempo"].add("NoteOff")
             if self.config.use_chords:
-                dic["Tempo"] += ["Chord"]
+                dic["Tempo"] |= {"Chord"}
             if self.config.use_rests:
-                dic["Tempo"].append("Rest")  # only for first token
+                dic["Tempo"].add("Rest")  # only for first token
             if self.config.use_pitch_intervals:
-                dic["Tempo"] += ["PitchIntervalTime", "PitchIntervalChord"]
+                dic["Tempo"] |= {"PitchIntervalTime", "PitchIntervalChord"}
 
         if self.config.use_time_signatures:
-            dic["TimeShift"] += ["TimeSig"]
-            dic["TimeSig"] = [first_note_token_type, "TimeShift"]
+            dic["TimeShift"] |= {"TimeSig"}
+            dic["TimeSig"] = {first_note_token_type, "TimeShift"}
             if not self.config.use_programs or self.config.program_changes:
-                dic["TimeSig"].append("NoteOff")
+                dic["TimeSig"].add("NoteOff")
             if self.config.use_chords:
-                dic["TimeSig"] += ["Chord"]
+                dic["TimeSig"] |= {"Chord"}
             if self.config.use_rests:
-                dic["TimeSig"].append("Rest")  # only for first token
+                dic["TimeSig"].add("Rest")  # only for first token
             if self.config.use_tempos:
-                dic["TimeSig"].append("Tempo")
+                dic["TimeSig"].add("Tempo")
             if self.config.use_pitch_intervals:
-                dic["TimeSig"] += ["PitchIntervalTime", "PitchIntervalChord"]
+                dic["TimeSig"] |= {"PitchIntervalTime", "PitchIntervalChord"}
 
         if self.config.use_sustain_pedals:
-            dic["TimeShift"].append("Pedal")
-            dic["NoteOff"].append("Pedal")
+            dic["TimeShift"].add("Pedal")
+            dic["NoteOff"].add("Pedal")
             if not self.config.sustain_pedal_duration:
-                dic["NoteOff"].append("PedalOff")
+                dic["NoteOff"].add("PedalOff")
             if self.config.sustain_pedal_duration:
-                dic["Pedal"] = ["Duration"]
-                dic["Duration"] = [
+                dic["Pedal"] = {"Duration"}
+                dic["Duration"] = {
                     first_note_token_type,
                     "NoteOff",
                     "TimeShift",
                     "Pedal",
-                ]
+                }
                 if self.config.use_pitch_intervals:
-                    dic["Duration"] += ["PitchIntervalTime", "PitchIntervalChord"]
+                    dic["Duration"] |= {"PitchIntervalTime", "PitchIntervalChord"}
             else:
-                dic["PedalOff"] = [
+                dic["PedalOff"] = {
                     "Pedal",
                     "PedalOff",
                     first_note_token_type,
                     "NoteOff",
                     "TimeShift",
-                ]
-                dic["Pedal"] = ["Pedal", first_note_token_type, "NoteOff", "TimeShift"]
-                dic["TimeShift"].append("PedalOff")
+                }
+                dic["Pedal"] = {"Pedal", first_note_token_type, "NoteOff", "TimeShift"}
+                dic["TimeShift"].add("PedalOff")
                 if self.config.use_pitch_intervals:
-                    dic["Pedal"] += ["PitchIntervalTime", "PitchIntervalChord"]
-                    dic["PedalOff"] += ["PitchIntervalTime", "PitchIntervalChord"]
+                    dic["Pedal"] |= {"PitchIntervalTime", "PitchIntervalChord"}
+                    dic["PedalOff"] |= {"PitchIntervalTime", "PitchIntervalChord"}
             if self.config.use_chords:
-                dic["Pedal"].append("Chord")
+                dic["Pedal"].add("Chord")
                 if not self.config.sustain_pedal_duration:
-                    dic["PedalOff"].append("Chord")
-                    dic["Chord"].append("PedalOff")
+                    dic["PedalOff"].add("Chord")
+                    dic["Chord"].add("PedalOff")
             if self.config.use_rests:
-                dic["Pedal"].append("Rest")
+                dic["Pedal"].add("Rest")
                 if not self.config.sustain_pedal_duration:
-                    dic["PedalOff"].append("Rest")
+                    dic["PedalOff"].add("Rest")
             if self.config.use_tempos:
-                dic["Tempo"].append("Pedal")
+                dic["Tempo"].add("Pedal")
                 if not self.config.sustain_pedal_duration:
-                    dic["Tempo"].append("PedalOff")
+                    dic["Tempo"].add("PedalOff")
             if self.config.use_time_signatures:
-                dic["TimeSig"].append("Pedal")
+                dic["TimeSig"].add("Pedal")
                 if not self.config.sustain_pedal_duration:
-                    dic["TimeSig"].append("PedalOff")
+                    dic["TimeSig"].add("PedalOff")
 
         if self.config.use_pitch_bends:
             # As a Program token will precede PitchBend otherwise
             # Else no need to add Program as its already in
-            dic["PitchBend"] = [first_note_token_type, "NoteOff", "TimeShift"]
+            dic["PitchBend"] = {first_note_token_type, "NoteOff", "TimeShift"}
             if self.config.use_programs and not self.config.program_changes:
-                dic["Program"].append("PitchBend")
+                dic["Program"].add("PitchBend")
             else:
-                dic["TimeShift"].append("PitchBend")
-                dic["NoteOff"].append("PitchBend")
+                dic["TimeShift"].add("PitchBend")
+                dic["NoteOff"].add("PitchBend")
                 if self.config.use_tempos:
-                    dic["Tempo"].append("PitchBend")
+                    dic["Tempo"].add("PitchBend")
                 if self.config.use_time_signatures:
-                    dic["TimeSig"].append("PitchBend")
+                    dic["TimeSig"].add("PitchBend")
                 if self.config.use_sustain_pedals:
-                    dic["Pedal"].append("PitchBend")
+                    dic["Pedal"].add("PitchBend")
                     if self.config.sustain_pedal_duration:
-                        dic["Duration"].append("PitchBend")
+                        dic["Duration"].add("PitchBend")
                     else:
-                        dic["PedalOff"].append("PitchBend")
+                        dic["PedalOff"].add("PitchBend")
             if self.config.use_chords:
-                dic["PitchBend"].append("Chord")
+                dic["PitchBend"].add("Chord")
             if self.config.use_rests:
-                dic["PitchBend"].append("Rest")
+                dic["PitchBend"].add("Rest")
 
         if self.config.use_rests:
-            dic["Rest"] = ["Rest", first_note_token_type, "TimeShift"]
-            dic["NoteOff"] += ["Rest"]
+            dic["Rest"] = {"Rest", first_note_token_type, "TimeShift"}
+            dic["NoteOff"] |= {"Rest"}
             if self.config.use_chords:
-                dic["Rest"] += ["Chord"]
+                dic["Rest"] |= {"Chord"}
             if self.config.use_tempos:
-                dic["Rest"].append("Tempo")
+                dic["Rest"].add("Tempo")
             if self.config.use_time_signatures:
-                dic["Rest"].append("TimeSig")
+                dic["Rest"].add("TimeSig")
             if self.config.use_sustain_pedals:
-                dic["Rest"].append("Pedal")
+                dic["Rest"].add("Pedal")
                 if self.config.sustain_pedal_duration:
-                    dic["Duration"].append("Rest")
+                    dic["Duration"].add("Rest")
                 else:
-                    dic["Rest"].append("PedalOff")
-                    dic["PedalOff"].append("Rest")
+                    dic["Rest"].add("PedalOff")
+                    dic["PedalOff"].add("Rest")
             if self.config.use_pitch_bends:
-                dic["Rest"].append("PitchBend")
+                dic["Rest"].add("PitchBend")
             if self.config.use_pitch_intervals:
-                dic["Rest"] += ["PitchIntervalTime", "PitchIntervalChord"]
+                dic["Rest"] |= {"PitchIntervalTime", "PitchIntervalChord"}
         else:
-            dic["TimeShift"].append("TimeShift")
+            dic["TimeShift"].add("TimeShift")
 
         if self.config.program_changes:
-            for token_type in [
+            for token_type in {
                 "TimeShift",
                 "Rest",
                 "PitchBend",
                 "Pedal",
                 "PedalOff",
                 "Tempo",
                 "TimeSig",
                 "Chord",
-            ]:
+            }:
                 if token_type in dic:
-                    dic["Program"].append(token_type)
-                    dic[token_type].append("Program")
+                    dic["Program"].add(token_type)
+                    dic[token_type].add("Program")
 
         if self.config.use_pitchdrum_tokens:
             for tok1, tok2 in (("DrumOn", "NoteOn"), ("DrumOff", "NoteOff")):
                 dic[tok1] = dic[tok2]
                 for key, values in dic.items():
                     if tok2 in values:
-                        dic[key].append(tok1)
+                        dic[key].add(tok1)
 
         return dic
 
     def _tokens_errors(self, tokens: list[str]) -> int:
         r"""
         Return the number of errors in a sequence of tokens.
```

### Comparing `miditok-3.0.2/miditok/tokenizations/mumidi.py` & `miditok-3.0.3/miditok/tokenizations/mumidi.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 from math import ceil
 from typing import TYPE_CHECKING
 
 from symusic import Note, Score, Tempo, Track
 
 from miditok.classes import Event, TokSequence
 from miditok.constants import MIDI_INSTRUMENTS
-from miditok.midi_tokenizer import MIDITokenizer
-from miditok.utils import detect_chords, get_midi_ticks_per_beat
+from miditok.midi_tokenizer import MusicTokenizer
+from miditok.utils import detect_chords, get_score_ticks_per_beat
 
 if TYPE_CHECKING:
     import numpy as np
 
 
-class MuMIDI(MIDITokenizer):
+class MuMIDI(MusicTokenizer):
     r"""
     MuMIDI tokenizer.
 
     Introduced with `PopMAG (Ren et al.) <https://arxiv.org/abs/2008.07703>`_,
     this tokenization made for multitrack tasks and uses embedding pooling. Time is
     represented with *Bar* and *Position* tokens. The key idea of MuMIDI is to represent
     all tracks in a single token sequence. At each time step, *Track* tokens preceding
@@ -55,15 +55,14 @@
         self.config.use_pitch_bends = False
         self.config.use_programs = True
         self.config.use_pitch_intervals = True
         self.config.one_token_stream_for_programs = True
         self.config.program_changes = False
 
         if "max_bar_embedding" not in self.config.additional_params:
-            # this attribute might increase if the tokenizer encounter longer MIDIs
             self.config.additional_params["max_bar_embedding"] = 60
 
         self.vocab_types_idx = {
             "Pitch": 0,
             "PitchDrum": 0,
             "Position": 0,
             "Bar": 0,
@@ -83,68 +82,69 @@
     def _add_time_events(self, events: list[Event], time_division: int) -> list[Event]:
         """
         Create the time events from a list of global and track events.
 
         Unused here.
 
         :param events: sequence of global and track events to create tokens time from.
-        :param time_division: time division in ticks per quarter of the MIDI being
-            tokenized.
+        :param time_division: time division in ticks per quarter of the
+            ``symusic.Score`` being tokenized.
         :return: the same events, with time events inserted.
         """
 
-    def _midi_to_tokens(self, midi: Score) -> TokSequence:
+    def _score_to_tokens(self, score: Score) -> TokSequence:
         r"""
-        Convert a **preprocessed** MIDI object to a sequence of tokens.
+        Convert a **preprocessed** ``symusic.Score`` object to a sequence of tokens.
 
         MuMIDI has its own implementation and doesn't use `_add_time_events`.
 
-        :param midi: the MIDI :class:`symusic.Score` object to convert.
+        :param score: the :class:`symusic.Score` object to convert.
         :return: a :class:`miditok.TokSequence` if ``tokenizer.one_token_stream`` is
             ``True``, else a list of :class:`miditok.TokSequence` objects.
         """
         # Check bar embedding limit, update if needed
-        num_bars = ceil(midi.end() / (midi.ticks_per_quarter * 4))
+        num_bars = ceil(score.end() / (score.ticks_per_quarter * 4))
         if self.config.additional_params["max_bar_embedding"] < num_bars:
-            for i in range(
-                self.config.additional_params["max_bar_embedding"], num_bars
-            ):
-                self.add_to_vocab(f"BarPosEnc_{i}", 1)
-            self.config.additional_params["max_bar_embedding"] = num_bars
+            msg = (
+                "miditok: MuMIDI cannot handle this file as it contains "
+                f"{num_bars} whereas the limit of the tokenizer is "
+                f"{self.config.additional_params['max_bar_embedding']}"
+            )
+            raise ValueError(msg)
 
         # Convert each track to tokens (except first pos to track time)
         if self.config.use_chords:
-            ticks_per_beat = get_midi_ticks_per_beat(midi)
+            ticks_per_beat = get_score_ticks_per_beat(score)
         else:
             ticks_per_beat = None
         note_tokens = []
-        for track in midi.tracks:
+        for track in score.tracks:
             if track.program in self.config.programs:
                 note_tokens += self._track_to_tokens(track, ticks_per_beat)
 
         note_tokens.sort(
             key=lambda x: (x[0].time, x[0].desc)
         )  # Sort by time then track
 
-        ticks_per_sample = midi.ticks_per_quarter / self.config.max_num_pos_per_beat
-        ticks_per_bar = midi.ticks_per_quarter * 4
+        ticks_per_sample = score.ticks_per_quarter / self.config.max_num_pos_per_beat
+        ticks_per_bar = score.ticks_per_quarter * 4
         tokens = []
 
         current_tick = -1
         current_bar = -1
         current_pos = -1
         current_track = -2  # because -2 doesn't exist
         current_tempo_idx = 0
-        current_tempo = round(midi.tempos[current_tempo_idx].tempo, 2)
+        current_tempo = round(score.tempos[current_tempo_idx].tempo, 2)
         for note_token in note_tokens:
             # (Tempo) update tempo values current_tempo
             # If the current tempo is not the last one
-            if self.config.use_tempos and current_tempo_idx + 1 < len(midi.tempos):
+            if self.config.use_tempos and current_tempo_idx + 1 < len(score.tempos):
                 # Will loop over incoming tempo changes
-                for tempo_change in midi.tempos[current_tempo_idx + 1 :]:
+                for tempo_change in score.tempos[current_tempo_idx + 1 :]:
                     # If this tempo change happened before the current moment
                     if tempo_change.time <= note_token[0].time:
                         current_tempo = round(tempo_change.tempo, 2)
                         current_tempo_idx += (
                             1  # update tempo value (might not change) and index
                         )
                     elif tempo_change.time > note_token[0].time:
@@ -212,22 +212,22 @@
         * 0: Pitch (as an Event object for sorting purpose afterward);
         * 1: Velocity;
         * 2: Duration.
 
         :param track: track object to convert.
         :param ticks_per_beat: array indicating the number of ticks per beat per
             time signature denominator section. The numbers of ticks per beat depend on
-            the time signatures of the MIDI being parsed. The array has a shape
+            the time signatures of the ``Score`` being parsed. The array has a shape
             ``(N,2)``, for ``N`` changes of ticks per beat, and the second dimension
             representing the end tick of each section and the number of ticks per beat
             respectively. Only used when using chords. (default: ``None``)
         :return: sequence of corresponding tokens.
         """
         # Make sure the notes are sorted first by their onset (start) times, second by
-        # pitch: notes.sort(key=lambda x: (x.start, x.pitch)) (done in midi_to_tokens)
+        # pitch: notes.sort(key=lambda x: (x.start, x.pitch)) (done in preprocess_score)
 
         tokens = []
         tpb = self.time_division
         for note in track.notes:
             # Note
             duration = note.end - note.start
             dur_token = self._tpb_ticks_to_tokens[tpb][duration]
@@ -274,45 +274,45 @@
                 unsqueezed.append([chords[c]])
             tokens = (
                 unsqueezed + tokens
             )  # chords at the beginning to keep the good order during sorting
 
         return tokens
 
-    def _tokens_to_midi(
+    def _tokens_to_score(
         self,
         tokens: TokSequence,
         _: None = None,
     ) -> Score:
         r"""
-        Convert tokens (:class:`miditok.TokSequence`) into a MIDI.
+        Convert tokens (:class:`miditok.TokSequence`) into a ``symusic.Score``.
 
-        This is an internal method called by ``self.tokens_to_midi``, intended to be
-        implemented by classes inheriting :class:`miditok.MidiTokenizer`.
+        This is an internal method called by ``self.decode``, intended to be
+        implemented by classes inheriting :class:`miditok.MusicTokenizer`.
 
         :param tokens: tokens to convert. Can be either a list of
             :class:`miditok.TokSequence` or a list of :class:`miditok.TokSequence`s.
         :param _: in place of programs of the parent method, unused here.
             (default: ``None``)
-        :return: the midi object (:class:`symusic.Score`).
+        :return: the ``symusic.Score`` object.
         """
-        midi = Score(self.time_division)
+        score = Score(self.time_division)
 
         # Tempos
         if self.config.use_tempos and len(tokens) > 0:
             first_tempo = float(tokens.tokens[0][3].split("_")[1])
         else:
             first_tempo = self.default_tempo
-        midi.tempos.append(Tempo(0, first_tempo))
+        score.tempos.append(Tempo(0, first_tempo))
 
         tracks = {}
         current_tick = 0
         current_bar = -1
         current_track = 0  # default set to piano
-        ticks_per_beat = midi.ticks_per_quarter
+        ticks_per_beat = score.ticks_per_quarter
         for time_step in tokens.tokens:
             tok_type, tok_val = time_step[0].split("_")
             if tok_type == "Bar":
                 current_bar += 1
                 current_tick = current_bar * ticks_per_beat * 4
             elif tok_type == "Position":
                 if current_bar == -1:
@@ -335,43 +335,43 @@
                 duration = self._tpb_tokens_to_ticks[ticks_per_beat][duration]
 
                 tracks[current_track].append(Note(current_tick, duration, pitch, vel))
 
             # Decode tempo if required
             if self.config.use_tempos:
                 tempo_val = float(time_step[3].split("_")[1])
-                if tempo_val != midi.tempos[-1].tempo:
-                    midi.tempos.append(Tempo(current_tick, tempo_val))
+                if tempo_val != score.tempos[-1].tempo:
+                    score.tempos.append(Tempo(current_tick, tempo_val))
 
-        # Appends created notes to MIDI object
+        # Appends created notes to Score object
         for program, notes in tracks.items():
             if int(program) == -1:
-                midi.tracks.append(Track(name="Drums", program=0, is_drum=True))
+                score.tracks.append(Track(name="Drums", program=0, is_drum=True))
             else:
-                midi.tracks.append(
+                score.tracks.append(
                     Track(
                         name=MIDI_INSTRUMENTS[int(program)]["name"],
                         program=int(program),
                         is_drum=False,
                     )
                 )
-            midi.tracks[-1].notes = notes
+            score.tracks[-1].notes = notes
 
-        return midi
+        return score
 
     def _create_base_vocabulary(self) -> list[list[str]]:
         r"""
         Create the vocabulary, as a list of string tokens.
 
         Each token is given as the form ``"Type_Value"``, with its type and value
         separated with an underscore. Example: ``Pitch_58``.
-        The :class:`miditok.MIDITokenizer` main class will then create the "real"
+        The :class:`miditok.MusicTokenizer` main class will then create the "real"
         vocabulary as a dictionary. Special tokens have to be given when creating the
         tokenizer, and will be added to the vocabulary by
-        :class:`miditok.MIDITokenizer`.
+        :class:`miditok.MusicTokenizer`.
 
         For MUMIDI, token index 0 is used as a padding index for training.
         * 0: Pitch / PitchDrum / Position / Bar / Program / (Chord) / (Rest)
         * 1: BarPosEnc
         * 2: PositionPosEnc
         * (-3 / 3: Tempo)
         * -2: Velocity
@@ -421,44 +421,44 @@
         # DURATION
         vocab.append(
             [f'Duration_{".".join(map(str, duration))}' for duration in self.durations]
         )
 
         return vocab
 
-    def _create_token_types_graph(self) -> dict[str, list[str]]:
+    def _create_token_types_graph(self) -> dict[str, set[str]]:
         r"""
         Return a graph/dictionary of the possible token types successions.
 
         :return: the token types transitions dictionary.
         """
         dic = {
-            "Bar": ["Bar", "Position"],
-            "Position": ["Program"],
-            "Program": ["Pitch", "PitchDrum"],
-            "Pitch": ["Pitch", "Program", "Bar", "Position"],
-            "PitchDrum": ["PitchDrum", "Program", "Bar", "Position"],
+            "Bar": {"Bar", "Position"},
+            "Position": {"Program"},
+            "Program": {"Pitch", "PitchDrum"},
+            "Pitch": {"Pitch", "Program", "Bar", "Position"},
+            "PitchDrum": {"PitchDrum", "Program", "Bar", "Position"},
         }
 
         if self.config.use_chords:
-            dic["Program"] += ["Chord"]
-            dic["Chord"] = ["Pitch"]
+            dic["Program"] |= {"Chord"}
+            dic["Chord"] = {"Pitch"}
 
         return dic
 
     def _tokens_errors(self, tokens: list[list[str]]) -> int:
         r"""
         Return the number of errors in a sequence of tokens.
 
         The method checks if a sequence of tokens is made of good token types
         successions and values. The number of errors should not be higher than the
         number of tokens.
 
         This method is intended to be overridden by tokenizer classes. The
-        implementation in the ``MIDITokenizer`` class will check token types,
+        implementation in the ``MusicTokenizer`` class will check token types,
         duplicated notes and time errors. It works for ``REMI``, ``TSD`` and
         ``Structured``.
 
         :param tokens: sequence of tokens string to check.
         :return: the number of errors predicted (no more than one per token).
         """
         err = 0
```

### Comparing `miditok-3.0.2/miditok/tokenizations/octuple.py` & `miditok-3.0.3/miditok/tokenizations/octuple.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 from __future__ import annotations
 
 from symusic import Note, Score, Tempo, TimeSignature, Track
 
 from miditok.classes import Event, TokSequence
 from miditok.constants import MIDI_INSTRUMENTS, TIME_SIGNATURE
-from miditok.midi_tokenizer import MIDITokenizer
+from miditok.midi_tokenizer import MusicTokenizer
 from miditok.utils import compute_ticks_per_bar, compute_ticks_per_beat, get_bars_ticks
 
 
-class Octuple(MIDITokenizer):
+class Octuple(MusicTokenizer):
     r"""
     Octuple tokenizer.
 
     Introduced with `MusicBert (Zeng et al.) <https://arxiv.org/abs/2106.05630>`_,
     the idea of Octuple is to use embedding pooling so that each pooled embedding
     represents a single note. Tokens (*Pitch*, *Velocity*...) are first independently
     converted to embeddings which are then merged (pooled) into a single one.
@@ -45,28 +45,27 @@
         cannot represent time signature accurately, hence some unavoidable errors of
         conversion can happen. **For this reason, Octuple is implemented with Time
         Signature but tested without.**
     * Tokens are first sorted by time, then track, then pitch values.
     * Tracks with the same *Program* will be merged.
     * When decoding multiple token sequences (of multiple tracks), i.e. when
         `config.use_programs` is False, only the tempos and time signatures of the
-        first sequence will be decoded for the whole MIDI.
+        first sequence will be decoded for the whole music.
     """
 
     def _tweak_config_before_creating_voc(self) -> None:
         self.config.use_chords = False
         self.config.use_rests = False
         self.config.use_sustain_pedals = False
         self.config.use_pitch_bends = False
         self.config.use_pitch_intervals = False
         self.config.delete_equal_successive_tempo_changes = True
         self.config.program_changes = False
 
         # used in place of positional encoding
-        # This attribute might increase if the tokenizer encounter longer MIDIs
         if "max_bar_embedding" not in self.config.additional_params:
             self.config.additional_params["max_bar_embedding"] = 60
 
         token_types = ["Pitch", "Velocity", "Duration", "Position", "Bar"]
         if self.config.use_programs:
             token_types.append("Program")
         if self.config.use_tempos:
@@ -84,16 +83,16 @@
         Create the time events from a list of global and track events.
 
         Internal method intended to be implemented by child classes.
         The returned sequence is the final token sequence ready to be converted to ids
         to be fed to a model.
 
         :param events: sequence of global and track events to create tokens time from.
-        :param time_division: time division in ticks per quarter of the MIDI being
-            tokenized.
+        :param time_division: time division in ticks per quarter of the
+            ``symusic.Score`` being tokenized.
         :return: the same events, with time events inserted.
         """
         # Add time events
         all_events = []
         current_bar = 0
         current_bar_from_ts_time = 0
         current_tick_from_ts_time = 0
@@ -158,102 +157,109 @@
                             value=f"{current_time_sig[0]}/{current_time_sig[1]}",
                         )
                     )
                 all_events.append(new_event)
 
         return all_events
 
-    def _midi_to_tokens(self, midi: Score) -> TokSequence | list[TokSequence]:
+    def _score_to_tokens(self, score: Score) -> TokSequence | list[TokSequence]:
         r"""
-        Convert a **preprocessed** MIDI object to a sequence of tokens.
+        Convert a **preprocessed** ``symusic.Score`` object to a sequence of tokens.
+
+        We override the parent method in order to check the number of bars in the file.
 
-        We override the parent method in order to check the number of bars in the MIDI.
         The workflow of this method is as follows: the global events (*Tempo*,
         *TimeSignature*...) and track events (*Pitch*, *Velocity*, *Pedal*...) are
         gathered into a list, then the time events are added. If `one_token_stream` is
         ``True``, all events of all tracks are treated all at once, otherwise the
         events of each track are treated independently.
 
-        :param midi: the MIDI :class:`symusic.Score` object to convert.
+        :param score: the :class:`symusic.Score` object to convert.
         :return: a :class:`miditok.TokSequence` if ``tokenizer.one_token_stream`` is
             ``True``, else a list of :class:`miditok.TokSequence` objects.
         """
         # Check bar embedding limit, update if needed
-        num_bars = len(get_bars_ticks(midi))
+        num_bars = len(get_bars_ticks(score))
         if self.config.additional_params["max_bar_embedding"] < num_bars:
-            for i in range(
-                self.config.additional_params["max_bar_embedding"], num_bars
-            ):
-                self.add_to_vocab(f"Bar_{i}", 4)
-            self.config.additional_params["max_bar_embedding"] = num_bars
+            msg = (
+                "miditok: Octuple cannot handle this file, as it contains "
+                f"{num_bars} whereas the limit of the tokenizer is "
+                f"{self.config.additional_params['max_bar_embedding']}"
+            )
+            raise ValueError(msg)
 
-        return super()._midi_to_tokens(midi)
+        return super()._score_to_tokens(score)
 
-    def _tokens_to_midi(
+    def _tokens_to_score(
         self,
         tokens: TokSequence | list[TokSequence],
         programs: list[tuple[int, bool]] | None = None,
     ) -> Score:
         r"""
-        Convert tokens (:class:`miditok.TokSequence`) into a MIDI.
+        Convert tokens (:class:`miditok.TokSequence`) into a ``symusic.Score``.
 
-        This is an internal method called by ``self.tokens_to_midi``, intended to be
-        implemented by classes inheriting :class:`miditok.MidiTokenizer`.
+        This is an internal method called by ``self.decode``, intended to be
+        implemented by classes inheriting :class:`miditok.MusicTokenizer`.
 
         :param tokens: tokens to convert. Can be either a list of
             :class:`miditok.TokSequence` or a list of :class:`miditok.TokSequence`s.
         :param programs: programs of the tracks. If none is given, will default to
             piano, program 0. (default: ``None``)
-        :return: the midi object (:class:`symusic.Score`).
+        :return: the ``symusic.Score`` object.
         """
         # Unsqueeze tokens in case of one_token_stream
         if self.one_token_stream:  # ie single token seq
             tokens = [tokens]
         for i in range(len(tokens)):
             tokens[i] = tokens[i].tokens
-        midi = Score(self.time_division)
+        score = Score(self.time_division)
 
         # RESULTS
         tracks: dict[int, Track] = {}
         tempo_changes, time_signature_changes = [Tempo(-1, self.default_tempo)], []
         tempo_changes[0].tempo = -1
 
         def check_inst(prog: int) -> None:
             if prog not in tracks:
                 tracks[prog] = Track(
                     program=0 if prog == -1 else prog,
                     is_drum=prog == -1,
                     name="Drums" if prog == -1 else MIDI_INSTRUMENTS[prog]["name"],
                 )
 
+        def is_track_empty(track: Track) -> bool:
+            return (
+                len(track.notes) == len(track.controls) == len(track.pitch_bends) == 0
+            )
+
         bar_at_last_ts_change = 0
         tick_at_last_ts_change = 0
         current_program = 0
-        current_instrument = None
+        current_track = None
         for si, seq in enumerate(tokens):
             # First look for the first time signature if needed
             if si == 0 and self.config.use_time_signatures:
                 num, den = self._parse_token_time_signature(
                     seq[0][self.vocab_types_idx["TimeSig"]].split("_")[1]
                 )
                 time_signature_changes.append(TimeSignature(0, num, den))
             else:
                 time_signature_changes.append(TimeSignature(0, *TIME_SIGNATURE))
             current_time_sig = time_signature_changes[0]
             ticks_per_bar = compute_ticks_per_bar(
-                current_time_sig, midi.ticks_per_quarter
+                current_time_sig, score.ticks_per_quarter
             )
             ticks_per_beat = self._tpb_per_ts[current_time_sig.denominator]
             ticks_per_pos = ticks_per_beat // self.config.max_num_pos_per_beat
             # Set track / sequence program if needed
             if not self.one_token_stream:
                 is_drum = False
                 if programs is not None:
                     current_program, is_drum = programs[si]
-                current_instrument = Track(
+                current_track = Track(
                     program=current_program,
                     is_drum=is_drum,
                     name="Drums"
                     if current_program == -1
                     else MIDI_INSTRUMENTS[current_program]["name"],
                 )
 
@@ -301,15 +307,15 @@
                         current_time_sig = TimeSignature(
                             tick_at_last_ts_change, num, den
                         )
                         if si == 0:
                             time_signature_changes.append(current_time_sig)
                         bar_at_last_ts_change = event_bar
                         ticks_per_bar = compute_ticks_per_bar(
-                            current_time_sig, midi.ticks_per_quarter
+                            current_time_sig, score.ticks_per_quarter
                         )
                         ticks_per_beat = self._tpb_per_ts[current_time_sig.denominator]
                         ticks_per_pos = (
                             ticks_per_beat // self.config.max_num_pos_per_beat
                         )
 
                 # Note duration
@@ -319,61 +325,61 @@
 
                 # Append the created note
                 new_note = Note(current_tick, duration, pitch, vel)
                 if self.one_token_stream:
                     check_inst(current_program)
                     tracks[current_program].notes.append(new_note)
                 else:
-                    current_instrument.notes.append(new_note)
+                    current_track.notes.append(new_note)
 
                 # Tempo, adds a TempoChange if necessary
                 if (
                     si == 0
                     and self.config.use_tempos
                     and time_step[self.vocab_types_idx["Tempo"]].split("_")[1] != "None"
                 ):
                     tempo = float(
                         time_step[self.vocab_types_idx["Tempo"]].split("_")[1]
                     )
                     if tempo != round(tempo_changes[-1].tempo, 2):
                         tempo_changes.append(Tempo(current_tick, tempo))
 
-            # Add current_inst to midi and handle notes still active
-            if not self.one_token_stream:
-                midi.tracks.append(current_instrument)
+            # Add current_inst to the score and handle notes still active
+            if not self.one_token_stream and not is_track_empty(current_track):
+                score.tracks.append(current_track)
 
         # Delete mocked
         # And handle first tempo (tick 0) here instead of super
         del tempo_changes[0]
         if len(tempo_changes) == 0 or (
             tempo_changes[0].time != 0
             and round(tempo_changes[0].tempo, 2) != self.default_tempo
         ):
             tempo_changes.insert(0, Tempo(0, self.default_tempo))
         elif round(tempo_changes[0].tempo, 2) == self.default_tempo:
             tempo_changes[0].time = 0
 
-        # create MidiFile
+        # Add global events to the score
         if self.one_token_stream:
-            midi.tracks = list(tracks.values())
-        midi.tempos = tempo_changes
-        midi.time_signatures = time_signature_changes
+            score.tracks = list(tracks.values())
+        score.tempos = tempo_changes
+        score.time_signatures = time_signature_changes
 
-        return midi
+        return score
 
     def _create_base_vocabulary(self) -> list[list[str]]:
         r"""
         Create the vocabulary, as a list of string tokens.
 
         Each token is given as the form ``"Type_Value"``, with its type and value
         separated with an underscore. Example: ``Pitch_58``.
-        The :class:`miditok.MIDITokenizer` main class will then create the "real"
+        The :class:`miditok.MusicTokenizer` main class will then create the "real"
         vocabulary as a dictionary. Special tokens have to be given when creating the
         tokenizer, and will be added to the vocabulary by
-        :class:`miditok.MIDITokenizer`.
+        :class:`miditok.MusicTokenizer`.
 
         :return: the vocabulary as a list of string.
         """
         vocab = [[] for _ in range(5)]
 
         # PITCH
         vocab[0] += [f"Pitch_{i}" for i in range(*self.config.pitch_range)]
@@ -412,15 +418,15 @@
 
         # TIME_SIGNATURE
         if self.config.use_time_signatures:
             vocab.append([f"TimeSig_{i[0]}/{i[1]}" for i in self.time_signatures])
 
         return vocab
 
-    def _create_token_types_graph(self) -> dict[str, list[str]]:
+    def _create_token_types_graph(self) -> dict[str, set[str]]:
         r"""
         Return a graph/dictionary of the possible token types successions.
 
         Not relevant for Octuple as it is not subject to token type errors.
 
         :return: the token types transitions dictionary.
         """
```

### Comparing `miditok-3.0.2/miditok/tokenizations/remi.py` & `miditok-3.0.3/miditok/tokenizations/remi.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,23 +11,23 @@
     Score,
     Tempo,
     TimeSignature,
     Track,
 )
 
 from miditok.classes import Event, TokenizerConfig, TokSequence
-from miditok.constants import MIDI_INSTRUMENTS, TIME_SIGNATURE
-from miditok.midi_tokenizer import MIDITokenizer
+from miditok.constants import MIDI_INSTRUMENTS, TIME_SIGNATURE, USE_BAR_END_TOKENS
+from miditok.midi_tokenizer import MusicTokenizer
 from miditok.utils import compute_ticks_per_bar, compute_ticks_per_beat
 
 if TYPE_CHECKING:
     from pathlib import Path
 
 
-class REMI(MIDITokenizer):
+class REMI(MusicTokenizer):
     r"""
     REMI (Revamped MIDI) tokenizer.
 
     Introduced with the `Pop Music Transformer (Huang and Yang) <https://dl.acm.org/doi/10.1145/3394171.3413671>`_,
     REMI represents notes as successions of *Pitch*, *Velocity* and
     *Duration* tokens, and time with *Bar* and *Position* tokens. A *Bar* token
     indicate that a new bar is beginning, and *Position* the current position within
@@ -41,15 +41,15 @@
 
     **Note:** in the original paper, the tempo information is represented as the
     succession of two token types: a *TempoClass* indicating if the tempo is fast or
     slow, and a *TempoValue* indicating its value. MidiTok only uses one *Tempo* token
     for its value (see :ref:`Additional tokens`).
     **Note:** When decoding multiple token sequences (of multiple tracks), i.e. when
     `config.use_programs` is False, only the tempos and time signatures of the first
-    sequence will be decoded for the whole MIDI.
+    sequence will be decoded for the whole music.
 
     :param tokenizer_config: the tokenizer's configuration, as a
         :class:`miditok.classes.TokenizerConfig` object.
     :param max_bar_embedding: Maximum number of bars ("Bar_0", "Bar_1",...,
         "Bar_{num_bars-1}"). If None passed, creates "Bar_None" token only in
         vocabulary for Bar token.
     :param params: path to a tokenizer config file. This will override other arguments
@@ -64,38 +64,36 @@
         params: str | Path | None = None,
     ) -> None:
         if (
             max_bar_embedding is not None
             and tokenizer_config is not None
             and "max_bar_embedding" not in tokenizer_config.additional_params
         ):
-            # If used, this attribute might increase if the tokenizer encounter longer
-            # MIDIs
             tokenizer_config.additional_params["max_bar_embedding"] = max_bar_embedding
         super().__init__(tokenizer_config, params)
 
     def _tweak_config_before_creating_voc(self) -> None:
         # In case the tokenizer has been created without specifying any config or
         # params file path
         if "max_bar_embedding" not in self.config.additional_params:
-            # If used, this attribute might increase over tokenizations, if the
-            # tokenizer encounter longer MIDIs
             self.config.additional_params["max_bar_embedding"] = None
+        if "use_bar_end_tokens" not in self.config.additional_params:
+            self.config.additional_params["use_bar_end_tokens"] = USE_BAR_END_TOKENS
 
     def _add_time_events(self, events: list[Event], time_division: int) -> list[Event]:
         r"""
         Create the time events from a list of global and track events.
 
         Internal method intended to be implemented by child classes.
         The returned sequence is the final token sequence ready to be converted to ids
         to be fed to a model.
 
         :param events: sequence of global and track events to create tokens time from.
-        :param time_division: time division in ticks per quarter of the MIDI being
-            tokenized.
+        :param time_division: time division in ticks per quarter of the
+            ``symusic.Score`` being tokenized.
         :return: the same events, with time events inserted.
         """
         # Add time events
         all_events = []
         current_bar = -1
         bar_at_last_ts_change = 0
         previous_tick = -1
@@ -164,45 +162,56 @@
 
                 # Bar
                 num_new_bars = (
                     bar_at_last_ts_change
                     + (event.time - tick_at_last_ts_change) // ticks_per_bar
                     - current_bar
                 )
-                if num_new_bars >= 1:
-                    for i in range(num_new_bars):
+                for i in range(num_new_bars):
+                    current_bar += 1
+                    tick_at_current_bar = (
+                        tick_at_last_ts_change
+                        + (current_bar - bar_at_last_ts_change) * ticks_per_bar
+                    )
+                    if (
+                        self.config.additional_params["use_bar_end_tokens"]
+                        and current_bar > 0
+                    ):
                         all_events.append(
                             Event(
                                 type_="Bar",
-                                value=str(current_bar + i + 1)
-                                if self.config.additional_params["max_bar_embedding"]
-                                is not None
-                                else "None",
-                                time=(current_bar + i + 1) * ticks_per_bar,
+                                value="End",
+                                time=tick_at_current_bar - 1,
                                 desc=0,
                             )
                         )
-                        # Add a TimeSignature token, except for the last new Bar token
-                        # if the current event is a TS
-                        if self.config.use_time_signatures and not (
-                            event.type_ == "TimeSig" and i + 1 == num_new_bars
-                        ):
-                            all_events.append(
-                                Event(
-                                    type_="TimeSig",
-                                    value=f"{current_time_sig[0]}/{current_time_sig[1]}",
-                                    time=(current_bar + i + 1) * ticks_per_bar,
-                                    desc=0,
-                                )
-                            )
-                    current_bar += num_new_bars
-                    tick_at_current_bar = (
-                        tick_at_last_ts_change
-                        + (current_bar - bar_at_last_ts_change) * ticks_per_bar
+                    all_events.append(
+                        Event(
+                            type_="Bar",
+                            value=str(current_bar + i)
+                            if self.config.additional_params["max_bar_embedding"]
+                            is not None
+                            else "None",
+                            time=tick_at_current_bar,
+                            desc=0,
+                        )
                     )
+                    # Add a TimeSignature token, except for the last new Bar token
+                    # if the current event is a TS
+                    if self.config.use_time_signatures and not (
+                        event.type_ == "TimeSig" and i + 1 == num_new_bars
+                    ):
+                        all_events.append(
+                            Event(
+                                type_="TimeSig",
+                                value=f"{current_time_sig[0]}/{current_time_sig[1]}",
+                                time=tick_at_current_bar,
+                                desc=0,
+                            )
+                        )
 
                 # Position
                 if event.type_ != "TimeSig":
                     pos_index = (event.time - tick_at_current_bar) // ticks_per_pos
                     all_events.append(
                         Event(
                             type_="Position",
@@ -251,51 +260,56 @@
                 "PitchBend",
                 "Chord",
             }:
                 previous_note_end = max(previous_note_end, event.time)
 
         return all_events
 
-    def _tokens_to_midi(
+    def _tokens_to_score(
         self,
         tokens: TokSequence | list[TokSequence],
         programs: list[tuple[int, bool]] | None = None,
     ) -> Score:
         r"""
-        Convert tokens (:class:`miditok.TokSequence`) into a MIDI.
+        Convert tokens (:class:`miditok.TokSequence`) into a ``symusic.Score``.
 
-        This is an internal method called by ``self.tokens_to_midi``, intended to be
-        implemented by classes inheriting :class:`miditok.MidiTokenizer`.
+        This is an internal method called by ``self.decode``, intended to be
+        implemented by classes inheriting :class:`miditok.MusicTokenizer`.
 
         :param tokens: tokens to convert. Can be either a list of
             :class:`miditok.TokSequence` or a list of :class:`miditok.TokSequence`s.
         :param programs: programs of the tracks. If none is given, will default to
             piano, program 0. (default: ``None``)
-        :return: the midi object (:class:`symusic.Score`).
+        :return: the ``symusic.Score`` object.
         """
         # Unsqueeze tokens in case of one_token_stream
         if self.one_token_stream:  # ie single token seq
             tokens = [tokens]
         for i in range(len(tokens)):
             tokens[i] = tokens[i].tokens
-        midi = Score(self.time_division)
+        score = Score(self.time_division)
 
         # RESULTS
         tracks: dict[int, Track] = {}
         tempo_changes, time_signature_changes = [], []
 
         def check_inst(prog: int) -> None:
             if prog not in tracks:
                 tracks[prog] = Track(
                     program=0 if prog == -1 else prog,
                     is_drum=prog == -1,
                     name="Drums" if prog == -1 else MIDI_INSTRUMENTS[prog]["name"],
                 )
 
-        current_instrument = None
+        def is_track_empty(track: Track) -> bool:
+            return (
+                len(track.notes) == len(track.controls) == len(track.pitch_bends) == 0
+            )
+
+        current_track = None
         for si, seq in enumerate(tokens):
             # First look for the first time signature if needed
             if si == 0:
                 if self.config.use_time_signatures:
                     for token in seq:
                         tok_type, tok_val = token.split("_")
                         if tok_type == "TimeSig":
@@ -312,15 +326,15 @@
                             "Pedal",
                         ]:
                             break
                 if len(time_signature_changes) == 0:
                     time_signature_changes.append(TimeSignature(0, *TIME_SIGNATURE))
             current_time_sig = time_signature_changes[-1]
             ticks_per_bar = compute_ticks_per_bar(
-                current_time_sig, midi.ticks_per_quarter
+                current_time_sig, score.ticks_per_quarter
             )
             ticks_per_beat = self._tpb_per_ts[current_time_sig.denominator]
             ticks_per_pos = ticks_per_beat // self.config.max_num_pos_per_beat
 
             # Set tracking variables
             current_tick = tick_at_last_ts_change = tick_at_current_bar = 0
             current_bar = -1
@@ -332,26 +346,26 @@
             active_pedals = {}
 
             # Set track / sequence program if needed
             if not self.one_token_stream:
                 is_drum = False
                 if programs is not None:
                     current_program, is_drum = programs[si]
-                current_instrument = Track(
+                current_track = Track(
                     program=current_program,
                     is_drum=is_drum,
                     name="Drums"
                     if current_program == -1
                     else MIDI_INSTRUMENTS[current_program]["name"],
                 )
 
             # Decode tokens
             for ti, token in enumerate(seq):
                 tok_type, tok_val = token.split("_")
-                if tok_type == "Bar":
+                if token == "Bar_None":
                     current_bar += 1
                     if current_bar > 0:
                         current_tick = tick_at_current_bar + ticks_per_bar
                     tick_at_current_bar = current_tick
                 elif tok_type == "Rest":
                     current_tick = max(previous_note_end, current_tick)
                     current_tick += self._tpb_rests_to_ticks[ticks_per_beat][tok_val]
@@ -409,25 +423,31 @@
                                 pitch,
                                 int(vel),
                             )
                             if self.one_token_stream:
                                 check_inst(current_program)
                                 tracks[current_program].notes.append(new_note)
                             else:
-                                current_instrument.notes.append(new_note)
+                                current_track.notes.append(new_note)
                             previous_note_end = max(
                                 previous_note_end, current_tick + dur
                             )
                     except IndexError:
                         # A well constituted sequence should not raise an exception
                         # However with generated sequences this can happen, or if the
                         # sequence isn't finished
                         pass
                 elif tok_type == "Program":
                     current_program = int(tok_val)
+                    if not self.one_token_stream and self.config.program_changes:
+                        if current_program != -1:
+                            current_track.program = current_program
+                        else:
+                            current_track.program = 0
+                            current_track.is_drum = True
                 elif tok_type == "Tempo":
                     if si == 0:
                         tempo_changes.append(Tempo(current_tick, float(tok_val)))
                     previous_note_end = max(previous_note_end, current_tick)
                 elif tok_type == "TimeSig":
                     num, den = self._parse_token_time_signature(tok_val)
                     if (
@@ -436,15 +456,15 @@
                     ):
                         current_time_sig = TimeSignature(current_tick, num, den)
                         if si == 0:
                             time_signature_changes.append(current_time_sig)
                         tick_at_last_ts_change = tick_at_current_bar  # == current_tick
                         bar_at_last_ts_change = current_bar
                         ticks_per_bar = compute_ticks_per_bar(
-                            current_time_sig, midi.ticks_per_quarter
+                            current_time_sig, score.ticks_per_quarter
                         )
                         ticks_per_beat = self._tpb_per_ts[den]
                         ticks_per_pos = (
                             ticks_per_beat // self.config.max_num_pos_per_beat
                         )
                 elif tok_type == "Pedal":
                     pedal_prog = (
@@ -458,80 +478,77 @@
                             # Add instrument if it doesn't exist, can happen for the
                             # first tokens
                             new_pedal = Pedal(current_tick, duration)
                             if self.one_token_stream:
                                 check_inst(pedal_prog)
                                 tracks[pedal_prog].pedals.append(new_pedal)
                             else:
-                                current_instrument.pedals.append(new_pedal)
+                                current_track.pedals.append(new_pedal)
                     elif pedal_prog not in active_pedals:
                         active_pedals[pedal_prog] = current_tick
                 elif tok_type == "PedalOff":
                     pedal_prog = (
                         int(tok_val) if self.config.use_programs else current_program
                     )
                     if pedal_prog in active_pedals:
                         new_pedal = Pedal(
                             active_pedals[pedal_prog],
                             current_tick - active_pedals[pedal_prog],
                         )
                         if self.one_token_stream:
                             check_inst(pedal_prog)
-                            tracks[pedal_prog].pedals.append(
-                                Pedal(
-                                    active_pedals[pedal_prog],
-                                    current_tick - active_pedals[pedal_prog],
-                                )
-                            )
+                            tracks[pedal_prog].pedals.append(new_pedal)
                         else:
-                            current_instrument.pedals.append(new_pedal)
+                            current_track.pedals.append(new_pedal)
                         del active_pedals[pedal_prog]
                 elif tok_type == "PitchBend":
                     new_pitch_bend = PitchBend(current_tick, int(tok_val))
                     if self.one_token_stream:
                         check_inst(current_program)
                         tracks[current_program].pitch_bends.append(new_pitch_bend)
                     else:
-                        current_instrument.pitch_bends.append(new_pitch_bend)
+                        current_track.pitch_bends.append(new_pitch_bend)
 
-            # Add current_inst to midi and handle notes still active
-            if not self.one_token_stream:
-                midi.tracks.append(current_instrument)
+            # Add current_inst to score and handle notes still active
+            if not self.one_token_stream and not is_track_empty(current_track):
+                score.tracks.append(current_track)
 
-        # create MidiFile
+        # Add global events to the score
         if self.one_token_stream:
-            midi.tracks = list(tracks.values())
-        midi.tempos = tempo_changes
-        midi.time_signatures = time_signature_changes
+            score.tracks = list(tracks.values())
+        score.tempos = tempo_changes
+        score.time_signatures = time_signature_changes
 
-        return midi
+        return score
 
     def _create_base_vocabulary(self) -> list[str]:
         r"""
         Create the vocabulary, as a list of string tokens.
 
         Each token is given as the form ``"Type_Value"``, with its type and value
         separated with an underscore. Example: ``Pitch_58``.
-        The :class:`miditok.MIDITokenizer` main class will then create the "real"
+        The :class:`miditok.MusicTokenizer` main class will then create the "real"
         vocabulary as a dictionary. Special tokens have to be given when creating the
         tokenizer, and will be added to the vocabulary by
-        :class:`miditok.MIDITokenizer`.
+        :class:`miditok.MusicTokenizer`.
 
         :return: the vocabulary as a list of string.
         """
         vocab = []
 
         # Bar
         if self.config.additional_params["max_bar_embedding"] is not None:
             vocab += [
                 f"Bar_{i}"
                 for i in range(self.config.additional_params["max_bar_embedding"])
             ]
         else:
             vocab += ["Bar_None"]
+        if self.config.additional_params["use_bar_end_tokens"]:
+            vocab.append("Bar_End")
 
         # NoteOn/NoteOff/Velocity
         self._add_note_tokens_to_vocab_list(vocab)
 
         # Position
         # self.time_division is equal to the maximum possible ticks/beat value.
         max_num_beats = max(ts[0] for ts in self.time_signatures)
@@ -539,173 +556,178 @@
         vocab += [f"Position_{i}" for i in range(num_positions)]
 
         # Add additional tokens
         self._add_additional_tokens_to_vocab_list(vocab)
 
         return vocab
 
-    def _create_token_types_graph(self) -> dict[str, list[str]]:
+    def _create_token_types_graph(self) -> dict[str, set[str]]:
         r"""
         Return a graph/dictionary of the possible token types successions.
 
         :return: the token types transitions dictionary.
         """
-        dic: dict[str, list[str]] = {}
+        dic: dict[str, set[str]] = {}
 
         if self.config.use_programs:
             first_note_token_type = (
                 "Pitch" if self.config.program_changes else "Program"
             )
-            dic["Program"] = ["Pitch"]
+            dic["Program"] = {"Pitch"}
         else:
             first_note_token_type = "Pitch"
-        dic["Pitch"] = ["Velocity"]
-        dic["Velocity"] = ["Duration"]
-        dic["Duration"] = [first_note_token_type, "Position", "Bar"]
-        dic["Bar"] = ["Position", "Bar"]
-        dic["Position"] = [first_note_token_type]
+        dic["Pitch"] = {"Velocity"}
+        dic["Velocity"] = {"Duration"}
+        dic["Duration"] = {first_note_token_type, "Position", "Bar"}
+        dic["Bar"] = {"Position", "Bar"}
+        dic["Position"] = {first_note_token_type}
         if self.config.use_pitch_intervals:
             for token_type in ("PitchIntervalTime", "PitchIntervalChord"):
-                dic[token_type] = ["Velocity"]
-                if self.config.use_programs:
-                    dic["Program"].append(token_type)
+                dic[token_type] = {"Velocity"}
+                if (
+                    self.config.use_programs
+                    and self.config.one_token_stream_for_programs
+                ):
+                    dic["Program"].add(token_type)
                 else:
-                    dic["Duration"].append(token_type)
-                    dic["Position"].append(token_type)
+                    dic["Duration"].add(token_type)
+                    dic["Position"].add(token_type)
         if self.config.program_changes:
-            dic["Duration"].append("Program")
+            dic["Duration"].add("Program")
 
         if self.config.use_chords:
-            dic["Chord"] = [first_note_token_type]
-            dic["Position"] += ["Chord"]
+            dic["Chord"] = {first_note_token_type}
+            dic["Position"] |= {"Chord"}
             if self.config.use_programs:
-                dic["Program"].append("Chord")
+                dic["Program"].add("Chord")
             if self.config.use_pitch_intervals:
-                dic["Chord"] += ["PitchIntervalTime", "PitchIntervalChord"]
+                dic["Chord"] |= {"PitchIntervalTime", "PitchIntervalChord"}
 
         if self.config.use_tempos:
-            dic["Position"] += ["Tempo"]
-            dic["Tempo"] = [first_note_token_type, "Position", "Bar"]
+            dic["Position"] |= {"Tempo"}
+            dic["Tempo"] = {first_note_token_type, "Position", "Bar"}
             if self.config.use_chords:
-                dic["Tempo"] += ["Chord"]
+                dic["Tempo"] |= {"Chord"}
             if self.config.use_rests:
-                dic["Tempo"].append("Rest")  # only for first token
+                dic["Tempo"].add("Rest")  # only for first token
             if self.config.use_pitch_intervals:
-                dic["Tempo"] += ["PitchIntervalTime", "PitchIntervalChord"]
+                dic["Tempo"] |= {"PitchIntervalTime", "PitchIntervalChord"}
 
         if self.config.use_time_signatures:
-            dic["Bar"] = ["TimeSig"]
-            dic["TimeSig"] = [first_note_token_type, "Position", "Bar"]
+            dic["Bar"] = {"TimeSig"}
+            if self.config.additional_params["use_bar_end_tokens"]:
+                dic["Bar"].add("Bar")
+            dic["TimeSig"] = {first_note_token_type, "Position", "Bar"}
             if self.config.use_chords:
-                dic["TimeSig"] += ["Chord"]
+                dic["TimeSig"] |= {"Chord"}
             if self.config.use_rests:
-                dic["TimeSig"].append("Rest")  # only for first token
+                dic["TimeSig"].add("Rest")  # only for first token
             if self.config.use_tempos:
-                dic["Tempo"].append("TimeSig")
+                dic["Tempo"].add("TimeSig")
             if self.config.use_pitch_intervals:
-                dic["TimeSig"] += ["PitchIntervalTime", "PitchIntervalChord"]
+                dic["TimeSig"] |= {"PitchIntervalTime", "PitchIntervalChord"}
 
         if self.config.use_sustain_pedals:
-            dic["Position"].append("Pedal")
+            dic["Position"].add("Pedal")
             if self.config.sustain_pedal_duration:
-                dic["Pedal"] = ["Duration"]
-                dic["Duration"].append("Pedal")
+                dic["Pedal"] = {"Duration"}
+                dic["Duration"].add("Pedal")
             else:
-                dic["PedalOff"] = [
+                dic["PedalOff"] = {
                     "Pedal",
                     "PedalOff",
                     first_note_token_type,
                     "Position",
                     "Bar",
-                ]
-                dic["Pedal"] = ["Pedal", first_note_token_type, "Position", "Bar"]
-                dic["Position"].append("PedalOff")
+                }
+                dic["Pedal"] = {"Pedal", first_note_token_type, "Position", "Bar"}
+                dic["Position"].add("PedalOff")
             if self.config.use_chords:
-                dic["Pedal"].append("Chord")
+                dic["Pedal"].add("Chord")
                 if not self.config.sustain_pedal_duration:
-                    dic["PedalOff"].append("Chord")
-                    dic["Chord"].append("PedalOff")
+                    dic["PedalOff"].add("Chord")
+                    dic["Chord"].add("PedalOff")
             if self.config.use_rests:
-                dic["Pedal"].append("Rest")
+                dic["Pedal"].add("Rest")
                 if not self.config.sustain_pedal_duration:
-                    dic["PedalOff"].append("Rest")
+                    dic["PedalOff"].add("Rest")
             if self.config.use_tempos:
-                dic["Tempo"].append("Pedal")
+                dic["Tempo"].add("Pedal")
                 if not self.config.sustain_pedal_duration:
-                    dic["Tempo"].append("PedalOff")
+                    dic["Tempo"].add("PedalOff")
             if self.config.use_time_signatures:
-                dic["TimeSig"].append("Pedal")
+                dic["TimeSig"].add("Pedal")
                 if not self.config.sustain_pedal_duration:
-                    dic["TimeSig"].append("PedalOff")
+                    dic["TimeSig"].add("PedalOff")
             if self.config.use_pitch_intervals:
                 if self.config.sustain_pedal_duration:
-                    dic["Duration"] += ["PitchIntervalTime", "PitchIntervalChord"]
+                    dic["Duration"] |= {"PitchIntervalTime", "PitchIntervalChord"}
                 else:
-                    dic["Pedal"] += ["PitchIntervalTime", "PitchIntervalChord"]
-                    dic["PedalOff"] += ["PitchIntervalTime", "PitchIntervalChord"]
+                    dic["Pedal"] |= {"PitchIntervalTime", "PitchIntervalChord"}
+                    dic["PedalOff"] |= {"PitchIntervalTime", "PitchIntervalChord"}
 
         if self.config.use_pitch_bends:
             # As a Program token will precede PitchBend otherwise
             # Else no need to add Program as its already in
-            dic["PitchBend"] = [first_note_token_type, "Position", "Bar"]
+            dic["PitchBend"] = {first_note_token_type, "Position", "Bar"}
             if self.config.use_programs and not self.config.program_changes:
-                dic["Program"].append("PitchBend")
+                dic["Program"].add("PitchBend")
             else:
-                dic["Position"].append("PitchBend")
+                dic["Position"].add("PitchBend")
                 if self.config.use_tempos:
-                    dic["Tempo"].append("PitchBend")
+                    dic["Tempo"].add("PitchBend")
                 if self.config.use_time_signatures:
-                    dic["TimeSig"].append("PitchBend")
+                    dic["TimeSig"].add("PitchBend")
                 if self.config.use_sustain_pedals:
-                    dic["Pedal"].append("PitchBend")
+                    dic["Pedal"].add("PitchBend")
                     if self.config.sustain_pedal_duration:
-                        dic["Duration"].append("PitchBend")
+                        dic["Duration"].add("PitchBend")
                     else:
-                        dic["PedalOff"].append("PitchBend")
+                        dic["PedalOff"].add("PitchBend")
             if self.config.use_chords:
-                dic["PitchBend"].append("Chord")
+                dic["PitchBend"].add("Chord")
             if self.config.use_rests:
-                dic["PitchBend"].append("Rest")
+                dic["PitchBend"].add("Rest")
 
         if self.config.use_rests:
-            dic["Rest"] = ["Rest", first_note_token_type, "Position", "Bar"]
-            dic["Duration"].append("Rest")
+            dic["Rest"] = {"Rest", first_note_token_type, "Position", "Bar"}
+            dic["Duration"].add("Rest")
             if self.config.use_chords:
-                dic["Rest"] += ["Chord"]
+                dic["Rest"] |= {"Chord"}
             if self.config.use_tempos:
-                dic["Rest"].append("Tempo")
+                dic["Rest"].add("Tempo")
             if self.config.use_time_signatures:
-                dic["Rest"].append("TimeSig")
+                dic["Rest"].add("TimeSig")
             if self.config.use_sustain_pedals:
-                dic["Rest"].append("Pedal")
+                dic["Rest"].add("Pedal")
                 if self.config.sustain_pedal_duration:
-                    dic["Duration"].append("Rest")
+                    dic["Duration"].add("Rest")
                 else:
-                    dic["Rest"].append("PedalOff")
-                    dic["PedalOff"].append("Rest")
+                    dic["Rest"].add("PedalOff")
+                    dic["PedalOff"].add("Rest")
             if self.config.use_pitch_bends:
-                dic["Rest"].append("PitchBend")
+                dic["Rest"].add("PitchBend")
             if self.config.use_pitch_intervals:
-                dic["Rest"] += ["PitchIntervalTime", "PitchIntervalChord"]
+                dic["Rest"] |= {"PitchIntervalTime", "PitchIntervalChord"}
 
         if self.config.program_changes:
-            for token_type in [
+            for token_type in {
                 "Position",
                 "Rest",
                 "PitchBend",
                 "Pedal",
                 "PedalOff",
                 "Tempo",
                 "TimeSig",
                 "Chord",
-            ]:
+            }:
                 if token_type in dic:
-                    dic["Program"].append(token_type)
-                    dic[token_type].append("Program")
+                    dic["Program"].add(token_type)
+                    dic[token_type].add("Program")
 
         if self.config.use_pitchdrum_tokens:
             dic["PitchDrum"] = dic["Pitch"]
             for key, values in dic.items():
                 if "Pitch" in values:
-                    dic[key].append("PitchDrum")
+                    dic[key].add("PitchDrum")
 
         return dic
```

### Comparing `miditok-3.0.2/miditok/tokenizations/structured.py` & `miditok-3.0.3/miditok/tokenizations/structured.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 from __future__ import annotations
 
 import numpy as np
 from symusic import Note, Score, Track
 
 from miditok.classes import Event, TokSequence
 from miditok.constants import MIDI_INSTRUMENTS
-from miditok.midi_tokenizer import MIDITokenizer
+from miditok.midi_tokenizer import MusicTokenizer
 from miditok.utils.utils import np_get_closest
 
 
-class Structured(MIDITokenizer):
+class Structured(MusicTokenizer):
     r"""
     Structured tokenizer, with a recurrent token type succession.
 
     Introduced with the `Piano Inpainting Application <https://arxiv.org/abs/2002.00212>`_,
     it is similar to :ref:`TSD` but is based on a consistent token type successions.
     Token types always follow the same pattern: *Pitch* -> *Velocity* -> *Duration* ->
     *TimeShift*. The latter is set to 0 for simultaneous notes. To keep this property,
@@ -43,24 +43,24 @@
     def _create_track_events(self, track: Track, _: None = None) -> list[Event]:
         r"""
         Extract the tokens/events from a track (``symusic.Track``).
 
         Concerned events are: *Pitch*, *Velocity*, *Duration*, *NoteOn*, *NoteOff* and
         optionally *Chord*, *Pedal* and *PitchBend*.
         **If the tokenizer is using pitch intervals, the notes must be sorted by time
-        then pitch values. This is done in** ``preprocess_midi``.
+        then pitch values. This is done in** ``preprocess_score``.
 
         :param track: ``symusic.Track`` to extract events from.
         :param _: in place of ``ticks_per_beat``, unused here as Structured do not
             support time signatures, hence the ticks_per_beat value is always the same
-            and equal to the MIDI's time division.
+            and equal to the Score's time division.
         :return: sequence of corresponding ``Event``s.
         """
         # Make sure the notes are sorted first by their onset (start) times, second by
-        # pitch: notes.sort(key=lambda x: (x.start, x.pitch)) done in midi_to_tokens
+        # pitch: notes.sort(key=lambda x: (x.start, x.pitch)) done in preprocess_score
         program = track.program if not track.is_drum else -1
         events = []
 
         # Creates the Note On, Note Off and Velocity events
         previous_tick = 0
         ticks_per_beat = self.time_division
         for note in track.notes:
@@ -134,16 +134,16 @@
         Create the time events from a list of global and track events.
 
         Internal method intended to be implemented by child classes.
         The returned sequence is the final token sequence ready to be converted to ids
         to be fed to a model.
 
         :param events: sequence of global and track events to create tokens time from.
-        :param time_division: time division in ticks per quarter of the MIDI being
-            tokenized.
+        :param time_division: time division in ticks per quarter of the
+            ``symusic.Score`` being tokenized.
         :return: the same events, with time events inserted.
         """
         all_events = []
         token_types_to_check = (
             {"Program"} if self.one_token_stream else {"Pitch", "PitchDrum"}
         )
 
@@ -175,106 +175,117 @@
                 )
                 previous_tick = event.time
 
             all_events.append(event)
 
         return all_events
 
-    def _midi_to_tokens(self, midi: Score) -> TokSequence | list[TokSequence]:
+    def _score_to_tokens(self, score: Score) -> TokSequence | list[TokSequence]:
         r"""
-        Convert a **preprocessed** MIDI object to a sequence of tokens.
+        Convert a **preprocessed** ``symusic.Score`` object to a sequence of tokens.
 
         We override the parent method to handle the "non-program" case where
         *TimeShift* events have already been added by `_notes_to_events`.
         The workflow of this method is as follows: the global events (*Tempo*,
         *TimeSignature*...) and track events (*Pitch*, *Velocity*, *Pedal*...) are
         gathered into a list, then the time events are added. If `one_token_stream` is
         ``True``, all events of all tracks are treated all at once, otherwise the
         events of each track are treated independently.
 
-        :param midi: the MIDI :class:`symusic.Score` object to convert.
+        The workflow of this method is as follows: the global events (*Tempo*,
+        *TimeSignature*...) and track events (*Pitch*, *Velocity*, *Pedal*...) are
+        gathered into a list, then the time events are added. If `one_token_stream` is
+        ``True``, all events of all tracks are treated all at once, otherwise the
+        events of each track are treated independently.
+
+        :param score: the :class:`symusic.Score` object to convert.
         :return: a :class:`miditok.TokSequence` if ``tokenizer.one_token_stream`` is
             ``True``, else a list of :class:`miditok.TokSequence` objects.
         """
         # Convert each track to tokens
         all_events = []
 
         # Adds note tokens
-        if not self.one_token_stream and len(midi.tracks) == 0:
+        if not self.one_token_stream and len(score.tracks) == 0:
             all_events.append([])
-        for track in midi.tracks:
+        for track in score.tracks:
             note_events = self._create_track_events(track)
             if self.one_token_stream:
                 all_events += note_events
             else:
                 all_events.append(note_events)
 
         # Add time events
         if self.one_token_stream:
-            if len(midi.tracks) > 1:
+            if len(score.tracks) > 1:
                 all_events.sort(key=lambda x: x.time)
-            all_events = self._add_time_events(all_events, midi.ticks_per_quarter)
+            all_events = self._add_time_events(all_events, score.ticks_per_quarter)
             tok_sequence = TokSequence(events=all_events)
             self.complete_sequence(tok_sequence)
         else:
             tok_sequence = []
             for i in range(len(all_events)):
                 # No call to __add_time_note_events here as not needed
                 tok_sequence.append(TokSequence(events=all_events[i]))
                 self.complete_sequence(tok_sequence[-1])
 
         return tok_sequence
 
-    def _tokens_to_midi(
+    def _tokens_to_score(
         self,
         tokens: TokSequence | list[TokSequence],
         programs: list[tuple[int, bool]] | None = None,
     ) -> Score:
         r"""
-        Convert tokens (:class:`miditok.TokSequence`) into a MIDI.
+        Convert tokens (:class:`miditok.TokSequence`) into a ``symusic.Score``.
 
-        This is an internal method called by ``self.tokens_to_midi``, intended to be
-        implemented by classes inheriting :class:`miditok.MidiTokenizer`.
+        This is an internal method called by ``self.decode``, intended to be
+        implemented by classes inheriting :class:`miditok.MusicTokenizer`.
 
         :param tokens: tokens to convert. Can be either a list of
             :class:`miditok.TokSequence` or a list of :class:`miditok.TokSequence`s.
         :param programs: programs of the tracks. If none is given, will default to
             piano, program 0. (default: ``None``)
-        :return: the midi object (:class:`symusic.Score`).
+        :return: the ``symusic.Score`` object.
         """
         # Unsqueeze tokens in case of one_token_stream
         if self.one_token_stream:  # ie single token seq
             tokens = [tokens]
         for i in range(len(tokens)):
             tokens[i] = tokens[i].tokens
-        midi = Score(self.time_division)
+        score = Score(self.time_division)
 
         # RESULTS
         instruments: dict[int, Track] = {}
 
         def check_inst(prog: int) -> None:
             if prog not in instruments:
                 instruments[prog] = Track(
                     program=0 if prog == -1 else prog,
                     is_drum=prog == -1,
                     name="Drums" if prog == -1 else MIDI_INSTRUMENTS[prog]["name"],
                 )
 
+        def is_track_empty(track: Track) -> bool:
+            return (
+                len(track.notes) == len(track.controls) == len(track.pitch_bends) == 0
+            )
+
         current_tick = 0
         current_program = 0
-        current_instrument = None
-        ticks_per_beat = midi.ticks_per_quarter
+        current_track = None
+        ticks_per_beat = score.ticks_per_quarter
         for si, seq in enumerate(tokens):
             # Set track / sequence program if needed
             if not self.one_token_stream:
                 current_tick = 0
                 is_drum = False
                 if programs is not None:
                     current_program, is_drum = programs[si]
-                current_instrument = Track(
+                current_track = Track(
                     program=current_program,
                     is_drum=is_drum,
                     name="Drums"
                     if current_program == -1
                     else MIDI_INSTRUMENTS[current_program]["name"],
                 )
 
@@ -295,43 +306,42 @@
                                 seq[ti + 2].split("_")[1]
                             ]
                             new_note = Note(current_tick, duration, pitch, vel)
                             if self.one_token_stream:
                                 check_inst(current_program)
                                 instruments[current_program].notes.append(new_note)
                             else:
-                                current_instrument.notes.append(new_note)
+                                current_track.notes.append(new_note)
                     except IndexError:
                         # A well constituted sequence should not raise an exception,
                         # however with generated sequences this can happen, or if the
                         # sequence isn't finished
                         pass
                 elif token_type == "Program":
                     current_program = int(token_val)
 
-            # Add current_inst to midi and handle notes still active
-            if not self.one_token_stream:
-                midi.tracks.append(current_instrument)
+            # Add current_inst to score and handle notes still active
+            if not self.one_token_stream and not is_track_empty(current_track):
+                score.tracks.append(current_track)
 
-        # create MidiFile
         if self.one_token_stream:
-            midi.tracks = list(instruments.values())
+            score.tracks = list(instruments.values())
 
-        return midi
+        return score
 
     def _create_base_vocabulary(self) -> list[str]:
         r"""
         Create the vocabulary, as a list of string tokens.
 
         Each token is given as the form ``"Type_Value"``, with its type and value
         separated with an underscore. Example: ``Pitch_58``.
-        The :class:`miditok.MIDITokenizer` main class will then create the "real"
+        The :class:`miditok.MusicTokenizer` main class will then create the "real"
         vocabulary as a dictionary. Special tokens have to be given when creating the
         tokenizer, and will be added to the vocabulary by
-        :class:`miditok.MIDITokenizer`.
+        :class:`miditok.MusicTokenizer`.
 
         :return: the vocabulary as a list of string.
         """
         vocab = []
 
         # NoteOn/NoteOff/Velocity
         self._add_note_tokens_to_vocab_list(vocab)
@@ -343,24 +353,24 @@
         ]
 
         # Add additional tokens (just Program for Structured)
         self._add_additional_tokens_to_vocab_list(vocab)
 
         return vocab
 
-    def _create_token_types_graph(self) -> dict[str, list[str]]:
+    def _create_token_types_graph(self) -> dict[str, set[str]]:
         r"""
         Return a graph/dictionary of the possible token types successions.
 
         :return: the token types transitions dictionary.
         """
         dic = {
-            "Pitch": ["Velocity"],
-            "PitchDrum": ["Velocity"],
-            "Velocity": ["Duration"],
-            "Duration": ["TimeShift"],
-            "TimeShift": ["Pitch", "PitchDrum"],
+            "Pitch": {"Velocity"},
+            "PitchDrum": {"Velocity"},
+            "Velocity": {"Duration"},
+            "Duration": {"TimeShift"},
+            "TimeShift": {"Pitch", "PitchDrum"},
         }
         if self.config.use_programs:
-            dic["Program"] = ["Pitch", "PitchDrum"]
-            dic["TimeShift"] = ["Program"]
+            dic["Program"] = {"Pitch", "PitchDrum"}
+            dic["TimeShift"] = {"Program"}
         return dic
```

### Comparing `miditok-3.0.2/miditok/tokenizations/tsd.py` & `miditok-3.0.3/miditok/tokenizations/tsd.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,35 +10,35 @@
     Tempo,
     TimeSignature,
     Track,
 )
 
 from miditok.classes import Event, TokSequence
 from miditok.constants import MIDI_INSTRUMENTS, TIME_SIGNATURE
-from miditok.midi_tokenizer import MIDITokenizer
+from miditok.midi_tokenizer import MusicTokenizer
 from miditok.utils import compute_ticks_per_beat
 
 
-class TSD(MIDITokenizer):
+class TSD(MusicTokenizer):
     r"""
     TSD (Time Shift Duration) tokenizer.
 
-    It is similar to MIDI-Like :ref:`MIDI-Like` but uses explicit *Duration* tokens to
+    It is similar to :ref:`MIDI-Like` but uses explicit *Duration* tokens to
     represent note durations, which have showed `better results than with *NoteOff*
     tokens <https://arxiv.org/abs/2002.00212>`_. If you specify ``use_programs`` as
     ``True`` in the config file, the tokenizer will add *Program* tokens before each
     *Pitch* tokens to specify its instrument, and will treat all tracks as a single
     stream of tokens.
 
     **Note:** as ``TSD`` uses *TimeShifts* events to move the time from note to note,
     it can be unsuited for tracks with pauses longer than the maximum *TimeShift*
     value. In such cases, the maximum *TimeShift* value will be used.
     **Note:** When decoding multiple token sequences (of multiple tracks), i.e. when
     ``config.use_programs`` is False, only the tempos and time signatures of the first
-    sequence will be decoded for the whole MIDI.
+    sequence will be decoded for the whole music.
     """
 
     def _tweak_config_before_creating_voc(self) -> None:
         if self.config.use_programs:
             self.one_token_stream = True
 
     def _add_time_events(self, events: list[Event], time_division: int) -> list[Event]:
@@ -46,16 +46,16 @@
         Create the time events from a list of global and track events.
 
         Internal method intended to be implemented by child classes.
         The returned sequence is the final token sequence ready to be converted to ids
         to be fed to a model.
 
         :param events: sequence of global and track events to create tokens time from.
-        :param time_division: time division in ticks per quarter of the MIDI being
-            tokenized.
+        :param time_division: time division in ticks per quarter of the
+        ``symusic.Score`` being tokenized.
         :return: the same events, with time events inserted.
         """
         # Add time events
         all_events = []
         previous_tick = 0
         previous_note_end = 0
         ticks_per_beat = compute_ticks_per_beat(TIME_SIGNATURE[1], time_division)
@@ -125,67 +125,72 @@
                 "PitchBend",
                 "Chord",
             }:
                 previous_note_end = max(previous_note_end, event.time)
 
         return all_events
 
-    def _tokens_to_midi(
+    def _tokens_to_score(
         self,
         tokens: TokSequence | list[TokSequence],
         programs: list[tuple[int, bool]] | None = None,
     ) -> Score:
         r"""
-        Convert tokens (:class:`miditok.TokSequence`) into a MIDI.
+        Convert tokens (:class:`miditok.TokSequence`) into a ``symusic.Score``.
 
-        This is an internal method called by ``self.tokens_to_midi``, intended to be
-        implemented by classes inheriting :class:`miditok.MidiTokenizer`.
+        This is an internal method called by ``self.decode``, intended to be
+        implemented by classes inheriting :class:`miditok.MusicTokenizer`.
 
         :param tokens: tokens to convert. Can be either a list of
             :class:`miditok.TokSequence` or a list of :class:`miditok.TokSequence`s.
         :param programs: programs of the tracks. If none is given, will default to
             piano, program 0. (default: ``None``)
-        :return: the midi object (:class:`symusic.Score`).
+        :return: the ``symusic.Score`` object.
         """
         # Unsqueeze tokens in case of one_token_stream
         if self.one_token_stream:  # ie single token seq
             tokens = [tokens]
         for i in range(len(tokens)):
             tokens[i] = tokens[i].tokens
-        midi = Score(self.time_division)
+        score = Score(self.time_division)
 
         # RESULTS
         tracks: dict[int, Track] = {}
         tempo_changes, time_signature_changes = [], []
 
         def check_inst(prog: int) -> None:
             if prog not in tracks:
                 tracks[prog] = Track(
                     program=0 if prog == -1 else prog,
                     is_drum=prog == -1,
                     name="Drums" if prog == -1 else MIDI_INSTRUMENTS[prog]["name"],
                 )
 
-        current_instrument = None  # only use in when one_token_stream is False
+        def is_track_empty(track: Track) -> bool:
+            return (
+                len(track.notes) == len(track.controls) == len(track.pitch_bends) == 0
+            )
+
+        current_track = None  # only use in when one_token_stream is False
         for si, seq in enumerate(tokens):
             # Set tracking variables
             current_tick = 0
             current_program = 0
             previous_note_end = 0
             previous_pitch_onset = {prog: -128 for prog in self.config.programs}
             previous_pitch_chord = {prog: -128 for prog in self.config.programs}
             active_pedals = {}
-            ticks_per_beat = midi.ticks_per_quarter
+            ticks_per_beat = score.ticks_per_quarter
 
             # Set track / sequence program if needed
             if not self.one_token_stream:
                 is_drum = False
                 if programs is not None:
                     current_program, is_drum = programs[si]
-                current_instrument = Track(
+                current_track = Track(
                     program=current_program,
                     is_drum=is_drum,
                     name="Drums"
                     if current_program == -1
                     else MIDI_INSTRUMENTS[current_program]["name"],
                 )
 
@@ -228,25 +233,31 @@
                         if vel_type == "Velocity" and dur_type == "Duration":
                             dur = self._tpb_tokens_to_ticks[ticks_per_beat][dur]
                             new_note = Note(current_tick, dur, pitch, int(vel))
                             if self.one_token_stream:
                                 check_inst(current_program)
                                 tracks[current_program].notes.append(new_note)
                             else:
-                                current_instrument.notes.append(new_note)
+                                current_track.notes.append(new_note)
                             previous_note_end = max(
                                 previous_note_end, current_tick + dur
                             )
                     except IndexError:
                         # A well constituted sequence should not raise an exception
                         # However with generated sequences this can happen, or if the
                         # sequence isn't finished
                         pass
                 elif tok_type == "Program":
                     current_program = int(tok_val)
+                    if not self.one_token_stream and self.config.program_changes:
+                        if current_program != -1:
+                            current_track.program = current_program
+                        else:
+                            current_track.program = 0
+                            current_track.is_drum = True
                 elif tok_type == "Tempo" and si == 0:
                     tempo_changes.append(Tempo(current_tick, float(tok_val)))
                 elif tok_type == "TimeSig":
                     num, den = self._parse_token_time_signature(tok_val)
                     if si == 0:
                         time_signature_changes.append(
                             TimeSignature(current_tick, num, den)
@@ -264,15 +275,15 @@
                             # Add instrument if it doesn't exist, can happen for the
                             # first tokens
                             new_pedal = Pedal(current_tick, duration)
                             if self.one_token_stream:
                                 check_inst(pedal_prog)
                                 tracks[pedal_prog].pedals.append(new_pedal)
                             else:
-                                current_instrument.pedals.append(new_pedal)
+                                current_track.pedals.append(new_pedal)
                     elif pedal_prog not in active_pedals:
                         active_pedals[pedal_prog] = current_tick
                 elif tok_type == "PedalOff":
                     pedal_prog = (
                         int(tok_val) if self.config.use_programs else current_program
                     )
                     if pedal_prog in active_pedals:
@@ -285,57 +296,57 @@
                             tracks[pedal_prog].pedals.append(
                                 Pedal(
                                     active_pedals[pedal_prog],
                                     current_tick - active_pedals[pedal_prog],
                                 )
                             )
                         else:
-                            current_instrument.pedals.append(new_pedal)
+                            current_track.pedals.append(new_pedal)
                         del active_pedals[pedal_prog]
                 elif tok_type == "PitchBend":
                     new_pitch_bend = PitchBend(current_tick, int(tok_val))
                     if self.one_token_stream:
                         check_inst(current_program)
                         tracks[current_program].pitch_bends.append(new_pitch_bend)
                     else:
-                        current_instrument.pitch_bends.append(new_pitch_bend)
+                        current_track.pitch_bends.append(new_pitch_bend)
 
                 if tok_type in [
                     "Program",
                     "Tempo",
                     "TimeSig",
                     "Pedal",
                     "PedalOff",
                     "PitchBend",
                     "Chord",
                 ]:
                     previous_note_end = max(previous_note_end, current_tick)
 
-            # Add current_inst to midi and handle notes still active
-            if not self.one_token_stream:
-                midi.tracks.append(current_instrument)
+            # Add current_inst to the score and handle notes still active
+            if not self.one_token_stream and not is_track_empty(current_track):
+                score.tracks.append(current_track)
 
-        # create MidiFile
+        # Add global events to the score
         if self.one_token_stream:
-            midi.tracks = list(tracks.values())
-        midi.tempos = tempo_changes
-        midi.time_signatures = time_signature_changes
+            score.tracks = list(tracks.values())
+        score.tempos = tempo_changes
+        score.time_signatures = time_signature_changes
 
-        return midi
+        return score
 
     def _create_base_vocabulary(self) -> list[str]:
         r"""
         Create the vocabulary, as a list of string tokens.
 
         Each token is given as the form ``"Type_Value"``, with its type and value
         separated with an underscore. Example: ``Pitch_58``.
-        The :class:`miditok.MIDITokenizer` main class will then create the "real"
+        The :class:`miditok.MusicTokenizer` main class will then create the "real"
         vocabulary as a dictionary. Special tokens have to be given when creating the
         tokenizer, and will be added to the vocabulary by
-        :class:`miditok.MIDITokenizer`.
+        :class:`miditok.MusicTokenizer`.
 
         :return: the vocabulary as a list of string.
         """
         vocab = []
 
         # NoteOn/NoteOff/Velocity
         self._add_note_tokens_to_vocab_list(vocab)
@@ -347,173 +358,176 @@
         ]
 
         # Add additional tokens
         self._add_additional_tokens_to_vocab_list(vocab)
 
         return vocab
 
-    def _create_token_types_graph(self) -> dict[str, list[str]]:
+    def _create_token_types_graph(self) -> dict[str, set[str]]:
         r"""
         Return a graph/dictionary of the possible token types successions.
 
         :return: the token types transitions dictionary.
         """
-        dic = {}
+        dic: dict[str, set[str]] = {}
 
         if self.config.use_programs:
             first_note_token_type = (
                 "Pitch" if self.config.program_changes else "Program"
             )
-            dic["Program"] = ["Pitch"]
+            dic["Program"] = {"Pitch"}
         else:
             first_note_token_type = "Pitch"
-        dic["Pitch"] = ["Velocity"]
-        dic["Velocity"] = ["Duration"]
-        dic["Duration"] = [first_note_token_type, "TimeShift"]
-        dic["TimeShift"] = [first_note_token_type, "TimeShift"]
+        dic["Pitch"] = {"Velocity"}
+        dic["Velocity"] = {"Duration"}
+        dic["Duration"] = {first_note_token_type, "TimeShift"}
+        dic["TimeShift"] = {first_note_token_type, "TimeShift"}
         if self.config.use_pitch_intervals:
             for token_type in ("PitchIntervalTime", "PitchIntervalChord"):
-                dic[token_type] = ["Velocity"]
-                if self.config.use_programs:
-                    dic["Program"].append(token_type)
+                dic[token_type] = {"Velocity"}
+                if (
+                    self.config.use_programs
+                    and self.config.one_token_stream_for_programs
+                ):
+                    dic["Program"].add(token_type)
                 else:
-                    dic["Duration"].append(token_type)
-                    dic["TimeShift"].append(token_type)
+                    dic["Duration"].add(token_type)
+                    dic["TimeShift"].add(token_type)
         if self.config.program_changes:
-            dic["Duration"].append("Program")
+            dic["Duration"].add("Program")
 
         if self.config.use_chords:
-            dic["Chord"] = [first_note_token_type]
-            dic["TimeShift"] += ["Chord"]
+            dic["Chord"] = {first_note_token_type}
+            dic["TimeShift"] |= {"Chord"}
             if self.config.use_programs:
-                dic["Program"].append("Chord")
+                dic["Program"].add("Chord")
             if self.config.use_pitch_intervals:
-                dic["Chord"] += ["PitchIntervalTime", "PitchIntervalChord"]
+                dic["Chord"] |= {"PitchIntervalTime", "PitchIntervalChord"}
 
         if self.config.use_tempos:
-            dic["TimeShift"] += ["Tempo"]
-            dic["Tempo"] = [first_note_token_type, "TimeShift"]
+            dic["TimeShift"] |= {"Tempo"}
+            dic["Tempo"] = {first_note_token_type, "TimeShift"}
             if self.config.use_chords:
-                dic["Tempo"] += ["Chord"]
+                dic["Tempo"] |= {"Chord"}
             if self.config.use_rests:
-                dic["Tempo"].append("Rest")  # only for first token
+                dic["Tempo"].add("Rest")  # only for first token
             if self.config.use_pitch_intervals:
-                dic["Tempo"] += ["PitchIntervalTime", "PitchIntervalChord"]
+                dic["Tempo"] |= {"PitchIntervalTime", "PitchIntervalChord"}
 
         if self.config.use_time_signatures:
-            dic["TimeShift"] += ["TimeSig"]
-            dic["TimeSig"] = [first_note_token_type, "TimeShift"]
+            dic["TimeShift"] |= {"TimeSig"}
+            dic["TimeSig"] = {first_note_token_type, "TimeShift"}
             if self.config.use_chords:
-                dic["TimeSig"] += ["Chord"]
+                dic["TimeSig"] |= {"Chord"}
             if self.config.use_rests:
-                dic["TimeSig"].append("Rest")  # only for first token
+                dic["TimeSig"].add("Rest")  # only for first token
             if self.config.use_tempos:
-                dic["TimeSig"].append("Tempo")
+                dic["TimeSig"].add("Tempo")
             if self.config.use_pitch_intervals:
-                dic["TimeSig"] += ["PitchIntervalTime", "PitchIntervalChord"]
+                dic["TimeSig"] |= {"PitchIntervalTime", "PitchIntervalChord"}
 
         if self.config.use_sustain_pedals:
-            dic["TimeShift"].append("Pedal")
+            dic["TimeShift"].add("Pedal")
             if self.config.sustain_pedal_duration:
-                dic["Pedal"] = ["Duration"]
-                dic["Duration"].append("Pedal")
+                dic["Pedal"] = {"Duration"}
+                dic["Duration"].add("Pedal")
             else:
-                dic["PedalOff"] = [
+                dic["PedalOff"] = {
                     "Pedal",
                     "PedalOff",
                     first_note_token_type,
                     "TimeShift",
-                ]
-                dic["Pedal"] = ["Pedal", first_note_token_type, "TimeShift"]
-                dic["TimeShift"].append("PedalOff")
+                }
+                dic["Pedal"] = {"Pedal", first_note_token_type, "TimeShift"}
+                dic["TimeShift"].add("PedalOff")
             if self.config.use_chords:
-                dic["Pedal"].append("Chord")
+                dic["Pedal"].add("Chord")
                 if not self.config.sustain_pedal_duration:
-                    dic["PedalOff"].append("Chord")
-                    dic["Chord"].append("PedalOff")
+                    dic["PedalOff"].add("Chord")
+                    dic["Chord"].add("PedalOff")
             if self.config.use_rests:
-                dic["Pedal"].append("Rest")
+                dic["Pedal"].add("Rest")
                 if not self.config.sustain_pedal_duration:
-                    dic["PedalOff"].append("Rest")
+                    dic["PedalOff"].add("Rest")
             if self.config.use_tempos:
-                dic["Tempo"].append("Pedal")
+                dic["Tempo"].add("Pedal")
                 if not self.config.sustain_pedal_duration:
-                    dic["Tempo"].append("PedalOff")
+                    dic["Tempo"].add("PedalOff")
             if self.config.use_time_signatures:
-                dic["TimeSig"].append("Pedal")
+                dic["TimeSig"].add("Pedal")
                 if not self.config.sustain_pedal_duration:
-                    dic["TimeSig"].append("PedalOff")
+                    dic["TimeSig"].add("PedalOff")
             if self.config.use_pitch_intervals:
                 if self.config.sustain_pedal_duration:
-                    dic["Duration"] += ["PitchIntervalTime", "PitchIntervalChord"]
+                    dic["Duration"] |= {"PitchIntervalTime", "PitchIntervalChord"}
                 else:
-                    dic["Pedal"] += ["PitchIntervalTime", "PitchIntervalChord"]
-                    dic["PedalOff"] += ["PitchIntervalTime", "PitchIntervalChord"]
+                    dic["Pedal"] |= {"PitchIntervalTime", "PitchIntervalChord"}
+                    dic["PedalOff"] |= {"PitchIntervalTime", "PitchIntervalChord"}
 
         if self.config.use_pitch_bends:
             # As a Program token will precede PitchBend otherwise
             # Else no need to add Program as its already in
-            dic["PitchBend"] = [first_note_token_type, "TimeShift"]
+            dic["PitchBend"] = {first_note_token_type, "TimeShift"}
             if self.config.use_programs and not self.config.program_changes:
-                dic["Program"].append("PitchBend")
+                dic["Program"].add("PitchBend")
             else:
-                dic["TimeShift"].append("PitchBend")
+                dic["TimeShift"].add("PitchBend")
                 if self.config.use_tempos:
-                    dic["Tempo"].append("PitchBend")
+                    dic["Tempo"].add("PitchBend")
                 if self.config.use_time_signatures:
-                    dic["TimeSig"].append("PitchBend")
+                    dic["TimeSig"].add("PitchBend")
                 if self.config.use_sustain_pedals:
-                    dic["Pedal"].append("PitchBend")
+                    dic["Pedal"].add("PitchBend")
                     if self.config.sustain_pedal_duration:
-                        dic["Duration"].append("PitchBend")
+                        dic["Duration"].add("PitchBend")
                     else:
-                        dic["PedalOff"].append("PitchBend")
+                        dic["PedalOff"].add("PitchBend")
             if self.config.use_chords:
-                dic["PitchBend"].append("Chord")
+                dic["PitchBend"].add("Chord")
             if self.config.use_rests:
-                dic["PitchBend"].append("Rest")
+                dic["PitchBend"].add("Rest")
 
         if self.config.use_rests:
-            dic["Rest"] = ["Rest", first_note_token_type, "TimeShift"]
-            dic["Duration"].append("Rest")
+            dic["Rest"] = {"Rest", first_note_token_type, "TimeShift"}
+            dic["Duration"].add("Rest")
             if self.config.use_chords:
-                dic["Rest"] += ["Chord"]
+                dic["Rest"] |= {"Chord"}
             if self.config.use_tempos:
-                dic["Rest"].append("Tempo")
+                dic["Rest"].add("Tempo")
             if self.config.use_time_signatures:
-                dic["Rest"].append("TimeSig")
+                dic["Rest"].add("TimeSig")
             if self.config.use_sustain_pedals:
-                dic["Rest"].append("Pedal")
+                dic["Rest"].add("Pedal")
                 if self.config.sustain_pedal_duration:
-                    dic["Duration"].append("Rest")
+                    dic["Duration"].add("Rest")
                 else:
-                    dic["Rest"].append("PedalOff")
-                    dic["PedalOff"].append("Rest")
+                    dic["Rest"].add("PedalOff")
+                    dic["PedalOff"].add("Rest")
             if self.config.use_pitch_bends:
-                dic["Rest"].append("PitchBend")
+                dic["Rest"].add("PitchBend")
             if self.config.use_pitch_intervals:
-                dic["Rest"] += ["PitchIntervalTime", "PitchIntervalChord"]
+                dic["Rest"] |= {"PitchIntervalTime", "PitchIntervalChord"}
         else:
-            dic["TimeShift"].append("TimeShift")
+            dic["TimeShift"].add("TimeShift")
 
         if self.config.program_changes:
-            for token_type in [
+            for token_type in {
                 "TimeShift",
                 "Rest",
                 "PitchBend",
                 "Pedal",
                 "PedalOff",
                 "Tempo",
                 "TimeSig",
                 "Chord",
-            ]:
+            }:
                 if token_type in dic:
-                    dic["Program"].append(token_type)
-                    dic[token_type].append("Program")
+                    dic["Program"].add(token_type)
+                    dic[token_type].add("Program")
 
         if self.config.use_pitchdrum_tokens:
             dic["PitchDrum"] = dic["Pitch"]
             for key, values in dic.items():
                 if "Pitch" in values:
-                    dic[key].append("PitchDrum")
+                    dic[key].add("PitchDrum")
 
         return dic
```

### Comparing `miditok-3.0.2/miditok/utils/__init__.py` & `miditok-3.0.3/miditok/utils/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 """Module containing utils methods than can be used outside of tokenization."""
 
 from .utils import (
     compute_ticks_per_bar,
     compute_ticks_per_beat,
-    concat_midis,
+    concat_scores,
     convert_ids_tensors_to_list,
     detect_chords,
-    extract_chunk_from_midi,
+    filter_dataset,
     fix_offsets_overlapping_notes,
     get_bars_ticks,
     get_beats_ticks,
-    get_midi_programs,
-    get_midi_ticks_per_beat,
     get_num_notes_per_bar,
-    merge_midis,
+    get_score_programs,
+    get_score_ticks_per_beat,
     merge_same_program_tracks,
+    merge_scores,
     merge_tracks,
     merge_tracks_per_class,
     num_bar_pos,
     remove_duplicated_notes,
-    split_midi_per_beats,
-    split_midi_per_ticks,
-    split_midi_per_tracks,
+    split_score_per_beats,
+    split_score_per_ticks,
+    split_score_per_tracks,
 )
 
 __all__ = [
     "compute_ticks_per_bar",
     "compute_ticks_per_beat",
-    "concat_midis",
+    "concat_scores",
     "convert_ids_tensors_to_list",
     "detect_chords",
-    "extract_chunk_from_midi",
+    "filter_dataset",
     "fix_offsets_overlapping_notes",
     "get_bars_ticks",
     "get_beats_ticks",
-    "get_midi_programs",
-    "get_midi_ticks_per_beat",
-    "merge_midis",
+    "get_score_programs",
+    "get_score_ticks_per_beat",
+    "merge_scores",
     "merge_same_program_tracks",
     "merge_tracks",
     "merge_tracks_per_class",
     "num_bar_pos",
     "get_num_notes_per_bar",
     "remove_duplicated_notes",
-    "split_midi_per_beats",
-    "split_midi_per_ticks",
-    "split_midi_per_tracks",
+    "split_score_per_beats",
+    "split_score_per_ticks",
+    "split_score_per_tracks",
 ]
```

### Comparing `miditok-3.0.2/miditok/utils/utils.py` & `miditok-3.0.3/miditok/utils/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 """Useful methods."""
 from __future__ import annotations
 
 import warnings
 from copy import copy
 from math import ceil
+from pathlib import Path
 from typing import TYPE_CHECKING
 
 import numpy as np
 from symusic import (
     ControlChange,
-    KeySignature,
     Note,
     Pedal,
     PitchBend,
     Score,
     Tempo,
     TextMeta,
     TimeSignature,
     Track,
 )
 from symusic.core import NoteTickList
 
-from miditok.classes import Event
+from miditok.classes import Event, TokSequence
 from miditok.constants import (
     DRUM_PITCH_RANGE,
     INSTRUMENT_CLASSES,
     MIDI_INSTRUMENTS,
     PITCH_CLASSES,
+    SCORE_LOADING_EXCEPTION,
     TIME_SIGNATURE,
     UNKNOWN_CHORD_PREFIX,
 )
 
 if TYPE_CHECKING:
-    from collections.abc import Sequence
+    from collections.abc import Callable, Sequence
 
     from miditoolkit import MidiFile
     from symusic.core import TrackTickList
 
 
 def convert_ids_tensors_to_list(ids) -> list[int] | list[list[int]]:  # noqa: ANN001
     """
@@ -72,22 +73,22 @@
             # Recursively try to convert elements of the list
             for ei in range(len(ids)):
                 ids[ei] = convert_ids_tensors_to_list(ids[ei])
 
     return ids
 
 
-def get_midi_programs(midi: Score) -> list[tuple[int, bool]]:
+def get_score_programs(score: Score) -> list[tuple[int, bool]]:
     r"""
-    Return the list of programs of the tracks of a MIDI.
+    Return the list of programs of the tracks of a ``symusic.Score``.
 
-    :param midi: the MIDI object to extract tracks programs
+    :param score: the ``symusic.Score`` object to extract tracks programs
     :return: the list of track programs, as a list of tuples (program, is_drum)
     """
-    return [(int(track.program), track.is_drum) for track in midi.tracks]
+    return [(int(track.program), track.is_drum) for track in score.tracks]
 
 
 def remove_duplicated_notes(
     notes: NoteTickList | dict[str, np.ndarray], consider_duration: bool = False
 ) -> None:
     r"""
     Remove (inplace) duplicated notes, i.e. with the same pitch and onset time.
@@ -158,23 +159,23 @@
     r"""
     Detect chords in a list of notes.
 
     Make sure to sort notes by start time then pitch
     before: ``notes.sort(key=lambda x: (x.start, x.pitch))``.
     **On very large tracks with high note density this method can be slow.**
     If you plan to use it with the Maestro or GiantMIDI datasets, it can take up to
-    hundreds of seconds per MIDI depending on your cpu.
+    hundreds of seconds per file depending on your cpu.
     This method works by iterating over each note, find if it played with other notes,
     and if it forms a chord from the chord maps. **It does not consider chord
     inversion.**.
 
     :param notes: notes to analyse (sorted by starting time, them pitch).
     :param ticks_per_beat: array indicating the number of ticks per beat per
         time signature denominator section. The numbers of ticks per beat depend on the
-        time signatures of the MIDI being parsed. The array has a shape ``(N,2)``, for
+        time signatures of the Score being parsed. The array has a shape ``(N,2)``, for
         ``N`` changes of ticks per beat, and the second dimension representing the end
         tick of each section and the number of ticks per beat respectively.
     :param chord_maps: list of chord maps, to be given as a dictionary where keys are
         chord qualities (e.g. "maj") and values pitch maps as tuples of integers
         (e.g. (0, 4, 7)). You can use ``miditok.constants.CHORD_MAPS`` as an example.
     :param program: program of the track of the notes. Used to specify the program when
         creating the Event object. (default: None)
@@ -272,15 +273,15 @@
         previous_tick = max(onset_notes[:, 1])
         count += len(onset_notes)  # Move to the next notes
 
     return chords
 
 
 def merge_tracks_per_class(
-    midi: Score,
+    score: Score,
     classes_to_merge: list[int] | None = None,
     new_program_per_class: dict[int, int] | None = None,
     max_num_of_tracks_per_inst_class: dict[int, int] | None = None,
     valid_programs: list[int] | None = None,
     filter_pitches: bool = True,
 ) -> None:
     r"""
@@ -288,15 +289,15 @@
 
     Example, a list of tracks / programs ``[0, 3, 8, 10, 11, 24, 25, 44, 47]`` will
     become ``[0, 8, 24, 25, 40]`` if ``classes_to_merge`` is ``[0, 1, 5]``.
     The classes are in ``miditok.constants.INSTRUMENT_CLASSES``.
 
     **Note:** programs of drum tracks will be set to -1.
 
-    :param midi: MIDI object to merge tracks
+    :param score: ``symusic.Score`` object to merge tracks
     :param classes_to_merge: instrument classes to merge, to give as list of indexes
         (see miditok.constants.INSTRUMENT_CLASSES). Give None to merge nothing, the
         function will still remove non-valid programs/tracks if given. (default:
         ``None``)
     :param new_program_per_class: new program of the final merged tracks, to be given
         per instrument class as a dict ``{class_id: program}``. (default: ``None``)
     :param max_num_of_tracks_per_inst_class: max number of tracks per instrument class,
@@ -306,30 +307,30 @@
         for keep all programs. (default ``None``)
     :param filter_pitches: after merging, will remove notes whose pitches are out the
         recommended range defined by the GM2 specs. (default: ``True``)
     """
     # remove non-valid tracks (instruments)
     if valid_programs is not None:
         i = 0
-        while i < len(midi.tracks):
-            if midi.tracks[i].is_drum:
-                midi.tracks[i].program = 128  # sets program of drums to 128
-            if midi.tracks[i].program not in valid_programs:
-                del midi.tracks[i]
-                if len(midi.tracks) == 0:
+        while i < len(score.tracks):
+            if score.tracks[i].is_drum:
+                score.tracks[i].program = 128  # sets program of drums to 128
+            if score.tracks[i].program not in valid_programs:
+                del score.tracks[i]
+                if len(score.tracks) == 0:
                     return
             else:
                 i += 1
 
     # merge tracks of the same instrument classes
     if classes_to_merge is not None:
-        midi.tracks.sort(key=lambda trac: trac.program)
+        score.tracks.sort(key=lambda trac: trac.program)
         if max_num_of_tracks_per_inst_class is None:
             max_num_of_tracks_per_inst_class = {
-                cla: len(midi.tracks) for cla in classes_to_merge
+                cla: len(score.tracks) for cla in classes_to_merge
             }  # no limit
         if new_program_per_class is None:
             new_program_per_class = {
                 cla: INSTRUMENT_CLASSES[cla]["program_range"].start
                 for cla in classes_to_merge
             }
         else:
@@ -341,37 +342,37 @@
                         f"{INSTRUMENT_CLASSES[cla]['program_range']}"
                     )
                     raise ValueError(msg)
 
         for ci in classes_to_merge:
             idx_to_merge = [
                 ti
-                for ti in range(len(midi.tracks))
-                if midi.tracks[ti].program in INSTRUMENT_CLASSES[ci]["program_range"]
+                for ti in range(len(score.tracks))
+                if score.tracks[ti].program in INSTRUMENT_CLASSES[ci]["program_range"]
             ]
             if len(idx_to_merge) > 0:
-                midi.tracks[idx_to_merge[0]].program = new_program_per_class[ci]
+                score.tracks[idx_to_merge[0]].program = new_program_per_class[ci]
                 if len(idx_to_merge) > max_num_of_tracks_per_inst_class[ci]:
-                    lengths = [len(midi.tracks[idx].notes) for idx in idx_to_merge]
+                    lengths = [len(score.tracks[idx].notes) for idx in idx_to_merge]
                     idx_to_merge = np.argsort(lengths)
                     # could also be randomly picked
 
                 # Merges tracks to merge
-                midi.tracks[idx_to_merge[0]] = merge_tracks(
-                    [midi.tracks[i] for i in idx_to_merge]
+                score.tracks[idx_to_merge[0]] = merge_tracks(
+                    [score.tracks[i] for i in idx_to_merge]
                 )
 
                 # Removes tracks merged to index idx_to_merge[0]
-                new_len = len(midi.tracks) - len(idx_to_merge) + 1
-                while len(midi.tracks) > new_len:
-                    del midi.tracks[idx_to_merge[0] + 1]
+                new_len = len(score.tracks) - len(idx_to_merge) + 1
+                while len(score.tracks) > new_len:
+                    del score.tracks[idx_to_merge[0] + 1]
 
     # filters notes with pitches out of tessitura / recommended pitch range
     if filter_pitches:
-        for track in midi.tracks:
+        for track in score.tracks:
             ni = 0
             while ni < len(track.notes):
                 if track.is_drum:
                     tessitura = DRUM_PITCH_RANGE
                 else:
                     tessitura = MIDI_INSTRUMENTS[track.program]["pitch_range"]
                 if track.notes[ni].pitch not in tessitura:
@@ -428,42 +429,42 @@
     else:
         for _ in range(1, len(tracks)):
             del tracks[1]
         tracks[0] = tracks_[0]
     return tracks_[0]
 
 
-def merge_midis(midis: Sequence[Score]) -> Score:
-    """
-    Merge a list of MIDIs into a single one.
+def merge_scores(scores: Sequence[Score]) -> Score:
+    r"""
+    Merge a list of ``symusic.Score``\s into a single one.
 
     This method will combine all their tracks and global events such as tempo changes
     or time signature changes.
 
-    :param midis: MIDIs to merge.
-    :return: the merged MIDI.
+    :param scores: ``symusic.Score``\s to merge.
+    :return: the merged ``symusic.Score``.
     """
-    if not all(midi.tpq == midis[0].tpq for midi in midis):
+    if not all(score.tpq == scores[0].tpq for score in scores):
         msg = (
             "Some `Score`s have different time divisions (`tpq`). They must be all"
             "identical in order to merge the `Scores`s."
         )
         raise ValueError(msg)
 
-    midi = Score(midis[0].tpq)
-    for midi_split in midis:
-        midi.tracks.extend(midi_split.tracks)
-        midi.tempos.extend(midi_split.tempos)
-        midi.time_signatures.extend(midi_split.time_signatures)
-        midi.key_signatures.extend(midi_split.key_signatures)
-        midi.lyrics.extend(midi_split.lyrics)
-        midi.markers.extend(midi_split.markers)
+    score = Score(scores[0].tpq)
+    for score_split in scores:
+        score.tracks.extend(score_split.tracks)
+        score.tempos.extend(score_split.tempos)
+        score.time_signatures.extend(score_split.time_signatures)
+        score.key_signatures.extend(score_split.key_signatures)
+        score.lyrics.extend(score_split.lyrics)
+        score.markers.extend(score_split.markers)
 
     # sorting is done by Symusic automatically
-    return midi
+    return score
 
 
 def merge_same_program_tracks(
     tracks: list[Track] | TrackTickList, effects: bool = True
 ) -> None:
     r"""
     Merge tracks having the same program number.
@@ -617,15 +618,15 @@
 
 
 def compute_ticks_per_beat(time_sig_denominator: int, time_division: int) -> int:
     r"""
     Compute the number of ticks in a beat at a given time signature.
 
     :param time_sig_denominator: time signature denominator.
-    :param time_division: MIDI time division in ticks/quarter.
+    :param time_division: ``symusic.Score`` time division (``.tpq``) in ticks/quarter.
     :return: number of ticks per beat at the given time signature.
     """
     if time_sig_denominator == 4:
         return time_division
     # factor to multiply the time_division depending on the denominator
     # if we have a */8 time sig, one beat is an eighth note so one beat is
     # `time_division * 0.5` ticks.
@@ -636,387 +637,411 @@
 def compute_ticks_per_bar(time_sig: TimeSignature, time_division: int) -> int:
     r"""
     Compute the number of ticks in a bar.
 
     The number of ticks per bar depends on the time signature.
 
     :param time_sig: time signature object.
-    :param time_division: MIDI time division in ticks/quarter.
-    :return: MIDI bar resolution, in ticks/bar
+    :param time_division: ``symusic.Score`` time division (``.tpq``) in ticks/quarter.
+    :return: bar resolution, in ticks/bar
     """
     return int(
         compute_ticks_per_beat(time_sig.denominator, time_division) * time_sig.numerator
     )
 
 
-def get_bars_ticks(midi: Score) -> list[int]:
+def get_bars_ticks(score: Score) -> list[int]:
     """
-    Compute the ticks of the bars of a MIDI.
+    Compute the ticks of the bars of a ``symusic.Score``.
 
     **Note:** When encountering multiple time signature messages at a same tick, we
     this method will automatically consider the last one (coming in the list). Other
     software can proceed differently. Logic Pro, for example, uses the first one.
     I haven't found documentation or recommendations for this specific situation. It
     might be better to use the first one and discard the others.
 
-    :param midi: MIDI to analyze.
+    :param score: ``symusic.Score`` to analyze.
     :return: list of ticks for each bar.
     """
-    max_tick = midi.end()
+    max_tick = score.end()
     bars_ticks = []
-    time_sigs = copy(midi.time_signatures)
+    time_sigs = copy(score.time_signatures)
     # Mock the last one to cover the last section in the loop below
     if time_sigs[-1].time != max_tick:
         time_sigs.append(TimeSignature(max_tick, *TIME_SIGNATURE))
 
     # Section from tick 0 to first time sig is 4/4 if first time sig time is not 0
     if time_sigs[0].time == 0:
         current_time_sig = time_sigs[0]
     else:
         current_time_sig = TimeSignature(0, *TIME_SIGNATURE)
 
     # Compute bars, one time signature portion at a time
     for time_signature in time_sigs:
-        ticks_per_bar = compute_ticks_per_bar(current_time_sig, midi.ticks_per_quarter)
+        ticks_per_bar = compute_ticks_per_bar(current_time_sig, score.ticks_per_quarter)
         ticks_diff = time_signature.time - current_time_sig.time
         num_bars = ceil(ticks_diff / ticks_per_bar)
         bars_ticks += [
             current_time_sig.time + ticks_per_bar * i for i in range(num_bars)
         ]
         current_time_sig = time_signature
 
     return bars_ticks
 
 
-def get_beats_ticks(midi: Score) -> list[int]:
+def get_beats_ticks(score: Score) -> list[int]:
     """
-    Return the ticks of the beats of a MIDI.
+    Return the ticks of the beats of a ``symusic.Score``.
 
     **Note:** When encountering multiple time signature messages at a same tick, we
     this method will automatically consider the last one (coming in the list). Other
     software can proceed differently. Logic Pro, for example, uses the first one.
     I haven't found documentation or recommendations for this specific situation. It
     might be better to use the first one and discard the others.
 
-    :param midi: MIDI to analyze.
+    :param score: ``symusic.Score`` to analyze.
     :return: list of ticks for each beat.
     """
-    max_tick = midi.end()
+    max_tick = score.end()
     beat_ticks = []
-    time_sigs = copy(midi.time_signatures)
+    time_sigs = copy(score.time_signatures)
     # Mock the last one to cover the last section in the loop below
     if time_sigs[-1].time != max_tick:
         time_sigs.append(TimeSignature(max_tick, *TIME_SIGNATURE))
 
     # Section from tick 0 to first time sig is 4/4 if first time sig time is not 0
     if time_sigs[0].time == 0:
         current_time_sig = time_sigs[0]
     else:
         current_time_sig = TimeSignature(0, *TIME_SIGNATURE)
 
     # Compute beats, one time signature portion at a time
     for time_signature in time_sigs:
         ticks_per_beat = compute_ticks_per_beat(
-            current_time_sig.denominator, midi.ticks_per_quarter
+            current_time_sig.denominator, score.ticks_per_quarter
         )
         ticks_diff = time_signature.time - current_time_sig.time
         num_beats = ceil(ticks_diff / ticks_per_beat)
         beat_ticks += [
             current_time_sig.time + ticks_per_beat * i for i in range(num_beats)
         ]
         current_time_sig = time_signature
 
     return beat_ticks
 
 
+def add_bar_beats_ticks_to_tokseq(
+    tokseq: TokSequence | list[TokSequence],
+    score: Score | None = None,
+    bar_ticks: list[int] | None = None,
+    beat_ticks: list[int] | None = None,
+) -> None:
+    """
+    Add the ticks of the bars and beats of a Score to a :class:`miditok.TokSequence`.
+
+    :param tokseq: :class:`miditok.TokSequence` to add ticks attributes to.
+    :param score: ``symusic.Score`` object to add ticks from.
+    :param bar_ticks: ticks of the bars of the ``score``. Only used for recursivity.
+    :param beat_ticks: ticks of the beats of the ``score``. Only used for recursivity.
+    """
+    if bar_ticks is None:
+        bar_ticks = get_bars_ticks(score)
+    if beat_ticks is None:
+        beat_ticks = get_beats_ticks(score)
+
+    # Recursively adds bars/beats ticks
+    if isinstance(tokseq, list):
+        for seq in tokseq:
+            add_bar_beats_ticks_to_tokseq(
+                seq, bar_ticks=bar_ticks, beat_ticks=beat_ticks
+            )
+    else:
+        tokseq._ticks_bars = bar_ticks
+        tokseq._ticks_beats = beat_ticks
+
+
 def get_num_notes_per_bar(
-    midi: Score, tracks_indep: bool = False
+    score: Score, tracks_indep: bool = False
 ) -> list[int | list[int]]:
     """
-    Return the number of notes within each bar of a MIDI.
+    Return the number of notes within each bar of a ``symusic.Score``.
 
-    :param midi: MIDI object to analyze.
+    :param score: ``symusic.Score`` object to analyze.
     :param tracks_indep: whether to process each track independently or all together.
     :return: the number of notes within each bar.
     """
     # Get bar and note times
-    bar_ticks = get_bars_ticks(midi)
-    if bar_ticks[-1] != midi.end():
-        bar_ticks.append(midi.end())
-    tracks_times = [track.notes.numpy()["time"] for track in midi.tracks]
+    bar_ticks = get_bars_ticks(score)
+    if bar_ticks[-1] != score.end():
+        bar_ticks.append(score.end())
+    tracks_times = [track.notes.numpy()["time"] for track in score.tracks]
     num_notes_per_bar = []
     if not tracks_indep:
         tracks_times = [np.concatenate(tracks_times)]
         tracks_times[-1].sort()
-    elif len(midi.tracks) > 1:
+    elif len(score.tracks) > 1:
         num_notes_per_bar = [[] for _ in range(len(bar_ticks) - 1)]
 
     for notes_times in tracks_times:
         current_note_time_idx = previous_note_time_idx = 0
         current_bar_tick_idx = 0
         while current_bar_tick_idx < len(bar_ticks) - 1:
             while (
                 current_note_time_idx < len(notes_times)
                 and notes_times[current_note_time_idx]
                 < bar_ticks[current_bar_tick_idx + 1]
             ):
                 current_note_time_idx += 1
             num_notes = current_note_time_idx - previous_note_time_idx
-            if tracks_indep and len(midi.tracks) > 1:
+            if tracks_indep and len(score.tracks) > 1:
                 num_notes_per_bar[current_bar_tick_idx].append(num_notes)
             else:
                 num_notes_per_bar.append(num_notes)
 
             current_bar_tick_idx += 1
             previous_note_time_idx = current_note_time_idx
 
     return num_notes_per_bar
 
 
-def get_midi_ticks_per_beat(midi: Score) -> np.ndarray:
+def get_score_ticks_per_beat(score: Score) -> np.ndarray:
     """
-    Compute the portions of numbers of ticks in a beat in a MIDI.
+    Compute the portions of numbers of ticks in a beat in a ``symusic.Score``.
 
     The method returns a numpy array of shape ``(N,2)``, for N ticks-per-beat changes,
     and the second dimension corresponding to the ending tick and the number of ticks
     per beat of the portion.
 
-    :param midi: MIDI to analyze.
+    :param score: ``symusic.Score`` to analyze.
     :return: ticks per beat values as a numpy array.
     """
     ticks_per_beat = [
         [
-            midi.time_signatures[tsi + 1].time,
+            score.time_signatures[tsi + 1].time,
             compute_ticks_per_beat(
-                midi.time_signatures[tsi].denominator, midi.ticks_per_quarter
+                score.time_signatures[tsi].denominator, score.ticks_per_quarter
             ),
         ]
-        for tsi in range(len(midi.time_signatures) - 1)
+        for tsi in range(len(score.time_signatures) - 1)
     ]
 
-    # Handles the last one up to the max tick of the MIDI
+    # Handles the last one up to the max tick of the Score
     ticks_per_beat.append(
         [
-            midi.end() + 1,
+            score.end() + 1,
             compute_ticks_per_beat(
-                midi.time_signatures[-1].denominator, midi.ticks_per_quarter
+                score.time_signatures[-1].denominator, score.ticks_per_quarter
             ),
         ]
     )
 
     # Remove equal successive ones
     for i in range(len(ticks_per_beat) - 1, 0, -1):
         if ticks_per_beat[i][1] == ticks_per_beat[i - 1][1]:
             ticks_per_beat[i - 1][0] = ticks_per_beat[i][0]
             del ticks_per_beat[i]
 
     return np.array(ticks_per_beat)
 
 
-def split_midi_per_ticks(midi: Score, ticks: list[int]) -> list[Score]:
-    """
-    Split a MIDI into several smaller MIDIs.
-
-    The segmented MIDIs will all start at tick 0.
-    Example: for a MIDI with an end tick at 1000, and a list of tick
-    ``[2000, 5000, 7000]``, this method will return a list of four MIDIs which
-    correspond respectively to the portions of the original MIDI from tick 0 to 2000,
-    2000 to 5000, 5000 to 7000 and 10000 to 10000.
+def split_score_per_ticks(score: Score, ticks: list[int]) -> list[Score]:
+    r"""
+    Split a ``symusic.Score`` into several smaller ``symusic.Score``\s.
 
-    :param midi: MIDI object to split.
-    :param ticks: list of ticks to which the MIDI will be split.
-    :return: a list of segmented MIDI objects.
+    The ``symusic.Score`` chunks will all start at tick 0.
+    Example: for a ``symusic.Score`` with an end tick at 1000, and a list of tick
+    ``[2000, 5000, 7000]``, this method will return a list of four ``symusic.Score``
+    which correspond respectively to the portions of the original Score from tick 0 to
+    2000, 2000 to 5000, 5000 to 7000 and 10000 to 10000.
+
+    :param score: ``symusic.Score`` object to split.
+    :param ticks: list of ticks to which the score will be split.
+    :return: a list of segmented ``symusic.Score`` objects.
     """
-    midis_split = []
-    midi_end_tick = midi.end() + 1  # to encompass the last events
+    score_chunks = []
+    score_end_tick = score.end() + 1  # to encompass the last events
     ticks = ticks.copy()
-    if ticks[-1] != midi_end_tick:
-        ticks.append(midi_end_tick)
+    if ticks[-1] != score_end_tick:
+        ticks.append(score_end_tick)
 
     current_tick = 0
-    previous_tempo, previous_time_sig = None, None
-    previous_key_sig = KeySignature(0, 0, 0)
     for tick_end in ticks:
-        midi_split = midi.clip(current_tick, tick_end, clip_end=False).shift_time(
-            -current_tick
+        score_chunks.append(
+            score.clip(current_tick, tick_end, clip_end=False).shift_time(-current_tick)
         )
-        if len(midi_split.tempos) == 0:
-            midi_split.tempos.append(previous_tempo)
-        if len(midi_split.time_signatures) == 0:
-            midi_split.time_signatures.append(previous_time_sig)
-        if len(midi_split.key_signatures) == 0:
-            midi_split.key_signatures.append(previous_key_sig)
-        midis_split.append(midi_split)
-
-        # Update the variables for the next iteration
-        previous_tempo = midi_split.tempos[-1]
-        previous_time_sig = midi_split.time_signatures[-1]
-        previous_key_sig = midi_split.key_signatures[-1]
-        previous_tempo.time = previous_time_sig.time = previous_key_sig.time = 0
         current_tick = tick_end
 
-    return midis_split
+    return score_chunks
 
 
-def extract_chunk_from_midi(
-    midi: Score, tick_start: int, tick_end: int, clip_end: bool = False
-) -> Score:
-    """
-    Extract a chunk of a ``Score``.
-
-    The returned chunk will have a starting time at tick 0, i.e. the times of its
-    events will be shifted by ``-tick_start``.
-
-    :param midi: object to extract a chunk from.
-    :param tick_start: starting tick of the chunk to extract.
-    :param tick_end: ending tick of the chunk to extract.
-    :param clip_end: if given ``True``, the chunk at ``tick_end + 1`` and thus include
-        the events occurring at ``tick_end``. (default: ``False``)
-    :return: chunk of the ``midi`` starting at ``tick_start and ending at ``tick_end``.
-    """
-    # Get the tempo, time sig and key sig at the beginning of the chunk to extract
-    # There might not be default key signatures in the Score
-    tempo, time_signature, key_signature = None, None, KeySignature(0, 0, 0)
-    for tempo_ in midi.tempos:
-        if tempo_.time > tick_start:
-            break
-        tempo = tempo_
-    for time_signature_ in midi.time_signatures:
-        if time_signature_.time > tick_start:
-            break
-        time_signature = time_signature_
-    for key_signature_ in midi.key_signatures:
-        if key_signature_.time > tick_start:
-            break
-        key_signature = key_signature_
-    tempo.time = time_signature.time = key_signature.time = 0
-
-    # Clip the MIDI and append the global attributes
-    midi_split = midi.clip(tick_start, tick_end, clip_end=clip_end).shift_time(
-        -tick_start
-    )
-    midi_split.tempos.append(tempo)
-    midi_split.time_signatures.append(time_signature)
-    midi_split.key_signatures.append(key_signature)
-
-    return midi_split
-
-
-def split_midi_per_beats(
-    midi: Score, max_num_beats: int, min_num_beats: int = 1
+def split_score_per_beats(
+    score: Score, max_num_beats: int, min_num_beats: int = 1
 ) -> list[Score]:
     """
-    Split a MIDI into several smaller MIDIs per number of beats.
+    Split a ``symusic.Score`` into several smaller chunks per number of beats.
 
-    This method splits a MIDI into smaller chunks that contains ``max_num_beats``
-    beats. The segmented MIDIs will all start at tick 0.
+    This method splits a ``symusic.Score`` into smaller chunks that contains
+    ``max_num_beats`` beats. The ``symusic.Score`` chunks will all start at tick 0.
 
-    :param midi: MIDI object to split.
+    :param score: ``symusic.Score`` object to split.
     :param max_num_beats: maximum number of beats per segment.
     :param min_num_beats: minimum number of beats per segment. This only applied to the
-        last segment of the input MIDI. (default: ``1``)
-    :return: a list of segmented MIDI objects.
+        last segment of the input score. (default: ``1``)
+    :return: a list of ``symusic.Score`` chunks.
     """
     if min_num_beats < 1:
         raise ValueError(_ := f"`min_num_beats` must be > 0 (got {min_num_beats}).")
 
     ticks_split = []
-    beats_ticks = get_beats_ticks(midi)
+    beats_ticks = get_beats_ticks(score)
     current_beat = 0
     while current_beat < len(beats_ticks):
         # Determine the number of beats for this section
         num_beats = min(len(beats_ticks) - current_beat, max_num_beats)
         if num_beats < min_num_beats:
             break
 
         # Extract the section
         if (
             num_beats != max_num_beats
             or current_beat == len(beats_ticks) - max_num_beats
         ):
             # Will be the last iteration
-            tick_end = midi.end() + 1
+            tick_end = score.end() + 1
         else:
             tick_end = beats_ticks[current_beat + num_beats]
-        if tick_end > midi.end():
+        if tick_end > score.end():
             break
         ticks_split.append(tick_end)
         current_beat += num_beats
 
-    return split_midi_per_ticks(midi, ticks_split)
+    return split_score_per_ticks(score, ticks_split)
 
 
-def split_midi_per_tracks(midi: Score) -> list[Score]:
+def split_score_per_tracks(score: Score) -> list[Score]:
     """
-    Split a MIDI into several smaller MIDIs.
+    Split a ``symusic.Score`` into several scores for each of its tracks.
 
-    The segmented MIDIs will all start at tick 0.
-    Example: for a MIDI with an end tick at 1000, and a list of tick
-    ``[2000, 5000, 7000]``, this method will return a list of four MIDIs which
-    correspond respectively to the portions of the original MIDI from tick 0 to 2000,
+    The split scores will all start at tick 0.
+    Example: for a score with an end tick at 1000, and a list of tick
+    ``[2000, 5000, 7000]``, this method will return a list of four scores which
+    correspond respectively to the portions of the original score from tick 0 to 2000,
     2000 to 5000, 5000 to 7000 and 10000 to 10000.
 
-    :param midi: MIDI object to split.
-    :return: a list of segmented MIDI objects.
+    :param score: ``symusic.Score`` object to split.
+    :return: a list of split ``symusic.Score`` objects.
     """
-    midis_split = []
-    for track in midi.tracks:
-        midi_split = Score(midi.tpq)
-        midi_split.tempos = midi.tempos
-        midi_split.time_signatures = midi.time_signatures
-        midi_split.key_signatures = midi.key_signatures
-        midi_split.lyrics = midi.lyrics
-        midi_split.markers = midi.markers
-        midi_split.tracks.append(track.copy())
+    scores_split = []
+    for track in score.tracks:
+        score_split = Score(score.tpq)
+        score_split.tempos = score.tempos
+        score_split.time_signatures = score.time_signatures
+        score_split.key_signatures = score.key_signatures
+        score_split.lyrics = score.lyrics
+        score_split.markers = score.markers
+        score_split.tracks.append(track.copy())
 
-        midis_split.append(midi_split)
-    return midis_split
+        scores_split.append(score_split)
+    return scores_split
 
 
-def concat_midis(midis: Sequence[Score], end_ticks: Sequence[int]) -> Score:
-    """
-    Concatenate a sequence of MIDIs.
+def concat_scores(scores: Sequence[Score], end_ticks: Sequence[int]) -> Score:
+    r"""
+    Concatenate a sequence of ``symusic.Score``\s.
 
     **Note:** the tracks are concatenated in the same order as they are given.
-    **The MIDIs must all have the same time division.** (``midi.ticks_per_quarter``)
-    The concatenated MIDI might have identical consecutive tempos, time signatures or
+    **The scores must all have the same time division.** (``score.tpq``)
+    The concatenated score might have identical consecutive tempos, time signatures or
     key signatures values.
 
-    :param midis: MIDIs to concatenate.
-    :param end_ticks: the ticks indicating the end of each MIDI. The end for the last
-        MIDI is not required.
-    :return: the concatenated MIDI.
-    """
-    if not all(midi.ticks_per_quarter == midis[0].ticks_per_quarter for midi in midis):
-        err_msg = "The MIDIs given do not have all the same time division."
+    :param scores: ``symusic.Score``\s to concatenate.
+    :param end_ticks: the ticks indicating the end of each score. The end for the last
+        score is not required.
+    :return: the concatenated ``symusic.Score``.
+    """
+    if not all(
+        score.ticks_per_quarter == scores[0].ticks_per_quarter for score in scores
+    ):
+        err_msg = "The provided scores do not have all the same time division."
         raise ValueError(err_msg)
-    if not len(end_ticks) >= len(midis) - 1:
-        err = f"Missing end values: got {len(end_ticks)}, expected {len(midis) - 1}."
+    if not len(end_ticks) >= len(scores) - 1:
+        err = f"Missing end values: got {len(end_ticks)}, expected {len(scores) - 1}."
         raise ValueError(err)
 
-    # Create the concatenated MIDI with empty tracks
-    midi_concat = Score(midis[0].ticks_per_quarter)
-    midi_concat.tracks = midis[0].tracks
-
-    for mi in range(len(midis)):
-        # Shift the MIDI
-        midi = midis[mi]
+    # Create the concatenated Score with empty tracks
+    score_concat = Score(scores[0].ticks_per_quarter)
+    score_concat.tracks = scores[0].tracks
+
+    for mi in range(len(scores)):
+        # Shift the Score
+        score = scores[mi]
         if mi > 0:
-            midi = midi.shift_time(end_ticks[mi - 1])
+            score = score.shift_time(end_ticks[mi - 1])
 
         # Concatenate global messages
-        midi_concat.tempos.extend(midi.tempos)
-        midi_concat.time_signatures.extend(midi.time_signatures)
-        midi_concat.key_signatures.extend(midi.key_signatures)
-        midi_concat.lyrics.extend(midi.lyrics)
-        midi_concat.markers.extend(midi.markers)
+        score_concat.tempos.extend(score.tempos)
+        score_concat.time_signatures.extend(score.time_signatures)
+        score_concat.key_signatures.extend(score.key_signatures)
+        score_concat.lyrics.extend(score.lyrics)
+        score_concat.markers.extend(score.markers)
 
-        # Concatenate track messages (except for the first MIDI)
+        # Concatenate track messages (except for the first Score)
         if mi == 0:
             continue
-        for ti, track in enumerate(midi.tracks):
-            midi_concat.tracks[ti].notes.extend(track.notes)
-            midi_concat.tracks[ti].controls.extend(track.controls)
-            midi_concat.tracks[ti].pitch_bends.extend(track.pitch_bends)
-            midi_concat.tracks[ti].pedals.extend(track.pedals)
+        for ti, track in enumerate(score.tracks):
+            score_concat.tracks[ti].notes.extend(track.notes)
+            score_concat.tracks[ti].controls.extend(track.controls)
+            score_concat.tracks[ti].pitch_bends.extend(track.pitch_bends)
+            score_concat.tracks[ti].pedals.extend(track.pedals)
+
+    return score_concat
+
 
-    return midi_concat
+def get_deepest_common_subdir(paths: Sequence[Path]) -> Path:
+    """
+    Return the path of the deepest common subdirectory from several paths.
+
+    :param paths: paths to analyze.
+    :return: path of the deepest common subdirectory from the paths
+    """
+    all_parts = [path.resolve().parent.parts for path in paths]
+    max_depth = max(len(parts) for parts in all_parts)
+    root_parts = []
+    for depth in range(max_depth):
+        if len({parts[depth] for parts in all_parts}) > 1:
+            break
+        root_parts.append(all_parts[0][depth])
+    return Path(*root_parts)
+
+
+def filter_dataset(
+    files_paths: Sequence[Path],
+    valid_fn: Callable[[Score, Path], bool] | None = None,
+    delete_invalid_files: bool = False,
+) -> list[Path]:
+    """
+    Filter a list of paths to only retain valid files.
+
+    This method ise useful in order to filter corrupted files that cannot be loaded, or
+    that do not satisfy user-specified conditions thanks to the ``validation_fn``.
+
+    :param files_paths: paths to the files to filter.
+    :param valid_fn: an optional validation function. It must take a ``Score`` and a
+        ``Path`` arguments and return a boolean. (default: ``None``)
+    :param delete_invalid_files: if ``True``, will delete inplace the files on the file
+        system. (default: ``False``)
+    :return: the list of paths to the files satisfying your conditions.
+    """
+    paths_valid = []
+    for path in files_paths:
+        try:
+            file = Score(path)
+        except SCORE_LOADING_EXCEPTION:
+            if delete_invalid_files:
+                path.unlink()
+            continue
+        if valid_fn is not None and not valid_fn(file, path):
+            if delete_invalid_files:
+                path.unlink()
+            continue
+        paths_valid.append(path)
+    return paths_valid
```

### Comparing `miditok-3.0.2/.gitignore` & `miditok-3.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `miditok-3.0.2/LICENSE` & `miditok-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `miditok-3.0.2/README.md` & `miditok-3.0.3/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 # MidiTok
 
-Python package to tokenize MIDI music files, presented at the ISMIR 2021 LBDs.
+Python package to tokenize music files, introduced at the ISMIR 2021 LBDs.
 
 ![MidiTok Logo](docs/assets/logo.png?raw=true "")
 
 [![PyPI version fury.io](https://badge.fury.io/py/miditok.svg)](https://pypi.python.org/pypi/miditok/)
 [![Python 3.8](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/release/)
 [![Documentation Status](https://readthedocs.org/projects/miditok/badge/?version=latest)](https://miditok.readthedocs.io/en/latest/?badge=latest)
 [![GitHub CI](https://github.com/Natooz/MidiTok/actions/workflows/pytest.yml/badge.svg)](https://github.com/Natooz/MidiTok/actions/workflows/pytest.yml)
 [![Codecov](https://img.shields.io/codecov/c/github/Natooz/MidiTok)](https://codecov.io/gh/Natooz/MidiTok)
 [![GitHub license](https://img.shields.io/github/license/Natooz/MidiTok.svg)](https://github.com/Natooz/MidiTok/blob/main/LICENSE)
 [![Downloads](https://static.pepy.tech/badge/miditok)](https://pepy.tech/project/MidiTok)
 [![Code style](https://img.shields.io/badge/code%20style-ruff-000000.svg)](https://github.com/astral-sh/ruff)
 
-MidiTok can tokenize MIDI files, i.e. convert them into sequences of tokens ready to be fed to models such as Transformer, for any generation, transcription or MIR task.
-MidiTok features most known [MIDI tokenizations](https://miditok.readthedocs.io/en/latest/tokenizations.html) (e.g. [REMI](https://arxiv.org/abs/2002.00212), [Compound Word](https://arxiv.org/abs/2101.02402)...), and is built around the idea that they all share common parameters and methods. It supports [Byte Pair Encoding (BPE)](https://arxiv.org/abs/2301.11975) and data augmentation.
+MidiTok can tokenize MIDI and abc files, i.e. convert them into sequences of tokens ready to be fed to models such as Transformer, for any generation, transcription or MIR task.
+MidiTok features most known [music tokenizations](https://miditok.readthedocs.io/en/latest/tokenizations.html) (e.g. [REMI](https://arxiv.org/abs/2002.00212), [Compound Word](https://arxiv.org/abs/2101.02402)...), and is built around the idea that they all share common parameters and methods. Tokenizers can be trained with [Byte Pair Encoding (BPE)](https://aclanthology.org/2023.emnlp-main.123/), [Unigram](https://aclanthology.org/P18-1007/) and [WordPiece](https://arxiv.org/abs/1609.08144), and it offers data augmentation methods.
 
 MidiTok is integrated with the Hugging Face Hub 🤗! Don't hesitate to share your models to the community!
 
 **Documentation:** [miditok.readthedocs.com](https://miditok.readthedocs.io/en/latest/index.html)
 
 ## Install
 
 ```shell
 pip install miditok
 ```
-MidiTok uses [Symusic](https://github.com/Yikai-Liao/symusic) to read and write MIDI files, and BPE is backed by [Hugging Face 🤗tokenizers](https://github.com/huggingface/tokenizers) for super-fast encoding.
+MidiTok uses [Symusic](https://github.com/Yikai-Liao/symusic) to read and write MIDI and abc files, and BPE/Unigram is backed by [Hugging Face 🤗tokenizers](https://github.com/huggingface/tokenizers) for superfast encoding.
 
 ## Usage example
 
 Tokenizing and detokenzing can be done by calling the tokenizer:
 
 ```python
 from miditok import REMI, TokenizerConfig
@@ -38,54 +38,54 @@
 # Creating a multitrack tokenizer, read the doc to explore all the parameters
 config = TokenizerConfig(num_velocities=16, use_chords=True, use_programs=True)
 tokenizer = REMI(config)
 
 # Loads a midi, converts to tokens, and back to a MIDI
 midi = Score("path/to/your_midi.mid")
 tokens = tokenizer(midi)  # calling the tokenizer will automatically detect MIDIs, paths and tokens
-converted_back_midi = tokenizer(tokens)  # PyTorch / Tensorflow / Numpy tensors supported
+converted_back_midi = tokenizer(tokens)  # PyTorch, Tensorflow and Numpy tensors are supported
 ```
 
-Here is a complete yet concise example of how you can use MidiTok to train any PyTorch model. And [here](colab-notebooks/Full_Example_HuggingFace_GPT2_Transformer.ipynb) is a simple notebook example showing how to use Hugging Face models to generate music, with MidiTok taking care of tokenizing MIDIs.
+Here is a complete yet concise example of how you can use MidiTok to train any PyTorch model. And [here](colab-notebooks/Full_Example_HuggingFace_GPT2_Transformer.ipynb) is a simple notebook example showing how to use Hugging Face models to generate music, with MidiTok taking care of tokenizing music files.
 
 ```python
 from miditok import REMI, TokenizerConfig
-from miditok.pytorch_data import DatasetMIDI, DataCollator, split_midis_for_training
+from miditok.pytorch_data import DatasetMIDI, DataCollator, split_files_for_training
 from torch.utils.data import DataLoader
 from pathlib import Path
 
 # Creating a multitrack tokenizer, read the doc to explore all the parameters
 config = TokenizerConfig(num_velocities=16, use_chords=True, use_programs=True)
 tokenizer = REMI(config)
 
 # Train the tokenizer with Byte Pair Encoding (BPE)
-midi_paths = list(Path("path", "to", "midis").glob("**/*.mid"))
-tokenizer.learn_bpe(vocab_size=30000, files_paths=midi_paths)
+files_paths = list(Path("path", "to", "midis").glob("**/*.mid"))
+tokenizer.train(vocab_size=30000, files_paths=files_paths)
 tokenizer.save_params(Path("path", "to", "save", "tokenizer.json"))
 # And pushing it to the Hugging Face hub (you can download it back with .from_pretrained)
 tokenizer.push_to_hub("username/model-name", private=True, token="your_hf_token")
 
 # Split MIDIs into smaller chunks for training
 dataset_chunks_dir = Path("path", "to", "midi_chunks")
-split_midis_for_training(
-    files_paths=midi_paths,
+split_files_for_training(
+    files_paths=files_paths,
     tokenizer=tokenizer,
     save_dir=dataset_chunks_dir,
     max_seq_len=1024,
 )
 
 # Create a Dataset, a DataLoader and a collator to train a model
 dataset = DatasetMIDI(
     files_paths=list(dataset_chunks_dir.glob("**/*.mid")),
     tokenizer=tokenizer,
     max_seq_len=1024,
     bos_token_id=tokenizer["BOS_None"],
     eos_token_id=tokenizer["EOS_None"],
 )
-collator = DataCollator(tokenizer["PAD_None"])
+collator = DataCollator(tokenizer.pad_token_id)
 dataloader = DataLoader(dataset, batch_size=64, collate_fn=collator)
 
 # Iterate over the dataloader to train a model
 for batch in dataloader:
     print("Train your model on this batch...")
 ```
 
@@ -106,18 +106,18 @@
 
 ## Contributions
 
 Contributions are gratefully welcomed, feel free to open an issue or send a PR if you want to add a tokenization or speed up the code. You can read the [contribution guide](CONTRIBUTING.md) for details.
 
 ### Todos
 
+* Support music-xml files;
 * `no_duration_drums` option, discarding duration tokens for drum notes;
-* Extend unimplemented additional tokens to all compatible tokenizations;
 * Control Change messages;
-* Speeding up the MIDI preprocess + global/track events parsing with Rust or C++ binding.
+* Speed-up global/track events parsing with Rust or C++ bindings.
 
 ## Citation
 
 If you use MidiTok for your research, a citation in your manuscript would be gladly appreciated. ❤️
 
 [**[MidiTok paper]**](https://arxiv.org/abs/2310.17202)
 [**[MidiTok original ISMIR publication]**](https://archives.ismir.net/ismir2021/latebreaking/000005.pdf)
```

### Comparing `miditok-3.0.2/pyproject.toml` & `miditok-3.0.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "miditok"
-version = "3.0.2"
+version = "3.0.3"
 description = "MIDI / symbolic music tokenizers for Deep Learning models."
 readme = "README.md"
 license = "MIT"
 requires-python = ">=3.8.0"
 authors = [
     { name = "Nathan Fradet" },
 ]
@@ -34,15 +34,15 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "numpy>=1.19",
-    "symusic>=0.3.2",
+    "symusic>=0.4.3",
     "tqdm",
     "tokenizers>=0.13.0",
     "huggingface_hub>=0.16.4",
 ]
 
 [project.optional-dependencies]
 tests = [
@@ -71,19 +71,16 @@
 ]
 
 [tool.coverage.report]
 exclude_also = [
     "def __repr__",
 ]
 omit = [
-    # omit benchmark files
-    "tests/benchmark_fast_bpe.py",
-    "tests/benchmark_midi_read.py",
-    "tests/benchmark_preprocess.py",
-    "tests/benchmark_tokenize.py",
+    # files to omit to check
+    "benchmarks/*"
 ]
 
 [tool.ruff]
 target-version = "py312"
 
 [tool.ruff.lint]
 extend-select = [
```

### Comparing `miditok-3.0.2/PKG-INFO` & `miditok-3.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: miditok
-Version: 3.0.2
+Version: 3.0.3
 Summary: MIDI / symbolic music tokenizers for Deep Learning models.
 Project-URL: Homepage, https://github.com/Natooz/MidiTok
 Project-URL: Documentation, https://miditok.readthedocs.io
 Author: Nathan Fradet
 License-Expression: MIT
 License-File: LICENSE
 Keywords: artificial intelligence,deep learning,midi,mir,music,tokenization,transformer
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Multimedia :: Sound/Audio :: MIDI
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8.0
 Requires-Dist: huggingface-hub>=0.16.4
 Requires-Dist: numpy>=1.19
-Requires-Dist: symusic>=0.3.2
+Requires-Dist: symusic>=0.4.3
 Requires-Dist: tokenizers>=0.13.0
 Requires-Dist: tqdm
 Provides-Extra: docs
 Requires-Dist: furo; extra == 'docs'
 Requires-Dist: sphinx-copybutton; extra == 'docs'
 Requires-Dist: torch; extra == 'docs'
 Provides-Extra: tests
@@ -37,40 +37,40 @@
 Requires-Dist: pytest-xdist[psutil]; extra == 'tests'
 Requires-Dist: tensorflow; extra == 'tests'
 Requires-Dist: torch; extra == 'tests'
 Description-Content-Type: text/markdown
 
 # MidiTok
 
-Python package to tokenize MIDI music files, presented at the ISMIR 2021 LBDs.
+Python package to tokenize music files, introduced at the ISMIR 2021 LBDs.
 
 ![MidiTok Logo](docs/assets/logo.png?raw=true "")
 
 [![PyPI version fury.io](https://badge.fury.io/py/miditok.svg)](https://pypi.python.org/pypi/miditok/)
 [![Python 3.8](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/release/)
 [![Documentation Status](https://readthedocs.org/projects/miditok/badge/?version=latest)](https://miditok.readthedocs.io/en/latest/?badge=latest)
 [![GitHub CI](https://github.com/Natooz/MidiTok/actions/workflows/pytest.yml/badge.svg)](https://github.com/Natooz/MidiTok/actions/workflows/pytest.yml)
 [![Codecov](https://img.shields.io/codecov/c/github/Natooz/MidiTok)](https://codecov.io/gh/Natooz/MidiTok)
 [![GitHub license](https://img.shields.io/github/license/Natooz/MidiTok.svg)](https://github.com/Natooz/MidiTok/blob/main/LICENSE)
 [![Downloads](https://static.pepy.tech/badge/miditok)](https://pepy.tech/project/MidiTok)
 [![Code style](https://img.shields.io/badge/code%20style-ruff-000000.svg)](https://github.com/astral-sh/ruff)
 
-MidiTok can tokenize MIDI files, i.e. convert them into sequences of tokens ready to be fed to models such as Transformer, for any generation, transcription or MIR task.
-MidiTok features most known [MIDI tokenizations](https://miditok.readthedocs.io/en/latest/tokenizations.html) (e.g. [REMI](https://arxiv.org/abs/2002.00212), [Compound Word](https://arxiv.org/abs/2101.02402)...), and is built around the idea that they all share common parameters and methods. It supports [Byte Pair Encoding (BPE)](https://arxiv.org/abs/2301.11975) and data augmentation.
+MidiTok can tokenize MIDI and abc files, i.e. convert them into sequences of tokens ready to be fed to models such as Transformer, for any generation, transcription or MIR task.
+MidiTok features most known [music tokenizations](https://miditok.readthedocs.io/en/latest/tokenizations.html) (e.g. [REMI](https://arxiv.org/abs/2002.00212), [Compound Word](https://arxiv.org/abs/2101.02402)...), and is built around the idea that they all share common parameters and methods. Tokenizers can be trained with [Byte Pair Encoding (BPE)](https://aclanthology.org/2023.emnlp-main.123/), [Unigram](https://aclanthology.org/P18-1007/) and [WordPiece](https://arxiv.org/abs/1609.08144), and it offers data augmentation methods.
 
 MidiTok is integrated with the Hugging Face Hub 🤗! Don't hesitate to share your models to the community!
 
 **Documentation:** [miditok.readthedocs.com](https://miditok.readthedocs.io/en/latest/index.html)
 
 ## Install
 
 ```shell
 pip install miditok
 ```
-MidiTok uses [Symusic](https://github.com/Yikai-Liao/symusic) to read and write MIDI files, and BPE is backed by [Hugging Face 🤗tokenizers](https://github.com/huggingface/tokenizers) for super-fast encoding.
+MidiTok uses [Symusic](https://github.com/Yikai-Liao/symusic) to read and write MIDI and abc files, and BPE/Unigram is backed by [Hugging Face 🤗tokenizers](https://github.com/huggingface/tokenizers) for superfast encoding.
 
 ## Usage example
 
 Tokenizing and detokenzing can be done by calling the tokenizer:
 
 ```python
 from miditok import REMI, TokenizerConfig
@@ -79,54 +79,54 @@
 # Creating a multitrack tokenizer, read the doc to explore all the parameters
 config = TokenizerConfig(num_velocities=16, use_chords=True, use_programs=True)
 tokenizer = REMI(config)
 
 # Loads a midi, converts to tokens, and back to a MIDI
 midi = Score("path/to/your_midi.mid")
 tokens = tokenizer(midi)  # calling the tokenizer will automatically detect MIDIs, paths and tokens
-converted_back_midi = tokenizer(tokens)  # PyTorch / Tensorflow / Numpy tensors supported
+converted_back_midi = tokenizer(tokens)  # PyTorch, Tensorflow and Numpy tensors are supported
 ```
 
-Here is a complete yet concise example of how you can use MidiTok to train any PyTorch model. And [here](colab-notebooks/Full_Example_HuggingFace_GPT2_Transformer.ipynb) is a simple notebook example showing how to use Hugging Face models to generate music, with MidiTok taking care of tokenizing MIDIs.
+Here is a complete yet concise example of how you can use MidiTok to train any PyTorch model. And [here](colab-notebooks/Full_Example_HuggingFace_GPT2_Transformer.ipynb) is a simple notebook example showing how to use Hugging Face models to generate music, with MidiTok taking care of tokenizing music files.
 
 ```python
 from miditok import REMI, TokenizerConfig
-from miditok.pytorch_data import DatasetMIDI, DataCollator, split_midis_for_training
+from miditok.pytorch_data import DatasetMIDI, DataCollator, split_files_for_training
 from torch.utils.data import DataLoader
 from pathlib import Path
 
 # Creating a multitrack tokenizer, read the doc to explore all the parameters
 config = TokenizerConfig(num_velocities=16, use_chords=True, use_programs=True)
 tokenizer = REMI(config)
 
 # Train the tokenizer with Byte Pair Encoding (BPE)
-midi_paths = list(Path("path", "to", "midis").glob("**/*.mid"))
-tokenizer.learn_bpe(vocab_size=30000, files_paths=midi_paths)
+files_paths = list(Path("path", "to", "midis").glob("**/*.mid"))
+tokenizer.train(vocab_size=30000, files_paths=files_paths)
 tokenizer.save_params(Path("path", "to", "save", "tokenizer.json"))
 # And pushing it to the Hugging Face hub (you can download it back with .from_pretrained)
 tokenizer.push_to_hub("username/model-name", private=True, token="your_hf_token")
 
 # Split MIDIs into smaller chunks for training
 dataset_chunks_dir = Path("path", "to", "midi_chunks")
-split_midis_for_training(
-    files_paths=midi_paths,
+split_files_for_training(
+    files_paths=files_paths,
     tokenizer=tokenizer,
     save_dir=dataset_chunks_dir,
     max_seq_len=1024,
 )
 
 # Create a Dataset, a DataLoader and a collator to train a model
 dataset = DatasetMIDI(
     files_paths=list(dataset_chunks_dir.glob("**/*.mid")),
     tokenizer=tokenizer,
     max_seq_len=1024,
     bos_token_id=tokenizer["BOS_None"],
     eos_token_id=tokenizer["EOS_None"],
 )
-collator = DataCollator(tokenizer["PAD_None"])
+collator = DataCollator(tokenizer.pad_token_id)
 dataloader = DataLoader(dataset, batch_size=64, collate_fn=collator)
 
 # Iterate over the dataloader to train a model
 for batch in dataloader:
     print("Train your model on this batch...")
 ```
 
@@ -147,18 +147,18 @@
 
 ## Contributions
 
 Contributions are gratefully welcomed, feel free to open an issue or send a PR if you want to add a tokenization or speed up the code. You can read the [contribution guide](CONTRIBUTING.md) for details.
 
 ### Todos
 
+* Support music-xml files;
 * `no_duration_drums` option, discarding duration tokens for drum notes;
-* Extend unimplemented additional tokens to all compatible tokenizations;
 * Control Change messages;
-* Speeding up the MIDI preprocess + global/track events parsing with Rust or C++ binding.
+* Speed-up global/track events parsing with Rust or C++ bindings.
 
 ## Citation
 
 If you use MidiTok for your research, a citation in your manuscript would be gladly appreciated. ❤️
 
 [**[MidiTok paper]**](https://arxiv.org/abs/2310.17202)
 [**[MidiTok original ISMIR publication]**](https://archives.ismir.net/ismir2021/latebreaking/000005.pdf)
```

