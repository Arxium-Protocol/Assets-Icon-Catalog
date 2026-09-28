# Asset icon repository

For live Console assets, add an SVG at **`icons/<asset-reference>.svg`**, where `<asset-reference>` is the full lowercase `arxasset1…` chain-wide reference. Open a pull request against this public repository; after merging into `main`, the configured HTTPS host serves the icon. Issuers register assets without selecting or uploading an icon. The Console uses a default icon until the image exists. References are unique to an issuer and asset slug; do not use the slug, symbol, or wallet address as the filename.

The following `assets/asset-icons/` catalog is kept as historical test artwork; it is not used for automatic asset icon lookup.

The source of approved Console asset icons is `assets/asset-icons/`. Each `catalog.json` entry has an immutable `id`, a display `name`, an optional `symbol`, and a relative `file`. IDs must never be reused for a different icon. To retire an icon, remove its entry; existing assets will display the Console's default icon.

Maintainers add a PNG, JPEG, WebP, or static SVG file and its entry here, then publish the changes to the public repository's `main` branch. The Console fetches the catalog from the Git-backed jsDelivr HTTPS endpoint, validates its IDs, names, and supported file paths, and loads images from the same endpoint. The Console refreshes its server-side catalog cache after one minute; CDN caching can delay updates. No Console commit or redeploy is needed. Users cannot upload icons through the Console.

The ten crypto logos are test icons adapted from [Simple Icons v15.21.0](https://github.com/simple-icons/simple-icons/tree/15.21.0/icons) (CC0). They are illustrative choices, not issuer verification or an affiliation claim. The former `asset-*` placeholder IDs were retired; assets using those IDs fall back to the default glyph.
