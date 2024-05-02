# Comparing `tmp/dillwave-1.0.1-py3-none-any.whl.zip` & `tmp/dillwave-1.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 17998 bytes, number of entries: 13
--rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-26 22:34 dillwave/__init__.py
--rw-rw-rw-  2.0 fat     2155 b- defN 24-Mar-26 22:34 dillwave/__main__.py
--rw-rw-rw-  2.0 fat     5919 b- defN 24-Mar-26 22:34 dillwave/dataset.py
--rw-rw-rw-  2.0 fat     4428 b- defN 24-Mar-26 22:34 dillwave/inference.py
--rw-rw-rw-  2.0 fat     7125 b- defN 24-Mar-26 22:34 dillwave/learner.py
--rw-rw-rw-  2.0 fat     5656 b- defN 24-Mar-26 22:34 dillwave/model.py
--rw-rw-rw-  2.0 fat     1778 b- defN 24-Mar-26 22:34 dillwave/params.py
--rw-rw-rw-  2.0 fat     2229 b- defN 24-Mar-26 22:34 dillwave/preprocess.py
--rw-rw-rw-  2.0 fat    11556 b- defN 24-Mar-26 22:39 dillwave-1.0.1.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     2652 b- defN 24-Mar-26 22:39 dillwave-1.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Mar-26 22:39 dillwave-1.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 24-Mar-26 22:39 dillwave-1.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1004 b- defN 24-Mar-26 22:39 dillwave-1.0.1.dist-info/RECORD
-13 files, 44603 bytes uncompressed, 16340 bytes compressed:  63.4%
+Zip file size: 18106 bytes, number of entries: 13
+-rw-r--r--  2.0 unx        0 b- defN 24-May-02 15:51 dillwave/__init__.py
+-rw-r--r--  2.0 unx     2103 b- defN 24-May-02 15:51 dillwave/__main__.py
+-rw-r--r--  2.0 unx     5753 b- defN 24-May-02 15:51 dillwave/dataset.py
+-rw-r--r--  2.0 unx     4317 b- defN 24-May-02 15:51 dillwave/inference.py
+-rw-r--r--  2.0 unx     7795 b- defN 24-May-02 15:51 dillwave/learner.py
+-rw-r--r--  2.0 unx     5495 b- defN 24-May-02 15:51 dillwave/model.py
+-rw-r--r--  2.0 unx     1720 b- defN 24-May-02 15:51 dillwave/params.py
+-rw-r--r--  2.0 unx     2164 b- defN 24-May-02 15:51 dillwave/preprocess.py
+-rw-r--r--  2.0 unx    11356 b- defN 24-May-02 15:52 dillwave-1.0.2.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     2613 b- defN 24-May-02 15:52 dillwave-1.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-02 15:52 dillwave-1.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 24-May-02 15:52 dillwave-1.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1004 b- defN 24-May-02 15:52 dillwave-1.0.2.dist-info/RECORD
+13 files, 44421 bytes uncompressed, 16448 bytes compressed:  63.0%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: dillwave/params.py
 Comment: 
 
 Filename: dillwave/preprocess.py
 Comment: 
 
-Filename: dillwave-1.0.1.dist-info/LICENSE.txt
+Filename: dillwave-1.0.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: dillwave-1.0.1.dist-info/METADATA
+Filename: dillwave-1.0.2.dist-info/METADATA
 Comment: 
 
-Filename: dillwave-1.0.1.dist-info/WHEEL
+Filename: dillwave-1.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: dillwave-1.0.1.dist-info/top_level.txt
+Filename: dillwave-1.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: dillwave-1.0.1.dist-info/RECORD
+Filename: dillwave-1.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dillwave/__main__.py

 * *Ordering differences only*

```diff
@@ -1,52 +1,52 @@
-# Copyright 2020 LMNT, Inc. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-# ==============================================================================
-
-from argparse import ArgumentParser
-from torch.cuda import device_count
-from torch.multiprocessing import spawn
-
-from dillwave.learner import train, train_distributed
-from dillwave.params import params
-
-
-def _get_free_port():
-  import socketserver
-  with socketserver.TCPServer(('localhost', 0), None) as s:
-    return s.server_address[1]
-
-
-def main(args):
-  replica_count = device_count()
-  if replica_count > 1:
-    if params.batch_size % replica_count != 0:
-      raise ValueError(f'Batch size {params.batch_size} is not evenly divisble by # GPUs {replica_count}.')
-    params.batch_size = params.batch_size // replica_count
-    port = _get_free_port()
-    spawn(train_distributed, args=(replica_count, port, args, params), nprocs=replica_count, join=True)
-  else:
-    train(args, params)
-
-
-if __name__ == '__main__':
-  parser = ArgumentParser(description='train (or resume training) a DillWave model')
-  parser.add_argument('model_dir',
-      help='directory in which to store model checkpoints and training logs')
-  parser.add_argument('data_dirs', nargs='+',
-      help='space separated list of directories from which to read .wav files for training')
-  parser.add_argument('--max_steps', default=None, type=int,
-      help='maximum number of training steps')
-  parser.add_argument('--fp16', action='store_true', default=False,
-      help='use 16-bit floating point operations for training')
-  main(parser.parse_args())
+# Copyright 2020 LMNT, Inc. All Rights Reserved.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+# ==============================================================================
+
+from argparse import ArgumentParser
+from torch.cuda import device_count
+from torch.multiprocessing import spawn
+
+from dillwave.learner import train, train_distributed
+from dillwave.params import params
+
+
+def _get_free_port():
+  import socketserver
+  with socketserver.TCPServer(('localhost', 0), None) as s:
+    return s.server_address[1]
+
+
+def main(args):
+  replica_count = device_count()
+  if replica_count > 1:
+    if params.batch_size % replica_count != 0:
+      raise ValueError(f'Batch size {params.batch_size} is not evenly divisble by # GPUs {replica_count}.')
+    params.batch_size = params.batch_size // replica_count
+    port = _get_free_port()
+    spawn(train_distributed, args=(replica_count, port, args, params), nprocs=replica_count, join=True)
+  else:
+    train(args, params)
+
+
+if __name__ == '__main__':
+  parser = ArgumentParser(description='train (or resume training) a DillWave model')
+  parser.add_argument('model_dir',
+      help='directory in which to store model checkpoints and training logs')
+  parser.add_argument('data_dirs', nargs='+',
+      help='space separated list of directories from which to read .wav files for training')
+  parser.add_argument('--max_steps', default=None, type=int,
+      help='maximum number of training steps')
+  parser.add_argument('--fp16', action='store_true', default=False,
+      help='use 16-bit floating point operations for training')
+  main(parser.parse_args())
```

## dillwave/dataset.py

 * *Ordering differences only*

