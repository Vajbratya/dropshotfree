# Dropshot Free

Free, open-source device mockup & screen recording tool. Zero-install, single HTML file, runs entirely in the browser. No signup, no watermark, no upload — everything stays on your machine.

**Live**: open `index.html` in Chrome/Edge/Safari.

## Features

### Devices
- iPhone 17 Pro (Natural / Black / White / Desert Titanium)
- iPhone 17 Pro Max, iPhone 17
- iPad Pro 13"
- MacBook Pro 14"
- Pixel 9 Pro
- No-frame mode

### Content sources
- Image upload / drag-drop / paste (`⌘V`)
- Video upload (MP4, WebM) — auto-loop
- Live screen capture (`getDisplayMedia`)

### Backgrounds
- Linear gradient, radial gradient, solid color
- Mesh gradient (animated noise)
- Grainy noise, blurred content, transparent
- 15 built-in presets (Midnight, Sunset, Ocean, Cyberpunk, etc.)
- Custom color pickers + angle control

### Motion (10 types)
Float · Sway · Tilt · Orbit · Pulse · Spin · Wobble · Drift · Bounce · Heartbeat

### Post-processing (14 effects)
Specular Glide · Dynamic Lighting · Glass Glare · Chromatic Shift · Noir · Heat Ripple · Glitch · Vignette · Film Grain · Bloom · Scanlines · Sepia · Saturate · Gaussian Blur · Pixelate · CRT Curvature · Invert

### Shadow styles
Soft · Hard · Glow (hue-colored) · Neon · Floor Reflection

### Scene presets
Product Hunt · Social Story · Studio Clean · Instagram Post · Dramatic · Retro Wave · Film Grain · Minimal

### Export
- WebM / MP4 recording (MediaRecorder)
- 30 / 60 FPS · 4–24 Mbps bitrate
- Duration limit (0 = unlimited)
- PNG snapshot at 1x / 2x / 3x / 4x
- Transparent PNG export
- Copy frame to clipboard

### UI
- Aspect ratios: 9:16, 16:9, 1:1, 4:5, 3:4, 21:9
- Padding, scale, rotation, flip H/V, position X/Y
- Screen corner radius, fit mode, zoom
- Keyboard shortcuts (`?` for help)

## Keyboard shortcuts
| Action | Key |
|---|---|
| Record / stop | `R` |
| Snapshot PNG | `S` |
| Copy frame | `⌘C` |
| Paste image | `⌘V` |
| Open media | `O` |
| Live capture | `L` |
| Reset scene | `⌘0` |
| Toggle panel | `P` |
| Help | `?` |

## Tech

- WebGL2 two-pass pipeline (scene FBO → post-FX → canvas)
- `MediaRecorder` + `canvas.captureStream()` for video export
- No dependencies, no build step, ~1700 LoC single file

## License

MIT
