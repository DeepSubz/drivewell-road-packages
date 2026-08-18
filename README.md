# DriveWell road packages

Versioned OSM-derived posted-speed-limit packages for DriveWell Android.

`Tiles/manifest.json` maps each regional package to its geographic bounds,
file name, edge count, size, and SHA-256 checksum. The Android app downloads
the package whose bounds contain the current GPS coordinate and caches the
decompressed package locally for offline matching.

The source data is © OpenStreetMap contributors and is distributed under the
Open Database License (ODbL). Packages contain only roads with explicit OSM
`maxspeed` tags; missing limits are intentionally left unavailable.