```diff
@@ -1,166 +1,166 @@
-# Copyright 2020 LMNT, Inc. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-# ==============================================================================
-
-import numpy as np
-import os
-import random
-import torch
-import torch.nn.functional as F
-import torchaudio
-
-from glob import glob
-from torch.utils.data.distributed import DistributedSampler
-
-
-class ConditionalDataset(torch.utils.data.Dataset):
-  def __init__(self, paths):
-    super().__init__()
-    self.filenames = []
-    for path in paths:
-      self.filenames += glob(f'{path}/**/*.wav', recursive=True)
-
-  def __len__(self):
-    return len(self.filenames)
-
-  def __getitem__(self, idx):
-    audio_filename = self.filenames[idx]
-    spec_filename = f'{audio_filename}.spec.npy'
-    signal, _ = torchaudio.load(audio_filename)
-    spectrogram = np.load(spec_filename)
-    return {
-        'audio': signal[0],
-        'spectrogram': spectrogram.T
-    }
-
-
-class UnconditionalDataset(torch.utils.data.Dataset):
-  def __init__(self, paths):
-    super().__init__()
-    self.filenames = []
-    for path in paths:
-      self.filenames += glob(f'{path}/**/*.wav', recursive=True)
-
-  def __len__(self):
-    return len(self.filenames)
-
-  def __getitem__(self, idx):
-    audio_filename = self.filenames[idx]
-    spec_filename = f'{audio_filename}.spec.npy'
-    signal, _ = torchaudio.load(audio_filename)
-    return {
-        'audio': signal[0],
-        'spectrogram': None
-    }
-
-
-class Collator:
-  def __init__(self, params):
-    self.params = params
-
-  def collate(self, minibatch):
-    samples_per_frame = self.params.hop_samples
-    for record in minibatch:
-      if self.params.unconditional:
-          # Filter out records that aren't long enough.
-          if len(record['audio']) < self.params.audio_len:
-            del record['spectrogram']
-            del record['audio']
-            continue
-
-          start = random.randint(0, record['audio'].shape[-1] - self.params.audio_len)
-          end = start + self.params.audio_len
-          record['audio'] = record['audio'][start:end]
-          record['audio'] = np.pad(record['audio'], (0, (end - start) - len(record['audio'])), mode='constant')
-      else:
-          # Filter out records that aren't long enough.
-          if len(record['spectrogram']) < self.params.crop_mel_frames:
-            del record['spectrogram']
-            del record['audio']
-            continue
-
-          start = random.randint(0, record['spectrogram'].shape[0] - self.params.crop_mel_frames)
-          end = start + self.params.crop_mel_frames
-          record['spectrogram'] = record['spectrogram'][start:end].T
-
-          start *= samples_per_frame
-          end *= samples_per_frame
-          record['audio'] = record['audio'][start:end]
-          record['audio'] = np.pad(record['audio'], (0, (end-start) - len(record['audio'])), mode='constant')
-
-    audio = np.stack([record['audio'] for record in minibatch if 'audio' in record])
-    if self.params.unconditional:
-        return {
-            'audio': torch.from_numpy(audio),
-            'spectrogram': None,
-        }
-    spectrogram = np.stack([record['spectrogram'] for record in minibatch if 'spectrogram' in record])
-    return {
-        'audio': torch.from_numpy(audio),
-        'spectrogram': torch.from_numpy(spectrogram),
-    }
-
-  # for gtzan
-  def collate_gtzan(self, minibatch):
-    ldata = []
-    mean_audio_len = self.params.audio_len # change to fit in gpu memory
-    # audio total generated time = audio_len * sample_rate
-    # GTZAN statistics
-    # max len audio 675808; min len audio sample 660000; mean len audio sample 662117
-    # max audio sample 1; min audio sample -1; mean audio sample -0.0010 (normalized)
-    # sample rate of all is 22050
-    for data in minibatch:
-      if data[0].shape[-1] < mean_audio_len:  # pad
-        data_audio = F.pad(data[0], (0, mean_audio_len - data[0].shape[-1]), mode='constant', value=0)
-      elif data[0].shape[-1] > mean_audio_len:  # crop
-        start = random.randint(0, data[0].shape[-1] - mean_audio_len)
-        end = start + mean_audio_len
-        data_audio = data[0][:, start:end]
-      else:
-        data_audio = data[0]
-      ldata.append(data_audio)
-    audio = torch.cat(ldata, dim=0)
-    return {
-          'audio': audio,
-          'spectrogram': None,
-    }
-
-
-def from_path(data_dirs, params, is_distributed=False):
-  if params.unconditional:
-    dataset = UnconditionalDataset(data_dirs)
-  else:#with condition
-    dataset = ConditionalDataset(data_dirs)
-  return torch.utils.data.DataLoader(
-      dataset,
-      batch_size=params.batch_size,
-      collate_fn=Collator(params).collate,
-      shuffle=not is_distributed,
-      num_workers=os.cpu_count(),
-      sampler=DistributedSampler(dataset) if is_distributed else None,
-      pin_memory=True,
-      drop_last=True)
-
-
-def from_gtzan(params, is_distributed=False):
-  dataset = torchaudio.datasets.GTZAN('./data', download=True)
-  return torch.utils.data.DataLoader(
-      dataset,
-      batch_size=params.batch_size,
-      collate_fn=Collator(params).collate_gtzan,
-      shuffle=not is_distributed,
-      num_workers=os.cpu_count(),
-      sampler=DistributedSampler(dataset) if is_distributed else None,
-      pin_memory=True,
-      drop_last=True)
+# Copyright 2020 LMNT, Inc. All Rights Reserved.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+# ==============================================================================
+
+import numpy as np
+import os
+import random
+import torch
+import torch.nn.functional as F
+import torchaudio
+
+from glob import glob
+from torch.utils.data.distributed import DistributedSampler
+
+
+class ConditionalDataset(torch.utils.data.Dataset):
+  def __init__(self, paths):
+    super().__init__()
+    self.filenames = []
+    for path in paths:
+      self.filenames += glob(f'{path}/**/*.wav', recursive=True)
+
+  def __len__(self):
+    return len(self.filenames)
+
+  def __getitem__(self, idx):
+    audio_filename = self.filenames[idx]
+    spec_filename = f'{audio_filename}.spec.npy'
+    signal, _ = torchaudio.load(audio_filename)
+    spectrogram = np.load(spec_filename)
+    return {
+        'audio': signal[0],
+        'spectrogram': spectrogram.T
+    }
+
+
+class UnconditionalDataset(torch.utils.data.Dataset):
+  def __init__(self, paths):
+    super().__init__()
+    self.filenames = []
+    for path in paths:
+      self.filenames += glob(f'{path}/**/*.wav', recursive=True)
+
+  def __len__(self):
+    return len(self.filenames)
+
+  def __getitem__(self, idx):
+    audio_filename = self.filenames[idx]
+    spec_filename = f'{audio_filename}.spec.npy'
+    signal, _ = torchaudio.load(audio_filename)
+    return {
+        'audio': signal[0],
+        'spectrogram': None
+    }
+
+
+class Collator:
+  def __init__(self, params):
+    self.params = params
+
+  def collate(self, minibatch):
+    samples_per_frame = self.params.hop_samples
+    for record in minibatch:
+      if self.params.unconditional:
+          # Filter out records that aren't long enough.
+          if len(record['audio']) < self.params.audio_len:
+            del record['spectrogram']
+            del record['audio']
+            continue
+
+          start = random.randint(0, record['audio'].shape[-1] - self.params.audio_len)
+          end = start + self.params.audio_len
+          record['audio'] = record['audio'][start:end]
+          record['audio'] = np.pad(record['audio'], (0, (end - start) - len(record['audio'])), mode='constant')
+      else:
+          # Filter out records that aren't long enough.
+          if len(record['spectrogram']) < self.params.crop_mel_frames:
+            del record['spectrogram']
+            del record['audio']
+            continue
+
+          start = random.randint(0, record['spectrogram'].shape[0] - self.params.crop_mel_frames)
+          end = start + self.params.crop_mel_frames
+          record['spectrogram'] = record['spectrogram'][start:end].T
+
+          start *= samples_per_frame
+          end *= samples_per_frame
+          record['audio'] = record['audio'][start:end]
+          record['audio'] = np.pad(record['audio'], (0, (end-start) - len(record['audio'])), mode='constant')
+
+    audio = np.stack([record['audio'] for record in minibatch if 'audio' in record])
+    if self.params.unconditional:
+        return {
+            'audio': torch.from_numpy(audio),
+            'spectrogram': None,
+        }
+    spectrogram = np.stack([record['spectrogram'] for record in minibatch if 'spectrogram' in record])
+    return {
+        'audio': torch.from_numpy(audio),
+        'spectrogram': torch.from_numpy(spectrogram),
+    }
+
+  # for gtzan
+  def collate_gtzan(self, minibatch):
+    ldata = []
+    mean_audio_len = self.params.audio_len # change to fit in gpu memory
+    # audio total generated time = audio_len * sample_rate
+    # GTZAN statistics
+    # max len audio 675808; min len audio sample 660000; mean len audio sample 662117
+    # max audio sample 1; min audio sample -1; mean audio sample -0.0010 (normalized)
+    # sample rate of all is 22050
+    for data in minibatch:
+      if data[0].shape[-1] < mean_audio_len:  # pad
+        data_audio = F.pad(data[0], (0, mean_audio_len - data[0].shape[-1]), mode='constant', value=0)
+      elif data[0].shape[-1] > mean_audio_len:  # crop
+        start = random.randint(0, data[0].shape[-1] - mean_audio_len)
+        end = start + mean_audio_len
+        data_audio = data[0][:, start:end]
+      else:
+        data_audio = data[0]
+      ldata.append(data_audio)
+    audio = torch.cat(ldata, dim=0)
+    return {
+          'audio': audio,
+          'spectrogram': None,
+    }
+
+
+def from_path(data_dirs, params, is_distributed=False):
+  if params.unconditional:
+    dataset = UnconditionalDataset(data_dirs)
+  else:#with condition
+    dataset = ConditionalDataset(data_dirs)
+  return torch.utils.data.DataLoader(
+      dataset,
+      batch_size=params.batch_size,
+      collate_fn=Collator(params).collate,
+      shuffle=not is_distributed,
+      num_workers=os.cpu_count(),
+      sampler=DistributedSampler(dataset) if is_distributed else None,
+      pin_memory=True,
+      drop_last=True)
+
+
+def from_gtzan(params, is_distributed=False):
+  dataset = torchaudio.datasets.GTZAN('./data', download=True)
+  return torch.utils.data.DataLoader(
+      dataset,
+      batch_size=params.batch_size,
+      collate_fn=Collator(params).collate_gtzan,
+      shuffle=not is_distributed,
+      num_workers=os.cpu_count(),
+      sampler=DistributedSampler(dataset) if is_distributed else None,
+      pin_memory=True,
+      drop_last=True)
```

