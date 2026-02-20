# Interface & Basic Features

<p align="center">
  <a href="INTERFACE.md">한국어</a> | <a href="INTERFACE_ja.md">日本語</a>
</p>

> [Back to Main README](README_en.md)

Learn about SimplePaint's layout, menus, toolbar, layer system, and blend modes.

---

## Table of Contents

1. [Interface Overview](#interface-overview)
2. [Menu Bar](#menu-bar-file--edit--view)
3. [Toolbar](#toolbar)
4. [Layer System](#layer-system)
5. [Blend Modes](#blend-modes-14-types)

---

## Interface Overview

Learn about the layout of SimplePaint.

- **Menu Bar (File / Edit / View):** Contains menus for file save/load, editing, and view options.
- **Toolbar:** The top bar for quick access to frequently used features. Includes Undo/Redo, Save/Load, Color, Eraser, Clear, Brush Size, and Zoom.
- **Tools Panel:** Located on the left. Select between Pen and Eraser tools.
- **Canvas:** The central workspace where all drawing and editing takes place.
- **Layers / AI Panel:** Located on the right. Switch between layer management and AI features using the [Layers] / [AI Features] tabs at the bottom.

---

## Menu Bar (File / Edit / View)

Description of each item in the top menu bar.

### File Menu

| Item | Shortcut | Description |
|------|----------|-------------|
| Save Project | Ctrl+S | Saves the current work as a project file. Layer structure is preserved. |
| Open Project | Ctrl+O | Opens a saved project file. |
| Export Image | Ctrl+E | Exports the current canvas as an image file (PNG, etc.). |
| Import Image to Layer | — | Imports an external image file as a new layer. |
| Import PSD | Ctrl+Shift+O | Imports a Photoshop PSD file with its layer structure intact. |
| Export as PSD | Ctrl+Shift+S | Exports the current work as a PSD file. Layers are preserved for use in other editors. |
| Exit | Ctrl+Q | Closes the application. |

### Edit Menu

| Item | Shortcut | Description |
|------|----------|-------------|
| Undo | Ctrl+Z | Undoes the last action. |
| Redo | Ctrl+Y | Redoes the previously undone action. |
| Free Transform | Ctrl+T | Freely transforms the selected layer. Supports resizing, rotation, and repositioning. |
| Canvas Size | — | Changes the canvas dimensions. |
| AI Variations | — | Uses AI to generate variations of the current image. |
| Clear Layer | — | Clears all content on the currently selected layer. |

### View Menu

| Item | Shortcut | Description |
|------|----------|-------------|
| Zoom In | Ctrl++ | Zooms into the canvas. |
| Zoom Out | Ctrl+- | Zooms out of the canvas. |
| Reset Zoom | Ctrl+0 | Resets the canvas to the default zoom level (100%). |
| Show Grid | — | Toggles the grid overlay on the canvas. |

---

## Toolbar

Description of each function in the top toolbar.

| Tool | Shortcut | Description |
|------|----------|-------------|
| Undo / Redo | Ctrl+Z / Ctrl+Y | Undo or redo your actions. |
| Save / Load | — | Save the current canvas as an image file (PNG, etc.) or load an image file. |
| Color | — | Select the drawing color. Four default colors (black, red, green, blue) are provided, and you can click to choose a custom color. |
| Eraser | — | Toggle eraser mode on or off. Same function as the Eraser in the Tools panel. |
| Clear | — | Clears all content on the currently selected layer. |
| Brush Size | — | Adjust the brush (pen/eraser) size. Change via number input or +/- buttons. |
| Zoom | — | Adjust the canvas zoom level. Use -/+ buttons to control, with the current magnification shown as a percentage. |

---

## Layer System

Description of each feature in the Layers panel.

### Layer Settings

- **Blend Mode:** Select the layer blend mode from the dropdown at the top of the Layers panel. Supports 14 modes including Normal, Multiply, Screen, etc.
- **Opacity:** Adjust layer opacity between 0% and 100% using the slider.

### Layer Management

| Feature | Description |
|---------|-------------|
| +Layer | Adds a new empty layer. |
| +Folder | Adds a folder to group layers together. |
| Delete | Deletes the selected layer or folder. |
| Up / Down | Moves the selected layer one step up or down in the stack. |
| Show / Hide | Hides or shows the selected layer. |

### Advanced Features

| Feature | Description |
|---------|-------------|
| +Mask | Adds a mask to the selected layer. |
| -Mask | Removes the mask from the selected layer. |
| Edit Mask | Enters mask editing mode. Use the eraser to mask areas. Click Edit Mask again to exit when done. |
| Clip | Clips the selected layer to the layer below. The current layer will only be visible within the painted area of the layer below. |

---

## Blend Modes (14 types)

| Group | Modes |
|-------|-------|
| Darken | Normal, Darken, Multiply, Color Burn, Linear Burn |
| Lighten | Lighten, Screen, Color Dodge, Add (Linear Dodge) |
| Contrast | Overlay, Soft Light, Hard Light |
| Difference | Difference, Exclusion |
