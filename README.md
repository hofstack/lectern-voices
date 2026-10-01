# lectern-voices

Voice packs that [Lectern](https://github.com/hofstack/lectern) downloads on request. Each pack is published as a GitHub release asset. The app pins every asset by SHA-256 and byte size, so a release asset is never replaced in place. A changed pack gets a new tag.

## Supertonic

The Supertonic packs contain model weights by Supertone Inc. (Supertonic, https://github.com/supertone-oss-archive/supertonic). The weights are licensed under the **BigScience Open RAIL-M License**, and every pack carries the full licence text (`LICENSE`) and a `NOTICE`.

The use restrictions in Attachment A of that licence apply to anyone who uses these packs. Read them before you use them.

These files are derivatives of the upstream weights:

- int8 quantisation done with the sherpa-onnx project's own scripts.
- For the English (v1) pack, a graph patch that removes the language-tag tokens sherpa-onnx adds before synthesis. The weights are unchanged.

The build is reproducible with `tools/supertonic-pack` in the Lectern repository.

Copyright (c) Supertone Inc. for the model weights. "Supertonic" names the upstream model and implies no endorsement.