## dillwave/inference.py

 * *Ordering differences only*

```diff
@@ -1,111 +1,111 @@
-# Copyright 2020 LMNT, Inc. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-# ==============================================================================
-
-import numpy as np
-import os
-import torch
-import torchaudio
-
-from argparse import ArgumentParser
-
-from dillwave.params import AttrDict, params as base_params
-from dillwave.model import DillWave
-
-
-models = {}
-
-def predict(spectrogram=None, model_dir=None, params=None, device=torch.device('cuda'), fast_sampling=False):
-  # Lazy load model.
-  if not model_dir in models:
-    if os.path.exists(f'{model_dir}/weights.pt'):
-      checkpoint = torch.load(f'{model_dir}/weights.pt')
-    else:
-      checkpoint = torch.load(model_dir)
-    model = DillWave(AttrDict(base_params)).to(device)
-    model.load_state_dict(checkpoint['model'])
-    model.eval()
-    models[model_dir] = model
-
-  model = models[model_dir]
-  model.params.override(params)
-  with torch.no_grad():
-    # Change in notation from the DillWave paper for fast sampling.
-    # DillWave paper -> Implementation below
-    # --------------------------------------
-    # alpha -> talpha
-    # beta -> training_noise_schedule
-    # gamma -> alpha
-    # eta -> beta
-    training_noise_schedule = np.array(model.params.noise_schedule)
-    inference_noise_schedule = np.array(model.params.inference_noise_schedule) if fast_sampling else training_noise_schedule
-
-    talpha = 1 - training_noise_schedule
-    talpha_cum = np.cumprod(talpha)
-
-    beta = inference_noise_schedule
-    alpha = 1 - beta
-    alpha_cum = np.cumprod(alpha)
-
-    T = []
-    for s in range(len(inference_noise_schedule)):
-      for t in range(len(training_noise_schedule) - 1):
-        if talpha_cum[t+1] <= alpha_cum[s] <= talpha_cum[t]:
-          twiddle = (talpha_cum[t]**0.5 - alpha_cum[s]**0.5) / (talpha_cum[t]**0.5 - talpha_cum[t+1]**0.5)
-          T.append(t + twiddle)
-          break
-    T = np.array(T, dtype=np.float32)
-
-
-    if not model.params.unconditional:
-      if len(spectrogram.shape) == 2:# Expand rank 2 tensors by adding a batch dimension.
-        spectrogram = spectrogram.unsqueeze(0)
-      spectrogram = spectrogram.to(device)
-      audio = torch.randn(spectrogram.shape[0], model.params.hop_samples * spectrogram.shape[-1], device=device)
-    else:
-      audio = torch.randn(1, params.audio_len, device=device)
-    noise_scale = torch.from_numpy(alpha_cum**0.5).float().unsqueeze(1).to(device)
-
-    for n in range(len(alpha) - 1, -1, -1):
-      c1 = 1 / alpha[n]**0.5
-      c2 = beta[n] / (1 - alpha_cum[n])**0.5
-      audio = c1 * (audio - c2 * model(audio, torch.tensor([T[n]], device=audio.device), spectrogram).squeeze(1))
-      if n > 0:
-        noise = torch.randn_like(audio)
-        sigma = ((1.0 - alpha_cum[n-1]) / (1.0 - alpha_cum[n]) * beta[n])**0.5
-        audio += sigma * noise
-      audio = torch.clamp(audio, -1.0, 1.0)
-  return audio, model.params.sample_rate
-
-
-def main(args):
-  if args.spectrogram_path:
-    spectrogram = torch.from_numpy(np.load(args.spectrogram_path))
-  else:
-    spectrogram = None
-  audio, sr = predict(spectrogram, model_dir=args.model_dir, fast_sampling=args.fast, params=base_params)
-  torchaudio.save(args.output, audio.cpu(), sample_rate=sr)
-
-
-if __name__ == '__main__':
-  parser = ArgumentParser(description='runs inference on a spectrogram file generated by dillwave.preprocess')
-  parser.add_argument('model_dir',
-      help='directory containing a trained model (or full path to weights.pt file)')
-  parser.add_argument('--spectrogram_path', '-s',
-      help='path to a spectrogram file generated by dillwave.preprocess')
-  parser.add_argument('--output', '-o', default='output.wav',
-      help='output file name')
-  parser.add_argument('--fast', '-f', action='store_true',
-      help='fast sampling procedure')
-  main(parser.parse_args())
+# Copyright 2020 LMNT, Inc. All Rights Reserved.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+# ==============================================================================
+
+import numpy as np
+import os
+import torch
+import torchaudio
+
+from argparse import ArgumentParser
+
+from dillwave.params import AttrDict, params as base_params
+from dillwave.model import DillWave
+
+
+models = {}
+
+def predict(spectrogram=None, model_dir=None, params=None, device=torch.device('cuda'), fast_sampling=False):
+  # Lazy load model.
+  if not model_dir in models:
+    if os.path.exists(f'{model_dir}/weights.pt'):
+      checkpoint = torch.load(f'{model_dir}/weights.pt')
+    else:
+      checkpoint = torch.load(model_dir)
+    model = DillWave(AttrDict(base_params)).to(device)
+    model.load_state_dict(checkpoint['model'])
+    model.eval()
+    models[model_dir] = model
+
+  model = models[model_dir]
+  model.params.override(params)
+  with torch.no_grad():
+    # Change in notation from the DillWave paper for fast sampling.
+    # DillWave paper -> Implementation below
+    # --------------------------------------
+    # alpha -> talpha
+    # beta -> training_noise_schedule
+    # gamma -> alpha
+    # eta -> beta
+    training_noise_schedule = np.array(model.params.noise_schedule)
+    inference_noise_schedule = np.array(model.params.inference_noise_schedule) if fast_sampling else training_noise_schedule
+
+    talpha = 1 - training_noise_schedule
+    talpha_cum = np.cumprod(talpha)
+
+    beta = inference_noise_schedule
+    alpha = 1 - beta
+    alpha_cum = np.cumprod(alpha)
+
+    T = []
+    for s in range(len(inference_noise_schedule)):
+      for t in range(len(training_noise_schedule) - 1):
+        if talpha_cum[t+1] <= alpha_cum[s] <= talpha_cum[t]:
+          twiddle = (talpha_cum[t]**0.5 - alpha_cum[s]**0.5) / (talpha_cum[t]**0.5 - talpha_cum[t+1]**0.5)
+          T.append(t + twiddle)
+          break
+    T = np.array(T, dtype=np.float32)
+
+
+    if not model.params.unconditional:
+      if len(spectrogram.shape) == 2:# Expand rank 2 tensors by adding a batch dimension.
+        spectrogram = spectrogram.unsqueeze(0)
+      spectrogram = spectrogram.to(device)
+      audio = torch.randn(spectrogram.shape[0], model.params.hop_samples * spectrogram.shape[-1], device=device)
+    else:
+      audio = torch.randn(1, params.audio_len, device=device)
+    noise_scale = torch.from_numpy(alpha_cum**0.5).float().unsqueeze(1).to(device)
+
+    for n in range(len(alpha) - 1, -1, -1):
+      c1 = 1 / alpha[n]**0.5
+      c2 = beta[n] / (1 - alpha_cum[n])**0.5
+      audio = c1 * (audio - c2 * model(audio, torch.tensor([T[n]], device=audio.device), spectrogram).squeeze(1))
+      if n > 0:
+        noise = torch.randn_like(audio)
+        sigma = ((1.0 - alpha_cum[n-1]) / (1.0 - alpha_cum[n]) * beta[n])**0.5
+        audio += sigma * noise
+      audio = torch.clamp(audio, -1.0, 1.0)
+  return audio, model.params.sample_rate
+
+
+def main(args):
+  if args.spectrogram_path:
+    spectrogram = torch.from_numpy(np.load(args.spectrogram_path))
+  else:
+    spectrogram = None
+  audio, sr = predict(spectrogram, model_dir=args.model_dir, fast_sampling=args.fast, params=base_params)
+  torchaudio.save(args.output, audio.cpu(), sample_rate=sr)
+
+
+if __name__ == '__main__':
+  parser = ArgumentParser(description='runs inference on a spectrogram file generated by dillwave.preprocess')
+  parser.add_argument('model_dir',
+      help='directory containing a trained model (or full path to weights.pt file)')
+  parser.add_argument('--spectrogram_path', '-s',
+      help='path to a spectrogram file generated by dillwave.preprocess')
+  parser.add_argument('--output', '-o', default='output.wav',
+      help='output file name')
+  parser.add_argument('--fast', '-f', action='store_true',
+      help='fast sampling procedure')
+  main(parser.parse_args())
```

