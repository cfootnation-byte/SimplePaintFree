<p align="center">
  <img src="https://simplepaint.pages.dev/favicon.ico" width="80" />
</p>

<h1 align="center">SimplePaint</h1>

<p align="center">
  AI-Powered Illustration & Webtoon Assistant Tool
</p>

<p align="center">
  <img src="https://img.shields.io/badge/version-1.0.0-blue" alt="Version" />
  <img src="https://img.shields.io/badge/platform-Windows%2010%2B-0078D6?logo=windows" alt="Platform" />
  <img src="https://img.shields.io/badge/license-Proprietary-red" alt="License" />
  <img src="https://img.shields.io/badge/Qt-6.7-41CD52?logo=qt" alt="Qt" />
</p>

<p align="center">
  <a href="../README.md">한국어</a> | <b>English</b> | <a href="README_ja.md">日本語</a>
</p>

---

## Introduction

SimplePaint is an illustration & webtoon creation tool where AI automates everything from lineart to coloring and shading.
Use your own API keys (Gemini, Flux) to access AI features for free.

---

## AI Features

### 1. AI Shading

Automatically generates cel shading from lineart layers. Analyzes light direction and intensity to create natural shadows.

**How to use:**
1. Select lineart layer
2. Click [AI] → [Generate Shading] from top menu
3. Choose option: Hard Cel Shading / Soft Shading / 3-Tone Cel Shading
4. Click Generate button

### 2. AI Colorize

Automatically applies flat coloring to lineart. Maintain consistent colors by referencing character sheets.

**How to use:**
1. Select lineart layer
2. Select [AI] → [Generate Base Colors]
3. (Optional) Specify character sheet file
4. Execute auto coloring

### 3. Character Sheet Generation

Auto-generate turnaround character sheets from reference images. Provides 4 views: front, side, back, and closeup.

**How to use:**
1. Select [AI] → [Generate Character Sheet]
2. Upload reference image (front or 3/4 angle recommended)
3. Select views to generate (front/side/back/closeup)
4. Execute generation

### 4. AI Line Art

Generate lineart with new poses based on character sheets. Choose from clean lineart, natural pen lines, or sketch style.

**How to use:**
1. Load character sheet
2. Select [AI] → [Generate Line Art]
3. Enter desired pose prompt (e.g., "sitting pose")
4. Select lineart style
5. Execute generation

### 5. AI Segmentation

Automatically separates images into meaningful units, creating separate layers for each.

**How to use:**
1. Select layer to separate
2. Select [AI] → [Segmentation]
3. Enter elements to separate (e.g., "character, background, props")
4. Execute auto separation

### 6. Shading Color Swap

Convert grayscale shading to desired colors to create various atmospheres. This is an internal conversion (not AI), so no API key is needed.

**How to use:**
1. Select shading layer
2. Select [AI] → [Shading Color Swap]
3. Choose color to convert (color picker)
4. Click Apply button

---

## Interface & Basic Features

### Menu Bar

**File Menu**
- **Save Project (Ctrl+S):** Saves the current work as a project file. Layer structure is preserved.
- **Open Project (Ctrl+O):** Opens a saved project file.
- **Export Image (Ctrl+E):** Exports the current canvas as an image file (PNG, etc.).
- **Import Image to Layer:** Imports an external image file as a new layer.
- **Import PSD (Ctrl+Shift+O):** Imports a Photoshop PSD file with its layer structure intact.
- **Export as PSD (Ctrl+Shift+S):** Exports the current work as a PSD file.
- **Exit (Ctrl+Q):** Closes the application.

**Edit Menu**
- **Undo (Ctrl+Z):** Undoes the last action.
- **Redo (Ctrl+Y):** Redoes the previously undone action.
- **Free Transform (Ctrl+T):** Freely transforms the selected layer. Supports resizing, rotation, and repositioning.
- **Canvas Size:** Changes the canvas dimensions.
- **AI Variations:** Uses AI to generate variations of the current image.
- **Clear Layer:** Clears all content on the currently selected layer.

**View Menu**
- **Zoom In (Ctrl++):** Zooms into the canvas.
- **Zoom Out (Ctrl+-):** Zooms out of the canvas.
- **Reset Zoom (Ctrl+0):** Resets the canvas to the default zoom level (100%).
- **Show Grid:** Toggles the grid overlay on the canvas.

### Toolbar

- **Undo / Redo (Ctrl+Z / Ctrl+Y):** Undo or redo your actions.
- **Save / Load:** Save the current canvas as an image file or load an image file.
- **Color:** Select the drawing color. Four default colors are provided, and you can click to choose a custom color.
- **Eraser:** Toggle eraser mode on or off.
- **Clear:** Clears all content on the currently selected layer.
- **Brush Size:** Adjust the brush (pen/eraser) size.
- **Zoom:** Adjust the canvas zoom level.

### Layer System

**Layer Settings**
- **Blend Mode:** Select the layer blend mode from the dropdown at the top of the Layers panel. Supports 14 modes.
- **Opacity:** Adjust layer opacity between 0% and 100% using the slider.

**Layer Management**
- **+Layer:** Adds a new empty layer.
- **+Folder:** Adds a folder to group layers together.
- **Delete:** Deletes the selected layer or folder.
- **Up / Down:** Moves the selected layer one step up or down in the stack.
- **Show / Hide:** Hides or shows the selected layer.

**Advanced Features**
- **+Mask:** Adds a mask to the selected layer.
- **-Mask:** Removes the mask from the selected layer.
- **Edit Mask:** Enters mask editing mode. Use the eraser to mask areas. Click Edit Mask again to exit when done.
- **Clip:** Clips the selected layer to the layer below. The current layer will only be visible within the painted area of the layer below.

### Blend Modes (14 types)

| Group | Modes |
|-------|-------|
| Darken | Normal, Darken, Multiply, Color Burn, Linear Burn |
| Lighten | Lighten, Screen, Color Dodge, Add (Linear Dodge) |
| Contrast | Overlay, Soft Light, Hard Light |
| Difference | Difference, Exclusion |

---

## API Key Setup

SimplePaint Free uses your own API keys. The following API keys are required for AI features:

| API | Usage | Provider |
|-----|-------|----------|
| Flux (BFL) | Shading, colorize, line art generation | [Black Forest Labs](https://api.bfl.ml/) |
| Gemini (Google) | Character sheet generation, segmentation, color analysis | [Google AI Studio](https://aistudio.google.com/) |

Enter your keys in **Settings → API Settings** after launching the app.

---

## System Requirements

| | Minimum | Recommended |
|---|---------|-------------|
| OS | Windows 10 (64-bit) | Windows 11 (64-bit) |
| CPU | Intel i5 | Intel i7 |
| RAM | 8GB | 16GB+ |
| GPU | 2GB VRAM | 4GB VRAM (NVIDIA) |
| Storage | 5GB | 10GB |

---

## Installation

1. Download the latest installer from the [Releases](../../releases) page.
2. Run the downloaded installer file.
3. Follow the installation wizard to complete setup.
4. Launch SimplePaint and configure your API keys.

---

## Links

- [Official Website](https://simplepaint.pages.dev)
- [Documentation](https://simplepaint.pages.dev/docs)
- [Pro Version](https://simplepaint.pages.dev/pricing) — Server-based AI, no API key setup needed

---

## License

Copyright (c) 2026 SimplePaint. All rights reserved.

This software is proprietary.
Source code is not distributed; only installer-based usage is permitted.
Unauthorized copying, modification, and redistribution is prohibited.
