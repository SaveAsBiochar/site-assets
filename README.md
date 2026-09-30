# site-assets

Rendered media for the SaveAsBiochar public site, served through jsDelivr.

Copyright (c) 2026 SaveAsBiochar. All rights reserved. These files are
proprietary and are published here only so they can be delivered to visitors
of https://saveasbiochar.com through a content delivery network. No license is
granted. See [LICENSE](./LICENSE).

## Layout

- `journey/<tier>/frame_NNNN.avif` scroll-scrubbed frame sequences, one folder per breakpoint tier
- `journey/manifest.json` frame count, file naming and tier sizes; `journey/tracks.json` where each
  tagged object sits in every frame
- `models/` compressed GLB models used by the live 3D showcase, and their rendered stills

## Serving

Files are addressed by commit hash so every render has a permanent URL:

    https://cdn.jsdelivr.net/gh/SaveAsBiochar/site-assets@<commit>/<path>

Source files (`.blend`, textures, render scripts) live in the private
`SaveAsBiochar/site-3d` repository. Nothing in this repository is hand-made;
every file is produced by that pipeline.
