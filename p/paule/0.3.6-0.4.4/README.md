# Comparing `tmp/paule-0.3.6.tar.gz` & `tmp/paule-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paule-0.3.6.tar", max compression
+gzip compressed data, was "paule-0.4.4.tar", max compression
```

## Comparing `paule-0.3.6.tar` & `paule-0.4.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    35149 2023-12-14 20:09:13.136970 paule-0.3.6/LICENSE
--rw-r--r--   0        0        0      470 2023-12-14 20:09:13.136970 paule-0.3.6/README.rst
--rw-r--r--   0        0        0     3066 2023-12-14 20:09:13.136970 paule-0.3.6/paule/__init__.py
--rw-r--r--   0        0        0    34445 2023-12-14 20:09:13.136970 paule-0.3.6/paule/gradient_planning.ipynb
--rw-r--r--   0        0        0    32654 2023-12-14 20:09:13.140970 paule-0.3.6/paule/models.py
--rw-r--r--   0        0        0    74932 2023-12-14 20:09:13.140970 paule-0.3.6/paule/paule.py
--rw-r--r--   0        0        0    32735 2023-12-14 20:09:13.140970 paule-0.3.6/paule/util.py
--rw-r--r--   0        0        0     7002 2023-12-14 20:09:13.140970 paule-0.3.6/paule/visualize.py
--rw-r--r--   0        0        0    91067 2023-12-14 20:09:13.140970 paule-0.3.6/paule/vocaltractlab_api/JD3.speaker
--rw-r--r--   0        0        0   645632 2023-12-14 20:09:13.144970 paule-0.3.6/paule/vocaltractlab_api/VocalTractLabApi.dll
--rwxr-xr-x   0        0        0   986240 2023-12-14 20:09:13.152970 paule-0.3.6/paule/vocaltractlab_api/libVocalTractLabApi.dylib
--rwxr-xr-x   0        0        0  1106344 2023-12-14 20:09:13.160970 paule-0.3.6/paule/vocaltractlab_api/libVocalTractLabApi.so
--rw-r--r--   0        0        0     2014 2023-12-14 20:09:13.160970 paule-0.3.6/pyproject.toml
--rw-r--r--   0        0        0     2019 1970-01-01 00:00:00.000000 paule-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0    35149 2021-04-12 16:18:04.987300 paule-0.4.4/LICENSE
+-rw-r--r--   0        0        0      470 2022-11-30 08:35:53.004096 paule-0.4.4/README.rst
+-rw-r--r--   0        0        0     3066 2023-01-19 20:53:16.541593 paule-0.4.4/paule/__init__.py
+-rw-r--r--   0        0        0    34445 2023-01-02 19:33:34.278200 paule-0.4.4/paule/gradient_planning.ipynb
+-rw-r--r--   0        0        0    36486 2024-03-21 14:24:24.491913 paule-0.4.4/paule/models.py
+-rw-r--r--   0        0        0    87784 2024-04-25 19:23:02.818076 paule-0.4.4/paule/paule.py
+-rw-r--r--   0        0        0    33971 2024-04-25 19:23:02.818076 paule-0.4.4/paule/util.py
+-rw-r--r--   0        0        0     8571 2024-03-21 20:45:38.437907 paule-0.4.4/paule/visualize.py
+-rw-r--r--   0        0        0    91067 2022-05-09 15:11:01.909215 paule-0.4.4/paule/vocaltractlab_api/JD3.speaker
+-rw-r--r--   0        0        0   645632 2023-01-02 19:34:41.854999 paule-0.4.4/paule/vocaltractlab_api/VocalTractLabApi.dll
+-rwxr-xr-x   0        0        0   986240 2023-01-02 12:42:06.425438 paule-0.4.4/paule/vocaltractlab_api/libVocalTractLabApi.dylib
+-rwxr-xr-x   0        0        0  1106344 2022-12-22 14:35:42.360610 paule-0.4.4/paule/vocaltractlab_api/libVocalTractLabApi.so
+-rw-r--r--   0        0        0     2015 2024-04-25 19:23:02.818076 paule-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0     2070 1970-01-01 00:00:00.000000 paule-0.4.4/PKG-INFO
```

### Comparing `paule-0.3.6/LICENSE` & `paule-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `paule-0.3.6/paule/__init__.py` & `paule-0.4.4/paule/__init__.py`

 * *Files identical despite different names*

### Comparing `paule-0.3.6/paule/gradient_planning.ipynb` & `paule-0.4.4/paule/gradient_planning.ipynb`

 * *Files identical despite different names*

### Comparing `paule-0.3.6/paule/models.py` & `paule-0.4.4/paule/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,20 @@
+import math
+
 import torch
+from torch.nn import (
+    Transformer,
+    TransformerEncoder,
+    Module,
+    Sequential,
+    Linear,
+    GELU,
+)
+from torch import nn
+
 
 
 ########################################################################################################################
 ######################################### Modules & Helper Functions ###################################################
 ########################################################################################################################
 def time_conv_Allx1(input_units):
     """Allx1 convolution over time (taking all input channels into account at each timestep"""
@@ -782,7 +794,118 @@
         output, _ = self.lstm(output)
         #output = torch.stack([output[i, (last - 1).long(), :] for i, last in enumerate(lens)])
         
         output = self.post_linear(output)
         output = self.output_activation(output)
 
         return output
+
+
+
+class PositionalEncoding(Module):
+    def __init__(self, d_model: int, dropout: float = 0.1, max_len: int = 5000):
+        super().__init__()
+
+        position = torch.arange(0, max_len)
+        position = position.unsqueeze(1)
+        div_term = torch.exp(
+            torch.arange(0, d_model, 2) * (-math.log(10000.0) / d_model)
+        )
+        pe = torch.zeros(max_len, d_model)
+        pe[:, 0::2] = torch.sin(position * div_term)
+        pe[:, 1::2] = torch.cos(position * div_term)
+        pe = pe.unsqueeze(0)
+        self.register_buffer("pe", pe)
+
+    def forward(self, input_):
+        output = input_ + self.pe[:, : input_.size(1), :]
+        return output
+
+
+class CustomTransformerEncoderLayer(nn.Module):
+    def __init__(
+        self, d_model, nhead, dim_feedforward=2048, dropout=0.1, activation=GELU()
+    ):
+        super(CustomTransformerEncoderLayer, self).__init__()
+        self.self_attn = nn.MultiheadAttention(
+            d_model, nhead, dropout=dropout, batch_first=True
+        )
+        self.linear1 = nn.Linear(d_model, dim_feedforward)
+        self.dropout = nn.Dropout(dropout)
+        self.linear2 = nn.Linear(dim_feedforward, d_model)
+
+        self.norm1 = nn.LayerNorm(d_model)
+        self.norm2 = nn.LayerNorm(d_model)
+        self.dropout1 = nn.Dropout(dropout)
+        self.dropout2 = nn.Dropout(dropout)
+
+        self.activation = activation
+
+    def forward(self, src, src_mask=None, src_key_padding_mask=None, is_causal=None):
+        src2 = self.self_attn(
+            src, src, src, attn_mask=src_mask, key_padding_mask=src_key_padding_mask
+        )[0]
+        src = src + self.dropout1(src2)
+        src = self.norm1(src)
+
+        src2 = self.linear2(self.dropout(self.activation(self.linear1(src))))
+        src = src + self.dropout2(src2)
+        src = self.norm2(src)
+
+        return src
+
+
+class SpeechNonSpeechTransformer(Transformer):
+    def __init__(self, input_dim, num_layers, nhead, output_dim):
+        super().__init__()
+
+        self.pos_encoder = PositionalEncoding(input_dim, dropout=0.1)
+        self.encoder_layer = CustomTransformerEncoderLayer(
+            d_model=input_dim, nhead=nhead, dim_feedforward=1024, activation=GELU()
+        )
+        self.transformer_encoder = TransformerEncoder(
+            self.encoder_layer, num_layers=num_layers, enable_nested_tensor=False
+        )
+        self.linear = Sequential(Linear(input_dim, 20), GELU(), Linear(20, 1))
+
+
+    def forward(self, input_, *, src_lens=None):
+        mask = torch.zeros((input_.size(0), input_.size(1)), device=input_.device, dtype=input_.dtype)
+        if src_lens is not None:
+            for ii, len_ in enumerate(src_lens):
+                mask[ii, len_:] = float("-inf")
+
+        output = self.pos_encoder(input_)
+        output = self.transformer_encoder(output, src_key_padding_mask=mask)
+        output = output.mean(dim=1)
+        output = self.linear(output)
+
+        output = torch.squeeze(output, 1)
+
+        return output
+
+
+class LinearClassifier(Module):
+    def __init__(self, input_dim, output_dim):
+        super().__init__()
+
+        self.linear = Linear(input_dim, output_dim)
+
+
+    def forward(self, input_, *, src_lens=None):
+
+        output = self.linear(input_)
+        output = torch.squeeze(output, 2)
+
+        # set all padded values to zero
+        if src_lens is not None:
+            for ii, len_ in enumerate(src_lens):
+                output[ii, len_:] = 0.0
+
+        # sum all values and devide by seq length
+        if src_lens is not None:
+            output = output.sum(dim=1) / torch.tensor(src_lens, device=output.device)
+        else:
+            output = output.mean(dim=1)
+
+        return output
+
```

### Comparing `paule-0.3.6/paule/paule.py` & `paule-0.4.4/paule/paule.py`

 * *Files 7% similar despite different names*

```diff
@@ -40,60 +40,54 @@
 
 tqdm.pandas()
 
 from .util import (speak, inv_normalize_cp, normalize_mel_librosa,
         stereo_to_mono, librosa_melspec, RMSELoss, get_vel_acc_jerk,
         cp_trajectory_loss, mel_to_sig, pad_batch_online,
         speak_and_extract_tube_information, normalize_tube,
-        get_area_info_within_oral_cavity, get_pretrained_weights_version)
+        get_area_info_within_oral_cavity, get_pretrained_weights_version, local_linear)
 
