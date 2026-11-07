# BEAN YARD CAFÉ — Optimized Website

## What changed
- Converted the website's large JPG photography and logo assets to WebP.
- Resized oversized image assets and compressed the images.
- Updated the HTML to use WebP assets.
- Added image preloading for the hero image and asynchronous image decoding.
- Kept below-the-fold images lazy-loaded.
- Removed font-face declarations that pointed to font files missing from the supplied ZIP.
- Corrected the social icon filename casing so it resolves consistently on case-sensitive hosting.
- Added small accessibility and reduced-motion/performance refinements.
- Removed `.git` history and `node_modules` from the delivery ZIP to avoid shipping unnecessary files.

## Run locally
This is a static website. You can open `index.html` directly, or run a local server from this folder:

```bash
python -m http.server 8000
```

Then open `http://localhost:8000`.

## Rebuild Tailwind CSS (only if you edit `src/input.css`)
Install the development dependencies and build:

```bash
npm install
npm run build
```

## Notes
- Existing page content, section structure, navigation, and core visual identity have been preserved.
- The supplied archive did not include the custom font files referenced by the CSS. Those broken font requests were removed; system font fallbacks are now used.
- Performance scores depend on hosting, server response time, caching, and the user's network/device. No PageSpeed score is guaranteed by a local ZIP optimization alone.
