# AYVRO road packages

Versioned OSM-derived posted-speed-limit packages for AYVRO Android.

`Tiles/manifest.json` maps each regional package to its geographic bounds,
file name, size, and SHA-256 checksum. The Android app downloads
the package whose bounds contain the current GPS coordinate and caches the
decompressed package locally for offline matching.

The first metro-city package rollout has been retired. Texas is the current
pilot region. The current extract contains 32 spatial packages generated from
the Geofabrik Texas OSM extract on 2026-08-21. Each package is compact JSON
compressed with gzip (approximately 1.2–1.5 MB) and the manifest carries its
geographic bounds and SHA-256 checksum. The Android client selects tiles from
GPS coordinates and does not use a manual region selector.

Source extract SHA-256: `35e0a5f239b758aa136009ef3c72dd4259931d9767bdcf4188e354d8ebcd9f67`.

The source data is © OpenStreetMap contributors and is distributed under the
Open Database License (ODbL). Packages contain drivable roads and available
speed-limit attributes; missing limits are intentionally left unavailable.
