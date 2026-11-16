# Changelog

## 1.3.0

- Reasoning with item IDs or encrypted content and assistant item IDs are replayed; `content` tool outputs become `input_text`/`input_image` arrays; image detail is honoured; warning texts and media metadata match upstream; function tools send only their input schema; `maxImagesPerCall` is 3.
  Compatibility: Source-compatible; changes are additive. Request bodies, results, warnings and errors change to match the reviewed upstream package.