-from .models import (ForwardModel, InverseModelMelTimeSmoothResidual, EmbeddingModel, Generator, NonLinearModel)
+from .models import (ForwardModel, InverseModelMelTimeSmoothResidual,
+        EmbeddingModel, Generator, NonLinearModel, SpeechNonSpeechTransformer, LinearClassifier)
 
 from . import visualize
 
 DIR = os.path.dirname(__file__)
 
 
 PlanningResults = namedtuple('PlanningResults', "planned_cp, initial_cp, initial_sig, initial_sr, initial_prod_mel,initial_pred_mel, target_sig, target_sr, target_mel, prod_sig, prod_sr, prod_mel, pred_mel, initial_prod_semvec, initial_pred_semvec, prod_semvec, pred_semvec, prod_loss_steps, planned_loss_steps, planned_mel_loss_steps, vel_loss_steps, jerk_loss_steps, pred_semvec_loss_steps, prod_semvec_loss_steps, cp_steps, pred_semvec_steps, prod_semvec_steps, grad_steps, sig_steps, prod_mel_steps, pred_mel_steps, pred_model_loss, inv_model_loss")
+PlanningResultsWithSpeechClassifier = namedtuple('PlanningResultsWithSpeechClassifier', "planned_cp, initial_cp, initial_sig, initial_sr, initial_prod_mel, initial_pred_mel, target_sig, target_sr, target_mel, prod_sig, prod_sr, prod_mel, pred_mel, initial_prod_semvec, initial_pred_semvec, prod_semvec, pred_semvec, prod_loss_steps, planned_loss_steps, planned_mel_loss_steps, vel_loss_steps, jerk_loss_steps, pred_semvec_loss_steps, prod_semvec_loss_steps, pred_speech_classifier_loss_steps, prod_speech_classifier_loss_steps, cp_steps, pred_semvec_steps, prod_semvec_steps, grad_steps, sig_steps, prod_mel_steps, pred_mel_steps, pred_model_loss, inv_model_loss")
 PlanningResultsWithSomatosensory = namedtuple('PlanningResultsWithSomatosensory', "planned_cp, initial_cp, initial_sig, initial_sr, initial_prod_mel,initial_pred_mel, initial_prod_tube, initial_pred_tube, initial_prod_tube_mel, initial_pred_tube_mel, target_sig, target_sr, target_mel, prod_sig, prod_sr, prod_mel, pred_mel, prod_tube, pred_tube, prod_tube_mel, pred_tube_mel, initial_prod_semvec, initial_pred_semvec, initial_prod_tube_semvec, initial_pred_tube_semvec, prod_semvec, pred_semvec, prod_tube_semvec, pred_tube_semvec, prod_loss_steps, planned_loss_steps, planned_mel_loss_steps, vel_loss_steps, jerk_loss_steps, pred_semvec_loss_steps, prod_semvec_loss_steps, prod_tube_loss_steps, pred_tube_mel_loss_steps,prod_tube_mel_loss_steps, pred_tube_semvec_loss_steps, prod_tube_semvec_loss_steps, cp_steps, pred_semvec_steps, prod_semvec_steps, grad_steps, sig_steps, prod_mel_steps, pred_mel_steps, prod_tube_steps, pred_tube_steps, prod_tube_mel_steps, pred_tube_mel_steps, prod_tube_semvec_steps, pred_tube_semvec_steps, pred_model_loss, inv_model_loss, tube_model_loss, tube_mel_model_loss")
 
+
 BestSynthesisAcoustic = namedtuple('BestSynthesisAcoustic', "mel_loss, planned_cp, prod_sig, prod_mel, pred_mel")
 BestSynthesisSemantic = namedtuple('BestSynthesisSemantic', "semvec_loss, planned_cp, prod_sig, prod_semvec, pred_semvec")
 BestSynthesisSomatosensory = namedtuple('BestSynthesisSomatosensory',"tube_loss, tube_mel_loss, tube_semvec_loss, planned_cp, prod_sig, prod_tube, pred_tube, prod_tube_mel, pred_tube_mel, prod_tube_semvec, pred_tube_semvec")
 
+SubLosses = namedtuple('SubLosses', "mel_loss, semvec_loss, velocity_loss, jerk_loss, local_linear_loss, speech_classifier_loss, tube_mel_loss, tube_semvec_loss")
+
 rmse_loss = RMSELoss(eps=0)
-l2 = MSELoss()
+mse_loss = l2 = MSELoss()
 l1 = L1Loss()
+bce_loss = torch.nn.BCEWithLogitsLoss()
 
 
-def velocity_jerk_loss(pred, loss, *, guiding_factor=None):
-    """returns (velocity_loss, jerk_loss) tuple"""
-    vel1, acc1, jerk1 = get_vel_acc_jerk(pred)
-    vel2, acc2, jerk2 = get_vel_acc_jerk(pred, lag=2)
-    vel4, acc4, jerk4 = get_vel_acc_jerk(pred, lag=4)
 
-    loss = rmse_loss
+def velocity_jerk_loss(pred, *, loss=rmse_loss, guiding_factor=None):
+    """returns (velocity_loss, jerk_loss) tuple"""
+    #vel1, acc1, jerk1 = get_vel_acc_jerk(pred, delta_t=1.0/401)
+    vel1, acc1, jerk1 = get_vel_acc_jerk(pred, delta_t=1.0)
 
-    # in the lag calculation higher lags are already normalised to standard
-    # units
     if guiding_factor is None:
-        velocity_loss = (loss(vel1, torch.zeros_like(vel1))
-                         + loss(vel2, torch.zeros_like(vel2))
-                         + loss(vel4, torch.zeros_like(vel4)))
-        jerk_loss = (loss(jerk1, torch.zeros_like(jerk1))
-                     + loss(jerk2, torch.zeros_like(jerk2))
-                     + loss(jerk4, torch.zeros_like(jerk4)))
+        velocity_loss = loss(vel1, torch.zeros_like(vel1))
+        jerk_loss = loss(jerk1, torch.zeros_like(jerk1))
     else:
         assert 0.0 < guiding_factor < 1.0
-        velocity_loss = (loss(vel1, guiding_factor * vel1.detach().clone())
-                         + loss(vel2, guiding_factor * vel2.detach().clone())
-                         + loss(vel4, guiding_factor * vel4.detach().clone()))
-        jerk_loss = (loss(jerk1, guiding_factor * jerk1.detach().clone())
-                     + loss(jerk2, guiding_factor * jerk2.detach().clone())
-                     + loss(jerk4, guiding_factor * jerk4.detach().clone()))
+        velocity_loss = loss(vel1, guiding_factor * vel1.detach().clone())
+        jerk_loss = loss(jerk1, guiding_factor * jerk1.detach().clone())
 
     return velocity_loss, jerk_loss
 
 
 
 class Paule():
     """
@@ -104,24 +98,29 @@
 
     """
 
     def __init__(self, *, pred_model=None, pred_optimizer=None, inv_model=None, inv_optimizer=None,
                  embedder=None, cp_gen_model=None, mel_gen_model=None,
                  use_somatosensory_feedback=False, cp_tube_model=None, tube_optimizer=None,
                  tube_mel_model=None, tube_mel_optimizer=None, tube_embedder=None,
-                 continue_data=None, device=torch.device('cpu'), smiling=False):
+                 continue_data=None, device=torch.device('cpu'), smiling=False,
+                 use_speech_classifier=False, speech_classifier=None,
+                 speech_classifier_optimizer=None):
 
         # load the pred_model, inv_model and embedder here
         # for cpu
         self.device = device
 
         self.smiling = smiling
 
         print(f'Version of pretrained weights is "{get_pretrained_weights_version()}"')
 
