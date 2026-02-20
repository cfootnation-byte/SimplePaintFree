# AI Features Guide

<p align="center">
  <a href="AI_FEATURES.md">한국어</a> | <a href="AI_FEATURES_ja.md">日本語</a>
</p>

> [Back to Main README](README_en.md)

---

## Table of Contents

1. [AI Shading](#1-ai-shading)
2. [AI Colorize](#2-ai-colorize)
3. [Character Sheet Generation](#3-character-sheet-generation)
4. [AI Line Art](#4-ai-line-art)
5. [AI Segmentation](#5-ai-segmentation)

---

## 1. AI Shading

AI automatically generates shading for lineart images. Choose from 4 variation candidates, and the shading layer is added automatically.

> Credits: 0.0825 credits / use

### How to use

**Step 1.** Prepare lineart on canvas, then click the Shading button in the AI Features panel.

![Step 1](../media/shading-step1.png)

**Step 2.** Select area — Drag to select the area to apply shading. Shift+drag for multiple area selection, ESC to cancel.

![Step 2](../media/shading-step2.png)

**Step 3.** Select shading style — Choose your preferred shading style. Skip (AI auto-select) is also available.

![Step 3](../media/shading-step3.png)

**Step 4.** AI generates 4 variation candidates. Click the variation you prefer to select it.

![Step 4](../media/shading-step4.png)

**Step 5.** The selected shading is automatically added as a Shading (AI) layer, placed below the lineart.

![Step 5](../media/shading-step5.png)

### Extra: Shading Color Swap

After generating shading, use the Shading Color Swap button to convert grayscale shading to your desired colors. Select the shading layer, then specify the target color to create various atmospheres. This is an image processing feature, not AI-powered.

---

## 2. AI Colorize

AI automatically applies flat coloring to lineart. Reference character sheets for consistent colors, and choose from 4 variation candidates.

> Credits: 0.0825 credits / use

### How to use

**Step 1.** Prepare lineart on canvas, then click the Colorize button in the AI Features panel.

![Step 1](../media/colorize-step1.png)

**Step 2.** Select area — Drag to select the area to apply base colors. ESC to cancel.

![Step 2](../media/colorize-step2.png)

**Step 3.** Select character sheet — Choose a character sheet for color reference. Multi-select with Ctrl+click, load from file, or select no reference.

![Step 3](../media/colorize-step3.png)

**Step 4.** AI generates 4 variation candidates. Click the variation you prefer to select it.

![Step 4](../media/colorize-step4.png)

**Step 5.** The selected base colors are automatically added as a Colorize (AI) layer, placed between the lineart and shading layers.

![Step 5](../media/colorize-step5.png)

> **Tip:** When referencing a character sheet, it is better not to enter separate color instructions for more natural results.

---

## 3. Character Sheet Generation

Automatically generates a 4-direction turnaround character sheet (front, side, back, 3/4 view) using AI from canvas artwork or external images.

> Credits: 0.264 credits / use

### How to use

**Step 1.** Click the Character Sheet button in the AI Features panel.

![Step 1](../media/character-step1.png)

**Step 2.** Select style — Rich Sheet (Flux): high-quality sheet with rich details / Flat Color Sheet (Gemini): simple flat color-based sheet

![Step 2](../media/character-step2.png)

**Step 3.** Select reference image — Select area from canvas or load from file

![Step 3](../media/character-step3.png)

**Step 4.** Enter a character name.

![Step 4](../media/character-step4.png)

**Step 5.** AI automatically generates 4 directional views (front, side, back, 3/4 view).

![Step 5](../media/character-step5.png)

**Step 6.** Generated sheets are saved in the Character Sheet List and can be viewed anytime by clicking. Unwanted sheets can be removed with Delete Selected Sheet.

---

## 4. AI Line Art

Automatically generates lineart for desired poses and scenes using AI with character sheet reference. Choose from 4 variation candidates.

> Credits: 0.0825 credits / use

### How to use

**Step 1.** Click the Line Art button in the AI Features panel.

![Step 1](../media/lineart-step1.png)

**Step 2.** Select character sheet — Choose a character sheet to reference. Multi-select with Ctrl+click, load from file, or select no reference.

![Step 2](../media/lineart-step2.png)

**Step 3.** Describe pose/scene — Describe the pose or scene to generate in text. (e.g., running pose, sitting and reading a book, waving hand)

![Step 3](../media/lineart-step3.png)

**Step 4.** Select lineart style — Choose your preferred lineart style. Skip (AI auto-select) is also available.

![Step 4](../media/lineart-step4.png)

**Step 5.** Select output ratio — Choose the output image ratio. (1:1 square, etc.)

![Step 5](../media/lineart-step5.png)

**Step 6.** AI generates 4 variation candidates. Click the variation you prefer to select it.

![Step 6](../media/lineart-step6.png)

**Step 7.** Add layer confirmation — Choose whether to add the generated lineart as a new layer.

![Step 7](../media/lineart-step7.png)

**Step 8.** The selected lineart is added to the canvas as a new layer.

![Step 8](../media/lineart-step8.png)

---

## 5. AI Segmentation

Automatically separates images into meaningful units (character, background, etc.) and creates separate layers for each. Lineart, base color, and shading layers can all be separated at once.

### How to use

**Step 1.** Click the Segmentation button in the AI Features panel.

![Step 1](../media/segment-step1.png)

**Step 2.** Enter elements — Type the elements you want to separate. (e.g., character, book, bench, background)

![Step 2](../media/segment-step2.png)

**Step 3.** Preview and layer selection — A segmentation preview is displayed, and you can multi-select layers to separate. (e.g., Background, Lineart, Colorize, Shading) Choose Execute or Save.

![Step 3](../media/segment-step3.png)

**Step 4.** The selected layers are separated by region and added as individual layers. (e.g., Lineart (AI) - Region 1/2/3, Colorize (AI) - Region 1/2/3, Shading (AI) - Region 1/2/3)
