# Asset icon catalog

The source of approved Console asset icons is `assets/asset-icons/`. Each `catalog.json` entry has an immutable `id`, a display `name`, an optional `symbol`, and a relative `file`. IDs must never be reused for a different icon. To retire an icon, remove its entry; existing assets will display the Console's default icon.

Maintainers add a PNG, JPEG, WebP, or static SVG file and its entry here, then publish the changes to the public repository's `main` branch. The Console fetches the catalog from the Git-backed jsDelivr HTTPS endpoint, validates its IDs, names, and supported file paths, and loads images from the same endpoint. The Console refreshes its server-side catalog cache after one minute; CDN caching can delay updates. No Console commit or redeploy is needed. Users cannot upload icons through the Console.