+        if use_somatosensory_feedback and use_speech_classifier:
+            raise NotImplementedError("at the moment you have to choose either to use `use_somatosenrosry_feedback=True` OR to use `use_speech_classifier=True` or none")
+
         # PREDictive MODEL (cp -> mel)
         if pred_model:
             self.pred_model = pred_model
         else:
             self.pred_model = ForwardModel(num_lstm_layers=1, hidden_size=720).double()
             self.pred_model.load_state_dict(
                 torch.load(os.path.join(DIR, "pretrained_models/predictive/pred_model_common_voice_1_720_lr_0001_50_00001_50_000001_50_0000001_200.pt"),
@@ -199,14 +198,30 @@
             self.mel_gen_model = Generator(output_size=60).double()
             self.mel_gen_model.load_state_dict(torch.load(
                 os.path.join(DIR, "pretrained_models/mel_gan/conditional_trained_mel_generator_synthesized_critic_it_5_10_20_40_80_100_400.pt"),
                                                           map_location=self.device))
         self.mel_gen_model = self.mel_gen_model.to(self.device)
         self.mel_gen_model.eval()
 
+        self.use_speech_classifier = use_speech_classifier
+        if self.use_speech_classifier:
+            # SPEECH CLASSIFIER (binary classifier with 0 is speech-like)
+            if speech_classifier:
+                self.speech_classifier = speech_classifier
+            else:
+                self.speech_classifier = LinearClassifier(input_dim=60, output_dim=1)
+                #self.speech_classifier = SpeechNonSpeechTransformer(input_dim=60, num_layers=3, nhead=6, output_dim=1)
+                self.speech_classifier.load_state_dict(torch.load(
+                    os.path.join(DIR, "pretrained_models/speech_classifier/linear_model_rec_as_nonspeech.pt"),
+                    #os.path.join(DIR, "pretrained_models/speech_classifier/model_rec_as_nonspeech.pt"),
+                           map_location=self.device))
+                self.speech_classifier = self.speech_classifier.double()
+            self.speech_classifier = self.speech_classifier.to(self.device)
+            self.speech_classifier.eval()
+
         self.use_somatosensory_feedback = use_somatosensory_feedback
         if self.use_somatosensory_feedback:
             # CP-Tube Model (cp -> tube)
             if cp_tube_model:
                 self.cp_tube_model = cp_tube_model
             else:
                 self.cp_tube_model = ForwardModel(num_lstm_layers=1,
@@ -244,15 +259,14 @@
                                                     post_upsampling_size=0).double()
                 self.tube_embedder.load_state_dict(torch.load(
                     os.path.join(DIR, "pretrained_models/somatosensory/tube_to_vector_model_2_720_0_dropout_07_noise_6e05_rmse_lr_00001_200.pt"),
                            map_location=self.device))
             self.tube_embedder = self.tube_embedder.to(self.device)
             self.tube_embedder.eval()
 
-
         # DATA to continue learning
         self.continue_data = continue_data
         self.continue_data_limit = 1000  # max amount of training data stored in paule instance
 
         if self.continue_data is not None:
             if len(self.continue_data) > self.continue_data_limit:
                 random_sample = random.sample(range(len(self.continue_data)), self.continue_data_limit)
@@ -278,14 +292,21 @@
             self.tube_criterion = rmse_loss
             if tube_mel_optimizer:
                 self.tube_mel_optimizer = tube_optimizer
             else:
                 self.tube_mel_optimizer = torch.optim.Adam(self.tube_mel_model.parameters(), lr=0.001)
             self.tube_mel_criterion = rmse_loss
 
+        if self.use_speech_classifier:
+            if speech_classifier_optimizer:
+                self.speech_classifier_optimizer = speech_classifier_optimizer
+            else:
+                self.speech_classifier_optimizer = torch.optim.Adam(self.speech_classifier.parameters(), lr=0.001)
+            self.speech_classifier_criterion = torch.nn.BCEWithLogitsLoss()
+
         self.best_synthesis_acoustic = None
         self.best_synthesis_semantic = None
         if self.use_somatosensory_feedback:
             self.best_synthesis_somatosensory = None
 
     def create_epoch_batches(self, df_length, batch_size, shuffle=True, same_size_batching=False, sorted_training_length_keys=None, training_length_dict=None):
         """
@@ -457,29 +478,44 @@
             target_sig, target_sr = sf.read(target_acoustic)
             if len(target_sig.shape) == 2:
                 target_sig = stereo_to_mono(target_sig)
             # assert target_sr == 44100, 'sampling rate of wave name must be 44100'
 
         elif target_acoustic is None:
             pass
-        else:
+        elif len(target_acoustic) == 2:
             target_sig, target_sr = target_acoustic
+        else:
+            if len(target_acoustic.shape) == 2:
+                target_mel = target_acoustic.copy()
+                target_mel.shape = (1,) + target_mel.shape
+                target_mel = torch.from_numpy(target_mel)
+            else:
+                if not isinstance(target_acoustic, torch.Tensor):
+                    target_mel = torch.from_numpy(target_acoustic)
+                else:
+                    target_mel = target_acoustic.copy()
+            if not isinstance(target_mel, torch.Tensor):
+                raise ValueError("target_acoustic has to be torch.Tensor at this point")
+            target_seq_length = target_mel.shape[1]
+            target_sig = None
+            target_sr = None
+
 
         if target_acoustic is None and (target_seq_length is None or target_semvec is None):
             raise ValueError("if target_acoustic is None you need to give a target_seq_length and a target_semvec")
-
         elif target_acoustic is None:
             mel_gen_noise = torch.randn(1, 1, 100).to(self.device)
             if not isinstance(target_semvec, torch.Tensor):
                 target_semvec = torch.tensor(target_semvec)
             mel_gen_semvec = target_semvec.view(1, 300).detach().clone()
             target_mel = self.mel_gen_model(mel_gen_noise, target_seq_length, mel_gen_semvec)
             target_mel = target_mel.detach().clone()
             target_sig, target_sr = mel_to_sig(target_mel.view(target_mel.shape[1], target_mel.shape[2]).cpu().numpy())
-        else:
+        elif len(target_acoustic) == 2 or isinstance(target_acoustic, str):
             target_mel = librosa_melspec(target_sig, target_sr)
             target_mel = normalize_mel_librosa(target_mel)
             target_mel -= target_mel.min()
             target_mel.shape = (1,) + target_mel.shape
             target_mel = torch.from_numpy(target_mel)
             target_seq_length = target_mel.shape[1]
 
@@ -509,15 +545,15 @@
                     initial_cp = self.inv_model(xx)
                 initial_cp = initial_cp.detach().cpu().numpy().clip(min=-1, max=1)
                 initial_cp.shape = (initial_cp.shape[1], initial_cp.shape[2])
                 del xx
             elif initialize_from == "semvec":
                 cp_gen_noise = torch.randn(1, 1, 100).to(self.device)
                 if not isinstance(target_semvec, torch.Tensor):
-                    target_semvec = torch.tensor(target_semvec)
+                    target_semvec = torch.tensor(target_semvec, device=self.device)
                 cp_gen_semvec = target_semvec.view(1, 300).detach().clone()
                 initial_cp = self.cp_gen_model(cp_gen_noise, 2 * target_seq_length, cp_gen_semvec)
                 initial_cp = initial_cp.detach().cpu().numpy()
                 initial_cp.shape = (initial_cp.shape[1], initial_cp.shape[2])
             else:
                 raise ValueError("initialize_from has to be either 'acoustic' or 'semvec'")
 
@@ -540,82 +576,196 @@
         xx_new = initial_cp.copy()
         xx_new.shape = (1, xx_new.shape[0], xx_new.shape[1])
         xx_new = torch.from_numpy(xx_new)
         xx_new = xx_new.to(self.device)
         xx_new.requires_grad_()
         xx_new.retain_grad()
 
+        MEL_WEIGHT = 5.0
+        VELOCITY_WEIGHT = 80.0  # alternative: 1000
+        JERK_WEIGHT = 400.0  # alternative: 4000
+        SEMANTIC_WEIGHT = 10.0
+        SPEECH_CLASSIFIER_WEIGHT = 0.1
+        LOCAL_LINEAR_WEIGHT = 100_000
+        TUBE_MEL_WEIGHT = MEL_WEIGHT
+        TUBE_SEMANTIC_WEIGHT = SEMANTIC_WEIGHT
+
 
         if objective == 'acoustic_semvec':
-            if self.use_somatosensory_feedback:
+            if self.use_speech_classifier:
+                def criterion(pred_mel, target_mel, pred_semvec, target_semvec, cps, pred_speech_classifier):
+                    mel_loss = rmse_loss(pred_mel, target_mel)
+                    semvec_loss = rmse_loss(pred_semvec, target_semvec)
+                    velocity_loss, jerk_loss = velocity_jerk_loss(cps, loss=mse_loss)
+                    ll = local_linear(cps)
+                    local_linear_loss = mse_loss(ll, torch.zeros_like(ll, dtype=ll.dtype))
+                    speech_classifier_loss = bce_loss(pred_speech_classifier,
+                            torch.zeros_like(pred_speech_classifier,
+                                dtype=pred_speech_classifier.dtype))
+
+                    mel_loss = MEL_WEIGHT * mel_loss
+                    semvec_loss = SEMANTIC_WEIGHT * semvec_loss
+                    velocity_loss = VELOCITY_WEIGHT * velocity_loss
+                    jerk_loss = JERK_WEIGHT * jerk_loss
+                    local_linear_loss = LOCAL_LINEAR_WEIGHT * local_linear_loss
+                    speech_classifier_loss = SPEECH_CLASSIFIER_WEIGHT * speech_classifier_loss
+
+                    loss = mel_loss + velocity_loss + jerk_loss + semvec_loss + speech_classifier_loss + local_linear_loss
+                    return loss, SubLosses(mel_loss, semvec_loss, velocity_loss, jerk_loss, local_linear_loss, speech_classifier_loss, None, None)
+
+            elif self.use_somatosensory_feedback:
                 def criterion(pred_mel, target_mel, pred_semvec, target_semvec, cps, pred_tube_mel, pred_tube_semvec):
                     mel_loss = rmse_loss(pred_mel, target_mel)
                     semvec_loss = rmse_loss(pred_semvec, target_semvec)
-                    velocity_loss, jerk_loss = velocity_jerk_loss(cps, rmse_loss)
+                    velocity_loss, jerk_loss = velocity_jerk_loss(cps, loss=mse_loss)
+                    ll = local_linear(cps)
+                    local_linear_loss = mse_loss(ll, torch.zeros_like(ll, dtype=ll.dtype))
                     tube_mel_loss = rmse_loss(pred_tube_mel, target_mel)
                     tube_semvec_loss = rmse_loss(pred_tube_semvec, target_semvec)
-                    velocity_loss = 4 * velocity_loss
-                    jerk_loss = 4 * jerk_loss
-                    semvec_loss = 10 * semvec_loss
-                    tube_mel_loss = tube_mel_loss
-                    tube_semvec_loss = 10 * tube_semvec_loss
-                    loss = mel_loss + velocity_loss + jerk_loss + semvec_loss + tube_mel_loss + tube_semvec_loss
-                    return loss, mel_loss, velocity_loss, jerk_loss, semvec_loss, tube_mel_loss, tube_semvec_loss
+
+                    mel_loss = MEL_WEIGHT * mel_loss
+                    semvec_loss = SEMANTIC_WEIGHT * semvec_loss
+                    velocity_loss = VELOCITY_WEIGHT * velocity_loss
+                    jerk_loss = JERK_WEIGHT * jerk_loss
+                    local_linear_loss = LOCAL_LINEAR_WEIGHT * local_linear_loss
+                    tube_mel_loss = TUBE_MEL_WEIGHT * tube_mel_loss
+                    tube_semvec_loss = TUBE_SEMANTIC_WEIGHT * tube_semvec_loss
+
+                    loss = mel_loss + velocity_loss + jerk_loss + semvec_loss + local_linear_loss + tube_mel_loss + tube_semvec_loss
+
+                    return loss, SubLosses(mel_loss, semvec_loss, velocity_loss, jerk_loss, local_linear_loss, None, tube_mel_loss, tube_semvec_loss)
+
             else:
                 def criterion(pred_mel, target_mel, pred_semvec, target_semvec, cps):
                     mel_loss = rmse_loss(pred_mel, target_mel)
                     semvec_loss = rmse_loss(pred_semvec, target_semvec)
-                    velocity_loss, jerk_loss = velocity_jerk_loss(cps, rmse_loss)
-                    velocity_loss = 2 * velocity_loss
-                    jerk_loss = 2 * jerk_loss
-                    semvec_loss = 10 * semvec_loss
-                    loss = mel_loss + velocity_loss + jerk_loss + semvec_loss
-                    return loss, mel_loss, velocity_loss, jerk_loss, semvec_loss
+                    velocity_loss, jerk_loss = velocity_jerk_loss(cps, loss=mse_loss)
+                    ll = local_linear(cps)
+                    local_linear_loss = mse_loss(ll, torch.zeros_like(ll, dtype=ll.dtype))
+
+                    mel_loss = MEL_WEIGHT * mel_loss
+                    semvec_loss = SEMANTIC_WEIGHT * semvec_loss
+                    velocity_loss = VELOCITY_WEIGHT * velocity_loss
+                    jerk_loss = JERK_WEIGHT * jerk_loss
+                    local_linear_loss = LOCAL_LINEAR_WEIGHT * local_linear_loss
+
+                    loss = mel_loss + velocity_loss + jerk_loss + semvec_loss + local_linear_loss
+
+                    return loss, SubLosses(mel_loss, semvec_loss, velocity_loss, jerk_loss, local_linear_loss, None, None, None)
 
         elif objective == 'acoustic':
-            if self.use_somatosensory_feedback:
+            if self.use_speech_classifier:
+                def criterion(pred_mel, target_mel, cps, pred_speech_classifier):
+                    mel_loss = rmse_loss(pred_mel, target_mel)
+                    velocity_loss, jerk_loss = velocity_jerk_loss(cps, loss=mse_loss)
+                    ll = local_linear(cps)
+                    local_linear_loss = mse_loss(ll, torch.zeros_like(ll, dtype=ll.dtype))
+                    speech_classifier_loss = bce_loss(pred_speech_classifier,
+                            torch.zeros_like(pred_speech_classifier,
+                                dtype=pred_speech_classifier.dtype))
+
+                    mel_loss = MEL_WEIGHT * mel_loss
+                    velocity_loss = VELOCITY_WEIGHT * velocity_loss
+                    jerk_loss = JERK_WEIGHT * jerk_loss
+                    local_linear_loss = LOCAL_LINEAR_WEIGHT * local_linear_loss
+                    speech_classifier_loss = SPEECH_CLASSIFIER_WEIGHT * speech_classifier_loss
+
+                    loss = mel_loss + velocity_loss + jerk_loss + local_linear_loss + speech_classifier_loss
+
+                    return loss, SubLosses(mel_loss, None, velocity_loss, jerk_loss, local_linear_loss, speech_classifier_loss, None, None)
+
+            elif self.use_somatosensory_feedback:
                 def criterion(pred_mel, target_mel, cps, pred_tube_mel):
                     mel_loss = rmse_loss(pred_mel, target_mel)
-                    velocity_loss, jerk_loss = velocity_jerk_loss(cps, rmse_loss)
+                    velocity_loss, jerk_loss = velocity_jerk_loss(cps, loss=mse_loss)
+                    ll = local_linear(cps)
+                    local_linear_loss = mse_loss(ll, torch.zeros_like(ll, dtype=ll.dtype))
                     tube_mel_loss = rmse_loss(pred_tube_mel, target_mel)
-                    velocity_loss = 4 * velocity_loss
-                    jerk_loss = 4 * jerk_loss
-                    tube_mel_loss = tube_mel_loss
-                    loss = mel_loss + velocity_loss + jerk_loss + tube_mel_loss
-                    return loss, mel_loss, velocity_loss, jerk_loss, tube_mel_loss
+                    tube_semvec_loss = rmse_loss(pred_tube_semvec, target_semvec)
+
+                    mel_loss = MEL_WEIGHT * mel_loss
+                    velocity_loss = VELOCITY_WEIGHT * velocity_loss
+                    jerk_loss = JERK_WEIGHT * jerk_loss
+                    local_linear_loss = LOCAL_LINEAR_WEIGHT * local_linear_loss
+                    tube_mel_loss = TUBE_MEL_WEIGHT * tube_mel_loss
+                    tube_semvec_loss = TUBE_SEMANTIC_WEIGHT * tube_semvec_loss
+
+                    loss = mel_loss + velocity_loss + jerk_loss + local_linear_loss + tube_mel_loss + tube_semvec_loss
+                    return loss, SubLosses(mel_loss, None, velocity_loss, jerk_loss, local_linear_loss, None, tube_mel_loss, tube_semvec_loss)
+
             else:
                 def criterion(pred_mel, target_mel, cps):
                     mel_loss = rmse_loss(pred_mel, target_mel)
-                    velocity_loss, jerk_loss = velocity_jerk_loss(cps, rmse_loss)
-                    velocity_loss = 2 * velocity_loss
-                    jerk_loss = 2 * jerk_loss
-                    loss = mel_loss + velocity_loss + jerk_loss
-                    return loss, mel_loss, velocity_loss, jerk_loss
+                    velocity_loss, jerk_loss = velocity_jerk_loss(cps, loss=mse_loss)
+                    ll = local_linear(cps)
+                    local_linear_loss = mse_loss(ll, torch.zeros_like(ll, dtype=ll.dtype))
+
+                    mel_loss = MEL_WEIGHT * mel_loss
+                    velocity_loss = VELOCITY_WEIGHT * velocity_loss
+                    jerk_loss = JERK_WEIGHT * jerk_loss
+                    local_linear_loss = LOCAL_LINEAR_WEIGHT * local_linear_loss
+
+                    loss = mel_loss + velocity_loss + jerk_loss + local_linear_loss
+                    return loss, SubLosses(mel_loss, None, velocity_loss, jerk_loss, local_linear_loss, None, None, None)
 
         elif objective == 'semvec':
-            if self.use_somatosensory_feedback:
+            if self.use_speech_classifier:
+                def criterion(pred_semvec, target_semvec, cps, pred_speech_classifier):
+                    semvec_loss = rmse_loss(pred_semvec, target_semvec)
+                    velocity_loss, jerk_loss = velocity_jerk_loss(cps, loss=mse_loss)
+                    ll = local_linear(cps)
+                    local_linear_loss = mse_loss(ll, torch.zeros_like(ll, dtype=ll.dtype))
+                    speech_classifier_loss = bce_loss(pred_speech_classifier,
+                            torch.zeros_like(pred_speech_classifier,
+                                dtype=pred_speech_classifier.dtype))
+
+                    semvec_loss = SEMANTIC_WEIGHT * semvec_loss
+                    velocity_loss = VELOCITY_WEIGHT * velocity_loss
+                    jerk_loss = JERK_WEIGHT * jerk_loss
+                    local_linear_loss = LOCAL_LINEAR_WEIGHT * local_linear_loss
+                    speech_classifier_loss = SPEECH_CLASSIFIER_WEIGHT * speech_classifier_loss
+
+                    loss = velocity_loss + jerk_loss + semvec_loss + speech_classifier_loss + local_linear_loss
+                    return loss, SubLosses(None, semvec_loss, velocity_loss, jerk_loss, local_linear_loss, speech_classifier_loss, None, None)
+
+            elif self.use_somatosensory_feedback:
                 def criterion(pred_semvec, target_semvec, cps, pred_tube_semvec):
                     semvec_loss = rmse_loss(pred_semvec, target_semvec)
-                    velocity_loss, jerk_loss = velocity_jerk_loss(cps, rmse_loss)
+                    velocity_loss, jerk_loss = velocity_jerk_loss(cps, loss=mse_loss)
+                    ll = local_linear(cps)
+                    local_linear_loss = mse_loss(ll, torch.zeros_like(ll, dtype=ll.dtype))
+                    tube_mel_loss = rmse_loss(pred_tube_mel, target_mel)
                     tube_semvec_loss = rmse_loss(pred_tube_semvec, target_semvec)
-                    velocity_loss = 4 * velocity_loss
-                    jerk_loss = 4 * jerk_loss
-                    semvec_loss = 10 * semvec_loss
-                    tube_semvec_loss = 10 * tube_semvec_loss
-                    loss = velocity_loss + jerk_loss + semvec_loss + tube_semvec_loss
-                    return loss, velocity_loss, jerk_loss, semvec_loss, tube_semvec_loss
+
+                    semvec_loss = SEMANTIC_WEIGHT * semvec_loss
+                    velocity_loss = VELOCITY_WEIGHT * velocity_loss
+                    jerk_loss = JERK_WEIGHT * jerk_loss
+                    local_linear_loss = LOCAL_LINEAR_WEIGHT * local_linear_loss
+                    tube_mel_loss = TUBE_MEL_WEIGHT * tube_mel_loss
+                    tube_semvec_loss = TUBE_SEMANTIC_WEIGHT * tube_semvec_loss
+
+                    loss = velocity_loss + jerk_loss + semvec_loss + local_linear_loss + tube_mel_loss + tube_semvec_loss
+
+                    return loss, SubLosses(None, semvec_loss, velocity_loss, jerk_loss, local_linear_loss, None, tube_mel_loss, tube_semvec_loss)
+
             else:
                 def criterion(pred_semvec, target_semvec, cps):
                     semvec_loss = rmse_loss(pred_semvec, target_semvec)
-                    velocity_loss, jerk_loss = velocity_jerk_loss(cps, rmse_loss)
-                    velocity_loss = 2 * velocity_loss
-                    jerk_loss = 2 * jerk_loss
-                    semvec_loss = 10 * semvec_loss
-                    loss = velocity_loss + jerk_loss + semvec_loss
-                    return loss, velocity_loss, jerk_loss, semvec_loss
+                    velocity_loss, jerk_loss = velocity_jerk_loss(cps, loss=mse_loss)
+                    ll = local_linear(cps)
+                    local_linear_loss = mse_loss(ll, torch.zeros_like(ll, dtype=ll.dtype))
+
+                    semvec_loss = SEMANTIC_WEIGHT * semvec_loss
+                    velocity_loss = VELOCITY_WEIGHT * velocity_loss
+                    jerk_loss = JERK_WEIGHT * jerk_loss
+                    local_linear_loss = LOCAL_LINEAR_WEIGHT * local_linear_loss
+
+                    loss = velocity_loss + jerk_loss + semvec_loss + local_linear_loss
+
+                    return loss, SubLosses(None, semvec_loss, velocity_loss, jerk_loss, local_linear_loss, None, None, None)
 
         else:
             raise ValueError("objective has to be one of 'acoustic_semvec', 'acoustic' or 'semvec'")
 
         # 1.0 create variables for logging
         prod_loss_steps = list()
         planned_loss_steps = list()
@@ -649,14 +799,18 @@
             prod_tube_mel_steps = list()
             pred_tube_mel_steps = list()
             pred_tube_semvec_steps = list()
             prod_tube_semvec_steps = list()
 
             tube_model_loss = list()
             tube_mel_model_loss = list()
+        elif self.use_speech_classifier:
+            prod_speech_classifier_loss_steps = list()
+            pred_speech_classifier_loss_steps = list()
+
 
 
         # initial results
         with torch.no_grad():
             initial_pred_mel = self.pred_model(xx_new)
             initial_pred_semvec = self.embedder(initial_pred_mel, (torch.tensor(initial_pred_mel.shape[1]),))
 
@@ -690,15 +844,15 @@
             initial_prod_tube_mel = initial_prod_tube_mel[-1, :, :].detach().cpu().numpy().copy()
             initial_pred_tube_mel = initial_pred_tube_mel[-1, :, :].detach().cpu().numpy().copy()
             initial_prod_tube_semvec = initial_prod_tube_semvec[-1, :].detach().cpu().numpy().copy()
             initial_pred_tube_semvec = initial_pred_tube_semvec[-1, :].detach().cpu().numpy().copy()
 
         else:
             initial_sig, initial_sr = speak(inv_normalize_cp(xx_new_numpy))
-        
+
         initial_prod_mel = librosa_melspec(initial_sig, initial_sr)
         initial_prod_mel = normalize_mel_librosa(initial_prod_mel)
         initial_prod_mel.shape = initial_pred_mel.shape
         initial_prod_mel = torch.from_numpy(initial_prod_mel)
         initial_prod_mel = initial_prod_mel.to(self.device)
 
         # if past_cp prepend the first past_cp / 2 steps to target_mel
@@ -711,15 +865,15 @@
 
         initial_prod_mel = initial_prod_mel[-1, :, :].detach().cpu().numpy().copy()
         initial_pred_mel = initial_pred_mel[-1, :, :].detach().cpu().numpy().copy()
         initial_prod_semvec = initial_prod_semvec[-1, :].detach().cpu().numpy().copy()
         initial_pred_semvec = initial_pred_semvec[-1, :].detach().cpu().numpy().copy()
 
 
-        self.best_synthesis_acoustic = BestSynthesisAcoustic(np.Inf, initial_cp, initial_sig, initial_prod_mel, initial_pred_mel)  
+        self.best_synthesis_acoustic = BestSynthesisAcoustic(np.Inf, initial_cp, initial_sig, initial_prod_mel, initial_pred_mel)
         self.best_synthesis_semantic = BestSynthesisSemantic(np.Inf, initial_cp, initial_sig, initial_prod_semvec, initial_pred_semvec)
         if self.use_somatosensory_feedback:
             self.best_synthesis_somatosensory = BestSynthesisSomatosensory(np.Inf, np.Inf, np.Inf, initial_cp, initial_sig,
                                                                            initial_prod_tube,
                                                                            initial_pred_tube,
                                                                            initial_prod_tube_mel,
                                                                            initial_pred_tube_mel,
@@ -744,14 +898,16 @@
                 pred_tube_semvec_steps_ii = list()
                 prod_tube_semvec_steps_ii = list()
 
             for ii in range(n_inner):
                 optimizer.zero_grad()
 
                 pred_mel = self.pred_model(xx_new)
+                if self.use_speech_classifier:
+                    pred_speech_classifier = self.speech_classifier(pred_mel)
                 if self.use_somatosensory_feedback:
                     pred_tube = self.cp_tube_model(xx_new)
                     pred_tube.retain_grad()
                     pred_tube_mel = self.tube_mel_model(pred_tube)
 
                 if objective in ('semvec', 'acoustic_semvec'):
                     seq_length = pred_mel.shape[1]
@@ -761,128 +917,141 @@
 
                     if self.use_somatosensory_feedback:
                         tube_seq_length = pred_tube.shape[1]
                         self.tube_embedder = self.tube_embedder.train()
                         pred_tube_semvec = self.tube_embedder(pred_tube, (torch.tensor(tube_seq_length),))
                         pred_tube_semvec_steps_ii.append(pred_tube_semvec[-1, :].detach().cpu().numpy().copy())
 
-                # discrepancy,mel_loss, vel_loss, jerk_loss, pred_mel = constrained_criterion(tanh_straight_through(xx_new), target_mel)
                 if objective == 'acoustic':
-                    if self.use_somatosensory_feedback:
-                        discrepancy, mel_loss, vel_loss, jerk_loss, tube_mel_loss = criterion(pred_mel, target_mel, xx_new, pred_tube_mel)
+                    if self.use_speech_classifier:
+                        discrepancy, sub_loss = criterion(pred_mel, target_mel, xx_new, pred_speech_classifier)
+                    elif self.use_somatosensory_feedback:
+                        discrepancy, sub_loss = criterion(pred_mel, target_mel, xx_new, pred_tube_mel)
                     else:
-                        discrepancy, mel_loss, vel_loss, jerk_loss = criterion(pred_mel, target_mel, xx_new)
+                        discrepancy, sub_loss = criterion(pred_mel, target_mel, xx_new)
 
                     if (ii + 1) % log_ii == 0:
                         planned_loss_steps.append(float(discrepancy.item()))
-                        planned_mel_loss_steps.append(float(mel_loss.item()))
-                        vel_loss_steps.append(float(vel_loss.item()))
-                        jerk_loss_steps.append(float(jerk_loss.item()))
+                        planned_mel_loss_steps.append(float(sub_loss.mel_loss.item()))
+                        vel_loss_steps.append(float(sub_loss.velocity_loss.item()))
+                        jerk_loss_steps.append(float(sub_loss.jerk_loss.item()))
+                        if self.use_speech_classifier:
+                            pred_speech_classifier_loss_steps.append(float(sub_loss.speech_classifier_loss.item()))
                         if self.use_somatosensory_feedback:
-                            pred_tube_mel_loss_steps.append(float(tube_mel_loss.item()))
+                            pred_tube_mel_loss_steps.append(float(sub_loss.tube_mel_loss.item()))
 
                         if log_semantics:
                             seq_length = pred_mel.shape[1]
                             pred_semvec = self.embedder(pred_mel, (torch.tensor(seq_length),))
                             pred_semvec_steps_ii.append(pred_semvec[-1, :].detach().cpu().numpy().copy())
-                            semvec_loss = float(rmse_loss(pred_semvec, target_semvec).item())
+                            semvec_loss = SEMANTIC_WEIGHT * float(rmse_loss(pred_semvec, target_semvec).item())
                             pred_semvec_loss_steps.append(semvec_loss)
                             if self.use_somatosensory_feedback:
                                 tube_seq_length = pred_tube.shape[1]
                                 pred_tube_semvec = self.tube_embedder(pred_tube, (torch.tensor(tube_seq_length),))
                                 pred_tube_semvec_steps_ii.append(pred_tube_semvec[-1, :].detach().cpu().numpy().copy())
-                                tube_semvec_loss = 10*float(rmse_loss(pred_tube_semvec, target_semvec).item())
+                                tube_semvec_loss = TUBE_SEMANTIC_WEIGHT * float(rmse_loss(pred_tube_semvec, target_semvec).item())
                                 pred_tube_semvec_loss_steps.append(tube_semvec_loss)
 
                     if verbose:
                         print("Iteration %d" % ii)
                         print("Planned Loss: ", float(discrepancy.item()))
-                        print("Mel Loss: ", float(mel_loss.item()))
-                        print("Vel Loss: ", float(vel_loss.item()))
-                        print("Jerk Loss: ", float(jerk_loss.item()))
+                        print("Mel Loss: ", float(sub_loss.mel_loss.item()))
+                        print("Vel Loss: ", float(sub_loss.velocity_loss.item()))
+                        print("Jerk Loss: ", float(sub_loss.jerk_loss.item()))
+                        print("Local Linear Loss: ", float(sub_loss.local_linear_loss.item()))
+                        if self.use_speech_classifier:
+                            print("Speech Classifier Loss: ", float(sub_loss.speech_classifier_loss.item()))
                         if self.use_somatosensory_feedback:
-                            print("Tube Mel Loss: ", float(tube_mel_loss.item()))
+                            print("Tube Mel Loss: ", float(sub_loss.tube_mel_loss.item()))
                         if log_semantics:
                             print("Semvec Loss: ", float(semvec_loss))
                             if self.use_somatosensory_feedback:
                                 print("Tube Semvec Loss: ", float(tube_semvec_loss))
 
                 elif objective == 'acoustic_semvec':
-                    if self.use_somatosensory_feedback:
-                        discrepancy, mel_loss, vel_loss, jerk_loss, semvec_loss, tube_mel_loss, tube_semvec_loss = criterion(pred_mel, target_mel,
-                                                                                            pred_semvec, target_semvec,
-                                                                                            xx_new, pred_tube_mel, pred_tube_semvec)
+                    if self.use_speech_classifier:
+                        discrepancy, sub_loss = criterion(pred_mel, target_mel, pred_semvec, target_semvec, xx_new, pred_speech_classifier)
+                    elif self.use_somatosensory_feedback:
+                        discrepancy, sub_loss = criterion(pred_mel, target_mel, pred_semvec, target_semvec, xx_new, pred_tube_mel, pred_tube_semvec)
                     else:
-                        discrepancy, mel_loss, vel_loss, jerk_loss, semvec_loss = criterion(pred_mel, target_mel,
-                                                                                            pred_semvec, target_semvec,
-                                                                                            xx_new)
+                        discrepancy, sub_loss = criterion(pred_mel, target_mel, pred_semvec, target_semvec, xx_new)
                     if (ii + 1) % log_ii == 0:
                         planned_loss_steps.append(float(discrepancy.item()))
-                        planned_mel_loss_steps.append(float(mel_loss.item()))
-                        vel_loss_steps.append(float(vel_loss.item()))
-                        jerk_loss_steps.append(float(jerk_loss.item()))
-                        pred_semvec_loss_steps.append(float(semvec_loss.item()))
+                        planned_mel_loss_steps.append(float(sub_loss.mel_loss.item()))
+                        vel_loss_steps.append(float(sub_loss.velocity_loss.item()))
+                        jerk_loss_steps.append(float(sub_loss.jerk_loss.item()))
+                        pred_semvec_loss_steps.append(float(sub_loss.semvec_loss.item()))
+                        if self.use_speech_classifier:
+                            pred_speech_classifier_loss_steps.append(float(sub_loss.speech_classifier_loss.item()))
                         if self.use_somatosensory_feedback:
-                            pred_tube_mel_loss_steps.append(float(tube_mel_loss.item()))
-                            pred_tube_semvec_loss_steps.append(float(tube_semvec_loss.item()))
+                            pred_tube_mel_loss_steps.append(float(sub_loss.tube_mel_loss.item()))
+                            pred_tube_semvec_loss_steps.append(float(sub_loss.tube_semvec_loss.item()))
 
                     if verbose:
                         print("Iteration %d" % ii)
                         print("Planned Loss: ", float(discrepancy.item()))
-                        print("Mel Loss: ", float(mel_loss.item()))
-                        print("Vel Loss: ", float(vel_loss.item()))
-                        print("Jerk Loss: ", float(jerk_loss.item()))
-                        print("Semvec Loss: ", float(semvec_loss.item()))
+                        print("Mel Loss: ", float(sub_loss.mel_loss.item()))
+                        print("Vel Loss: ", float(sub_loss.velocity_loss.item()))
+                        print("Jerk Loss: ", float(sub_loss.jerk_loss.item()))
+                        print("Local Linear Loss: ", float(sub_loss.local_linear_loss.item()))
+                        print("Semvec Loss: ", float(sub_loss.semvec_loss.item()))
+                        if self.use_speech_classifier:
+                            print("Speech Classifier Loss: ", float(sub_loss.speech_classifier_loss.item()))
                         if self.use_somatosensory_feedback:
-                            print("Tube Mel Loss: ", float(tube_mel_loss.item()))
-                            print("Tube Semvec Loss: ", float(tube_semvec_loss.item()))
+                            print("Tube Mel Loss: ", float(sub_loss.tube_mel_loss.item()))
+                            print("Tube Semvec Loss: ", float(sub_loss.tube_semvec_loss.item()))
 
                 elif objective == 'semvec':
-                    if self.use_somatosensory_feedback:
-                        discrepancy, vel_loss, jerk_loss, semvec_loss, tube_semvec_loss = criterion(pred_semvec, target_semvec, xx_new, pred_tube_semvec)
-                        mel_loss = rmse_loss(pred_mel, target_mel)
-                        tube_mel_loss = rmse_loss(pred_tube_mel, target_mel)
+                    if self.use_speech_classifier:
+                        discrepancy, sub_loss = criterion(pred_semvec, target_semvec, xx_new, pred_speech_classifier)
+                    elif self.use_somatosensory_feedback:
+                        discrepancy, sub_loss = criterion(pred_semvec, target_semvec, xx_new, pred_tube_semvec)
+                        tube_mel_loss = TUBE_MEL_WEIGHT * rmse_loss(pred_tube_mel, target_mel)
                     else:
-                        discrepancy, vel_loss, jerk_loss, semvec_loss = criterion(pred_semvec, target_semvec, xx_new)
-                        mel_loss = rmse_loss(pred_mel, target_mel)
+                        discrepancy, sub_loss = criterion(pred_semvec, target_semvec, xx_new)
+                    mel_loss = MEL_WEIGHT * rmse_loss(pred_mel, target_mel)
 
                     if (ii + 1) % log_ii == 0:
                         planned_loss_steps.append(float(discrepancy.item()))
-                        vel_loss_steps.append(float(vel_loss.item()))
-                        jerk_loss_steps.append(float(jerk_loss.item()))
-                        pred_semvec_loss_steps.append(float(semvec_loss.item()))
+                        vel_loss_steps.append(float(sub_loss.velocity_loss.item()))
+                        jerk_loss_steps.append(float(sub_loss.jerk_loss.item()))
+                        pred_semvec_loss_steps.append(float(sub_loss.semvec_loss.item()))
                         planned_mel_loss_steps.append(float(mel_loss.item()))
 
+                        if self.use_speech_classifier:
+                            pred_speech_classifier_loss_steps.append(float(sub_loss.speech_classifier_loss.item()))
                         if self.use_somatosensory_feedback:
-                            pred_tube_semvec_loss_steps.append(float(tube_semvec_loss.item()))
+                            pred_tube_semvec_loss_steps.append(float(sub_loss.tube_semvec_loss.item()))
                             pred_tube_mel_loss_steps.append(float(tube_mel_loss.item()))
 
                     if verbose:
                         print("Iteration %d" % ii)
                         print("Planned Loss: ", float(discrepancy.item()))
                         print("Mel Loss: ", float(mel_loss.item()))
-                        print("Vel Loss: ", float(vel_loss.item()))
-                        print("Jerk Loss: ", float(jerk_loss.item()))
-                        print("Semvec Loss: ", float(semvec_loss.item()))
+                        print("Vel Loss: ", float(sub_loss.velocity_loss.item()))
+                        print("Jerk Loss: ", float(sub_loss.jerk_loss.item()))
+                        print("Semvec Loss: ", float(sub_loss.semvec_loss.item()))
+                        if self.use_speech_classifier:
+                            print("Speech Classifier Loss: ", float(sub_loss.speech_classifier_loss.item()))
                         if self.use_somatosensory_feedback:
                             print("Tube Mel Loss: ", float(tube_mel_loss.item()))
-                            print("Tube Semvec Loss: ", float(tube_semvec_loss.item()))
+                            print("Tube Semvec Loss: ", float(sub_loss.tube_semvec_loss.item()))
 
                 else:
                     raise ValueError(f'unkown objective {objective}')
 
                 discrepancy.backward()
 
                 # if verbose:
                 # print(f"grad.abs().max() {grad.abs().max()}")
-                if xx_new.grad.max() > 10:
-                    if verbose:
+                if verbose:
+                    if xx_new.grad.max() > 10:
                         print("WARNING: gradient is larger than 10")
-                if xx_new.grad.min() < -10:
-                    if verbose:
+                    if xx_new.grad.min() < -10:
                         print("WARNING: gradient is smaller than -10")
 
                 if log_gradients:
                     grad_steps.append(xx_new.grad.detach().clone())
 
                 if (ii + 1) % log_ii == 0:
                     xx_new_numpy = xx_new[-1, :, :].detach().cpu().numpy().copy()
@@ -906,15 +1075,15 @@
                             prod_tube_mel = self.tube_mel_model(prod_tube)
 
                         pred_tube_steps_ii.append(pred_tube[-1, :, :].detach().cpu().numpy().copy())
 
                         prod_tube_loss = rmse_loss(pred_tube, prod_tube)
                         prod_tube_loss_steps.append(float(prod_tube_loss.item()))
 
-                        prod_tube_mel_loss = rmse_loss(prod_tube_mel, target_mel)
+                        prod_tube_mel_loss = TUBE_MEL_WEIGHT * rmse_loss(prod_tube_mel, target_mel)
                         prod_tube_mel_loss_steps.append(float(prod_tube_mel_loss.item()))
 
                         pred_tube_mel_steps_ii.append(pred_tube_mel[-1, :, :].detach().cpu().numpy().copy())
                         prod_tube_mel_steps_ii.append(prod_tube_mel[-1, :, :].detach().cpu().numpy().copy())
 
 
                     else:
@@ -929,35 +1098,50 @@
 
                     prod_mel.shape = pred_mel.shape
                     prod_mel = torch.from_numpy(prod_mel)
                     prod_mel = prod_mel.to(self.device)
                     pred_mel_steps_ii.append(pred_mel[-1, :, :].detach().cpu().numpy().copy())
 
                     prod_loss = rmse_loss(prod_mel, target_mel)
+                    prod_loss *= MEL_WEIGHT
                     prod_loss_steps.append(float(prod_loss.item()))
 
+                    if self.use_speech_classifier:
+                        prod_speech_classifier = self.speech_classifier(prod_mel)
+                        prod_speech_classifier_loss = bce_loss(
+                                prod_speech_classifier,
+                                torch.zeros_like(prod_speech_classifier, dtype=prod_speech_classifier.dtype))
+                        prod_speech_classifier_loss *= SPEECH_CLASSIFIER_WEIGHT
+
+                        prod_speech_classifier_loss_steps.append(float(
+                            prod_speech_classifier_loss.item()))
+
                     if verbose:
                         print("Produced Mel Loss: ", float(prod_loss.item()))
+                        if self.use_speech_classifier:
+                            print("Produced Speech Classifier Loss: ", float(prod_speech_classifier_loss.item()))
                         if self.use_somatosensory_feedback:
                             print("Produced Tube Loss: ", float(prod_tube_loss.item()))
 
                     if objective in ('semvec', 'acoustic_semvec') or log_semantics:
                         self.embedder = self.embedder.eval()
                         prod_semvec = self.embedder(prod_mel, (torch.tensor(prod_mel.shape[1]),))
                         prod_semvec_steps_ii.append(prod_semvec[-1, :].detach().cpu().numpy().copy())
 
-                        prod_semvec_loss = 10*rmse_loss(prod_semvec, target_semvec)
+                        prod_semvec_loss = rmse_loss(prod_semvec, target_semvec)
+                        prod_semvec_loss *= SEMANTIC_WEIGHT
                         prod_semvec_loss_steps.append(float(prod_semvec_loss.item()))
 
                         if self.use_somatosensory_feedback:
                             self.tube_embedder = self.tube_embedder.eval()
                             prod_tube_semvec = self.tube_embedder(prod_tube, (torch.tensor(prod_tube.shape[1]),))
                             prod_tube_semvec_steps_ii.append(prod_tube_semvec[-1, :].detach().cpu().numpy().copy())
 
-                            prod_tube_semvec_loss = 10*rmse_loss(prod_tube_semvec, target_semvec)
+                            prod_tube_semvec_loss = rmse_loss(prod_tube_semvec, target_semvec)
+                            prod_tube_semvec_loss *= TUBE_SEMANTIC_WEIGHT
                             prod_tube_semvec_loss_steps.append(float(prod_tube_semvec_loss.item()))
 
                         if verbose:
                             print("Produced Semvec Loss: ", float(prod_semvec_loss.item()))
                             if self.use_somatosensory_feedback:
                                 print("Produced Tube Semvec Loss: ", float(prod_tube_semvec_loss.item()))
                             print("")
@@ -995,15 +1179,15 @@
                                                                                            pred_tube[-1, :].detach().cpu().numpy().copy(),
                                                                                            prod_tube_mel[-1, :].detach().cpu().numpy().copy(),
                                                                                            pred_tube_mel[-1, :].detach().cpu().numpy().copy(),
                                                                                            None,
                                                                                            None)
                             if self.best_synthesis_somatosensory.tube_loss > new_synthesis_somatosensory.tube_loss:
                                 self.best_synthesis_somatosensory = new_synthesis_somatosensory
-                        
+
                     if verbose:
                         print("")
 
                 optimizer.step()
 
                 with torch.no_grad():
                     xx_new.data = xx_new.data.clamp(-1.05, 1.05) # clamp between -1.05 and 1.05
@@ -1325,16 +1509,23 @@
         # 27. prod_semvec_steps
         # 28. grad_steps
         # 29. sig_steps
         # 30. prod_mel_steps
         # 31. pred_mel_steps
         # 32. pred_model_loss
         # 33. inv_model_loss
-
-        if self.use_somatosensory_feedback:
+        if self.use_speech_classifier:
+            return PlanningResultsWithSpeechClassifier(planned_cp, initial_cp, initial_sig, initial_sr, initial_prod_mel, initial_pred_mel,
+                    target_sig, target_sr, target_mel, prod_sig, prod_sr, prod_mel,
+                    pred_mel, initial_prod_semvec, initial_pred_semvec, prod_semvec, pred_semvec, prod_loss_steps, planned_loss_steps,
+                    planned_mel_loss_steps, vel_loss_steps, jerk_loss_steps,
+                    pred_semvec_loss_steps, prod_semvec_loss_steps, pred_speech_classifier_loss_steps, prod_speech_classifier_loss_steps,
+                    cp_steps, pred_semvec_steps, prod_semvec_steps, grad_steps, sig_steps,
+                    prod_mel_steps, pred_mel_steps, pred_model_loss, inv_model_loss)
+        elif self.use_somatosensory_feedback:
             return PlanningResultsWithSomatosensory(planned_cp, initial_cp, initial_sig, initial_sr, initial_prod_mel, initial_pred_mel, initial_prod_tube, initial_pred_tube, initial_prod_tube_mel, initial_pred_tube_mel,
                                    target_sig, target_sr, target_mel, prod_sig, prod_sr, prod_mel,
                                    pred_mel, prod_tube, pred_tube, prod_tube_mel, pred_tube_mel, initial_prod_semvec, initial_pred_semvec, initial_prod_tube_semvec, initial_pred_tube_semvec, prod_semvec, pred_semvec, prod_tube_semvec, pred_tube_semvec,
                                    prod_loss_steps, planned_loss_steps,
                                    planned_mel_loss_steps, vel_loss_steps, jerk_loss_steps,
                                    pred_semvec_loss_steps, prod_semvec_loss_steps, prod_tube_loss_steps, pred_tube_mel_loss_steps, prod_tube_mel_loss_steps, pred_tube_semvec_loss_steps, prod_tube_semvec_loss_steps, cp_steps,
                                    pred_semvec_steps, prod_semvec_steps, grad_steps, sig_steps,
```

### Comparing `paule-0.3.6/paule/util.py` & `paule-0.4.4/paule/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import ctypes
 import io
 import os
 import shutil
 import sys
 import tempfile
+import warnings
 import zipfile
 
 import numpy as np
 import matplotlib.pyplot as plt
 import librosa
 import torch.nn
 import pandas as pd
@@ -42,14 +43,15 @@
 
 # This should be done on all cp_deltas
 #np.max(np.stack((np.abs(np.min(delta, axis=0)), np.max(delta, axis=0))), axis=0)
 #np.max(np.stack((np.abs(np.min(cp_param, axis=0)), np.max(cp_param, axis=0))), axis=0)
 
 # absolute value from max / min
 
+#Vocal tract parameters: " 0  1  2  3  4  5  6  7   8   9  10  11  12  13  14  15  16  17  18"
 #Vocal tract parameters: "HX HY JX JA LP LD VS VO TCX TCY TTX TTY TBX TBY TRX TRY TS1 TS2 TS3"
 #Glottis parameters: "f0 pressure x_bottom x_top chink_area lag rel_amp double_pulsing pulse_skewness flutter aspiration_strength "
 
 
 cp_means = np.array([ 5.3000e-01, -5.0800e+00, -3.0000e-02, -3.7300e+00,  7.0000e-02,
                       7.3000e-01,  4.8000e-01, -5.0000e-02,  9.6000e-01, -1.5800e+00,
                       4.4600e+00, -9.3000e-01,  2.9900e+00, -5.0000e-02, -1.4600e+00,
@@ -567,32 +569,75 @@
 
     def forward(self, yhat, y):
         loss = torch.sqrt(self.mse(yhat, y) + self.eps)
         return loss
 
 rmse_loss = RMSELoss(eps=0)
 
-def get_vel_acc_jerk(trajectory, *, lag=1):
+
+def calculate_five_point_stencil_without_padding(trajectory, *, delta_t=1.0):
+    """
+    Caculates the five-point stencil as a numeric approximation of the first derivative.
+
+    https://en.wikipedia.org/wiki/Five-point_stencil
+
+    Parameters
+    ==========
+    trajectory : np.array
+
+    Returns
+    =======
+    derivative : np.array
+
+    Equation
+    ========
+
+    .. math::
+
+        f'(x) \approx {\frac {-f(x+2h)+8f(x+h)-8f(x-h)+f(x-2h)}{12h}}}
+
+    """
+    xx = trajectory
+    return (-xx[:, 4:, :] + 8.0 * xx[:, 3:-1, :] - 8.0 * xx[:, 1:-3, :] + xx[:, :-4, :]) / (12.0 * delta_t)
+
+
+def numeric_derivative(xx, *, delta_t=1.0):
+    xx_prime = calculate_five_point_stencil_without_padding(xx, delta_t=delta_t)
+    return xx_prime
+
+
+def local_linear(trajectory, *, delta_t=1.0):
+    """
+    A locally linear trajectory will return a torch.tensor of zeros.
+
+    """
+    tt = trajectory
+    return (2 * tt[:, 1:-1, :] - tt[:, :-2, :] - tt[:, 2:, :]) / (2 * delta_t)
+
+
+def get_vel_acc_jerk(trajectory, *, lag=None, delta_t=1.0):
     """
     Approximates the velocity, acceleration, jerk for the given trajectory for a given lag
 
     Parameters
     ==========
     trajectory : np.array
-    lag : int
+    lag : int (deprecated; ignored)
 
     Returns
     =======
     (velocity, acceleration, jerk) : np.array, np.array, np.array
         returns the approximated velocity, acceleration and jerk of the trajectory for a given lag
-    """
 
-    velocity = (trajectory[:, lag:, :] - trajectory[:, :-lag, :]) / lag
-    acc = (velocity[:, 1:, :] - velocity[:, :-1, :]) / 1.0
-    jerk = (acc[:, 1:, :] - acc[:, :-1, :]) / 1.0
+    """
+    if lag is not None:
+        warnings.warn("lag should not used anymore and is ignored", DeprecationWarning, stacklevel=2)
+    velocity = numeric_derivative(trajectory, delta_t=delta_t)
+    acc = numeric_derivative(velocity, delta_t=delta_t)
+    jerk = numeric_derivative(acc, delta_t=delta_t)
     return velocity, acc, jerk
 
 
 def cp_trajectory_loss(Y_hat, tgts):
     """
     Calculates an additive loss using the RMSE between predicted and target position, velocity, acc and jerk
```

### Comparing `paule-0.3.6/paule/visualize.py` & `paule-0.4.4/paule/visualize.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 import os
 
 import soundfile as sf
 from matplotlib import pyplot as plt
 import librosa.display
 from matplotlib import cm
+import numpy as np
 
 from . import util
 
 
 def visualize_results(results, condition='prefix', folder='data'):
     """
     Stores all results in data/ folder.
@@ -24,15 +25,16 @@
     plot_mels(f"{base_name}_mel.png", results.target_mel, results.initial_pred_mel,
             results.initial_prod_mel, results.pred_mel, results.prod_mel)
 
     # save audio
     target_sr = prod_sr = 44100
     sf.write(f'{base_name}_planned.flac', results.prod_sig, results.prod_sr)
     sf.write(f'{base_name}_initial.flac', results.initial_sig, results.initial_sr)
-    sf.write(f'{base_name}_target.flac', results.target_sig, results.target_sr)
+    if results.target_sig is not None:
+        sf.write(f'{base_name}_target.flac', results.target_sig, results.target_sr)
 
     # save loss plot
     fig, ax = plt.subplots(figsize=(15, 8), facecolor="white")
     ax.plot(results.planned_loss_steps, label="planned loss", c="C0")
     ax.legend()
     fig.tight_layout()
     fig.savefig(f"{base_name}_loss.png")
@@ -56,29 +58,62 @@
     fig, ax = plt.subplots(figsize=(15, 8), facecolor="white")
     ax.plot(results.pred_semvec_loss_steps, label="planned semvec loss", c="C0")
     ax.plot(results.prod_semvec_loss_steps, label="produced semvec loss", c="C1")
     ax.legend()
     fig.tight_layout()
     fig.savefig(f"{base_name}_loss_semvec.png")
 
+    # save speech classifier loss plot
+    if hasattr(results, 'pred_speech_classifier_loss_steps'):
+        fig, ax = plt.subplots(figsize=(15, 8), facecolor="white")
+        ax.plot(results.pred_speech_classifier_loss_steps, label="planned speech classifier loss", c="C0")
+        ax.plot(np.array(results.prod_speech_classifier_loss_steps) / 10.0, label="produced speech classifier loss", c="C1")
+        ax.legend()
+        fig.tight_layout()
+        fig.savefig(f"{base_name}_loss_speech_classifier.png")
+
     # save cp change plot
     fig = plt.figure(figsize=(15, 12))
     ax1 = fig.add_axes([0.1, 0.68, 0.88, 0.30], xticklabels=[])
     ax2 = fig.add_axes([0.1, 0.36, 0.88, 0.30], xticklabels=[], sharex=ax1)
     ax3 = fig.add_axes([0.1, 0.04, 0.88, 0.30], xticklabels=[], sharex=ax1)
     img1 = results.initial_cp  #target['cp'].iloc[0]
     img2 = results.planned_cp
     img3 = img2 - img1
-    ax1.plot(img1[:, 8:16])  # , label='tongue'
+    ax1.plot(img1[:,  3: 4], label='JA')
+    ax1.plot(img1[:,  8: 9], label='TCX')
+    ax1.plot(img1[:,  9:10], label='TCY')
+    ax1.plot(img1[:, 10:11], label='TTX')
+    ax1.plot(img1[:, 11:12], label='TTY')
+    ax1.plot(img1[:, 12:13], label='TBX')
+    ax1.plot(img1[:, 13:14], label='TBY')
+    ax1.plot(img1[:, 14:15], label='TRX')
+    ax1.plot(img1[:, 15:16], label='TRY')
     ax1.plot(img1[:, 19:20], label='f0')
     ax1.set_ylabel("initial")
-    ax2.plot(img2[:, 8:16], label='tongue')
+    ax2.plot(img2[:,  3: 4], label='JA')
+    ax2.plot(img2[:,  8: 9], label='TCX')
+    ax2.plot(img2[:,  9:10], label='TCY')
+    ax2.plot(img2[:, 10:11], label='TTX')
+    ax2.plot(img2[:, 11:12], label='TTY')
+    ax2.plot(img2[:, 12:13], label='TBX')
+    ax2.plot(img2[:, 13:14], label='TBY')
+    ax2.plot(img2[:, 14:15], label='TRX')
+    ax2.plot(img2[:, 15:16], label='TRY')
     ax2.plot(img2[:, 19:20], label='f0')
     ax2.set_ylabel("optimized")
-    ax3.plot(img3[:, 8:16], label='tongue')
+    ax3.plot(img3[:,  3: 4], label='JA')
+    ax3.plot(img3[:,  8: 9], label='TCX')
+    ax3.plot(img3[:,  9:10], label='TCY')
+    ax3.plot(img3[:, 10:11], label='TTX')
+    ax3.plot(img3[:, 11:12], label='TTY')
+    ax3.plot(img3[:, 12:13], label='TBX')
+    ax3.plot(img3[:, 13:14], label='TBY')
+    ax3.plot(img3[:, 14:15], label='TRX')
+    ax3.plot(img3[:, 15:16], label='TRY')
     ax3.plot(img3[:, 19:20], label='f0')
     ax3.set_ylabel("difference")
     ax1.legend()
     fig.tight_layout()
     fig.savefig(f'{base_name}_cps.png')
 
     # save svgs and create mp4s
@@ -106,15 +141,15 @@
         print("WARNING: creating the planning animation went wrong")
     ## recode to 60 Hz
     #system_call = f'cd {path}; /usr/bin/ffmpeg -loglevel error -i ../{condition}_planned_80Hz.mp4 -r 60 ../{condition}_planned_60Hz.mp4'
     #return_value = os.system(system_call)
     #if return_value != 0:
     #    print("WARNING: creating the planned animation went wrong")
 
-    plt.show()  # this shows all saved figures
+    #plt.show()  # this shows all saved figures
 
 
 def plot_mels(file_name, target_mel, initial_pred_mel, initial_prod_mel,
         pred_mel, prod_mel):
     """
     Plots target, initial prediction, initial production, prediction and
     production log mel spectrograms.
```

### Comparing `paule-0.3.6/paule/vocaltractlab_api/JD3.speaker` & `paule-0.4.4/paule/vocaltractlab_api/JD3.speaker`

 * *Files identical despite different names*

### Comparing `paule-0.3.6/paule/vocaltractlab_api/VocalTractLabApi.dll` & `paule-0.4.4/paule/vocaltractlab_api/VocalTractLabApi.dll`

 * *Files identical despite different names*

### Comparing `paule-0.3.6/paule/vocaltractlab_api/libVocalTractLabApi.dylib` & `paule-0.4.4/paule/vocaltractlab_api/libVocalTractLabApi.dylib`

 * *Files identical despite different names*

### Comparing `paule-0.3.6/paule/vocaltractlab_api/libVocalTractLabApi.so` & `paule-0.4.4/paule/vocaltractlab_api/libVocalTractLabApi.so`

 * *Files identical despite different names*

### Comparing `paule-0.3.6/pyproject.toml` & `paule-0.4.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "paule"
-version = "0.3.6"
+version = "0.4.4"
 description = "paule implements the Predictive Articulatory speech synthesis model Utilizing Lexical Embeddings (PAULE), which is a control model for the articulatory speech synthesizer VocalTractLab (VTL)."
 
 license = "GPLv3+"
 
 authors = ["Konstantin Sering <konstantin.sering@uni-tuebingen.de>",
            "Paul Schmidt-Barbo"
            ]
@@ -21,15 +21,15 @@
                'Operating System :: MacOS',
                'Operating System :: Microsoft :: Windows',
                'Topic :: Scientific/Engineering',
                'Topic :: Scientific/Engineering :: Artificial Intelligence',
                'Topic :: Scientific/Engineering :: Information Analysis',]
 
 [tool.poetry.dependencies]
-python = ">=3.9,<3.12"  # Compatible python versions must be declared here
+python = ">=3.9,<3.13"  # Compatible python versions must be declared here
 numpy = ">=1.23.1"
 pandas = ">=1.4.3"
 soundfile = ">=0.11.0"
 tqdm = ">=4.64.1"
 torch = ">=1.13.1"
 llvmlite = ">=0.39.1"
 librosa = ">=0.9.2"
@@ -47,15 +47,15 @@
 notebook = ">=6.4.10"
 seaborn = ">=0.12.1"
 numpydoc = ">=1.2"
 sphinx-copybutton = ">=0.5.1"
 pylint = ">=2.0.0"
 nbsphinx = ">=0.8.8"
 vulture = ">=2.3"
-Jinja2 = "<3.1.0"
+Jinja2 = ">=3.1.3"
 
 [tool.pytest.ini_options]
 addopts = '--doctest-glob "*.rst"'
 
 [tool.pylint]
   [tool.pylint.basic]
   good-names = ["nn", "ii", "_", "jj", "df"]
```

### Comparing `paule-0.3.6/PKG-INFO` & `paule-0.4.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: paule
-Version: 0.3.6
+Version: 0.4.4
 Summary: paule implements the Predictive Articulatory speech synthesis model Utilizing Lexical Embeddings (PAULE), which is a control model for the articulatory speech synthesizer VocalTractLab (VTL).
 Home-page: https://paule.readthedocs.io/en/latest/
 License: GPLv3+
 Author: Konstantin Sering
 Author-email: konstantin.sering@uni-tuebingen.de
-Requires-Python: >=3.9,<3.12
+Requires-Python: >=3.9,<3.13
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Requires-Dist: librosa (>=0.9.2)
 Requires-Dist: llvmlite (>=0.39.1)
 Requires-Dist: matplotlib (>=3.8.0)
 Requires-Dist: numba (>=0.56.4)
```

