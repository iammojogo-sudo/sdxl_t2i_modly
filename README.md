# SDXL Text-to-Image — Modly Extension

Text-to-image generation using Stable Diffusion XL. Runs locally on your GPU with CPU offloading for 6GB+ cards.

Weights are ~7GB. You'll need around 6GB of VRAM with CPU offloading.

## Installation

1. Open Modly and go to the **Extensions** tab
2. Click **Install from GitHub** and paste this repo URL
3. Wait for setup to finish
4. Once installed, click **Download** on the Generate Image node to grab the model weights from HuggingFace

## Usage

1. Drag an **Image** node onto the canvas and point it at `fake_image.png`
2. Drag a **Generate Image** node onto the canvas and connect the Image node to it
3. Type your prompt in the **Prompt** field
4. Optionally enter a **Negative Prompt**
5. Adjust parameters as needed
6. Hit **Run**

## Parameters

| Parameter | Default | Notes |
|---|---|---|
| Prompt | — | What you want to generate |
| Negative Prompt | — | What to avoid in the image |
| Width | 1024 | 512–1280 |
| Height | 1024 | 512–1280 |
| Steps | 30 | Higher = slower but more detail |
| Guidance Scale | 7.0 | How closely it follows the prompt |
| Seed | 0 | 0 picks a random seed each run |