## dillwave/learner.py

```diff
@@ -1,180 +1,197 @@
-# Copyright 2020 LMNT, Inc. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-# ==============================================================================
-
-import numpy as np
-import os
-import torch
-import torch.nn as nn
-
-from torch.nn.parallel import DistributedDataParallel
-from torch.utils.tensorboard import SummaryWriter
-from tqdm import tqdm
-
-from dillwave.dataset import from_path, from_gtzan
-from dillwave.model import DillWave
-from dillwave.params import AttrDict
-
-
-def _nested_map(struct, map_fn):
-  if isinstance(struct, tuple):
-    return tuple(_nested_map(x, map_fn) for x in struct)
-  if isinstance(struct, list):
-    return [_nested_map(x, map_fn) for x in struct]
-  if isinstance(struct, dict):
-    return { k: _nested_map(v, map_fn) for k, v in struct.items() }
-  return map_fn(struct)
-
-
-class DillWaveLearner:
-  def __init__(self, model_dir, model, dataset, optimizer, params, *args, **kwargs):
-    os.makedirs(model_dir, exist_ok=True)
-    self.model_dir = model_dir
-    self.model = model
-    self.dataset = dataset
-    self.optimizer = optimizer
-    self.params = params
-    self.autocast = torch.cuda.amp.autocast(enabled=kwargs.get('fp16', False))
-    self.scaler = torch.cuda.amp.GradScaler(enabled=kwargs.get('fp16', False))
-    self.step = 0
-    self.is_master = True
-
-    beta = np.array(self.params.noise_schedule)
-    noise_level = np.cumprod(1 - beta)
-    self.noise_level = torch.tensor(noise_level.astype(np.float32))
-    self.loss_fn = nn.L1Loss()
-    self.summary_writer = None
-
-  def state_dict(self):
-    if hasattr(self.model, 'module') and isinstance(self.model.module, nn.Module):
-      model_state = self.model.module.state_dict()
-    else:
-      model_state = self.model.state_dict()
-    return {
-        'step': self.step,
-        'model': { k: v.cpu() if isinstance(v, torch.Tensor) else v for k, v in model_state.items() },
-        'optimizer': { k: v.cpu() if isinstance(v, torch.Tensor) else v for k, v in self.optimizer.state_dict().items() },
-        'params': dict(self.params),
-        'scaler': self.scaler.state_dict(),
-    }
-
-  def load_state_dict(self, state_dict):
-    if hasattr(self.model, 'module') and isinstance(self.model.module, nn.Module):
-      self.model.module.load_state_dict(state_dict['model'])
-    else:
-      self.model.load_state_dict(state_dict['model'])
-    self.optimizer.load_state_dict(state_dict['optimizer'])
-    self.scaler.load_state_dict(state_dict['scaler'])
-    self.step = state_dict['step']
-
-  def save_to_checkpoint(self, filename='weights'):
-      save_name = f'{self.model_dir}/{filename}.pt'
-      torch.save(self.state_dict(), save_name)
-
-  def restore_from_checkpoint(self, filename='weights'):
-    try:
-      checkpoint = torch.load(f'{self.model_dir}/{filename}.pt')
-      self.load_state_dict(checkpoint)
-      return True
-    except FileNotFoundError:
-      return False
-
-  def train(self, max_steps=None):
-    device = next(self.model.parameters()).device
-    while True:
-      for features in tqdm(self.dataset, desc=f'Epoch {self.step // len(self.dataset)}') if self.is_master else self.dataset:
-        if max_steps is not None and self.step >= max_steps:
-          return
-        features = _nested_map(features, lambda x: x.to(device) if isinstance(x, torch.Tensor) else x)
-        loss = self.train_step(features)
-        if torch.isnan(loss).any():
-          raise RuntimeError(f'Detected NaN loss at step {self.step}.')
-        if self.is_master:
-          if self.step % 50 == 0:
-            self._write_summary(self.step, features, loss)
-          if self.step % len(self.dataset) == 0:
-            self.save_to_checkpoint()
-        self.step += 1
-
-  def train_step(self, features):
-    for param in self.model.parameters():
-      param.grad = None
-
-    audio = features['audio']
-    spectrogram = features['spectrogram']
-
-    N, T = audio.shape
-    device = audio.device
-    self.noise_level = self.noise_level.to(device)
-
-    with self.autocast:
-      t = torch.randint(0, len(self.params.noise_schedule), [N], device=audio.device)
-      noise_scale = self.noise_level[t].unsqueeze(1)
-      noise_scale_sqrt = noise_scale**0.5
-      noise = torch.randn_like(audio)
-      noisy_audio = noise_scale_sqrt * audio + (1.0 - noise_scale)**0.5 * noise
-
-      predicted = self.model(noisy_audio, t, spectrogram)
-      loss = self.loss_fn(noise, predicted.squeeze(1))
-
-    self.scaler.scale(loss).backward()
-    self.scaler.unscale_(self.optimizer)
-    self.grad_norm = nn.utils.clip_grad_norm_(self.model.parameters(), self.params.max_grad_norm or 1e9)
-    self.scaler.step(self.optimizer)
-    self.scaler.update()
-    return loss
-
-  def _write_summary(self, step, features, loss):
-    writer = self.summary_writer or SummaryWriter(self.model_dir, purge_step=step)
-    writer.add_audio('feature/audio', features['audio'][0], step, sample_rate=self.params.sample_rate)
-    if not self.params.unconditional:
-      writer.add_image('feature/spectrogram', torch.flip(features['spectrogram'][:1], [1]), step)
-    writer.add_scalar('train/loss', loss, step)
-    writer.add_scalar('train/grad_norm', self.grad_norm, step)
-    writer.flush()
-    self.summary_writer = writer
-
-
-def _train_impl(replica_id, model, dataset, args, params):
-  torch.backends.cudnn.benchmark = True
-  opt = torch.optim.Adam(model.parameters(), lr=params.learning_rate)
-
-  learner = DillWaveLearner(args.model_dir, model, dataset, opt, params, fp16=args.fp16)
-  learner.is_master = (replica_id == 0)
-  learner.restore_from_checkpoint()
-  learner.train(max_steps=args.max_steps)
-
-
-def train(args, params):
-  if args.data_dirs[0] == 'gtzan':
-    dataset = from_gtzan(params)
-  else:
-    dataset = from_path(args.data_dirs, params)
-  model = DillWave(params).cuda()
-  _train_impl(0, model, dataset, args, params)
-
-
-def train_distributed(replica_id, replica_count, port, args, params):
-  os.environ['MASTER_ADDR'] = 'localhost'
-  os.environ['MASTER_PORT'] = str(port)
-  torch.distributed.init_process_group('nccl', rank=replica_id, world_size=replica_count)
-  if args.data_dirs[0] == 'gtzan':
-    dataset = from_gtzan(params, is_distributed=True)
-  else:
-    dataset = from_path(args.data_dirs, params, is_distributed=True)
-  device = torch.device('cuda', replica_id)
-  torch.cuda.set_device(device)
-  model = DillWave(params).to(device)
-  model = DistributedDataParallel(model, device_ids=[replica_id])
-  _train_impl(replica_id, model, dataset, args, params)
+# Copyright 2020 LMNT, Inc. All Rights Reserved.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+# ==============================================================================
+
+import numpy as np
+import os
+import torch
+import torch.nn as nn
+import signal
+import sys
+import threading
+
+from torch.nn.parallel import DistributedDataParallel
+from torch.utils.tensorboard import SummaryWriter
+from tqdm import tqdm
+
+from dillwave.dataset import from_path, from_gtzan
+from dillwave.model import DillWave
+from dillwave.params import AttrDict
+
+signal_lock = threading.Lock()
+
+def _nested_map(struct, map_fn):
+  if isinstance(struct, tuple):
+    return tuple(_nested_map(x, map_fn) for x in struct)
+  if isinstance(struct, list):
+    return [_nested_map(x, map_fn) for x in struct]
+  if isinstance(struct, dict):
+    return { k: _nested_map(v, map_fn) for k, v in struct.items() }
+  return map_fn(struct)
+
+class DillWaveLearner:
+  def __init__(self, model_dir, model, dataset, optimizer, params, *args, **kwargs):
+    self.step = 0
+    signal.signal(signal.SIGINT, self.signal_handler)
+    os.makedirs(model_dir, exist_ok=True)
+    self.model_dir = model_dir
+    self.model = model
+    self.dataset = dataset
+    self.optimizer = optimizer
+    self.params = params
+    self.autocast = torch.cuda.amp.autocast(enabled=kwargs.get('fp16', False))
+    self.scaler = torch.cuda.amp.GradScaler(enabled=kwargs.get('fp16', False))
+    self.is_master = True
+
+    beta = np.array(self.params.noise_schedule)
+    noise_level = np.cumprod(1 - beta)
+    self.noise_level = torch.tensor(noise_level.astype(np.float32))
+    self.loss_fn = nn.L1Loss()
+    self.summary_writer = None
+
+  def signal_handler(self, sig, frame):
+      with signal_lock:
+          print('Caught SIGINT, saving interrupt checkpoint...')
+          print(f'Saving step: {self.step}')
+          self.save_to_checkpoint(filename='weights')
+          print('Interrupt checkpoint saved. Exiting...')
+          sys.exit(0)
+
+  def state_dict(self):
+    if hasattr(self.model, 'module') and isinstance(self.model.module, nn.Module):
+      model_state = self.model.module.state_dict()
+    else:
+      model_state = self.model.state_dict()
+    return {
+        'step': int(self.step),
+        'model': { k: v.cpu() if isinstance(v, torch.Tensor) else v for k, v in model_state.items() },
+        'optimizer': { k: v.cpu() if isinstance(v, torch.Tensor) else v for k, v in self.optimizer.state_dict().items() },
+        'params': dict(self.params),
+        'scaler': self.scaler.state_dict(),
+    }
+
+  def load_state_dict(self, state_dict):
+      if hasattr(self.model, 'module') and isinstance(self.model.module, nn.Module):
+          self.model.module.load_state_dict(state_dict['model'])
+      else:
+          self.model.load_state_dict(state_dict['model'])
+      self.optimizer.load_state_dict(state_dict['optimizer'])
+      self.scaler.load_state_dict(state_dict['scaler'])
+      self.step = state_dict['step']
+
+  def save_to_checkpoint(self, filename='weights'):
+      save_name = f'{self.model_dir}/{filename}.pt'
+      torch.save(self.state_dict(), save_name)
+
+  def restore_from_checkpoint(self, filename=None):
+      if filename is None:
+          filename = 'weights'
+      try:
+          checkpoint = torch.load(f'{self.model_dir}/{filename}.pt')
+          print(f'Loaded step: {checkpoint["step"]}')
+          self.load_state_dict(checkpoint)
+          self.step = checkpoint["step"]
+          return True
+      except FileNotFoundError:
+          return False
+
+  def train(self, max_steps=None):
+      device = next(self.model.parameters()).device
+      while True:
+          for features in tqdm(self.dataset, desc=f'Epoch {self.step // len(self.dataset)}', initial=self.step % len(self.dataset)) if self.is_master else self.dataset:
+              if max_steps is not None and self.step >= max_steps:
+                  return
+              features = _nested_map(features, lambda x: x.to(device) if isinstance(x, torch.Tensor) else x)
+              loss = self.train_step(features)
+              if torch.isnan(loss).any():
+                  raise RuntimeError(f'Detected NaN loss at step {self.step}.')
+              if self.is_master:
+                  if self.step % 50 == 0:
+                      self._write_summary(self.step, features, loss)
+                  # Remove the following line to prevent saving initial weights file
+                  # if self.step % len(self.dataset) == 0:
+                  #     self.save_to_checkpoint()
+              self.step += 1
+
+  def train_step(self, features):
+    for param in self.model.parameters():
+      param.grad = None
+
+    audio = features['audio']
+    spectrogram = features['spectrogram']
+
+    N, T = audio.shape
+    device = audio.device
+    self.noise_level = self.noise_level.to(device)
+
+    with self.autocast:
+      t = torch.randint(0, len(self.params.noise_schedule), [N], device=audio.device)
+      noise_scale = self.noise_level[t].unsqueeze(1)
+      noise_scale_sqrt = noise_scale**0.5
+      noise = torch.randn_like(audio)
+      noisy_audio = noise_scale_sqrt * audio + (1.0 - noise_scale)**0.5 * noise
+
+      predicted = self.model(noisy_audio, t, spectrogram)
+      loss = self.loss_fn(noise, predicted.squeeze(1))
+
+    self.scaler.scale(loss).backward()
+    self.scaler.unscale_(self.optimizer)
+    self.grad_norm = nn.utils.clip_grad_norm_(self.model.parameters(), self.params.max_grad_norm or 1e9)
+    self.scaler.step(self.optimizer)
+    self.scaler.update()
+    return loss
+
+  def _write_summary(self, step, features, loss):
+    writer = self.summary_writer or SummaryWriter(self.model_dir, purge_step=step)
+    writer.add_audio('feature/audio', features['audio'][0], step, sample_rate=self.params.sample_rate)
+    if not self.params.unconditional:
+      writer.add_image('feature/spectrogram', torch.flip(features['spectrogram'][:1], [1]), step)
+    writer.add_scalar('train/loss', loss, step)
+    writer.add_scalar('train/grad_norm', self.grad_norm, step)
+    writer.flush()
+    self.summary_writer = writer
+
+
+def _train_impl(replica_id, model, dataset, args, params):
+  torch.backends.cudnn.benchmark = True
+  opt = torch.optim.Adam(model.parameters(), lr=params.learning_rate)
+
+  learner = DillWaveLearner(args.model_dir, model, dataset, opt, params, fp16=args.fp16)
+  learner.is_master = (replica_id == 0)
+  learner.restore_from_checkpoint()
+  learner.train(max_steps=args.max_steps)
+
+
+def train(args, params):
+  if args.data_dirs[0] == 'gtzan':
+    dataset = from_gtzan(params)
+  else:
+    dataset = from_path(args.data_dirs, params)
+  model = DillWave(params).cuda()
+  _train_impl(0, model, dataset, args, params)
+
+
+def train_distributed(replica_id, replica_count, port, args, params):
+  os.environ['MASTER_ADDR'] = 'localhost'
+  os.environ['MASTER_PORT'] = str(port)
+  torch.distributed.init_process_group('nccl', rank=replica_id, world_size=replica_count)
+  if args.data_dirs[0] == 'gtzan':
+    dataset = from_gtzan(params, is_distributed=True)
+  else:
+    dataset = from_path(args.data_dirs, params, is_distributed=True)
+  device = torch.device('cuda', replica_id)
+  torch.cuda.set_device(device)
+  model = DillWave(params).to(device)
+  model = DistributedDataParallel(model, device_ids=[replica_id])
+  _train_impl(replica_id, model, dataset, args, params)
```

