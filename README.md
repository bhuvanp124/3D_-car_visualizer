# 3D Car Visualizer

A browser-based car configurator built on Google's **`<model-viewer>`** web component — orbit,
inspect and customise a vehicle in real time. No build step, no framework: one HTML file.

## Features

- 🎨 **Paint** — live colour picker applied to the car body
- ✨ **Materials** — matte, glossy and metallic finishes
- 💡 **Lighting scenes** — neutral, sunset and city environments
- 🚗 **Body variants** — standard, spoiler and convertible models
- 🛞 **Wheel styles** — standard, racing and off-road
- 🪟 **Window tint** toggle
- 🪑 **Interior view** — swing the camera into the cabin
- 🥽 **VR mode** — enter AR/VR on supported devices

## Tech

**`<model-viewer>` 4.0.0** (loaded from Google's CDN) · vanilla HTML/CSS/JS · glTF (`.glb`) assets

Camera controls, environment lighting and AR come from `model-viewer`; the control panel wires
DOM inputs to model attributes and material properties.

## Running

Serve the folder over HTTP — `model-viewer` won't load `.glb` files from `file://`:

```bash
npx serve .
# then open work.html
```

`settings.json` configures the VS Code **Live Server** extension (port 5501) if you prefer that.

## ⚠️ Model assets not included

The `.glb` models (`ferrari.glb`, `ferrari-spoiler.glb`, `ferrari-open.glb`) are **not committed**
to this repo. Drop your own glTF models in alongside `work.html` using those filenames, or edit
the `src` and variant options to point at models you have.

---

Built by [Bhuvan Prakash](https://github.com/bhuvanp124)
