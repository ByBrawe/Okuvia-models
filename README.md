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
## Pocket TTS French and Dutch — experimental

[Release, manifest and seven generated previews](https://github.com/ByBrawe/Okuvia-models/releases/tag/pocket-multilingual-preset-20261026)

- French / Estelle: `fr-pocket-tts-202610-preset.zip`, 193598080 bytes.
  SHA-256: `6068d9e5fa2b91c92bda8a3d874c34a3f99799cd5bef45634644b4e37febf718`.
- Dutch / Daan: `nl-pocket-tts-202610-preset.zip`, 191902278 bytes.
  SHA-256: `4ae35adbf240233d33786cec71db20216e26ace044b229b61e97b989a82bf1d8`.

Official public Kyutai weights and official precomputed voice states are CC BY 4.0.
Weights are pinned to revision `1e08e6a23401048648a9fdcfde2f89348215c2a7`;
voice states to `a7056f505a4a8ca72d8b5fb1440071d6f1a35739`.
Every ZIP includes the full model license and voice attribution. Names identify
upstream presets and do not imply endorsement. No raw reference recordings or
user voice-cloning feature are included. Okuvia converted the ONNX graphs,
tokenizer and fixed KV preset representation; upstream source and runtime notices
remain in the package. Runtime code uses MIT and Apache-2.0 components.

Official Python-reference and Android API36 x86_64 WAV tests passed, including
active cancellation and restart. This does not establish numerical graph parity,
physical ARM64 compatibility or independent pronunciation-quality acceptance.
Other preview languages use their separately attributed upstream packages;
these two ZIPs do not contain all seven models. Install a compatible Okuvia build.