## dillwave/model.py

 * *Ordering differences only*

```diff
@@ -1,161 +1,161 @@
-# Copyright 2020 LMNT, Inc. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-# ==============================================================================
-
-import numpy as np
-import torch
-import torch.nn as nn
-import torch.nn.functional as F
-
-from math import sqrt
-
-
-Linear = nn.Linear
-ConvTranspose2d = nn.ConvTranspose2d
-
-
-def Conv1d(*args, **kwargs):
-  layer = nn.Conv1d(*args, **kwargs)
-  nn.init.kaiming_normal_(layer.weight)
-  return layer
-
-
-@torch.jit.script
-def silu(x):
-  return x * torch.sigmoid(x)
-
-
-class DiffusionEmbedding(nn.Module):
-  def __init__(self, max_steps):
-    super().__init__()
-    self.register_buffer('embedding', self._build_embedding(max_steps), persistent=False)
-    self.projection1 = Linear(128, 512)
-    self.projection2 = Linear(512, 512)
-
-  def forward(self, diffusion_step):
-    if diffusion_step.dtype in [torch.int32, torch.int64]:
-      x = self.embedding[diffusion_step]
-    else:
-      x = self._lerp_embedding(diffusion_step)
-    x = self.projection1(x)
-    x = silu(x)
-    x = self.projection2(x)
-    x = silu(x)
-    return x
-
-  def _lerp_embedding(self, t):
-    low_idx = torch.floor(t).long()
-    high_idx = torch.ceil(t).long()
-    low = self.embedding[low_idx]
-    high = self.embedding[high_idx]
-    return low + (high - low) * (t - low_idx)
-
-  def _build_embedding(self, max_steps):
-    steps = torch.arange(max_steps).unsqueeze(1)  # [T,1]
-    dims = torch.arange(64).unsqueeze(0)          # [1,64]
-    table = steps * 10.0**(dims * 4.0 / 63.0)     # [T,64]
-    table = torch.cat([torch.sin(table), torch.cos(table)], dim=1)
-    return table
-
-
-class SpectrogramUpsampler(nn.Module):
-  def __init__(self, n_mels):
-    super().__init__()
-    self.conv1 = ConvTranspose2d(1, 1, [3, 32], stride=[1, 16], padding=[1, 8])
-    self.conv2 = ConvTranspose2d(1, 1,  [3, 32], stride=[1, 16], padding=[1, 8])
-
-  def forward(self, x):
-    x = torch.unsqueeze(x, 1)
-    x = self.conv1(x)
-    x = F.leaky_relu(x, 0.4)
-    x = self.conv2(x)
-    x = F.leaky_relu(x, 0.4)
-    x = torch.squeeze(x, 1)
-    return x
-
-
-class ResidualBlock(nn.Module):
-  def __init__(self, n_mels, residual_channels, dilation, uncond=False):
-    '''
-    :param n_mels: inplanes of conv1x1 for spectrogram conditional
-    :param residual_channels: audio conv
-    :param dilation: audio conv dilation
-    :param uncond: disable spectrogram conditional
-    '''
-    super().__init__()
-    self.dilated_conv = Conv1d(residual_channels, 2 * residual_channels, 3, padding=dilation, dilation=dilation)
-    self.diffusion_projection = Linear(512, residual_channels)
-    if not uncond: # conditional model
-      self.conditioner_projection = Conv1d(n_mels, 2 * residual_channels, 1)
-    else: # unconditional model
-      self.conditioner_projection = None
-
-    self.output_projection = Conv1d(residual_channels, 2 * residual_channels, 1)
-
-  def forward(self, x, diffusion_step, conditioner=None):
-
-    diffusion_step = self.diffusion_projection(diffusion_step).unsqueeze(-1)
-    y = x + diffusion_step
-    if self.conditioner_projection is None: # using a unconditional model
-      y = self.dilated_conv(y)
-    else:
-      conditioner = self.conditioner_projection(conditioner)
-      y = self.dilated_conv(y) + conditioner
-
-    gate, filter = torch.chunk(y, 2, dim=1)
-    y = torch.sigmoid(gate) * torch.tanh(filter)
-
-    y = self.output_projection(y)
-    residual, skip = torch.chunk(y, 2, dim=1)
-    return (x + residual) / sqrt(2.0), skip
-
-
-class DillWave(nn.Module):
-  def __init__(self, params):
-    super().__init__()
-    self.params = params
-    self.input_projection = Conv1d(1, params.residual_channels, 1)
-    self.diffusion_embedding = DiffusionEmbedding(len(params.noise_schedule))
-    if self.params.unconditional: # use unconditional model
-      self.spectrogram_upsampler = None
-    else:
-      self.spectrogram_upsampler = SpectrogramUpsampler(params.n_mels)
-
-    self.residual_layers = nn.ModuleList([
-        ResidualBlock(params.n_mels, params.residual_channels, 2**(i % params.dilation_cycle_length), uncond=params.unconditional)
-        for i in range(params.residual_layers)
-    ])
-    self.skip_projection = Conv1d(params.residual_channels, params.residual_channels, 1)
-    self.output_projection = Conv1d(params.residual_channels, 1, 1)
-    nn.init.zeros_(self.output_projection.weight)
-
-  def forward(self, audio, diffusion_step, spectrogram=None):
-    x = audio.unsqueeze(1)
-    x = self.input_projection(x)
-    x = F.relu(x)
-
-    diffusion_step = self.diffusion_embedding(diffusion_step)
-    if self.spectrogram_upsampler: # use conditional model
-      spectrogram = self.spectrogram_upsampler(spectrogram)
-
-    skip = None
-    for layer in self.residual_layers:
-      x, skip_connection = layer(x, diffusion_step, spectrogram)
-      skip = skip_connection if skip is None else skip_connection + skip
-
-    x = skip / sqrt(len(self.residual_layers))
-    x = self.skip_projection(x)
-    x = F.relu(x)
-    x = self.output_projection(x)
-    return x
+# Copyright 2020 LMNT, Inc. All Rights Reserved.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+# ==============================================================================
+
+import numpy as np
+import torch
+import torch.nn as nn
+import torch.nn.functional as F
+
+from math import sqrt
+
+
+Linear = nn.Linear
+ConvTranspose2d = nn.ConvTranspose2d
+
+
+def Conv1d(*args, **kwargs):
+  layer = nn.Conv1d(*args, **kwargs)
+  nn.init.kaiming_normal_(layer.weight)
+  return layer
+
+
+@torch.jit.script
+def silu(x):
+  return x * torch.sigmoid(x)
+
+
+class DiffusionEmbedding(nn.Module):
+  def __init__(self, max_steps):
+    super().__init__()
+    self.register_buffer('embedding', self._build_embedding(max_steps), persistent=False)
+    self.projection1 = Linear(128, 512)
+    self.projection2 = Linear(512, 512)
+
+  def forward(self, diffusion_step):
+    if diffusion_step.dtype in [torch.int32, torch.int64]:
+      x = self.embedding[diffusion_step]
+    else:
+      x = self._lerp_embedding(diffusion_step)
+    x = self.projection1(x)
+    x = silu(x)
+    x = self.projection2(x)
+    x = silu(x)
+    return x
+
+  def _lerp_embedding(self, t):
+    low_idx = torch.floor(t).long()
+    high_idx = torch.ceil(t).long()
+    low = self.embedding[low_idx]
+    high = self.embedding[high_idx]
+    return low + (high - low) * (t - low_idx)
+
+  def _build_embedding(self, max_steps):
+    steps = torch.arange(max_steps).unsqueeze(1)  # [T,1]
+    dims = torch.arange(64).unsqueeze(0)          # [1,64]
+    table = steps * 10.0**(dims * 4.0 / 63.0)     # [T,64]
+    table = torch.cat([torch.sin(table), torch.cos(table)], dim=1)
+    return table
+
+
+class SpectrogramUpsampler(nn.Module):
+  def __init__(self, n_mels):
+    super().__init__()
+    self.conv1 = ConvTranspose2d(1, 1, [3, 32], stride=[1, 16], padding=[1, 8])
+    self.conv2 = ConvTranspose2d(1, 1,  [3, 32], stride=[1, 16], padding=[1, 8])
+
+  def forward(self, x):
+    x = torch.unsqueeze(x, 1)
+    x = self.conv1(x)
+    x = F.leaky_relu(x, 0.4)
+    x = self.conv2(x)
+    x = F.leaky_relu(x, 0.4)
+    x = torch.squeeze(x, 1)
+    return x
+
+
+class ResidualBlock(nn.Module):
+  def __init__(self, n_mels, residual_channels, dilation, uncond=False):
+    '''
+    :param n_mels: inplanes of conv1x1 for spectrogram conditional
+    :param residual_channels: audio conv
+    :param dilation: audio conv dilation
+    :param uncond: disable spectrogram conditional
+    '''
+    super().__init__()
+    self.dilated_conv = Conv1d(residual_channels, 2 * residual_channels, 3, padding=dilation, dilation=dilation)
+    self.diffusion_projection = Linear(512, residual_channels)
+    if not uncond: # conditional model
+      self.conditioner_projection = Conv1d(n_mels, 2 * residual_channels, 1)
+    else: # unconditional model
+      self.conditioner_projection = None
+
+    self.output_projection = Conv1d(residual_channels, 2 * residual_channels, 1)
+
+  def forward(self, x, diffusion_step, conditioner=None):
+
+    diffusion_step = self.diffusion_projection(diffusion_step).unsqueeze(-1)
+    y = x + diffusion_step
+    if self.conditioner_projection is None: # using a unconditional model
+      y = self.dilated_conv(y)
+    else:
+      conditioner = self.conditioner_projection(conditioner)
+      y = self.dilated_conv(y) + conditioner
+
+    gate, filter = torch.chunk(y, 2, dim=1)
+    y = torch.sigmoid(gate) * torch.tanh(filter)
+
+    y = self.output_projection(y)
+    residual, skip = torch.chunk(y, 2, dim=1)
+    return (x + residual) / sqrt(2.0), skip
+
+
+class DillWave(nn.Module):
+  def __init__(self, params):
+    super().__init__()
+    self.params = params
+    self.input_projection = Conv1d(1, params.residual_channels, 1)
+    self.diffusion_embedding = DiffusionEmbedding(len(params.noise_schedule))
+    if self.params.unconditional: # use unconditional model
+      self.spectrogram_upsampler = None
+    else:
+      self.spectrogram_upsampler = SpectrogramUpsampler(params.n_mels)
+
+    self.residual_layers = nn.ModuleList([
+        ResidualBlock(params.n_mels, params.residual_channels, 2**(i % params.dilation_cycle_length), uncond=params.unconditional)
+        for i in range(params.residual_layers)
+    ])
+    self.skip_projection = Conv1d(params.residual_channels, params.residual_channels, 1)
+    self.output_projection = Conv1d(params.residual_channels, 1, 1)
+    nn.init.zeros_(self.output_projection.weight)
+
+  def forward(self, audio, diffusion_step, spectrogram=None):
+    x = audio.unsqueeze(1)
+    x = self.input_projection(x)
+    x = F.relu(x)
+
+    diffusion_step = self.diffusion_embedding(diffusion_step)
+    if self.spectrogram_upsampler: # use conditional model
+      spectrogram = self.spectrogram_upsampler(spectrogram)
+
+    skip = None
+    for layer in self.residual_layers:
+      x, skip_connection = layer(x, diffusion_step, spectrogram)
+      skip = skip_connection if skip is None else skip_connection + skip
+
+    x = skip / sqrt(len(self.residual_layers))
+    x = self.skip_projection(x)
+    x = F.relu(x)
+    x = self.output_projection(x)
+    return x
```

