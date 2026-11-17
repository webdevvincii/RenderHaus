# RenderHaus - Agent Instructions

## Tech Stack & Architecture
- **Type**: Static multi-page website (HTML/CSS/JavaScript) for a video editing agency.
- **Pages**: `index.html`, `about-us.html`, `video.html`, `get-started.html`.
- **Styling**: Tailwind CSS loaded via CDN with custom inline configuration, plus `css/style.css`.
- **Animations & Effects**: Vanta.js / Three.js (`js/background.js`) for background effects, AOS (Animate On Scroll) for scroll animations.
- **Assets**: 
  - `Videos/` (portfolio/sample video files)
  - `Thumbnails/` (logo & portfolio images)
  - `PDF file/` (Terms of Service, etc.)

## Development & Preview
- No build system, bundler, or `package.json` required.
- **Local Preview**: Serve static files using any local HTTP server:
  ```bash
  python -m http.server 8080
  ```
  Or use VS Code Live Server (configured in `.vscode/launch.json` for port `8080`).

## Key Conventions & Gotchas
- All scripts are vanilla JavaScript located in `js/` (`script.js`, `video.js`, `youtube.js`, `contact-form.js`, `banner.js`, `background.js`).
- External CDNs are used for Tailwind, Three.js, Vanta.js, and AOS; internet connection or cached CDN assets are required for full styling and effects.
