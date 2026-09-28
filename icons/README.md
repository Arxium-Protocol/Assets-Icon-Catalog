# Asset-reference icons

Add `<asset-reference>.svg` here after registering an asset, for example:

`icons/arxasset1z8d4jt8yt0xtjm6lvk8umc9relegrwq4xu928eqxyjfcsnjuex6qe873qa.svg`

The reference is the complete lowercase `arxasset1…` value returned by the chain. Keep files self-contained static SVGs; do not use remote images, scripts, or private URLs. Once the pull request is merged and the public CDN serves the file, existing asset views pick it up after their missing-icon cache expires or the page is refreshed.
