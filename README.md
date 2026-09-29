# Asset icon repository

For live assets, add a square PNG (at least 128 × 128 pixels) at **`icons/<asset-reference>.png`**, where `<asset-reference>` is the full lowercase `arxasset1…` chain-wide reference. Open a pull request against this public repository; after merging into `main`, the configured HTTPS host serves the icon. Issuers register assets without selecting or uploading an icon. Clients use a default icon until the image exists. References are unique to an issuer and asset slug; do not use the slug, symbol, or wallet address as the filename. Do not add the reference as PNG metadata.

The supplied fallback artwork is `assets/asset-icons/default-asset-icon.png`; the Console and iOS app bundle copies so missing-image fallback also works when the icon host is unavailable.

The old `assets/asset-icons/catalog.json` and ten crypto test logos are retained as PNG historical artwork, not used for automatic lookup. The crypto shapes were adapted from [Simple Icons v15.21.0](https://github.com/simple-icons/simple-icons/tree/15.21.0/icons) (CC0); they do not imply issuer verification or affiliation. GitHub raw controls HTTP caching of this repository; clients recheck images in ten-minute windows. Host caching may delay a newly merged image beyond the next check.
