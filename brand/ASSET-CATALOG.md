# Media asset catalog

## Banners and product art

| File | Size | Intended use |
|---|---:|---|
| `github-social-preview-1280x640.jpg` | 1280×640 | GitHub repository social preview |
| `patreon-cover-2500x1000.jpg` | 2500×1000 | Patreon wide cover with safe-zone branding and real UI |
| `patreon-product-984x554.jpg` | 984×554 | Patreon digital product landscape image |
| `kofi-cover-1200x400.jpg` | 1200×400 | Ko-fi 3:1 page cover |
| `kofi-product-1080x1080.jpg` | 1080×1080 | Ko-fi Shop/product/social square |
| `omnigpu-feature-collage-1600x900.jpg` | 1600×900 | README, posts and press overview |

## Screenshots

- `omnigpu-1.0.0-home.jpg`
- `omnigpu-1.0.0-drivers.jpg`
- `omnigpu-1.0.0-profile-inspector.jpg`
- `omnigpu-1.0.0-driver-reset.jpg`
- `omnigpu-1.0.0-performance-tuning.jpg`
- `omnigpu-1.0.0-monitoring.jpg`
- `omnigpu-1.0.0-displays-hdr.jpg`
- `omnigpu-1.0.0-settings.jpg`
- `omnigpu-1.0.0-setup.jpg`

The application captures are real 1440×900 frames from the rebuilt 1.0.0 executable on 2026-08-19. The Setup capture is a real 622×412 frame from the matching bootstrapper. Hardware-specific data is visible only where it explains the product and no local filesystem path appears in the published captures.

## Icons

- `omnigpu-icon-master.png`: 1254×1254 transparent high-resolution application/installer icon derived directly from the exact user-approved final full-tile artwork, with a clean dark defringed perimeter.
- `omnigpu-symbol.png`: 1254×1254 transparent standalone GPU/fan mark for compact in-product branding.
- `omnigpu.ico`: halo-safe multi-resolution Windows icon container with 16, 20, 24, 32, 40, 48, 64, 96, 128 and 256 px frames for private packaging/reference; it is artwork, not an executable.
- `omnigpu-setup-icon-master.png`: tightly framed transparent Setup/MSI master with a 2–3% antialiased safety margin and no heavy black outer band.
- `omnigpu-setup.ico`: matching 10-frame Windows icon container used by the private Setup/MSI packaging.

## Export rules

- Keep GitHub social preview below 1 MB.
- Keep Patreon cover below the current platform limit and confirm crop in the live editor.
- Keep Ko-fi cover below 8 MB and use a static JPEG/PNG.
- Do not recompress screenshots until text becomes soft.
- Preserve dark RGB in transparent/antialiased icon-edge samples so Windows downscaling cannot introduce a pale matte.
- Preserve the approved master icons and regenerate platform derivatives through `distribution/media-source` when screenshots change.
