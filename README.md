# Asset icon repository

For live Console assets, add an SVG at **`icons/<asset-reference>.svg`**, where `<asset-reference>` is the full lowercase `arxasset1…` chain-wide reference. Open a pull request against this public repository; after merging into `main`, the configured HTTPS host serves the icon. Issuers register assets without selecting or uploading an icon. The Console uses a default icon until the image exists. References are unique to an issuer and asset slug; do not use the slug, symbol, or wallet address as the filename.

The supplied fallback artwork is `assets/asset-icons/default-asset-icon.svg`; the Console embeds its vector so missing-image fallback also works offline.

The old `assets/asset-icons/catalog.json` and ten crypto test logos are retained as historical artwork, not used for automatic lookup. The crypto shapes were adapted from [Simple Icons v15.21.0](https://github.com/simple-icons/simple-icons/tree/15.21.0/icons) (CC0); they do not imply issuer verification or affiliation.