## dillwave/params.py

 * *Ordering differences only*

```diff
@@ -1,58 +1,58 @@
-# Copyright 2020 LMNT, Inc. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-# ==============================================================================
-
-import numpy as np
-
-
-class AttrDict(dict):
-  def __init__(self, *args, **kwargs):
-      super(AttrDict, self).__init__(*args, **kwargs)
-      self.__dict__ = self
-
-  def override(self, attrs):
-    if isinstance(attrs, dict):
-      self.__dict__.update(**attrs)
-    elif isinstance(attrs, (list, tuple, set)):
-      for attr in attrs:
-        self.override(attr)
-    elif attrs is not None:
-      raise NotImplementedError
-    return self
-
-
-params = AttrDict(
-    # Training params
-    batch_size=16,
-    learning_rate=2e-4,
-    max_grad_norm=None,
-
-    # Data params
-    sample_rate=48000,
-    n_mels=128,
-    n_fft=1024,
-    hop_samples=256,
-    crop_mel_frames=62,  # Probably an error in paper.
-
-    # Model params
-    residual_layers=50,
-    residual_channels=80,
-    dilation_cycle_length=10,
-    unconditional = False,
-    noise_schedule=np.linspace(1e-4, 0.05, 50).tolist(),
-    inference_noise_schedule=[0.0001, 0.001, 0.01, 0.05, 0.2, 0.5],
-
-    # unconditional sample len
-    audio_len = 48000*5, # unconditional_synthesis_samples
-)
+# Copyright 2020 LMNT, Inc. All Rights Reserved.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+# ==============================================================================
+
+import numpy as np
+
+
+class AttrDict(dict):
+  def __init__(self, *args, **kwargs):
+      super(AttrDict, self).__init__(*args, **kwargs)
+      self.__dict__ = self
+
+  def override(self, attrs):
+    if isinstance(attrs, dict):
+      self.__dict__.update(**attrs)
+    elif isinstance(attrs, (list, tuple, set)):
+      for attr in attrs:
+        self.override(attr)
+    elif attrs is not None:
+      raise NotImplementedError
+    return self
+
+
+params = AttrDict(
+    # Training params
+    batch_size=16,
+    learning_rate=2e-4,
+    max_grad_norm=None,
+
+    # Data params
+    sample_rate=48000,
+    n_mels=128,
+    n_fft=1024,
+    hop_samples=256,
+    crop_mel_frames=62,  # Probably an error in paper.
+
+    # Model params
+    residual_layers=50,
+    residual_channels=80,
+    dilation_cycle_length=10,
+    unconditional = False,
+    noise_schedule=np.linspace(1e-4, 0.05, 50).tolist(),
+    inference_noise_schedule=[0.0001, 0.001, 0.01, 0.05, 0.2, 0.5],
+
+    # unconditional sample len
+    audio_len = 48000*5, # unconditional_synthesis_samples
+)
```

