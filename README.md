# Shader Study 01 — Fractal Bloom

## Live Demo

[Open the real-time WebGL shader](https://wuyian95.github.io/shader-portfolio/)

A single-file WebGL portfolio page. The fragment shader uses a Shadertoy-style `mainImage` entry point with `iResolution` and `iTime` uniforms. No build step or external libraries are required.

## Run locally

Open `index.html` in a modern browser, or serve this folder with any static HTTP server.

## Publish with GitHub Pages

1. Create a GitHub repository and upload the **contents** of this folder to its `main` branch.
2. In the repository, open **Settings → Pages** and set the build/deployment source to **GitHub Actions**.
3. The included workflow deploys the site on each push to `main`. The published URL appears in the workflow run and the Pages settings.

The pasted ShaderToy text contained formatting artifacts and two missing multiplication operators. The shader in `index.html` removes those artifacts and uses `length(uv) * exp(...)` and `i * 2.0`.
