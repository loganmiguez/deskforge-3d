# DeskForge 3D — iPad PWA package

This package contains the current DeskForge 3D room-editor prototype packaged as an installable Progressive Web App (PWA).

## Publish it
Upload the *contents* of this folder to a static HTTPS host (for example, a GitHub Pages site, Netlify, or Cloudflare Pages). Upload all six files from this package into the repository root (the same level as index.html).

## Install on iPad
1. Open the published HTTPS address in Safari.
2. Tap Share.
3. Choose **Add to Home Screen**.
4. Enable **Open as Web App** if that option appears, then tap Add.

## Current capabilities
- Interactive Three.js room viewport with orbit/zoom/pan.
- Adjustable room dimensions.
- Desk, cabinet, chair, monitor, shelf, and custom-block primitives.
- Select, move, rotate, resize, duplicate, and delete.
- Grid snapping, back-wall placement, and basic stacking.
- Finish/color selection.
- Browser-local save plus JSON export/import.

## Current limitations
- Three.js is loaded from a CDN, so the first load and 3D engine still require internet access.
- This is an early editor prototype, not a production CAD application.
- AI photo-to-3D, detailed furniture assets, robust face-aware wall mounting, true edge-to-edge auto-snap, cloud sync, and full undo history are not implemented yet.
- The service worker caches the app shell, not the third-party Three.js CDN modules.

## Local testing
A PWA must be served from HTTPS (or localhost) for service-worker installation. Opening index.html directly from Files will not install it as a PWA.