## dillwave/preprocess.py

 * *Ordering differences only*

```diff
@@ -1,65 +1,65 @@
-# Copyright 2020 LMNT, Inc. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-# ==============================================================================
-
-import numpy as np
-import torch
-import torchaudio as T
-import torchaudio.transforms as TT
-
-from argparse import ArgumentParser
-from concurrent.futures import ProcessPoolExecutor
-from glob import glob
-from tqdm import tqdm
-
-from dillwave.params import params
-
-
-def transform(filename):
-  audio, sr = T.load(filename)
-  audio = torch.clamp(audio[0], -1.0, 1.0)
-
-  if params.sample_rate != sr:
-    raise ValueError(f'Invalid sample rate {sr}.')
-  mel_args = {
-      'sample_rate': sr,
-      'win_length': params.hop_samples * 4,
-      'hop_length': params.hop_samples,
-      'n_fft': params.n_fft,
-      'f_min': 20.0,
-      'f_max': sr / 2.0,
-      'n_mels': params.n_mels,
-      'power': 1.0,
-      'normalized': True,
-  }
-  mel_spec_transform = TT.MelSpectrogram(**mel_args)
-
-  with torch.no_grad():
-    spectrogram = mel_spec_transform(audio)
-    spectrogram = 20 * torch.log10(torch.clamp(spectrogram, min=1e-5)) - 20
-    spectrogram = torch.clamp((spectrogram + 100) / 100, 0.0, 1.0)
-    np.save(f'{filename}.spec.npy', spectrogram.cpu().numpy())
-
-
-def main(args):
-  filenames = glob(f'{args.dir}/**/*.wav', recursive=True)
-  with ProcessPoolExecutor() as executor:
-    list(tqdm(executor.map(transform, filenames), desc='Preprocessing', total=len(filenames)))
-
-
-if __name__ == '__main__':
-  parser = ArgumentParser(description='prepares a dataset to train DillWave')
-  parser.add_argument('dir',
-      help='directory containing .wav files for training')
-  main(parser.parse_args())
+# Copyright 2020 LMNT, Inc. All Rights Reserved.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+# ==============================================================================
+
+import numpy as np
+import torch
+import torchaudio as T
+import torchaudio.transforms as TT
+
+from argparse import ArgumentParser
+from concurrent.futures import ProcessPoolExecutor
+from glob import glob
+from tqdm import tqdm
+
+from dillwave.params import params
+
+
+def transform(filename):
+  audio, sr = T.load(filename)
+  audio = torch.clamp(audio[0], -1.0, 1.0)
+
+  if params.sample_rate != sr:
+    raise ValueError(f'Invalid sample rate {sr}.')
+  mel_args = {
+      'sample_rate': sr,
+      'win_length': params.hop_samples * 4,
+      'hop_length': params.hop_samples,
+      'n_fft': params.n_fft,
+      'f_min': 20.0,
+      'f_max': sr / 2.0,
+      'n_mels': params.n_mels,
+      'power': 1.0,
+      'normalized': True,
+  }
+  mel_spec_transform = TT.MelSpectrogram(**mel_args)
+
+  with torch.no_grad():
+    spectrogram = mel_spec_transform(audio)
+    spectrogram = 20 * torch.log10(torch.clamp(spectrogram, min=1e-5)) - 20
+    spectrogram = torch.clamp((spectrogram + 100) / 100, 0.0, 1.0)
+    np.save(f'{filename}.spec.npy', spectrogram.cpu().numpy())
+
+
+def main(args):
+  filenames = glob(f'{args.dir}/**/*.wav', recursive=True)
+  with ProcessPoolExecutor() as executor:
+    list(tqdm(executor.map(transform, filenames), desc='Preprocessing', total=len(filenames)))
+
+
+if __name__ == '__main__':
+  parser = ArgumentParser(description='prepares a dataset to train DillWave')
+  parser.add_argument('dir',
+      help='directory containing .wav files for training')
+  main(parser.parse_args())
```

