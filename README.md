# Asset icon catalog

The source of approved Console asset icons is `assets/asset-icons/`. Each `catalog.json` entry has an immutable `id`, a display `name`, an optional `symbol`, and a relative `file`. IDs must never be reused for a different icon. To retire an icon, remove its entry; existing assets will display the Console's default icon.

Maintainers add a PNG, JPEG, WebP, or static SVG file and its entry here, then run `npm run sync:asset-icons` from the sibling `Arxium-Console` checkout. Commit the generated `public/asset-icons/` files in the Console repository and deploy the Console. The Console build checks every entry and file. Users cannot upload icons through the Console. The repository is private; clients load only the deployed Console static assets, not GitHub.
