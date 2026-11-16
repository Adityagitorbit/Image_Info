# Metadata Viewer

A single-page website that shows all the metadata inside an image or video you upload, with a plain-English summary and an AI-generated check.

## Features
- File details, image/video properties, SHA-256 checksum
- EXIF, GPS, XMP, IPTC, ICC, JFIF, PNG header data (via [exifr](https://github.com/MikeKovarik/exifr))
- Summary: date, time, location, device (mobile phone or camera) and an AI-generated label
- Filter tags, copy or download everything as JSON
- 100% client-side: files never leave your browser

## Run locally
Open `index.html` in any modern browser (double-click it). An internet connection is needed once to load the exifr library from a CDN.

## Deploy with GitHub Pages
Repo **Settings → Pages → Deploy from a branch → main / (root)**. Your site will be at `https://<username>.github.io/<repo>/`.

## Note on the AI check
The AI label only looks for markers in metadata (IPTC source type, generator names, C2PA). Metadata can be stripped or faked, so treat it as a clue, not proof.