## Comparing `dillwave-1.0.1.dist-info/LICENSE.txt` & `dillwave-1.0.2.dist-info/LICENSE.txt`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
    limitations under the License.
```

## Comparing `dillwave-1.0.1.dist-info/METADATA` & `dillwave-1.0.2.dist-info/METADATA`

 * *Files 13% similar despite different names*

```diff
@@ -1,75 +1,73 @@
-Metadata-Version: 2.1
-Name: dillwave
-Version: 1.0.1
-Summary: dillwave
-Home-page: https://dill.moe
-Author: Cross Nastasi
-Author-email: cross@dill.moe
-License: Apache 2.0
-Keywords: dillwave machine learning neural vocoder tts speech
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Software Development :: Libraries
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-Requires-Dist: numpy
-Requires-Dist: torch
-Requires-Dist: torchaudio
-Requires-Dist: tqdm
-Requires-Dist: tensorboard
-Requires-Dist: packaging
-Requires-Dist: soundfile
-
-# DillWave
-
-DillWave is a fast, high-quality neural vocoder and waveform synthesizer. It starts with Gaussian noise and converts it into speech via iterative refinement. The speech can be controlled by providing a conditioning signal (e.g. log-scaled Mel spectrogram). The model and architecture details are described in [DiffWave: A Versatile Diffusion Model for Audio Synthesis](https://arxiv.org/pdf/2009.09761.pdf).
-
-Credit to the original repo [here](https://github.com/lmnt-com/diffwave).
-
-## Install
-
-(First install [Pytorch](https://pytorch.org), GPU version recommended!)
-
-As a package:
-```bash
-pip install dillwave
-```
-
-From GitHub:
-```bash
-git clone https://github.com/dillfrescott/dillwave
-pip install -e dillwave
-```
-or
-```bash
-pip install git+https://github.com/dillfrescott/dillwave
-```
-You need [Git](https://git-scm.com) installed for either of these "From GitHub" install methods to work.
-
-### Training
-
-```bash
-python -m dillwave.preprocess /path/to/dir/containing/wavs # 48000hz, 1 channel
-python -m dillwave /path/to/model/dir /path/to/dir/containing/wavs
-
-# in another shell to monitor training progress:
-tensorboard --logdir /path/to/model/dir --bind_all
-```
-
-You should expect to hear intelligible (but noisy) speech by ~8k steps (~1.5h on a 2080 Ti).
-
-### Inference CLI
-```bash
-python -m dillwave.inference /path/to/model --spectrogram_path /path/to/spectrogram -o output.wav [--fast]
-```
-
-I plan to release a pretrained model if it turns out good enough! :)
+Metadata-Version: 2.1
+Name: dillwave
+Version: 1.0.2
+Summary: dillwave
+Home-page: https://dill.moe
+Author: Cross Nastasi
+Author-email: cross@dill.moe
+License: Apache 2.0
+Keywords: dillwave machine learning neural vocoder tts speech
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Topic :: Scientific/Engineering :: Mathematics
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Software Development :: Libraries
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Requires-Dist: numpy
+Requires-Dist: torch
+Requires-Dist: torchaudio
+Requires-Dist: tqdm
+Requires-Dist: tensorboard
+Requires-Dist: packaging
+Requires-Dist: soundfile
+
+# DillWave
+
+DillWave is a fast, high-quality neural vocoder and waveform synthesizer. It starts with Gaussian noise and converts it into speech via iterative refinement. The speech can be controlled by providing a conditioning signal (e.g. log-scaled Mel spectrogram). The model and architecture details are described in [DiffWave: A Versatile Diffusion Model for Audio Synthesis](https://arxiv.org/pdf/2009.09761.pdf).
+
+Credit to the original repo [here](https://github.com/lmnt-com/diffwave).
+
+## Install
+
+First install [Pytorch](https://pytorch.org), GPU version recommended! Also you need [Python](https://www.python.org) of course! Version 3.10.X is recommended for dillwave.
+
+As a package:
+```bash
+pip install dillwave
+```
+
+From GitHub:
+```bash
+git clone https://github.com/dillfrescott/dillwave
+pip install -e dillwave
+```
+or
+```bash
+pip install git+https://github.com/dillfrescott/dillwave
+```
+You need [Git](https://git-scm.com) installed for either of these "From GitHub" install methods to work.
+
+### Training
+
+```bash
+python -m dillwave.preprocess /path/to/dir/containing/wavs # 48000hz, 1 channel
+python -m dillwave /path/to/model/dir /path/to/dir/containing/wavs
+
+# in another shell to monitor training progress:
+tensorboard --logdir /path/to/model/dir --bind_all
+```
+
+### Inference CLI
+```bash
+python -m dillwave.inference /path/to/model --spectrogram_path /path/to/spectrogram -o output.wav [--fast]
+```
+
+Pretrained models are going to be released [here](https://github.com/dillfrescott/dillwave-model).
```

