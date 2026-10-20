# Offline Parrot speech models

This public repository distributes the optional on-device speech models used by Offline Parrot STT. It contains model files and their license notices; it does not contain the Android application or user data.

## Model choices

- **Parakeet Unified** — English; NVIDIA Open Model License; approximately 630 MiB.
- **Parakeet v3** — 25 languages; NVIDIA model under CC BY 4.0; approximately 640 MiB.

The full license and attribution notice is included with each model's release assets. The models are INT8 ONNX conversions produced using [sherpa-onnx](https://github.com/k2-fsa/sherpa-onnx).

## Downloads

The app downloads only the model the user selects, from the pinned release listed in its bundled `model_release_manifest.json`. Each asset is checked against its expected byte count and SHA-256 digest before the model can be used. Published model releases are versioned; a changed model set uses a new tag.

The app needs an internet connection to download a model. Speech recognition itself runs locally after the download. Audio and transcripts are not uploaded.
