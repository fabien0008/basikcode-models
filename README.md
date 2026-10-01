# BasikCode models

Model files downloaded on demand by BasikCode apps, mirrored here so the apps depend on a stable,
pinned URL rather than a third-party link that could move.

## omnilingual-300m-ctc-v2-int8

Used by **Speech to Text Offline** for languages where it is far more accurate than Whisper-base
(measured on Google FLEURS — e.g. Egyptian Arabic 4.0% vs 16.6% character error rate, Hindi 6.3%
vs unusable). Downloaded only when the user accepts it.

- `model.int8.onnx.gz` — gzip of `model.int8.onnx` (365,841,453 bytes,
  SHA-256 `e3042b2f3b3ef0af2211bf99d2b4bf94a21f5ac0e9898827e7dd6d003a860e91`; the app verifies it)
- Source: Meta **Omnilingual ASR** 300M CTC v2, int8 ONNX export by the
  [sherpa-onnx](https://github.com/k2-fsa/sherpa-onnx) project
  (`sherpa-onnx-omnilingual-asr-1600-languages-300M-ctc-v2-int8-2026-02-05`)
- License: Apache License 2.0, Copyright 2025 (c) Meta Platforms, Inc. and affiliates —
  see `LICENSE-omnilingual-asr`. The file is redistributed unmodified apart from gzip compression.
