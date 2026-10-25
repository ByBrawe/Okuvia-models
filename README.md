# Okuvia optional model assets

Only model packages, checksums and license notices are published here. The Okuvia application source is not included.

## Pocket TTS English — experimental

Three optional CPU ONNX packages, each with one matching official Alba preset. No user voice cloning.

### Pocket TTS 1.9M

- [Download ZIP](https://github.com/ByBrawe/Okuvia-models/releases/download/pocket-small-onnx-20261025/en-pocket-small-2m-202610.zip)
- Download: 7728565 bytes; installed payload: 8752512 bytes.
- SHA-256: 15cad856bb11491e153f9a7bcfeb7df4d19b65c29414127b861c216540e8356a

### Pocket TTS 6.9M

- [Download ZIP](https://github.com/ByBrawe/Okuvia-models/releases/download/pocket-small-onnx-20261025/en-pocket-small-7m-202610.zip)
- Download: 26596432 bytes; installed payload: 29457832 bytes.
- SHA-256: f92ad29e947299592ca2d19e7c1c699085424bbc8c1549248a765d21604af1b2

### Pocket TTS 18.2M

- [Download ZIP](https://github.com/ByBrawe/Okuvia-models/releases/download/pocket-small-onnx-20261025/en-pocket-small-18m-202610.zip)
- Download: 71426315 bytes; installed payload: 77786400 bytes.
- SHA-256: 5b36f5d6914dea492cb9b1d18812075de45a9cadc2539916f2969d586ef4596f

## Provenance and licenses

- Original weights and matching voice states: [Kyutai Pocket TTS](https://huggingface.co/kyutai/pocket-tts-without-voice-cloning/tree/a7056f505a4a8ca72d8b5fb1440071d6f1a35739), CC BY 4.0.
- Original reference performance: Alba MacKenna; CC BY 4.0 attribution is included in every ZIP.
- Upstream inference/export architecture: [Pocket TTS source](https://github.com/kyutai-labs/pocket-tts/tree/44cb63eaa4144f32ff80863968515165a5554353), Apache-2.0.
- Changes by Okuvia: architecture-specific ONNX graphs, explicit GQA caches, bounded full-span decoder, precomputed preset state conversion.
- MODEL_LICENSE.txt and MODEL_NOTICE.txt inside each ZIP retain the required notices. The names identify upstream presets and do not imply endorsement.

## Validation limits

Windows ONNX and Android API 36 x86_64 release WAV smoke tests passed. Physical ARM64 and general pronunciation-quality acceptance remain pending. These are experimental model assets, not an application APK/AAB.
All model weights are optional downloads; users should install a compatible Okuvia build.
